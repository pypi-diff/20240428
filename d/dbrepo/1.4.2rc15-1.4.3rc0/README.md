# Comparing `tmp/dbrepo-1.4.2rc15.tar.gz` & `tmp/dbrepo-1.4.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbrepo-1.4.2rc15.tar", last modified: Wed Apr 24 09:25:02 2024, max compression
+gzip compressed data, was "dbrepo-1.4.3rc0.tar", last modified: Sun Apr 28 16:09:12 2024, max compression
```

## Comparing `dbrepo-1.4.2rc15.tar` & `dbrepo-1.4.3rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/LICENSE
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/README.md
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.771814 dbrepo-1.4.2rc15/dbrepo/
--rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/dbrepo/AmqpClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/dbrepo/RestClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/dbrepo/UploadClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/dbrepo/__init__.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.771814 dbrepo-1.4.2rc15/dbrepo/api/
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/dbrepo/api/__init__.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    21346 2024-04-24 09:24:36.000000 dbrepo-1.4.2rc15/dbrepo/api/dto.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.2rc15/dbrepo/api/encoder.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/dbrepo/api/exceptions.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/dbrepo.egg-info/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/SOURCES.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/dependency_links.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/requires.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-24 09:25:02.000000 dbrepo-1.4.2rc15/dbrepo.egg-info/top_level.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1103 2024-04-24 09:24:57.000000 dbrepo-1.4.2rc15/pyproject.toml
--rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/setup.cfg
--rw-r--r--   0 mweise    (1000) mweise    (1000)      411 2024-04-24 09:24:57.000000 dbrepo-1.4.2rc15/setup.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-24 09:25:02.775814 dbrepo-1.4.2rc15/tests/
--rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_analyse.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_container.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_database.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_identifier.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_license.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_query.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.2rc15/tests/test_rest_client.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_table.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_user.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.2rc15/tests/test_view.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/LICENSE
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/README.md
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/dbrepo/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/dbrepo/AmqpClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/dbrepo/RestClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/dbrepo/UploadClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/dbrepo/__init__.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/dbrepo/api/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/dbrepo/api/__init__.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    21706 2024-04-28 16:07:17.000000 dbrepo-1.4.3rc0/dbrepo/api/dto.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.3rc0/dbrepo/api/encoder.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/dbrepo/api/exceptions.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/dbrepo.egg-info/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/requires.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-28 16:09:12.000000 dbrepo-1.4.3rc0/dbrepo.egg-info/top_level.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1102 2024-04-28 16:09:09.000000 dbrepo-1.4.3rc0/pyproject.toml
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/setup.cfg
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      410 2024-04-28 16:09:09.000000 dbrepo-1.4.3rc0/setup.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-28 16:09:12.864843 dbrepo-1.4.3rc0/tests/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_analyse.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_container.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_database.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_identifier.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_license.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_query.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc0/tests/test_rest_client.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_table.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_user.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc0/tests/test_view.py
```

### Comparing `dbrepo-1.4.2rc15/LICENSE` & `dbrepo-1.4.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/PKG-INFO` & `dbrepo-1.4.3rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.2rc15
+Version: 1.4.3rc0
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.2rc15/README.md` & `dbrepo-1.4.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/dbrepo/AmqpClient.py` & `dbrepo-1.4.3rc0/dbrepo/AmqpClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/dbrepo/RestClient.py` & `dbrepo-1.4.3rc0/dbrepo/RestClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/dbrepo/UploadClient.py` & `dbrepo-1.4.3rc0/dbrepo/UploadClient.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/dbrepo/api/dto.py` & `dbrepo-1.4.3rc0/dbrepo/api/dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,27 +580,29 @@
     result_number: Optional[int] = None
     publication_day: Optional[int] = None
     publication_month: Optional[int] = None
 
 
 class Identifier(BaseModel):
     id: int
+    database_id: int
     type: IdentifierType
-    creators: List[IdentifierCreator]
+    creator: UserBrief
+    status: IdentifierStatusType
     created: Timestamp
-    publication_year: int
     last_modified: Timestamp
+    publication_year: Optional[int] = None
+    creators: Optional[List[IdentifierCreator]] = field(default_factory=list)
     titles: Optional[List[IdentifierTitle]] = field(default_factory=list)
     descriptions: Optional[List[IdentifierDescription]] = field(default_factory=list)
     funders: Optional[List[IdentifierFunder]] = field(default_factory=list)
     doi: Optional[str] = None
     publisher: Optional[str] = None
     language: Optional[str] = None
     licenses: Optional[List[License]] = field(default_factory=list)
-    database_id: Optional[int] = None
     query_id: Optional[int] = None
     table_id: Optional[int] = None
     view_id: Optional[int] = None
     query: Optional[str] = None
     query_normalized: Optional[str] = None
     execution: Optional[str] = None
     related_identifiers: Optional[List[RelatedIdentifier]] = field(default_factory=list)
@@ -817,14 +819,25 @@
     DATABASE = "database"
     """The identifier is identifying a database."""
 
     TABLE = "table"
     """The identifier is identifying a table."""
 
 
+class IdentifierStatusType(str, Enum):
+    """
+    Enumeration of identifier status types.
+    """
+    PUBLISHED = "published"
+    """The identifier is published and immutable."""
+
+    DRAFT = "draft"
+    """The identifier is a draft and can still be edited."""
+
+
 class IdentifierType(str, Enum):
     """
     Enumeration of identifier types.
     """
     TABLE = "table"
     """The identifier identifies a table."""
```

### Comparing `dbrepo-1.4.2rc15/dbrepo/api/exceptions.py` & `dbrepo-1.4.3rc0/dbrepo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/dbrepo.egg-info/PKG-INFO` & `dbrepo-1.4.3rc0/dbrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.2rc15
+Version: 1.4.3rc0
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `dbrepo-1.4.2rc15/dbrepo.egg-info/SOURCES.txt` & `dbrepo-1.4.3rc0/dbrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/pyproject.toml` & `dbrepo-1.4.3rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbrepo"
-version = "1.4.2rc15"
+version = "1.4.3rc0"
 description = "DBRepo Python Library"
 keywords = [
     "DBRepo",
     "Database Repository"
 ]
 authors = [
     { name = "Martin Weise, TU Wien", email = "martin.weise@tuwien.ac.at" }
```

### Comparing `dbrepo-1.4.2rc15/tests/test_analyse.py` & `dbrepo-1.4.3rc0/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_container.py` & `dbrepo-1.4.3rc0/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_database.py` & `dbrepo-1.4.3rc0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_identifier.py` & `dbrepo-1.4.3rc0/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_license.py` & `dbrepo-1.4.3rc0/tests/test_license.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_query.py` & `dbrepo-1.4.3rc0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_rest_client.py` & `dbrepo-1.4.3rc0/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_table.py` & `dbrepo-1.4.3rc0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_user.py` & `dbrepo-1.4.3rc0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc15/tests/test_view.py` & `dbrepo-1.4.3rc0/tests/test_view.py`

 * *Files identical despite different names*

