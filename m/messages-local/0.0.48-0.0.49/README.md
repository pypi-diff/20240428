# Comparing `tmp/messages-local-0.0.48.tar.gz` & `tmp/messages_local-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messages-local-0.0.48.tar", last modified: Fri Apr  5 09:47:49 2024, max compression
+gzip compressed data, was "messages_local-0.0.49.tar", last modified: Sun Apr 28 05:51:08 2024, max compression
```

## Comparing `messages-local-0.0.48.tar` & `messages_local-0.0.49.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:49.289157 messages-local-0.0.48/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-05 09:47:49.289157 messages-local-0.0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-05 09:47:09.000000 messages-local-0.0.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:49.285157 messages-local-0.0.48/messages_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:49.289157 messages-local-0.0.48/messages_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-05 09:47:09.000000 messages-local-0.0.48/messages_local/src/MessagesLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:09.000000 messages-local-0.0.48/messages_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:49.289157 messages-local-0.0.48/messages_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-05 09:47:09.000000 messages-local-0.0.48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:47:49.289157 messages-local-0.0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-05 09:47:09.000000 messages-local-0.0.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:51:08.363937 messages_local-0.0.49/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-28 05:51:08.363937 messages_local-0.0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-28 05:50:27.000000 messages_local-0.0.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:51:08.359937 messages_local-0.0.49/messages_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:51:08.363937 messages_local-0.0.49/messages_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-28 05:50:27.000000 messages_local-0.0.49/messages_local/src/MessagesLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:50:27.000000 messages_local-0.0.49/messages_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:51:08.363937 messages_local-0.0.49/messages_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-28 05:50:27.000000 messages_local-0.0.49/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:51:08.363937 messages_local-0.0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-28 05:50:27.000000 messages_local-0.0.49/setup.py
```

### Comparing `messages-local-0.0.48/PKG-INFO` & `messages_local-0.0.49/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.48
+Version: 0.0.49
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: message-local>=0.0.67
-Requires-Dist: sms-message-aws-sns-local>=0.0.8
-Requires-Dist: queue-worker-local>=0.0.12
-Requires-Dist: variable-local>=0.0.45
+Requires-Dist: item-local
+Requires-Dist: message-local>=0.0.118
+Requires-Dist: queue-worker-local>=0.0.37
 Requires-Dist: label-message-local>=0.0.2
 Requires-Dist: whatsapp-message-vonage-local
 Requires-Dist: whataspp-inforu-local
 Requires-Dist: email-message-aws-ses-local
+Requires-Dist: sms-message-aws-sns-local>=0.0.8
 
 messages-local
```

### Comparing `messages-local-0.0.48/README.md` & `messages_local-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `messages-local-0.0.48/messages_local/src/MessagesLocal.py` & `messages_local-0.0.49/messages_local/src/MessagesLocal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import os
 from datetime import datetime
 from typing import List
 
 from email_message_aws_ses_local.ses_email import EmailMessageAwsSesLocal
 from label_message_local.LabelConstants import MESSAGE_OUTBOX_LABEL_ID
 from label_message_local.LabelMessage import LabelsMessageLocal
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
@@ -15,41 +15,100 @@
 from message_local.MessageLocal import MessageLocal
 from message_local.Recipient import Recipient
 from queue_worker_local.queue_worker import QueueWorker
 from sms_message_aws_sns_local.sms_message_aws_sns import SmsMessageAwsSnsLocal
 from whataspp_inforu_local.WhatsAppMessageInforuLocal import WhatsAppMessageInforuLocal
 from whatsapp_message_vonage_local.vonage_whatsapp_message_local import WhatsAppMessageVonageLocal
 
-# Relative imports makes the worker confused, so we are not using constants.py
 # TODO Replace Magic Number with enum in a separate file in this repo which will be created by Sql2Code in the future
 MESSAGES_API_TYPE_ID = 5
+SEND_SYNC_ACTION_ID = 15
 MESSAGE_LOCAL_PYTHON_COMPONENT_ID = 259
 MESSAGE_LOCAL_PYTHON_COMPONENT_COMPONENT_NAME = 'messages-local-python-package'
 DEVELOPER_EMAIL = 'akiva.s@circ.zone'
 
 logger_object_message = {
     'component_id': MESSAGE_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': MESSAGE_LOCAL_PYTHON_COMPONENT_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': DEVELOPER_EMAIL
 }
 
 
+# SEND_SYNC_ACTION_ID = 15
+
+
 class MessagesLocal(metaclass=MetaLogger, object=logger_object_message):
     # no classes type, so the worker can init it with json.
     def __init__(self, default_original_body: str = None, default_subject: str = None,
-                 default_importance: int = MessageImportance.MEDIUM.value, recipients: List[dict] = None):
+                 default_importance: int = MessageImportance.MEDIUM.value, recipients: List[dict] = None,
+                 is_test_data: bool = False):
         self.recipients = recipients
 
         self.default_original_body = default_original_body
         self.default_subject = default_subject
         self.default_importance = default_importance
+        self.is_test_data = is_test_data
         self.label_crud = LabelsMessageLocal()
-        self.queue_worker = QueueWorker(schema_name="message", table_name="message_table",
-                                        view_name="message_outbox_view", id_column_name="message_id")
+        self.queue_worker = None  # This is called by the queue worker, so we can't init it here
+
+    def get_queue_worker(self):
+        self.queue_worker = self.queue_worker or QueueWorker(schema_name="message", table_name="message_table",
+                                                             view_name="message_outbox_view",
+                                                             id_column_name="message_id",
+                                                             is_test_data=self.is_test_data)
+        return self.queue_worker
+
+    @staticmethod
+    def __send(recipient: Recipient, message_local: MessageLocal, importance: MessageImportance,
+               campaign_id: int) -> list[int]:
+        message_recipient_channel = message_local.get_message_channel(recipient)
+        message_recipient_provider_id = message_local.get_message_provider_id(message_recipient_channel, recipient)
+        body = message_local.get_body_text_after_template_processing(recipient, message_recipient_channel)
+        if not body:
+            return []
+        init_kwargs = {}
+        send_kwargs = {"body": body, "recipients": [recipient],
+                       "compound_message_dict": message_local.get_compound_message_dict(message_recipient_channel)}
+        if (message_recipient_channel == MessageChannel.SMS and
+                message_recipient_provider_id == AWS_SNS_SMS_MESSAGE_PROVIDER_ID):
+            message_local.__class__ = SmsMessageAwsSnsLocal
+
+        elif message_recipient_channel == MessageChannel.WHATSAPP:
+            if message_recipient_provider_id == INFORU_MESSAGE_PROVIDER_ID:
+                message_local.__class__ = WhatsAppMessageInforuLocal
+            elif message_recipient_provider_id == VONAGE_MESSAGE_PROVIDER_ID:
+                message_local.__class__ = WhatsAppMessageVonageLocal
+            else:
+                raise Exception("Don't know which WhatsAppMessageLocal class to use "
+                                f"(provider_id: {message_recipient_provider_id})")
+        elif (message_recipient_channel == MessageChannel.EMAIL and
+              message_recipient_provider_id == AWS_SES_EMAIL_MESSAGE_PROVIDER_ID):
+            # Parameters to the function we call???
+            init_kwargs = {"subject": message_local.get_subject_text_after_template_processing(recipient)}
+            message_local.__class__ = EmailMessageAwsSesLocal
+
+        else:
+            # TODO We need to add to the message Recipient country, message plain text length after template,
+            #  message HTML length after template, number of attachments, attachments' types and sizes.
+            compound_message_dict = message_local.get_compound_message_dict()
+            data_json = {"channel_id": message_recipient_channel,
+                         "provider_id": message_recipient_provider_id,
+                         "recipient": recipient,
+                         "compound_message_dict": compound_message_dict,
+                         "compound_message_length": len(compound_message_dict),
+                         "importance": importance,
+                         "campaign_id": campaign_id
+                         }
+            error_message = "Don't know which MessageLocal class to use." + " Data: " + str(data_json)
+            # data_json will be printed anyway, as the meta logger prints the object & local variables
+            raise Exception(error_message)
+
+        message_local.__init__(**init_kwargs)
+        return message_local.send(**send_kwargs)
 
     # This method should be used by Queue Worker
     # Make sure send_sync has all the parameters in the function_parameters_json below
     def send_sync(self, message_id: int, campaign_id: int,
                   recipients: List[dict] = None,
                   cc_recipients: List[dict] = None,
                   bcc_recipients: List[dict] = None,
@@ -57,128 +116,99 @@
                   # TODO What is exactly the operational meaning of start_timestamp?
                   #  There is start_timestamp, when the message can be sent?
                   start_timestamp: datetime = datetime.now(),
                   importance: int = None,
                   requested_message_type: int = None,
                   sender_profile_id: int = None) -> None:
         """send method"""
-        details = {
-            "message_id": message_id,
-            "campaign_id": campaign_id,
-            "recipients": recipients,
-            "request_datetime": request_datetime,
-            "importance": importance,
-            "requested_message_type": requested_message_type
-        }
 
         recipients = Recipient.recipients_from_json(recipients or self.recipients)
         importance = MessageImportance(importance or self.default_importance)
         message_local = MessageLocal(message_id=message_id,
                                      original_body=self.default_original_body,
                                      original_subject=self.default_subject,
                                      campaign_id=campaign_id,
                                      recipients=recipients,
                                      importance=importance,
                                      api_type_id=MESSAGES_API_TYPE_ID,
-                                     sender_profile_id=sender_profile_id)
+                                     sender_profile_id=sender_profile_id,
+                                     is_test_data=self.is_test_data)
         for recipient in recipients:
-            init_kwargs = {}
-            send_kwargs = {}
-
-            message_recipient_channel = message_local.get_message_channel(recipient)
-            message_recipient_provider_id = message_local.get_message_provider_id(message_recipient_channel, recipient)
-            # profile_body_block = message_local.get_profile_block( recipient.get_profile_id(), message_recipient_channel, part="body")
-            body = message_local.get_body_after_text_template(recipient, message_recipient_channel)
-            if (message_recipient_channel == MessageChannel.SMS and
-                    message_recipient_provider_id == AWS_SNS_SMS_MESSAGE_PROVIDER_ID):
-                message_local.__class__ = SmsMessageAwsSnsLocal
-
-            elif message_recipient_channel == MessageChannel.WHATSAPP:
-                if message_recipient_provider_id == INFORU_MESSAGE_PROVIDER_ID:
-                    message_local.__class__ = WhatsAppMessageInforuLocal
-                elif message_recipient_provider_id == VONAGE_MESSAGE_PROVIDER_ID:
-                    message_local.__class__ = WhatsAppMessageVonageLocal
-                else:
-                    raise Exception("Don't know which WhatsAppMessageLocal class to use "
-                                    f"(provider_id: {message_recipient_provider_id})")
-            elif (message_recipient_channel == MessageChannel.EMAIL and
-                  message_recipient_provider_id == AWS_SES_EMAIL_MESSAGE_PROVIDER_ID):
-                # Parameters to the function we call???
-                init_kwargs = {"subject": message_local.get_profile_block(
-                    recipient.get_profile_id(), message_recipient_channel, part="subject").get("processedTemplate")}
-                message_local.__class__ = EmailMessageAwsSesLocal
-
-            else:
-                # TODO We need to add to the message Recipient country, message plain text length after template,
-                #  message HTML length after template, number of attachments, attachments' types and sizes.
-                compound_message_dict = message_local.get_compound_message_dict()
-                data_json = {"channel_id": message_recipient_channel,
-                             "provider_id": message_recipient_provider_id,
-                             "recipient": recipient,
-                             "compound_message_dict": compound_message_dict,
-                             "compound_message_length": len(compound_message_dict),
-                             "importance": importance,
-                             "campaign_id": campaign_id
-                             }
-                error_message = "Don't know which MessageLocal class to use." + " Data: " + str(data_json)
-                # data_json will be printed anyway, as the meta logger prints the object & local variables
-                raise Exception(error_message)
-
-            message_local.__init__(**init_kwargs)  # noqa, calling the son's init
-            # TODO: should we send multiple recipients outside this loop?
-            message_local.send(
-                body=body,
-                recipients=[recipient],
-                compound_message_dict=message_local.get_compound_message_dict(message_recipient_channel),
-                **send_kwargs)
+            self.__send(recipient, message_local, importance, campaign_id)
+            # TODO: should we send to multiple recipients outside this loop?
 
     # This method will push the messages to the queue in message_outbox_table
-    def send_scheduled(self, campaign_id: int, action_id: int,
+    def send_scheduled(self, campaign_id: int = None, message_template_id: int = None,
                        recipients: List[Recipient] = None,
                        cc_recipients: List[Recipient] = None,
                        bcc_recipients: List[Recipient] = None,
                        request_datetime: datetime = None,
                        importance: MessageImportance = None,
                        requested_message_type: MessageChannel = None,
                        start_timestamp: datetime = datetime.now(),
-                       sender_profile_id: int = None) -> list[int]:
+                       sender_profile_id: int = None,
+                       is_require_moderator: bool = True) -> list[int]:
         """The message will be sent any time between start_timestamp and end_timestamp
         For every bcc_recipient, a message will be pushed to the queue with the same parameters
         (message_id per bcc_recipient, or one if none provided)
         """
         importance = importance or MessageImportance(self.default_importance)
+        recipients = recipients or [Recipient(**recipient) for recipient in self.recipients]
         message_ids = []
         for bcc_recipient in bcc_recipients or [None]:
+            # Proccess template:
+            message_local = MessageLocal(original_body=self.default_original_body,
+                                         original_subject=self.default_subject,
+                                         campaign_id=campaign_id,
+                                         message_template_id=message_template_id,
+                                         recipients=recipients,
+                                         importance=importance,
+                                         api_type_id=MESSAGES_API_TYPE_ID,
+                                         sender_profile_id=sender_profile_id,
+                                         is_require_moderator=is_require_moderator,
+                                         is_test_data=self.is_test_data)
+            message_id = message_local.message_id
+            if not message_id:
+                raise Exception("Message ID is None")
             function_parameters_json = {
-                # Make sure send_sync accepts all these parameters + message_id
+                # Make sure send_sync accepts all these parameters.
+                "message_id": message_id,
                 "campaign_id": campaign_id,
-                "recipients": Recipient.recipients_to_json(recipients),
                 "cc_recipients": Recipient.recipients_to_json(cc_recipients),
                 "bcc_recipients": bcc_recipient.to_json() if bcc_recipient else None,
                 "request_datetime": str(request_datetime),
                 "importance": importance.value,
                 "requested_message_type": requested_message_type.value if requested_message_type else None,
                 "start_timestamp": str(start_timestamp),
                 "sender_profile_id": sender_profile_id
             }
 
             # Make sure MessagesLocal.__init__ accepts all these parameters
             class_parameters_json = {"default_original_body": self.default_original_body,
                                      "default_subject": self.default_subject,
                                      "default_importance": self.default_importance,
-                                     "recipients": self.recipients
+                                     "recipients": self.recipients,
+                                     "is_test_data": self.is_test_data
                                      }
 
-            message_id = self.queue_worker.push({"function_parameters_json": function_parameters_json,
-                                                 "class_parameters_json": class_parameters_json,
-                                                 "action_id": action_id})
-            function_parameters_json["message_id"] = message_id
-            # update function_parameters_json in the queue
-            self.queue_worker.update_by_id(id_column_value=message_id,
-                                           data_json={"function_parameters_json": json.dumps(function_parameters_json)})
+            self.get_queue_worker().push({"function_parameters_json": function_parameters_json,
+                                          "class_parameters_json": class_parameters_json,
+                                          "message_id": message_id,
+                                          "action_id": SEND_SYNC_ACTION_ID})
             try:
                 self.label_crud.add_label_message(label_id=MESSAGE_OUTBOX_LABEL_ID, message_id=message_id)
             except Exception as e:
                 self.logger.exception("Failed to add label to message", object=e)
             self.logger.info("Message pushed to the queue successfully", object={"message_id": message_id})
             message_ids.append(message_id)
         return message_ids
+
+    def send_sync_from_queue(self, total_missions: int = 1) -> bool:
+        if self.is_test_data:
+            working_directory = os.path.dirname(os.path.realpath(__file__))
+        else:
+            working_directory = None
+        return self.get_queue_worker().execute(install_packages=not self.is_test_data,
+                                               working_directory=working_directory,
+                                               total_missions=total_missions,
+                                               custom_condition="is_require_moderator = 1 AND is_moderator_approved = 1",
+                                               action_ids=(SEND_SYNC_ACTION_ID,))
```

### Comparing `messages-local-0.0.48/messages_local.egg-info/PKG-INFO` & `messages_local-0.0.49/messages_local.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.48
+Version: 0.0.49
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: message-local>=0.0.67
-Requires-Dist: sms-message-aws-sns-local>=0.0.8
-Requires-Dist: queue-worker-local>=0.0.12
-Requires-Dist: variable-local>=0.0.45
+Requires-Dist: item-local
+Requires-Dist: message-local>=0.0.118
+Requires-Dist: queue-worker-local>=0.0.37
 Requires-Dist: label-message-local>=0.0.2
 Requires-Dist: whatsapp-message-vonage-local
 Requires-Dist: whataspp-inforu-local
 Requires-Dist: email-message-aws-ses-local
+Requires-Dist: sms-message-aws-sns-local>=0.0.8
 
 messages-local
```

### Comparing `messages-local-0.0.48/setup.py` & `messages_local-0.0.49/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 PACKAGE_NAME = "messages-local"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.48', # https://pypi.org/project/messages-local
+    version='0.0.49', # https://pypi.org/project/messages-local
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/messages-local-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="messages-local",
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["message-local>=0.0.67",  # https://pypi.org/project/message-local/
-                      "sms-message-aws-sns-local>=0.0.8",  # https://pypi.org/project/sms-message-aws-sns-local/
-                      "queue-worker-local>=0.0.12",  # https://pypi.org/project/queue-worker-local/
-                      "variable-local>=0.0.45",  # https://pypi.org/project/variable-local/
+    install_requires=["item-local",
+                      "message-local>=0.0.118",
+                      "queue-worker-local>=0.0.37",
                       "label-message-local>=0.0.2",
                       "whatsapp-message-vonage-local",
                       "whataspp-inforu-local",
-                      "email-message-aws-ses-local"
+                      "email-message-aws-ses-local",
+                      "sms-message-aws-sns-local>=0.0.8",
                       ]
 )
```

