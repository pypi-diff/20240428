# Comparing `tmp/lit_data_layers-0.1.1.tar.gz` & `tmp/lit_data_layers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lit_data_layers-0.1.1.tar", max compression
+gzip compressed data, was "lit_data_layers-0.1.2.tar", max compression
```

## Comparing `lit_data_layers-0.1.1.tar` & `lit_data_layers-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-01 17:39:40.930046 lit_data_layers-0.1.1/LICENSE
--rw-r--r--   0        0        0     1712 2024-04-02 13:00:23.234734 lit_data_layers-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-01 17:39:40.968049 lit_data_layers-0.1.1/lit_data_layers/__init__.py
--rw-r--r--   0        0        0    24361 2024-04-28 04:49:33.984893 lit_data_layers-0.1.1/lit_data_layers/sqldb/__init__.py
--rw-r--r--   0        0        0     3528 2024-04-28 04:49:33.985193 lit_data_layers-0.1.1/lit_data_layers/sqldb/models.py
--rw-r--r--   0        0        0      641 2024-04-28 04:50:06.235608 lit_data_layers-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 lit_data_layers-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 17:39:40.930046 lit_data_layers-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1712 2024-04-02 13:00:23.234734 lit_data_layers-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 17:39:40.968049 lit_data_layers-0.1.2/lit_data_layers/__init__.py
+-rw-r--r--   0        0        0    24525 2024-04-28 07:04:24.358082 lit_data_layers-0.1.2/lit_data_layers/sqldb/__init__.py
+-rw-r--r--   0        0        0     3618 2024-04-28 07:04:24.358401 lit_data_layers-0.1.2/lit_data_layers/sqldb/models.py
+-rw-r--r--   0        0        0      641 2024-04-28 07:04:24.358848 lit_data_layers-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 lit_data_layers-0.1.2/PKG-INFO
```

### Comparing `lit_data_layers-0.1.1/LICENSE` & `lit_data_layers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lit_data_layers-0.1.1/README.md` & `lit_data_layers-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lit_data_layers-0.1.1/lit_data_layers/sqldb/__init__.py` & `lit_data_layers-0.1.2/lit_data_layers/sqldb/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,22 +60,21 @@
 
             user_model = result.scalars().first()
 
             if user_model:
                 return PersistedUser(
                     id=user_model.id,
                     identifier=user_model.identifier,
-                    createdAt=user_model.createdAt,
-                    metadata=user_model.metadata_
+                    createdAt=str(user_model.createdAt),
+                    metadata=user_model.metadata_ or {}
                 )
 
-            else:
-                return self.create_user(
-                    user=User(identifier=identifier)
-                )
+        return await self.create_user(
+            user=User(identifier=identifier)
+        )
 
     async def create_user(self, user: "User") -> Optional["PersistedUser"]:
         """
         Create a new user or update an existing user's metadata.
 
         :param user: An instance of User containing the user's details.
         :return: An instance of PersistedUser with the created or updated user's details.
@@ -87,24 +86,24 @@
             user_model = result.scalars().first()
             if user_model:
                 user_model.metadata_ = user.metadata
             else:
                 user_model = PersistedUserModel(
                     id=str(uuid.uuid4()),
                     identifier=user.identifier,
-                    createdAt=str(datetime.now(timezone.utc)),
+                    createdAt=datetime.now(timezone.utc),
                     metadata=user.metadata
                 )
                 session.add(user_model)
             await session.commit()
 
             return PersistedUser(
                 id=user_model.id,
                 identifier=user_model.identifier,
-                createdAt=user_model.createdAt,
+                createdAt=str(user_model.createdAt),
                 metadata=user_model.metadata_
             )
 
     async def delete_user_session(self, id: str) -> bool:
         """
         Delete a user session by its ID.
 
@@ -123,24 +122,24 @@
         if feedback.id:
             async with self.AsyncSession() as session:
                 await session.execute(
                     update(FeedbackModel).
                     where(FeedbackModel.id == feedback.id).
                     values(
                         comment=feedback.comment,
-                        value=feedback.value
+                        value=str(feedback.value)
                     )
                 )
                 await session.commit()
             return feedback.id
         else:
             async with self.AsyncSession() as session:
                 new_feedback = FeedbackModel(
                     for_id=feedback.forId,
-                    value=feedback.value,
+                    value=str(feedback.value),
                     comment=feedback.comment,
                 )
                 session.add(new_feedback)
                 await session.commit()
                 return str(new_feedback.id)
 
     @queue_until_user_message()
@@ -261,32 +260,32 @@
                 thread_id=step_dict["threadId"],
                 parent_id=step_dict.get("parentId"),
                 name=step_dict["name"],
                 type=step_dict["type"],
                 input=step_dict.get("input"),
                 output=step_dict.get("output"),
                 metadata_=step_dict.get("metadata"),
-                created_at=datetime.utcnow(),
-                start_time=datetime.utcnow(),
+                created_at=datetime.now(timezone.utc),
+                start_time=datetime.now(timezone.utc),
                 end_time=None,
             )
             session.add(new_step)
             await session.commit()
 
             return {
                 "id": new_step.id,
                 "threadId": new_step.thread_id,
                 "name": new_step.name,
                 "type": new_step.type,
                 "input": new_step.input,
                 "output": new_step.output,
                 "metadata": new_step.metadata_,
-                "createdAt": new_step.created_at,
-                "start": new_step.start_time,
-                "end": new_step.end_time,
+                "createdAt": date_serialize(new_step.created_at),
+                "start": date_serialize(new_step.start_time),
+                "end": date_serialize(new_step.end_time),
             }
 
     @queue_until_user_message()
     async def update_step(self, step_dict: "StepDict") -> "StepDict":
         """
         Update an existing step's details in the database.
 
@@ -317,17 +316,17 @@
                     "id": step.id,
                     "threadId": step.thread_id,
                     "name": step.name,
                     "type": step.type,
                     "input": step.input,
                     "output": step.output,
                     "metadata": step.metadata_,
-                    "createdAt": step.created_at,
-                    "start": step.start_time,
-                    "end": step.end_time,
+                    "createdAt": date_serialize(step.created_at),
+                    "start": date_serialize(step.start_time),
+                    "end": date_serialize(step.end_time),
                 }
             else:
                 raise ValueError(f"Step with ID {step_dict['id']} not found")
 
     @queue_until_user_message()
     async def delete_step(self, step_id: str) -> bool:
         """
@@ -376,37 +375,37 @@
                 user_result = await session.execute(
                     select(PersistedUserModel).where(PersistedUserModel.id == thread_model.user_id)
                 )
                 user_model = user_result.scalars().first()
                 user_dict = {
                     "id": user_model.id,
                     "identifier": user_model.identifier,
-                    "createdAt": user_model.createdAt,
+                    "createdAt": user_model.createdAt.isoformat() if thread_model.createdAt else None,
                     "metadata": user_model.metadata_
                 } if user_model else None
 
                 return {
                     "id": thread_model.id,
                     "name": thread_model.name,
-                    "createdAt": thread_model.createdAt,
+                    "createdAt": date_serialize(thread_model.createdAt),
                     "metadata": thread_model.metadata_,
                     "tags": thread_model.tags,
                     "user": user_dict,
                     "steps": [{
                         "id": step.id,
                         "threadId": step.thread_id,
                         "parentId": step.parent_id,
                         "name": step.name,
                         "type": step.type,
                         "input": step.input,
                         "output": step.output,
                         "metadata": step.metadata_,
-                        "createdAt": step.created_at.isoformat() if step.created_at else None,
-                        "start": step.start_time.isoformat() if step.start_time else None,
-                        "end": step.end_time.isoformat() if step.end_time else None,
+                        "createdAt": date_serialize(step.created_at),
+                        "start": date_serialize(step.start_time),
+                        "end": date_serialize(step.end_time),
                     } for step in steps],
                     "elements": [{
                         "id": element.id,
                         "threadId": element.thread_id,
                         "type": element.type,
                         "chainlitKey": element.chainlit_key,
                         "url": element.url,
@@ -494,34 +493,34 @@
                     select(ElementModel).where(ElementModel.thread_id == thread.id)
                 )
                 elements = elements_result.scalars().all()
 
                 threads_data.append({
                     "id": thread.id,
                     "name": thread.name,
-                    "createdAt": thread.createdAt,
+                    "createdAt": date_serialize(thread.createdAt),
                     "metadata": thread.metadata_,
                     "tags": thread.tags,
                     "user": {
                         "id": thread.user.id,
                         "identifier": thread.user.identifier,
-                        "createdAt": thread.user.createdAt,
+                        "createdAt": date_serialize(thread.user.createdAt),
                         "metadata": thread.user.metadata_
                     },
                     "steps": [{
                         "id": step.id,
                         "threadId": step.thread_id,
                         "name": step.name,
                         "type": step.type,
                         "input": step.input,
                         "output": step.output,
                         "metadata": step.metadata_,
-                        "createdAt": step.created_at.isoformat() if step.created_at else None,
-                        "start": step.start_time.isoformat() if step.start_time else None,
-                        "end": step.end_time.isoformat() if step.end_time else None,
+                        "createdAt": date_serialize(step.created_at),
+                        "start": date_serialize(step.start_time),
+                        "end": date_serialize(step.end_time),
                     } for step in steps],
                     "elements": [{
                         "id": element.id,
                         "threadId": element.thread_id,
                         "type": element.type,
                         "chainlitKey": element.chainlit_key,
                         "url": element.url,
@@ -577,7 +576,14 @@
             if metadata is not None:
                 thread.metadata_ = metadata
             if tags is not None:
                 thread.tags = tags
 
             session.add(thread)
             await session.commit()
+
+
+def date_serialize(date: datetime) -> str:
+    if date is None:
+        return None
+
+    return date.isoformat()
```

### Comparing `lit_data_layers-0.1.1/lit_data_layers/sqldb/models.py` & `lit_data_layers-0.1.2/lit_data_layers/sqldb/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 class PersistedUserModel(Base):
     __tablename__ = 'users'
 
     id = Column(String, primary_key=True)
     identifier = Column(String, nullable=False)
-    createdAt = Column(String, nullable=False)
+    createdAt = Column(DateTime(timezone=True), nullable=False)
     metadata_ = Column(JSON)  # Using JSON field for metadata
 
     def __repr__(self):
         return f"<PersistedUser(id='{self.id}', identifier='{self.identifier}')>"
 
 
 class Feedback(Base):
@@ -68,15 +68,15 @@
 
 
 class ThreadModel(Base):
     __tablename__ = 'threads'
 
     id = Column(String, primary_key=True)
     name = Column(String, nullable=True)
-    createdAt = Column(String, nullable=False)
+    createdAt = Column(DateTime(timezone=True), nullable=False)
     metadata_ = Column(JSON)
     user_id = Column(String, ForeignKey('users.id'), nullable=True)
     tags = Column(JSON)
 
     # Relationships
     user = relationship("PersistedUserModel", backref="threads")
     elements = relationship("ElementModel", back_populates="thread", cascade="all, delete, delete-orphan")
@@ -96,16 +96,16 @@
     thread_id = Column(String, ForeignKey('threads.id'), nullable=False)
     parent_id = Column(String, nullable=True, default=None)
     name = Column(String, nullable=False)
     type = Column(String, nullable=False)
     input = Column(Text)
     output = Column(Text)
     metadata_ = Column(JSON)
-    created_at = Column(DateTime, default=datetime.datetime.utcnow)
-    start_time = Column(DateTime)
-    end_time = Column(DateTime)
+    created_at = Column(DateTime(timezone=True), default=lambda : datetime.now(timezone.utc))
+    start_time = Column(DateTime(timezone=True))
+    end_time = Column(DateTime(timezone=True))
 
     # Relationships
     thread = relationship("ThreadModel", back_populates="steps")
 
     def __repr__(self):
         return f"<StepModel(id='{self.id}', name='{self.name}', type='{self.type}')>"
```

### Comparing `lit_data_layers-0.1.1/pyproject.toml` & `lit_data_layers-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lit-data-layers"
-version = "0.1.1"
+version = "0.1.2"
 description = "A collection of data layers for Chainlit, persist state on your own infrastructure!"
 authors = ["Aniruddha Adhikary"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 chainlit = "^1.0.401"
```

### Comparing `lit_data_layers-0.1.1/PKG-INFO` & `lit_data_layers-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit-data-layers
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of data layers for Chainlit, persist state on your own infrastructure!
 Author: Aniruddha Adhikary
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

