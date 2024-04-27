# Comparing `tmp/dialog_workflow_local-0.0.97.tar.gz` & `tmp/dialog_workflow_local-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_workflow_local-0.0.97.tar", last modified: Mon Apr 15 17:46:41 2024, max compression
+gzip compressed data, was "dialog_workflow_local-0.0.98.tar", last modified: Sat Apr 27 23:36:07 2024, max compression
```

## Comparing `dialog_workflow_local-0.0.97.tar` & `dialog_workflow_local-0.0.98.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:41.704679 dialog_workflow_local-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 17:46:41.704679 dialog_workflow_local-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:41.700679 dialog_workflow_local-0.0.97/dialog_workflow_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:41.704679 dialog_workflow_local-0.0.97/dialog_workflow_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/dialog_workflow_local/src/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/dialog_workflow_local/src/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/dialog_workflow_local/src/ProfileContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/dialog_workflow_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29813 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/dialog_workflow_local/src/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/dialog_workflow_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:41.704679 dialog_workflow_local-0.0.97/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 17:46:41.000000 dialog_workflow_local-0.0.97/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-15 17:46:41.000000 dialog_workflow_local-0.0.97/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:46:41.000000 dialog_workflow_local-0.0.97/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 17:46:41.000000 dialog_workflow_local-0.0.97/dialog_workflow_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 17:46:41.000000 dialog_workflow_local-0.0.97/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:46:41.704679 dialog_workflow_local-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 17:46:13.000000 dialog_workflow_local-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:36:07.032055 dialog_workflow_local-0.0.98/dialog_workflow_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/dialog_workflow_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/ProfileContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/setup.py
```

### Comparing `dialog_workflow_local-0.0.97/PKG-INFO` & `dialog_workflow_local-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.97
+Version: 0.0.98
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog_workflow_local-0.0.97/README.md` & `dialog_workflow_local-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.97/dialog_workflow_local/src/Constants.py` & `dialog_workflow_local-0.0.98/dialog_workflow_local/src/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.97/dialog_workflow_local/src/DialogWorkflow.py` & `dialog_workflow_local-0.0.98/dialog_workflow_local/src/DialogWorkflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 
 from database_mysql_local.generic_crud import GenericCRUD
 from language_remote.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from message_local.CompoundMessage import CompoundMessage
 from user_context_remote.user_context import UserContext
-from variable_local.variable import VariablesLocal
+from variable_local.variables_local import VariablesLocal
 
 from .Constants import DIALOG_WORKFLOW_CODE_LOGGER_OBJECT
 from .ProfileContext import DialogWorkflowRecord
 from .action import Action
 from .utils import get_curr_state, update_profile_curr_state_in_db
 
 user = UserContext()
@@ -49,16 +49,17 @@
     logger.start(object={'profile_id': profile_id, 'incoming_message': incoming_message})
     profile_id = profile_id or user.get_effective_profile_id()
     # TODO Save the message using MessagesLocal (from DIALOG_WORKFLOW_PROFILE_ID, to UserContext.getEffectiveProfileId, ...)
     variables = VariablesLocal()
     profile_curr_state = get_curr_state(profile_id)
     lang_code = user.get_effective_profile_preferred_lang_code()
     got_response = incoming_message.strip() != ""  # This variable indicates if we must act now as we got a response from the user or as if we should send one to him
-    init_action = Action(incoming_message, profile_id,
-                         lang_code, profile_curr_state, variables)
+    init_action = Action(incoming_message=incoming_message, profile_id=profile_id,
+                         lang_code=lang_code, profile_curr_state=profile_curr_state,
+                         variables=variables)
     while True:
         dialog_workflow_record = get_dialog_workflow_record(init_action.profile_curr_state, lang_code)
         is_state_changed, outgoing_message = init_action.act(dialog_workflow_record, got_response)
         # TODO Save the message using MessagesLocal (from DIALOG_WORKFLOW_PROFILE_ID, to UserContext.getEffectiveProfileId, ...)
         if outgoing_message is not None:
             if not isinstance(outgoing_message, list):
                 outgoing_compound_message = CompoundMessage(body=outgoing_message).get_message_fields()
```

### Comparing `dialog_workflow_local-0.0.97/dialog_workflow_local/src/ProfileContext.py` & `dialog_workflow_local-0.0.98/dialog_workflow_local/src/ProfileContext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from database_mysql_local.generic_crud import GenericCRUD
+# from database_mysql_local.generic_crud import GenericCRUD
 from logger_local.LoggerLocal import Logger
-from variable_local.variable import VariablesLocal
+from variable_local.variables_local import VariablesLocal
 
 from .Constants import DIALOG_WORKFLOW_CODE_LOGGER_OBJECT
 from .utils import get_curr_state
 
 logger = Logger.create_logger(object=DIALOG_WORKFLOW_CODE_LOGGER_OBJECT)
 
 
-class ProfileContext(GenericCRUD, object):
+class ProfileContext(object):
     # TODO We should consider to take ProfileContact to a separate package or merge it with UserContext
     def __init__(self, profile_id):
-        super().__init__(default_schema_name='logger', default_table_name='logger_table')
+        # super().__init__(default_schema_name='logger', default_table_name='logger_table')
         self.profile_id = profile_id
         self.chosen_poll_options = {}
         self.curr_state_id = get_curr_state(self.profile_id)
         self.variables = VariablesLocal()
         self.groups = []
 
     def save_chosen_options(self, question_asked: str, variable_id: int, chosen_numbers_list: list,
```

### Comparing `dialog_workflow_local-0.0.97/dialog_workflow_local/src/action.py` & `dialog_workflow_local-0.0.98/dialog_workflow_local/src/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 # import requests
 # from AgeDetection import DetectAge
 from database_mysql_local.connector import Connector
 from language_remote.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from message_local.CompoundMessage import CompoundMessage
 from variable_local.template import ReplaceFieldsWithValues
-from variable_local.variable import VariablesLocal
+from variable_local.variables_local import VariablesLocal
 
 from .Constants import (COMMUNICATION_TYPE, DIALOG_WORKFLOW_CODE_LOGGER_OBJECT,
                         CommunicationTypeEnum, WorkflowActionEnum)
 from .ProfileContext import DialogWorkflowRecord, ProfileContext
 from .utils import (Group, generic_menu, get_child_nodes_of_current_state,
                     get_curr_state, process_message,
                     update_profile_curr_state_in_db)
 
 logger = Logger.create_logger(object=DIALOG_WORKFLOW_CODE_LOGGER_OBJECT)
 
 
 class Action(object):
-    def __init__(self, incoming_message: str, profile_id: int, language: LangCode, profile_curr_state: int,
+    def __init__(self, *, incoming_message: str, profile_id: int,
+                 lang_code: LangCode, profile_curr_state: int,
                  variables: VariablesLocal):
         self.incoming_message = incoming_message
         self.profile_id = profile_id
-        self.language = language
+        self.lang_code = lang_code
         self.variables = variables
         self.profile_curr_state = profile_curr_state
         self.accumulated_message = ""
         self.profile = ProfileContext(self.profile_id)
-        self.variable = VariablesLocal()
+        self.variables = VariablesLocal()
         self.record = None
         self.got_response = False
 
     def act(self, dialog_workflow_record: DialogWorkflowRecord, got_response: bool):
         """This function applies the action of the relevant record with the profile's current state id.
         Params:
             1. dialog_workflow_record: The current record from the dialog workflow state table that is applied.
@@ -98,15 +99,15 @@
 
     def text_message_action(self):
         """Prints the paramter1 message after formatting: 
         "Hello {First Name}, how are you {feeling|doing}?" --> "Hello Tal, how are you doing? """
         logger.start()
         message = self.record.parameter1
         replace_fields_with_values_class = ReplaceFieldsWithValues(
-            message, self.language, self.variable)
+            message=message, lang_code=self.lang_code, variables=self.variables)
         formatted_message = replace_fields_with_values_class.get_variable_values_and_chosen_option(self.profile_id)
         self.accumulated_message = self.accumulated_message + formatted_message + '~'
         text_message_act = False, None
         logger.end(object={'text_message_act': str(text_message_act)})
         return text_message_act
 
     # TODO Rename all those functions to question_workflow_action() - Add the word 'workflow'
@@ -148,15 +149,15 @@
                 logger.end(object={'question_act': question_act})
                 return question_act
             else:
                 question_act = False, None
                 logger.end(object={'question_act': question_act})
                 return question_act
         else:
-            self.variable.set_variable_value_by_variable_id(
+            self.variables.set_variable_value_by_variable_id(
                 self.record.variable1_id, self.incoming_message, self.profile_id, self.profile_curr_state)
             question_act = False, None
             logger.end(object={'question_act': question_act})
             return question_act
 
     def jump_action(self):
         """Jumps from one state to another."""
@@ -184,28 +185,28 @@
         return API_post
 
     def assign_variable_action(self):
         """Assigns a value to a given variable"""
         logger.start()
         parameter_value = self.record.parameter1
         variable_id = self.record.variable1_id
-        self.variable.set_variable_value_by_variable_id(
+        self.variables.set_variable_value_by_variable_id(
             variable_id, parameter_value, self.profile_id, self.profile_curr_state)
         assinged_variable_action = self.got_response, None
         logger.end(
             object={'assinged_variable_action': assinged_variable_action})
         return assinged_variable_action
 
     def increment_variable_action(self):
         """Increments a value to a given variable by the amount of the given paramter1"""
         logger.start()
         number_to_add = int(self.record.parameter1)
         variable_id = self.record.variable1_id
         current_variable_value = self.variables.get_variable_value_by_variable_id(
-            variable_id, self.language, self.profile_id)
+            variable_id, self.lang_code, self.profile_id)
         self.variables.set_variable_value_by_variable_id(variable_id, str(
             int(current_variable_value) + number_to_add), self.profile_id, self.profile_curr_state)
         incremented_variable_action = self.got_response, None
         logger.end(
             object={'incremented_variable_action': incremented_variable_action})
         return incremented_variable_action
 
@@ -215,17 +216,17 @@
         if isinstance(self.record.parameter1, str) and not self.record.parameter1.isdigit():
             error = f"Parameter1 must be a number (got {self.record.parameter1})"
             logger.error(error)
             raise ValueError(error)
         number_to_add = int(self.record.parameter1)
         variable_id = self.record.variable1_id
         current_variable_value = self.variables.get_variable_value_by_variable_id(
-            variable_id, self.language, self.profile_id)
-        self.variable.set_variable_value_by_variable_id(variable_id, str(int(current_variable_value) - number_to_add),
-                                                        self.profile_id, get_curr_state(self.profile_id))
+            variable_id, self.lang_code, self.profile_id)
+        self.variables.set_variable_value_by_variable_id(variable_id, str(int(current_variable_value) - number_to_add),
+                                                         self.profile_id, get_curr_state(self.profile_id))
         decremented_variable_action = False, None
         logger.end(
             object={'decremented_variable_action': decremented_variable_action})
         return decremented_variable_action
 
     """I have put this in remark right now because this action need to work with multiple profiles,
     But right now this change makes it difficult to do that. Will work on it later."""
@@ -411,15 +412,15 @@
     def present_and_choose_script(self):
         """Action for asking the user which workflo script he would like to run next and change the next state id according to his choice."""
         logger.start()
         connection = Connector.connect('dialog_workflow')
         cursor = connection.cursor(dictionary=True, buffered=True)
         cursor.execute(
             """SELECT d.start_state_id, dml.title FROM dialog_workflow_script_view AS d JOIN dialog_workflow_script_ml_view AS dml on dml.dialog_workflow_script_id=d.dialog_workflow_script_id WHERE dml.lang_code = %s""",
-            (self.language,))
+            (self.lang_code,))
         available_scripts_dict = cursor.fetchall()
         available_scripts = [script["title"]
                              for script in available_scripts_dict]
         outgoing_message = "Please choose your desired script out of the following:~"
         menu = generic_menu(available_scripts, self.got_response, self.incoming_message,
                             choose_one_option=True, outgoing_message=outgoing_message)
         if COMMUNICATION_TYPE == CommunicationTypeEnum.WEBSOCKET and not self.got_response:
```

### Comparing `dialog_workflow_local-0.0.97/dialog_workflow_local/src/utils.py` & `dialog_workflow_local-0.0.98/dialog_workflow_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.97/dialog_workflow_local.egg-info/PKG-INFO` & `dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.97
+Version: 0.0.98
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog_workflow_local-0.0.97/setup.py` & `dialog_workflow_local-0.0.98/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "dialog-workflow-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.97',  # https://pypi.org/project/dialog-workflow-local/
+    version='0.0.98',  # https://pypi.org/project/dialog-workflow-local/
     author="Circles",
     author_email="info@circle.life",
     description="PyPI Package for dialog workflow",
     long_description="This is a package for running the dialog workflow",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

