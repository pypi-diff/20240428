# Comparing `tmp/streamlit_chat_handler-0.1.3.dev2.tar.gz` & `tmp/streamlit_chat_handler-0.1.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.1.3.dev2.tar", last modified: Sun Apr 28 02:51:47 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.1.3.dev3.tar", last modified: Sun Apr 28 02:59:18 2024, max compression
```

## Comparing `streamlit_chat_handler-0.1.3.dev2.tar` & `streamlit_chat_handler-0.1.3.dev3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.3.dev2/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.3.dev2/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev2/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-28 02:50:17.000000 streamlit_chat_handler-0.1.3.dev2/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.3.dev2/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8281 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2312 2024-04-28 02:51:11.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:51:47.609328 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:51:47.000000 streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:59:18.612244 streamlit_chat_handler-0.1.3.dev3/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.3.dev3/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:59:18.612244 streamlit_chat_handler-0.1.3.dev3/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.3.dev3/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:59:18.608244 streamlit_chat_handler-0.1.3.dev3/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev3/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-28 02:59:11.000000 streamlit_chat_handler-0.1.3.dev3/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.3.dev3/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:59:18.612244 streamlit_chat_handler-0.1.3.dev3/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:59:18.608244 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9804 2024-04-28 02:57:51.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2312 2024-04-28 02:51:11.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:59:18.608244 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.1.3.dev2/LICENSE` & `streamlit_chat_handler-0.1.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev2/PKG-INFO` & `streamlit_chat_handler-0.1.3.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.3.dev2
+Version: 0.1.3.dev3
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.1.3.dev2/README.md` & `streamlit_chat_handler-0.1.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev2/examples/template.py` & `streamlit_chat_handler-0.1.3.dev3/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev2/pyproject.toml` & `streamlit_chat_handler-0.1.3.dev3/pyproject.toml`

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
-version = "0.1.3dev02"
+version = "0.1.3dev03"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,31 +51,36 @@
         """Ensure only one instance per session_id."""
         if session_id not in cls._instances:
             instance = super(StreamlitChatHandler, cls).__new__(cls)
             cls._instances[session_id] = instance
             instance.session_state = session_state
             instance.session_id = session_id
             instance._init_session_state()
+            instance.step_counter = -1
         return cls._instances[session_id]
 
     def __init__(self, session_state: SessionStateProxy, session_id: str):
         """Initialize the instance with the session state and ID."""
         self.session_state = session_state
         self.session_id = session_id
         self._init_session_state()
         self.rendered_elements: OrderedDict[str, Any] | None = OrderedDict({})
+        self.step_counter += 1
 
     def append(
         self,
         role: Literal["user", "assistant"] = None,
         type: str = None,
         content: Any = None,
         index: str | None = None,
         render: bool = False,
         chat_element: StreamlitChatElement | None = None,
+        parent: str | None = None,
+        parent_args: Tuple[Any, ...] = (),
+        parent_kwargs: dict[str, Any] = {},
         *args,
         **kwargs,
     ) -> Any | None:
         """Append a new chat element to the session state.
 
         Args:
             role: The role of the message ('user' or 'assistant').
@@ -83,40 +88,39 @@
             content: The content of the message.
             index: Optional; a unique identifier for the chat element. Automatically generated if not provided.
             render: Optional; if True, the message is rendered immediately.
 
         Raises:
             ValueError: If an unsupported type is provided.
         """
-        if index is None:
-            index = uuid.uuid4().hex
 
-        if not chat_element:
+        index = self._set_index(index)
 
-            args_were_passed = all(
-                [_check_argument(arg) for arg in (role, type, content)]
+        if not chat_element:
+            chat_element = self._get_chat_element(
+                role,
+                type,
+                content,
+                parent,
+                parent_args,
+                parent_kwargs,
+                *args,
+                **kwargs,
             )
 
-            if args_were_passed:
-                chat_element = StreamlitChatElement(
-                    role=role,
-                    type=type,
-                    content=content,
-                    args=args,
-                    kwargs=kwargs,
-                )
-            else:
-                raise ValueError("Missing required arguments for StreamlitChatElement.")
-
         self.session_state[self.elements_label][index] = chat_element
 
         if render:
             return chat_element.render()
         return self
 
+    def increment_step_counter(self) -> None:
+        """Finish the current step."""
+        self.step_counter += 1
+
     def render_last(self) -> None:
         """Render the last added chat element."""
         last_key, last_element = _get_last_item(self.session_state[self.elements_label])
         self.rendered_elements[last_key] = last_element.render()
 
     def render(self) -> "StreamlitChatHandler":
         """Render all chat elements in the session."""
@@ -126,14 +130,55 @@
         return self
 
     def _init_session_state(self) -> None:
         """Initialize the session state for storing chat elements if it doesn't already exist."""
         if self.elements_label not in self.session_state:
             self.session_state[self.elements_label] = OrderedDict({})
 
+    def _set_index(self, index: str | None) -> str:
+        """Set the index for the chat element.
+
+        Args:
+            index: The index to set.
+
+        Returns:
+            The set index.
+        """
+        if index is None:
+            index = uuid.uuid4().hex
+        index = f"{str(self.step_counter).zfill(6)}{index}"
+        return index
+
+    def _get_chat_element(
+        self,
+        role: Literal["user", "assistant"] = None,
+        type: str = None,
+        content: Any = None,
+        parent: str | None = None,
+        parent_args: Tuple[Any, ...] = (),
+        parent_kwargs: dict[str, Any] = {},
+        *args,
+        **kwargs,
+    ):
+        args_were_passed = all([_check_argument(arg) for arg in (role, type, content)])
+
+        if args_were_passed:
+            return StreamlitChatElement(
+                role=role,
+                type=type,
+                content=content,
+                parent=parent,
+                parent_args=parent_args,
+                parent_kwargs=parent_kwargs,
+                args=args,
+                kwargs=kwargs,
+            )
+        else:
+            raise ValueError("Missing required arguments for StreamlitChatElement.")
+
     @staticmethod
     def _render_elements(
         chat_element: StreamlitChatElement | OrderedDict[str, StreamlitChatElement]
     ) -> OrderedDict[str, Any]:
         """Render chat elements, handling both individual elements and collections.
 
         Args:
@@ -149,25 +194,33 @@
         chat_element_list = [v for v in chat_element.values()]
         element_groups = _group_elements_by_role(chat_element_list)
 
         response = OrderedDict({})
         count = 0
         for element_list in element_groups:
             role = element_list[0].role
-            with st.chat_message(role):
-                for element in element_list:
-                    try:
-                        response[list(chat_element)[count]] = getattr(st, element.type)(
-                            element.content, *element.args, **element.kwargs
-                        )
-                    except Exception as err:
-                        logger.warning(
-                            f"Error rendering element {element} in key {list(chat_element)[count]}: {err}"
+            chat_message = st.chat_message(role)
+            for element in element_list:
+                try:
+                    parent = (
+                        getattr(chat_message, element.parent)(
+                            *element.parent_args, **element.parent_kwargs
                         )
-                    count += 1
+                        if element.parent
+                        else chat_message
+                    )
+                    response[list(chat_element)[count]] = getattr(parent, element.type)(
+                        element.content, *element.args, **element.kwargs
+                    )
+                except Exception as err:
+                    logger.warning(
+                        f"Error rendering element {element} in key {list(chat_element)[count]}: {err}"
+                    )
+                count += 1
+
         return response
 
 
 def _get_last_item(ordered_dict: OrderedDict) -> Tuple[str, Any]:
     """Retrieve the last key-value pair from an OrderedDict.
 
     This function fetches the last key and its corresponding value from an OrderedDict
@@ -222,8 +275,8 @@
 
     return grouped_elements
 
 
 def _check_argument(argument: Any):
     if argument is not None:
         return True
-    return False
+    return False
```

### Comparing `streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/types.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev2/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.3.dev2
+Version: 0.1.3.dev3
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

