# Comparing `tmp/pulumiverse_vercel-1.3.0.tar.gz` & `tmp/pulumiverse_vercel-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_vercel-1.3.0.tar", last modified: Wed Mar 13 12:24:48 2024, max compression
+gzip compressed data, was "pulumiverse_vercel-1.9.0.tar", last modified: Sun Apr 28 08:52:16 2024, max compression
```

## Comparing `pulumiverse_vercel-1.3.0.tar` & `pulumiverse_vercel-1.9.0.tar`

### file list

```diff
@@ -1,36 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:24:48.205062 pulumiverse_vercel-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-13 12:24:48.205062 pulumiverse_vercel-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:24:48.205062 pulumiverse_vercel-1.3.0/pulumiverse_vercel/
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18724 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:24:48.205062 pulumiverse_vercel-1.3.0/pulumiverse_vercel/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    30241 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_prebuilt_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_project_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_shared_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    25629 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    61417 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    20437 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/project_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    24186 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/project_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel/shared_environment_variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:24:48.205062 pulumiverse_vercel-1.3.0/pulumiverse_vercel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-13 12:24:48.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-13 12:24:48.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:24:48.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:24:48.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-13 12:24:48.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-13 12:24:48.000000 pulumiverse_vercel-1.3.0/pulumiverse_vercel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 12:24:48.205062 pulumiverse_vercel-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-13 12:24:47.000000 pulumiverse_vercel-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:52:16.169277 pulumiverse_vercel-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-28 08:52:16.169277 pulumiverse_vercel-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:52:16.169277 pulumiverse_vercel-1.9.0/pulumiverse_vercel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:52:16.169277 pulumiverse_vercel-1.9.0/pulumiverse_vercel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30241 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33228 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/edge_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/edge_config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17514 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/edge_config_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_edge_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_edge_config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_edge_config_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_endpoint_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_log_drain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_prebuilt_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23333 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_project_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_shared_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34183 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/log_drain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30376 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95435 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20281 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/project_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24670 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/project_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19661 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/shared_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17349 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:52:16.169277 pulumiverse_vercel-1.9.0/pulumiverse_vercel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-28 08:52:16.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-28 08:52:16.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 08:52:16.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 08:52:16.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-28 08:52:16.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-28 08:52:16.000000 pulumiverse_vercel-1.9.0/pulumiverse_vercel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 08:52:16.169277 pulumiverse_vercel-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-28 08:52:15.000000 pulumiverse_vercel-1.9.0/setup.py
```

### Comparing `pulumiverse_vercel-1.3.0/PKG-INFO` & `pulumiverse_vercel-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_vercel
-Version: 1.3.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-vercel
 Keywords: pulumi vercel category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_vercel-1.3.0/README.md` & `pulumiverse_vercel-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/__init__.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,25 +4,36 @@
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .alias import *
 from .deployment import *
 from .dns_record import *
+from .edge_config import *
+from .edge_config_schema import *
+from .edge_config_token import *
 from .get_alias import *
+from .get_deployment import *
+from .get_edge_config import *
+from .get_edge_config_schema import *
+from .get_edge_config_token import *
+from .get_endpoint_verification import *
 from .get_file import *
+from .get_log_drain import *
 from .get_prebuilt_project import *
 from .get_project import *
 from .get_project_directory import *
 from .get_shared_environment_variable import *
+from .log_drain import *
 from .project import *
 from .project_domain import *
 from .project_environment_variable import *
 from .provider import *
 from .shared_environment_variable import *
+from .webhook import *
 from ._inputs import *
 from . import outputs
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
     import pulumiverse_vercel.config as __config
     config = __config
@@ -54,14 +65,46 @@
   "fqn": "pulumiverse_vercel",
   "classes": {
    "vercel:index/dnsRecord:DnsRecord": "DnsRecord"
   }
  },
  {
   "pkg": "vercel",
+  "mod": "index/edgeConfig",
+  "fqn": "pulumiverse_vercel",
+  "classes": {
+   "vercel:index/edgeConfig:EdgeConfig": "EdgeConfig"
+  }
+ },
+ {
+  "pkg": "vercel",
+  "mod": "index/edgeConfigSchema",
+  "fqn": "pulumiverse_vercel",
+  "classes": {
+   "vercel:index/edgeConfigSchema:EdgeConfigSchema": "EdgeConfigSchema"
+  }
+ },
+ {
+  "pkg": "vercel",
+  "mod": "index/edgeConfigToken",
+  "fqn": "pulumiverse_vercel",
+  "classes": {
+   "vercel:index/edgeConfigToken:EdgeConfigToken": "EdgeConfigToken"
+  }
+ },
+ {
+  "pkg": "vercel",
+  "mod": "index/logDrain",
+  "fqn": "pulumiverse_vercel",
+  "classes": {
+   "vercel:index/logDrain:LogDrain": "LogDrain"
+  }
+ },
+ {
+  "pkg": "vercel",
   "mod": "index/project",
   "fqn": "pulumiverse_vercel",
   "classes": {
    "vercel:index/project:Project": "Project"
   }
  },
  {
@@ -83,14 +126,22 @@
  {
   "pkg": "vercel",
   "mod": "index/sharedEnvironmentVariable",
   "fqn": "pulumiverse_vercel",
   "classes": {
    "vercel:index/sharedEnvironmentVariable:SharedEnvironmentVariable": "SharedEnvironmentVariable"
   }
+ },
+ {
+  "pkg": "vercel",
+  "mod": "index/webhook",
+  "fqn": "pulumiverse_vercel",
+  "classes": {
+   "vercel:index/webhook:Webhook": "Webhook"
+  }
  }
 ]
 """,
     resource_packages="""
 [
  {
   "pkg": "vercel",
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/_inputs.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/_inputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'DeploymentProjectSettingsArgs',
     'DnsRecordSrvArgs',
     'ProjectEnvironmentArgs',
+    'ProjectGitCommentsArgs',
     'ProjectGitRepositoryArgs',
+    'ProjectGitRepositoryDeployHookArgs',
     'ProjectPasswordProtectionArgs',
     'ProjectTrustedIpsArgs',
     'ProjectTrustedIpsAddressArgs',
     'ProjectVercelAuthenticationArgs',
 ]
 
 @pulumi.input_type
@@ -271,26 +273,67 @@
 
     @sensitive.setter
     def sensitive(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sensitive", value)
 
 
 @pulumi.input_type
+class ProjectGitCommentsArgs:
+    def __init__(__self__, *,
+                 on_commit: pulumi.Input[bool],
+                 on_pull_request: pulumi.Input[bool]):
+        """
+        :param pulumi.Input[bool] on_commit: Whether Commit comments are enabled
+        :param pulumi.Input[bool] on_pull_request: Whether Pull Request comments are enabled
+        """
+        pulumi.set(__self__, "on_commit", on_commit)
+        pulumi.set(__self__, "on_pull_request", on_pull_request)
+
+    @property
+    @pulumi.getter(name="onCommit")
+    def on_commit(self) -> pulumi.Input[bool]:
+        """
+        Whether Commit comments are enabled
+        """
+        return pulumi.get(self, "on_commit")
+
+    @on_commit.setter
+    def on_commit(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "on_commit", value)
+
+    @property
+    @pulumi.getter(name="onPullRequest")
+    def on_pull_request(self) -> pulumi.Input[bool]:
+        """
+        Whether Pull Request comments are enabled
+        """
+        return pulumi.get(self, "on_pull_request")
+
+    @on_pull_request.setter
+    def on_pull_request(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "on_pull_request", value)
+
+
+@pulumi.input_type
 class ProjectGitRepositoryArgs:
     def __init__(__self__, *,
                  repo: pulumi.Input[str],
                  type: pulumi.Input[str],
+                 deploy_hooks: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectGitRepositoryDeployHookArgs']]]] = None,
                  production_branch: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] repo: The name of the git repository. For example: `vercel/next.js`.
         :param pulumi.Input[str] type: The git provider of the repository. Must be either `github`, `gitlab`, or `bitbucket`.
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectGitRepositoryDeployHookArgs']]] deploy_hooks: Deploy hooks are unique URLs that allow you to trigger a deployment of a given branch. See https://vercel.com/docs/deployments/deploy-hooks for full information.
         :param pulumi.Input[str] production_branch: By default, every commit pushed to the main branch will trigger a Production Deployment instead of the usual Preview Deployment. You can switch to a different branch here.
         """
         pulumi.set(__self__, "repo", repo)
         pulumi.set(__self__, "type", type)
+        if deploy_hooks is not None:
+            pulumi.set(__self__, "deploy_hooks", deploy_hooks)
         if production_branch is not None:
             pulumi.set(__self__, "production_branch", production_branch)
 
     @property
     @pulumi.getter
     def repo(self) -> pulumi.Input[str]:
         """
@@ -311,27 +354,108 @@
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
+    @pulumi.getter(name="deployHooks")
+    def deploy_hooks(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectGitRepositoryDeployHookArgs']]]]:
+        """
+        Deploy hooks are unique URLs that allow you to trigger a deployment of a given branch. See https://vercel.com/docs/deployments/deploy-hooks for full information.
+        """
+        return pulumi.get(self, "deploy_hooks")
+
+    @deploy_hooks.setter
+    def deploy_hooks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectGitRepositoryDeployHookArgs']]]]):
+        pulumi.set(self, "deploy_hooks", value)
+
+    @property
     @pulumi.getter(name="productionBranch")
     def production_branch(self) -> Optional[pulumi.Input[str]]:
         """
         By default, every commit pushed to the main branch will trigger a Production Deployment instead of the usual Preview Deployment. You can switch to a different branch here.
         """
         return pulumi.get(self, "production_branch")
 
     @production_branch.setter
     def production_branch(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "production_branch", value)
 
 
 @pulumi.input_type
+class ProjectGitRepositoryDeployHookArgs:
+    def __init__(__self__, *,
+                 name: pulumi.Input[str],
+                 ref: pulumi.Input[str],
+                 id: Optional[pulumi.Input[str]] = None,
+                 url: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] name: The name of the deploy hook.
+        :param pulumi.Input[str] ref: The branch or commit hash that should be deployed.
+        :param pulumi.Input[str] id: The ID of the deploy hook.
+        :param pulumi.Input[str] url: A URL that, when a POST request is made to, will trigger a new deployment.
+        """
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "ref", ref)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if url is not None:
+            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        The name of the deploy hook.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def ref(self) -> pulumi.Input[str]:
+        """
+        The branch or commit hash that should be deployed.
+        """
+        return pulumi.get(self, "ref")
+
+    @ref.setter
+    def ref(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ref", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the deploy hook.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def url(self) -> Optional[pulumi.Input[str]]:
+        """
+        A URL that, when a POST request is made to, will trigger a new deployment.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "url", value)
+
+
+@pulumi.input_type
 class ProjectPasswordProtectionArgs:
     def __init__(__self__, *,
                  deployment_type: pulumi.Input[str],
                  password: pulumi.Input[str]):
         """
         :param pulumi.Input[str] deployment_type: The deployment environment to protect. Must be one of `standard_protection`, `all_deployments`, or `only_preview_deployments`.
         :param pulumi.Input[str] password: The password that visitors must enter to gain access to your Preview Deployments. Drift detection is not possible for this field.
@@ -419,26 +543,26 @@
 
 @pulumi.input_type
 class ProjectTrustedIpsAddressArgs:
     def __init__(__self__, *,
                  value: pulumi.Input[str],
                  note: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] value: The value of the Environment Variable.
+        :param pulumi.Input[str] value: The address or CIDR range that can access deployments.
         :param pulumi.Input[str] note: A description for the value
         """
         pulumi.set(__self__, "value", value)
         if note is not None:
             pulumi.set(__self__, "note", note)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
         """
-        The value of the Environment Variable.
+        The address or CIDR range that can access deployments.
         """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/_utilities.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/alias.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/alias.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/config/vars.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/deployment.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/deployment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/dns_record.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/dns_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,14 @@
 
         > The `value` field must be specified on all DNS record types except `SRV`. When using `SRV` DNS records, the `srv` field must be specified.
 
         For more detailed information, please see the [Vercel documentation](https://vercel.com/docs/concepts/projects/custom-domains#dns-records)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         dns_record = vercel.DnsRecord("dnsRecord",
             domain="example.com",
             ttl=60,
@@ -417,33 +416,36 @@
             type="SRV")
         txt = vercel.DnsRecord("txt",
             domain="example.com",
             ttl=60,
             type="TXT",
             value="some text value")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         If importing into a personal account, or with a team configured on
 
         the provider, simply use the record id.
 
-        - record_id is hard to find, but can be taken from the network tab, inside developer tools, on the domains page.
+        - record_id can be taken from the network tab inside developer tools, while you are on the domains page,
+
+        or can be queried from the Vercel API directly (https://vercel.com/docs/rest-api/endpoints/dns#list-existing-dns-records).
 
         ```sh
         $ pulumi import vercel:index/dnsRecord:DnsRecord example rec_xxxxxxxxxxxxxxxxxxxxxxxxxxxx
         ```
 
         Alternatively, you can import via the team_id and record_id.
 
         - team_id can be found in the team `settings` tab in the Vercel UI.
 
-        - record_id is hard to find, but can be taken from the network tab, inside developer tools, on the domains page.
+        - record_id can be taken from the network tab inside developer tools, while you are on the domains page,
+
+        or can be queried from the Vercel API directly (https://vercel.com/docs/rest-api/endpoints/dns#list-existing-dns-records).
 
         ```sh
         $ pulumi import vercel:index/dnsRecord:DnsRecord example team_xxxxxxxxxxxxxxxxxxxxxxxx/rec_xxxxxxxxxxxxxxxxxxxxxxxxxxxx
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -477,15 +479,14 @@
 
         > The `value` field must be specified on all DNS record types except `SRV`. When using `SRV` DNS records, the `srv` field must be specified.
 
         For more detailed information, please see the [Vercel documentation](https://vercel.com/docs/concepts/projects/custom-domains#dns-records)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         dns_record = vercel.DnsRecord("dnsRecord",
             domain="example.com",
             ttl=60,
@@ -529,33 +530,36 @@
             type="SRV")
         txt = vercel.DnsRecord("txt",
             domain="example.com",
             ttl=60,
             type="TXT",
             value="some text value")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         If importing into a personal account, or with a team configured on
 
         the provider, simply use the record id.
 
-        - record_id is hard to find, but can be taken from the network tab, inside developer tools, on the domains page.
+        - record_id can be taken from the network tab inside developer tools, while you are on the domains page,
+
+        or can be queried from the Vercel API directly (https://vercel.com/docs/rest-api/endpoints/dns#list-existing-dns-records).
 
         ```sh
         $ pulumi import vercel:index/dnsRecord:DnsRecord example rec_xxxxxxxxxxxxxxxxxxxxxxxxxxxx
         ```
 
         Alternatively, you can import via the team_id and record_id.
 
         - team_id can be found in the team `settings` tab in the Vercel UI.
 
-        - record_id is hard to find, but can be taken from the network tab, inside developer tools, on the domains page.
+        - record_id can be taken from the network tab inside developer tools, while you are on the domains page,
+
+        or can be queried from the Vercel API directly (https://vercel.com/docs/rest-api/endpoints/dns#list-existing-dns-records).
 
         ```sh
         $ pulumi import vercel:index/dnsRecord:DnsRecord example team_xxxxxxxxxxxxxxxxxxxxxxxx/rec_xxxxxxxxxxxxxxxxxxxxxxxxxxxx
         ```
 
         :param str resource_name: The name of the resource.
         :param DnsRecordArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_alias.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_alias.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_file.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,27 +70,25 @@
     """
     Provides information about a file on disk.
 
     This will read a single file, providing metadata for use with a `Deployment`.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vercel as vercel
     import pulumiverse_vercel as vercel
 
     example_file = vercel.get_file(path="index.html")
     example_project = vercel.get_project(name="my-project")
     example_deployment = vercel.Deployment("exampleDeployment",
         project_id=example_project.id,
         files=example_file.file)
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     __args__['path'] = path
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('vercel:index/getFile:getFile', __args__, opts=opts, typ=GetFileResult).value
 
     return AwaitableGetFileResult(
@@ -105,22 +103,20 @@
     """
     Provides information about a file on disk.
 
     This will read a single file, providing metadata for use with a `Deployment`.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vercel as vercel
     import pulumiverse_vercel as vercel
 
     example_file = vercel.get_file(path="index.html")
     example_project = vercel.get_project(name="my-project")
     example_deployment = vercel.Deployment("exampleDeployment",
         project_id=example_project.id,
         files=example_file.file)
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_prebuilt_project.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_prebuilt_project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_project.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_project.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,27 +18,51 @@
 ]
 
 @pulumi.output_type
 class GetProjectResult:
     """
     A collection of values returned by getProject.
     """
-    def __init__(__self__, build_command=None, dev_command=None, environments=None, framework=None, git_repository=None, id=None, ignore_command=None, install_command=None, name=None, output_directory=None, password_protection=None, public_source=None, root_directory=None, serverless_function_region=None, team_id=None, trusted_ips=None, vercel_authentication=None):
+    def __init__(__self__, auto_assign_custom_domains=None, automatically_expose_system_environment_variables=None, build_command=None, customer_success_code_visibility=None, dev_command=None, directory_listing=None, environments=None, framework=None, function_failover=None, git_comments=None, git_fork_protection=None, git_lfs=None, git_repository=None, id=None, ignore_command=None, install_command=None, name=None, output_directory=None, password_protection=None, preview_comments=None, prioritise_production_builds=None, protection_bypass_for_automation=None, public_source=None, root_directory=None, serverless_function_region=None, skew_protection=None, team_id=None, trusted_ips=None, vercel_authentication=None):
+        if auto_assign_custom_domains and not isinstance(auto_assign_custom_domains, bool):
+            raise TypeError("Expected argument 'auto_assign_custom_domains' to be a bool")
+        pulumi.set(__self__, "auto_assign_custom_domains", auto_assign_custom_domains)
+        if automatically_expose_system_environment_variables and not isinstance(automatically_expose_system_environment_variables, bool):
+            raise TypeError("Expected argument 'automatically_expose_system_environment_variables' to be a bool")
+        pulumi.set(__self__, "automatically_expose_system_environment_variables", automatically_expose_system_environment_variables)
         if build_command and not isinstance(build_command, str):
             raise TypeError("Expected argument 'build_command' to be a str")
         pulumi.set(__self__, "build_command", build_command)
+        if customer_success_code_visibility and not isinstance(customer_success_code_visibility, bool):
+            raise TypeError("Expected argument 'customer_success_code_visibility' to be a bool")
+        pulumi.set(__self__, "customer_success_code_visibility", customer_success_code_visibility)
         if dev_command and not isinstance(dev_command, str):
             raise TypeError("Expected argument 'dev_command' to be a str")
         pulumi.set(__self__, "dev_command", dev_command)
+        if directory_listing and not isinstance(directory_listing, bool):
+            raise TypeError("Expected argument 'directory_listing' to be a bool")
+        pulumi.set(__self__, "directory_listing", directory_listing)
         if environments and not isinstance(environments, list):
             raise TypeError("Expected argument 'environments' to be a list")
         pulumi.set(__self__, "environments", environments)
         if framework and not isinstance(framework, str):
             raise TypeError("Expected argument 'framework' to be a str")
         pulumi.set(__self__, "framework", framework)
+        if function_failover and not isinstance(function_failover, bool):
+            raise TypeError("Expected argument 'function_failover' to be a bool")
+        pulumi.set(__self__, "function_failover", function_failover)
+        if git_comments and not isinstance(git_comments, dict):
+            raise TypeError("Expected argument 'git_comments' to be a dict")
+        pulumi.set(__self__, "git_comments", git_comments)
+        if git_fork_protection and not isinstance(git_fork_protection, bool):
+            raise TypeError("Expected argument 'git_fork_protection' to be a bool")
+        pulumi.set(__self__, "git_fork_protection", git_fork_protection)
+        if git_lfs and not isinstance(git_lfs, bool):
+            raise TypeError("Expected argument 'git_lfs' to be a bool")
+        pulumi.set(__self__, "git_lfs", git_lfs)
         if git_repository and not isinstance(git_repository, dict):
             raise TypeError("Expected argument 'git_repository' to be a dict")
         pulumi.set(__self__, "git_repository", git_repository)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if ignore_command and not isinstance(ignore_command, str):
@@ -52,50 +76,94 @@
         pulumi.set(__self__, "name", name)
         if output_directory and not isinstance(output_directory, str):
             raise TypeError("Expected argument 'output_directory' to be a str")
         pulumi.set(__self__, "output_directory", output_directory)
         if password_protection and not isinstance(password_protection, dict):
             raise TypeError("Expected argument 'password_protection' to be a dict")
         pulumi.set(__self__, "password_protection", password_protection)
+        if preview_comments and not isinstance(preview_comments, bool):
+            raise TypeError("Expected argument 'preview_comments' to be a bool")
+        pulumi.set(__self__, "preview_comments", preview_comments)
+        if prioritise_production_builds and not isinstance(prioritise_production_builds, bool):
+            raise TypeError("Expected argument 'prioritise_production_builds' to be a bool")
+        pulumi.set(__self__, "prioritise_production_builds", prioritise_production_builds)
+        if protection_bypass_for_automation and not isinstance(protection_bypass_for_automation, bool):
+            raise TypeError("Expected argument 'protection_bypass_for_automation' to be a bool")
+        pulumi.set(__self__, "protection_bypass_for_automation", protection_bypass_for_automation)
         if public_source and not isinstance(public_source, bool):
             raise TypeError("Expected argument 'public_source' to be a bool")
         pulumi.set(__self__, "public_source", public_source)
         if root_directory and not isinstance(root_directory, str):
             raise TypeError("Expected argument 'root_directory' to be a str")
         pulumi.set(__self__, "root_directory", root_directory)
         if serverless_function_region and not isinstance(serverless_function_region, str):
             raise TypeError("Expected argument 'serverless_function_region' to be a str")
         pulumi.set(__self__, "serverless_function_region", serverless_function_region)
+        if skew_protection and not isinstance(skew_protection, str):
+            raise TypeError("Expected argument 'skew_protection' to be a str")
+        pulumi.set(__self__, "skew_protection", skew_protection)
         if team_id and not isinstance(team_id, str):
             raise TypeError("Expected argument 'team_id' to be a str")
         pulumi.set(__self__, "team_id", team_id)
         if trusted_ips and not isinstance(trusted_ips, dict):
             raise TypeError("Expected argument 'trusted_ips' to be a dict")
         pulumi.set(__self__, "trusted_ips", trusted_ips)
         if vercel_authentication and not isinstance(vercel_authentication, dict):
             raise TypeError("Expected argument 'vercel_authentication' to be a dict")
         pulumi.set(__self__, "vercel_authentication", vercel_authentication)
 
     @property
+    @pulumi.getter(name="autoAssignCustomDomains")
+    def auto_assign_custom_domains(self) -> bool:
+        """
+        Automatically assign custom production domains after each Production deployment via merge to the production branch or Vercel CLI deploy with --prod. Defaults to `true`
+        """
+        return pulumi.get(self, "auto_assign_custom_domains")
+
+    @property
+    @pulumi.getter(name="automaticallyExposeSystemEnvironmentVariables")
+    def automatically_expose_system_environment_variables(self) -> bool:
+        """
+        Vercel provides a set of Environment Variables that are automatically populated by the System, such as the URL of the Deployment or the name of the Git branch deployed. To expose them to your Deployments, enable this field
+        """
+        return pulumi.get(self, "automatically_expose_system_environment_variables")
+
+    @property
     @pulumi.getter(name="buildCommand")
     def build_command(self) -> str:
         """
         The build command for this project. If omitted, this value will be automatically detected.
         """
         return pulumi.get(self, "build_command")
 
     @property
+    @pulumi.getter(name="customerSuccessCodeVisibility")
+    def customer_success_code_visibility(self) -> bool:
+        """
+        Allows Vercel Customer Support to inspect all Deployments' source code in this project to assist with debugging.
+        """
+        return pulumi.get(self, "customer_success_code_visibility")
+
+    @property
     @pulumi.getter(name="devCommand")
     def dev_command(self) -> str:
         """
         The dev command for this project. If omitted, this value will be automatically detected.
         """
         return pulumi.get(self, "dev_command")
 
     @property
+    @pulumi.getter(name="directoryListing")
+    def directory_listing(self) -> bool:
+        """
+        If no index file is present within a directory, the directory contents will be displayed.
+        """
+        return pulumi.get(self, "directory_listing")
+
+    @property
     @pulumi.getter
     def environments(self) -> Sequence['outputs.GetProjectEnvironmentResult']:
         """
         A list of environment variables that should be configured for the project.
         """
         return pulumi.get(self, "environments")
 
@@ -104,14 +172,46 @@
     def framework(self) -> str:
         """
         The framework that is being used for this project. If omitted, no framework is selected.
         """
         return pulumi.get(self, "framework")
 
     @property
+    @pulumi.getter(name="functionFailover")
+    def function_failover(self) -> bool:
+        """
+        Automatically failover Serverless Functions to the nearest region. You can customize regions through vercel.json. A new Deployment is required for your changes to take effect.
+        """
+        return pulumi.get(self, "function_failover")
+
+    @property
+    @pulumi.getter(name="gitComments")
+    def git_comments(self) -> 'outputs.GetProjectGitCommentsResult':
+        """
+        Configuration for Git Comments.
+        """
+        return pulumi.get(self, "git_comments")
+
+    @property
+    @pulumi.getter(name="gitForkProtection")
+    def git_fork_protection(self) -> bool:
+        """
+        Ensures that pull requests targeting your Git repository must be authorized by a member of your Team before deploying if your Project has Environment Variables or if the pull request includes a change to vercel.json.
+        """
+        return pulumi.get(self, "git_fork_protection")
+
+    @property
+    @pulumi.getter(name="gitLfs")
+    def git_lfs(self) -> bool:
+        """
+        Enables Git LFS support. Git LFS replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.
+        """
+        return pulumi.get(self, "git_lfs")
+
+    @property
     @pulumi.getter(name="gitRepository")
     def git_repository(self) -> 'outputs.GetProjectGitRepositoryResult':
         """
         The Git Repository that will be connected to the project. When this is defined, any pushes to the specified connected Git Repository will be automatically deployed. This requires the corresponding Vercel for [Github](https://vercel.com/docs/concepts/git/vercel-for-github), [Gitlab](https://vercel.com/docs/concepts/git/vercel-for-gitlab) or [Bitbucket](https://vercel.com/docs/concepts/git/vercel-for-bitbucket) plugins to be installed.
         """
         return pulumi.get(self, "git_repository")
 
@@ -160,14 +260,38 @@
     def password_protection(self) -> 'outputs.GetProjectPasswordProtectionResult':
         """
         Ensures visitors of your Preview Deployments must enter a password in order to gain access.
         """
         return pulumi.get(self, "password_protection")
 
     @property
+    @pulumi.getter(name="previewComments")
+    def preview_comments(self) -> bool:
+        """
+        Whether comments are enabled on your Preview Deployments.
+        """
+        return pulumi.get(self, "preview_comments")
+
+    @property
+    @pulumi.getter(name="prioritiseProductionBuilds")
+    def prioritise_production_builds(self) -> bool:
+        """
+        If enabled, builds for the Production environment will be prioritized over Preview environments.
+        """
+        return pulumi.get(self, "prioritise_production_builds")
+
+    @property
+    @pulumi.getter(name="protectionBypassForAutomation")
+    def protection_bypass_for_automation(self) -> bool:
+        """
+        Allows automation services to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments on this project when using an HTTP header named `x-vercel-protection-bypass`.
+        """
+        return pulumi.get(self, "protection_bypass_for_automation")
+
+    @property
     @pulumi.getter(name="publicSource")
     def public_source(self) -> bool:
         """
         Specifies whether the source code and logs of the deployments for this project should be public or not.
         """
         return pulumi.get(self, "public_source")
 
@@ -184,14 +308,22 @@
     def serverless_function_region(self) -> str:
         """
         The region on Vercel's network to which your Serverless Functions are deployed. It should be close to any data source your Serverless Function might depend on. A new Deployment is required for your changes to take effect. Please see [Vercel's documentation](https://vercel.com/docs/concepts/edge-network/regions) for a full list of regions.
         """
         return pulumi.get(self, "serverless_function_region")
 
     @property
+    @pulumi.getter(name="skewProtection")
+    def skew_protection(self) -> str:
+        """
+        Ensures that outdated clients always fetch the correct version for a given deployment. This value defines how long Vercel keeps Skew Protection active.
+        """
+        return pulumi.get(self, "skew_protection")
+
+    @property
     @pulumi.getter(name="teamId")
     def team_id(self) -> str:
         """
         The team ID the project exists beneath. Required when configuring a team resource if a default team has not been set in the provider.
         """
         return pulumi.get(self, "team_id")
 
@@ -214,28 +346,40 @@
 
 class AwaitableGetProjectResult(GetProjectResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetProjectResult(
+            auto_assign_custom_domains=self.auto_assign_custom_domains,
+            automatically_expose_system_environment_variables=self.automatically_expose_system_environment_variables,
             build_command=self.build_command,
+            customer_success_code_visibility=self.customer_success_code_visibility,
             dev_command=self.dev_command,
+            directory_listing=self.directory_listing,
             environments=self.environments,
             framework=self.framework,
+            function_failover=self.function_failover,
+            git_comments=self.git_comments,
+            git_fork_protection=self.git_fork_protection,
+            git_lfs=self.git_lfs,
             git_repository=self.git_repository,
             id=self.id,
             ignore_command=self.ignore_command,
             install_command=self.install_command,
             name=self.name,
             output_directory=self.output_directory,
             password_protection=self.password_protection,
+            preview_comments=self.preview_comments,
+            prioritise_production_builds=self.prioritise_production_builds,
+            protection_bypass_for_automation=self.protection_bypass_for_automation,
             public_source=self.public_source,
             root_directory=self.root_directory,
             serverless_function_region=self.serverless_function_region,
+            skew_protection=self.skew_protection,
             team_id=self.team_id,
             trusted_ips=self.trusted_ips,
             vercel_authentication=self.vercel_authentication)
 
 
 def get_project(name: Optional[str] = None,
                 team_id: Optional[str] = None,
@@ -245,49 +389,59 @@
 
     A Project groups deployments and custom domains. To deploy on Vercel, you need a Project.
 
     For more detailed information, please see the [Vercel documentation](https://vercel.com/docs/concepts/projects/overview).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vercel as vercel
 
     foo = vercel.get_project(name="my-existing-project")
     pulumi.export("projectId", foo.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the project.
     :param str team_id: The team ID the project exists beneath. Required when configuring a team resource if a default team has not been set in the provider.
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['teamId'] = team_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('vercel:index/getProject:getProject', __args__, opts=opts, typ=GetProjectResult).value
 
     return AwaitableGetProjectResult(
+        auto_assign_custom_domains=pulumi.get(__ret__, 'auto_assign_custom_domains'),
+        automatically_expose_system_environment_variables=pulumi.get(__ret__, 'automatically_expose_system_environment_variables'),
         build_command=pulumi.get(__ret__, 'build_command'),
+        customer_success_code_visibility=pulumi.get(__ret__, 'customer_success_code_visibility'),
         dev_command=pulumi.get(__ret__, 'dev_command'),
+        directory_listing=pulumi.get(__ret__, 'directory_listing'),
         environments=pulumi.get(__ret__, 'environments'),
         framework=pulumi.get(__ret__, 'framework'),
+        function_failover=pulumi.get(__ret__, 'function_failover'),
+        git_comments=pulumi.get(__ret__, 'git_comments'),
+        git_fork_protection=pulumi.get(__ret__, 'git_fork_protection'),
+        git_lfs=pulumi.get(__ret__, 'git_lfs'),
         git_repository=pulumi.get(__ret__, 'git_repository'),
         id=pulumi.get(__ret__, 'id'),
         ignore_command=pulumi.get(__ret__, 'ignore_command'),
         install_command=pulumi.get(__ret__, 'install_command'),
         name=pulumi.get(__ret__, 'name'),
         output_directory=pulumi.get(__ret__, 'output_directory'),
         password_protection=pulumi.get(__ret__, 'password_protection'),
+        preview_comments=pulumi.get(__ret__, 'preview_comments'),
+        prioritise_production_builds=pulumi.get(__ret__, 'prioritise_production_builds'),
+        protection_bypass_for_automation=pulumi.get(__ret__, 'protection_bypass_for_automation'),
         public_source=pulumi.get(__ret__, 'public_source'),
         root_directory=pulumi.get(__ret__, 'root_directory'),
         serverless_function_region=pulumi.get(__ret__, 'serverless_function_region'),
+        skew_protection=pulumi.get(__ret__, 'skew_protection'),
         team_id=pulumi.get(__ret__, 'team_id'),
         trusted_ips=pulumi.get(__ret__, 'trusted_ips'),
         vercel_authentication=pulumi.get(__ret__, 'vercel_authentication'))
 
 
 @_utilities.lift_output_func(get_project)
 def get_project_output(name: Optional[pulumi.Input[str]] = None,
@@ -298,22 +452,20 @@
 
     A Project groups deployments and custom domains. To deploy on Vercel, you need a Project.
 
     For more detailed information, please see the [Vercel documentation](https://vercel.com/docs/concepts/projects/overview).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vercel as vercel
 
     foo = vercel.get_project(name="my-existing-project")
     pulumi.export("projectId", foo.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the project.
     :param str team_id: The team ID the project exists beneath. Required when configuring a team resource if a default team has not been set in the provider.
     """
     ...
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_project_directory.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_project_directory.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/get_shared_environment_variable.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/get_shared_environment_variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,27 +126,25 @@
 
     A Shared Environment Variable resource defines an Environment Variable that can be shared between multiple Vercel Projects.
 
     For more detailed information, please see the [Vercel documentation](https://vercel.com/docs/concepts/projects/environment-variables/shared-environment-variables).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vercel as vercel
 
     example = vercel.get_shared_environment_variable(id="xxxxxxxxxxxxxxx")
     example_by_key_and_target = vercel.get_shared_environment_variable(key="MY_ENV_VAR",
         targets=[
             "production",
             "preview",
         ])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Environment Variable.
     :param str key: The name of the Environment Variable.
     :param Sequence[str] targets: The environments that the Environment Variable should be present on. Valid targets are either `production`, `preview`, or `development`.
     :param str team_id: The ID of the Vercel team. Shared environment variables require a team.
     """
@@ -179,27 +177,25 @@
 
     A Shared Environment Variable resource defines an Environment Variable that can be shared between multiple Vercel Projects.
 
     For more detailed information, please see the [Vercel documentation](https://vercel.com/docs/concepts/projects/environment-variables/shared-environment-variables).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vercel as vercel
 
     example = vercel.get_shared_environment_variable(id="xxxxxxxxxxxxxxx")
     example_by_key_and_target = vercel.get_shared_environment_variable(key="MY_ENV_VAR",
         targets=[
             "production",
             "preview",
         ])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Environment Variable.
     :param str key: The name of the Environment Variable.
     :param Sequence[str] targets: The environments that the Environment Variable should be present on. Valid targets are either `production`, `preview`, or `development`.
     :param str team_id: The ID of the Vercel team. Shared environment variables require a team.
     """
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/outputs.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/outputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 from . import _utilities
 from . import outputs
 
 __all__ = [
     'DeploymentProjectSettings',
     'DnsRecordSrv',
     'ProjectEnvironment',
+    'ProjectGitComments',
     'ProjectGitRepository',
+    'ProjectGitRepositoryDeployHook',
     'ProjectPasswordProtection',
     'ProjectTrustedIps',
     'ProjectTrustedIpsAddress',
     'ProjectVercelAuthentication',
     'GetProjectEnvironmentResult',
+    'GetProjectGitCommentsResult',
     'GetProjectGitRepositoryResult',
     'GetProjectPasswordProtectionResult',
     'GetProjectTrustedIpsResult',
     'GetProjectTrustedIpsAddressResult',
     'GetProjectVercelAuthenticationResult',
 ]
 
@@ -258,19 +261,69 @@
         """
         Whether the Environment Variable is sensitive or not.
         """
         return pulumi.get(self, "sensitive")
 
 
 @pulumi.output_type
+class ProjectGitComments(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "onCommit":
+            suggest = "on_commit"
+        elif key == "onPullRequest":
+            suggest = "on_pull_request"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ProjectGitComments. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ProjectGitComments.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ProjectGitComments.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 on_commit: bool,
+                 on_pull_request: bool):
+        """
+        :param bool on_commit: Whether Commit comments are enabled
+        :param bool on_pull_request: Whether Pull Request comments are enabled
+        """
+        pulumi.set(__self__, "on_commit", on_commit)
+        pulumi.set(__self__, "on_pull_request", on_pull_request)
+
+    @property
+    @pulumi.getter(name="onCommit")
+    def on_commit(self) -> bool:
+        """
+        Whether Commit comments are enabled
+        """
+        return pulumi.get(self, "on_commit")
+
+    @property
+    @pulumi.getter(name="onPullRequest")
+    def on_pull_request(self) -> bool:
+        """
+        Whether Pull Request comments are enabled
+        """
+        return pulumi.get(self, "on_pull_request")
+
+
+@pulumi.output_type
 class ProjectGitRepository(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "productionBranch":
+        if key == "deployHooks":
+            suggest = "deploy_hooks"
+        elif key == "productionBranch":
             suggest = "production_branch"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ProjectGitRepository. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ProjectGitRepository.__key_warning(key)
@@ -279,22 +332,26 @@
     def get(self, key: str, default = None) -> Any:
         ProjectGitRepository.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  repo: str,
                  type: str,
+                 deploy_hooks: Optional[Sequence['outputs.ProjectGitRepositoryDeployHook']] = None,
                  production_branch: Optional[str] = None):
         """
         :param str repo: The name of the git repository. For example: `vercel/next.js`.
         :param str type: The git provider of the repository. Must be either `github`, `gitlab`, or `bitbucket`.
+        :param Sequence['ProjectGitRepositoryDeployHookArgs'] deploy_hooks: Deploy hooks are unique URLs that allow you to trigger a deployment of a given branch. See https://vercel.com/docs/deployments/deploy-hooks for full information.
         :param str production_branch: By default, every commit pushed to the main branch will trigger a Production Deployment instead of the usual Preview Deployment. You can switch to a different branch here.
         """
         pulumi.set(__self__, "repo", repo)
         pulumi.set(__self__, "type", type)
+        if deploy_hooks is not None:
+            pulumi.set(__self__, "deploy_hooks", deploy_hooks)
         if production_branch is not None:
             pulumi.set(__self__, "production_branch", production_branch)
 
     @property
     @pulumi.getter
     def repo(self) -> str:
         """
@@ -307,23 +364,84 @@
     def type(self) -> str:
         """
         The git provider of the repository. Must be either `github`, `gitlab`, or `bitbucket`.
         """
         return pulumi.get(self, "type")
 
     @property
+    @pulumi.getter(name="deployHooks")
+    def deploy_hooks(self) -> Optional[Sequence['outputs.ProjectGitRepositoryDeployHook']]:
+        """
+        Deploy hooks are unique URLs that allow you to trigger a deployment of a given branch. See https://vercel.com/docs/deployments/deploy-hooks for full information.
+        """
+        return pulumi.get(self, "deploy_hooks")
+
+    @property
     @pulumi.getter(name="productionBranch")
     def production_branch(self) -> Optional[str]:
         """
         By default, every commit pushed to the main branch will trigger a Production Deployment instead of the usual Preview Deployment. You can switch to a different branch here.
         """
         return pulumi.get(self, "production_branch")
 
 
 @pulumi.output_type
+class ProjectGitRepositoryDeployHook(dict):
+    def __init__(__self__, *,
+                 name: str,
+                 ref: str,
+                 id: Optional[str] = None,
+                 url: Optional[str] = None):
+        """
+        :param str name: The name of the deploy hook.
+        :param str ref: The branch or commit hash that should be deployed.
+        :param str id: The ID of the deploy hook.
+        :param str url: A URL that, when a POST request is made to, will trigger a new deployment.
+        """
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "ref", ref)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if url is not None:
+            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The name of the deploy hook.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def ref(self) -> str:
+        """
+        The branch or commit hash that should be deployed.
+        """
+        return pulumi.get(self, "ref")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        The ID of the deploy hook.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def url(self) -> Optional[str]:
+        """
+        A URL that, when a POST request is made to, will trigger a new deployment.
+        """
+        return pulumi.get(self, "url")
+
+
+@pulumi.output_type
 class ProjectPasswordProtection(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "deploymentType":
             suggest = "deployment_type"
 
@@ -427,26 +545,26 @@
 
 @pulumi.output_type
 class ProjectTrustedIpsAddress(dict):
     def __init__(__self__, *,
                  value: str,
                  note: Optional[str] = None):
         """
-        :param str value: The value of the Environment Variable.
+        :param str value: The address or CIDR range that can access deployments.
         :param str note: A description for the value
         """
         pulumi.set(__self__, "value", value)
         if note is not None:
             pulumi.set(__self__, "note", note)
 
     @property
     @pulumi.getter
     def value(self) -> str:
         """
-        The value of the Environment Variable.
+        The address or CIDR range that can access deployments.
         """
         return pulumi.get(self, "value")
 
     @property
     @pulumi.getter
     def note(self) -> Optional[str]:
         """
@@ -560,14 +678,43 @@
         """
         The value of the environment variable.
         """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
+class GetProjectGitCommentsResult(dict):
+    def __init__(__self__, *,
+                 on_commit: bool,
+                 on_pull_request: bool):
+        """
+        :param bool on_commit: Whether Commit comments are enabled
+        :param bool on_pull_request: Whether Pull Request comments are enabled
+        """
+        pulumi.set(__self__, "on_commit", on_commit)
+        pulumi.set(__self__, "on_pull_request", on_pull_request)
+
+    @property
+    @pulumi.getter(name="onCommit")
+    def on_commit(self) -> bool:
+        """
+        Whether Commit comments are enabled
+        """
+        return pulumi.get(self, "on_commit")
+
+    @property
+    @pulumi.getter(name="onPullRequest")
+    def on_pull_request(self) -> bool:
+        """
+        Whether Pull Request comments are enabled
+        """
+        return pulumi.get(self, "on_pull_request")
+
+
+@pulumi.output_type
 class GetProjectGitRepositoryResult(dict):
     def __init__(__self__, *,
                  production_branch: str,
                  repo: str,
                  type: str):
         """
         :param str production_branch: By default, every commit pushed to the main branch will trigger a Production Deployment instead of the usual Preview Deployment. You can switch to a different branch here.
@@ -662,31 +809,25 @@
 
 
 @pulumi.output_type
 class GetProjectTrustedIpsAddressResult(dict):
     def __init__(__self__, *,
                  note: str,
                  value: str):
-        """
-        :param str value: The value of the environment variable.
-        """
         pulumi.set(__self__, "note", note)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def note(self) -> str:
         return pulumi.get(self, "note")
 
     @property
     @pulumi.getter
     def value(self) -> str:
-        """
-        The value of the environment variable.
-        """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
 class GetProjectVercelAuthenticationResult(dict):
     def __init__(__self__, *,
                  deployment_type: str):
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/project.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/project.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,111 +12,203 @@
 from ._inputs import *
 
 __all__ = ['ProjectArgs', 'Project']
 
 @pulumi.input_type
 class ProjectArgs:
     def __init__(__self__, *,
+                 auto_assign_custom_domains: Optional[pulumi.Input[bool]] = None,
+                 automatically_expose_system_environment_variables: Optional[pulumi.Input[bool]] = None,
                  build_command: Optional[pulumi.Input[str]] = None,
+                 customer_success_code_visibility: Optional[pulumi.Input[bool]] = None,
                  dev_command: Optional[pulumi.Input[str]] = None,
+                 directory_listing: Optional[pulumi.Input[bool]] = None,
                  environments: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentArgs']]]] = None,
                  framework: Optional[pulumi.Input[str]] = None,
+                 function_failover: Optional[pulumi.Input[bool]] = None,
+                 git_comments: Optional[pulumi.Input['ProjectGitCommentsArgs']] = None,
+                 git_fork_protection: Optional[pulumi.Input[bool]] = None,
+                 git_lfs: Optional[pulumi.Input[bool]] = None,
                  git_repository: Optional[pulumi.Input['ProjectGitRepositoryArgs']] = None,
                  ignore_command: Optional[pulumi.Input[str]] = None,
                  install_command: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  output_directory: Optional[pulumi.Input[str]] = None,
                  password_protection: Optional[pulumi.Input['ProjectPasswordProtectionArgs']] = None,
+                 preview_comments: Optional[pulumi.Input[bool]] = None,
+                 prioritise_production_builds: Optional[pulumi.Input[bool]] = None,
                  protection_bypass_for_automation: Optional[pulumi.Input[bool]] = None,
                  public_source: Optional[pulumi.Input[bool]] = None,
                  root_directory: Optional[pulumi.Input[str]] = None,
                  serverless_function_region: Optional[pulumi.Input[str]] = None,
+                 skew_protection: Optional[pulumi.Input[str]] = None,
                  team_id: Optional[pulumi.Input[str]] = None,
                  trusted_ips: Optional[pulumi.Input['ProjectTrustedIpsArgs']] = None,
                  vercel_authentication: Optional[pulumi.Input['ProjectVercelAuthenticationArgs']] = None):
         """
         The set of arguments for constructing a Project resource.
+        :param pulumi.Input[bool] auto_assign_custom_domains: Automatically assign custom production domains after each Production deployment via merge to the production branch or Vercel CLI deploy with --prod. Defaults to `true`
+        :param pulumi.Input[bool] automatically_expose_system_environment_variables: Vercel provides a set of Environment Variables that are automatically populated by the System, such as the URL of the Deployment or the name of the Git branch deployed. To expose them to your Deployments, enable this field
         :param pulumi.Input[str] build_command: The build command for this project. If omitted, this value will be automatically detected.
+        :param pulumi.Input[bool] customer_success_code_visibility: Allows Vercel Customer Support to inspect all Deployments' source code in this project to assist with debugging.
         :param pulumi.Input[str] dev_command: The dev command for this project. If omitted, this value will be automatically detected.
+        :param pulumi.Input[bool] directory_listing: If no index file is present within a directory, the directory contents will be displayed.
         :param pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentArgs']]] environments: A set of Environment Variables that should be configured for the project.
         :param pulumi.Input[str] framework: The framework that is being used for this project. If omitted, no framework is selected.
+        :param pulumi.Input[bool] function_failover: Automatically failover Serverless Functions to the nearest region. You can customize regions through vercel.json. A new Deployment is required for your changes to take effect.
+        :param pulumi.Input['ProjectGitCommentsArgs'] git_comments: Configuration for Git Comments.
+        :param pulumi.Input[bool] git_fork_protection: Ensures that pull requests targeting your Git repository must be authorized by a member of your Team before deploying if your Project has Environment Variables or if the pull request includes a change to vercel.json. Defaults to `true`.
+        :param pulumi.Input[bool] git_lfs: Enables Git LFS support. Git LFS replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.
         :param pulumi.Input['ProjectGitRepositoryArgs'] git_repository: The Git Repository that will be connected to the project. When this is defined, any pushes to the specified connected Git Repository will be automatically deployed. This requires the corresponding Vercel for [Github](https://vercel.com/docs/concepts/git/vercel-for-github), [Gitlab](https://vercel.com/docs/concepts/git/vercel-for-gitlab) or [Bitbucket](https://vercel.com/docs/concepts/git/vercel-for-bitbucket) plugins to be installed.
         :param pulumi.Input[str] ignore_command: When a commit is pushed to the Git repository that is connected with your Project, its SHA will determine if a new Build has to be issued. If the SHA was deployed before, no new Build will be issued. You can customize this behavior with a command that exits with code 1 (new Build needed) or code 0.
         :param pulumi.Input[str] install_command: The install command for this project. If omitted, this value will be automatically detected.
         :param pulumi.Input[str] name: The desired name for the project.
         :param pulumi.Input[str] output_directory: The output directory of the project. If omitted, this value will be automatically detected.
         :param pulumi.Input['ProjectPasswordProtectionArgs'] password_protection: Ensures visitors of your Preview Deployments must enter a password in order to gain access.
+        :param pulumi.Input[bool] preview_comments: Whether to enable comments on your Preview Deployments. If omitted, comments are controlled at the team level (default behaviour).
+        :param pulumi.Input[bool] prioritise_production_builds: If enabled, builds for the Production environment will be prioritized over Preview environments.
         :param pulumi.Input[bool] protection_bypass_for_automation: Allow automation services to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments on this project when using an HTTP header named `x-vercel-protection-bypass` with a value of the `password_protection_for_automation_secret` field.
         :param pulumi.Input[bool] public_source: By default, visitors to the `/_logs` and `/_src` paths of your Production and Preview Deployments must log in with Vercel (requires being a member of your team) to see the Source, Logs and Deployment Status of your project. Setting `public_source` to `true` disables this behaviour, meaning the Source, Logs and Deployment Status can be publicly viewed.
         :param pulumi.Input[str] root_directory: The name of a directory or relative path to the source code of your project. If omitted, it will default to the project root.
         :param pulumi.Input[str] serverless_function_region: The region on Vercel's network to which your Serverless Functions are deployed. It should be close to any data source your Serverless Function might depend on. A new Deployment is required for your changes to take effect. Please see [Vercel's documentation](https://vercel.com/docs/concepts/edge-network/regions) for a full list of regions.
+        :param pulumi.Input[str] skew_protection: Ensures that outdated clients always fetch the correct version for a given deployment. This value defines how long Vercel keeps Skew Protection active.
         :param pulumi.Input[str] team_id: The team ID to add the project to. Required when configuring a team resource if a default team has not been set in the provider.
         :param pulumi.Input['ProjectTrustedIpsArgs'] trusted_ips: Ensures only visitors from an allowed IP address can access your deployment.
         :param pulumi.Input['ProjectVercelAuthenticationArgs'] vercel_authentication: Ensures visitors to your Preview Deployments are logged into Vercel and have a minimum of Viewer access on your team.
         """
+        if auto_assign_custom_domains is not None:
+            pulumi.set(__self__, "auto_assign_custom_domains", auto_assign_custom_domains)
+        if automatically_expose_system_environment_variables is not None:
+            pulumi.set(__self__, "automatically_expose_system_environment_variables", automatically_expose_system_environment_variables)
         if build_command is not None:
             pulumi.set(__self__, "build_command", build_command)
+        if customer_success_code_visibility is not None:
+            pulumi.set(__self__, "customer_success_code_visibility", customer_success_code_visibility)
         if dev_command is not None:
             pulumi.set(__self__, "dev_command", dev_command)
+        if directory_listing is not None:
+            pulumi.set(__self__, "directory_listing", directory_listing)
         if environments is not None:
             pulumi.set(__self__, "environments", environments)
         if framework is not None:
             pulumi.set(__self__, "framework", framework)
+        if function_failover is not None:
+            pulumi.set(__self__, "function_failover", function_failover)
+        if git_comments is not None:
+            pulumi.set(__self__, "git_comments", git_comments)
+        if git_fork_protection is not None:
+            pulumi.set(__self__, "git_fork_protection", git_fork_protection)
+        if git_lfs is not None:
+            pulumi.set(__self__, "git_lfs", git_lfs)
         if git_repository is not None:
             pulumi.set(__self__, "git_repository", git_repository)
         if ignore_command is not None:
             pulumi.set(__self__, "ignore_command", ignore_command)
         if install_command is not None:
             pulumi.set(__self__, "install_command", install_command)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if output_directory is not None:
             pulumi.set(__self__, "output_directory", output_directory)
         if password_protection is not None:
             pulumi.set(__self__, "password_protection", password_protection)
+        if preview_comments is not None:
+            pulumi.set(__self__, "preview_comments", preview_comments)
+        if prioritise_production_builds is not None:
+            pulumi.set(__self__, "prioritise_production_builds", prioritise_production_builds)
         if protection_bypass_for_automation is not None:
             pulumi.set(__self__, "protection_bypass_for_automation", protection_bypass_for_automation)
         if public_source is not None:
             pulumi.set(__self__, "public_source", public_source)
         if root_directory is not None:
             pulumi.set(__self__, "root_directory", root_directory)
         if serverless_function_region is not None:
             pulumi.set(__self__, "serverless_function_region", serverless_function_region)
+        if skew_protection is not None:
+            pulumi.set(__self__, "skew_protection", skew_protection)
         if team_id is not None:
             pulumi.set(__self__, "team_id", team_id)
         if trusted_ips is not None:
             pulumi.set(__self__, "trusted_ips", trusted_ips)
         if vercel_authentication is not None:
             pulumi.set(__self__, "vercel_authentication", vercel_authentication)
 
     @property
+    @pulumi.getter(name="autoAssignCustomDomains")
+    def auto_assign_custom_domains(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically assign custom production domains after each Production deployment via merge to the production branch or Vercel CLI deploy with --prod. Defaults to `true`
+        """
+        return pulumi.get(self, "auto_assign_custom_domains")
+
+    @auto_assign_custom_domains.setter
+    def auto_assign_custom_domains(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_assign_custom_domains", value)
+
+    @property
+    @pulumi.getter(name="automaticallyExposeSystemEnvironmentVariables")
+    def automatically_expose_system_environment_variables(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Vercel provides a set of Environment Variables that are automatically populated by the System, such as the URL of the Deployment or the name of the Git branch deployed. To expose them to your Deployments, enable this field
+        """
+        return pulumi.get(self, "automatically_expose_system_environment_variables")
+
+    @automatically_expose_system_environment_variables.setter
+    def automatically_expose_system_environment_variables(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "automatically_expose_system_environment_variables", value)
+
+    @property
     @pulumi.getter(name="buildCommand")
     def build_command(self) -> Optional[pulumi.Input[str]]:
         """
         The build command for this project. If omitted, this value will be automatically detected.
         """
         return pulumi.get(self, "build_command")
 
     @build_command.setter
     def build_command(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "build_command", value)
 
     @property
+    @pulumi.getter(name="customerSuccessCodeVisibility")
+    def customer_success_code_visibility(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Allows Vercel Customer Support to inspect all Deployments' source code in this project to assist with debugging.
+        """
+        return pulumi.get(self, "customer_success_code_visibility")
+
+    @customer_success_code_visibility.setter
+    def customer_success_code_visibility(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "customer_success_code_visibility", value)
+
+    @property
     @pulumi.getter(name="devCommand")
     def dev_command(self) -> Optional[pulumi.Input[str]]:
         """
         The dev command for this project. If omitted, this value will be automatically detected.
         """
         return pulumi.get(self, "dev_command")
 
     @dev_command.setter
     def dev_command(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dev_command", value)
 
     @property
+    @pulumi.getter(name="directoryListing")
+    def directory_listing(self) -> Optional[pulumi.Input[bool]]:
+        """
+        If no index file is present within a directory, the directory contents will be displayed.
+        """
+        return pulumi.get(self, "directory_listing")
+
+    @directory_listing.setter
+    def directory_listing(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "directory_listing", value)
+
+    @property
     @pulumi.getter
     def environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentArgs']]]]:
         """
         A set of Environment Variables that should be configured for the project.
         """
         return pulumi.get(self, "environments")
 
@@ -133,14 +225,62 @@
         return pulumi.get(self, "framework")
 
     @framework.setter
     def framework(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "framework", value)
 
     @property
+    @pulumi.getter(name="functionFailover")
+    def function_failover(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically failover Serverless Functions to the nearest region. You can customize regions through vercel.json. A new Deployment is required for your changes to take effect.
+        """
+        return pulumi.get(self, "function_failover")
+
+    @function_failover.setter
+    def function_failover(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "function_failover", value)
+
+    @property
+    @pulumi.getter(name="gitComments")
+    def git_comments(self) -> Optional[pulumi.Input['ProjectGitCommentsArgs']]:
+        """
+        Configuration for Git Comments.
+        """
+        return pulumi.get(self, "git_comments")
+
+    @git_comments.setter
+    def git_comments(self, value: Optional[pulumi.Input['ProjectGitCommentsArgs']]):
+        pulumi.set(self, "git_comments", value)
+
+    @property
+    @pulumi.getter(name="gitForkProtection")
+    def git_fork_protection(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Ensures that pull requests targeting your Git repository must be authorized by a member of your Team before deploying if your Project has Environment Variables or if the pull request includes a change to vercel.json. Defaults to `true`.
+        """
+        return pulumi.get(self, "git_fork_protection")
+
+    @git_fork_protection.setter
+    def git_fork_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "git_fork_protection", value)
+
+    @property
+    @pulumi.getter(name="gitLfs")
+    def git_lfs(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enables Git LFS support. Git LFS replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.
+        """
+        return pulumi.get(self, "git_lfs")
+
+    @git_lfs.setter
+    def git_lfs(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "git_lfs", value)
+
+    @property
     @pulumi.getter(name="gitRepository")
     def git_repository(self) -> Optional[pulumi.Input['ProjectGitRepositoryArgs']]:
         """
         The Git Repository that will be connected to the project. When this is defined, any pushes to the specified connected Git Repository will be automatically deployed. This requires the corresponding Vercel for [Github](https://vercel.com/docs/concepts/git/vercel-for-github), [Gitlab](https://vercel.com/docs/concepts/git/vercel-for-gitlab) or [Bitbucket](https://vercel.com/docs/concepts/git/vercel-for-bitbucket) plugins to be installed.
         """
         return pulumi.get(self, "git_repository")
 
@@ -205,14 +345,38 @@
         return pulumi.get(self, "password_protection")
 
     @password_protection.setter
     def password_protection(self, value: Optional[pulumi.Input['ProjectPasswordProtectionArgs']]):
         pulumi.set(self, "password_protection", value)
 
     @property
+    @pulumi.getter(name="previewComments")
+    def preview_comments(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether to enable comments on your Preview Deployments. If omitted, comments are controlled at the team level (default behaviour).
+        """
+        return pulumi.get(self, "preview_comments")
+
+    @preview_comments.setter
+    def preview_comments(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "preview_comments", value)
+
+    @property
+    @pulumi.getter(name="prioritiseProductionBuilds")
+    def prioritise_production_builds(self) -> Optional[pulumi.Input[bool]]:
+        """
+        If enabled, builds for the Production environment will be prioritized over Preview environments.
+        """
+        return pulumi.get(self, "prioritise_production_builds")
+
+    @prioritise_production_builds.setter
+    def prioritise_production_builds(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "prioritise_production_builds", value)
+
+    @property
     @pulumi.getter(name="protectionBypassForAutomation")
     def protection_bypass_for_automation(self) -> Optional[pulumi.Input[bool]]:
         """
         Allow automation services to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments on this project when using an HTTP header named `x-vercel-protection-bypass` with a value of the `password_protection_for_automation_secret` field.
         """
         return pulumi.get(self, "protection_bypass_for_automation")
 
@@ -253,14 +417,26 @@
         return pulumi.get(self, "serverless_function_region")
 
     @serverless_function_region.setter
     def serverless_function_region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "serverless_function_region", value)
 
     @property
+    @pulumi.getter(name="skewProtection")
+    def skew_protection(self) -> Optional[pulumi.Input[str]]:
+        """
+        Ensures that outdated clients always fetch the correct version for a given deployment. This value defines how long Vercel keeps Skew Protection active.
+        """
+        return pulumi.get(self, "skew_protection")
+
+    @skew_protection.setter
+    def skew_protection(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "skew_protection", value)
+
+    @property
     @pulumi.getter(name="teamId")
     def team_id(self) -> Optional[pulumi.Input[str]]:
         """
         The team ID to add the project to. Required when configuring a team resource if a default team has not been set in the provider.
         """
         return pulumi.get(self, "team_id")
 
@@ -292,115 +468,207 @@
     def vercel_authentication(self, value: Optional[pulumi.Input['ProjectVercelAuthenticationArgs']]):
         pulumi.set(self, "vercel_authentication", value)
 
 
 @pulumi.input_type
 class _ProjectState:
     def __init__(__self__, *,
+                 auto_assign_custom_domains: Optional[pulumi.Input[bool]] = None,
+                 automatically_expose_system_environment_variables: Optional[pulumi.Input[bool]] = None,
                  build_command: Optional[pulumi.Input[str]] = None,
+                 customer_success_code_visibility: Optional[pulumi.Input[bool]] = None,
                  dev_command: Optional[pulumi.Input[str]] = None,
+                 directory_listing: Optional[pulumi.Input[bool]] = None,
                  environments: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentArgs']]]] = None,
                  framework: Optional[pulumi.Input[str]] = None,
+                 function_failover: Optional[pulumi.Input[bool]] = None,
+                 git_comments: Optional[pulumi.Input['ProjectGitCommentsArgs']] = None,
+                 git_fork_protection: Optional[pulumi.Input[bool]] = None,
+                 git_lfs: Optional[pulumi.Input[bool]] = None,
                  git_repository: Optional[pulumi.Input['ProjectGitRepositoryArgs']] = None,
                  ignore_command: Optional[pulumi.Input[str]] = None,
                  install_command: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  output_directory: Optional[pulumi.Input[str]] = None,
                  password_protection: Optional[pulumi.Input['ProjectPasswordProtectionArgs']] = None,
+                 preview_comments: Optional[pulumi.Input[bool]] = None,
+                 prioritise_production_builds: Optional[pulumi.Input[bool]] = None,
                  protection_bypass_for_automation: Optional[pulumi.Input[bool]] = None,
                  protection_bypass_for_automation_secret: Optional[pulumi.Input[str]] = None,
                  public_source: Optional[pulumi.Input[bool]] = None,
                  root_directory: Optional[pulumi.Input[str]] = None,
                  serverless_function_region: Optional[pulumi.Input[str]] = None,
+                 skew_protection: Optional[pulumi.Input[str]] = None,
                  team_id: Optional[pulumi.Input[str]] = None,
                  trusted_ips: Optional[pulumi.Input['ProjectTrustedIpsArgs']] = None,
                  vercel_authentication: Optional[pulumi.Input['ProjectVercelAuthenticationArgs']] = None):
         """
         Input properties used for looking up and filtering Project resources.
+        :param pulumi.Input[bool] auto_assign_custom_domains: Automatically assign custom production domains after each Production deployment via merge to the production branch or Vercel CLI deploy with --prod. Defaults to `true`
+        :param pulumi.Input[bool] automatically_expose_system_environment_variables: Vercel provides a set of Environment Variables that are automatically populated by the System, such as the URL of the Deployment or the name of the Git branch deployed. To expose them to your Deployments, enable this field
         :param pulumi.Input[str] build_command: The build command for this project. If omitted, this value will be automatically detected.
+        :param pulumi.Input[bool] customer_success_code_visibility: Allows Vercel Customer Support to inspect all Deployments' source code in this project to assist with debugging.
         :param pulumi.Input[str] dev_command: The dev command for this project. If omitted, this value will be automatically detected.
+        :param pulumi.Input[bool] directory_listing: If no index file is present within a directory, the directory contents will be displayed.
         :param pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentArgs']]] environments: A set of Environment Variables that should be configured for the project.
         :param pulumi.Input[str] framework: The framework that is being used for this project. If omitted, no framework is selected.
+        :param pulumi.Input[bool] function_failover: Automatically failover Serverless Functions to the nearest region. You can customize regions through vercel.json. A new Deployment is required for your changes to take effect.
+        :param pulumi.Input['ProjectGitCommentsArgs'] git_comments: Configuration for Git Comments.
+        :param pulumi.Input[bool] git_fork_protection: Ensures that pull requests targeting your Git repository must be authorized by a member of your Team before deploying if your Project has Environment Variables or if the pull request includes a change to vercel.json. Defaults to `true`.
+        :param pulumi.Input[bool] git_lfs: Enables Git LFS support. Git LFS replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.
         :param pulumi.Input['ProjectGitRepositoryArgs'] git_repository: The Git Repository that will be connected to the project. When this is defined, any pushes to the specified connected Git Repository will be automatically deployed. This requires the corresponding Vercel for [Github](https://vercel.com/docs/concepts/git/vercel-for-github), [Gitlab](https://vercel.com/docs/concepts/git/vercel-for-gitlab) or [Bitbucket](https://vercel.com/docs/concepts/git/vercel-for-bitbucket) plugins to be installed.
         :param pulumi.Input[str] ignore_command: When a commit is pushed to the Git repository that is connected with your Project, its SHA will determine if a new Build has to be issued. If the SHA was deployed before, no new Build will be issued. You can customize this behavior with a command that exits with code 1 (new Build needed) or code 0.
         :param pulumi.Input[str] install_command: The install command for this project. If omitted, this value will be automatically detected.
         :param pulumi.Input[str] name: The desired name for the project.
         :param pulumi.Input[str] output_directory: The output directory of the project. If omitted, this value will be automatically detected.
         :param pulumi.Input['ProjectPasswordProtectionArgs'] password_protection: Ensures visitors of your Preview Deployments must enter a password in order to gain access.
+        :param pulumi.Input[bool] preview_comments: Whether to enable comments on your Preview Deployments. If omitted, comments are controlled at the team level (default behaviour).
+        :param pulumi.Input[bool] prioritise_production_builds: If enabled, builds for the Production environment will be prioritized over Preview environments.
         :param pulumi.Input[bool] protection_bypass_for_automation: Allow automation services to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments on this project when using an HTTP header named `x-vercel-protection-bypass` with a value of the `password_protection_for_automation_secret` field.
         :param pulumi.Input[str] protection_bypass_for_automation_secret: If `protection_bypass_for_automation` is enabled, use this value in the `x-vercel-protection-bypass` header to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments.
         :param pulumi.Input[bool] public_source: By default, visitors to the `/_logs` and `/_src` paths of your Production and Preview Deployments must log in with Vercel (requires being a member of your team) to see the Source, Logs and Deployment Status of your project. Setting `public_source` to `true` disables this behaviour, meaning the Source, Logs and Deployment Status can be publicly viewed.
         :param pulumi.Input[str] root_directory: The name of a directory or relative path to the source code of your project. If omitted, it will default to the project root.
         :param pulumi.Input[str] serverless_function_region: The region on Vercel's network to which your Serverless Functions are deployed. It should be close to any data source your Serverless Function might depend on. A new Deployment is required for your changes to take effect. Please see [Vercel's documentation](https://vercel.com/docs/concepts/edge-network/regions) for a full list of regions.
+        :param pulumi.Input[str] skew_protection: Ensures that outdated clients always fetch the correct version for a given deployment. This value defines how long Vercel keeps Skew Protection active.
         :param pulumi.Input[str] team_id: The team ID to add the project to. Required when configuring a team resource if a default team has not been set in the provider.
         :param pulumi.Input['ProjectTrustedIpsArgs'] trusted_ips: Ensures only visitors from an allowed IP address can access your deployment.
         :param pulumi.Input['ProjectVercelAuthenticationArgs'] vercel_authentication: Ensures visitors to your Preview Deployments are logged into Vercel and have a minimum of Viewer access on your team.
         """
+        if auto_assign_custom_domains is not None:
+            pulumi.set(__self__, "auto_assign_custom_domains", auto_assign_custom_domains)
+        if automatically_expose_system_environment_variables is not None:
+            pulumi.set(__self__, "automatically_expose_system_environment_variables", automatically_expose_system_environment_variables)
         if build_command is not None:
             pulumi.set(__self__, "build_command", build_command)
+        if customer_success_code_visibility is not None:
+            pulumi.set(__self__, "customer_success_code_visibility", customer_success_code_visibility)
         if dev_command is not None:
             pulumi.set(__self__, "dev_command", dev_command)
+        if directory_listing is not None:
+            pulumi.set(__self__, "directory_listing", directory_listing)
         if environments is not None:
             pulumi.set(__self__, "environments", environments)
         if framework is not None:
             pulumi.set(__self__, "framework", framework)
+        if function_failover is not None:
+            pulumi.set(__self__, "function_failover", function_failover)
+        if git_comments is not None:
+            pulumi.set(__self__, "git_comments", git_comments)
+        if git_fork_protection is not None:
+            pulumi.set(__self__, "git_fork_protection", git_fork_protection)
+        if git_lfs is not None:
+            pulumi.set(__self__, "git_lfs", git_lfs)
         if git_repository is not None:
             pulumi.set(__self__, "git_repository", git_repository)
         if ignore_command is not None:
             pulumi.set(__self__, "ignore_command", ignore_command)
         if install_command is not None:
             pulumi.set(__self__, "install_command", install_command)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if output_directory is not None:
             pulumi.set(__self__, "output_directory", output_directory)
         if password_protection is not None:
             pulumi.set(__self__, "password_protection", password_protection)
+        if preview_comments is not None:
+            pulumi.set(__self__, "preview_comments", preview_comments)
+        if prioritise_production_builds is not None:
+            pulumi.set(__self__, "prioritise_production_builds", prioritise_production_builds)
         if protection_bypass_for_automation is not None:
             pulumi.set(__self__, "protection_bypass_for_automation", protection_bypass_for_automation)
         if protection_bypass_for_automation_secret is not None:
             pulumi.set(__self__, "protection_bypass_for_automation_secret", protection_bypass_for_automation_secret)
         if public_source is not None:
             pulumi.set(__self__, "public_source", public_source)
         if root_directory is not None:
             pulumi.set(__self__, "root_directory", root_directory)
         if serverless_function_region is not None:
             pulumi.set(__self__, "serverless_function_region", serverless_function_region)
+        if skew_protection is not None:
+            pulumi.set(__self__, "skew_protection", skew_protection)
         if team_id is not None:
             pulumi.set(__self__, "team_id", team_id)
         if trusted_ips is not None:
             pulumi.set(__self__, "trusted_ips", trusted_ips)
         if vercel_authentication is not None:
             pulumi.set(__self__, "vercel_authentication", vercel_authentication)
 
     @property
+    @pulumi.getter(name="autoAssignCustomDomains")
+    def auto_assign_custom_domains(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically assign custom production domains after each Production deployment via merge to the production branch or Vercel CLI deploy with --prod. Defaults to `true`
+        """
+        return pulumi.get(self, "auto_assign_custom_domains")
+
+    @auto_assign_custom_domains.setter
+    def auto_assign_custom_domains(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_assign_custom_domains", value)
+
+    @property
+    @pulumi.getter(name="automaticallyExposeSystemEnvironmentVariables")
+    def automatically_expose_system_environment_variables(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Vercel provides a set of Environment Variables that are automatically populated by the System, such as the URL of the Deployment or the name of the Git branch deployed. To expose them to your Deployments, enable this field
+        """
+        return pulumi.get(self, "automatically_expose_system_environment_variables")
+
+    @automatically_expose_system_environment_variables.setter
+    def automatically_expose_system_environment_variables(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "automatically_expose_system_environment_variables", value)
+
+    @property
     @pulumi.getter(name="buildCommand")
     def build_command(self) -> Optional[pulumi.Input[str]]:
         """
         The build command for this project. If omitted, this value will be automatically detected.
         """
         return pulumi.get(self, "build_command")
 
     @build_command.setter
     def build_command(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "build_command", value)
 
     @property
+    @pulumi.getter(name="customerSuccessCodeVisibility")
+    def customer_success_code_visibility(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Allows Vercel Customer Support to inspect all Deployments' source code in this project to assist with debugging.
+        """
+        return pulumi.get(self, "customer_success_code_visibility")
+
+    @customer_success_code_visibility.setter
+    def customer_success_code_visibility(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "customer_success_code_visibility", value)
+
+    @property
     @pulumi.getter(name="devCommand")
     def dev_command(self) -> Optional[pulumi.Input[str]]:
         """
         The dev command for this project. If omitted, this value will be automatically detected.
         """
         return pulumi.get(self, "dev_command")
 
     @dev_command.setter
     def dev_command(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dev_command", value)
 
     @property
+    @pulumi.getter(name="directoryListing")
+    def directory_listing(self) -> Optional[pulumi.Input[bool]]:
+        """
+        If no index file is present within a directory, the directory contents will be displayed.
+        """
+        return pulumi.get(self, "directory_listing")
+
+    @directory_listing.setter
+    def directory_listing(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "directory_listing", value)
+
+    @property
     @pulumi.getter
     def environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentArgs']]]]:
         """
         A set of Environment Variables that should be configured for the project.
         """
         return pulumi.get(self, "environments")
 
@@ -417,14 +685,62 @@
         return pulumi.get(self, "framework")
 
     @framework.setter
     def framework(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "framework", value)
 
     @property
+    @pulumi.getter(name="functionFailover")
+    def function_failover(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically failover Serverless Functions to the nearest region. You can customize regions through vercel.json. A new Deployment is required for your changes to take effect.
+        """
+        return pulumi.get(self, "function_failover")
+
+    @function_failover.setter
+    def function_failover(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "function_failover", value)
+
+    @property
+    @pulumi.getter(name="gitComments")
+    def git_comments(self) -> Optional[pulumi.Input['ProjectGitCommentsArgs']]:
+        """
+        Configuration for Git Comments.
+        """
+        return pulumi.get(self, "git_comments")
+
+    @git_comments.setter
+    def git_comments(self, value: Optional[pulumi.Input['ProjectGitCommentsArgs']]):
+        pulumi.set(self, "git_comments", value)
+
+    @property
+    @pulumi.getter(name="gitForkProtection")
+    def git_fork_protection(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Ensures that pull requests targeting your Git repository must be authorized by a member of your Team before deploying if your Project has Environment Variables or if the pull request includes a change to vercel.json. Defaults to `true`.
+        """
+        return pulumi.get(self, "git_fork_protection")
+
+    @git_fork_protection.setter
+    def git_fork_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "git_fork_protection", value)
+
+    @property
+    @pulumi.getter(name="gitLfs")
+    def git_lfs(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enables Git LFS support. Git LFS replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.
+        """
+        return pulumi.get(self, "git_lfs")
+
+    @git_lfs.setter
+    def git_lfs(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "git_lfs", value)
+
+    @property
     @pulumi.getter(name="gitRepository")
     def git_repository(self) -> Optional[pulumi.Input['ProjectGitRepositoryArgs']]:
         """
         The Git Repository that will be connected to the project. When this is defined, any pushes to the specified connected Git Repository will be automatically deployed. This requires the corresponding Vercel for [Github](https://vercel.com/docs/concepts/git/vercel-for-github), [Gitlab](https://vercel.com/docs/concepts/git/vercel-for-gitlab) or [Bitbucket](https://vercel.com/docs/concepts/git/vercel-for-bitbucket) plugins to be installed.
         """
         return pulumi.get(self, "git_repository")
 
@@ -489,14 +805,38 @@
         return pulumi.get(self, "password_protection")
 
     @password_protection.setter
     def password_protection(self, value: Optional[pulumi.Input['ProjectPasswordProtectionArgs']]):
         pulumi.set(self, "password_protection", value)
 
     @property
+    @pulumi.getter(name="previewComments")
+    def preview_comments(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether to enable comments on your Preview Deployments. If omitted, comments are controlled at the team level (default behaviour).
+        """
+        return pulumi.get(self, "preview_comments")
+
+    @preview_comments.setter
+    def preview_comments(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "preview_comments", value)
+
+    @property
+    @pulumi.getter(name="prioritiseProductionBuilds")
+    def prioritise_production_builds(self) -> Optional[pulumi.Input[bool]]:
+        """
+        If enabled, builds for the Production environment will be prioritized over Preview environments.
+        """
+        return pulumi.get(self, "prioritise_production_builds")
+
+    @prioritise_production_builds.setter
+    def prioritise_production_builds(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "prioritise_production_builds", value)
+
+    @property
     @pulumi.getter(name="protectionBypassForAutomation")
     def protection_bypass_for_automation(self) -> Optional[pulumi.Input[bool]]:
         """
         Allow automation services to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments on this project when using an HTTP header named `x-vercel-protection-bypass` with a value of the `password_protection_for_automation_secret` field.
         """
         return pulumi.get(self, "protection_bypass_for_automation")
 
@@ -549,14 +889,26 @@
         return pulumi.get(self, "serverless_function_region")
 
     @serverless_function_region.setter
     def serverless_function_region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "serverless_function_region", value)
 
     @property
+    @pulumi.getter(name="skewProtection")
+    def skew_protection(self) -> Optional[pulumi.Input[str]]:
+        """
+        Ensures that outdated clients always fetch the correct version for a given deployment. This value defines how long Vercel keeps Skew Protection active.
+        """
+        return pulumi.get(self, "skew_protection")
+
+    @skew_protection.setter
+    def skew_protection(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "skew_protection", value)
+
+    @property
     @pulumi.getter(name="teamId")
     def team_id(self) -> Optional[pulumi.Input[str]]:
         """
         The team ID to add the project to. Required when configuring a team resource if a default team has not been set in the provider.
         """
         return pulumi.get(self, "team_id")
 
@@ -590,36 +942,46 @@
 
 
 class Project(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 auto_assign_custom_domains: Optional[pulumi.Input[bool]] = None,
+                 automatically_expose_system_environment_variables: Optional[pulumi.Input[bool]] = None,
                  build_command: Optional[pulumi.Input[str]] = None,
+                 customer_success_code_visibility: Optional[pulumi.Input[bool]] = None,
                  dev_command: Optional[pulumi.Input[str]] = None,
+                 directory_listing: Optional[pulumi.Input[bool]] = None,
                  environments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentArgs']]]]] = None,
                  framework: Optional[pulumi.Input[str]] = None,
+                 function_failover: Optional[pulumi.Input[bool]] = None,
+                 git_comments: Optional[pulumi.Input[pulumi.InputType['ProjectGitCommentsArgs']]] = None,
+                 git_fork_protection: Optional[pulumi.Input[bool]] = None,
+                 git_lfs: Optional[pulumi.Input[bool]] = None,
                  git_repository: Optional[pulumi.Input[pulumi.InputType['ProjectGitRepositoryArgs']]] = None,
                  ignore_command: Optional[pulumi.Input[str]] = None,
                  install_command: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  output_directory: Optional[pulumi.Input[str]] = None,
                  password_protection: Optional[pulumi.Input[pulumi.InputType['ProjectPasswordProtectionArgs']]] = None,
+                 preview_comments: Optional[pulumi.Input[bool]] = None,
+                 prioritise_production_builds: Optional[pulumi.Input[bool]] = None,
                  protection_bypass_for_automation: Optional[pulumi.Input[bool]] = None,
                  public_source: Optional[pulumi.Input[bool]] = None,
                  root_directory: Optional[pulumi.Input[str]] = None,
                  serverless_function_region: Optional[pulumi.Input[str]] = None,
+                 skew_protection: Optional[pulumi.Input[str]] = None,
                  team_id: Optional[pulumi.Input[str]] = None,
                  trusted_ips: Optional[pulumi.Input[pulumi.InputType['ProjectTrustedIpsArgs']]] = None,
                  vercel_authentication: Optional[pulumi.Input[pulumi.InputType['ProjectVercelAuthenticationArgs']]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         # A project that is connected to a git repository.
         # Deployments will be created automatically
         # on every branch push and merges onto the Production Branch.
@@ -630,15 +992,14 @@
                 type="github",
             ))
         # A project that is not connected to a git repository.
         # Deployments will need to be created manually through
         # terraform, or via the vercel CLI.
         example = vercel.Project("example", framework="nextjs")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         If importing into a personal account, or with a team configured on
 
         the provider, simply use the project ID.
 
@@ -656,42 +1017,52 @@
 
         ```sh
         $ pulumi import vercel:index/project:Project example team_xxxxxxxxxxxxxxxxxxxxxxxx/prj_xxxxxxxxxxxxxxxxxxxxxxxxxxxx
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_assign_custom_domains: Automatically assign custom production domains after each Production deployment via merge to the production branch or Vercel CLI deploy with --prod. Defaults to `true`
+        :param pulumi.Input[bool] automatically_expose_system_environment_variables: Vercel provides a set of Environment Variables that are automatically populated by the System, such as the URL of the Deployment or the name of the Git branch deployed. To expose them to your Deployments, enable this field
         :param pulumi.Input[str] build_command: The build command for this project. If omitted, this value will be automatically detected.
+        :param pulumi.Input[bool] customer_success_code_visibility: Allows Vercel Customer Support to inspect all Deployments' source code in this project to assist with debugging.
         :param pulumi.Input[str] dev_command: The dev command for this project. If omitted, this value will be automatically detected.
+        :param pulumi.Input[bool] directory_listing: If no index file is present within a directory, the directory contents will be displayed.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentArgs']]]] environments: A set of Environment Variables that should be configured for the project.
         :param pulumi.Input[str] framework: The framework that is being used for this project. If omitted, no framework is selected.
+        :param pulumi.Input[bool] function_failover: Automatically failover Serverless Functions to the nearest region. You can customize regions through vercel.json. A new Deployment is required for your changes to take effect.
+        :param pulumi.Input[pulumi.InputType['ProjectGitCommentsArgs']] git_comments: Configuration for Git Comments.
+        :param pulumi.Input[bool] git_fork_protection: Ensures that pull requests targeting your Git repository must be authorized by a member of your Team before deploying if your Project has Environment Variables or if the pull request includes a change to vercel.json. Defaults to `true`.
+        :param pulumi.Input[bool] git_lfs: Enables Git LFS support. Git LFS replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.
         :param pulumi.Input[pulumi.InputType['ProjectGitRepositoryArgs']] git_repository: The Git Repository that will be connected to the project. When this is defined, any pushes to the specified connected Git Repository will be automatically deployed. This requires the corresponding Vercel for [Github](https://vercel.com/docs/concepts/git/vercel-for-github), [Gitlab](https://vercel.com/docs/concepts/git/vercel-for-gitlab) or [Bitbucket](https://vercel.com/docs/concepts/git/vercel-for-bitbucket) plugins to be installed.
         :param pulumi.Input[str] ignore_command: When a commit is pushed to the Git repository that is connected with your Project, its SHA will determine if a new Build has to be issued. If the SHA was deployed before, no new Build will be issued. You can customize this behavior with a command that exits with code 1 (new Build needed) or code 0.
         :param pulumi.Input[str] install_command: The install command for this project. If omitted, this value will be automatically detected.
         :param pulumi.Input[str] name: The desired name for the project.
         :param pulumi.Input[str] output_directory: The output directory of the project. If omitted, this value will be automatically detected.
         :param pulumi.Input[pulumi.InputType['ProjectPasswordProtectionArgs']] password_protection: Ensures visitors of your Preview Deployments must enter a password in order to gain access.
+        :param pulumi.Input[bool] preview_comments: Whether to enable comments on your Preview Deployments. If omitted, comments are controlled at the team level (default behaviour).
+        :param pulumi.Input[bool] prioritise_production_builds: If enabled, builds for the Production environment will be prioritized over Preview environments.
         :param pulumi.Input[bool] protection_bypass_for_automation: Allow automation services to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments on this project when using an HTTP header named `x-vercel-protection-bypass` with a value of the `password_protection_for_automation_secret` field.
         :param pulumi.Input[bool] public_source: By default, visitors to the `/_logs` and `/_src` paths of your Production and Preview Deployments must log in with Vercel (requires being a member of your team) to see the Source, Logs and Deployment Status of your project. Setting `public_source` to `true` disables this behaviour, meaning the Source, Logs and Deployment Status can be publicly viewed.
         :param pulumi.Input[str] root_directory: The name of a directory or relative path to the source code of your project. If omitted, it will default to the project root.
         :param pulumi.Input[str] serverless_function_region: The region on Vercel's network to which your Serverless Functions are deployed. It should be close to any data source your Serverless Function might depend on. A new Deployment is required for your changes to take effect. Please see [Vercel's documentation](https://vercel.com/docs/concepts/edge-network/regions) for a full list of regions.
+        :param pulumi.Input[str] skew_protection: Ensures that outdated clients always fetch the correct version for a given deployment. This value defines how long Vercel keeps Skew Protection active.
         :param pulumi.Input[str] team_id: The team ID to add the project to. Required when configuring a team resource if a default team has not been set in the provider.
         :param pulumi.Input[pulumi.InputType['ProjectTrustedIpsArgs']] trusted_ips: Ensures only visitors from an allowed IP address can access your deployment.
         :param pulumi.Input[pulumi.InputType['ProjectVercelAuthenticationArgs']] vercel_authentication: Ensures visitors to your Preview Deployments are logged into Vercel and have a minimum of Viewer access on your team.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProjectArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         # A project that is connected to a git repository.
         # Deployments will be created automatically
         # on every branch push and merges onto the Production Branch.
@@ -702,15 +1073,14 @@
                 type="github",
             ))
         # A project that is not connected to a git repository.
         # Deployments will need to be created manually through
         # terraform, or via the vercel CLI.
         example = vercel.Project("example", framework="nextjs")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         If importing into a personal account, or with a team configured on
 
         the provider, simply use the project ID.
 
@@ -741,153 +1111,240 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 auto_assign_custom_domains: Optional[pulumi.Input[bool]] = None,
+                 automatically_expose_system_environment_variables: Optional[pulumi.Input[bool]] = None,
                  build_command: Optional[pulumi.Input[str]] = None,
+                 customer_success_code_visibility: Optional[pulumi.Input[bool]] = None,
                  dev_command: Optional[pulumi.Input[str]] = None,
+                 directory_listing: Optional[pulumi.Input[bool]] = None,
                  environments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentArgs']]]]] = None,
                  framework: Optional[pulumi.Input[str]] = None,
+                 function_failover: Optional[pulumi.Input[bool]] = None,
+                 git_comments: Optional[pulumi.Input[pulumi.InputType['ProjectGitCommentsArgs']]] = None,
+                 git_fork_protection: Optional[pulumi.Input[bool]] = None,
+                 git_lfs: Optional[pulumi.Input[bool]] = None,
                  git_repository: Optional[pulumi.Input[pulumi.InputType['ProjectGitRepositoryArgs']]] = None,
                  ignore_command: Optional[pulumi.Input[str]] = None,
                  install_command: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  output_directory: Optional[pulumi.Input[str]] = None,
                  password_protection: Optional[pulumi.Input[pulumi.InputType['ProjectPasswordProtectionArgs']]] = None,
+                 preview_comments: Optional[pulumi.Input[bool]] = None,
+                 prioritise_production_builds: Optional[pulumi.Input[bool]] = None,
                  protection_bypass_for_automation: Optional[pulumi.Input[bool]] = None,
                  public_source: Optional[pulumi.Input[bool]] = None,
                  root_directory: Optional[pulumi.Input[str]] = None,
                  serverless_function_region: Optional[pulumi.Input[str]] = None,
+                 skew_protection: Optional[pulumi.Input[str]] = None,
                  team_id: Optional[pulumi.Input[str]] = None,
                  trusted_ips: Optional[pulumi.Input[pulumi.InputType['ProjectTrustedIpsArgs']]] = None,
                  vercel_authentication: Optional[pulumi.Input[pulumi.InputType['ProjectVercelAuthenticationArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectArgs.__new__(ProjectArgs)
 
+            __props__.__dict__["auto_assign_custom_domains"] = auto_assign_custom_domains
+            __props__.__dict__["automatically_expose_system_environment_variables"] = automatically_expose_system_environment_variables
             __props__.__dict__["build_command"] = build_command
+            __props__.__dict__["customer_success_code_visibility"] = customer_success_code_visibility
             __props__.__dict__["dev_command"] = dev_command
+            __props__.__dict__["directory_listing"] = directory_listing
             __props__.__dict__["environments"] = environments
             __props__.__dict__["framework"] = framework
+            __props__.__dict__["function_failover"] = function_failover
+            __props__.__dict__["git_comments"] = git_comments
+            __props__.__dict__["git_fork_protection"] = git_fork_protection
+            __props__.__dict__["git_lfs"] = git_lfs
             __props__.__dict__["git_repository"] = git_repository
             __props__.__dict__["ignore_command"] = ignore_command
             __props__.__dict__["install_command"] = install_command
             __props__.__dict__["name"] = name
             __props__.__dict__["output_directory"] = output_directory
             __props__.__dict__["password_protection"] = password_protection
+            __props__.__dict__["preview_comments"] = preview_comments
+            __props__.__dict__["prioritise_production_builds"] = prioritise_production_builds
             __props__.__dict__["protection_bypass_for_automation"] = protection_bypass_for_automation
             __props__.__dict__["public_source"] = public_source
             __props__.__dict__["root_directory"] = root_directory
             __props__.__dict__["serverless_function_region"] = serverless_function_region
+            __props__.__dict__["skew_protection"] = skew_protection
             __props__.__dict__["team_id"] = team_id
             __props__.__dict__["trusted_ips"] = trusted_ips
             __props__.__dict__["vercel_authentication"] = vercel_authentication
             __props__.__dict__["protection_bypass_for_automation_secret"] = None
         super(Project, __self__).__init__(
             'vercel:index/project:Project',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            auto_assign_custom_domains: Optional[pulumi.Input[bool]] = None,
+            automatically_expose_system_environment_variables: Optional[pulumi.Input[bool]] = None,
             build_command: Optional[pulumi.Input[str]] = None,
+            customer_success_code_visibility: Optional[pulumi.Input[bool]] = None,
             dev_command: Optional[pulumi.Input[str]] = None,
+            directory_listing: Optional[pulumi.Input[bool]] = None,
             environments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentArgs']]]]] = None,
             framework: Optional[pulumi.Input[str]] = None,
+            function_failover: Optional[pulumi.Input[bool]] = None,
+            git_comments: Optional[pulumi.Input[pulumi.InputType['ProjectGitCommentsArgs']]] = None,
+            git_fork_protection: Optional[pulumi.Input[bool]] = None,
+            git_lfs: Optional[pulumi.Input[bool]] = None,
             git_repository: Optional[pulumi.Input[pulumi.InputType['ProjectGitRepositoryArgs']]] = None,
             ignore_command: Optional[pulumi.Input[str]] = None,
             install_command: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             output_directory: Optional[pulumi.Input[str]] = None,
             password_protection: Optional[pulumi.Input[pulumi.InputType['ProjectPasswordProtectionArgs']]] = None,
+            preview_comments: Optional[pulumi.Input[bool]] = None,
+            prioritise_production_builds: Optional[pulumi.Input[bool]] = None,
             protection_bypass_for_automation: Optional[pulumi.Input[bool]] = None,
             protection_bypass_for_automation_secret: Optional[pulumi.Input[str]] = None,
             public_source: Optional[pulumi.Input[bool]] = None,
             root_directory: Optional[pulumi.Input[str]] = None,
             serverless_function_region: Optional[pulumi.Input[str]] = None,
+            skew_protection: Optional[pulumi.Input[str]] = None,
             team_id: Optional[pulumi.Input[str]] = None,
             trusted_ips: Optional[pulumi.Input[pulumi.InputType['ProjectTrustedIpsArgs']]] = None,
             vercel_authentication: Optional[pulumi.Input[pulumi.InputType['ProjectVercelAuthenticationArgs']]] = None) -> 'Project':
         """
         Get an existing Project resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_assign_custom_domains: Automatically assign custom production domains after each Production deployment via merge to the production branch or Vercel CLI deploy with --prod. Defaults to `true`
+        :param pulumi.Input[bool] automatically_expose_system_environment_variables: Vercel provides a set of Environment Variables that are automatically populated by the System, such as the URL of the Deployment or the name of the Git branch deployed. To expose them to your Deployments, enable this field
         :param pulumi.Input[str] build_command: The build command for this project. If omitted, this value will be automatically detected.
+        :param pulumi.Input[bool] customer_success_code_visibility: Allows Vercel Customer Support to inspect all Deployments' source code in this project to assist with debugging.
         :param pulumi.Input[str] dev_command: The dev command for this project. If omitted, this value will be automatically detected.
+        :param pulumi.Input[bool] directory_listing: If no index file is present within a directory, the directory contents will be displayed.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentArgs']]]] environments: A set of Environment Variables that should be configured for the project.
         :param pulumi.Input[str] framework: The framework that is being used for this project. If omitted, no framework is selected.
+        :param pulumi.Input[bool] function_failover: Automatically failover Serverless Functions to the nearest region. You can customize regions through vercel.json. A new Deployment is required for your changes to take effect.
+        :param pulumi.Input[pulumi.InputType['ProjectGitCommentsArgs']] git_comments: Configuration for Git Comments.
+        :param pulumi.Input[bool] git_fork_protection: Ensures that pull requests targeting your Git repository must be authorized by a member of your Team before deploying if your Project has Environment Variables or if the pull request includes a change to vercel.json. Defaults to `true`.
+        :param pulumi.Input[bool] git_lfs: Enables Git LFS support. Git LFS replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.
         :param pulumi.Input[pulumi.InputType['ProjectGitRepositoryArgs']] git_repository: The Git Repository that will be connected to the project. When this is defined, any pushes to the specified connected Git Repository will be automatically deployed. This requires the corresponding Vercel for [Github](https://vercel.com/docs/concepts/git/vercel-for-github), [Gitlab](https://vercel.com/docs/concepts/git/vercel-for-gitlab) or [Bitbucket](https://vercel.com/docs/concepts/git/vercel-for-bitbucket) plugins to be installed.
         :param pulumi.Input[str] ignore_command: When a commit is pushed to the Git repository that is connected with your Project, its SHA will determine if a new Build has to be issued. If the SHA was deployed before, no new Build will be issued. You can customize this behavior with a command that exits with code 1 (new Build needed) or code 0.
         :param pulumi.Input[str] install_command: The install command for this project. If omitted, this value will be automatically detected.
         :param pulumi.Input[str] name: The desired name for the project.
         :param pulumi.Input[str] output_directory: The output directory of the project. If omitted, this value will be automatically detected.
         :param pulumi.Input[pulumi.InputType['ProjectPasswordProtectionArgs']] password_protection: Ensures visitors of your Preview Deployments must enter a password in order to gain access.
+        :param pulumi.Input[bool] preview_comments: Whether to enable comments on your Preview Deployments. If omitted, comments are controlled at the team level (default behaviour).
+        :param pulumi.Input[bool] prioritise_production_builds: If enabled, builds for the Production environment will be prioritized over Preview environments.
         :param pulumi.Input[bool] protection_bypass_for_automation: Allow automation services to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments on this project when using an HTTP header named `x-vercel-protection-bypass` with a value of the `password_protection_for_automation_secret` field.
         :param pulumi.Input[str] protection_bypass_for_automation_secret: If `protection_bypass_for_automation` is enabled, use this value in the `x-vercel-protection-bypass` header to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments.
         :param pulumi.Input[bool] public_source: By default, visitors to the `/_logs` and `/_src` paths of your Production and Preview Deployments must log in with Vercel (requires being a member of your team) to see the Source, Logs and Deployment Status of your project. Setting `public_source` to `true` disables this behaviour, meaning the Source, Logs and Deployment Status can be publicly viewed.
         :param pulumi.Input[str] root_directory: The name of a directory or relative path to the source code of your project. If omitted, it will default to the project root.
         :param pulumi.Input[str] serverless_function_region: The region on Vercel's network to which your Serverless Functions are deployed. It should be close to any data source your Serverless Function might depend on. A new Deployment is required for your changes to take effect. Please see [Vercel's documentation](https://vercel.com/docs/concepts/edge-network/regions) for a full list of regions.
+        :param pulumi.Input[str] skew_protection: Ensures that outdated clients always fetch the correct version for a given deployment. This value defines how long Vercel keeps Skew Protection active.
         :param pulumi.Input[str] team_id: The team ID to add the project to. Required when configuring a team resource if a default team has not been set in the provider.
         :param pulumi.Input[pulumi.InputType['ProjectTrustedIpsArgs']] trusted_ips: Ensures only visitors from an allowed IP address can access your deployment.
         :param pulumi.Input[pulumi.InputType['ProjectVercelAuthenticationArgs']] vercel_authentication: Ensures visitors to your Preview Deployments are logged into Vercel and have a minimum of Viewer access on your team.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectState.__new__(_ProjectState)
 
+        __props__.__dict__["auto_assign_custom_domains"] = auto_assign_custom_domains
+        __props__.__dict__["automatically_expose_system_environment_variables"] = automatically_expose_system_environment_variables
         __props__.__dict__["build_command"] = build_command
+        __props__.__dict__["customer_success_code_visibility"] = customer_success_code_visibility
         __props__.__dict__["dev_command"] = dev_command
+        __props__.__dict__["directory_listing"] = directory_listing
         __props__.__dict__["environments"] = environments
         __props__.__dict__["framework"] = framework
+        __props__.__dict__["function_failover"] = function_failover
+        __props__.__dict__["git_comments"] = git_comments
+        __props__.__dict__["git_fork_protection"] = git_fork_protection
+        __props__.__dict__["git_lfs"] = git_lfs
         __props__.__dict__["git_repository"] = git_repository
         __props__.__dict__["ignore_command"] = ignore_command
         __props__.__dict__["install_command"] = install_command
         __props__.__dict__["name"] = name
         __props__.__dict__["output_directory"] = output_directory
         __props__.__dict__["password_protection"] = password_protection
+        __props__.__dict__["preview_comments"] = preview_comments
+        __props__.__dict__["prioritise_production_builds"] = prioritise_production_builds
         __props__.__dict__["protection_bypass_for_automation"] = protection_bypass_for_automation
         __props__.__dict__["protection_bypass_for_automation_secret"] = protection_bypass_for_automation_secret
         __props__.__dict__["public_source"] = public_source
         __props__.__dict__["root_directory"] = root_directory
         __props__.__dict__["serverless_function_region"] = serverless_function_region
+        __props__.__dict__["skew_protection"] = skew_protection
         __props__.__dict__["team_id"] = team_id
         __props__.__dict__["trusted_ips"] = trusted_ips
         __props__.__dict__["vercel_authentication"] = vercel_authentication
         return Project(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="autoAssignCustomDomains")
+    def auto_assign_custom_domains(self) -> pulumi.Output[bool]:
+        """
+        Automatically assign custom production domains after each Production deployment via merge to the production branch or Vercel CLI deploy with --prod. Defaults to `true`
+        """
+        return pulumi.get(self, "auto_assign_custom_domains")
+
+    @property
+    @pulumi.getter(name="automaticallyExposeSystemEnvironmentVariables")
+    def automatically_expose_system_environment_variables(self) -> pulumi.Output[bool]:
+        """
+        Vercel provides a set of Environment Variables that are automatically populated by the System, such as the URL of the Deployment or the name of the Git branch deployed. To expose them to your Deployments, enable this field
+        """
+        return pulumi.get(self, "automatically_expose_system_environment_variables")
+
+    @property
     @pulumi.getter(name="buildCommand")
     def build_command(self) -> pulumi.Output[Optional[str]]:
         """
         The build command for this project. If omitted, this value will be automatically detected.
         """
         return pulumi.get(self, "build_command")
 
     @property
+    @pulumi.getter(name="customerSuccessCodeVisibility")
+    def customer_success_code_visibility(self) -> pulumi.Output[bool]:
+        """
+        Allows Vercel Customer Support to inspect all Deployments' source code in this project to assist with debugging.
+        """
+        return pulumi.get(self, "customer_success_code_visibility")
+
+    @property
     @pulumi.getter(name="devCommand")
     def dev_command(self) -> pulumi.Output[Optional[str]]:
         """
         The dev command for this project. If omitted, this value will be automatically detected.
         """
         return pulumi.get(self, "dev_command")
 
     @property
+    @pulumi.getter(name="directoryListing")
+    def directory_listing(self) -> pulumi.Output[bool]:
+        """
+        If no index file is present within a directory, the directory contents will be displayed.
+        """
+        return pulumi.get(self, "directory_listing")
+
+    @property
     @pulumi.getter
     def environments(self) -> pulumi.Output[Optional[Sequence['outputs.ProjectEnvironment']]]:
         """
         A set of Environment Variables that should be configured for the project.
         """
         return pulumi.get(self, "environments")
 
@@ -896,14 +1353,46 @@
     def framework(self) -> pulumi.Output[Optional[str]]:
         """
         The framework that is being used for this project. If omitted, no framework is selected.
         """
         return pulumi.get(self, "framework")
 
     @property
+    @pulumi.getter(name="functionFailover")
+    def function_failover(self) -> pulumi.Output[bool]:
+        """
+        Automatically failover Serverless Functions to the nearest region. You can customize regions through vercel.json. A new Deployment is required for your changes to take effect.
+        """
+        return pulumi.get(self, "function_failover")
+
+    @property
+    @pulumi.getter(name="gitComments")
+    def git_comments(self) -> pulumi.Output[Optional['outputs.ProjectGitComments']]:
+        """
+        Configuration for Git Comments.
+        """
+        return pulumi.get(self, "git_comments")
+
+    @property
+    @pulumi.getter(name="gitForkProtection")
+    def git_fork_protection(self) -> pulumi.Output[bool]:
+        """
+        Ensures that pull requests targeting your Git repository must be authorized by a member of your Team before deploying if your Project has Environment Variables or if the pull request includes a change to vercel.json. Defaults to `true`.
+        """
+        return pulumi.get(self, "git_fork_protection")
+
+    @property
+    @pulumi.getter(name="gitLfs")
+    def git_lfs(self) -> pulumi.Output[bool]:
+        """
+        Enables Git LFS support. Git LFS replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.
+        """
+        return pulumi.get(self, "git_lfs")
+
+    @property
     @pulumi.getter(name="gitRepository")
     def git_repository(self) -> pulumi.Output[Optional['outputs.ProjectGitRepository']]:
         """
         The Git Repository that will be connected to the project. When this is defined, any pushes to the specified connected Git Repository will be automatically deployed. This requires the corresponding Vercel for [Github](https://vercel.com/docs/concepts/git/vercel-for-github), [Gitlab](https://vercel.com/docs/concepts/git/vercel-for-gitlab) or [Bitbucket](https://vercel.com/docs/concepts/git/vercel-for-bitbucket) plugins to be installed.
         """
         return pulumi.get(self, "git_repository")
 
@@ -944,14 +1433,30 @@
     def password_protection(self) -> pulumi.Output[Optional['outputs.ProjectPasswordProtection']]:
         """
         Ensures visitors of your Preview Deployments must enter a password in order to gain access.
         """
         return pulumi.get(self, "password_protection")
 
     @property
+    @pulumi.getter(name="previewComments")
+    def preview_comments(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Whether to enable comments on your Preview Deployments. If omitted, comments are controlled at the team level (default behaviour).
+        """
+        return pulumi.get(self, "preview_comments")
+
+    @property
+    @pulumi.getter(name="prioritiseProductionBuilds")
+    def prioritise_production_builds(self) -> pulumi.Output[bool]:
+        """
+        If enabled, builds for the Production environment will be prioritized over Preview environments.
+        """
+        return pulumi.get(self, "prioritise_production_builds")
+
+    @property
     @pulumi.getter(name="protectionBypassForAutomation")
     def protection_bypass_for_automation(self) -> pulumi.Output[Optional[bool]]:
         """
         Allow automation services to bypass Vercel Authentication and Password Protection for both Preview and Production Deployments on this project when using an HTTP header named `x-vercel-protection-bypass` with a value of the `password_protection_for_automation_secret` field.
         """
         return pulumi.get(self, "protection_bypass_for_automation")
 
@@ -984,14 +1489,22 @@
     def serverless_function_region(self) -> pulumi.Output[str]:
         """
         The region on Vercel's network to which your Serverless Functions are deployed. It should be close to any data source your Serverless Function might depend on. A new Deployment is required for your changes to take effect. Please see [Vercel's documentation](https://vercel.com/docs/concepts/edge-network/regions) for a full list of regions.
         """
         return pulumi.get(self, "serverless_function_region")
 
     @property
+    @pulumi.getter(name="skewProtection")
+    def skew_protection(self) -> pulumi.Output[Optional[str]]:
+        """
+        Ensures that outdated clients always fetch the correct version for a given deployment. This value defines how long Vercel keeps Skew Protection active.
+        """
+        return pulumi.get(self, "skew_protection")
+
+    @property
     @pulumi.getter(name="teamId")
     def team_id(self) -> pulumi.Output[str]:
         """
         The team ID to add the project to. Required when configuring a team resource if a default team has not been set in the provider.
         """
         return pulumi.get(self, "team_id")
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/project_domain.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/project_domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,14 @@
 
         A Project Domain is used to associate a domain name with a `Project`.
 
         By default, Project Domains will be automatically applied to any `production` deployments.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         example_project = vercel.Project("exampleProject")
         # A simple domain that will be automatically
         # applied to each production deployment
@@ -253,15 +252,14 @@
         # The status_code can optionally be controlled.
         example_redirect = vercel.ProjectDomain("exampleRedirect",
             project_id=example_project.id,
             domain="i-also-love.vercel.app",
             redirect=example_project_domain.domain,
             redirect_status_code=307)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         If importing into a personal account, or with a team configured on
 
         the provider, simply use the project ID and domain.
 
@@ -301,15 +299,14 @@
 
         A Project Domain is used to associate a domain name with a `Project`.
 
         By default, Project Domains will be automatically applied to any `production` deployments.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         example_project = vercel.Project("exampleProject")
         # A simple domain that will be automatically
         # applied to each production deployment
@@ -320,15 +317,14 @@
         # The status_code can optionally be controlled.
         example_redirect = vercel.ProjectDomain("exampleRedirect",
             project_id=example_project.id,
             domain="i-also-love.vercel.app",
             redirect=example_project_domain.domain,
             redirect_status_code=307)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         If importing into a personal account, or with a team configured on
 
         the provider, simply use the project ID and domain.
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/project_environment_variable.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/project_environment_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,14 @@
                  targets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  team_id: Optional[pulumi.Input[str]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         example_project = vercel.Project("exampleProject", git_repository=vercel.ProjectGitRepositoryArgs(
             type="github",
             repo="vercel/some-repo",
@@ -292,25 +291,26 @@
         example_sensitive = vercel.ProjectEnvironmentVariable("exampleSensitive",
             project_id=example_project.id,
             key="foo",
             value="bar-production",
             targets=["production"],
             sensitive=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         If importing into a personal account, or with a team configured on
 
         the provider, simply use the project_id and environment variable id.
 
         - project_id can be found in the project `settings` tab in the Vercel UI.
 
-        - environment variable id is hard to find, but can be taken from the network tab, inside developer tools, on the project page.
+        - environment variable id can be taken from the network tab inside developer tools, while you are on the project page,
+
+        or can be queried from Vercel API directly (https://vercel.com/docs/rest-api/endpoints/projects#retrieve-the-environment-variables-of-a-project-by-id-or-name)
 
         # 
 
         Note also, that the value field for sensitive environment variables will be imported as `null`.
 
         ```sh
         $ pulumi import vercel:index/projectEnvironmentVariable:ProjectEnvironmentVariable example prj_xxxxxxxxxxxxxxxxxxxxxxxxxxxx/FdT2e1E5Of6Cihmt
@@ -320,15 +320,17 @@
 
         environment variable id.
 
         - team_id can be found in the team `settings` tab in the Vercel UI.
 
         - project_id can be found in the project `settings` tab in the Vercel UI.
 
-        - environment variable id is hard to find, but can be taken from the network tab, inside developer tools, on the project page.
+        - environment variable id can be taken from the network tab inside developer tools, while you are on the project page,
+
+        or can be queried from Vercel API directly (https://vercel.com/docs/rest-api/endpoints/projects#retrieve-the-environment-variables-of-a-project-by-id-or-name)
 
         # 
 
         Note also, that the value field for sensitive environment variables will be imported as `null`.
 
         ```sh
         $ pulumi import vercel:index/projectEnvironmentVariable:ProjectEnvironmentVariable example team_xxxxxxxxxxxxxxxxxxxxxxxx/prj_xxxxxxxxxxxxxxxxxxxxxxxxxxxx/FdT2e1E5Of6Cihmt
@@ -349,15 +351,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectEnvironmentVariableArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         example_project = vercel.Project("exampleProject", git_repository=vercel.ProjectGitRepositoryArgs(
             type="github",
             repo="vercel/some-repo",
@@ -382,25 +383,26 @@
         example_sensitive = vercel.ProjectEnvironmentVariable("exampleSensitive",
             project_id=example_project.id,
             key="foo",
             value="bar-production",
             targets=["production"],
             sensitive=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         If importing into a personal account, or with a team configured on
 
         the provider, simply use the project_id and environment variable id.
 
         - project_id can be found in the project `settings` tab in the Vercel UI.
 
-        - environment variable id is hard to find, but can be taken from the network tab, inside developer tools, on the project page.
+        - environment variable id can be taken from the network tab inside developer tools, while you are on the project page,
+
+        or can be queried from Vercel API directly (https://vercel.com/docs/rest-api/endpoints/projects#retrieve-the-environment-variables-of-a-project-by-id-or-name)
 
         # 
 
         Note also, that the value field for sensitive environment variables will be imported as `null`.
 
         ```sh
         $ pulumi import vercel:index/projectEnvironmentVariable:ProjectEnvironmentVariable example prj_xxxxxxxxxxxxxxxxxxxxxxxxxxxx/FdT2e1E5Of6Cihmt
@@ -410,15 +412,17 @@
 
         environment variable id.
 
         - team_id can be found in the team `settings` tab in the Vercel UI.
 
         - project_id can be found in the project `settings` tab in the Vercel UI.
 
-        - environment variable id is hard to find, but can be taken from the network tab, inside developer tools, on the project page.
+        - environment variable id can be taken from the network tab inside developer tools, while you are on the project page,
+
+        or can be queried from Vercel API directly (https://vercel.com/docs/rest-api/endpoints/projects#retrieve-the-environment-variables-of-a-project-by-id-or-name)
 
         # 
 
         Note also, that the value field for sensitive environment variables will be imported as `null`.
 
         ```sh
         $ pulumi import vercel:index/projectEnvironmentVariable:ProjectEnvironmentVariable example team_xxxxxxxxxxxxxxxxxxxxxxxx/prj_xxxxxxxxxxxxxxxxxxxxxxxxxxxx/FdT2e1E5Of6Cihmt
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/provider.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel/shared_environment_variable.py` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel/shared_environment_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,14 @@
 
         A Shared Environment Variable resource defines an Environment Variable that can be shared between multiple Vercel Projects.
 
         For more detailed information, please see the [Vercel documentation](https://vercel.com/docs/concepts/projects/environment-variables/shared-environment-variables).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         example_project = vercel.Project("exampleProject", git_repository=vercel.ProjectGitRepositoryArgs(
             type="github",
             repo="vercel/some-repo",
@@ -249,23 +248,22 @@
         # and associated with the "example" project.
         example_shared_environment_variable = vercel.SharedEnvironmentVariable("exampleSharedEnvironmentVariable",
             key="EXAMPLE",
             value="some_value",
             targets=["production"],
             project_ids=[example_project.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         You can import via the team_id and environment variable id.
 
         - team_id can be found in the team `settings` tab in the Vercel UI.
 
-        - environment variable id is hard to find, but can be taken from the network tab, inside developer tools, on the shared environment variable page.
+        - environment variable id can be taken from the network tab inside developer tools, while you are on the project page.
 
         # 
 
         Note also, that the value field for sensitive environment variables will be imported as `null`.
 
         ```sh
         $ pulumi import vercel:index/sharedEnvironmentVariable:SharedEnvironmentVariable example team_xxxxxxxxxxxxxxxxxxxxxxxx/env_yyyyyyyyyyyyy
@@ -291,15 +289,14 @@
 
         A Shared Environment Variable resource defines an Environment Variable that can be shared between multiple Vercel Projects.
 
         For more detailed information, please see the [Vercel documentation](https://vercel.com/docs/concepts/projects/environment-variables/shared-environment-variables).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_vercel as vercel
 
         example_project = vercel.Project("exampleProject", git_repository=vercel.ProjectGitRepositoryArgs(
             type="github",
             repo="vercel/some-repo",
@@ -308,23 +305,22 @@
         # and associated with the "example" project.
         example_shared_environment_variable = vercel.SharedEnvironmentVariable("exampleSharedEnvironmentVariable",
             key="EXAMPLE",
             value="some_value",
             targets=["production"],
             project_ids=[example_project.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         You can import via the team_id and environment variable id.
 
         - team_id can be found in the team `settings` tab in the Vercel UI.
 
-        - environment variable id is hard to find, but can be taken from the network tab, inside developer tools, on the shared environment variable page.
+        - environment variable id can be taken from the network tab inside developer tools, while you are on the project page.
 
         # 
 
         Note also, that the value field for sensitive environment variables will be imported as `null`.
 
         ```sh
         $ pulumi import vercel:index/sharedEnvironmentVariable:SharedEnvironmentVariable example team_xxxxxxxxxxxxxxxxxxxxxxxx/env_yyyyyyyyyyyyy
```

### Comparing `pulumiverse_vercel-1.3.0/pulumiverse_vercel.egg-info/PKG-INFO` & `pulumiverse_vercel-1.9.0/pulumiverse_vercel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-vercel
-Version: 1.3.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-vercel
 Keywords: pulumi vercel category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_vercel-1.3.0/setup.py` & `pulumiverse_vercel-1.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0"
+VERSION = "1.9.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "vercel Pulumi Package - Development Version"
```

