# Comparing `tmp/streamlit_chat_handler-0.1.1.tar.gz` & `tmp/streamlit_chat_handler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.1.1.tar", last modified: Sun Apr 28 02:19:57 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.1.2.tar", last modified: Sun Apr 28 02:23:26 2024, max compression
```

## Comparing `streamlit_chat_handler-0.1.1.tar` & `streamlit_chat_handler-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:19:57.604391 streamlit_chat_handler-0.1.1/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.1/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-28 02:19:57.604391 streamlit_chat_handler-0.1.1/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.1/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:19:57.604391 streamlit_chat_handler-0.1.1/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 01:47:34.000000 streamlit_chat_handler-0.1.1/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 02:07:47.000000 streamlit_chat_handler-0.1.1/examples/template_expander.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-28 02:19:23.000000 streamlit_chat_handler-0.1.1/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.1/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:19:57.604391 streamlit_chat_handler-0.1.1/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:19:57.604391 streamlit_chat_handler-0.1.1/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.1/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9658 2024-04-28 02:18:57.000000 streamlit_chat_handler-0.1.1/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2313 2024-04-28 01:41:17.000000 streamlit_chat_handler-0.1.1/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:19:57.604391 streamlit_chat_handler-0.1.1/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-28 02:19:57.000000 streamlit_chat_handler-0.1.1/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-28 02:19:57.000000 streamlit_chat_handler-0.1.1/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:19:57.000000 streamlit_chat_handler-0.1.1/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:19:57.000000 streamlit_chat_handler-0.1.1/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:19:57.000000 streamlit_chat_handler-0.1.1/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:23:26.893136 streamlit_chat_handler-0.1.2/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.2/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-28 02:23:26.893136 streamlit_chat_handler-0.1.2/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.2/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:23:26.889136 streamlit_chat_handler-0.1.2/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 01:47:34.000000 streamlit_chat_handler-0.1.2/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 02:07:47.000000 streamlit_chat_handler-0.1.2/examples/template_expander.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-28 02:23:04.000000 streamlit_chat_handler-0.1.2/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.2/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:23:26.893136 streamlit_chat_handler-0.1.2/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:23:26.889136 streamlit_chat_handler-0.1.2/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9805 2024-04-28 02:22:38.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2313 2024-04-28 01:41:17.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:23:26.893136 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.1.1/LICENSE` & `streamlit_chat_handler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.1/PKG-INFO` & `streamlit_chat_handler-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.1
+Version: 0.1.2
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.1.1/README.md` & `streamlit_chat_handler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.1/examples/template.py` & `streamlit_chat_handler-0.1.2/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.1/examples/template_expander.py` & `streamlit_chat_handler-0.1.2/examples/template_expander.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.1/pyproject.toml` & `streamlit_chat_handler-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
   {name = "Eduardo Messias de Morais", email = "emdemor415@gmail.com" },
 ]
-version = "0.1.1"
+version = "0.1.2"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.1.1/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.1.2/streamlit_chat_handler/_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,25 @@
     def __new__(cls, session_state: SessionStateProxy, session_id: str):
         """Ensure only one instance per session_id."""
         if session_id not in cls._instances:
             instance = super(StreamlitChatHandler, cls).__new__(cls)
             cls._instances[session_id] = instance
             instance.session_state = session_state
             instance.session_id = session_id
-            instance.step_counter = -1
             instance._init_session_state()
+            instance.step_counter = -1
         return cls._instances[session_id]
 
     def __init__(self, session_state: SessionStateProxy, session_id: str):
         """Initialize the instance with the session state and ID."""
+        self.session_state = session_state
+        self.session_id = session_id
+        self._init_session_state()
+        self.rendered_elements: OrderedDict[str, Any] | None = OrderedDict({})
         self.step_counter += 1
-        self.rendered_elements = OrderedDict()
 
     def append(
         self,
         role: Literal["user", "assistant"] = None,
         type: str = None,
         content: Any = None,
         index: str | None = None,
```

### Comparing `streamlit_chat_handler-0.1.1/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.1.2/streamlit_chat_handler/types.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.1/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.1
+Version: 0.1.2
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

