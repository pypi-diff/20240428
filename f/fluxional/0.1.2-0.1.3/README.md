# Comparing `tmp/fluxional-0.1.2.tar.gz` & `tmp/fluxional-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxional-0.1.2.tar", max compression
+gzip compressed data, was "fluxional-0.1.3.tar", max compression
```

## Comparing `fluxional-0.1.2.tar` & `fluxional-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1059 2024-02-02 01:48:46.163715 fluxional-0.1.2/LICENSE
--rw-r--r--   0        0        0     3464 2024-04-22 20:27:58.523354 fluxional-0.1.2/README.md
--rw-r--r--   0        0        0      398 2024-04-06 03:52:15.283626 fluxional-0.1.2/fluxional/__init__.py
--rw-r--r--   0        0        0       85 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/__main__.py
--rw-r--r--   0        0        0     1429 2024-04-03 20:50:44.146193 fluxional-0.1.2/fluxional/cli/__init__.py
--rw-r--r--   0        0        0      397 2024-04-06 03:52:08.843621 fluxional-0.1.2/fluxional/core/__init__.py
--rw-r--r--   0        0        0    21257 2024-04-09 17:46:38.063914 fluxional-0.1.2/fluxional/core/app.py
--rw-r--r--   0        0        0     6976 2024-04-08 20:56:52.652758 fluxional-0.1.2/fluxional/core/core.py
--rw-r--r--   0        0        0     2927 2024-04-05 19:49:43.040843 fluxional-0.1.2/fluxional/core/events.py
--rw-r--r--   0        0        0    11708 2024-04-08 20:56:56.662776 fluxional-0.1.2/fluxional/core/handlers.py
--rw-r--r--   0        0        0        1 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/core/infrastructure/__init__.py
--rw-r--r--   0        0        0    19616 2024-04-07 16:13:07.372714 fluxional-0.1.2/fluxional/core/infrastructure/base.py
--rw-r--r--   0        0        0     7603 2024-04-07 16:07:21.912790 fluxional-0.1.2/fluxional/core/infrastructure/cdk.py
--rw-r--r--   0        0        0     9506 2024-04-07 16:08:36.732773 fluxional-0.1.2/fluxional/core/infrastructure/resources.py
--rw-r--r--   0        0        0      816 2024-04-07 16:02:37.282853 fluxional-0.1.2/fluxional/core/infrastructure/types.py
--rw-r--r--   0        0        0     5818 2024-04-08 20:56:58.162781 fluxional-0.1.2/fluxional/core/logic.py
--rw-r--r--   0        0        0     8343 2024-04-09 17:45:40.573927 fluxional-0.1.2/fluxional/core/settings.py
--rw-r--r--   0        0        0     4045 2024-04-08 20:57:01.432779 fluxional-0.1.2/fluxional/core/tools.py
--rw-r--r--   0        0        0     5158 2024-04-06 03:51:27.790814 fluxional-0.1.2/fluxional/core/types.py
--rw-r--r--   0        0        0       74 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/deployment/__init__.py
--rw-r--r--   0        0        0     1164 2024-02-02 02:20:07.747714 fluxional-0.1.2/fluxional/deployment/constants.py
--rw-r--r--   0        0        0    15256 2024-04-03 23:29:19.551745 fluxional-0.1.2/fluxional/deployment/engine.py
--rw-r--r--   0        0        0      345 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/deployment/exceptions.py
--rw-r--r--   0        0        0        1 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/deployment/utils.py
--rw-r--r--   0        0        0     3652 2024-04-05 19:50:15.280830 fluxional-0.1.2/fluxional/dev/__init__.py
--rw-r--r--   0        0        0     3003 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/dev/client.py
--rw-r--r--   0        0        0     3350 2024-04-03 20:50:44.146193 fluxional-0.1.2/fluxional/dev/runner.py
--rw-r--r--   0        0        0      326 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/py.typed
--rw-r--r--   0        0        0      461 2024-04-03 20:50:44.146193 fluxional-0.1.2/fluxional/types.py
--rw-r--r--   0        0        0      935 2024-02-02 01:50:49.633706 fluxional-0.1.2/fluxional/utils.py
--rw-r--r--   0        0        0     1151 2024-04-27 18:14:08.821086 fluxional-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 fluxional-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-02-02 01:48:46.163715 fluxional-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3464 2024-04-22 20:27:58.523354 fluxional-0.1.3/README.md
+-rw-r--r--   0        0        0      398 2024-04-06 03:52:15.283626 fluxional-0.1.3/fluxional/__init__.py
+-rw-r--r--   0        0        0       85 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/__main__.py
+-rw-r--r--   0        0        0     1429 2024-04-03 20:50:44.146193 fluxional-0.1.3/fluxional/cli/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-06 03:52:08.843621 fluxional-0.1.3/fluxional/core/__init__.py
+-rw-r--r--   0        0        0    21402 2024-04-28 00:09:22.534943 fluxional-0.1.3/fluxional/core/app.py
+-rw-r--r--   0        0        0     6976 2024-04-08 20:56:52.652758 fluxional-0.1.3/fluxional/core/core.py
+-rw-r--r--   0        0        0     2927 2024-04-05 19:49:43.040843 fluxional-0.1.3/fluxional/core/events.py
+-rw-r--r--   0        0        0    11708 2024-04-08 20:56:56.662776 fluxional-0.1.3/fluxional/core/handlers.py
+-rw-r--r--   0        0        0        1 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/core/infrastructure/__init__.py
+-rw-r--r--   0        0        0    19676 2024-04-28 00:09:59.214928 fluxional-0.1.3/fluxional/core/infrastructure/base.py
+-rw-r--r--   0        0        0     7699 2024-04-28 00:07:24.364991 fluxional-0.1.3/fluxional/core/infrastructure/cdk.py
+-rw-r--r--   0        0        0     9554 2024-04-28 00:08:07.284974 fluxional-0.1.3/fluxional/core/infrastructure/resources.py
+-rw-r--r--   0        0        0      816 2024-04-07 16:02:37.282853 fluxional-0.1.3/fluxional/core/infrastructure/types.py
+-rw-r--r--   0        0        0     5818 2024-04-08 20:56:58.162781 fluxional-0.1.3/fluxional/core/logic.py
+-rw-r--r--   0        0        0     8343 2024-04-09 17:45:40.573927 fluxional-0.1.3/fluxional/core/settings.py
+-rw-r--r--   0        0        0     4045 2024-04-08 20:57:01.432779 fluxional-0.1.3/fluxional/core/tools.py
+-rw-r--r--   0        0        0     5158 2024-04-06 03:51:27.790814 fluxional-0.1.3/fluxional/core/types.py
+-rw-r--r--   0        0        0       74 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/deployment/__init__.py
+-rw-r--r--   0        0        0     1164 2024-02-02 02:20:07.747714 fluxional-0.1.3/fluxional/deployment/constants.py
+-rw-r--r--   0        0        0    15256 2024-04-03 23:29:19.551745 fluxional-0.1.3/fluxional/deployment/engine.py
+-rw-r--r--   0        0        0      345 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/deployment/exceptions.py
+-rw-r--r--   0        0        0        1 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/deployment/utils.py
+-rw-r--r--   0        0        0     3652 2024-04-05 19:50:15.280830 fluxional-0.1.3/fluxional/dev/__init__.py
+-rw-r--r--   0        0        0     3003 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/dev/client.py
+-rw-r--r--   0        0        0     3350 2024-04-03 20:50:44.146193 fluxional-0.1.3/fluxional/dev/runner.py
+-rw-r--r--   0        0        0      326 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/py.typed
+-rw-r--r--   0        0        0      461 2024-04-03 20:50:44.146193 fluxional-0.1.3/fluxional/types.py
+-rw-r--r--   0        0        0      935 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/utils.py
+-rw-r--r--   0        0        0     1151 2024-04-28 00:19:41.426103 fluxional-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 fluxional-0.1.3/PKG-INFO
```

### Comparing `fluxional-0.1.2/LICENSE` & `fluxional-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/README.md` & `fluxional-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/cli/__init__.py` & `fluxional-0.1.3/fluxional/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/core/app.py` & `fluxional-0.1.3/fluxional/core/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,14 +317,16 @@
             existing_resource=False,
             **asdict(self.settings.build.event_lambda),
         )
 
         queue = SqsQueue(
             id=self.settings.system.default_event_queue_id,
             queue_name=f"{stack_name}_{self.settings.system.default_event_queue_id}",
+            # Visibility Timeout cannot be less than the lambda timeout
+            visibility_timeout=self.settings.build.event_lambda.timeout,
         )
 
         queue.permissions.append(
             LambdaPermission(
                 resource_id=event_lambda.id,
                 resource_type=event_lambda.resource_type,
                 allow_invoke=True,
```

### Comparing `fluxional-0.1.2/fluxional/core/core.py` & `fluxional-0.1.3/fluxional/core/core.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/core/events.py` & `fluxional-0.1.3/fluxional/core/events.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/core/handlers.py` & `fluxional-0.1.3/fluxional/core/handlers.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/core/infrastructure/base.py` & `fluxional-0.1.3/fluxional/core/infrastructure/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         return self._app
 
     def add_sqs_queue(self, resource: SqsQueue):
         queue = add_sqs_queue_to_stack(
             stack=self,
             id=resource.id,
             queue_name=resource.queue_name,
+            visibility_timeout=resource.visibility_timeout,
         )
 
         if resource.permissions:
             for k in resource.permissions:
                 if ResourceTypeGuard.is_lambda_permission(k):
 
                     if k.allow_invoke:
```

### Comparing `fluxional-0.1.2/fluxional/core/infrastructure/cdk.py` & `fluxional-0.1.3/fluxional/core/infrastructure/cdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,17 +287,20 @@
     )
 
     setattr(stack, id, bucket)
 
     return bucket
 
 
-def add_sqs_queue_to_stack(*, stack: Stack, id: str, queue_name: str) -> aws_sqs.Queue:
+def add_sqs_queue_to_stack(
+    *, stack: Stack, id: str, queue_name: str, visibility_timeout: int
+) -> aws_sqs.Queue:
     queue = aws_sqs.Queue(
         stack,
         id,
         queue_name=queue_name,
+        visibility_timeout=Duration.seconds(visibility_timeout),
     )
 
     setattr(stack, id, queue)
 
     return queue
```

### Comparing `fluxional-0.1.2/fluxional/core/infrastructure/resources.py` & `fluxional-0.1.3/fluxional/core/infrastructure/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     display_name: str
     resource_type: Literal["sns_topic"] = field(default="sns_topic")
 
 
 @dataclass(kw_only=True)
 class SqsQueue(_ResourceT):
     queue_name: str
+    visibility_timeout: int = field(default=30)
     resource_type: Literal["sqs_queue"] = field(default="sqs_queue")
 
 
 @dataclass(kw_only=True)
 class S3Bucket(_ResourceT):
     bucket_name: str
     remove_on_delete: bool = field(default=True)
```

### Comparing `fluxional-0.1.2/fluxional/core/infrastructure/types.py` & `fluxional-0.1.3/fluxional/core/infrastructure/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/core/logic.py` & `fluxional-0.1.3/fluxional/core/logic.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/core/settings.py` & `fluxional-0.1.3/fluxional/core/settings.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/core/tools.py` & `fluxional-0.1.3/fluxional/core/tools.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/core/types.py` & `fluxional-0.1.3/fluxional/core/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/deployment/constants.py` & `fluxional-0.1.3/fluxional/deployment/constants.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/deployment/engine.py` & `fluxional-0.1.3/fluxional/deployment/engine.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/dev/__init__.py` & `fluxional-0.1.3/fluxional/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/dev/client.py` & `fluxional-0.1.3/fluxional/dev/client.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/dev/runner.py` & `fluxional-0.1.3/fluxional/dev/runner.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/fluxional/utils.py` & `fluxional-0.1.3/fluxional/utils.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.2/pyproject.toml` & `fluxional-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluxional"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["fluxional"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.10 < 4.0"
```

### Comparing `fluxional-0.1.2/PKG-INFO` & `fluxional-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxional
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: fluxional
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

