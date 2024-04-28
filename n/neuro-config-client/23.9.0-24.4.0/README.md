# Comparing `tmp/neuro-config-client-23.9.0.tar.gz` & `tmp/neuro_config_client-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-config-client-23.9.0.tar", last modified: Fri Sep  8 11:05:11 2023, max compression
+gzip compressed data, was "neuro_config_client-24.4.0.tar", last modified: Sun Apr 28 15:16:31 2024, max compression
```

## Comparing `neuro-config-client-23.9.0.tar` & `neuro_config_client-24.4.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 11:05:11.323180 neuro-config-client-23.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 11:05:11.319180 neuro-config-client-23.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.github/actionlint-matcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 11:05:11.319180 neuro-config-client-23.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.github/workflows/remove-automerge.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.github/workflows/setup-automerge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-09-08 11:05:11.323180 neuro-config-client-23.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 11:05:11.323180 neuro-config-client-23.9.0/neuro_config_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/neuro_config_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/neuro_config_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13272 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/neuro_config_client/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    41847 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/neuro_config_client/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/neuro_config_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 11:05:11.323180 neuro-config-client-23.9.0/neuro_config_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-09-08 11:05:11.000000 neuro-config-client-23.9.0/neuro_config_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-09-08 11:05:11.000000 neuro-config-client-23.9.0/neuro_config_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 11:05:11.000000 neuro-config-client-23.9.0/neuro_config_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 11:05:11.000000 neuro-config-client-23.9.0/neuro_config_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-08 11:05:11.000000 neuro-config-client-23.9.0/neuro_config_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-08 11:05:11.000000 neuro-config-client-23.9.0/neuro_config_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-09-08 11:05:11.323180 neuro-config-client-23.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 11:05:11.323180 neuro-config-client-23.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    70730 2023-09-08 11:04:55.000000 neuro-config-client-23.9.0/tests/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:16:31.884713 neuro_config_client-24.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:16:31.884713 neuro_config_client-24.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.github/actionlint-matcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:16:31.884713 neuro_config_client-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.github/workflows/remove-automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.github/workflows/setup-automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-28 15:16:31.884713 neuro_config_client-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:16:31.884713 neuro_config_client-24.4.0/neuro_config_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/neuro_config_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/neuro_config_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/neuro_config_client/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42249 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/neuro_config_client/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/neuro_config_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:16:31.884713 neuro_config_client-24.4.0/neuro_config_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-28 15:16:31.000000 neuro_config_client-24.4.0/neuro_config_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-28 15:16:31.000000 neuro_config_client-24.4.0/neuro_config_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:16:31.000000 neuro_config_client-24.4.0/neuro_config_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:16:31.000000 neuro_config_client-24.4.0/neuro_config_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-28 15:16:31.000000 neuro_config_client-24.4.0/neuro_config_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-28 15:16:31.000000 neuro_config_client-24.4.0/neuro_config_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-28 15:16:31.888713 neuro_config_client-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:16:31.884713 neuro_config_client-24.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    70849 2024-04-28 15:16:21.000000 neuro_config_client-24.4.0/tests/test_factories.py
```

### Comparing `neuro-config-client-23.9.0/.github/workflows/ci.yaml` & `neuro_config_client-24.4.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `neuro-config-client-23.9.0/.github/workflows/remove-automerge.yml` & `neuro_config_client-24.4.0/.github/workflows/remove-automerge.yml`

 * *Files identical despite different names*

### Comparing `neuro-config-client-23.9.0/.github/workflows/setup-automerge.yml` & `neuro_config_client-24.4.0/.github/workflows/setup-automerge.yml`

 * *Files identical despite different names*

### Comparing `neuro-config-client-23.9.0/.gitignore` & `neuro_config_client-24.4.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 .ipynb_checkpoints
 
 # IPython
 profile_default/
 ipython_config.py
 
 # pyenv
-.python-version
+# .python-version
 
 # pipenv
 #   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
 #   However, in case of collaboration, if having platform-specific dependencies or dependencies
 #   having no cross-platform support, pipenv may install dependencies that don't work, or not
 #   install all needed dependencies.
 #Pipfile.lock
```

### Comparing `neuro-config-client-23.9.0/.pre-commit-config.yaml` & `neuro_config_client-24.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `neuro-config-client-23.9.0/LICENSE` & `neuro_config_client-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-config-client-23.9.0/PKG-INFO` & `neuro_config_client-24.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-config-client
-Version: 23.9.0
+Version: 24.4.0
 Summary: Internal client for Neu.ro config service
 Home-page: https://github.com/neuro-inc/neuro-config-client
 License: Apache 2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `neuro-config-client-23.9.0/neuro_config_client/__init__.py` & `neuro_config_client-24.4.0/neuro_config_client/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-config-client-23.9.0/neuro_config_client/client.py` & `neuro_config_client-24.4.0/neuro_config_client/client.py`

 * *Files identical despite different names*

### Comparing `neuro-config-client-23.9.0/neuro_config_client/entities.py` & `neuro_config_client-24.4.0/neuro_config_client/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,16 +459,17 @@
 
 @dataclass(frozen=True)
 class ResourcePreset:
     name: str
     credits_per_hour: Decimal
     cpu: float
     memory: int
-    gpu: int | None = None
-    gpu_model: str | None = None
+    nvidia_gpu: int | None = None
+    amd_gpu: int | None = None
+    intel_gpu: int | None = None
     tpu: TPUPreset | None = None
     scheduler_enabled: bool = False
     preemptible_node: bool = False
     resource_affinity: Sequence[str] = ()
     is_external_job: bool = False
 
 
@@ -479,16 +480,17 @@
     max_size: int = 1
     idle_size: int = 0
     cpu: float = 1.0
     available_cpu: float = 1.0
     memory: int = 2**30  # 1gb
     available_memory: int = 2**30  # 1gb
     disk_size: int = 150 * 2**30  # 150gb
-    gpu: int | None = None
-    gpu_model: str | None = None
+    nvidia_gpu: int | None = None
+    amd_gpu: int | None = None
+    intel_gpu: int | None = None
     price: Decimal = Decimal()
     currency: str | None = None
     tpu: TPUResource | None = None
     is_preemptible: bool = False
 
 
 @dataclass(frozen=True)
```

### Comparing `neuro-config-client-23.9.0/neuro_config_client/factories.py` & `neuro_config_client-24.4.0/neuro_config_client/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,16 +258,17 @@
             idle_size=payload.get("idle_size", ResourcePoolType.idle_size),
             cpu=payload.get("cpu", ResourcePoolType.cpu),
             available_cpu=payload.get("available_cpu", ResourcePoolType.available_cpu),
             memory=payload.get("memory", ResourcePoolType.memory),
             available_memory=payload.get(
                 "available_memory", ResourcePoolType.available_memory
             ),
-            gpu=payload.get("gpu"),
-            gpu_model=payload.get("gpu_model"),
+            nvidia_gpu=payload.get("nvidia_gpu"),
+            amd_gpu=payload.get("amd_gpu"),
+            intel_gpu=payload.get("intel_gpu"),
             price=Decimal(payload.get("price", ResourcePoolType.price)),
             currency=payload.get("currency"),
             tpu=tpu,
             is_preemptible=payload.get(
                 "is_preemptible", ResourcePoolType.is_preemptible
             ),
         )
@@ -284,16 +285,17 @@
         if payload.get("tpu"):
             tpu = self.create_tpu_preset(payload["tpu"])
         return ResourcePreset(
             name=payload["name"],
             credits_per_hour=Decimal(payload["credits_per_hour"]),
             cpu=payload["cpu"],
             memory=payload["memory"],
-            gpu=payload.get("gpu"),
-            gpu_model=payload.get("gpu_model"),
+            nvidia_gpu=payload.get("nvidia_gpu"),
+            amd_gpu=payload.get("amd_gpu"),
+            intel_gpu=payload.get("intel_gpu"),
             tpu=tpu,
             scheduler_enabled=payload.get("scheduler_enabled", False),
             preemptible_node=payload.get("preemptible_node", False),
             resource_affinity=payload.get("resource_affinity", ()),
             is_external_job=payload.get("is_external_job", False),
         )
 
@@ -824,17 +826,17 @@
             result["allow_job_priority"] = orchestrator.allow_job_priority
         if orchestrator.resource_pool_types:
             result["resource_pool_types"] = [
                 self.create_resource_pool_type(r)
                 for r in orchestrator.resource_pool_types
             ]
         if orchestrator.job_internal_hostname_template:
-            result[
-                "job_internal_hostname_template"
-            ] = orchestrator.job_internal_hostname_template
+            result["job_internal_hostname_template"] = (
+                orchestrator.job_internal_hostname_template
+            )
         if orchestrator.resource_presets:
             result["resource_presets"] = [
                 self.create_resource_preset(preset)
                 for preset in orchestrator.resource_presets
             ]
         if orchestrator.pre_pull_images:
             result["pre_pull_images"] = orchestrator.pre_pull_images
@@ -856,17 +858,20 @@
             "idle_size": resource_pool_type.idle_size,
             "cpu": resource_pool_type.cpu,
             "available_cpu": resource_pool_type.available_cpu,
             "memory": resource_pool_type.memory,
             "available_memory": resource_pool_type.available_memory,
             "disk_size": resource_pool_type.disk_size,
         }
-        if resource_pool_type.gpu:
-            result["gpu"] = resource_pool_type.gpu
-            result["gpu_model"] = resource_pool_type.gpu_model
+        if resource_pool_type.nvidia_gpu:
+            result["nvidia_gpu"] = resource_pool_type.nvidia_gpu
+        if resource_pool_type.amd_gpu:
+            result["amd_gpu"] = resource_pool_type.amd_gpu
+        if resource_pool_type.intel_gpu:
+            result["intel_gpu"] = resource_pool_type.intel_gpu
         if resource_pool_type.currency:
             result["price"] = str(resource_pool_type.price)
             result["currency"] = resource_pool_type.currency
         if resource_pool_type.tpu:
             result["tpu"] = cls.create_tpu_resource(resource_pool_type.tpu)
         return result
 
@@ -882,17 +887,20 @@
     def create_resource_preset(cls, preset: ResourcePreset) -> dict[str, Any]:
         result: dict[str, Any] = {
             "name": preset.name,
             "credits_per_hour": str(preset.credits_per_hour),
             "cpu": preset.cpu,
             "memory": preset.memory,
         }
-        if preset.gpu:
-            result["gpu"] = preset.gpu
-            result["gpu_model"] = preset.gpu_model
+        if preset.nvidia_gpu:
+            result["nvidia_gpu"] = preset.nvidia_gpu
+        if preset.amd_gpu:
+            result["amd_gpu"] = preset.amd_gpu
+        if preset.intel_gpu:
+            result["intel_gpu"] = preset.intel_gpu
         if preset.tpu:
             result["tpu"] = cls._create_tpu_preset(preset.tpu)
         if preset.scheduler_enabled:
             result["scheduler_enabled"] = preset.scheduler_enabled
         if preset.preemptible_node:
             result["preemptible_node"] = preset.preemptible_node
         return result
```

### Comparing `neuro-config-client-23.9.0/neuro_config_client.egg-info/PKG-INFO` & `neuro_config_client-24.4.0/neuro_config_client.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-config-client
-Version: 23.9.0
+Version: 24.4.0
 Summary: Internal client for Neu.ro config service
 Home-page: https://github.com/neuro-inc/neuro-config-client
 License: Apache 2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `neuro-config-client-23.9.0/neuro_config_client.egg-info/SOURCES.txt` & `neuro_config_client-24.4.0/neuro_config_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
+.python-version
 LICENSE
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/actionlint-matcher.json
```

### Comparing `neuro-config-client-23.9.0/setup.cfg` & `neuro_config_client-24.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `neuro-config-client-23.9.0/tests/test_factories.py` & `neuro_config_client-24.4.0/tests/test_factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,16 +274,17 @@
                 "max_size": 2,
                 "idle_size": 1,
                 "cpu": 4.0,
                 "available_cpu": 3.0,
                 "memory": 12 * 1024,
                 "available_memory": 10 * 1024,
                 "disk_size": 700,
-                "gpu": 1,
-                "gpu_model": "nvidia-tesla-k80",
+                "nvidia_gpu": 1,
+                "amd_gpu": 2,
+                "intel_gpu": 3,
                 "tpu": {
                     "ipv4_cidr_block": "10.0.0.0/8",
                     "types": ["tpu"],
                     "software_versions": ["v1"],
                 },
                 "is_preemptible": True,
                 "price": "1.0",
@@ -296,16 +297,17 @@
             min_size=1,
             max_size=2,
             idle_size=1,
             cpu=4.0,
             available_cpu=3.0,
             memory=12 * 1024,
             available_memory=10 * 1024,
-            gpu=1,
-            gpu_model="nvidia-tesla-k80",
+            nvidia_gpu=1,
+            amd_gpu=2,
+            intel_gpu=3,
             tpu=mock.ANY,
             is_preemptible=True,
             price=Decimal("1.0"),
             currency="USD",
         )
 
     def test_create_empty_resource_pool_type(self, factory: EntityFactory) -> None:
@@ -336,45 +338,45 @@
             }
         )
 
         assert result == ResourcePreset(
             name="cpu-small", credits_per_hour=Decimal("10"), cpu=4.0, memory=1024
         )
 
-    def test_create_resource_preset_custom(
-        self, factory: EntityFactory
-    ) -> None:
+    def test_create_resource_preset_custom(self, factory: EntityFactory) -> None:
         result = factory.create_resource_preset(
             {
                 "name": "gpu-small",
                 "credits_per_hour": "10",
                 "cpu": 4.0,
                 "memory": 12288,
-                "gpu": 1,
-                "gpu_model": "nvidia-tesla-k80",
+                "nvidia_gpu": 1,
+                "amd_gpu": 2,
+                "intel_gpu": 3,
                 "tpu": {"type": "tpu", "software_version": "v1"},
                 "scheduler_enabled": True,
                 "preemptible_node": True,
                 "resource_affinity": ["gpu-k80"],
                 "is_external_job": True,
             }
         )
 
         assert result == ResourcePreset(
             name="gpu-small",
             credits_per_hour=Decimal("10"),
             cpu=4.0,
             memory=12288,
-            gpu=1,
-            gpu_model="nvidia-tesla-k80",
+            nvidia_gpu=1,
+            amd_gpu=2,
+            intel_gpu=3,
             tpu=TPUPreset(type="tpu", software_version="v1"),
             scheduler_enabled=True,
             preemptible_node=True,
             resource_affinity=["gpu-k80"],
-            is_external_job=True
+            is_external_job=True,
         )
 
     def test_create_storage(self, factory: EntityFactory) -> None:
         result = factory.create_storage({"url": "https://storage-dev.neu.ro"})
 
         assert result == StorageConfig(
             url=URL("https://storage-dev.neu.ro"), volumes=[]
@@ -1542,16 +1544,17 @@
                 max_size=2,
                 idle_size=1,
                 cpu=4.0,
                 available_cpu=3.0,
                 memory=12 * 1024,
                 available_memory=10 * 1024,
                 disk_size=700,
-                gpu=1,
-                gpu_model="nvidia-tesla-k80",
+                nvidia_gpu=1,
+                amd_gpu=2,
+                intel_gpu=3,
                 tpu=TPUResource(
                     ipv4_cidr_block="10.0.0.0/8",
                     types=["tpu"],
                     software_versions=["v1"],
                 ),
                 is_preemptible=True,
                 price=Decimal("1.0"),
@@ -1565,16 +1568,17 @@
             "max_size": 2,
             "idle_size": 1,
             "cpu": 4.0,
             "available_cpu": 3.0,
             "memory": 12 * 1024,
             "available_memory": 10 * 1024,
             "disk_size": 700,
-            "gpu": 1,
-            "gpu_model": "nvidia-tesla-k80",
+            "nvidia_gpu": 1,
+            "amd_gpu": 2,
+            "intel_gpu": 3,
             "tpu": {
                 "ipv4_cidr_block": "10.0.0.0/8",
                 "types": ["tpu"],
                 "software_versions": ["v1"],
             },
             "is_preemptible": True,
             "price": "1.0",
@@ -1632,30 +1636,32 @@
     ) -> None:
         result = factory.create_resource_preset(
             ResourcePreset(
                 name="gpu-small",
                 credits_per_hour=Decimal("10"),
                 cpu=4.0,
                 memory=12288,
-                gpu=1,
-                gpu_model="nvidia-tesla-k80",
+                nvidia_gpu=1,
+                amd_gpu=2,
+                intel_gpu=3,
                 tpu=TPUPreset(type="tpu", software_version="v1"),
                 scheduler_enabled=True,
                 preemptible_node=True,
                 resource_affinity=["gpu-k80"],
             )
         )
 
         assert result == {
             "name": "gpu-small",
             "credits_per_hour": "10",
             "cpu": 4.0,
             "memory": 12288,
-            "gpu": 1,
-            "gpu_model": "nvidia-tesla-k80",
+            "nvidia_gpu": 1,
+            "amd_gpu": 2,
+            "intel_gpu": 3,
             "tpu": {"type": "tpu", "software_version": "v1"},
             "scheduler_enabled": True,
             "preemptible_node": True,
         }
 
     def test_create_storage(self, factory: PayloadFactory) -> None:
         result = factory.create_storage(
```

