# Comparing `tmp/streamlit_chat_handler-0.1.2.tar.gz` & `tmp/streamlit_chat_handler-0.1.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.1.2.tar", last modified: Sun Apr 28 02:23:26 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.1.3.dev1.tar", last modified: Sun Apr 28 02:38:44 2024, max compression
```

## Comparing `streamlit_chat_handler-0.1.2.tar` & `streamlit_chat_handler-0.1.3.dev1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:23:26.893136 streamlit_chat_handler-0.1.2/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.2/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-28 02:23:26.893136 streamlit_chat_handler-0.1.2/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.2/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:23:26.889136 streamlit_chat_handler-0.1.2/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 01:47:34.000000 streamlit_chat_handler-0.1.2/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 02:07:47.000000 streamlit_chat_handler-0.1.2/examples/template_expander.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-28 02:23:04.000000 streamlit_chat_handler-0.1.2/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.2/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:23:26.893136 streamlit_chat_handler-0.1.2/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:23:26.889136 streamlit_chat_handler-0.1.2/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9805 2024-04-28 02:22:38.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2313 2024-04-28 01:41:17.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:23:26.893136 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:23:26.000000 streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:38:44.593614 streamlit_chat_handler-0.1.3.dev1/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.3.dev1/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:38:44.593614 streamlit_chat_handler-0.1.3.dev1/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.3.dev1/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:38:44.589614 streamlit_chat_handler-0.1.3.dev1/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev1/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-28 02:38:32.000000 streamlit_chat_handler-0.1.3.dev1/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.3.dev1/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:38:44.593614 streamlit_chat_handler-0.1.3.dev1/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:38:44.589614 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8281 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2056 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:38:44.593614 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:38:44.000000 streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.1.2/LICENSE` & `streamlit_chat_handler-0.1.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.2/PKG-INFO` & `streamlit_chat_handler-0.1.3.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.2
+Version: 0.1.3.dev1
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.1.2/README.md` & `streamlit_chat_handler-0.1.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.2/examples/template.py` & `streamlit_chat_handler-0.1.3.dev1/examples/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,24 @@
 
 from streamlit_chat_handler import StreamlitChatHandler
 
 
 if "session_id" not in st.session_state:
     st.session_state["session_id"] = str(uuid.uuid4())
 
+print(type(st.session_state))
+
 st.title("Template")
 
 chat_handler = StreamlitChatHandler(
     st.session_state,
     session_id=st.session_state["session_id"],
 ).render()
 
 if prompt := st.chat_input("Digite aqui..."):
     chat_handler.append(role="user", type="markdown", content=prompt, render=True)
 
     with st.spinner("Processando..."):
         sleep(1)
         chat_handler.append(
-            role="assistant",
-            type="markdown",
-            content=f'{chat_handler.step_counter} - resposta',
-            render=True,
+            role="assistant", type="markdown", content="resposta", render=True
         )
-
```

### Comparing `streamlit_chat_handler-0.1.2/pyproject.toml` & `streamlit_chat_handler-0.1.3.dev1/pyproject.toml`

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
-version = "0.1.2"
+version = "0.1.3dev01"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.1.2/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,36 +51,31 @@
         """Ensure only one instance per session_id."""
         if session_id not in cls._instances:
             instance = super(StreamlitChatHandler, cls).__new__(cls)
             cls._instances[session_id] = instance
             instance.session_state = session_state
             instance.session_id = session_id
             instance._init_session_state()
-            instance.step_counter = -1
         return cls._instances[session_id]
 
     def __init__(self, session_state: SessionStateProxy, session_id: str):
         """Initialize the instance with the session state and ID."""
         self.session_state = session_state
         self.session_id = session_id
         self._init_session_state()
         self.rendered_elements: OrderedDict[str, Any] | None = OrderedDict({})
-        self.step_counter += 1
 
     def append(
         self,
         role: Literal["user", "assistant"] = None,
         type: str = None,
         content: Any = None,
         index: str | None = None,
         render: bool = False,
         chat_element: StreamlitChatElement | None = None,
-        parent: str | None = None,
-        parent_args: Tuple[Any, ...] = (),
-        parent_kwargs: dict[str, Any] = {},
         *args,
         **kwargs,
     ) -> Any | None:
         """Append a new chat element to the session state.
 
         Args:
             role: The role of the message ('user' or 'assistant').
@@ -88,39 +83,40 @@
             content: The content of the message.
             index: Optional; a unique identifier for the chat element. Automatically generated if not provided.
             render: Optional; if True, the message is rendered immediately.
 
         Raises:
             ValueError: If an unsupported type is provided.
         """
-
-        index = self._set_index(index)
+        if index is None:
+            index = uuid.uuid4().hex
 
         if not chat_element:
-            chat_element = self._get_chat_element(
-                role,
-                type,
-                content,
-                parent,
-                parent_args,
-                parent_kwargs,
-                *args,
-                **kwargs,
+
+            args_were_passed = all(
+                [_check_argument(arg) for arg in (role, type, content)]
             )
 
+            if args_were_passed:
+                chat_element = StreamlitChatElement(
+                    role=role,
+                    type=type,
+                    content=content,
+                    args=args,
+                    kwargs=kwargs,
+                )
+            else:
+                raise ValueError("Missing required arguments for StreamlitChatElement.")
+
         self.session_state[self.elements_label][index] = chat_element
 
         if render:
             return chat_element.render()
         return self
 
-    def increment_step_counter(self) -> None:
-        """Finish the current step."""
-        self.step_counter += 1
-
     def render_last(self) -> None:
         """Render the last added chat element."""
         last_key, last_element = _get_last_item(self.session_state[self.elements_label])
         self.rendered_elements[last_key] = last_element.render()
 
     def render(self) -> "StreamlitChatHandler":
         """Render all chat elements in the session."""
@@ -130,55 +126,14 @@
         return self
 
     def _init_session_state(self) -> None:
         """Initialize the session state for storing chat elements if it doesn't already exist."""
         if self.elements_label not in self.session_state:
             self.session_state[self.elements_label] = OrderedDict({})
 
-    def _set_index(self, index: str | None) -> str:
-        """Set the index for the chat element.
-
-        Args:
-            index: The index to set.
-
-        Returns:
-            The set index.
-        """
-        if index is None:
-            index = uuid.uuid4().hex
-        index = f"{str(self.step_counter).zfill(6)}{index}"
-        return index
-
-    def _get_chat_element(
-        self,
-        role: Literal["user", "assistant"] = None,
-        type: str = None,
-        content: Any = None,
-        parent: str | None = None,
-        parent_args: Tuple[Any, ...] = (),
-        parent_kwargs: dict[str, Any] = {},
-        *args,
-        **kwargs,
-    ):
-        args_were_passed = all([_check_argument(arg) for arg in (role, type, content)])
-
-        if args_were_passed:
-            return StreamlitChatElement(
-                role=role,
-                type=type,
-                content=content,
-                parent=parent,
-                parent_args=parent_args,
-                parent_kwargs=parent_kwargs,
-                args=args,
-                kwargs=kwargs,
-            )
-        else:
-            raise ValueError("Missing required arguments for StreamlitChatElement.")
-
     @staticmethod
     def _render_elements(
         chat_element: StreamlitChatElement | OrderedDict[str, StreamlitChatElement]
     ) -> OrderedDict[str, Any]:
         """Render chat elements, handling both individual elements and collections.
 
         Args:
@@ -194,33 +149,25 @@
         chat_element_list = [v for v in chat_element.values()]
         element_groups = _group_elements_by_role(chat_element_list)
 
         response = OrderedDict({})
         count = 0
         for element_list in element_groups:
             role = element_list[0].role
-            chat_message = st.chat_message(role)
-            for element in element_list:
-                try:
-                    parent = (
-                        getattr(chat_message, element.parent)(
-                            *element.parent_args, **element.parent_kwargs
+            with st.chat_message(role):
+                for element in element_list:
+                    try:
+                        response[list(chat_element)[count]] = getattr(st, element.type)(
+                            element.content, *element.args, **element.kwargs
                         )
-                        if element.parent
-                        else chat_message
-                    )
-                    response[list(chat_element)[count]] = getattr(parent, element.type)(
-                        element.content, *element.args, **element.kwargs
-                    )
-                except Exception as err:
-                    logger.warning(
-                        f"Error rendering element {element} in key {list(chat_element)[count]}: {err}"
-                    )
-                count += 1
-
+                    except Exception as err:
+                        logger.warning(
+                            f"Error rendering element {element} in key {list(chat_element)[count]}: {err}"
+                        )
+                    count += 1
         return response
 
 
 def _get_last_item(ordered_dict: OrderedDict) -> Tuple[str, Any]:
     """Retrieve the last key-value pair from an OrderedDict.
 
     This function fetches the last key and its corresponding value from an OrderedDict
```

### Comparing `streamlit_chat_handler-0.1.2/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,19 +20,16 @@
 
     Methods:
         render: Render the chat element using the specified Streamlit widget.
     """
     role: Literal["user", "assistant"]
     type: str
     content: Any
-    parent: str | None = None
     args: List[Any] = Field(default_factory=list)
     kwargs: Dict[str, Any] = Field(default_factory=dict)
-    parent_args: List[Any] = Field(default_factory=list)
-    parent_kwargs: Dict[str, Any] = Field(default_factory=dict)
 
     def render(self):
         """Render the chat element using the specified Streamlit widget.
 
         This method dynamically calls a Streamlit function based on the `type` attribute, passing
         `content`, `args`, and `kwargs` to it. The rendering context is defined by the `role`, using
         Streamlit's `chat_message` method.
@@ -40,11 +37,10 @@
         Returns:
             The result of the Streamlit function call, typically a Streamlit component instance.
 
         Example:
             # Assuming an instance `chat_element` with type 'text':
             chat_element.render()  # This would render the content using `st.text()`.
         """
-
-        chat_message = st.chat_message(self.role)
-        _parent = getattr(chat_message, self.parent)(*self.parent_args, **self.parent_kwargs) if self.parent else chat_message
-        return getattr(_parent, self.type)(self.content, *self.args, **self.kwargs)
+        with st.chat_message(self.role):
+            response = getattr(st, self.type)(self.content, *self.args, **self.kwargs)
+            return response
```

### Comparing `streamlit_chat_handler-0.1.2/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.1.3.dev1/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.2
+Version: 0.1.3.dev1
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```
