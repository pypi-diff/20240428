# Comparing `tmp/amqtt_db-0.1.2.tar.gz` & `tmp/amqtt_db-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqtt_db-0.1.2.tar", max compression
+gzip compressed data, was "amqtt_db-0.1.3.tar", max compression
```

## Comparing `amqtt_db-0.1.2.tar` & `amqtt_db-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,35 @@
--rw-r--r--   0        0        0     1078 2021-03-16 23:38:22.045011 amqtt_db-0.1.2/LICENSE
--rw-r--r--   0        0        0     2054 2021-04-14 20:45:54.707827 amqtt_db-0.1.2/README.md
--rw-r--r--   0        0        0       22 2021-03-16 21:44:12.449637 amqtt_db-0.1.2/amqtt_db/__init__.py
--rw-r--r--   0        0        0        0 2021-03-16 19:57:55.628000 amqtt_db-0.1.2/amqtt_db/base/__init__.py
--rw-r--r--   0        0        0     1101 2021-04-10 20:56:02.401883 amqtt_db-0.1.2/amqtt_db/base/base_db.py
--rw-r--r--   0        0        0      267 2021-03-28 16:32:55.694314 amqtt_db-0.1.2/amqtt_db/base/base_decoder.py
--rw-r--r--   0        0        0      410 2021-04-05 22:24:31.077975 amqtt_db-0.1.2/amqtt_db/base/base_deserializer.py
--rw-r--r--   0        0        0     1636 2021-04-12 21:45:40.414801 amqtt_db-0.1.2/amqtt_db/base/base_plugin.py
--rw-r--r--   0        0        0     1529 2021-04-12 21:46:29.954194 amqtt_db-0.1.2/amqtt_db/base/base_structure.py
--rw-r--r--   0        0        0     2681 2021-04-13 17:09:32.215020 amqtt_db-0.1.2/amqtt_db/base/base_topic.py
--rw-r--r--   0        0        0      385 2021-04-12 21:47:46.413255 amqtt_db-0.1.2/amqtt_db/base/constants.py
--rw-r--r--   0        0        0      971 2021-04-05 22:26:27.816521 amqtt_db-0.1.2/amqtt_db/base/delegator.py
--rw-r--r--   0        0        0      284 2021-04-05 22:32:54.003736 amqtt_db-0.1.2/amqtt_db/base/errors.py
--rw-r--r--   0        0        0      136 2021-03-22 22:32:31.168001 amqtt_db-0.1.2/amqtt_db/base/type_mapper.py
--rw-r--r--   0        0        0      696 2021-04-10 21:11:16.570450 amqtt_db-0.1.2/amqtt_db/base/utils.py
--rw-r--r--   0        0        0        0 2021-03-19 22:05:14.303000 amqtt_db-0.1.2/amqtt_db/db/__init__.py
--rw-r--r--   0        0        0      387 2021-04-05 22:32:54.011736 amqtt_db-0.1.2/amqtt_db/db/base.py
--rw-r--r--   0        0        0     8081 2021-04-13 17:11:00.037831 amqtt_db-0.1.2/amqtt_db/db/db_sa.py
--rw-r--r--   0        0        0      611 2021-04-13 15:07:42.204489 amqtt_db-0.1.2/amqtt_db/default_config.yaml
--rw-r--r--   0        0        0        0 2021-03-28 19:28:30.699558 amqtt_db-0.1.2/amqtt_db/payload/__init__.py
--rw-r--r--   0        0        0     1417 2021-04-13 17:10:40.282097 amqtt_db-0.1.2/amqtt_db/payload/flat_deserializer.py
--rw-r--r--   0        0        0      177 2021-04-13 17:11:10.873685 amqtt_db-0.1.2/amqtt_db/payload/json_decoder.py
--rw-r--r--   0        0        0      788 2021-04-13 17:10:53.169923 amqtt_db-0.1.2/amqtt_db/payload/topic_engine.py
--rw-r--r--   0        0        0     3402 2021-04-13 15:27:20.346016 amqtt_db-0.1.2/amqtt_db/plugin.py
--rw-r--r--   0        0        0      697 2021-04-10 21:01:28.121807 amqtt_db-0.1.2/amqtt_db/startup.py
--rw-r--r--   0        0        0        0 2021-03-19 22:05:14.303801 amqtt_db-0.1.2/amqtt_db/structure/__init__.py
--rw-r--r--   0        0        0     1130 2021-04-12 21:47:46.421255 amqtt_db-0.1.2/amqtt_db/structure/structure.py
--rw-r--r--   0        0        0     8192 2021-04-05 21:18:48.655117 amqtt_db-0.1.2/amqtt_db/test_topic.sqlite
--rw-r--r--   0        0        0        0 2021-03-16 21:44:12.449637 amqtt_db-0.1.2/amqtt_db/tests/__init__.py
--rw-r--r--   0        0        0     1130 2021-04-13 17:10:01.622620 amqtt_db-0.1.2/amqtt_db/tests/resources/mockups.py
--rw-r--r--   0        0        0        0 2021-04-05 21:16:58.320695 amqtt_db-0.1.2/amqtt_db/tests/test_db/__init__.py
--rw-r--r--   0        0        0     2415 2021-04-13 17:09:39.402922 amqtt_db-0.1.2/amqtt_db/tests/test_db/test_sa.py
--rw-r--r--   0        0        0        0 2021-04-05 21:16:58.320000 amqtt_db-0.1.2/amqtt_db/tests/test_plugin/__init__.py
--rw-r--r--   0        0        0      459 2021-04-13 17:10:29.898237 amqtt_db-0.1.2/amqtt_db/tests/test_plugin/test_plugin.py
--rw-r--r--   0        0        0     8192 2021-04-10 23:17:22.617924 amqtt_db-0.1.2/amqtt_db/tests/test_topic.qlite
--rw-r--r--   0        0        0      902 2021-04-14 20:37:38.009840 amqtt_db-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3268 2021-04-14 20:47:23.268338 amqtt_db-0.1.2/setup.py
--rw-r--r--   0        0        0     3153 2021-04-14 20:47:23.268650 amqtt_db-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2207 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_db.py
+-rw-r--r--   0        0        0      267 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_decoder.py
+-rw-r--r--   0        0        0      410 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_deserializer.py
+-rw-r--r--   0        0        0     1677 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_plugin.py
+-rw-r--r--   0        0        0     1529 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_structure.py
+-rw-r--r--   0        0        0     2967 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/base_topic.py
+-rw-r--r--   0        0        0      417 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/constants.py
+-rw-r--r--   0        0        0      971 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/delegator.py
+-rw-r--r--   0        0        0      645 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/errors.py
+-rw-r--r--   0        0        0      136 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/type_mapper.py
+-rw-r--r--   0        0        0      696 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/base/utils.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/db/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/db/base.py
+-rw-r--r--   0        0        0     8081 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/db/db_sa.py
+-rw-r--r--   0        0        0      633 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/default_config.yaml
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/payload/__init__.py
+-rw-r--r--   0        0        0     1536 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/payload/flat_deserializer.py
+-rw-r--r--   0        0        0      177 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/payload/json_decoder.py
+-rw-r--r--   0        0        0     3429 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/plugin.py
+-rw-r--r--   0        0        0      697 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/startup.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/structure/__init__.py
+-rw-r--r--   0        0        0     1187 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/structure/structure.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/__init__.py
+-rw-r--r--   0        0        0     3306 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/resources/mockups.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_db/__init__.py
+-rw-r--r--   0        0        0     2471 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_db/test_sa.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_plugin/__init__.py
+-rw-r--r--   0        0        0      952 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_plugin/test_functional.py
+-rw-r--r--   0        0        0     1434 2024-04-28 10:38:28.798809 amqtt_db-0.1.3/amqtt_db/tests/test_plugin/test_plugin.py
+-rw-r--r--   0        0        0      911 2024-04-28 10:46:36.937427 amqtt_db-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 amqtt_db-0.1.3/PKG-INFO
```

### Comparing `amqtt_db-0.1.2/LICENSE` & `amqtt_db-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.2/README.md` & `amqtt_db-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 amqtt_db
 ========
 
 ![license](https://img.shields.io/github/license/volkerjaenisch/amqtt_db?style=flat-square)
-![travis](https://api.travis-ci.org/volkerjaenisch/amqtt_db.svg?branch=main)
-![coverals](https://coveralls.io/repos/github/volkerjaenisch/amqtt_db/badge.svg)
-[![PyPI](https://img.shields.io/pypi/v/amqtt_db?style=flat-square)](https://pypi.org/project/amqtt/)
+[![Build Status](https://travis-ci.org/volkerjaenisch/amqtt_db.svg?branch=main)](https://travis-ci.org/volkerjaenisch/amqtt_db)
+[![Coverage Status](https://coveralls.io/repos/github/volkerjaenisch/amqtt_db/badge.svg?branch=main)](https://coveralls.io/github/volkerjaenisch/amqtt_db?branch=main)
+[![PyPI](https://img.shields.io/pypi/v/amqtt_db)](https://pypi.org/project/amqtt_db/)
 [![Documantation](https://img.shields.io/readthedocs/amqtt-db.svg)](https://amqtt_db.readthedocs.io/en/latest/)
 
-DB persistence for amqtt.
+DB persistence for [amqtt](https://github.com/Yakifo/amqtt).
 
 Objective
 ---------
 
-amqtt_db will persist payloads received by the [amqtt broker](https://github.com/Yakifo/amqtt) into performant relational databases.
+amqtt_db persists payloads received by the [amqtt broker](https://github.com/Yakifo/amqtt) into performant relational databases.
 SQLAlchemy as well as timescaleBD are the target RMDB-Systems.
 
 amqtt_db will do four steps to persist the amqtt data:
 
  1) decoding the payload (e.G. from binary, JSON or which ever encoding)
  1) deserializing the payload to typed Python entities
  1) structure the session, topic, property, value information into a relational model of your choice
```

### Comparing `amqtt_db-0.1.2/amqtt_db/base/base_db.py` & `amqtt_db-0.1.3/amqtt_db/base/base_db.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.2/amqtt_db/base/base_plugin.py` & `amqtt_db-0.1.3/amqtt_db/base/base_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
             ]
     }
 
     config_path = BASE_CONFIG_PATH   # dotted name path e.g 'plugins.timescaledb'
     config = None
 
     def __init__(self, context):
+        super(BasePlugin, self).__init__()
         self.context = context
         self.init_config(context)
 
     def init_config(self, context):
         """
         Use the config_path to derive the config portion of this test_plugin and store it under self.config.
         :param context:
@@ -34,15 +35,15 @@
             temp_config = context.config
             path_parts = self.config_path.split('.')
             for path_part in path_parts[:-1]:
                 temp_config = temp_config[path_part]
             if path_parts[-1] in temp_config:
                 self.config = context.config[path_parts[-1]]
             else:
-                raise ImportError()
+                raise ImportError
 
         except KeyError as e:
             msg = 'amqtt_db: Plugin config not found under "{}" in the config file '.format(self.config_path)
             self.context.logger.error(msg)
             raise ImportError(e)
 
     def register_events(self):
```

### Comparing `amqtt_db-0.1.2/amqtt_db/base/base_structure.py` & `amqtt_db-0.1.3/amqtt_db/base/base_structure.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.2/amqtt_db/base/base_topic.py` & `amqtt_db-0.1.3/amqtt_db/base/base_topic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Base of a topic engine, routing the payload to the configured deserializer
 """
 import re
 
 from amqtt_db.base.constants import PAYLOAD_CONFIG
-from amqtt_db.base.errors import TopicNotFound
+from amqtt_db.base.errors import TopicNotFound, NoPayloadDefinition, WrongPayloadDefinition
 from amqtt_db.base.utils import get_class_func_by_name
 
 
 class BaseTopicEngine(object):
 
     def __init__(self, parent):
         self.parent = parent
@@ -19,37 +19,43 @@
         self.read_config(parent.config)
 
     def read_config(self, config):
         """
         Build a simple parse tree out of the payload config
         :param config: The payload config
         """
-        payload_config = config[PAYLOAD_CONFIG]
-        for key, value in payload_config.items():
-            entry = list(value.items())[0]
-            decoder_cls_name = entry[0]
-            decoder_class = get_class_func_by_name(decoder_cls_name)
-            if decoder_cls_name in self.decoders:
-                decoder = self.decoders[decoder_cls_name]
-            else:
-                decoder = decoder_class()
-                self.decoders[decoder_cls_name] = decoder
-
-            deserialier_config = entry[1]
-            deserializer_cls_name, types = list(deserialier_config.items())[0]
-            deserializer_class = get_class_func_by_name(deserializer_cls_name)
-
-            if deserializer_cls_name in self.deserializers:
-                deserializer = self.deserializers[deserializer_cls_name]
-            else:
-                deserializer = deserializer_class(types)
-                self.deserializers[deserializer_cls_name] = deserializer
-
-            self.topic_handlers[key] = [decoder, deserializer]
-            self.topic_re[re.compile(key)] = self.topic_handlers[key]
+        try:
+            payload_config = config[PAYLOAD_CONFIG]
+        except KeyError:
+            raise NoPayloadDefinition
+        try:
+            for key, value in payload_config.items():
+                entry = list(value.items())[0]
+                decoder_cls_name = entry[0]
+                decoder_class = get_class_func_by_name(decoder_cls_name)
+                if decoder_cls_name in self.decoders:
+                    decoder = self.decoders[decoder_cls_name]
+                else:
+                    decoder = decoder_class()
+                    self.decoders[decoder_cls_name] = decoder
+
+                deserialier_config = entry[1]
+                deserializer_cls_name, types = list(deserialier_config.items())[0]
+                deserializer_class = get_class_func_by_name(deserializer_cls_name)
+
+                if deserializer_cls_name in self.deserializers:
+                    deserializer = self.deserializers[deserializer_cls_name]
+                else:
+                    deserializer = deserializer_class(types)
+                    self.deserializers[deserializer_cls_name] = deserializer
+
+                self.topic_handlers[key] = [decoder, deserializer]
+                self.topic_re[re.compile(key)] = self.topic_handlers[key]
+        except (KeyError, AttributeError):
+            raise WrongPayloadDefinition
 
     def topic2handler(self, topic):
         """
         Get a handler for a topic according to the payload definitions
         :param topic:
         :return: The handler
         """
@@ -66,11 +72,11 @@
         """
         Match a topic to an handler according to the config
         :param topic:
         :return:
         """
         for regex, handler in self.topic_re.items():
             if regex.match(topic):
-                self.topic_handlers[topic] = self.topic_handlers[regex]
-                return self.topic_handlers[regex]
+                self.topic_handlers[topic] = self.topic_re[regex]
+                return self.topic_re[regex]
 
         return None
```

### Comparing `amqtt_db-0.1.2/amqtt_db/base/delegator.py` & `amqtt_db-0.1.3/amqtt_db/base/delegator.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.2/amqtt_db/base/utils.py` & `amqtt_db-0.1.3/amqtt_db/base/utils.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.2/amqtt_db/db/db_sa.py` & `amqtt_db-0.1.3/amqtt_db/db/db_sa.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.2/amqtt_db/default_config.yaml` & `amqtt_db-0.1.3/amqtt_db/default_config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -13,18 +13,19 @@
   - amqtt_db
 
 topic-check:
   enabled: False
 
 amqtt_db:
   db_connection : 'sqlite:///test_topic.sqlite'
-  db_structure : amqtt_db.structure.structure:WideStructure
+  db_structure : amqtt_db.structure.structure.WideStructure
 
   payload :
     tinkershop/trh :
       amqtt_db.payload.json_decoder.JSONDecoder :
         amqtt_db.payload.flat_deserializer.FlatDeserializer :
+          moist : int
           temp : float
           rh : float
           press : float
           gas : float
           'current time' : datetime.datetime.utcfromtimestamp
```

### Comparing `amqtt_db-0.1.2/amqtt_db/payload/flat_deserializer.py` & `amqtt_db-0.1.3/amqtt_db/payload/flat_deserializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,10 +33,14 @@
     def deserialize(self, data):
         """
         Deserialize by key name assuming a flat data structure.
         :param data: data
         :return: typed data
         """
         result = {}
+        residual = {}
         for key, value in data.items():
-            result[key] = self.col2type[key](value)  # do the mapping
-        return result
+            try:
+                result[key] = self.col2type[key](value)  # do the mapping
+            except KeyError:
+                residual[key] = None
+        return result, residual
```

### Comparing `amqtt_db-0.1.2/amqtt_db/plugin.py` & `amqtt_db-0.1.3/amqtt_db/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import inspect
 import sys
 import traceback
 
 from amqtt_db.base.base_plugin import BasePlugin
 from amqtt_db.base.base_topic import BaseTopicEngine
 from amqtt_db.base.constants import TOPIC_ENGINE, DB_CONNECT_STRING, DB_STRUCTURE
+from amqtt_db.base.utils import get_class_func_by_name
 from amqtt_db.db.db_sa import SA
-from amqtt_db.structure.structure import WideStructure
 
 
 class DBPlugin(BasePlugin):
     """
     The DB Plugin
     """
 
     config_path = 'plugins.amqtt_db'
     db = None
-    mapper = None
+    structure = None
     topic_engine = None
 
     def __init__(self, context):
         super(DBPlugin, self).__init__(context)
         self.compose()
 
     def handle_exception(self, e):
         msg = "amqtt_db ERROR: {}".format(e.__repr__())
         self.context.logger.error(msg)
         exc_type, exc_value, exc_traceback = sys.exc_info()
         for line in traceback.format_tb(exc_traceback):
             self.context.logger.error(line[:-1])
-        raise ImportError
+        raise ImportError()
 
     def compose(self):
         """
         Constructs the plugin by choosing the structure and the DB interface according to the config
         """
         self.get_topic_engine()
         self.get_db()
-        self.get_mapper()
+        self.get_structure()
         self.register_events()
 
     def get_topic_engine(self):
         """
         Gets the topic engine according to the config
         """
         if TOPIC_ENGINE not in self.config:
@@ -55,53 +55,51 @@
             self.context.logger.error('No topic engine could be started')
             self.handle_exception(e)
 
     def get_db(self):
         """
         Gets the DB according to the config
         """
-        if DB_CONNECT_STRING not in self.config:
-            raise
-
         try:
             connect_string = self.config[DB_CONNECT_STRING]
         except KeyError as e:
             self.context.logger.error('No "db_connection" found in config file at: "{}"'.format(self.config_path))
             self.handle_exception(e)
 
         try:
             self.db = SA(self.context, connect_string)
         except Exception as e:
             msg = 'Connection to DB with connect string: "{}" failed'.format(connect_string)
             self.context.logger.error(msg)
             self.handle_exception(e)
 
-    def get_mapper(self):
+    def get_structure(self):
         """
         Gets the structure according to the config
         """
         try:
-            _mapper_type = self.config[DB_STRUCTURE]  # noqa: F841
+            structure_cls_str = self.config[DB_STRUCTURE]  # noqa: F841
         except KeyError as e:
             msg = 'Cannot read/find "db_structure" entry in config file part "{}"'.format(self.config_path)
             self.context.logger.error(msg)
             self.handle_exception(e)
 
         try:
-            self.mapper = WideStructure(self.topic_engine, self.db, self.context)  # ToDo: Mapper Factory
+            structure_cls = get_class_func_by_name(structure_cls_str)
+            self.structure = structure_cls(self.topic_engine, self.db, self.context)  # ToDo: Mapper Factory
         except Exception as e:
             self.handle_exception(e)
 
     def register_events(self):
         events = {}
-        method_names = inspect.getmembers(self.mapper, predicate=inspect.ismethod)
+        method_names = inspect.getmembers(self.structure, predicate=inspect.ismethod)
         for method_name, method in method_names:
             if method_name.startswith('on_'):
                 events[method_name] = method
         return events
 
     def __getattr__(self, item):
         try:
             result = self.__getattribute__(item)
         except AttributeError:
-            result = getattr(self.mapper, item)
+            result = getattr(self.structure, item)
         return result
```

### Comparing `amqtt_db-0.1.2/amqtt_db/startup.py` & `amqtt_db-0.1.3/amqtt_db/startup.py`

 * *Files identical despite different names*

### Comparing `amqtt_db-0.1.2/amqtt_db/tests/test_db/test_sa.py` & `amqtt_db-0.1.3/amqtt_db/tests/test_db/test_sa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 from datetime import date, time, datetime
 
 import unittest
 
 from amqtt_db.db.db_sa import SA
-from amqtt_db.tests.resources.mockups import context
+from amqtt_db.tests.resources.mockups import get_context, CONFIG_OK
 
 from tempfile import TemporaryDirectory
 
 
 class TestSA(unittest.TestCase):
 
     def create_test_db(self):
         temp_dir = TemporaryDirectory()
         temp_db_file_name = os.path.join(temp_dir.name, 'huhu')
+        context = get_context(CONFIG_OK)
         sa = SA(context, 'sqlite:///{}'.format(temp_db_file_name), echo=True)
         return temp_dir, sa
 
     def test_create_table(self):
         tempdir, sa = self.create_test_db()
 
         column_def = {
```

### Comparing `amqtt_db-0.1.2/pyproject.toml` & `amqtt_db-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amqtt_db"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["volker <volker.jaenisch@inqbus.de>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/volkerjaenisch/amqtt_db"
 repository = "https://github.com/volkerjaenisch/amqtt_db"
@@ -12,27 +12,27 @@
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-amqtt = "^0.10.0-alpha.3"
+#amqtt = "^0.10.0-alpha.3"
 SQLAlchemy = "^1.4.1"
 aiounittest = "^1.4.0"
-psycopg2 = "^2.8.6"
-PyYAML = "^5.4.1"
+psycopg2-binary = "^2.9.9"
+PyYAML = "^6.0.0"
 sqlalchemy-migrate = "^0.13.0"
-Sphinx = "^3.5.3"
-sphinx-rtd-theme = "^0.5.2"
-coverage = "^5.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.3"
+Sphinx = "^3.5.3"
+sphinx-rtd-theme = "^0.5.2"
+coverage = "^5.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.plugins."amqtt.broker.plugins"]
-amqtt_db = "amqtt_db.plugin:DBPlugin"
+amqtt_db = "amqtt_db.plugin:DBPlugin"
```

### Comparing `amqtt_db-0.1.2/PKG-INFO` & `amqtt_db-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
-Name: amqtt-db
-Version: 0.1.2
+Name: amqtt_db
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/volkerjaenisch/amqtt_db
 License: MIT
 Keywords: amqtt,MQTT,Persistence,SQLAlchemy,Database
 Author: volker
 Author-email: volker.jaenisch@inqbus.de
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.1,<2.0.0)
-Requires-Dist: Sphinx (>=3.5.3,<4.0.0)
 Requires-Dist: aiounittest (>=1.4.0,<2.0.0)
-Requires-Dist: amqtt (>=0.10.0-alpha.3,<0.11.0)
-Requires-Dist: coverage (>=5.5,<6.0)
-Requires-Dist: psycopg2 (>=2.8.6,<3.0.0)
-Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0)
+Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: sqlalchemy-migrate (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/volkerjaenisch/amqtt_db
 Description-Content-Type: text/markdown
 
 amqtt_db
 ========
 
 ![license](https://img.shields.io/github/license/volkerjaenisch/amqtt_db?style=flat-square)
-![travis](https://api.travis-ci.org/volkerjaenisch/amqtt_db.svg?branch=main)
-![coverals](https://coveralls.io/repos/github/volkerjaenisch/amqtt_db/badge.svg)
-[![PyPI](https://img.shields.io/pypi/v/amqtt_db?style=flat-square)](https://pypi.org/project/amqtt/)
+[![Build Status](https://travis-ci.org/volkerjaenisch/amqtt_db.svg?branch=main)](https://travis-ci.org/volkerjaenisch/amqtt_db)
+[![Coverage Status](https://coveralls.io/repos/github/volkerjaenisch/amqtt_db/badge.svg?branch=main)](https://coveralls.io/github/volkerjaenisch/amqtt_db?branch=main)
+[![PyPI](https://img.shields.io/pypi/v/amqtt_db)](https://pypi.org/project/amqtt_db/)
 [![Documantation](https://img.shields.io/readthedocs/amqtt-db.svg)](https://amqtt_db.readthedocs.io/en/latest/)
 
-DB persistence for amqtt.
+DB persistence for [amqtt](https://github.com/Yakifo/amqtt).
 
 Objective
 ---------
 
-amqtt_db will persist payloads received by the [amqtt broker](https://github.com/Yakifo/amqtt) into performant relational databases.
+amqtt_db persists payloads received by the [amqtt broker](https://github.com/Yakifo/amqtt) into performant relational databases.
 SQLAlchemy as well as timescaleBD are the target RMDB-Systems.
 
 amqtt_db will do four steps to persist the amqtt data:
 
  1) decoding the payload (e.G. from binary, JSON or which ever encoding)
  1) deserializing the payload to typed Python entities
  1) structure the session, topic, property, value information into a relational model of your choice
```

