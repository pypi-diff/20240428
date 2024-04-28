# Comparing `tmp/lit_data_layers-0.1.0.tar.gz` & `tmp/lit_data_layers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lit_data_layers-0.1.0.tar", max compression
+gzip compressed data, was "lit_data_layers-0.1.1.tar", max compression
```

## Comparing `lit_data_layers-0.1.0.tar` & `lit_data_layers-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-01 17:39:40.930046 lit_data_layers-0.1.0/LICENSE
--rw-r--r--   0        0        0     1712 2024-04-02 13:00:23.234734 lit_data_layers-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-01 17:39:40.968049 lit_data_layers-0.1.0/lit_data_layers/__init__.py
--rw-r--r--   0        0        0    24210 2024-04-02 12:41:07.343291 lit_data_layers-0.1.0/lit_data_layers/sqldb/__init__.py
--rw-r--r--   0        0        0     3468 2024-04-02 12:32:20.612347 lit_data_layers-0.1.0/lit_data_layers/sqldb/models.py
--rw-r--r--   0        0        0      641 2024-04-01 18:37:39.043831 lit_data_layers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 lit_data_layers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 17:39:40.930046 lit_data_layers-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1712 2024-04-02 13:00:23.234734 lit_data_layers-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 17:39:40.968049 lit_data_layers-0.1.1/lit_data_layers/__init__.py
+-rw-r--r--   0        0        0    24361 2024-04-28 04:49:33.984893 lit_data_layers-0.1.1/lit_data_layers/sqldb/__init__.py
+-rw-r--r--   0        0        0     3528 2024-04-28 04:49:33.985193 lit_data_layers-0.1.1/lit_data_layers/sqldb/models.py
+-rw-r--r--   0        0        0      641 2024-04-28 04:50:06.235608 lit_data_layers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 lit_data_layers-0.1.1/PKG-INFO
```

### Comparing `lit_data_layers-0.1.0/LICENSE` & `lit_data_layers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lit_data_layers-0.1.0/README.md` & `lit_data_layers-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lit_data_layers-0.1.0/lit_data_layers/sqldb/__init__.py` & `lit_data_layers-0.1.1/lit_data_layers/sqldb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,18 @@
                 return PersistedUser(
                     id=user_model.id,
                     identifier=user_model.identifier,
                     createdAt=user_model.createdAt,
                     metadata=user_model.metadata_
                 )
 
-            return None
+            else:
+                return self.create_user(
+                    user=User(identifier=identifier)
+                )
 
     async def create_user(self, user: "User") -> Optional["PersistedUser"]:
         """
         Create a new user or update an existing user's metadata.
 
         :param user: An instance of User containing the user's details.
         :return: An instance of PersistedUser with the created or updated user's details.
@@ -120,27 +123,25 @@
         if feedback.id:
             async with self.AsyncSession() as session:
                 await session.execute(
                     update(FeedbackModel).
                     where(FeedbackModel.id == feedback.id).
                     values(
                         comment=feedback.comment,
-                        strategy=feedback.strategy,
                         value=feedback.value
                     )
                 )
                 await session.commit()
             return feedback.id
         else:
             async with self.AsyncSession() as session:
                 new_feedback = FeedbackModel(
                     for_id=feedback.forId,
                     value=feedback.value,
                     comment=feedback.comment,
-                    strategy=feedback.strategy,
                 )
                 session.add(new_feedback)
                 await session.commit()
                 return str(new_feedback.id)
 
     @queue_until_user_message()
     async def create_element(self, element_dict: "ElementDict") -> "ElementDict":
@@ -254,14 +255,15 @@
                 "start") else None
             end_time = datetime.fromisoformat(step_dict.get("end").replace("Z", "+00:00")) if step_dict.get(
                 "end") else None
 
             new_step = StepModel(
                 id=step_dict["id"],
                 thread_id=step_dict["threadId"],
+                parent_id=step_dict.get("parentId"),
                 name=step_dict["name"],
                 type=step_dict["type"],
                 input=step_dict.get("input"),
                 output=step_dict.get("output"),
                 metadata_=step_dict.get("metadata"),
                 created_at=datetime.utcnow(),
                 start_time=datetime.utcnow(),
@@ -388,14 +390,15 @@
                     "createdAt": thread_model.createdAt,
                     "metadata": thread_model.metadata_,
                     "tags": thread_model.tags,
                     "user": user_dict,
                     "steps": [{
                         "id": step.id,
                         "threadId": step.thread_id,
+                        "parentId": step.parent_id,
                         "name": step.name,
                         "type": step.type,
                         "input": step.input,
                         "output": step.output,
                         "metadata": step.metadata_,
                         "createdAt": step.created_at.isoformat() if step.created_at else None,
                         "start": step.start_time.isoformat() if step.start_time else None,
@@ -457,16 +460,16 @@
 
         :param pagination: An instance of Pagination containing pagination details.
         :param filters: An instance of ThreadFilter containing filter criteria.
         :return: A PaginatedResponse containing a list of threads and page information.
         """
         async with self.AsyncSession() as session:
             query = select(ThreadModel).options(selectinload(ThreadModel.user)).join(PersistedUserModel)
-            if filters.userIdentifier:
-                query = query.where(PersistedUserModel.identifier == filters.userIdentifier)
+            if filters.userId:
+                query = query.where(PersistedUserModel.id == filters.userId)
             if filters.search:
                 query = query.where(ThreadModel.name.ilike(f'%{filters.search}%'))
             if filters.feedback is not None:
                 # Assuming there is a FeedbackModel with a thread_id and value fields
                 query = query.join(FeedbackModel).where(FeedbackModel.value == filters.feedback)
 
             query = query.order_by(ThreadModel.createdAt.desc())
@@ -531,14 +534,15 @@
                         "forId": element.for_id,
                         "page": element.page,
                     } for element in elements],
                 })
 
             page_info = PageInfo(
                 hasNextPage=len(threads) == pagination.first,
+                startCursor=threads[0].id if threads else None,
                 endCursor=threads[-1].id if threads else None
             ).to_dict()
 
             response = PaginatedResponse(data=threads_data, pageInfo=page_info)
             print(response)
             return response
```

### Comparing `lit_data_layers-0.1.0/lit_data_layers/sqldb/models.py` & `lit_data_layers-0.1.1/lit_data_layers/sqldb/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
 
 class StepModel(Base):
     __tablename__ = 'steps'
 
     id = Column(String, primary_key=True)
     thread_id = Column(String, ForeignKey('threads.id'), nullable=False)
+    parent_id = Column(String, nullable=True, default=None)
     name = Column(String, nullable=False)
     type = Column(String, nullable=False)
     input = Column(Text)
     output = Column(Text)
     metadata_ = Column(JSON)
     created_at = Column(DateTime, default=datetime.datetime.utcnow)
     start_time = Column(DateTime)
```

### Comparing `lit_data_layers-0.1.0/pyproject.toml` & `lit_data_layers-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lit-data-layers"
-version = "0.1.0"
+version = "0.1.1"
 description = "A collection of data layers for Chainlit, persist state on your own infrastructure!"
 authors = ["Aniruddha Adhikary"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 chainlit = "^1.0.401"
```

### Comparing `lit_data_layers-0.1.0/PKG-INFO` & `lit_data_layers-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit-data-layers
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of data layers for Chainlit, persist state on your own infrastructure!
 Author: Aniruddha Adhikary
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

