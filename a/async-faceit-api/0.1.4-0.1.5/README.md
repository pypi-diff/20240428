# Comparing `tmp/async_faceit_api-0.1.4.tar.gz` & `tmp/async_faceit_api-0.1.5.tar.gz`

## Comparing `async_faceit_api-0.1.4.tar` & `async_faceit_api-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.gitattributes
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.readthedocs.yaml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.idea/.gitignore
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.idea/AsyncFaceitApi.iml
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.idea/misc.xml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.idea/vcs.xml
--rw-r--r--   0        0        0    10253 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.idea/workspace.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/docs/Makefile
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/docs/async_faceit_api.rst
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/docs/conf.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/docs/make.bat
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/docs/modules.rst
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/docs/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/src/async_faceit_api/__init__.py
--rw-r--r--   0        0        0    43659 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/src/async_faceit_api/api.py
--rw-r--r--   0        0        0    45988 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/src/async_faceit_api/dataclasses.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/src/async_faceit_api/enums.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/tests/example.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/tests/subclassing.py
--rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/tests/test.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/LICENSE
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 async_faceit_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.gitattributes
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.readthedocs.yaml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/.gitignore
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/AsyncFaceitApi.iml
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/misc.xml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/vcs.xml
+-rw-r--r--   0        0        0    11016 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/Makefile
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/async_faceit_api.rst
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/conf.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/make.bat
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/modules.rst
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/docs/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/src/async_faceit_api/__init__.py
+-rw-r--r--   0        0        0    43678 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/src/async_faceit_api/api.py
+-rw-r--r--   0        0        0    45988 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/src/async_faceit_api/dataclasses.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/src/async_faceit_api/enums.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/tests/example.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/tests/subclassing.py
+-rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/tests/test.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 async_faceit_api-0.1.5/PKG-INFO
```

### Comparing `async_faceit_api-0.1.4/.idea/AsyncFaceitApi.iml` & `async_faceit_api-0.1.5/.idea/AsyncFaceitApi.iml`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/.idea/workspace.xml` & `async_faceit_api-0.1.5/.idea/workspace.xml`

 * *Files 4% similar despite different names*

#### Comparing `async_faceit_api-0.1.4/.idea/workspace.xml` & `async_faceit_api-0.1.5/.idea/workspace.xml`

```diff
@@ -1,21 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/.idea/AsyncFaceitApi.iml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/AsyncFaceitApi.iml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/.idea/misc.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/misc.xml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/async_faceit_api/enums.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/async_faceit_api/enums.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/test.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test.py" afterDir="false"/>
-    </list>
+    <list default="true" id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment="Fixing API request limit"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -42,20 +35,20 @@
   &quot;associatedIndex&quot;: 3
 }</component>
   <component name="ProjectId" id="2LMV0mUfKVJq9IJNiRVBR33s24J"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "last_opened_file_path": "D:/Programming/Projekte/AsyncFaceitApi",
-    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;last_opened_file_path&quot;: &quot;D:/Programming/Projekte/SmurfSniffer&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
-}]]></component>
+}</component>
   <component name="PyDebuggerOptionsProvider">
     <option name="mySaveCallSignatures" value="true"/>
   </component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="D:\Programming\Projekte\AsyncFaceitApi\docs"/>
       <recent name="D:\Programming\Projekte\AsyncFaceitApi"/>
@@ -185,28 +178,64 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment=""/>
       <created>1675680717988</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1675680717988</updated>
     </task>
+    <task id="LOCAL-00001" summary="Fixing API request limit">
+      <option name="closed" value="true"/>
+      <created>1714240622448</created>
+      <option name="number" value="00001"/>
+      <option name="presentableId" value="LOCAL-00001"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1714240622448</updated>
+    </task>
+    <task id="LOCAL-00002" summary="Fixing API request limit">
+      <option name="closed" value="true"/>
+      <created>1714240800461</created>
+      <option name="number" value="00002"/>
+      <option name="presentableId" value="LOCAL-00002"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1714240800461</updated>
+    </task>
+    <option name="localTasksCounter" value="3"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
+  <component name="VcsManagerConfiguration">
+    <MESSAGE value="Fixing API request limit"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Fixing API request limit"/>
+  </component>
   <component name="XDebuggerManager">
+    <breakpoint-manager>
+      <breakpoints>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/example.py</url>
+          <line>8</line>
+          <option name="timeStamp" value="1"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test.py</url>
+          <line>183</line>
+          <option name="timeStamp" value="3"/>
+        </line-breakpoint>
+      </breakpoints>
+    </breakpoint-manager>
     <watches-manager>
       <configuration name="PythonConfigurationType">
         <watch expression="retval[1]" language="Python"/>
+        <watch expression="match.teams"/>
       </configuration>
     </watches-manager>
   </component>
 </project>
```

### Comparing `async_faceit_api-0.1.4/docs/Makefile` & `async_faceit_api-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/docs/async_faceit_api.rst` & `async_faceit_api-0.1.5/docs/async_faceit_api.rst`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/docs/conf.py` & `async_faceit_api-0.1.5/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 sys.path.insert(0, os.path.abspath('../src'))
 
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Async Facit API'
-copyright = '2023, Stuart'
+copyright = '2024, Stuart'
 author = 'Stuart'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.todo',
     'sphinx.ext.viewcode',
     'sphinx.ext.autodoc',
+    'sphinx_rtd_theme',
 ]
 epub_show_urls = 'footnote'
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
```

### Comparing `async_faceit_api-0.1.4/docs/make.bat` & `async_faceit_api-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/src/async_faceit_api/api.py` & `async_faceit_api-0.1.5/src/async_faceit_api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 class FaceitAPI:
     """
     See the faceit data-api docs for more information:
     https://developers.faceit.com/docs/tools/data-api
     """
 
     __BASE_URL = 'https://open.faceit.com/data/v4/{}'
-    __LIMIT_PER_SEC = 100
+    __LIMIT_PER_10_SEC = 400
     __LIMIT_PER_H = 10_000
 
-    __sec_semaphore = Semaphore(__LIMIT_PER_SEC)
+    __10_sec_semaphore = Semaphore(__LIMIT_PER_10_SEC)
     __h_semaphore = Semaphore(__LIMIT_PER_H)
 
     def __init__(self, api_token: str, rate_limit_behaviour: RateLimitBehaviour = RateLimitBehaviour.WAIT_SOME_SEC):
         self.__header = {
             'accept': 'application/json',
             'Authorization': f'Bearer {api_token}'
         }
         self.__rate_limit_behaviour = rate_limit_behaviour
 
     async def __make_request(self, method: str, url: str) -> Tuple[int, Any]:
-        if self.__rate_limit_behaviour == RateLimitBehaviour.NEVER_WAIT and (self.__sec_semaphore.locked() or self.__h_semaphore.locked()):
+        if self.__rate_limit_behaviour == RateLimitBehaviour.NEVER_WAIT and (self.__10_sec_semaphore.locked() or self.__h_semaphore.locked()):
             return 429, {}
         if self.__rate_limit_behaviour == RateLimitBehaviour.WAIT_SOME_SEC and self.__h_semaphore.locked():
             return 429, {}
-        await self.__sec_semaphore.acquire()
+        await self.__10_sec_semaphore.acquire()
         await self.__h_semaphore.acquire()
         try:
             async with request(method, url, headers=self.__header) as response:
                 return response.status, await response.json()
         finally:
             loop = asyncio.get_event_loop()
-            loop.call_later(1, self.__sec_semaphore.release)
+            loop.call_later(10, self.__10_sec_semaphore.release)
             loop.call_later(3600, self.__h_semaphore.release)
 
     @staticmethod
     async def __create_object(response: Tuple[int, Any], object_class=None) -> Any:
         status, json_response = response
         if not 200 <= status < 300:
             if status == 429:
```

### Comparing `async_faceit_api-0.1.4/src/async_faceit_api/dataclasses.py` & `async_faceit_api-0.1.5/src/async_faceit_api/dataclasses.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/src/async_faceit_api/enums.py` & `async_faceit_api-0.1.5/src/async_faceit_api/enums.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/tests/subclassing.py` & `async_faceit_api-0.1.5/tests/subclassing.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/tests/test.py` & `async_faceit_api-0.1.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/.gitignore` & `async_faceit_api-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/LICENSE` & `async_faceit_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/README.md` & `async_faceit_api-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.4/pyproject.toml` & `async_faceit_api-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "async_faceit_api"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Stuart", email="stuart.the.yellow.one@gmail.com" },
 ]
 description = "Async wrapper for the faceit API"
 documentation = "https://async-faceit-api.readthedocs.io/en/latest/index.html"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `async_faceit_api-0.1.4/PKG-INFO` & `async_faceit_api-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: async_faceit_api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Async wrapper for the faceit API
 Project-URL: Homepage, https://github.com/StuartTheYellowOne/async_faceit_api
 Project-URL: Bug Tracker, https://github.com/StuartTheYellowOne/async_faceit_api/issues
 Author-email: Stuart <stuart.the.yellow.one@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

