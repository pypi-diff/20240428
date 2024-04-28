# Comparing `tmp/zodchy_notations-0.1.0.tar.gz` & `tmp/zodchy_notations-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_notations-0.1.0.tar", max compression
+gzip compressed data, was "zodchy_notations-0.1.1.tar", max compression
```

## Comparing `zodchy_notations-0.1.0.tar` & `zodchy_notations-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy_notations-0.1.0/README.md
--rw-r--r--   0        0        0      369 2024-04-27 07:00:13.436411 zodchy_notations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       20 2024-04-27 06:57:44.545249 zodchy_notations-0.1.0/zodchy_notations/__init__.py
--rw-r--r--   0        0        0       19 2024-04-27 06:57:44.549266 zodchy_notations-0.1.0/zodchy_notations/query/__init__.py
--rw-r--r--   0        0        0     7831 2024-04-26 14:09:47.292566 zodchy_notations-0.1.0/zodchy_notations/query/math.py
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 zodchy_notations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy_notations-0.1.1/README.md
+-rw-r--r--   0        0        0      368 2024-04-28 14:38:12.562312 zodchy_notations-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-04-27 06:57:44.545249 zodchy_notations-0.1.1/zodchy_notations/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-27 06:57:44.549266 zodchy_notations-0.1.1/zodchy_notations/query/__init__.py
+-rw-r--r--   0        0        0     7881 2024-04-28 14:38:12.571927 zodchy_notations-0.1.1/zodchy_notations/query/math.py
+-rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 zodchy_notations-0.1.1/PKG-INFO
```

### Comparing `zodchy_notations-0.1.0/zodchy_notations/query/math.py` & `zodchy_notations-0.1.1/zodchy_notations/query/math.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,20 @@
     datetime.datetime,
     datetime.date,
     int,
     float
 )
 
 
+@dataclasses.dataclass
+class Param:
+    name: str
+    value: codex.query.ClauseBit
+
+
 class Parser:
     def __init__(
         self,
         types_map: collections.abc.Mapping[FieldName, FieldType],
         casting_map: collections.abc.Mapping[
             FieldType,
             collections.abc.Callable[[str], typing.Any]
@@ -57,56 +63,57 @@
         self._types_map = types_map
         self._casting_map = casting_map
         self._parsing_schema = parsing_schema
 
     def __call__(
         self,
         query: str | collections.abc.Mapping[str, str]
-    ) -> collections.abc.Generator[codex.query.Param, None, None]:
+    ) -> collections.abc.Generator[tuple[str, codex.query.ClauseBit], None, None]:
         if isinstance(query, str):
             if '=' not in query:
                 raise ValueError('You have to specify name for parameter value')
             query = (pairs.split('=') for pairs in query.split('&'))
         elif isinstance(query, collections.abc.Mapping):
             query = query.items()
         else:
             raise ValueError('Query mast be string or mapping')
-        yield from self._parse(query)
+        for param in self._parse(query):
+            yield param.name, param.value
 
     def _parse(self, query: collections.abc.Iterable[tuple[str, str]]):
         for pair in query:
             k, v = pair
             if v is None:
                 continue
             if k == self._parsing_schema.order_by:
                 yield from self._parse_order_param(v)
             elif k == self._parsing_schema.limit:
-                yield codex.query.Param(
+                yield Param(
                     name=self._parsing_schema.limit,
                     value=codex.query.Limit(int(v))
                 )
             elif k == self._parsing_schema.offset:
-                yield codex.query.Param(
+                yield Param(
                     name=self._parsing_schema.offset,
                     value=codex.query.Offset(int(v))
                 )
             else:
                 yield self._parse_filter_param(k, v.strip())
 
     @staticmethod
     def _parse_order_param(
         names: FieldName
-    ) -> collections.abc.Generator[codex.query.Param, None, None]:
+    ) -> collections.abc.Generator[Param, None, None]:
         priority = 0
         for name in names.split(','):
             direction = codex.query.ASC
             if name.startswith('-'):
                 direction = codex.query.DESC
                 name = name[1:]
-            yield codex.query.Param(
+            yield Param(
                 name=name,
                 value=direction(priority)
             )
             priority += 1
 
     def _parse_filter_param(self, name: FieldName, value: str):
         if name not in self._types_map:
@@ -120,15 +127,15 @@
         self,
         field_name: str,
         field_value: str,
         operations: tuple[
             type[codex.query.GT | codex.query.GE],
             type[codex.query.LT | codex.query.LE]
         ]
-    ) -> codex.query.Param:
+    ) -> Param:
         if self._types_map[field_name] not in interval_types:
             raise TypeError(
                 f'Interval cannot be calculated for type {self._types_map[field_name]} for field {field_name}')
 
         _data = field_value.split(',')
         if len(_data) != 2:
             raise ValueError(f'Range must contain strictly two members for field {field_name}')
@@ -137,15 +144,15 @@
         right = None
         if _data[0]:
             left = operations[0](self._cast(_data[0], self._types_map[field_name]))
         if _data[1]:
             right = operations[1](self._cast(_data[1], self._types_map[field_name]))
         value = codex.query.RANGE(left, right)
 
-        return codex.query.Param(name=field_name, value=value)
+        return Param(name=field_name, value=value)
 
     def _multitude(
         self,
         field_name: str,
         field_value: str,
         inversion: bool = False
     ):
@@ -156,15 +163,15 @@
                 if v
             )
         )
 
         if inversion:
             field_value = codex.query.NOT(field_value)
 
-        return codex.query.Param(
+        return Param(
             name=field_name,
             value=field_value
         )
 
     def _literal(
         self,
         field_name: str,
@@ -173,15 +180,15 @@
         inversion: bool = False
     ):
         field_value = operation(self._cast(field_value, self._types_map[field_name]))
 
         if inversion:
             field_value = codex.query.NOT(field_value)
 
-        return codex.query.Param(
+        return Param(
             name=field_name,
             value=field_value,
         )
 
     def _cast(self, value: str, type_: type):
         if cast := self._casting_map.get(type_):
             return cast(value)
```

