# Comparing `tmp/bhbotlist-3.0.5.tar.gz` & `tmp/bhbotlist-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhbotlist-3.0.5.tar", last modified: Mon Apr  1 15:49:00 2024, max compression
+gzip compressed data, was "bhbotlist-3.0.6.tar", last modified: Sun Apr 28 05:50:08 2024, max compression
```

## Comparing `bhbotlist-3.0.5.tar` & `bhbotlist-3.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-01 15:49:00.514546 bhbotlist-3.0.5/
--rw-rw-rw-   0 anshtyagi   (501) staff       (20)     1088 2023-03-21 18:47:33.000000 bhbotlist-3.0.5/LICENSE
--rw-r--r--   0 anshtyagi   (501) staff       (20)     1199 2024-04-01 15:49:00.514462 bhbotlist-3.0.5/PKG-INFO
--rw-rw-rw-   0 anshtyagi   (501) staff       (20)      898 2023-03-21 18:47:06.000000 bhbotlist-3.0.5/README.md
--rw-r--r--   0 anshtyagi   (501) staff       (20)       38 2024-04-01 15:49:00.514760 bhbotlist-3.0.5/setup.cfg
--rw-rw-rw-   0 anshtyagi   (501) staff       (20)      652 2024-04-01 15:48:58.000000 bhbotlist-3.0.5/setup.py
-drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-01 15:49:00.512190 bhbotlist-3.0.5/src/
-drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-01 15:49:00.513068 bhbotlist-3.0.5/src/bhbotlist/
--rw-rw-rw-   0 anshtyagi   (501) staff       (20)      935 2024-04-01 15:41:56.000000 bhbotlist-3.0.5/src/bhbotlist/__init__.py
-drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-01 15:49:00.514187 bhbotlist-3.0.5/src/bhbotlist.egg-info/
--rw-r--r--   0 anshtyagi   (501) staff       (20)     1199 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/PKG-INFO
--rw-r--r--   0 anshtyagi   (501) staff       (20)      246 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/SOURCES.txt
--rw-r--r--   0 anshtyagi   (501) staff       (20)        1 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/dependency_links.txt
--rw-r--r--   0 anshtyagi   (501) staff       (20)        8 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/requires.txt
--rw-r--r--   0 anshtyagi   (501) staff       (20)       10 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/top_level.txt
+drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-28 05:50:08.814168 bhbotlist-3.0.6/
+-rw-rw-rw-   0 anshtyagi   (501) staff       (20)     1088 2023-03-21 18:47:33.000000 bhbotlist-3.0.6/LICENSE
+-rw-r--r--   0 anshtyagi   (501) staff       (20)     1199 2024-04-28 05:50:08.814058 bhbotlist-3.0.6/PKG-INFO
+-rw-rw-rw-   0 anshtyagi   (501) staff       (20)      898 2023-03-21 18:47:06.000000 bhbotlist-3.0.6/README.md
+-rw-r--r--   0 anshtyagi   (501) staff       (20)       38 2024-04-28 05:50:08.814491 bhbotlist-3.0.6/setup.cfg
+-rw-rw-rw-   0 anshtyagi   (501) staff       (20)      652 2024-04-28 05:49:04.000000 bhbotlist-3.0.6/setup.py
+drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-28 05:50:08.811154 bhbotlist-3.0.6/src/
+drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-28 05:50:08.812289 bhbotlist-3.0.6/src/bhbotlist/
+-rw-rw-rw-   0 anshtyagi   (501) staff       (20)     1115 2024-04-28 05:48:46.000000 bhbotlist-3.0.6/src/bhbotlist/__init__.py
+drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-28 05:50:08.813680 bhbotlist-3.0.6/src/bhbotlist.egg-info/
+-rw-r--r--   0 anshtyagi   (501) staff       (20)     1199 2024-04-28 05:50:08.000000 bhbotlist-3.0.6/src/bhbotlist.egg-info/PKG-INFO
+-rw-r--r--   0 anshtyagi   (501) staff       (20)      246 2024-04-28 05:50:08.000000 bhbotlist-3.0.6/src/bhbotlist.egg-info/SOURCES.txt
+-rw-r--r--   0 anshtyagi   (501) staff       (20)        1 2024-04-28 05:50:08.000000 bhbotlist-3.0.6/src/bhbotlist.egg-info/dependency_links.txt
+-rw-r--r--   0 anshtyagi   (501) staff       (20)        8 2024-04-28 05:50:08.000000 bhbotlist-3.0.6/src/bhbotlist.egg-info/requires.txt
+-rw-r--r--   0 anshtyagi   (501) staff       (20)       10 2024-04-28 05:50:08.000000 bhbotlist-3.0.6/src/bhbotlist.egg-info/top_level.txt
```

### Comparing `bhbotlist-3.0.5/LICENSE` & `bhbotlist-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bhbotlist-3.0.5/PKG-INFO` & `bhbotlist-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhbotlist
-Version: 3.0.5
+Version: 3.0.6
 Summary: API for bhlist.co.in
 Author: BHBL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `bhbotlist-3.0.5/README.md` & `bhbotlist-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bhbotlist-3.0.5/setup.py` & `bhbotlist-3.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bhbotlist",
-    version="3.0.5",
+    version="3.0.6",
     author="BHBL",
     description="API for bhlist.co.in",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `bhbotlist-3.0.5/src/bhbotlist/__init__.py` & `bhbotlist-3.0.6/src/bhbotlist/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import aiohttp
 
-class bhbotlist():
-  def __init__(self,client,token):
-    self.client = client
-    self.token = token
-  
-  async def serverCountPost(self):
-    async with aiohttp.ClientSession() as session:
-        res = await session.post(url="https://api.bhlist.co.in/post/stats",headers={'serverCount': str(len(self.client.guilds)),'Content-Type': 'application/json', 'Authorization': str(self.token)})
-        await print("Server count posted.")
-        return await res.json()
-  
-  async def hasVoted(self,id):
-    async with aiohttp.ClientSession(headers={"Authorization": self.token}) as session:
-      async with session.get(f"https://api.bhlist.co.in/vote/check/{id}") as res:
-        return await res.json()
-  
-  async def search(self,id):
-    async with aiohttp.ClientSession() as session:
-        async with session.get(f"https://api.bhlist.co.in/bots/{id}") as res:
-          return await res.json()
+class bhbotlist:
+    def __init__(self, client, token):
+        self.client = client
+        self.token = token
+
+    async def serverCountPost(self):
+        async with aiohttp.ClientSession() as session:
+            payload = {'serverCount': str(len(self.client.guilds))}
+            headers = {'Authorization': str(self.token), 'Content-Type': 'application/json'}
+            async with session.post(url="https://api.bhlist.co.in/post/stats", json=payload, headers=headers) as res:
+                print("Server count posted.")
+                return await res.json()
+
+    async def hasVoted(self, id):
+        async with aiohttp.ClientSession() as session:
+            headers = {'Authorization': str(self.token)}
+            async with session.get(f"https://api.bhlist.co.in/vote/check/{id}", headers=headers) as res:
+                return await res.json()
+
+    async def search(self, id):
+        async with aiohttp.ClientSession() as session:
+            async with session.get(f"https://api.bhlist.co.in/bots/{id}") as res:
+                return await res.json()
+ƒ
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bhbotlist-3.0.5/src/bhbotlist.egg-info/PKG-INFO` & `bhbotlist-3.0.6/src/bhbotlist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhbotlist
-Version: 3.0.5
+Version: 3.0.6
 Summary: API for bhlist.co.in
 Author: BHBL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

