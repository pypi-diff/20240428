# Comparing `tmp/espy_contact-0.3.tar.gz` & `tmp/espy_contact-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-0.3.tar", last modified: Sat Apr 27 15:24:04 2024, max compression
+gzip compressed data, was "espy_contact-0.4.tar", last modified: Sun Apr 28 03:42:05 2024, max compression
```

## Comparing `espy_contact-0.3.tar` & `espy_contact-0.4.tar`

### file list

```diff
@@ -1,32 +1,40 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.830377 espy_contact-0.3/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.3/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-27 15:24:04.830239 espy_contact-0.3/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-04-26 04:34:47.000000 espy_contact-0.3/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.827316 espy_contact-0.3/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.3/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.828256 espy_contact-0.3/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.3/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:19:13.000000 espy_contact-0.3/espy_contact/model/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1091 2024-04-26 04:22:51.000000 espy_contact-0.3/espy_contact/model/models.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.828636 espy_contact-0.3/espy_contact/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-0.3/espy_contact/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      120 2024-04-27 05:19:59.000000 espy_contact-0.3/espy_contact/schema/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2729 2024-04-27 03:04:08.000000 espy_contact-0.3/espy_contact/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.3/espy_contact/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.829406 espy_contact-0.3/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.3/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.3/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3777 2024-04-26 01:33:55.000000 espy_contact-0.3/espy_contact/util/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1387 2024-04-27 05:37:02.000000 espy_contact-0.3/espy_contact/util/pg.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.827901 espy_contact-0.3/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      610 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       63 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-04-27 15:24:04.000000 espy_contact-0.3/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-04-27 15:24:04.830424 espy_contact-0.3/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      631 2024-04-27 15:21:08.000000 espy_contact-0.3/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-27 15:24:04.830057 espy_contact-0.3/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.3/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.3/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.3/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 03:42:05.098526 espy_contact-0.4/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.4/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-28 03:42:05.098399 espy_contact-0.4/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-04-27 15:25:29.000000 espy_contact-0.4/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 03:42:05.091377 espy_contact-0.4/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.4/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 03:42:05.093686 espy_contact-0.4/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.4/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)    10969 2024-04-28 03:17:34.000000 espy_contact-0.4/espy_contact/model/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-0.4/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2616 2024-04-28 03:40:09.000000 espy_contact-0.4/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-0.4/espy_contact/model/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 03:42:05.095803 espy_contact-0.4/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-0.4/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2200 2024-04-28 03:20:57.000000 espy_contact-0.4/espy_contact/schema/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-0.4/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-0.4/espy_contact/schema/mgcampus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3204 2024-04-28 03:14:05.000000 espy_contact-0.4/espy_contact/schema/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-0.4/espy_contact/schema/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 03:42:05.096286 espy_contact-0.4/espy_contact/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-0.4/espy_contact/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.4/espy_contact/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 03:42:05.097525 espy_contact-0.4/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.4/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.4/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      184 2024-04-28 03:04:46.000000 espy_contact-0.4/espy_contact/util/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3777 2024-04-26 01:33:55.000000 espy_contact-0.4/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4356 2024-04-28 00:38:37.000000 espy_contact-0.4/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 03:42:05.092333 espy_contact-0.4/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-28 03:42:05.000000 espy_contact-0.4/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      830 2024-04-28 03:42:05.000000 espy_contact-0.4/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-04-28 03:42:05.000000 espy_contact-0.4/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       76 2024-04-28 03:42:05.000000 espy_contact-0.4/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-04-28 03:42:05.000000 espy_contact-0.4/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-04-28 03:42:05.098585 espy_contact-0.4/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      655 2024-04-28 03:41:53.000000 espy_contact-0.4/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 03:42:05.098240 espy_contact-0.4/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.4/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.4/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.4/tests/test_service.py
```

### Comparing `espy_contact-0.3/LICENSE` & `espy_contact-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-0.3/espy_contact/model/models.py` & `espy_contact-0.4/espy_contact/util/CONSTANTS.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,12 @@
 
 For permission requests, write to the publisher at the email address below:
 office@myeverlasting.net
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
-from pydantic import BaseModel, Field
-class SeoRequest(BaseModel):
-    url: str = Field(min_length=4, description="Your website url")
-class WebbuilderRequest(BaseModel):
-    id: str
-    content: str
-    product_id: int
+from dotenv import load_dotenv
+import os
 
+load_dotenv()
+SCHEMA = os.getenv("db_schema")
```

### Comparing `espy_contact-0.3/espy_contact/schema.py` & `espy_contact-0.4/espy_contact/model/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 For permission requests, write to the publisher at the email address below:
 office@myeverlasting.net
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 import uuid
+from sqlalchemy import Column, DateTime, ForeignKey, Enum
 from sqlalchemy.sql import func
 from sqlalchemy.sql.sqltypes import Integer,String,Boolean
 from sqlalchemy.dialects.postgresql import ARRAY
-from sqlalchemy import Column, DateTime, ForeignKey, Enum, MetaData
-from sqlalchemy.orm import relationship,declarative_base
+from sqlalchemy.orm import relationship
 from espy_contact.util.enums import AccessRoleEnum,StatusEnum
-from espy_contact.util.CONSTANTS import SCHEMA
-metadata = MetaData(schema=SCHEMA)
-Base = declarative_base(metadata=metadata)
+from espy_contact.util.db import Base
+
 class Webbuilder(Base):
     __tablename__ = "webbuilder"
     id = Column(String, primary_key=True, index=True)
     content = Column(String)
     product_id = Column(Integer)
     is_live = Column(Boolean, default=False)
     timestamp = Column(DateTime(), server_default=func.now())
```

### Comparing `espy_contact-0.3/espy_contact/service.py` & `espy_contact-0.4/espy_contact/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.3/espy_contact/util/enums.py` & `espy_contact-0.4/espy_contact/util/enums.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.3/setup.py` & `espy_contact-0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.2'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
-        'sqlalchemy==2.0.29'
+        'sqlalchemy==2.0.29',
+        'bson==0.5.10'
         ],
     author='Femi Adigun',
     author_email='femi.adigun@myeverlasting.net',
     description=DESCRIPTION,
     long_description_content_type='text/markdown',
     long_description=LONG_DESCRIPTION,
     keywords=['fastapi','ESSL','ReachAI']
```

### Comparing `espy_contact-0.3/tests/test_copyright.py` & `espy_contact-0.4/tests/test_copyright.py`

 * *Files identical despite different names*

