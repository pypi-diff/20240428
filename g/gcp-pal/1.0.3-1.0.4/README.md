# Comparing `tmp/gcp_pal-1.0.3.tar.gz` & `tmp/gcp_pal-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-1.0.3.tar", max compression
+gzip compressed data, was "gcp_pal-1.0.4.tar", max compression
```

## Comparing `gcp_pal-1.0.3.tar` & `gcp_pal-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    23782 2024-04-25 23:01:53.623017 gcp_pal-1.0.3/README.md
--rw-r--r--   0        0        0      810 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31402 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13855 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0      965 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    12490 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/firestore.py
--rw-r--r--   0        0        0     2248 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/project.py
--rw-r--r--   0        0        0     1674 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6860 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17133 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       82 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0      935 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/utils/lazy_loader.py
--rw-r--r--   0        0        0    11329 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0      958 2024-04-25 23:01:53.627017 gcp_pal-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    24172 1970-01-01 00:00:00.000000 gcp_pal-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    25169 2024-04-27 23:17:45.290956 gcp_pal-1.0.4/README.md
+-rw-r--r--   0        0        0      810 2024-04-27 23:17:45.290956 gcp_pal-1.0.4/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31402 2024-04-27 23:17:45.290956 gcp_pal-1.0.4/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-27 23:17:45.290956 gcp_pal-1.0.4/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13855 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    12490 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     3170 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/project.py
+-rw-r--r--   0        0        0     1674 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6860 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17133 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    11431 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0      958 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    25559 1970-01-01 00:00:00.000000 gcp_pal-1.0.4/PKG-INFO
```

### Comparing `gcp_pal-1.0.3/README.md` & `gcp_pal-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 [x] Cloud Run Module
 [x] Logging Module
 [x] Secret Manager Module
 [x] Cloud Scheduler Module
 [x] Add examples
 [x] Publish to PyPI
 [x] Tests
+[x] Project Module
 ...
 -->
 
 # GCP Pal Library
 
 The `gcp-pal` library provides a set of utilities for interacting with Google Cloud Platform (GCP) services, streamlining the process of implementing GCP functionalities within your Python applications.
 
@@ -953,7 +954,74 @@
 If the job is paused, it will be resumed before running. To prevent this, set the `force` parameter to `False`:
 
 ```python
 CloudScheduler("job-name").run(force=False)
 # Output: Cloud Scheduler job "job-name" not run if it is paused
 ```
 
+
+---
+
+## Project Module
+
+The Project module in the `gcp-pal` library allows you to access and manage Google Cloud projects.
+
+### Initializing Project
+
+Import the Project class from the `gcp_pal` module:
+
+```python
+from gcp_pal import Project
+```
+
+### Listing projects
+
+To list all projects available to the authenticated user, use the `ls` method:
+
+```python
+projects = Project().ls()
+print(projects)
+# Output: ['project1', 'project2']
+```
+
+### Creating projects
+
+To create a new project, use the `create` method:
+
+```python
+Project("new-project").create()
+# Output: Project "new-project" created
+```
+
+### Deleting projects
+
+To delete a project, use the `delete` method:
+
+```python
+Project("project-name").delete()
+# Output: Project "project-name" deleted
+```
+
+Google Cloud will delete the project after 30 days. During this time, to undelete a project, use the `undelete` method:
+
+```python
+Project("project-name").undelete()
+# Output: Project "project-name" undeleted
+```
+
+### Getting project details
+
+To get the details of a project, use the `get` method:
+
+```python
+details = Project("project-name").get()
+print(details)
+# Output: {'name': 'projects/project-id', 'project_id': 'project-id', ...}
+```
+
+To obtain the project number use the `number` method:
+
+```python
+project_number = Project("project-name").number()
+print(project_number)
+# Output: "1234567890"
+```
```

### Comparing `gcp_pal-1.0.3/gcp_pal/__init__.py` & `gcp_pal-1.0.4/gcp_pal/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/bigquery.py` & `gcp_pal-1.0.4/gcp_pal/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/cloudfunctions.py` & `gcp_pal-1.0.4/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/cloudrun.py` & `gcp_pal-1.0.4/gcp_pal/cloudrun.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/cloudscheduler.py` & `gcp_pal-1.0.4/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/config/vars.py` & `gcp_pal-1.0.4/gcp_pal/config/vars.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/firestore.py` & `gcp_pal-1.0.4/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/project.py` & `gcp_pal-1.0.4/gcp_pal/project.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 class Project:
 
     _clients = {}
 
     def __init__(self, project_id: str = None, folder: str = None):
         self.project_id = (
-            project_id or os.environ.get("PROJECT") or get_auth_default()[1]
+            project_id
+            or os.environ.get("PROJECT")
+            or get_auth_default(errors="ignore")[1]
         )
         self.folder = folder
         self.parent = f"folders/{self.folder}" if self.folder else None
         self.name = f"projects/{self.project_id}"
 
         if self.project_id in Project._clients:
             self.client = Project._clients[self.project_id]
@@ -40,22 +42,32 @@
         output = self.client.create_project(project=project)
         output = output.result(timeout=300)
         log(f"Project - Created project '{self.project_id}'.")
         return output
 
     def delete(self):
         """
-        Deletes a project.
+        Deletes a project. It will be marked for deletion, and will be deleted after 30 days.
 
         Returns:
         - None
         """
         self.client.delete_project(name=self.name)
         log(f"Project - Deleted project '{self.project_id}'.")
 
+    def undelete(self):
+        """
+        Restores a project which has been marked for deletion.
+
+        Returns:
+        - None
+        """
+        self.client.undelete_project(name=self.name)
+        log(f"Project - Restored project '{self.project_id}'.")
+
     def ls(self, active_only: bool = True):
         """
         Lists all projects which are available to the caller.
 
         Args:
         - active_only: (bool) If True, only return active projects. This filters out projects that are marked for deletion.
 
@@ -65,10 +77,32 @@
         projects = self.client.search_projects()
         projects = [x for x in projects]
         if active_only:
             projects = [x for x in projects if x.state.name == "ACTIVE"]
         project_ids = [x.project_id for x in projects]
         return project_ids
 
+    def get(self):
+        """
+        Retrieves the project identified by the specified project ID.
+
+        Returns:
+        - google.cloud.resourcemanager_v3.types.Project
+        """
+        project = self.client.get_project(name=self.name)
+        return project
+
+    def number(self):
+        """
+        Retrieves the project number.
+
+        Returns:
+        - (str) Project number (e.g. '123456789012')
+        """
+        got = self.get()
+        output = got.name.split("/")[-1]
+        return output
+
 
 if __name__ == "__main__":
-    print(Project().ls(active_only=True))
+    # print(Project().ls(active_only=True))
+    print(Project("vitaminb16").get())
```

### Comparing `gcp_pal-1.0.3/gcp_pal/pubsub.py` & `gcp_pal-1.0.4/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/pydocker.py` & `gcp_pal-1.0.4/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/pylogging.py` & `gcp_pal-1.0.4/gcp_pal/pylogging.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/request.py` & `gcp_pal-1.0.4/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/schema.py` & `gcp_pal-1.0.4/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/secretmanager.py` & `gcp_pal-1.0.4/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/storage/parquet.py` & `gcp_pal-1.0.4/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/storage/storage.py` & `gcp_pal-1.0.4/gcp_pal/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/utils/lazy_loader.py` & `gcp_pal-1.0.4/gcp_pal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.3/gcp_pal/utils/utils.py` & `gcp_pal-1.0.4/gcp_pal/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,18 +288,21 @@
         range_n = range(n_values)
         output = {k: [d[i][k] for i in range_n] for k in keys}
     else:
         output = d
     return output
 
 
-def get_auth_default(errors="raise"):
+def get_auth_default(allow_none=False, errors="raise"):
     """
     Get the default project from google.auth.default() and store it in an environment variable.
 
+    Args:
+    - errors (str): The error handling method. Can be "raise" or "warn".
+
     Returns:
     - str: The default project.
     """
     try_import("google.auth", "get_default_project")
     import google.auth as google_auth
 
     project = os.getenv("_GOOGLE_AUTH_DEFAULT_PROJECT", None)
```

### Comparing `gcp_pal-1.0.3/pyproject.toml` & `gcp_pal-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gcp_pal-1.0.3/PKG-INFO` & `gcp_pal-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,14 +25,15 @@
 [x] Cloud Run Module
 [x] Logging Module
 [x] Secret Manager Module
 [x] Cloud Scheduler Module
 [x] Add examples
 [x] Publish to PyPI
 [x] Tests
+[x] Project Module
 ...
 -->
 
 # GCP Pal Library
 
 The `gcp-pal` library provides a set of utilities for interacting with Google Cloud Platform (GCP) services, streamlining the process of implementing GCP functionalities within your Python applications.
 
@@ -967,7 +968,73 @@
 
 ```python
 CloudScheduler("job-name").run(force=False)
 # Output: Cloud Scheduler job "job-name" not run if it is paused
 ```
 
 
+---
+
+## Project Module
+
+The Project module in the `gcp-pal` library allows you to access and manage Google Cloud projects.
+
+### Initializing Project
+
+Import the Project class from the `gcp_pal` module:
+
+```python
+from gcp_pal import Project
+```
+
+### Listing projects
+
+To list all projects available to the authenticated user, use the `ls` method:
+
+```python
+projects = Project().ls()
+print(projects)
+# Output: ['project1', 'project2']
+```
+
+### Creating projects
+
+To create a new project, use the `create` method:
+
+```python
+Project("new-project").create()
+# Output: Project "new-project" created
+```
+
+### Deleting projects
+
+To delete a project, use the `delete` method:
+
+```python
+Project("project-name").delete()
+# Output: Project "project-name" deleted
+```
+
+Google Cloud will delete the project after 30 days. During this time, to undelete a project, use the `undelete` method:
+
+```python
+Project("project-name").undelete()
+# Output: Project "project-name" undeleted
+```
+
+### Getting project details
+
+To get the details of a project, use the `get` method:
+
+```python
+details = Project("project-name").get()
+print(details)
+# Output: {'name': 'projects/project-id', 'project_id': 'project-id', ...}
+```
+
+To obtain the project number use the `number` method:
+
+```python
+project_number = Project("project-name").number()
+print(project_number)
+# Output: "1234567890"
+```
```

