# Comparing `tmp/localdatamanager-0.1.0.tar.gz` & `tmp/localdatamanager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localdatamanager-0.1.0.tar", last modified: Mon Apr 22 02:28:49 2024, max compression
+gzip compressed data, was "localdatamanager-0.1.1.tar", last modified: Sun Apr 28 16:07:49 2024, max compression
```

## Comparing `localdatamanager-0.1.0.tar` & `localdatamanager-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.555317 localdatamanager-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.555317 localdatamanager-0.1.0/src/LocalDataManager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/src/LocalDataManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/src/LocalDataManager/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/src/LocalDataManager/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/src/LocalDataManager/db/db_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/src/LocalDataManager/file_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/src/LocalDataManager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/test/test_file_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:07:49.758658 localdatamanager-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-28 16:07:46.000000 localdatamanager-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-28 16:07:49.758658 localdatamanager-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-28 16:07:46.000000 localdatamanager-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-28 16:07:46.000000 localdatamanager-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:07:49.758658 localdatamanager-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:07:49.754658 localdatamanager-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:07:49.754658 localdatamanager-0.1.1/src/LocalDataManager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 16:07:46.000000 localdatamanager-0.1.1/src/LocalDataManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:07:49.754658 localdatamanager-0.1.1/src/LocalDataManager/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 16:07:46.000000 localdatamanager-0.1.1/src/LocalDataManager/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-28 16:07:46.000000 localdatamanager-0.1.1/src/LocalDataManager/db/db_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-28 16:07:46.000000 localdatamanager-0.1.1/src/LocalDataManager/file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:07:49.758658 localdatamanager-0.1.1/src/LocalDataManager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-28 16:07:49.000000 localdatamanager-0.1.1/src/LocalDataManager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-28 16:07:49.000000 localdatamanager-0.1.1/src/LocalDataManager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:07:49.000000 localdatamanager-0.1.1/src/LocalDataManager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 16:07:49.000000 localdatamanager-0.1.1/src/LocalDataManager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 16:07:49.000000 localdatamanager-0.1.1/src/LocalDataManager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:07:49.754658 localdatamanager-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-28 16:07:46.000000 localdatamanager-0.1.1/test/test_file_management.py
```

### Comparing `localdatamanager-0.1.0/LICENSE` & `localdatamanager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `localdatamanager-0.1.0/PKG-INFO` & `localdatamanager-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LocalDataManager
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for facilitating local file management
 Author-email: Blaine Perry <blainecperry@gmail.com>
 Project-URL: Homepage, https://github.com/bcperry/LocalDataManager
 Project-URL: Issues, https://github.com/bcperry/LocalDataManager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,21 +30,25 @@
 
 Install using pip
 ```sh
 # Using PyPI
 pip install LocalDataManager
 ```
 
-
 ## Dependencies
 
-``LocalDataManager`` only has one dependancy:
+``LocalDataManager`` only has two dependancies:
 
 [Pandas - Adds support for managing DataFrames as Files](https://pandas.pydata.org)
 
+[SQLAlchemy - Simplifies data management](https://www.sqlalchemy.org/)
+
+
+## Usage
+Examples can be found in the [examples](https://github.com/bcperry/LocalDataManager/tree/master/examples) directory.
 
 ## License
 [MIT](LICENSE)
 
 
 ## Background
 Work on ``LocalDataManager`` started in 2024 and
```

### Comparing `localdatamanager-0.1.0/README.md` & `localdatamanager-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,21 +14,25 @@
 
 Install using pip
 ```sh
 # Using PyPI
 pip install LocalDataManager
 ```
 
-
 ## Dependencies
 
-``LocalDataManager`` only has one dependancy:
+``LocalDataManager`` only has two dependancies:
 
 [Pandas - Adds support for managing DataFrames as Files](https://pandas.pydata.org)
 
+[SQLAlchemy - Simplifies data management](https://www.sqlalchemy.org/)
+
+
+## Usage
+Examples can be found in the [examples](https://github.com/bcperry/LocalDataManager/tree/master/examples) directory.
 
 ## License
 [MIT](LICENSE)
 
 
 ## Background
 Work on ``LocalDataManager`` started in 2024 and
```

### Comparing `localdatamanager-0.1.0/pyproject.toml` & `localdatamanager-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LocalDataManager"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Blaine Perry", email="blainecperry@gmail.com" },
 ]
 description = "A package for facilitating local file management"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `localdatamanager-0.1.0/src/LocalDataManager/db/db_classes.py` & `localdatamanager-0.1.1/src/LocalDataManager/db/db_classes.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,21 +11,24 @@
     pass
 
 class File(Base):
     __tablename__ = "files"
     hash: Mapped[str] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column(String(64))
     location: Mapped[Optional[str]]
-    # metadata: Mapped[List["Metadata"]] = relationship(
-    #     back_populates="file", cascade="all, delete-orphan"
-    # )
+    file_metadata: Mapped[List["Metadata"]] = relationship(back_populates="file")
+
     def __repr__(self) -> str:
-        return f"File(hash={self.hash!r}, name={self.name!r}, fullname={self.fullname!r})"
+        return f"File(hash={self.hash!r}, name={self.name!r}, location={self.location!r}, metadata={self.file_metadata!r})"
+    
+
+class Metadata(Base):
+    __tablename__ = "file_metadata"
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
+    hash: Mapped[str] = mapped_column(ForeignKey("files.hash"))
+    file: Mapped["File"] = relationship(back_populates="file_metadata")
+    metadata_key: Mapped[Optional[str]] 
+    metadata_value: Mapped[Optional[str]]
 
-# class Metadata(Base):
-#     __tablename__ = "metadata"
-#     id: Mapped[int] = mapped_column(primary_key=True)
-#     email_address: Mapped[str]
-#     user_id: Mapped[int] = mapped_column(ForeignKey("user_account.id"))
-#     file: Mapped["File"] = relationship(back_populates="metadata")
-#     def __repr__(self) -> str:
-#         return f"Metadata(id={self.id!r}, email_address={self.email_address!r})"
+
+    def __repr__(self) -> str:
+        return f"Metadata(hash={self.hash!r}, key={self.metadata_key!r}, value={self.metadata_value!r})"
```

### Comparing `localdatamanager-0.1.0/src/LocalDataManager/file_manager.py` & `localdatamanager-0.1.1/src/LocalDataManager/file_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 '''A local data management module'''
 
 import os
 import re
-import sqlite3
 import hashlib
 import logging
 import pandas as pd
 from io import BytesIO
 from sqlite3 import Error
 
 # ORM for databasing 
-from .db.db_classes import Base, File
+from .db.db_classes import Base, File, Metadata
 from sqlalchemy import create_engine, select
 from sqlalchemy.pool import NullPool
 from sqlalchemy.orm import Session
 
 
-from typing import Union, Literal
+from typing import List, Union, Literal
 
 
 class FileManager: 
     """
     A class to represent a the File Manager.
     ...
 
@@ -94,24 +93,25 @@
                 try:
                     os.makedirs(os.path.join(self.base_path,level))
                 except:
                     logging.error(f'Failed to create {os.path.join(self.base_path,level)}')
                     return False
         return True
 
-    def insert_file_into_files(self, name: str, hash: str, location: os.PathLike):
+    def insert_file_into_files(self, name: str, hash: str, file_metadata: List[Metadata], location: os.PathLike):
         """
         Create a new file into the files table
         :param file:
         :return: file id
         """
         with Session(self.engine) as session:
             file = File(name=name,
                         hash=hash,
-                        location=location
+                        location=location,
+                        file_metadata=file_metadata
                         )
             session.add(file)
             session.commit()
         return f"{name} Managed"
 
     def hash_file(self, file: BytesIO):
         """
@@ -217,58 +217,66 @@
         namelist = self.get_names()
 
         if filename in namelist:
             return True
         else:
             return False
 
-    def get_managed_files_df(self):
+    def get_managed_files_df(self, include_metadata: bool = True):
         """
         Provides functionality to get data on managed files.
 
         Parameters:
             None
 
         Returns:
             dataframe of all managed file information 
 
         """
-        df = pd.read_sql_table('files', self.engine)
-        # # df = pd.read_sql_table('table_name', 'postgres:///db_name')  
-        # with Session(self.engine) as session:
-        #     stmt = select(File)
-        #     files = list(session.scalars(stmt))
-        # # Convert ORM query result to a DataFrame
-        # df = pd.DataFrame([item.to_dict() for item in files])
-        # # df = pd.DataFrame(files, columns=['filename', 'hash', 'location'])
+        files_df = pd.read_sql_table('files', self.engine)
+        if include_metadata:
+            meta_df = pd.read_sql_table('file_metadata', self.engine)
+            files_df = pd.merge(files_df, meta_df, left_on='hash', right_on='hash')
+            files_df.drop('id', axis=1, inplace=True)
+        return files_df
 
-        return df
-
-    def save_file(self, file: BytesIO, data_level: str):
+    def save_file(self, file: BytesIO, data_level: str, metadata: dict):
         """
         Provides functionality to save documents per the data management
         system.
 
         Parameters:
             file:
             data_level:
+            metadata:
 
         Returns:
             true or error
         """
 
+
         if data_level not in self.data_levels:
             logging.error(f'{data_level} not in {self.data_levels}')
             return False
 
         filename = file.name.split('/')[-1]
         # check the management system for the file
         hash = self.hash_file(file)
         hash_managed = self.check_hashes(hash)
 
+        # create the metadata to add to the file
+        metadata_list = []
+        if metadata is not None:
+            for metadata_key, metadata_value in metadata.items():
+                metadata_list.append(
+                    Metadata(hash=hash, 
+                            metadata_key=metadata_key, 
+                            metadata_value=metadata_value)
+                    )
+
         # check if a file with this name already exists, if the hash is different
         file_managed = self.check_names(filename)
 
         if hash_managed:
             logging.info(f"{filename} already managed.")
             return f"{filename} already managed."
         
@@ -291,15 +299,15 @@
                 while True:
                     data = file.read(self.BUF_SIZE)
                     if not data:
                         break
                     f.write(data)
 
             # with the file saved, add it to the database
-            self.insert_file_into_files(name=filename, hash=hash, location=path)
+            self.insert_file_into_files(name=filename, hash=hash, location=path, file_metadata=metadata_list)
             return f"{filename} managed"
         except Exception as err:
             logging.error(err)
             return err
 
     def save_dataframe(self, dataframe: pd.DataFrame, name: str, data_level: str):
         """
```

### Comparing `localdatamanager-0.1.0/src/LocalDataManager.egg-info/PKG-INFO` & `localdatamanager-0.1.1/src/LocalDataManager.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LocalDataManager
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for facilitating local file management
 Author-email: Blaine Perry <blainecperry@gmail.com>
 Project-URL: Homepage, https://github.com/bcperry/LocalDataManager
 Project-URL: Issues, https://github.com/bcperry/LocalDataManager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,21 +30,25 @@
 
 Install using pip
 ```sh
 # Using PyPI
 pip install LocalDataManager
 ```
 
-
 ## Dependencies
 
-``LocalDataManager`` only has one dependancy:
+``LocalDataManager`` only has two dependancies:
 
 [Pandas - Adds support for managing DataFrames as Files](https://pandas.pydata.org)
 
+[SQLAlchemy - Simplifies data management](https://www.sqlalchemy.org/)
+
+
+## Usage
+Examples can be found in the [examples](https://github.com/bcperry/LocalDataManager/tree/master/examples) directory.
 
 ## License
 [MIT](LICENSE)
 
 
 ## Background
 Work on ``LocalDataManager`` started in 2024 and
```

### Comparing `localdatamanager-0.1.0/test/test_file_management.py` & `localdatamanager-0.1.1/test/test_file_management.py`

 * *Files identical despite different names*

