# Comparing `tmp/wbx_cpl-1.2.2.tar.gz` & `tmp/wbx_cpl-1.3.1.tar.gz`

## Comparing `wbx_cpl-1.2.2.tar` & `wbx_cpl-1.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/src/wbx_cpl/__init__.py
--rw-r--r--   0        0        0    16960 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/src/wbx_cpl/__main__.py
--rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/src/wbx_cpl/dataframe.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/src/wbx_cpl/utils.py
--rw-r--r--   0        0        0    12817 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/src/wbx_cpl/wbx.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/LICENSE
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 wbx_cpl-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/src/wbx_cpl/__init__.py
+-rw-r--r--   0        0        0    17724 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/src/wbx_cpl/__main__.py
+-rw-r--r--   0        0        0    14118 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/src/wbx_cpl/dataframe.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/src/wbx_cpl/utils.py
+-rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/src/wbx_cpl/wbx.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 wbx_cpl-1.3.1/PKG-INFO
```

### Comparing `wbx_cpl-1.2.2/src/wbx_cpl/__main__.py` & `wbx_cpl-1.3.1/src/wbx_cpl/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from datetime import timezone
 import importlib.metadata
 import inspect
 import sys
 
 import click
 from pprint import pprint
-import pandas
+import pandas as pd
 
 import wbx_cpl.utils as utils 
 import wbx_cpl.dataframe as wbxdf
 import wbx_cpl.wbx
 
 ut=wbx_cpl.utils.UtilsTrc()
 wbxr=wbx_cpl.wbx.WbxRequest()
@@ -107,15 +107,14 @@
         ut.trace(2, f"{csvdest} written.")
 
 
 # pull membership info in csv fmt  
 # 
 def print_memberships(members, csvFile):
     #
-    cols = {'personEmail':[],'personDisplayName':[],'created':[]}
     df=wbxdf.membershipDF()
     df=df.add_data(members)
     print(df.loc[:, ~df.columns.isin(['id','files', 'roomId'])])
     csvFile and df.to_csv(csvFile, index=False)
 
 
 #####################
@@ -224,14 +223,37 @@
 @click.argument('spaceId') 
 @click.option('-c', '--csvfile', help='Save results to CSV file.')
 def space_members(spaceid, csvfile):
     """List emails of members in given space ID."""
     data = wbxr.get_space_memberships(spaceid)
     print_memberships(data, csvfile)
 
+# get list of spaces for given user email 
+# 
+@click.command()
+@click.argument('email') 
+@click.option('-c', '--csvfile', help='Save results to CSV file.')
+def user_spaces(email, csvfile):
+    """List spaces joined by given user email """
+    df = wbxdf.spacesMembershipDF(email)
+    df.print(csvfile)
+
+@click.command()
+@click.argument('users_export') 
+@click.option('-c', '--csvfile', help='Save results to CSV file.')
+def spaces_count(users_export, csvfile):
+    """Search all spaces joined by users listed in csv export file.  """
+    spaces_DB={}
+    iscsv = re.match('.*\.csv$', users_export, re.IGNORECASE)
+    if (iscsv):
+        df = wbxdf.spacesCountDF(users_export)
+        df.print(csvfile)
+    else:
+        print ("I need a .CSV input file")
+
 # download files in given msg id   
 #
 @click.command()
 @click.argument('msgId') 
 @click.option('-d', '--dir', default="", help='directory name to downlaad to.')
 def message_files(msgid, dir):
     """Download files attached to given message ID. Files will be downloaded in current directoty by default."""
@@ -247,15 +269,17 @@
 @click.group()
 def messaging():
     pass
 
 messaging.add_command(message_files)
 messaging.add_command(space_messages) 
 messaging.add_command(user_messages) 
+messaging.add_command(user_spaces) 
 messaging.add_command(space_members) 
+messaging.add_command(spaces_count)
 
 
 #####################
 ### Recording     ###
 #####################
 
 @click.group()
@@ -328,15 +352,15 @@
 @click.option('-d', '--dir', default="", help='directory destination for downlaads.')
 @click.argument('id_or_csv') 
 def get_recording_media(id_or_csv, dir):
     """downloads media of given recording ID or list of IDs in .CSV file (in the 'id' column). """
     iscsv = re.match('.*\.csv$', id_or_csv, re.IGNORECASE)
     if (iscsv):
         try:
-            df = pandas.read_csv(id_or_csv)
+            df = pd.read_csv(id_or_csv)
             # print(df)
             for id in df['id']:
                 print(f"Processing recording {id}...")
                 data = wbxr.get_wbx_data(f"recordings/{id}")
                 if ( data ) :
                     rdl=data['temporaryDirectDownloadLinks']['recordingDownloadLink']
                     wbxr.download_contents(rdl, dir, f"recording-{id}-{data['hostEmail']}-{data['createTime']}.{data['format']}")
```

### Comparing `wbx_cpl-1.2.2/src/wbx_cpl/dataframe.py` & `wbx_cpl-1.3.1/src/wbx_cpl/dataframe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd 
 pd.set_option('display.max_colwidth', 80)
 import wbx_cpl.utils 
 from wbx_cpl.wbx import WbxRequest as Wbxr
 import json as json
+import re
 
 ut=wbx_cpl.utils.UtilsTrc()
 wbxr=Wbxr()
 
 # populates df with data obj based cols list of fields
 #
 def update_df_data(df,  data, cols):    
@@ -180,14 +181,92 @@
                     if f in mbr:
                         new_row[f]=mbr[f]
                 self.df = pd.concat([self.df, pd.DataFrame([new_row])], ignore_index=True)
         else:
             ut.trace(3, f"no membership data")
         # return DF
         return(self.df)
+    
+class spacesMembershipDF:
+
+    cols = {'roomId':[], 'created':[], 'roomType':[]}
+
+    def __init__(self, email):
+        mycols=self.cols
+        self.df = pd.DataFrame(mycols)
+        self.spaces = wbxr.get_user_spaces(email)
+        self.add_data()
+        self.user_email=email
+        
+    def add_data(self):
+        #
+        if 'items' in self.spaces:
+            for spc in self.spaces['items']:
+                new_row={}
+                for f in self.cols:
+                    if f in spc:
+                        new_row[f]=spc[f]
+                self.df = pd.concat([self.df, pd.DataFrame([new_row])], ignore_index=True)
+        else:
+            ut.trace(3, f"no membership data for {self.user_email}")
+
+    def print(self, csvfile):
+        print(self.df)
+        csvfile and self.df.to_csv(csvfile, index=False)
+
+class spacesCountDF:
+
+    cols = {'id':[], 'title':[], 'type':[]}
+
+    def __init__(self, users_csv_file):
+        mycols=self.cols
+        self.df = pd.DataFrame(mycols)
+        self.add_data(users_csv_file)
+        
+    def add_data(self, users_csv_file):
+        self.spaces_DB={}
+        try:
+            usesrsdf = pd.read_csv(users_csv_file)
+            for email in usesrsdf['User ID/Email (Required)']:
+                print(f"Processing user {email}...")
+                spaces = wbxr.get_user_spaces(email)
+                if (spaces) :
+                    if 'items' in spaces:
+                        for spc in spaces['items']:
+                            id = spc['roomId']
+                            print(f"space id {id}", end=' ')
+                            if ( id in self.spaces_DB ):
+                                print(f"Already exists")
+                                self.spaces_DB[id]['count'] = self.spaces_DB[id]['count'] + 1
+                            else:
+                                print(f"Adding space data")
+                                space_details = wbxr.get_wbx_data(f"rooms/{id}")
+                                if (space_details): 
+                                    if space_details['type'] == 'group':
+                                        self.spaces_DB[id] = {}
+                                        self.spaces_DB[id]['count'] = 1
+                                        self.spaces_DB[id]['details'] = space_details
+                    else:
+                        ut.trace(3, f"{email} has no membership data")
+            # build DF 
+            for id in self.spaces_DB:
+                new_row={}
+                new_row['count']=self.spaces_DB[id]['count']
+                for f in self.cols:
+                    if f in self.spaces_DB[id]['details']:
+                        new_row[f]=self.spaces_DB[id]['details'][f]
+                self.df = pd.concat([self.df, pd.DataFrame([new_row])], ignore_index=True)
+
+        except FileNotFoundError:
+            ut.trace(1, f"Error: File '{users_csv_file}' not found.")
+
+    def print(self, csvfile):
+        print(self.df.loc[:, ~self.df.columns.isin([])])
+        csvfile and self.df.to_csv(csvfile, index=False)
+
 
 class meetingDF:
 
     cols = {'email':[],'displayName':[],'host':[]}
 
     def __init__(self, meetingId):
         mycols=self.cols
@@ -225,14 +304,15 @@
                 emails.append(part['email'])
         return(emails)
     
     def add_details(self) :
         self.details=wbxr.get_wbx_data(f"meetings/{self.meetingId}")
  
 
+
 class meetingsDF:
 
     datafile="meeting_list.json"
     cols = {'meetingId':[], 'title':[], 'created':[],}
 
     def __init__(self):
         mycols=self.cols
```

### Comparing `wbx_cpl-1.2.2/src/wbx_cpl/utils.py` & `wbx_cpl-1.3.1/src/wbx_cpl/utils.py`

 * *Files identical despite different names*

### Comparing `wbx_cpl-1.2.2/src/wbx_cpl/wbx.py` & `wbx_cpl-1.3.1/src/wbx_cpl/wbx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import wbx_cpl.utils as utils
 import datetime 
 from datetime import timezone
 import requests
 import json
 import re
+import urllib.parse
 
 ut=utils.UtilsTrc()
 
 # move this to wbx.py
 now = datetime.datetime.now(timezone.utc)
 nowiso = now.isoformat(timespec='milliseconds')
 UTCNOW = re.sub('\+.+','', nowiso) + 'Z' # remove the tz suffix 
@@ -34,14 +35,15 @@
         name=re.findall('filename="(.+)"', cd)[0]
         return(name)
 
     # generic get data 
     # returns {} if not happy  
     #
     def get_wbx_data(self, ep, params="", ignore_error=False):
+        params = urllib.parse.quote(params, safe='/=?')
         url = "https://webexapis.com/v1/" + ep + params
         ut.trace(3, f"{url} ")
         hdr=self.setHeaders()
         try:
             r = requests.get(url, headers=hdr)
             s = r.status_code
             if (s == 200):
@@ -52,69 +54,46 @@
                 not ignore_error and ut.trace(1,f"error {url} {s}: {r.reason}")  
                 return({})
         except requests.exceptions.RequestException as e:
             ut.trace(1, f"error {e}")
 
 
     # returns user data json 
-    # returns "" if not found or some error   
     #
     def get_user_details(self, email_or_uid): 
         ut.trace (3, f"processing user {email_or_uid}")  
 
         if ( utils.is_email_format(email_or_uid)):
             uid = self.get_user_id(email_or_uid)
             if (uid=="") :
-                return ""
+                return {}
         else:
             uid=email_or_uid
 
-        url=f"https://webexapis.com/v1/people/{uid}"
-        r = requests.request("GET", url, headers=self.setHeaders())
-        s = r.status_code
-        if s == 200 :
-            ut.trace(3,f"found {uid}")
-            return(r.json())
-        else:
-            ut.trace(1,f"did not find {uid}")
-            return("")
-
+        url=f"people/{uid}"
+        return self.get_wbx_data(url)
     
     # returms user id of given user email address 
     # returns "" if not found or some error   
     #
     def get_user_id(self, ue, ignore_error=False):
-        # disable warnings about using certificate verification
-        requests.packages.urllib3.disable_warnings()
-        # get_user_url=urllib.parse.quote("https://webexapis.com/v1/people?email=" + ue)
-        get_user_url="https://webexapis.com/v1/people?email=" +ue
-
-        ut.trace (3, f"calling {get_user_url} T = {ACCESS_TOKEN}")  
-        # send GET request and do not verify SSL certificate for simplicity of this example
-        r = requests.get(get_user_url, headers=self.setHeaders(), verify=True)
-        s = r.status_code
-        if s == 200 :
-            j = r.json()
+      
+        j = self.get_wbx_data("people?", "email="+ue, ignore_error)
+        if ( j ) :
             if ( len(j["items"]) == 0 ):
                 not ignore_error and ut.trace (1, f"user email {ue} not found")
                 return("")
             else:
                 if ( len(j["items"]) > 1 ):
                     ut.trace(1, f"Error found more than one match for user {ue}")
                     return(-2)
                 if ( len(j["items"]) == 1 ):
                     u = j["items"][0]
                     ut.trace (3,f"email {ue} found {u['id']} ")
                     return(u['id'])     
-        elif s == 404:
-            not ignore_error and ut.trace(1,f"got error {s}: {r.reason}")  
-            return("")
-        else :
-            ut.trace(1,f"got error {s}: {r.reason}")  
-            return("")
         
     # generic head request  
     # 
     def req_head(self, url):
         ut.trace(3, f"{url} ")
         try:
             r = requests.head(url, headers=self.setHeaders())
@@ -129,51 +108,32 @@
         except requests.exceptions.RequestException as e:
             ut.trace(1, f"error {e}")
             return({})
 
     # generic events API 
     # 
     def get_events(self, opts):
-        url=f"https://webexapis.com/v1/events{opts}"
-        ut.trace(3, f"{url} ")
-        try:
-            r = requests.get(url, headers=self.setHeaders())
-            s = r.status_code
-            if (s == 200):
-                d = r.json()
-                ut.trace(3, f"success")  
-                return(d)
-            else:
-                ut.trace(1,f"error {s}: {r.reason}")  
-                return({})
-        except requests.exceptions.RequestException as e:
-            ut.trace(1, f"error {e}")
-            return({})
-
+        url=f"events{opts}"
+        ut.trace(3, f"get_events {url} ")
+        return self.get_wbx_data(url)
 
     # get membership list for given room id  
     # 
     def get_space_memberships(self, rid, ignore_error=False):
-        url=f"https://webexapis.com/v1/memberships/?roomId={rid}"
+        url=f"memberships/?roomId={rid}"
         ut.trace(3, f"{url} ")
-        try:
-            r = requests.get(url, headers=self.setHeaders())
-            s = r.status_code
-            if (s == 200):
-                d = r.json()
-                ut.trace(3, f"success for get_memberships")  
-                return(d)
-            else:
-                not ignore_error and ut.trace(1,f"get_memberships error {s}: {r.reason}")
-                ut.trace(3, f"error {s}: {r.reason} ")  
-                return({})
-        except requests.exceptions.RequestException as e:
-            ut.trace(1, f"error {e}")
-            return({})
+        return self.get_wbx_data(url, "", ignore_error)
 
+    # get list of spaces for a user email
+    # 
+    def get_user_spaces(self, email, ignore_error=False):
+        url=f"memberships"
+        data = self.get_wbx_data(url, f"?personEmail={email}", ignore_error)
+        ut.trace(3, f"get_user_spaces : got {json.dumps(data)} ")
+        return(data)
 
     # download url contents   
     # will use name from content dispostion by default
     # 
     def download_contents(self, url, dir="", name=""):
         hds=self.req_head(url)
         if ('Content-Disposition' in hds ):
@@ -325,16 +285,15 @@
         if (ue):
             try:
                 uid = self.get_user_id(ue, True)
                 actorIdParam=f"&actorId={uid}"
             except:
                 ut.trace(1, f"error host email {ue} not found.")
                 return({})
-        
-
+            
         frm = datetime.datetime.now(timezone.utc) - datetime.timedelta(30)
         frmiso = frm.isoformat(timespec='milliseconds')
         utcFrm = re.sub('\+.+','', frmiso) + 'Z' # remove the tz suffix 
 
         to = UTCNOW
         opts = {'max': 100,'from':utcFrm,'to':to}
```

### Comparing `wbx_cpl-1.2.2/LICENSE` & `wbx_cpl-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wbx_cpl-1.2.2/README.md` & `wbx_cpl-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -61,11 +61,16 @@
 
 # List members in given space ID, save to file
 # python3 -m wbx_cpl messaging space-members -c /tmp/members.csv Y2lzY29zcGFyazovL3VybjpURUFNOnVzLXdlc3QtMl9yL1JPT00vZjBhZTRjZDAtNTdhMS0xMWVlLWEyYjktYjU2MmFiZTI4YzY3
 
 # Download files attached to message id, save files under /tmp
 # python3 -m wbx_cpl messaging message-files -d /tmp/ Y2lzY29zcGFyazovL3VybjpURUFNOnVzLXdlc3QtMl9yL01FU1NBR0UvMWYwY2NkZDAtYTNmMi0xMWVlLWI4ZGQtM2RlYzU4YzM1NTJm
 
+# List spaces joined by given user email 
+# python3 -m wbx_cpl messaging user-spaces sc-ben@mail.com
+
+# List spaces joined by users listed in user export file (column 'User ID/Email (Required)')
+# python3 -m wbx_cpl messaging spaces-count exported_users-a.csv 
 ```
 
 ## Notes:
 - the --filter option follows the input parameters of [Webex Events End Point](https://developer.webex.com/docs/api/v1/events/list-events)
```

### Comparing `wbx_cpl-1.2.2/pyproject.toml` & `wbx_cpl-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wbx-cpl"
-version = "1.2.2"
+version = "1.3.1"
 description = "Commands for Webex Compliance Officers"
 readme = "README.md"
 authors = [{ name = "Stephane Cohen", email = "stecohen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `wbx_cpl-1.2.2/PKG-INFO` & `wbx_cpl-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wbx-cpl
-Version: 1.2.2
+Version: 1.3.1
 Summary: Commands for Webex Compliance Officers
 Author-email: Stephane Cohen <stecohen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephane Cohen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -98,11 +98,16 @@
 
 # List members in given space ID, save to file
 # python3 -m wbx_cpl messaging space-members -c /tmp/members.csv Y2lzY29zcGFyazovL3VybjpURUFNOnVzLXdlc3QtMl9yL1JPT00vZjBhZTRjZDAtNTdhMS0xMWVlLWEyYjktYjU2MmFiZTI4YzY3
 
 # Download files attached to message id, save files under /tmp
 # python3 -m wbx_cpl messaging message-files -d /tmp/ Y2lzY29zcGFyazovL3VybjpURUFNOnVzLXdlc3QtMl9yL01FU1NBR0UvMWYwY2NkZDAtYTNmMi0xMWVlLWI4ZGQtM2RlYzU4YzM1NTJm
 
+# List spaces joined by given user email 
+# python3 -m wbx_cpl messaging user-spaces sc-ben@mail.com
+
+# List spaces joined by users listed in user export file (column 'User ID/Email (Required)')
+# python3 -m wbx_cpl messaging spaces-count exported_users-a.csv 
 ```
 
 ## Notes:
 - the --filter option follows the input parameters of [Webex Events End Point](https://developer.webex.com/docs/api/v1/events/list-events)
```

