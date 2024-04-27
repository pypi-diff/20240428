# Comparing `tmp/variable_local-0.0.92.tar.gz` & `tmp/variable_local-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_local-0.0.92.tar", last modified: Fri Apr 26 13:08:01 2024, max compression
+gzip compressed data, was "variable_local-0.0.93.tar", last modified: Sat Apr 27 22:29:52 2024, max compression
```

## Comparing `variable_local-0.0.92.tar` & `variable_local-0.0.93.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:01.381364 variable_local-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 13:08:01.377364 variable_local-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-26 13:07:36.000000 variable_local-0.0.92/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-26 13:07:36.000000 variable_local-0.0.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:08:01.381364 variable_local-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-26 13:07:36.000000 variable_local-0.0.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:01.377364 variable_local-0.0.92/variable_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:01.377364 variable_local-0.0.92/variable_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:07:36.000000 variable_local-0.0.92/variable_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-26 13:07:36.000000 variable_local-0.0.92/variable_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-26 13:07:36.000000 variable_local-0.0.92/variable_local/src/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 13:07:36.000000 variable_local-0.0.92/variable_local/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-26 13:07:36.000000 variable_local-0.0.92/variable_local/src/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:01.377364 variable_local-0.0.92/variable_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 13:08:01.000000 variable_local-0.0.92/variable_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 13:08:01.000000 variable_local-0.0.92/variable_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:08:01.000000 variable_local-0.0.92/variable_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 13:08:01.000000 variable_local-0.0.92/variable_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 13:08:01.000000 variable_local-0.0.92/variable_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:52.604822 variable_local-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 22:29:52.604822 variable_local-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-27 22:29:28.000000 variable_local-0.0.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-27 22:29:28.000000 variable_local-0.0.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:29:52.604822 variable_local-0.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-27 22:29:28.000000 variable_local-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:52.600823 variable_local-0.0.93/variable_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:52.600823 variable_local-0.0.93/variable_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-27 22:29:28.000000 variable_local-0.0.93/variable_local/src/variables_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:29:52.600823 variable_local-0.0.93/variable_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 22:29:52.000000 variable_local-0.0.93/variable_local.egg-info/top_level.txt
```

### Comparing `variable_local-0.0.92/PKG-INFO` & `variable_local-0.0.93/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.92
+Version: 0.0.93
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `variable_local-0.0.92/README.md` & `variable_local-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.92/pyproject.toml` & `variable_local-0.0.93/pyproject.toml`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.92/setup.py` & `variable_local-0.0.93/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = 'variable-local'
 package_dir = PACKAGE_NAME.replace('-', '_')
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.92',  # https://pypi.org/project/variable-local
+    version='0.0.93',  # https://pypi.org/project/variable-local
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles variable Local/Remote Python",
     long_description="PyPI Package for Circles variable Local/Remote Python",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
```

### Comparing `variable_local-0.0.92/variable_local/src/constants.py` & `variable_local-0.0.93/variable_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.92/variable_local/src/template.py` & `variable_local-0.0.93/variable_local/src/template.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,107 +3,92 @@
 from datetime import datetime
 
 from language_local.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from smartlink_local.smartlink import SmartLinkLocal
 
 from .constants import variable_local_logger_init_object
-from .variable import VariablesLocal
+from .variables_local import VariablesLocal
 
 logger = Logger.create_logger(object=variable_local_logger_init_object)
 
 LEFT_BRACKETS = '{'
 RIGHT_BRACKETS = '}'
 
 
 class ReplaceFieldsWithValues:
-    def __init__(self, message, language: LangCode, variable: VariablesLocal):
+    def __init__(self, message, lang_code: LangCode, variables: VariablesLocal):
         self.message = message
-        self.language = language
-        self.variable = variable
+        self.lang_code = lang_code
+        self.variables = variables
         self.smartlink_local = None  # For performance reasons
 
-    # TODO: Not used anymore. Remove?
-    # Private method used by get_variable_names_and_chosen_option(self)
-    # def choose_option(self, message_index: int, first_param: str) -> (str, int):
-    #     """ Gets a message, an index of the first appearance of '|' , and the first parameter of the options
-    #         Returns:
-    #         1. One of the options randomly selected
-    #         2. The index of one char after the next '}'"""
-    #     logger.start(
-    #         object={'message_index': message_index, 'first_param': first_param})
-    #     list_of_params = [first_param]
-    #     while self.message[message_index] != '}':
-    #         next_param = ""
-    #         while self.message[message_index] != '|' and self.message[message_index] != '}':
-    #             next_param += self.message[message_index]
-    #             message_index += 1
-    #         list_of_params.append(next_param)
-    #         if self.message[message_index] != '}':
-    #             message_index += 1
-    #     random_index = random.randint(0, len(list_of_params) - 1)
-    #     random_option_selected, index = list_of_params[random_index], message_index + 1
-    #     logger.end(object={'random_option_selected': random_option_selected, 'index': index})
-    #     return random_option_selected, index
-
     @staticmethod
-    def get_smartlink_url(smartlink_identifier: str) -> str:
-        # TODO: move to url remote and improve
+    # TODO Shall it return Url type?
+    def get_smartlink_url_by_identifier(smartlink_identifier: str) -> str:
+        # TODO: move to url remote and improve:
+        #   In case of Brand=Circlez and Environment=play1, dvlp1 it should use www.circ.zone
+        #   In case of Brand=Circlez and Environment=prod1 it should use www.circlez.ai
         return f"www.circ.zone?a={smartlink_identifier}"
 
-    def get_smartlink(self, variable_name: str, **kwargs) -> str:
+    # TODO Shall we move this to smartink-local package?
+    # TODO Shall it return Url type?
+    def get_smartlink_url_by_variable_name_and_kwargs(self, variable_name: str, **kwargs) -> str:
         self.smartlink_local = self.smartlink_local or SmartLinkLocal()
-        smart_link_regex = r"smartLinkUrl\(smartLinkType=([0-9]+)\)"
-        smartlink_type_id = re.search(smart_link_regex, variable_name).group(1)
+        smartlink_regex = r"smartLinkUrl\(smartLinkType=([0-9]+)\)"
+        smartlink_type_id = re.search(smartlink_regex, variable_name).group(1)
         smartlink_details = self.smartlink_local.insert(smartlink_type_id=smartlink_type_id,
                                                         campaign_id=kwargs.get('campaign_id'),
                                                         from_recipient=kwargs.get('from_recipient'),
                                                         to_recipient=kwargs.get('to_recipient'))
-        return self.get_smartlink_url(smartlink_details['identifier'])
+        return self.get_smartlink_url_by_identifier(smartlink_details['identifier'])
 
-    def special_variable(self, variable_name: str, **kwargs) -> str:
+    # TODO variable_name: VariableName
+    def get_variable_value_by_variable_name_and_kwargs(self, variable_name: str, **kwargs) -> str:
         # TODO: use worker actions instead
         """Returns a special variable value by variable name"""
         logger.start(object={'variable_name': variable_name})
-        smart_link_regex = r"smartLinkUrl\(smartLinkType=([0-9]+)\)"
+        smartlink_regex = r"smartLinkUrl\(smartLinkType=([0-9]+)\)"
 
+        # TODO Shall we use SpecialVariableEnum.OTP for all special variables?
         if variable_name == 'otp':
             variable_value = ReplaceFieldsWithValues.generate_otp()
         elif variable_name == 'date_sortable':
-            variable_value = self.get_date_time()
-        elif re.match(smart_link_regex, variable_name):
-            variable_value = self.get_smartlink(variable_name, **kwargs)
+            variable_value = self.get_current_datetime_string()
+        elif re.match(smartlink_regex, variable_name):
+            variable_value = self.get_smartlink_url_by_variable_name_and_kwargs(variable_name, **kwargs)
         else:  # TODO: add more special variables
             logger.warning("Unknown special variable name `" + variable_name + "` in message: " + self.message,
                            object=kwargs)
             return ""
         logger.end(object={'variable_value': variable_value})
         return str(variable_value)
 
     @staticmethod
-    def generate_otp():  # TODO: move to the appropriate place
+    def generate_otp():  # TODO: move to the appropriate place. OTP Should be used in email, SMS ... Shall we create new package for it?
         """Generates a 6-digit OTP"""
         logger.start()
         otp = random.randint(100000, 999999)
         logger.end(object={'otp': otp})
         return otp
 
     @staticmethod
-    def get_date_time():
-        return datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    # TODO I think this can be moved to python-sdk
+    def get_current_datetime_string(strftime_format: str = "%Y-%m-%d %H:%M:%S") -> str:
+        return datetime.now().strftime(strftime_format)
 
     def get_variable_names_and_chosen_option(self, **kwargs) -> (list, str):
         """Returns:
             1. A list of all variable names that were inside curly braces of message
             2. A string that's a copy of the message but without the variable names inside curly braces,
             and a randomly chosen parameter out of each curly braces options:
             "Hello {First Name}, how are you {feeling|doing}?" --> "Hello {}, how are you doing?" 
         """
         logger.start(object={'kwargs': kwargs})
-        kwargs = kwargs.get('kwargs', kwargs)
+        kwargs = kwargs.get('kwargs', kwargs)  # in case someone sent the kwargs in a diff way
         variable_names_list = []
         message_without_variable_names = kwargs.get("message", self.message)
 
         pattern = re.compile(r'\${{[^}]*}}')  # ${{vraiable}}
         matches = pattern.findall(message_without_variable_names)
         for exact_match in matches:
             match = exact_match[3:-2].strip()  # remove '${{' and '}}'
@@ -114,22 +99,22 @@
                 message_without_variable_names = message_without_variable_names.replace(
                     exact_match, random_option, 1)
 
             elif match in kwargs:
                 message_without_variable_names = message_without_variable_names.replace(
                     exact_match, str(kwargs[match] if match in kwargs else kwargs[match]), 1)
 
-            elif match in self.variable.name2id_dict.keys():
+            elif match in self.variables.name2id_dict.keys():
                 # replace variable name with '{}' and add variable names to list
                 message_without_variable_names = message_without_variable_names.replace(exact_match, '{}', 1)
                 variable_names_list.append(match)
 
             else:
                 message_without_variable_names = message_without_variable_names.replace(
-                    exact_match, self.special_variable(match, **kwargs), 1)
+                    exact_match, self.get_variable_value_by_variable_name_and_kwargs(match, **kwargs), 1)
 
         return variable_names_list, message_without_variable_names
 
         # Old code:
         # For the following function to work the message must not have single '{' or '}'.
         # They should always come in pairs.
         #
@@ -174,15 +159,15 @@
             and a randomly chosen parameter out of each curly braces options:
             "Hello {First Name}, how are you {feeling|doing}?" --> "Hello {}, how are you doing?"
         """
         logger.start()
         variable_names_list, message_without_variable_names = self.get_variable_names_and_chosen_option(**kwargs)
         variable_value_list = []
         for variable_name in variable_names_list:
-            variable_id = self.variable.get_variable_id_by_variable_name(variable_name)
-            variable_value = self.variable.get_variable_value_by_variable_id(
-                variable_id=variable_id, lang_code=self.language, profile_id=profile_id)
+            variable_id = self.variables.get_variable_id_by_variable_name(variable_name)
+            variable_value = self.variables.get_variable_value_by_variable_id(
+                variable_id=variable_id, lang_code=self.lang_code, profile_id=profile_id)
             variable_value_list.append(variable_value)
 
         formatted_message = message_without_variable_names.format(*variable_value_list)
         logger.end(object={'formatted_message': formatted_message})
         return formatted_message
```

### Comparing `variable_local-0.0.92/variable_local/src/variable.py` & `variable_local-0.0.93/variable_local/src/variables_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         logger.end(object={'variable_value': variable_value})
         return variable_value
 
     def set_variable_value_by_variable_id(self, variable_id: int, variable_value: str, profile_id: int,
                                           state_id: int) -> None:
         logger.start(object={'variable_id': variable_id,
                              'variable_value': variable_value, 'profile_id': profile_id})
-        # TODO I believe we should keep more fields
+        # TODO I believe we should keep more fields  [like what?]
         data_json = {'variable_id': variable_id, 'variable_value_new': variable_value, 'profile_id': profile_id,
                      'state_id': state_id, 'record': '{}', 'message': '', 'path': '',
                      'component_id': VARIABLE_LOCAL_PYTHON_PACKAGE_COMPONENT_ID}
         self.insert(schema_name="logger", table_name='logger_table', data_json=data_json)
         logger.end()
 
     def get_variable_value_by_variable_id(self, variable_id: int, lang_code: LangCode, profile_id: int = None) -> str:
```

### Comparing `variable_local-0.0.92/variable_local.egg-info/PKG-INFO` & `variable_local-0.0.93/variable_local.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.92
+Version: 0.0.93
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

