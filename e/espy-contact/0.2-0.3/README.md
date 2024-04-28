# Comparing `tmp/espy_contact-0.2.tar.gz` & `tmp/espy_contact-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-0.2.tar", last modified: Sat Apr 27 02:59:59 2024, max compression
+gzip compressed data, was "espy_contact-0.3.tar", last modified: Sat Apr 27 15:24:04 2024, max compression
```

## Comparing `espy_contact-0.2.tar` & `espy_contact-0.3.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.376239 espy_contact-0.2/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.2/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-27 02:59:59.376114 espy_contact-0.2/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-04-26 04:34:47.000000 espy_contact-0.2/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.373762 espy_contact-0.2/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.2/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.374722 espy_contact-0.2/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.2/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1091 2024-04-26 04:22:51.000000 espy_contact-0.2/espy_contact/model/models.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2723 2024-04-26 04:04:33.000000 espy_contact-0.2/espy_contact/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.2/espy_contact/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.375289 espy_contact-0.2/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.2/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.2/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3777 2024-04-26 01:33:55.000000 espy_contact-0.2/espy_contact/util/enums.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.374490 espy_contact-0.2/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      489 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       63 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-04-27 02:59:59.000000 espy_contact-0.2/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-04-27 02:59:59.376293 espy_contact-0.2/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      631 2024-04-27 02:59:43.000000 espy_contact-0.2/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 02:59:59.375943 espy_contact-0.2/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.2/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.2/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.2/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.830377 espy_contact-0.3/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.3/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-27 15:24:04.830239 espy_contact-0.3/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-04-26 04:34:47.000000 espy_contact-0.3/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.827316 espy_contact-0.3/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.3/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.828256 espy_contact-0.3/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.3/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:19:13.000000 espy_contact-0.3/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1091 2024-04-26 04:22:51.000000 espy_contact-0.3/espy_contact/model/models.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.828636 espy_contact-0.3/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-0.3/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      120 2024-04-27 05:19:59.000000 espy_contact-0.3/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2729 2024-04-27 03:04:08.000000 espy_contact-0.3/espy_contact/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.3/espy_contact/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.829406 espy_contact-0.3/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.3/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.3/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3777 2024-04-26 01:33:55.000000 espy_contact-0.3/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1387 2024-04-27 05:37:02.000000 espy_contact-0.3/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.827901 espy_contact-0.3/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      610 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       63 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-04-27 15:24:04.830424 espy_contact-0.3/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      631 2024-04-27 15:21:08.000000 espy_contact-0.3/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.830057 espy_contact-0.3/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.3/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.3/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.3/tests/test_service.py
```

### Comparing `espy_contact-0.2/LICENSE` & `espy_contact-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-0.2/espy_contact/model/models.py` & `espy_contact-0.3/espy_contact/model/models.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.2/espy_contact/schema.py` & `espy_contact-0.3/espy_contact/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 """
 import uuid
 from sqlalchemy.sql import func
 from sqlalchemy.sql.sqltypes import Integer,String,Boolean
 from sqlalchemy.dialects.postgresql import ARRAY
 from sqlalchemy import Column, DateTime, ForeignKey, Enum, MetaData
 from sqlalchemy.orm import relationship,declarative_base
-from escontact.util.enums import AccessRoleEnum,StatusEnum
-from escontact.util.CONSTANTS import SCHEMA
+from espy_contact.util.enums import AccessRoleEnum,StatusEnum
+from espy_contact.util.CONSTANTS import SCHEMA
 metadata = MetaData(schema=SCHEMA)
 Base = declarative_base(metadata=metadata)
 class Webbuilder(Base):
     __tablename__ = "webbuilder"
     id = Column(String, primary_key=True, index=True)
     content = Column(String)
     product_id = Column(Integer)
```

### Comparing `espy_contact-0.2/espy_contact/service.py` & `espy_contact-0.3/espy_contact/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.2/espy_contact/util/CONSTANTS.py` & `espy_contact-0.3/espy_contact/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.2/espy_contact/util/enums.py` & `espy_contact-0.3/espy_contact/util/enums.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.2/setup.py` & `espy_contact-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.2'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29'
         ],
```

### Comparing `espy_contact-0.2/tests/test_copyright.py` & `espy_contact-0.3/tests/test_copyright.py`

 * *Files identical despite different names*

