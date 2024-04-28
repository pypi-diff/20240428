# Comparing `tmp/typedmongo-1.0.4.tar.gz` & `tmp/typedmongo-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.0.4.tar", last modified: Fri Apr 26 09:32:11 2024, max compression
+gzip compressed data, was "typedmongo-1.0.5.tar", last modified: Sun Apr 28 06:22:47 2024, max compression
```

## Comparing `typedmongo-1.0.4.tar` & `typedmongo-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-26 09:32:00.462717 typedmongo-1.0.4/LICENSE
--rw-r--r--   0        0        0      108 2024-04-26 09:32:00.462717 typedmongo-1.0.4/README.md
--rw-r--r--   0        0        0     1441 2024-04-26 09:32:11.946695 typedmongo-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5789 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     3014 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/sync.py
--rw-r--r--   0        0        0     5549 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/test_marshamallow.py
--rw-r--r--   0        0        0     3006 2024-04-26 09:32:00.462717 typedmongo-1.0.4/tests/test_table.py
--rw-r--r--   0        0        0      749 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/__init__.py
--rw-r--r--   0        0        0      749 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    11769 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     8894 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     7670 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    11551 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/expressions.py
--rw-r--r--   0        0        0     8894 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/fields.py
--rw-r--r--   0        0        0      351 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/sync.py
--rw-r--r--   0        0        0     7670 2024-04-26 09:32:00.462717 typedmongo-1.0.4/typedmongo/table.py
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-28 06:22:36.040321 typedmongo-1.0.5/LICENSE
+-rw-r--r--   0        0        0      108 2024-04-28 06:22:36.040321 typedmongo-1.0.5/README.md
+-rw-r--r--   0        0        0     1441 2024-04-28 06:22:47.528313 typedmongo-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5789 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     3211 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/sync.py
+-rw-r--r--   0        0        0     5549 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     3203 2024-04-28 06:22:36.040321 typedmongo-1.0.5/tests/test_table.py
+-rw-r--r--   0        0        0      749 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/__init__.py
+-rw-r--r--   0        0        0      749 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    11769 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     8920 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     7820 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    11551 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/expressions.py
+-rw-r--r--   0        0        0     8920 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/fields.py
+-rw-r--r--   0        0        0      351 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/sync.py
+-rw-r--r--   0        0        0     7820 2024-04-28 06:22:36.040321 typedmongo-1.0.5/typedmongo/table.py
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.0.5/PKG-INFO
```

### Comparing `typedmongo-1.0.4/LICENSE` & `typedmongo-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/pyproject.toml` & `typedmongo-1.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.0.4"
+version = "1.0.5"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.0.4/tests/asyncio/test_client.py` & `typedmongo-1.0.5/tests/asyncio/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/tests/asyncio/test_table.py` & `typedmongo-1.0.5/tests/test_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import uuid
 
 import pytest
 
-import typedmongo.asyncio as mongo
+import typedmongo as mongo
 from typedmongo.expressions import Expression
 
 
 class MongoTable(mongo.Table):
     __abstract__ = True
 
     _id: mongo.StringField = mongo.StringField(default=lambda: uuid.uuid4().hex)
@@ -87,14 +87,20 @@
             "wallet": {"balance": 100},
             "children": [],
         },
         partial=True,
     )
     assert isinstance(user._id, str)
 
+    user = User(
+        name="Aber", age=18, tags=["a", "b"], wallet=Wallet(balance=100), children=[]
+    )
+    assert not hasattr(user, "_id")
+    assert isinstance(user.dump(user)["_id"], str)
+
 
 def test_recursion_field():
     user = User.load(
         {
             "name": "Aber",
             "age": 18,
             "tags": ["a", "b"],
```

### Comparing `typedmongo-1.0.4/tests/sync.py` & `typedmongo-1.0.5/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/tests/test_client.py` & `typedmongo-1.0.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/tests/test_expressions.py` & `typedmongo-1.0.5/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/tests/test_marshamallow.py` & `typedmongo-1.0.5/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/tests/test_table.py` & `typedmongo-1.0.5/tests/asyncio/test_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import uuid
 
 import pytest
 
-import typedmongo as mongo
+import typedmongo.asyncio as mongo
 from typedmongo.expressions import Expression
 
 
 class MongoTable(mongo.Table):
     __abstract__ = True
 
     _id: mongo.StringField = mongo.StringField(default=lambda: uuid.uuid4().hex)
@@ -87,14 +87,20 @@
             "wallet": {"balance": 100},
             "children": [],
         },
         partial=True,
     )
     assert isinstance(user._id, str)
 
+    user = User(
+        name="Aber", age=18, tags=["a", "b"], wallet=Wallet(balance=100), children=[]
+    )
+    assert not hasattr(user, "_id")
+    assert isinstance(user.dump(user)["_id"], str)
+
 
 def test_recursion_field():
     user = User.load(
         {
             "name": "Aber",
             "age": 18,
             "tags": ["a", "b"],
```

### Comparing `typedmongo-1.0.4/typedmongo/__init__.py` & `typedmongo-1.0.5/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/typedmongo/asyncio/__init__.py` & `typedmongo-1.0.5/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/typedmongo/asyncio/client.py` & `typedmongo-1.0.5/typedmongo/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/typedmongo/asyncio/fields.py` & `typedmongo-1.0.5/typedmongo/asyncio/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 from typedmongo.expressions import CompareMixin, HasFieldName, OrderByMixin
 from typedmongo.marshamallow import MarshamallowObjectId
 
 if TYPE_CHECKING:
     from .table import Table
 
-A = TypeVar("A")
 TypeTable = TypeVar("TypeTable", bound=type["Table"])
 T = TypeVar("T", bound="Table")
 TypeTableOrAny = TypeVar("TypeTableOrAny", bound=type["Table"] | Any)
 FieldType = TypeVar("FieldType")
 
 
 @dataclasses.dataclass
@@ -60,14 +59,15 @@
         if not hasattr(self, "marshamallow"):
             self.marshamallow = fields.Field(required=True, allow_none=False)
 
         if self.default is not None:
             # https://github.com/marshmallow-code/marshmallow/issues/2151
             self.marshamallow.required = False
             self.marshamallow.load_default = self.default
+            self.marshamallow.dump_default = self.default
 
     @overload
     def __get__(self: Self, instance: None, cls: type) -> Self: ...
 
     @overload
     def __get__(self: Self, instance: object, cls: type) -> FieldType: ...
 
@@ -87,24 +87,23 @@
     def __delete__(self, instance: Table) -> None:
         try:
             del instance.__dict__[self._name]
         except KeyError:
             message = "{0} has no attribute '{1}'".format(instance, self._name)
             raise AttributeError(message)
 
-    @classmethod
-    def get_field_type(cls) -> type[FieldType]:
-        if hasattr(cls, "__field_type__"):
-            return cls.__field_type__  # type: ignore
-        for origin_base in cls.__orig_bases__:  # type: ignore
+    def get_field_type(self) -> type[FieldType]:
+        if hasattr(self, "__field_type__"):
+            return self.__field_type__  # type: ignore
+        for origin_base in self.__orig_bases__:  # type: ignore
             origin_class = get_origin(origin_base)
             if isinstance(origin_class, type) and issubclass(origin_class, Field):
-                cls.__field_type__ = generic_type = get_args(origin_base)[0]
+                self.__field_type__ = generic_type = get_args(origin_base)[0]
                 return generic_type
-        raise RuntimeError(f"Cannot get field type for {cls}")
+        raise RuntimeError(f"Cannot get field type for {self}")
 
     def load(self, value: Any, *, partial: bool = False) -> FieldType:
         return value
 
     def dump(self, value: FieldType) -> Any:
         return value
 
@@ -218,14 +217,17 @@
         self.dump = dump
 
     def __set_name__(self, owner: type[Table], name: str) -> None:
         if not issubclass(self.schema, owner):
             self.schema.__lazy_init_fields__()
         return super().__set_name__(owner, name)
 
+    def get_field_type(self) -> type[T]:
+        return self.schema
+
 
 @dataclasses.dataclass(eq=False)
 class ListFieldNameProxy(Generic[TypeTableOrAny], OrderByMixin, CompareMixin):
     number: int | None
     prefix: HasFieldName
     t: TypeTableOrAny
 
@@ -244,59 +246,62 @@
             )
         except KeyError:
             message = "{0} has no attribute '{1}'".format(self.t, name)
             raise AttributeError(message) from None
 
 
 @dataclasses.dataclass(eq=False)
-class ListField(Generic[A], Field[list[A]]):
+class ListField(Generic[FieldType], Field[list[FieldType]]):
     """
     List field
     """
 
-    _: ListFieldNameProxy[type[A]] = dataclasses.field(init=False)
+    _: ListFieldNameProxy[type[FieldType]] = dataclasses.field(init=False)
 
-    type_or_schema: type[A]
+    field: Field[FieldType]
 
-    def __getitem__(self, index: int) -> type[A]:
-        return ListFieldNameProxy(index, self, self.type_or_schema)  # type: ignore
+    def __getitem__(self, index: int) -> type[FieldType]:
+        return ListFieldNameProxy(index, self, self.field.get_field_type())  # type: ignore
 
     def __post_init__(self):
-        self._ = ListFieldNameProxy(None, self, self.type_or_schema)
+        self._ = ListFieldNameProxy(None, self, self.field.get_field_type())  # type: ignore
 
-        from .table import Table
+        self.marshamallow = fields.List(self.field.marshamallow)  # type: ignore
 
-        if issubclass(self.type_or_schema, Table):
-            self.marshamallow = fields.List(
-                fields.Nested(lambda: self.type_or_schema.__schema__)  # type: ignore
-            )
+        if isinstance(self.field, EmbeddedField):
+            self.marshamallow = fields.List(self.field.marshamallow)
 
-            def load(value: Any, *, partial: bool = False) -> list[A]:
-                return [
-                    self.type_or_schema.load(item, partial=partial)  # type: ignore
-                    for item in value
-                ]
+            def load(value: Any, *, partial: bool = False) -> list[FieldType]:
+                return [self.field.load(item, partial=partial) for item in value]  # type: ignore
 
-            def dump(value: list[A]) -> list[dict[str, Any]]:
-                return [self.type_or_schema.dump(item) for item in value]  # type: ignore
+            def dump(value: list[FieldType]) -> list[dict[str, Any]]:
+                return [self.field.dump(item) for item in value]  # type: ignore
 
             self.load = load
             self.dump = dump
-        else:
-            self.marshamallow = fields.List(
-                {
-                    int: fields.Integer(required=True, allow_none=False),
-                    float: fields.Float(required=True, allow_none=False),
-                    bool: fields.Boolean(required=True, allow_none=False),
-                    str: fields.String(required=True, allow_none=False),
-                    datetime: fields.DateTime(required=True, allow_none=False),
-                }[self.type_or_schema]  # type: ignore
-            )
 
-    def __set_name__(self, owner: type[Table], name: str) -> None:
-        from .table import Table
+    def get_field_type(self) -> type[list[FieldType]]:
+        return list[self.field.get_field_type()]  # type: ignore
 
-        if issubclass(self.type_or_schema, Table) and not issubclass(
-            self.type_or_schema, owner
-        ):
-            self.type_or_schema.__lazy_init_fields__()
-        return super().__set_name__(owner, name)
+
+def type_to_field(type_: type) -> Field:
+    from .table import Table
+
+    if type_ is str:
+        return StringField()
+    if type_ is int:
+        return IntegerField()
+    if type_ is float:
+        return FloatField()
+    if type_ is bool:
+        return BooleanField()
+    if type_ is datetime:
+        return DateTimeField()
+    if type_ is decimal.Decimal:
+        return DecimalField()
+    if type_ is ObjectId:
+        return ObjectIdField()
+    if issubclass(type_, Table):
+        return EmbeddedField(type_)
+    if get_origin(type_) is list:
+        return ListField(type_to_field(get_args(type_)[0]))
+    raise ValueError(f"Cannot convert type {type_} to field")
```

### Comparing `typedmongo-1.0.4/typedmongo/asyncio/table.py` & `typedmongo-1.0.5/typedmongo/asyncio/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from marshmallow import Schema
 from pymongo import IndexModel
 from typing_extensions import Self, dataclass_transform
 
 from typedmongo.exceptions import TableDefineError
 
 from .client import Manager
-from .fields import Field
+from .fields import Field, ListField, type_to_field
 
 
 def snake_case(name: str) -> str:
     """
     convert "SomeWords" to "some_words"
     """
     return "".join(
@@ -126,15 +126,17 @@
         fields = {
             **{
                 name: value()
                 for name, value in inspect.get_annotations(cls, eval_str=True).items()
                 if isinstance(value, type) and issubclass(value, Field)
             },
             **{
-                name: origin_class(*get_args(value))
+                name: origin_class(type_to_field(get_args(value)[0]))
+                if issubclass(origin_class, ListField)
+                else origin_class(*get_args(value))
                 for name, value in inspect.get_annotations(cls, eval_str=True).items()
                 if (origin_class := get_origin(value))
                 and isinstance(origin_class, type)
                 and issubclass(origin_class, Field)
             },
             **cls.__sfields__,
         }
```

### Comparing `typedmongo-1.0.4/typedmongo/client.py` & `typedmongo-1.0.5/typedmongo/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/typedmongo/expressions.py` & `typedmongo-1.0.5/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/typedmongo/fields.py` & `typedmongo-1.0.5/typedmongo/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 from typedmongo.expressions import CompareMixin, HasFieldName, OrderByMixin
 from typedmongo.marshamallow import MarshamallowObjectId
 
 if TYPE_CHECKING:
     from .table import Table
 
-A = TypeVar("A")
 TypeTable = TypeVar("TypeTable", bound=type["Table"])
 T = TypeVar("T", bound="Table")
 TypeTableOrAny = TypeVar("TypeTableOrAny", bound=type["Table"] | Any)
 FieldType = TypeVar("FieldType")
 
 
 @dataclasses.dataclass
@@ -60,14 +59,15 @@
         if not hasattr(self, "marshamallow"):
             self.marshamallow = fields.Field(required=True, allow_none=False)
 
         if self.default is not None:
             # https://github.com/marshmallow-code/marshmallow/issues/2151
             self.marshamallow.required = False
             self.marshamallow.load_default = self.default
+            self.marshamallow.dump_default = self.default
 
     @overload
     def __get__(self: Self, instance: None, cls: type) -> Self: ...
 
     @overload
     def __get__(self: Self, instance: object, cls: type) -> FieldType: ...
 
@@ -87,24 +87,23 @@
     def __delete__(self, instance: Table) -> None:
         try:
             del instance.__dict__[self._name]
         except KeyError:
             message = "{0} has no attribute '{1}'".format(instance, self._name)
             raise AttributeError(message)
 
-    @classmethod
-    def get_field_type(cls) -> type[FieldType]:
-        if hasattr(cls, "__field_type__"):
-            return cls.__field_type__  # type: ignore
-        for origin_base in cls.__orig_bases__:  # type: ignore
+    def get_field_type(self) -> type[FieldType]:
+        if hasattr(self, "__field_type__"):
+            return self.__field_type__  # type: ignore
+        for origin_base in self.__orig_bases__:  # type: ignore
             origin_class = get_origin(origin_base)
             if isinstance(origin_class, type) and issubclass(origin_class, Field):
-                cls.__field_type__ = generic_type = get_args(origin_base)[0]
+                self.__field_type__ = generic_type = get_args(origin_base)[0]
                 return generic_type
-        raise RuntimeError(f"Cannot get field type for {cls}")
+        raise RuntimeError(f"Cannot get field type for {self}")
 
     def load(self, value: Any, *, partial: bool = False) -> FieldType:
         return value
 
     def dump(self, value: FieldType) -> Any:
         return value
 
@@ -218,14 +217,17 @@
         self.dump = dump
 
     def __set_name__(self, owner: type[Table], name: str) -> None:
         if not issubclass(self.schema, owner):
             self.schema.__lazy_init_fields__()
         return super().__set_name__(owner, name)
 
+    def get_field_type(self) -> type[T]:
+        return self.schema
+
 
 @dataclasses.dataclass(eq=False)
 class ListFieldNameProxy(Generic[TypeTableOrAny], OrderByMixin, CompareMixin):
     number: int | None
     prefix: HasFieldName
     t: TypeTableOrAny
 
@@ -244,59 +246,62 @@
             )
         except KeyError:
             message = "{0} has no attribute '{1}'".format(self.t, name)
             raise AttributeError(message) from None
 
 
 @dataclasses.dataclass(eq=False)
-class ListField(Generic[A], Field[list[A]]):
+class ListField(Generic[FieldType], Field[list[FieldType]]):
     """
     List field
     """
 
-    _: ListFieldNameProxy[type[A]] = dataclasses.field(init=False)
+    _: ListFieldNameProxy[type[FieldType]] = dataclasses.field(init=False)
 
-    type_or_schema: type[A]
+    field: Field[FieldType]
 
-    def __getitem__(self, index: int) -> type[A]:
-        return ListFieldNameProxy(index, self, self.type_or_schema)  # type: ignore
+    def __getitem__(self, index: int) -> type[FieldType]:
+        return ListFieldNameProxy(index, self, self.field.get_field_type())  # type: ignore
 
     def __post_init__(self):
-        self._ = ListFieldNameProxy(None, self, self.type_or_schema)
+        self._ = ListFieldNameProxy(None, self, self.field.get_field_type())  # type: ignore
 
-        from .table import Table
+        self.marshamallow = fields.List(self.field.marshamallow)  # type: ignore
 
-        if issubclass(self.type_or_schema, Table):
-            self.marshamallow = fields.List(
-                fields.Nested(lambda: self.type_or_schema.__schema__)  # type: ignore
-            )
+        if isinstance(self.field, EmbeddedField):
+            self.marshamallow = fields.List(self.field.marshamallow)
 
-            def load(value: Any, *, partial: bool = False) -> list[A]:
-                return [
-                    self.type_or_schema.load(item, partial=partial)  # type: ignore
-                    for item in value
-                ]
+            def load(value: Any, *, partial: bool = False) -> list[FieldType]:
+                return [self.field.load(item, partial=partial) for item in value]  # type: ignore
 
-            def dump(value: list[A]) -> list[dict[str, Any]]:
-                return [self.type_or_schema.dump(item) for item in value]  # type: ignore
+            def dump(value: list[FieldType]) -> list[dict[str, Any]]:
+                return [self.field.dump(item) for item in value]  # type: ignore
 
             self.load = load
             self.dump = dump
-        else:
-            self.marshamallow = fields.List(
-                {
-                    int: fields.Integer(required=True, allow_none=False),
-                    float: fields.Float(required=True, allow_none=False),
-                    bool: fields.Boolean(required=True, allow_none=False),
-                    str: fields.String(required=True, allow_none=False),
-                    datetime: fields.DateTime(required=True, allow_none=False),
-                }[self.type_or_schema]  # type: ignore
-            )
 
-    def __set_name__(self, owner: type[Table], name: str) -> None:
-        from .table import Table
+    def get_field_type(self) -> type[list[FieldType]]:
+        return list[self.field.get_field_type()]  # type: ignore
 
-        if issubclass(self.type_or_schema, Table) and not issubclass(
-            self.type_or_schema, owner
-        ):
-            self.type_or_schema.__lazy_init_fields__()
-        return super().__set_name__(owner, name)
+
+def type_to_field(type_: type) -> Field:
+    from .table import Table
+
+    if type_ is str:
+        return StringField()
+    if type_ is int:
+        return IntegerField()
+    if type_ is float:
+        return FloatField()
+    if type_ is bool:
+        return BooleanField()
+    if type_ is datetime:
+        return DateTimeField()
+    if type_ is decimal.Decimal:
+        return DecimalField()
+    if type_ is ObjectId:
+        return ObjectIdField()
+    if issubclass(type_, Table):
+        return EmbeddedField(type_)
+    if get_origin(type_) is list:
+        return ListField(type_to_field(get_args(type_)[0]))
+    raise ValueError(f"Cannot convert type {type_} to field")
```

### Comparing `typedmongo-1.0.4/typedmongo/sync.py` & `typedmongo-1.0.5/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.4/typedmongo/table.py` & `typedmongo-1.0.5/typedmongo/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from marshmallow import Schema
 from pymongo import IndexModel
 from typing_extensions import Self, dataclass_transform
 
 from typedmongo.exceptions import TableDefineError
 
 from .client import Manager
-from .fields import Field
+from .fields import Field, ListField, type_to_field
 
 
 def snake_case(name: str) -> str:
     """
     convert "SomeWords" to "some_words"
     """
     return "".join(
@@ -126,15 +126,17 @@
         fields = {
             **{
                 name: value()
                 for name, value in inspect.get_annotations(cls, eval_str=True).items()
                 if isinstance(value, type) and issubclass(value, Field)
             },
             **{
-                name: origin_class(*get_args(value))
+                name: origin_class(type_to_field(get_args(value)[0]))
+                if issubclass(origin_class, ListField)
+                else origin_class(*get_args(value))
                 for name, value in inspect.get_annotations(cls, eval_str=True).items()
                 if (origin_class := get_origin(value))
                 and isinstance(origin_class, type)
                 and issubclass(origin_class, Field)
             },
             **cls.__sfields__,
         }
```

