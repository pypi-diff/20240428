# Comparing `tmp/avrotize-1.3.1.tar.gz` & `tmp/avrotize-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.3.1.tar` & `avrotize-1.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    25996 2024-04-18 12:20:03.776874 avrotize-1.3.1/README.md
--rw-r--r--   0        0        0     1673 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-18 12:20:09.772929 avrotize-1.3.1/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    15558 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotize.py
--rw-r--r--   0        0        0    43143 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    18563 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13101 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-18 12:20:03.776874 avrotize-1.3.1/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12889 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-04-18 12:20:03.780874 avrotize-1.3.1/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-04-18 12:20:03.780874 avrotize-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    26663 1970-01-01 00:00:00.000000 avrotize-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    26753 2024-04-28 10:06:15.632197 avrotize-1.3.2/README.md
+-rw-r--r--   0        0        0     1673 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-28 10:06:20.164220 avrotize-1.3.2/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    15558 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotize.py
+-rw-r--r--   0        0        0    43143 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    18563 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13101 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12889 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1138 2024-04-28 10:06:15.636197 avrotize-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    27420 1970-01-01 00:00:00.000000 avrotize-1.3.2/PKG-INFO
```

### Comparing `avrotize-1.3.1/README.md` & `avrotize-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -69,18 +69,27 @@
 - emerged out of the Apache Hadoop ecosystem and is widely used for
   serialization and storage of data and for data exchange between systems.
 - supports native and logical types that cover the needs of many business and
   technical use cases.
 - can describe the popular JSON data encoding very well and in a way that always
   maps cleanly to a wide range of programming languages and systems. In
   contrast, it's quite easy to inadvertently define a JSON Schema that is very
-  difficult to map to a programming language structure.
+  difficult to map to a programming language structure. 
 - is itself expressed as JSON. That makes it easy to parse and generate, which
   is not the case for Protobuf or ASN.1, which require bespoke parsers.
 
+> It needs to be noted here that while Avro Schema is great for defining data
+> structures, and data classes generated from Avro Schema using this tool or
+> other tools can be used to with the most popular JSON serialization libraries,
+> the Apache Avro project's own JSON encoding has fairly grave interoperability
+> issues with common usage of JSON. A alternate Avro JSON encoding that is more
+> interoperable is proposed in [`avrojson.md`](avrojson.md) for submission to
+> the Apache Avro project; the document also enumerates the specific
+> interoperability issues.
+
 Avro Schema does not support all the bells and whistles of XML Schema or JSON
 Schema, but that is a feature, not a bug, as it ensures the portability of the
 schemas across different systems and infrastructures. Specifically, Avro Schema
 does not support many of the data validation features found in JSON Schema or
 XML Schema. There are no `pattern`, `format`, `minimum`, `maximum`, or `required`
 keywords in Avro Schema, and Avro does not support conditional validation.
 
@@ -259,14 +268,17 @@
   Avro type.
 - `complexType` declarations that have simple content where a base type is augmented
   with attributes is mapped to a record type in Avro. Any other facets defined on
   the complex type are ignored.
 - If the schema defines a single root element, the tool will emit a single Avro
   record type. If the schema defines multiple root elements, the tool will emit a
   union of record types, each corresponding to a root element.
+- All fields in the resulting Avro Schema are annotated with an `xmlkind`
+  extension attribute that indicates whether the field was an `element` or an
+  `attribute` in the XML schema.
 
 ## Convert Avro schema to XML schema
 
 ```bash
 avrotize a2x --avsc <path_to_avro_schema_file> --xsd <path_to_xsd_schema_file>
 ```
```

### Comparing `avrotize-1.3.1/avrotize/__init__.py` & `avrotize-1.3.2/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/asn1toavro.py` & `avrotize-1.3.2/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotize.py` & `avrotize-1.3.2/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotocsharp.py` & `avrotize-1.3.2/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotojava.py` & `avrotize-1.3.2/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotojs.py` & `avrotize-1.3.2/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotojsons.py` & `avrotize-1.3.2/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotokusto.py` & `avrotize-1.3.2/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotoparquet.py` & `avrotize-1.3.2/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotoproto.py` & `avrotize-1.3.2/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotopython.py` & `avrotize-1.3.2/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotots.py` & `avrotize-1.3.2/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrototsql.py` & `avrotize-1.3.2/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/avrotoxsd.py` & `avrotize-1.3.2/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/common.py` & `avrotize-1.3.2/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/dependency_resolver.py` & `avrotize-1.3.2/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/generic/generic.avsc` & `avrotize-1.3.2/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/jsonstoavro.py` & `avrotize-1.3.2/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/kconnect.json` & `avrotize-1.3.2/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/kstructtoavro.py` & `avrotize-1.3.2/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/proto2parser.py` & `avrotize-1.3.2/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/proto3parser.py` & `avrotize-1.3.2/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototoavro.py` & `avrotize-1.3.2/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototypes/any.avsc` & `avrotize-1.3.2/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototypes/api.avsc` & `avrotize-1.3.2/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototypes/duration.avsc` & `avrotize-1.3.2/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototypes/field_mask.avsc` & `avrotize-1.3.2/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototypes/struct.avsc` & `avrotize-1.3.2/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototypes/timestamp.avsc` & `avrotize-1.3.2/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototypes/type.avsc` & `avrotize-1.3.2/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/prototypes/wrappers.avsc` & `avrotize-1.3.2/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/avrotize/xsdtoavro.py` & `avrotize-1.3.2/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.1/pyproject.toml` & `avrotize-1.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,26 @@
     "jsonschema>=4.17.3",
     "lark>=1.1.9",
     "pyarrow>=15.0.0",
     "asn1tools>=0.166.0",
     "jsonpointer>=2.4",
     "jsonpath-ng>=1.6.1",
     "jsoncomparison>=1.1.0",
-    "requests>=2.31.0"
+    "requests>=2.31.0",
 ]
 dev-dependencies = [
     "pytest>=7.2.1",
     "fastavro>=1.9.4",
     "xmlschema>=3.0.2",
     "xmlunittest>=0.5.0",
+    "pylint>=3.1.0",
+    "dataclasses_json>0.6.4",
+    "dataclasses>=0.6",
+    "pydantic>=2.7.1",
+    "avro>=1.11.3",
 ]
 
 [project.scripts]
 avrotize = "avrotize.avrotize:main"
 
 [tool.setuptools_scm]
 write_to = "avrotize/_version.py"
```

### Comparing `avrotize-1.3.1/PKG-INFO` & `avrotize-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -88,18 +88,27 @@
 - emerged out of the Apache Hadoop ecosystem and is widely used for
   serialization and storage of data and for data exchange between systems.
 - supports native and logical types that cover the needs of many business and
   technical use cases.
 - can describe the popular JSON data encoding very well and in a way that always
   maps cleanly to a wide range of programming languages and systems. In
   contrast, it's quite easy to inadvertently define a JSON Schema that is very
-  difficult to map to a programming language structure.
+  difficult to map to a programming language structure. 
 - is itself expressed as JSON. That makes it easy to parse and generate, which
   is not the case for Protobuf or ASN.1, which require bespoke parsers.
 
+> It needs to be noted here that while Avro Schema is great for defining data
+> structures, and data classes generated from Avro Schema using this tool or
+> other tools can be used to with the most popular JSON serialization libraries,
+> the Apache Avro project's own JSON encoding has fairly grave interoperability
+> issues with common usage of JSON. A alternate Avro JSON encoding that is more
+> interoperable is proposed in [`avrojson.md`](avrojson.md) for submission to
+> the Apache Avro project; the document also enumerates the specific
+> interoperability issues.
+
 Avro Schema does not support all the bells and whistles of XML Schema or JSON
 Schema, but that is a feature, not a bug, as it ensures the portability of the
 schemas across different systems and infrastructures. Specifically, Avro Schema
 does not support many of the data validation features found in JSON Schema or
 XML Schema. There are no `pattern`, `format`, `minimum`, `maximum`, or `required`
 keywords in Avro Schema, and Avro does not support conditional validation.
 
@@ -278,14 +287,17 @@
   Avro type.
 - `complexType` declarations that have simple content where a base type is augmented
   with attributes is mapped to a record type in Avro. Any other facets defined on
   the complex type are ignored.
 - If the schema defines a single root element, the tool will emit a single Avro
   record type. If the schema defines multiple root elements, the tool will emit a
   union of record types, each corresponding to a root element.
+- All fields in the resulting Avro Schema are annotated with an `xmlkind`
+  extension attribute that indicates whether the field was an `element` or an
+  `attribute` in the XML schema.
 
 ## Convert Avro schema to XML schema
 
 ```bash
 avrotize a2x --avsc <path_to_avro_schema_file> --xsd <path_to_xsd_schema_file>
 ```
```

