# Comparing `tmp/lit_data_layers-0.1.2.tar.gz` & `tmp/lit_data_layers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lit_data_layers-0.1.2.tar", max compression
+gzip compressed data, was "lit_data_layers-0.1.3.tar", max compression
```

## Comparing `lit_data_layers-0.1.2.tar` & `lit_data_layers-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-01 17:39:40.930046 lit_data_layers-0.1.2/LICENSE
--rw-r--r--   0        0        0     1712 2024-04-02 13:00:23.234734 lit_data_layers-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-01 17:39:40.968049 lit_data_layers-0.1.2/lit_data_layers/__init__.py
--rw-r--r--   0        0        0    24525 2024-04-28 07:04:24.358082 lit_data_layers-0.1.2/lit_data_layers/sqldb/__init__.py
--rw-r--r--   0        0        0     3618 2024-04-28 07:04:24.358401 lit_data_layers-0.1.2/lit_data_layers/sqldb/models.py
--rw-r--r--   0        0        0      641 2024-04-28 07:04:24.358848 lit_data_layers-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 lit_data_layers-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 17:39:40.930046 lit_data_layers-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1712 2024-04-02 13:00:23.234734 lit_data_layers-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 17:39:40.968049 lit_data_layers-0.1.3/lit_data_layers/__init__.py
+-rw-r--r--   0        0        0    24138 2024-04-28 07:28:43.929442 lit_data_layers-0.1.3/lit_data_layers/sqldb/__init__.py
+-rw-r--r--   0        0        0     3618 2024-04-28 07:04:24.358401 lit_data_layers-0.1.3/lit_data_layers/sqldb/models.py
+-rw-r--r--   0        0        0      641 2024-04-28 07:29:46.949732 lit_data_layers-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 lit_data_layers-0.1.3/PKG-INFO
```

### Comparing `lit_data_layers-0.1.2/LICENSE` & `lit_data_layers-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lit_data_layers-0.1.2/README.md` & `lit_data_layers-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lit_data_layers-0.1.2/lit_data_layers/sqldb/__init__.py` & `lit_data_layers-0.1.3/lit_data_layers/sqldb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         """
         Provide an asynchronous context manager for database sessions.
         This ensures that the session is properly closed after use.
         """
         async with self.AsyncSession() as session:
             return session.begin
 
-    async def get_user(self, identifier: str) -> Optional["PersistedUser"]:
+    async def get_user(self, identifier: str, no_create=False) -> Optional["PersistedUser"]:
         """
         Retrieve a user by their identifier.
 
         :param identifier: The unique identifier of the user.
         :return: An instance of PersistedUser if found, otherwise None.
         """
         async with self.AsyncSession() as session:
@@ -64,17 +64,22 @@
                 return PersistedUser(
                     id=user_model.id,
                     identifier=user_model.identifier,
                     createdAt=str(user_model.createdAt),
                     metadata=user_model.metadata_ or {}
                 )
 
-        return await self.create_user(
-            user=User(identifier=identifier)
-        )
+        if not no_create:
+            await self.create_user(
+                user=User(identifier=identifier)
+            )
+
+            return self.get_user(identifier, no_create=True)
+        else:
+            return None
 
     async def create_user(self, user: "User") -> Optional["PersistedUser"]:
         """
         Create a new user or update an existing user's metadata.
 
         :param user: An instance of User containing the user's details.
         :return: An instance of PersistedUser with the created or updated user's details.
@@ -243,22 +248,14 @@
         """
         Create a new step and persist it to the database.
 
         :param step_dict: A dictionary containing the step's details.
         :return: A dictionary with the created step's details.
         """
         async with self.AsyncSession() as session:
-            # Convert string timestamps to datetime objects
-            created_at = datetime.fromisoformat(step_dict.get("createdAt").replace("Z", "+00:00")) if step_dict.get(
-                "createdAt") else None
-            start_time = datetime.fromisoformat(step_dict.get("start").replace("Z", "+00:00")) if step_dict.get(
-                "start") else None
-            end_time = datetime.fromisoformat(step_dict.get("end").replace("Z", "+00:00")) if step_dict.get(
-                "end") else None
-
             new_step = StepModel(
                 id=step_dict["id"],
                 thread_id=step_dict["threadId"],
                 parent_id=step_dict.get("parentId"),
                 name=step_dict["name"],
                 type=step_dict["type"],
                 input=step_dict.get("input"),
@@ -538,15 +535,14 @@
             page_info = PageInfo(
                 hasNextPage=len(threads) == pagination.first,
                 startCursor=threads[0].id if threads else None,
                 endCursor=threads[-1].id if threads else None
             ).to_dict()
 
             response = PaginatedResponse(data=threads_data, pageInfo=page_info)
-            print(response)
             return response
 
     async def update_thread(self, thread_id: str, name: Optional[str] = None, user_id: Optional[str] = None,
                             metadata: Optional[Dict] = None, tags: Optional[List[str]] = None):
         """
         Update a thread's details in the database.
```

### Comparing `lit_data_layers-0.1.2/lit_data_layers/sqldb/models.py` & `lit_data_layers-0.1.3/lit_data_layers/sqldb/models.py`

 * *Files identical despite different names*

### Comparing `lit_data_layers-0.1.2/pyproject.toml` & `lit_data_layers-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lit-data-layers"
-version = "0.1.2"
+version = "0.1.3"
 description = "A collection of data layers for Chainlit, persist state on your own infrastructure!"
 authors = ["Aniruddha Adhikary"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 chainlit = "^1.0.401"
```

### Comparing `lit_data_layers-0.1.2/PKG-INFO` & `lit_data_layers-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit-data-layers
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of data layers for Chainlit, persist state on your own infrastructure!
 Author: Aniruddha Adhikary
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

