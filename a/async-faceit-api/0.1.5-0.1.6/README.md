# Comparing `tmp/async_faceit_api-0.1.5.tar.gz` & `tmp/async_faceit_api-0.1.6.tar.gz`

## Comparing `async_faceit_api-0.1.5.tar` & `async_faceit_api-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.gitattributes
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.readthedocs.yaml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/.gitignore
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/AsyncFaceitApi.iml
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0    11016 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/workspace.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/Makefile
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/async_faceit_api.rst
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/conf.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/make.bat
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/modules.rst
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/src/async_faceit_api/__init__.py
--rw-r--r--   0        0        0    43678 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/src/async_faceit_api/api.py
--rw-r--r--   0        0        0    45988 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/src/async_faceit_api/dataclasses.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/src/async_faceit_api/enums.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/tests/example.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/tests/subclassing.py
--rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/tests/test.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/LICENSE
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.gitattributes
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.readthedocs.yaml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.idea/.gitignore
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.idea/AsyncFaceitApi.iml
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.idea/misc.xml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.idea/vcs.xml
+-rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/docs/Makefile
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/docs/async_faceit_api.rst
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/docs/conf.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/docs/make.bat
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/docs/modules.rst
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/docs/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/src/async_faceit_api/__init__.py
+-rw-r--r--   0        0        0    43915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/src/async_faceit_api/api.py
+-rw-r--r--   0        0        0    45988 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/src/async_faceit_api/dataclasses.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/src/async_faceit_api/enums.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/tests/example.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/tests/subclassing.py
+-rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/tests/test.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 async_faceit_api-0.1.6/PKG-INFO
```

### Comparing `async_faceit_api-0.1.5/.idea/AsyncFaceitApi.iml` & `async_faceit_api-0.1.6/.idea/AsyncFaceitApi.iml`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/.idea/workspace.xml` & `async_faceit_api-0.1.6/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `async_faceit_api-0.1.5/.idea/workspace.xml` & `async_faceit_api-0.1.6/.idea/workspace.xml`

```diff
@@ -1,14 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment="Fixing API request limit"/>
+    <list default="true" id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment="Fixing API request limit">
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/async_faceit_api/api.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/async_faceit_api/api.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -37,15 +40,15 @@
   <component name="ProjectId" id="2LMV0mUfKVJq9IJNiRVBR33s24J"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">{
   &quot;keyToString&quot;: {
-    &quot;last_opened_file_path&quot;: &quot;D:/Programming/Projekte/SmurfSniffer&quot;,
+    &quot;last_opened_file_path&quot;: &quot;D:/Programming/Projekte/AsyncFaceitApi&quot;,
     &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
 }</component>
   <component name="PyDebuggerOptionsProvider">
     <option name="mySaveCallSignatures" value="true"/>
   </component>
   <component name="RecentsManager">
```

### Comparing `async_faceit_api-0.1.5/docs/Makefile` & `async_faceit_api-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/docs/async_faceit_api.rst` & `async_faceit_api-0.1.6/docs/async_faceit_api.rst`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/docs/conf.py` & `async_faceit_api-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/docs/make.bat` & `async_faceit_api-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/src/async_faceit_api/api.py` & `async_faceit_api-0.1.6/src/async_faceit_api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,39 +10,44 @@
 class FaceitAPI:
     """
     See the faceit data-api docs for more information:
     https://developers.faceit.com/docs/tools/data-api
     """
 
     __BASE_URL = 'https://open.faceit.com/data/v4/{}'
+    __LIMIT_PER_SEC = 100
     __LIMIT_PER_10_SEC = 400
     __LIMIT_PER_H = 10_000
 
+    __sec_semaphore = Semaphore(__LIMIT_PER_SEC)
     __10_sec_semaphore = Semaphore(__LIMIT_PER_10_SEC)
     __h_semaphore = Semaphore(__LIMIT_PER_H)
 
     def __init__(self, api_token: str, rate_limit_behaviour: RateLimitBehaviour = RateLimitBehaviour.WAIT_SOME_SEC):
         self.__header = {
             'accept': 'application/json',
             'Authorization': f'Bearer {api_token}'
         }
         self.__rate_limit_behaviour = rate_limit_behaviour
 
     async def __make_request(self, method: str, url: str) -> Tuple[int, Any]:
-        if self.__rate_limit_behaviour == RateLimitBehaviour.NEVER_WAIT and (self.__10_sec_semaphore.locked() or self.__h_semaphore.locked()):
+        if (self.__rate_limit_behaviour == RateLimitBehaviour.NEVER_WAIT and
+                (self.__10_sec_semaphore.locked() or self.__h_semaphore.locked() or self.__sec_semaphore.locked())):
             return 429, {}
         if self.__rate_limit_behaviour == RateLimitBehaviour.WAIT_SOME_SEC and self.__h_semaphore.locked():
             return 429, {}
+        await self.__sec_semaphore.acquire()
         await self.__10_sec_semaphore.acquire()
         await self.__h_semaphore.acquire()
         try:
             async with request(method, url, headers=self.__header) as response:
                 return response.status, await response.json()
         finally:
             loop = asyncio.get_event_loop()
+            loop.call_later(1, self.__sec_semaphore.release)
             loop.call_later(10, self.__10_sec_semaphore.release)
             loop.call_later(3600, self.__h_semaphore.release)
 
     @staticmethod
     async def __create_object(response: Tuple[int, Any], object_class=None) -> Any:
         status, json_response = response
         if not 200 <= status < 300:
```

### Comparing `async_faceit_api-0.1.5/src/async_faceit_api/dataclasses.py` & `async_faceit_api-0.1.6/src/async_faceit_api/dataclasses.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/src/async_faceit_api/enums.py` & `async_faceit_api-0.1.6/src/async_faceit_api/enums.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/tests/subclassing.py` & `async_faceit_api-0.1.6/tests/subclassing.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/tests/test.py` & `async_faceit_api-0.1.6/tests/test.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/.gitignore` & `async_faceit_api-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/LICENSE` & `async_faceit_api-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/README.md` & `async_faceit_api-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.5/pyproject.toml` & `async_faceit_api-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "async_faceit_api"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Stuart", email="stuart.the.yellow.one@gmail.com" },
 ]
 description = "Async wrapper for the faceit API"
 documentation = "https://async-faceit-api.readthedocs.io/en/latest/index.html"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `async_faceit_api-0.1.5/PKG-INFO` & `async_faceit_api-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: async_faceit_api
-Version: 0.1.5
+Version: 0.1.6
 Summary: Async wrapper for the faceit API
 Project-URL: Homepage, https://github.com/StuartTheYellowOne/async_faceit_api
 Project-URL: Bug Tracker, https://github.com/StuartTheYellowOne/async_faceit_api/issues
 Author-email: Stuart <stuart.the.yellow.one@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

