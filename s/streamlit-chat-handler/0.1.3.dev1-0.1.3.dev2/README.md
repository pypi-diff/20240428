# Comparing `tmp/streamlit_chat_handler-0.1.3.dev1.tar.gz` & `tmp/streamlit_chat_handler-0.1.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.1.3.dev1.tar", last modified: Sun Apr 28 02:38:44 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.1.3.dev2.tar", last modified: Sun Apr 28 02:51:47 2024, max compression
```

## Comparing `streamlit_chat_handler-0.1.3.dev1.tar` & `streamlit_chat_handler-0.1.3.dev2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:38:44.593614 streamlit_chat_handler-0.1.3.dev1/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.3.dev1/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:38:44.593614 streamlit_chat_handler-0.1.3.dev1/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.3.dev1/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:38:44.589614 streamlit_chat_handler-0.1.3.dev1/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev1/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-28 02:38:32.000000 streamlit_chat_handler-0.1.3.dev1/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.3.dev1/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:38:44.593614 streamlit_chat_handler-0.1.3.dev1/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:38:44.589614 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8281 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2056 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:38:44.593614 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.3.dev2/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.3.dev2/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev2/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-28 02:50:17.000000 streamlit_chat_handler-0.1.3.dev2/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.3.dev2/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8281 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2312 2024-04-28 02:51:11.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.1.3.dev1/LICENSE` & `streamlit_chat_handler-0.1.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev1/PKG-INFO` & `streamlit_chat_handler-0.1.3.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.3.dev1
+Version: 0.1.3.dev2
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.1.3.dev1/README.md` & `streamlit_chat_handler-0.1.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev1/examples/template.py` & `streamlit_chat_handler-0.1.3.dev2/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev1/pyproject.toml` & `streamlit_chat_handler-0.1.3.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
   {name = "Eduardo Messias de Morais", email = "emdemor415@gmail.com" },
 ]
-version = "0.1.3dev01"
+version = "0.1.3dev02"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 
     Methods:
         render: Render the chat element using the specified Streamlit widget.
     """
     role: Literal["user", "assistant"]
     type: str
     content: Any
+    parent: str | None = None
     args: List[Any] = Field(default_factory=list)
     kwargs: Dict[str, Any] = Field(default_factory=dict)
+    parent_args: List[Any] = Field(default_factory=list)
+    parent_kwargs: Dict[str, Any] = Field(default_factory=dict)
 
     def render(self):
         """Render the chat element using the specified Streamlit widget.
 
         This method dynamically calls a Streamlit function based on the `type` attribute, passing
         `content`, `args`, and `kwargs` to it. The rendering context is defined by the `role`, using
         Streamlit's `chat_message` method.
@@ -37,10 +40,11 @@
         Returns:
             The result of the Streamlit function call, typically a Streamlit component instance.
 
         Example:
             # Assuming an instance `chat_element` with type 'text':
             chat_element.render()  # This would render the content using `st.text()`.
         """
-        with st.chat_message(self.role):
-            response = getattr(st, self.type)(self.content, *self.args, **self.kwargs)
-            return response
+
+        chat_message = st.chat_message(self.role)
+        _parent = getattr(chat_message, self.parent)(*self.parent_args, **self.parent_kwargs) if self.parent else chat_message
+        return getattr(_parent, self.type)(self.content, *self.args, **self.kwargs)
```

### Comparing `streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.3.dev1
+Version: 0.1.3.dev2
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

