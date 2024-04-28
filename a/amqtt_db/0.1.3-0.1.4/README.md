# Comparing `tmp/amqtt_db-0.1.3.tar.gz` & `tmp/amqtt_db-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqtt_db-0.1.3.tar", max compression
+gzip compressed data, was "amqtt_db-0.1.4.tar", max compression
```

## Comparing `amqtt_db-0.1.3.tar` & `amqtt_db-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1078 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/LICENSE
--rw-r--r--   0        0        0     2207 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/README.md
--rw-r--r--   0        0        0       22 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_db.py
--rw-r--r--   0        0        0      267 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_decoder.py
--rw-r--r--   0        0        0      410 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_deserializer.py
--rw-r--r--   0        0        0     1677 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_plugin.py
--rw-r--r--   0        0        0     1529 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_structure.py
--rw-r--r--   0        0        0     2967 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_topic.py
--rw-r--r--   0        0        0      417 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/constants.py
--rw-r--r--   0        0        0      971 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/delegator.py
--rw-r--r--   0        0        0      645 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/errors.py
--rw-r--r--   0        0        0      136 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/type_mapper.py
--rw-r--r--   0        0        0      696 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/utils.py
--rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/db/__init__.py
--rw-r--r--   0        0        0      387 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/db/base.py
--rw-r--r--   0        0        0     8081 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/db/db_sa.py
--rw-r--r--   0        0        0      633 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/default_config.yaml
--rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/payload/__init__.py
--rw-r--r--   0        0        0     1536 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/payload/flat_deserializer.py
--rw-r--r--   0        0        0      177 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/payload/json_decoder.py
--rw-r--r--   0        0        0     3429 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/plugin.py
--rw-r--r--   0        0        0      697 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/startup.py
--rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/structure/__init__.py
--rw-r--r--   0        0        0     1187 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/structure/structure.py
--rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/__init__.py
--rw-r--r--   0        0        0     3306 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/resources/mockups.py
--rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_db/__init__.py
--rw-r--r--   0        0        0     2471 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_db/test_sa.py
--rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_plugin/__init__.py
--rw-r--r--   0        0        0      952 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_plugin/test_functional.py
--rw-r--r--   0        0        0     1434 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_plugin/test_plugin.py
--rw-r--r--   0        0        0      911 2024-04-28 10:46:36.937427 amqtt_db-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 amqtt_db-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2207 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/base_db.py
+-rw-r--r--   0        0        0      267 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/base_decoder.py
+-rw-r--r--   0        0        0      410 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/base_deserializer.py
+-rw-r--r--   0        0        0     1677 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/base_plugin.py
+-rw-r--r--   0        0        0     1529 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/base_structure.py
+-rw-r--r--   0        0        0     2967 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/base_topic.py
+-rw-r--r--   0        0        0      417 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/constants.py
+-rw-r--r--   0        0        0      971 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/delegator.py
+-rw-r--r--   0        0        0      645 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/errors.py
+-rw-r--r--   0        0        0      136 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/type_mapper.py
+-rw-r--r--   0        0        0      696 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/base/utils.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/db/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/db/base.py
+-rw-r--r--   0        0        0     8081 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/db/db_sa.py
+-rw-r--r--   0        0        0      633 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/default_config.yaml
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/payload/__init__.py
+-rw-r--r--   0        0        0     1536 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/payload/flat_deserializer.py
+-rw-r--r--   0        0        0      177 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/payload/json_decoder.py
+-rw-r--r--   0        0        0     3429 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/plugin.py
+-rw-r--r--   0        0        0      697 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/startup.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/structure/__init__.py
+-rw-r--r--   0        0        0     1187 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/structure/structure.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/tests/__init__.py
+-rw-r--r--   0        0        0     3306 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/tests/resources/mockups.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/tests/test_db/__init__.py
+-rw-r--r--   0        0        0     2471 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/tests/test_db/test_sa.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/tests/test_plugin/__init__.py
+-rw-r--r--   0        0        0      952 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/tests/test_plugin/test_functional.py
+-rw-r--r--   0        0        0     1434 2024-04-28 10:38:28.798809 amqtt_db-0.1.4/amqtt_db/tests/test_plugin/test_plugin.py
+-rw-r--r--   0        0        0      912 2024-04-28 11:06:02.376235 amqtt_db-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 amqtt_db-0.1.4/PKG-INFO
```

### Comparing `amqtt_db-0.1.3/LICENSE` & `amqtt_db-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/README.md` & `amqtt_db-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/base/base_db.py` & `amqtt_db-0.1.4/amqtt_db/base/base_db.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/base/base_plugin.py` & `amqtt_db-0.1.4/amqtt_db/base/base_plugin.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/base/base_structure.py` & `amqtt_db-0.1.4/amqtt_db/base/base_structure.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/base/base_topic.py` & `amqtt_db-0.1.4/amqtt_db/base/base_topic.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/base/delegator.py` & `amqtt_db-0.1.4/amqtt_db/base/delegator.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/base/errors.py` & `amqtt_db-0.1.4/amqtt_db/base/errors.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/base/utils.py` & `amqtt_db-0.1.4/amqtt_db/base/utils.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/db/db_sa.py` & `amqtt_db-0.1.4/amqtt_db/db/db_sa.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/default_config.yaml` & `amqtt_db-0.1.4/amqtt_db/default_config.yaml`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/payload/flat_deserializer.py` & `amqtt_db-0.1.4/amqtt_db/payload/flat_deserializer.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/plugin.py` & `amqtt_db-0.1.4/amqtt_db/plugin.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/startup.py` & `amqtt_db-0.1.4/amqtt_db/startup.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/structure/structure.py` & `amqtt_db-0.1.4/amqtt_db/structure/structure.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/tests/resources/mockups.py` & `amqtt_db-0.1.4/amqtt_db/tests/resources/mockups.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/tests/test_db/test_sa.py` & `amqtt_db-0.1.4/amqtt_db/tests/test_db/test_sa.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/tests/test_plugin/test_functional.py` & `amqtt_db-0.1.4/amqtt_db/tests/test_plugin/test_functional.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/amqtt_db/tests/test_plugin/test_plugin.py` & `amqtt_db-0.1.4/amqtt_db/tests/test_plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.3/pyproject.toml` & `amqtt_db-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amqtt_db"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["volker <volker.jaenisch@inqbus.de>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/volkerjaenisch/amqtt_db"
 repository = "https://github.com/volkerjaenisch/amqtt_db"
@@ -17,15 +17,15 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 #amqtt = "^0.10.0-alpha.3"
 SQLAlchemy = "^1.4.1"
 aiounittest = "^1.4.0"
 psycopg2-binary = "^2.9.9"
 PyYAML = "^6.0.0"
-sqlalchemy-migrate = "^0.13.0"
+#sqlalchemy-migrate = "^0.13.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.3"
 Sphinx = "^3.5.3"
 sphinx-rtd-theme = "^0.5.2"
 coverage = "^5.5"
```

### Comparing `amqtt_db-0.1.3/PKG-INFO` & `amqtt_db-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqtt_db
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/volkerjaenisch/amqtt_db
 License: MIT
 Keywords: amqtt,MQTT,Persistence,SQLAlchemy,Database
 Author: volker
 Author-email: volker.jaenisch@inqbus.de
 Requires-Python: >=3.7,<4.0
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.1,<2.0.0)
 Requires-Dist: aiounittest (>=1.4.0,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
-Requires-Dist: sqlalchemy-migrate (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/volkerjaenisch/amqtt_db
 Description-Content-Type: text/markdown
 
 amqtt_db
 ========
 
 ![license](https://img.shields.io/github/license/volkerjaenisch/amqtt_db?style=flat-square)
```

