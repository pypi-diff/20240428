# Comparing `tmp/pyracf-0.8.6.tar.gz` & `tmp/pyracf-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.8.6.tar", last modified: Sun Apr 21 10:13:56 2024, max compression
+gzip compressed data, was "pyracf-0.8.7.tar", last modified: Sun Apr 28 08:56:34 2024, max compression
```

## Comparing `pyracf-0.8.6.tar` & `pyracf-0.8.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.502463 pyracf-0.8.6/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2024-04-21 09:03:17.000000 pyracf-0.8.6/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2024-04-21 09:03:17.000000 pyracf-0.8.6/MANIFEST.in
--rw-r--r--   0 henri     (1000) henri     (1000)    16873 2024-04-21 10:13:56.502463 pyracf-0.8.6/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)    16265 2024-04-21 09:03:17.000000 pyracf-0.8.6/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)      161 2024-04-21 09:03:17.000000 pyracf-0.8.6/pyproject.toml
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-21 10:13:56.502463 pyracf-0.8.6/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-21 10:13:30.000000 pyracf-0.8.6/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.498463 pyracf-0.8.6/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.502463 pyracf-0.8.6/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    61872 2024-04-21 10:02:25.000000 pyracf-0.8.6/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-21 09:03:17.000000 pyracf-0.8.6/src/pyracf/getOffsets.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-21 09:03:17.000000 pyracf-0.8.6/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.502463 pyracf-0.8.6/src/pyracf.egg-info/
--rw-r--r--   0 henri     (1000) henri     (1000)    16873 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      412 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/top_level.txt
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.502463 pyracf-0.8.6/test/
--rw-rw-r--   0 henri     (1000) henri     (1000)      794 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_connect_df.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1461 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_frame_dataset.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1504 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_frame_general.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     6654 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_frames.py
--rw-rw-r--   0 henri     (1000) henri     (1000)      466 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_parsed.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.120563 pyracf-0.8.7/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2024-04-21 09:03:17.000000 pyracf-0.8.7/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2024-04-21 09:03:17.000000 pyracf-0.8.7/MANIFEST.in
+-rw-r--r--   0 henri     (1000) henri     (1000)    17335 2024-04-28 08:56:34.116563 pyracf-0.8.7/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)    16727 2024-04-28 08:25:21.000000 pyracf-0.8.7/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)      161 2024-04-21 09:03:17.000000 pyracf-0.8.7/pyproject.toml
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-28 08:56:34.120563 pyracf-0.8.7/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-28 08:19:24.000000 pyracf-0.8.7/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.116563 pyracf-0.8.7/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.116563 pyracf-0.8.7/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    62293 2024-04-28 08:42:05.000000 pyracf-0.8.7/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-21 09:03:17.000000 pyracf-0.8.7/src/pyracf/getOffsets.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-21 09:03:17.000000 pyracf-0.8.7/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.116563 pyracf-0.8.7/src/pyracf.egg-info/
+-rw-r--r--   0 henri     (1000) henri     (1000)    17335 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      412 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.116563 pyracf-0.8.7/test/
+-rw-rw-r--   0 henri     (1000) henri     (1000)      794 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_connect_df.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1461 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_frame_dataset.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1504 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_frame_general.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     6654 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_frames.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)      466 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_parsed.py
```

### Comparing `pyracf-0.8.6/LICENSE` & `pyracf-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.6/PKG-INFO` & `pyracf-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.6
+Version: 0.8.7
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -29,14 +29,24 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.7 (fixes for pickles, pytest, wiki)
+- grouptree and ownertree are now properties, no longer callables
+- accept * as a literal value in gfilter( )
+- r.connect('SYS1') and r.connect(None,'IBMUSER') return one level index
+- less contentious column name ALL_USER_ACCESS replaces EFFECTIVE_UACC
+- speed up single profile methods 
+- Single value selections return dataframe with columns again
+- giveMeProfiles, generic2regex are now 'internal' (_) functions
+
+
 ### 0.8.5 (fixes for pickles, pytest, wiki)
 - parse_fancycli now creates empty data frames for pickles it could not find
 - index added to data frames from old pickles, not for pickles that already have index fields
 - pytest framework for QA in development cycle, initial tests ensure attributes are the same with all 3 methods to obtain RACF profiles
 - wiki https://github.com/wizardofzos/pyracf/wiki
 
 ### 0.8.3 (tree print format for grouptree and ownertree)
```

### Comparing `pyracf-0.8.6/README.md` & `pyracf-0.8.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.7 (fixes for pickles, pytest, wiki)
+- grouptree and ownertree are now properties, no longer callables
+- accept * as a literal value in gfilter( )
+- r.connect('SYS1') and r.connect(None,'IBMUSER') return one level index
+- less contentious column name ALL_USER_ACCESS replaces EFFECTIVE_UACC
+- speed up single profile methods 
+- Single value selections return dataframe with columns again
+- giveMeProfiles, generic2regex are now 'internal' (_) functions
+
+
 ### 0.8.5 (fixes for pickles, pytest, wiki)
 - parse_fancycli now creates empty data frames for pickles it could not find
 - index added to data frames from old pickles, not for pickles that already have index fields
 - pytest framework for QA in development cycle, initial tests ensure attributes are the same with all 3 methods to obtain RACF profiles
 - wiki https://github.com/wizardofzos/pyracf/wiki
 
 ### 0.8.3 (tree print format for grouptree and ownertree)
```

### Comparing `pyracf-0.8.6/setup.py` & `pyracf-0.8.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.8.6",
+    version="0.8.7",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.8.6/src/pyracf/__init__.py` & `pyracf-0.8.7/src/pyracf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,33 +63,40 @@
                 ix = supgrpMembers.index(anchor)
                 supgrpMembers[ix] = {anchor: tree[anchor]}
                 deletes.append(anchor)
         for anchor in deletes:
             tree.pop(anchor)
         if '' in tree:  # bring SYS1 to the top, supgroup of SYS1 is ''
             tree = tree[''][0]
-        self.tree = tree
+        super().__init__(tree)
         self._format = 'unix'
         
-    def __get__(self):
-        ''' class objects have a value too '''
-        return self.tree
-
     def __str__(self):
         ''' what happens when print(object) is issued '''
-        return self.simple_format(self.tree) if self._format=='simple' else self.unix_format(self.tree)
+        return self.simple_format(self) if self._format=='simple' else self.unix_format(self)
+         
+    def format(self,format='unix'):
+        ''' return printable tree '''
+        if format in ['unix','simple']:
+            return self.simple_format(self) if format=='simple' else self.unix_format(self)
+        else:
+            warnings.warn(f'Unsupported format value {format}, select unix or simple.')
         
     def setformat(self,format='unix'):
         ''' set default format for next print '''
         if format in ['unix','simple']:
             self._format = format
-            return self
         else:
             warnings.warn(f'Unsupported format value {format}, select unix or simple.')
 
+    @property
+    def tree(self):
+        warnings.warn('.tree attribute is deprecated, this is now the default return value of the tree objected')
+        return self
+
     def unix_format(self,branch=None,prefix=''):
         ''' print groups, prefixed with vertical bars to show depth '''
         BOX_START = u'\u250C'
         BOX_ENTRY = u'\u251C'
         BOX_CONT = u'\u2502'
         BOX_END = u'\u2514'
         if not branch:
@@ -490,30 +497,30 @@
         if self.parsed("GPBD") > 0 and self.parsed("GPMEM") > 0 and self.parsed("USCON") > 0:
             self._connectData["GPMEM_AUTH"] = self._connects["GPMEM_AUTH"]
 
         # copy ID(*) access into resource frames, similar to UACC: IDSTAR_ACCESS and ALL_USER_ACCESS
         if self.parsed("DSBD") > 0 and self.parsed("DSACC") > 0 and 'IDSTAR_ACCESS' not in self._datasets.columns:
             uaccs = pd.DataFrame()
             uaccs["UACC_NUM"] = self._datasets["DSBD_UACC"].map(RACF.accessKeywords.index)
-            uaccs["IDSTAR_ACCESS"] = self._datasetAccess.gfilter(None, '*').droplevel([1,2])['DSACC_ACCESS'].drop_duplicates()
+            uaccs["IDSTAR_ACCESS"] = self._datasetAccess.gfilter(None, '*').droplevel([1,2])['DSACC_ACCESS']
             uaccs["IDSTAR_ACCESS"] = uaccs["IDSTAR_ACCESS"].fillna(' ')
             uaccs["IDSTAR_NUM"] = uaccs["IDSTAR_ACCESS"].map(RACF.accessKeywords.index)
             uaccs["ALL_USER_NUM"] = uaccs[["IDSTAR_NUM","UACC_NUM"]].max(axis=1)
             uaccs["ALL_USER_ACCESS"] = uaccs['ALL_USER_NUM'].map(RACF.accessKeywords.__getitem__)
             column = self._datasets.columns.to_list().index('DSBD_UACC')
             self._datasets.insert(column+1,"IDSTAR_ACCESS",uaccs["IDSTAR_ACCESS"])
             self._datasets.insert(column+2,"ALL_USER_ACCESS",uaccs["ALL_USER_ACCESS"])
             del uaccs
         
         if self.parsed("GRBD") > 0 and self.parsed("GRACC") > 0 and 'IDSTAR_ACCESS' not in self._generals.columns:
             uaccs = pd.DataFrame()
             uaccs["UACC"] = self._generals["GRBD_UACC"]
             uaccs["UACC"] = uaccs["UACC"].where(uaccs["UACC"].isin(RACF.accessKeywords),other=' ')  # DIGTCERT fields may be distorted
             uaccs["UACC_NUM"] = uaccs["UACC"].map(RACF.accessKeywords.index)
-            uaccs["IDSTAR_ACCESS"] = self._generalAccess.gfilter(None, '*').droplevel([1,2])['GRACC_ACCESS'].drop_duplicates()
+            uaccs["IDSTAR_ACCESS"] = self._generalAccess.gfilter(None, '*').droplevel([1,2]).drop_duplicates(['GRACC_CLASS_NAME','GRACC_NAME','GRACC_ACCESS'])['GRACC_ACCESS']
             uaccs["IDSTAR_ACCESS"] = uaccs["IDSTAR_ACCESS"].fillna(' ')
             uaccs["IDSTAR_NUM"] = uaccs["IDSTAR_ACCESS"].map(RACF.accessKeywords.index)
             uaccs["ALL_USER_NUM"] = uaccs[["IDSTAR_NUM","UACC_NUM"]].max(axis=1)
             uaccs["ALL_USER_ACCESS"] = uaccs['ALL_USER_NUM'].map(RACF.accessKeywords.__getitem__)
             column = self._generals.columns.to_list().index('GRBD_UACC')
             self._generals.insert(column+1,"IDSTAR_ACCESS",uaccs["IDSTAR_ACCESS"])
             self._generals.insert(column+2,"ALL_USER_ACCESS",uaccs["ALL_USER_ACCESS"])
@@ -578,15 +585,15 @@
             if rtype in self._records and self._records[rtype]['parsed']>0:
                 self.save_pickle(df=getattr(self, rinfo['df']), dfname=rinfo['name'], path=path, prefix=prefix)
             else:
                 # TODO: ensure consistent data, delete old pickles that were not saved
                 pass
 
 
-    def generic2regex(selection, lenient='%&*'):
+    def _generic2regex(selection, lenient='%&*'):
         ''' Change a RACF generic pattern into regex to match with text strings in pandas cells.  use lenient="" to match with dsnames/resources '''
         if selection in ('**',''):
             return '.*$'
         else:
             return selection.replace('*.**','`dot``ast`')\
                     .replace('.**',r'\`dot``dot``ast`')\
                     .replace('*',r'[\w@#$`lenient`]`ast`')\
@@ -594,15 +601,15 @@
                     .replace('.',r'\.')\
                     .replace('`dot`','.')\
                     .replace('`ast`','*')\
                     .replace('`lenient`',lenient)\
                     +'$'
 
 
-    def giveMeProfiles(self, df, selection=None, option=None):
+    def _giveMeProfiles(self, df, selection=None, option=None):
         ''' Search profiles using the index fields.  selection can be str or tuple.  Tuples check for group + user id in connects, or class + profile key in generals.
         option controls how selection is interpreted, and how data must be returned:
         None is for (expensive) backward compatibility, returns a df with 1 profile.
         LIST returns a series for 1 profile, much faster and easier to process.
         '''
         if not selection:
             raise StoopidException('profile criteria not specified...')
@@ -616,64 +623,64 @@
                 else:
                     selection = [selection]
             else:
                 pass
             try:
                 return df.loc[selection]
             except KeyError:
-                if not option:  # return DataFrame with profiles
-                    return pd.DataFrame()
+                if not option:  # return empty DataFrame with all the original columns
+                    return df.head(0)
                 else:  # return Series 
                     return []
         else:
             raise StoopidException(f'unexpected last parameter {option}')
 
 
     def gfilter(df, *selection):
         ''' Search profiles using GENERIC pattern on the index fields.  selection can be one or more values, corresponding to index levels of the df '''
         locs = pd.array([True]*df.shape[0])
         for s in range(len(selection)):
             if selection[s] not in (None,'**'):
                 if selection[s]=='*':
                     locs &= (df.index.get_level_values(s)=='*')
                 else: 
-                    locs &= (df.index.get_level_values(s).str.match(RACF.generic2regex(selection[s])))
+                    locs &= (df.index.get_level_values(s).str.match(RACF._generic2regex(selection[s])))
         return df.loc[locs]
 
     def rfilter(df, *selection):
         ''' Search profiles using refex on the index fields.  selection can be one or more values, corresponding to index levels of the df '''
         locs = pd.array([True]*df.shape[0])
         for s in range(len(selection)):
             if selection[s] not in (None,'**','.*'):
                 locs &= (df.index.get_level_values(s).str.match(selection[s]))
         return df.loc[locs]
 
     # user frames
 
     def user(self, userid=None, pattern=None):
-        return self.giveMeProfiles(self._users, userid, pattern)
+        return self._giveMeProfiles(self._users, userid, pattern)
 
     def connect(self, group=None, userid=None, pattern=None):
         ''' connect('SYS1') returns 1 index level with user IDs, connect(None,'IBMUSER') returns 1 index level with group names '''
         if pattern=='L' or pattern=='LIST':
-            return self.giveMeProfiles(self._connectData, (group,userid), pattern)
+            return self._giveMeProfiles(self._connectData, (group,userid), pattern)
         else:
             if group and (not userid or userid=='**'):
                 # with group given, return connected user IDs via index (.loc['group'] strips level(0))
                 selection = group
             elif userid and (not group or group=='**'):
                 # with user ID given, return connected groups via index (only level(0))
                 return self._connectData.loc[(slice(None),userid),].droplevel(1)
             else:
                 # with group + user ID given, return 1 entry with all index levels (because only the data columns will be of interest)
                 selection = [(group,userid)]
             try:
                 return self._connectData.loc[selection]
             except KeyError:
-                return pd.DataFrame()
+                return self._connectData.head(0)  # empty frame
 
 
     @property
     def userUSRDATA(self):
         # retained here due to deprecated property definition
         return self._userUSRDATA
 
@@ -703,33 +710,33 @@
     def revoked(self):
         return self._users.loc[self._users['USBD_REVOKE'] == 'YES']
 
 
     # group frames
 
     def group(self, group=None, pattern=None):
-        return self.giveMeProfiles(self._groups, group, pattern)
+        return self._giveMeProfiles(self._groups, group, pattern)
 
     @property
     def groupsWithoutUsers(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._groups.loc[~self.groups.GPBD_NAME.isin(self._connectData.USCON_GRP_ID)]
     
 
     # dataset frames
         
     def dataset(self, profile=None, pattern=None):
-        return self.giveMeProfiles(self._datasets, profile, pattern)
+        return self._giveMeProfiles(self._datasets, profile, pattern)
 
     def datasetConditionalPermit(self, profile=None, id=None, access=None, pattern=None):
-        return self.giveMeProfiles(self._datasetConditionalAccess, (profile,id,access), pattern)
+        return self._giveMeProfiles(self._datasetConditionalAccess, (profile,id,access), pattern)
 
     def datasetPermit(self, profile=None, id=None, access=None, pattern=None):
-        return self.giveMeProfiles(self._datasetAccess, (profile,id,access), pattern)
+        return self._giveMeProfiles(self._datasetAccess, (profile,id,access), pattern)
 
     @property
     def uacc_read_datasets(self):
         return self._datasets.loc[self._datasets.DSBD_UACC=="READ"]
     @property
     def uacc_update_datasets(self):
         return self._datasets.loc[self._datasets.DSBD_UACC=="UPDATE"]
@@ -749,15 +756,15 @@
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generals
 
     generics = property(deprecated(generals,"generics"))
 
     def general(self, resclass=None, profile=None, pattern=None):
-        return self.giveMeProfiles(self._generals, (resclass,profile), pattern)
+        return self._giveMeProfiles(self._generals, (resclass,profile), pattern)
 
     @property
     def generalMembers(self, query=None):
         # retained here due to deprecated property definition
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generalMembers    
@@ -770,28 +777,28 @@
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generalAccess
 
     genericAccess = property(deprecated(generalAccess,"genericAccess"))
     
     def generalPermit(self, resclass=None, profile=None, id=None, access=None, pattern=None):
-        return self.giveMeProfiles(self._generalAccess, (resclass,profile,id,access), pattern)
+        return self._giveMeProfiles(self._generalAccess, (resclass,profile,id,access), pattern)
     
     
     @property
     def generalConditionalAccess(self):
         # retained here due to deprecated property definition
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generalConditionalAccess
 
     genericConditionalAccess = property(deprecated(generalConditionalAccess,"genericConditionalAccess"))
     
     def generalConditionalPermit(self, resclass=None, profile=None, id=None, access=None, pattern=None):
-        return self.giveMeProfiles(self._generalConditionalAccess, (resclass,profile,id,access), pattern)
+        return self._giveMeProfiles(self._generalConditionalAccess, (resclass,profile,id,access), pattern)
 
     @property
     def SSIGNON(self): # GRSIGN
         return self._generalSSIGNON.join(self._generals['GRBD_APPL_DATA'])
 
 
 
@@ -1042,15 +1049,15 @@
                     useraccess = users.get_group(u)['GRACC_ACCESS'].values[0]
                     newdata[u][i] = accessLevels[useraccess]
             df1 = pd.DataFrame(newdata)
             df1.to_excel(writer, sheet_name=c, index=False)
             worksheet = writer.sheets[c]
             worksheet.set_row(0, 64, format_br)
             worksheet.set_column(1, len(authIDsInClass)+1, 2, format_center )
-            worksheet.set_column(0, 0, longestProfile + 2 )
+            worksheet.autofit()
             worksheet.write(0, 0, 'Profile', format_nr)
 
             shared_strings = sorted(worksheet.str_table.string_table, key=worksheet.str_table.string_table.get)
             for i in range(len(authIDsInClass)+1):
                 for j in range(len(profilesInClass)+1):
                     if i>0 and j>0:
                         rdict = worksheet.table.get(j,None)
```

### Comparing `pyracf-0.8.6/src/pyracf/getOffsets.py` & `pyracf-0.8.7/src/pyracf/getOffsets.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.6/src/pyracf/offsets.json` & `pyracf-0.8.7/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.6/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.8.7/src/pyracf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.6
+Version: 0.8.7
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -29,14 +29,24 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.7 (fixes for pickles, pytest, wiki)
+- grouptree and ownertree are now properties, no longer callables
+- accept * as a literal value in gfilter( )
+- r.connect('SYS1') and r.connect(None,'IBMUSER') return one level index
+- less contentious column name ALL_USER_ACCESS replaces EFFECTIVE_UACC
+- speed up single profile methods 
+- Single value selections return dataframe with columns again
+- giveMeProfiles, generic2regex are now 'internal' (_) functions
+
+
 ### 0.8.5 (fixes for pickles, pytest, wiki)
 - parse_fancycli now creates empty data frames for pickles it could not find
 - index added to data frames from old pickles, not for pickles that already have index fields
 - pytest framework for QA in development cycle, initial tests ensure attributes are the same with all 3 methods to obtain RACF profiles
 - wiki https://github.com/wizardofzos/pyracf/wiki
 
 ### 0.8.3 (tree print format for grouptree and ownertree)
```

### Comparing `pyracf-0.8.6/test/test_connect_df.py` & `pyracf-0.8.7/test/test_connect_df.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.6/test/test_frame_dataset.py` & `pyracf-0.8.7/test/test_frame_dataset.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.6/test/test_frame_general.py` & `pyracf-0.8.7/test/test_frame_general.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.6/test/test_frames.py` & `pyracf-0.8.7/test/test_frames.py`

 * *Files identical despite different names*

