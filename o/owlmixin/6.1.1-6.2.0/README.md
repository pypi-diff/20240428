# Comparing `tmp/owlmixin-6.1.1-py3-none-any.whl.zip` & `tmp/owlmixin-6.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20321 bytes, number of entries: 12
--rw-r--r--  2.0 fat    34064 b- defN 80-Jan-01 00:00 owlmixin/__init__.py
--rw-r--r--  2.0 fat     3228 b- defN 80-Jan-01 00:00 owlmixin/errors.py
--rw-r--r--  2.0 fat    26595 b- defN 80-Jan-01 00:00 owlmixin/owlcollections.py
--rw-r--r--  2.0 fat     1450 b- defN 80-Jan-01 00:00 owlmixin/owlenum.py
--rw-r--r--  2.0 fat     4413 b- defN 80-Jan-01 00:00 owlmixin/owloption.py
--rw-r--r--  2.0 fat      796 b- defN 80-Jan-01 00:00 owlmixin/samples.py
--rw-r--r--  2.0 fat    15548 b- defN 80-Jan-01 00:00 owlmixin/transformers.py
--rw-r--r--  2.0 fat     8093 b- defN 80-Jan-01 00:00 owlmixin/util.py
--rw-r--r--  2.0 fat     1071 b- defN 80-Jan-01 00:00 owlmixin-6.1.1.dist-info/LICENSE
--rw-r--r--  2.0 fat     5737 b- defN 80-Jan-01 00:00 owlmixin-6.1.1.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 owlmixin-6.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat      919 b- defN 16-Jan-01 00:00 owlmixin-6.1.1.dist-info/RECORD
-12 files, 102002 bytes uncompressed, 18809 bytes compressed:  81.6%
+Zip file size: 20386 bytes, number of entries: 12
+-rw-r--r--  2.0 unx    35066 b- defN 80-Jan-01 00:00 owlmixin/__init__.py
+-rw-r--r--  2.0 unx     3228 b- defN 80-Jan-01 00:00 owlmixin/errors.py
+-rw-r--r--  2.0 unx    26711 b- defN 80-Jan-01 00:00 owlmixin/owlcollections.py
+-rw-r--r--  2.0 unx     1443 b- defN 80-Jan-01 00:00 owlmixin/owlenum.py
+-rw-r--r--  2.0 unx     4435 b- defN 80-Jan-01 00:00 owlmixin/owloption.py
+-rw-r--r--  2.0 unx      796 b- defN 80-Jan-01 00:00 owlmixin/samples.py
+-rw-r--r--  2.0 unx    15771 b- defN 80-Jan-01 00:00 owlmixin/transformers.py
+-rw-r--r--  2.0 unx     8204 b- defN 80-Jan-01 00:00 owlmixin/util.py
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 owlmixin-6.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5777 b- defN 80-Jan-01 00:00 owlmixin-6.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 owlmixin-6.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      919 b- defN 16-Jan-01 00:00 owlmixin-6.2.0.dist-info/RECORD
+12 files, 103509 bytes uncompressed, 18874 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: owlmixin/transformers.py
 Comment: 
 
 Filename: owlmixin/util.py
 Comment: 
 
-Filename: owlmixin-6.1.1.dist-info/LICENSE
+Filename: owlmixin-6.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: owlmixin-6.1.1.dist-info/METADATA
+Filename: owlmixin-6.2.0.dist-info/METADATA
 Comment: 
 
-Filename: owlmixin-6.1.1.dist-info/WHEEL
+Filename: owlmixin-6.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: owlmixin-6.1.1.dist-info/RECORD
+Filename: owlmixin-6.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## owlmixin/__init__.py

```diff
@@ -1,25 +1,23 @@
 # coding: utf-8
 # pylint: disable=too-many-lines
 
 import inspect
 import sys
-from typing import TypeVar, Optional, Sequence, Iterable, List, Any
+from typing import Any, Iterable, List, Optional, Sequence, TypeVar
 
 from owlmixin import util
-from owlmixin.errors import RequiredError, UnknownPropertiesError, InvalidTypeError
+from owlmixin.errors import InvalidTypeError, RequiredError, UnknownPropertiesError
 from owlmixin.owlcollections import TDict, TIterator, TList
-from owlmixin.owlenum import OwlEnum, OwlObjectEnum
 from owlmixin.transformers import (
     DictTransformer,
     JsonTransformer,
-    YamlTransformer,
-    ValueTransformer,
-    traverse_dict,
     TOption,
+    ValueTransformer,
+    YamlTransformer,
 )
 
 T = TypeVar("T", bound="OwlMixin")
 
 
 def _is_generic(type_):
     return hasattr(type_, "__origin__")
@@ -34,15 +32,17 @@
 def assert_none(value, type_, cls, name):
     if value is None:
         raise RequiredError(cls=cls, prop=name, type_=type_)
 
 
 def assert_types(value, types: tuple, cls, name):
     if not isinstance(value, types):
-        raise InvalidTypeError(cls=cls, prop=name, value=value, expected=types, actual=type(value))
+        raise InvalidTypeError(
+            cls=cls, prop=name, value=value, expected=types, actual=type(value)
+        )
 
 
 def traverse(
     type_, name, value, cls, force_snake_case: bool, force_cast: bool, restrict: bool
 ) -> Any:
     # pylint: disable=too-many-return-statements,too-many-branches,too-many-arguments
     if isinstance(type_, str):
@@ -59,15 +59,18 @@
         if type_ is Any:
             return value
         if isinstance(value, type_):
             return value
         if issubclass(type_, OwlMixin):
             assert_types(value, (type_, dict), cls, name)
             return type_.from_dict(
-                value, force_snake_case=force_snake_case, force_cast=force_cast, restrict=restrict
+                value,
+                force_snake_case=force_snake_case,
+                force_cast=force_cast,
+                restrict=restrict,
             )
         if issubclass(type_, ValueTransformer):
             return type_.from_value(value)
         if force_cast:
             return type_(value)
 
         assert_types(value, (type_,), cls, name)
@@ -77,42 +80,60 @@
     g_type = type_.__args__
 
     if o_type == TList:
         assert_none(value, type_, cls, name)
         assert_types(value, (list,), cls, name)
         return TList(
             [
-                traverse(g_type[0], f"{name}.{i}", v, cls, force_snake_case, force_cast, restrict)
+                traverse(
+                    g_type[0],
+                    f"{name}.{i}",
+                    v,
+                    cls,
+                    force_snake_case,
+                    force_cast,
+                    restrict,
+                )
                 for i, v in enumerate(value)
             ]
         )
     if o_type == TIterator:
         assert_none(value, type_, cls, name)
         assert_types(value, (Iterable,), cls, name)
         return TIterator(
-            traverse(g_type[0], f"{name}.{i}", v, cls, force_snake_case, force_cast, restrict)
+            traverse(
+                g_type[0], f"{name}.{i}", v, cls, force_snake_case, force_cast, restrict
+            )
             for i, v in enumerate(value)
         )
     if o_type == TDict:
         assert_none(value, type_, cls, name)
         assert_types(value, (dict,), cls, name)
         return TDict(
             {
                 k: traverse(
-                    g_type[0], f"{name}.{k}", v, cls, force_snake_case, force_cast, restrict
+                    g_type[0],
+                    f"{name}.{k}",
+                    v,
+                    cls,
+                    force_snake_case,
+                    force_cast,
+                    restrict,
                 )
                 for k, v in value.items()
             }
         )
     if o_type == TOption:
         v = value.get() if isinstance(value, TOption) else value
         # TODO: Fot `from_csvf`... need to more simple!!
         if (isinstance(v, str) and v) or (not isinstance(v, str) and v is not None):
             return TOption(
-                traverse(g_type[0], name, v, cls, force_snake_case, force_cast, restrict)
+                traverse(
+                    g_type[0], name, v, cls, force_snake_case, force_cast, restrict
+                )
             )
         return TOption(None)
 
     raise RuntimeError(f"This generics is not supported `{o_type}`")
 
 
 class OwlMeta(type):
@@ -340,15 +361,18 @@
             <BLANKLINE>
                 * If `id` is certainly required, specify anything.
                 * If `id` is optional, change type from `<class 'int'>` to `TOption[<class 'int'>]`
             <BLANKLINE>
         """
         return TOption(
             cls.from_dict(
-                d, force_snake_case=force_snake_case, force_cast=force_cast, restrict=restrict
+                d,
+                force_snake_case=force_snake_case,
+                force_cast=force_cast,
+                restrict=restrict,
             )
             if d is not None
             else None
         )
 
     @classmethod
     def from_dicts(
@@ -378,15 +402,18 @@
             'Tom'
             >>> humans[1].name
             'John'
         """
         return TList(
             [
                 cls.from_dict(
-                    d, force_snake_case=force_snake_case, force_cast=force_cast, restrict=restrict
+                    d,
+                    force_snake_case=force_snake_case,
+                    force_cast=force_cast,
+                    restrict=restrict,
                 )
                 for d in ds
             ]
         )
 
     @classmethod
     def from_iterable_dicts(
@@ -415,15 +442,18 @@
             >>> humans.next_at(0).get().name
             'Tom'
             >>> humans.next_at(0).get().name
             'John'
         """
         return TIterator(
             cls.from_dict(
-                d, force_snake_case=force_snake_case, force_cast=force_cast, restrict=restrict
+                d,
+                force_snake_case=force_snake_case,
+                force_cast=force_cast,
+                restrict=restrict,
             )
             for d in ds
         )
 
     @classmethod
     def from_optional_dicts(
         cls,
@@ -447,15 +477,18 @@
             >>> Human.from_optional_dicts(None).is_none()
             True
             >>> Human.from_optional_dicts([]).get()
             []
         """
         return TOption(
             cls.from_dicts(
-                ds, force_snake_case=force_snake_case, force_cast=force_cast, restrict=restrict
+                ds,
+                force_snake_case=force_snake_case,
+                force_cast=force_cast,
+                restrict=restrict,
             )
             if ds is not None
             else None
         )
 
     @classmethod
     def from_optional_iterable_dicts(
@@ -480,15 +513,18 @@
             >>> Human.from_optional_dicts(None).is_none()
             True
             >>> Human.from_optional_dicts([]).get()
             []
         """
         return TOption(
             cls.from_iterable_dicts(
-                ds, force_snake_case=force_snake_case, force_cast=force_cast, restrict=restrict
+                ds,
+                force_snake_case=force_snake_case,
+                force_cast=force_cast,
+                restrict=restrict,
             )
             if ds is not None
             else None
         )
 
     @classmethod
     def from_dicts_by_key(
@@ -518,15 +554,18 @@
             'Tom'
             >>> humans_by_name['John'].name
             'John'
         """
         return TDict(
             {
                 k: cls.from_dict(
-                    v, force_snake_case=force_snake_case, force_cast=force_cast, restrict=restrict
+                    v,
+                    force_snake_case=force_snake_case,
+                    force_cast=force_cast,
+                    restrict=restrict,
                 )
                 for k, v in ds.items()
             }
         )
 
     @classmethod
     def from_optional_dicts_by_key(
@@ -551,23 +590,31 @@
             >>> Human.from_optional_dicts_by_key(None).is_none()
             True
             >>> Human.from_optional_dicts_by_key({}).get()
             {}
         """
         return TOption(
             cls.from_dicts_by_key(
-                ds, force_snake_case=force_snake_case, force_cast=force_cast, restrict=restrict
+                ds,
+                force_snake_case=force_snake_case,
+                force_cast=force_cast,
+                restrict=restrict,
             )
             if ds is not None
             else None
         )
 
     @classmethod
     def from_json(
-        cls, data: str, *, force_snake_case=True, force_cast: bool = False, restrict: bool = False
+        cls,
+        data: str,
+        *,
+        force_snake_case=True,
+        force_cast: bool = False,
+        restrict: bool = False,
     ) -> T:
         """From json string to instance
 
         :param data: Json string
         :param force_snake_case: Keys are transformed to snake case in order to compliant PEP8 if True
         :param force_cast: Cast forcibly if True
         :param restrict: Prohibit extra parameters if True
@@ -622,15 +669,20 @@
             force_snake_case=force_snake_case,
             force_cast=force_cast,
             restrict=restrict,
         )
 
     @classmethod
     def from_json_to_list(
-        cls, data: str, *, force_snake_case=True, force_cast: bool = False, restrict: bool = False
+        cls,
+        data: str,
+        *,
+        force_snake_case=True,
+        force_cast: bool = False,
+        restrict: bool = False,
     ) -> TList[T]:
         """From json string to list of instance
 
         :param data: Json string
         :param force_snake_case: Keys are transformed to snake case in order to compliant PEP8 if True
         :param force_cast: Cast forcibly if True
         :param restrict: Prohibit extra parameters if True
@@ -653,15 +705,20 @@
             force_snake_case=force_snake_case,
             force_cast=force_cast,
             restrict=restrict,
         )
 
     @classmethod
     def from_json_to_iterator(
-        cls, data: str, *, force_snake_case=True, force_cast: bool = False, restrict: bool = False
+        cls,
+        data: str,
+        *,
+        force_snake_case=True,
+        force_cast: bool = False,
+        restrict: bool = False,
     ) -> TIterator[T]:
         """From json string to iterable instance
 
         :param data: Json string
         :param force_snake_case: Keys are transformed to snake case in order to compliant PEP8 if True
         :param force_cast: Cast forcibly if True
         :param restrict: Prohibit extra parameters if True
@@ -736,15 +793,20 @@
             force_snake_case=force_snake_case,
             force_cast=force_cast,
             restrict=restrict,
         )
 
     @classmethod
     def from_yaml(
-        cls, data: str, *, force_snake_case=True, force_cast: bool = False, restrict: bool = True
+        cls,
+        data: str,
+        *,
+        force_snake_case=True,
+        force_cast: bool = False,
+        restrict: bool = True,
     ) -> T:
         """From yaml string to instance
 
         :param data: Yaml string
         :param force_snake_case: Keys are transformed to snake case in order to compliant PEP8 if True
         :param force_cast: Cast forcibly if True
         :param restrict: Prohibit extra parameters if True
@@ -801,15 +863,20 @@
             force_snake_case=force_snake_case,
             force_cast=force_cast,
             restrict=restrict,
         )
 
     @classmethod
     def from_yaml_to_list(
-        cls, data: str, *, force_snake_case=True, force_cast: bool = False, restrict: bool = True
+        cls,
+        data: str,
+        *,
+        force_snake_case=True,
+        force_cast: bool = False,
+        restrict: bool = True,
     ) -> TList[T]:
         """From yaml string to list of instance
 
         :param data: Yaml string
         :param force_snake_case: Keys are transformed to snake case in order to compliant PEP8 if True
         :param force_cast: Cast forcibly if True
         :param restrict: Prohibit extra parameters if True
@@ -840,15 +907,20 @@
             force_snake_case=force_snake_case,
             force_cast=force_cast,
             restrict=restrict,
         )
 
     @classmethod
     def from_yaml_to_iterator(
-        cls, data: str, *, force_snake_case=True, force_cast: bool = False, restrict: bool = True
+        cls,
+        data: str,
+        *,
+        force_snake_case=True,
+        force_cast: bool = False,
+        restrict: bool = True,
     ) -> TIterator[T]:
         """From yaml string to iterable instance
 
         :param data: Yaml string
         :param force_snake_case: Keys are transformed to snake case in order to compliant PEP8 if True
         :param force_cast: Cast forcibly if True
         :param restrict: Prohibit extra parameters if True
@@ -984,15 +1056,20 @@
             force_snake_case=force_snake_case,
             force_cast=True,
             restrict=restrict,
         )
 
     @classmethod
     def from_json_url(
-        cls, url: str, *, force_snake_case=True, force_cast: bool = False, restrict: bool = False
+        cls,
+        url: str,
+        *,
+        force_snake_case=True,
+        force_cast: bool = False,
+        restrict: bool = False,
     ) -> T:
         """From url which returns json to instance
 
         :param url: Url which returns json
         :param force_snake_case: Keys are transformed to snake case in order to compliant PEP8 if True
         :param force_cast: Cast forcibly if True
         :param restrict: Prohibit extra parameters if True
```

## owlmixin/errors.py

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-from typing import List, Sequence, Any
+from typing import Any, List, Sequence
 
 
 class OwlMixinError(Exception):
     title: str
 
     def __str__(self) -> str:
         return f"""
```

## owlmixin/owlcollections.py

```diff
@@ -1,22 +1,33 @@
 # coding: utf-8
 
 import functools
 from collections import deque
-from itertools import chain, islice, filterfalse, takewhile, tee, groupby
-from typing import TypeVar, Generic, Any, Callable, Dict, List, Tuple, Union, Iterable, Iterator
+from itertools import chain, filterfalse, groupby, islice, takewhile, tee
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Iterable,
+    Iterator,
+    List,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 from owlmixin.owloption import TOption
 from owlmixin.transformers import (
-    DictTransformer,
+    CsvTransformer,
     DictsTransformer,
+    DictTransformer,
     JsonTransformer,
-    YamlTransformer,
-    CsvTransformer,
     TableTransformer,
+    YamlTransformer,
 )
 
 T = TypeVar("T")
 U = TypeVar("U")
 K = TypeVar("K")
 
 
@@ -349,15 +360,20 @@
             >>> TList([1, 2, 3]).reverse()
             [3, 2, 1]
         """
         return TList(reversed(self))
 
 
 class TIterator(
-    DictsTransformer, JsonTransformer, YamlTransformer, CsvTransformer, TableTransformer, Generic[T]
+    DictsTransformer,
+    JsonTransformer,
+    YamlTransformer,
+    CsvTransformer,
+    TableTransformer,
+    Generic[T],
 ):
     __inner_iterator: Iterator
 
     def __init__(self, iterable: Iterable):
         """
         Usage:
 
@@ -565,15 +581,17 @@
                     k = func(element)
                     if k not in seen:
                         seen_add(k)
                         yield element
 
         return TIterator(make_generator())
 
-    def partition(self, func: Callable[[T], bool]) -> Tuple["TIterator[T]", "TIterator[T]"]:
+    def partition(
+        self, func: Callable[[T], bool]
+    ) -> Tuple["TIterator[T]", "TIterator[T]"]:
         """
         Usage:
 
             >>> ng, ok = TIterator([1, 2, 3, 4, 5]).partition(lambda x: x > 3)
             >>> ng.to_list()
             [1, 2, 3]
             >>> ng.to_list()
@@ -589,29 +607,33 @@
     def group_by(self, to_key: Callable[[T], str]) -> "TDict[TList[T]]":
         """
         Usage:
 
             >>> TIterator([1, 2, 3, 4, 5]).group_by(lambda x: x % 2).to_json()
             '{"0": [2,4],"1": [1,3,5]}'
         """
-        return TDict({k: TList(v) for k, v in groupby(sorted(self, key=to_key), to_key)})
+        return TDict(
+            {k: TList(v) for k, v in groupby(sorted(self, key=to_key), to_key)}
+        )
 
     def key_by(self, to_key: Callable[[T], str]) -> "TDict[T]":
         """
         :param to_key: value -> key
         Usage:
 
             >>> TIterator(['a1', 'b2', 'c3']).key_by(lambda x: x[0]).to_json()
             '{"a": "a1","b": "b2","c": "c3"}'
             >>> TIterator([1, 2, 3, 4, 5]).key_by(lambda x: x % 2).to_json()
             '{"0": 4,"1": 5}'
         """
         return TDict({to_key(x): x for x in self})
 
-    def order_by(self, func: Callable[[T], Any], reverse: bool = False) -> "TIterator[T]":
+    def order_by(
+        self, func: Callable[[T], Any], reverse: bool = False
+    ) -> "TIterator[T]":
         """
         Usage:
 
             >>> it = TIterator([12, 25, 31, 40, 57]).order_by(lambda x: x % 10)
             >>> it.to_list()
             [40, 31, 12, 25, 57]
             >>> it.to_list()
```

## owlmixin/owlenum.py

```diff
@@ -8,27 +8,26 @@
 
 T = TypeVar("T", bound="OwlObjectEnum")  # pylint: disable=invalid-name
 
 warnings.simplefilter("once")
 
 
 class OwlEnum(ValueTransformer, Enum):
-    """ This class is similar to Enum except that can dump as json or yaml
-    """
+    """This class is similar to Enum except that can dump as json or yaml"""
 
     @classmethod
     def from_value(cls, value: str):
         return cls(value)
 
     def to_value(self, ignore_none, force_value):
         return self.value
 
 
 class OwlObjectEnum(ValueTransformer, Enum):
-    """ This class is similar to OwlEnum except that can have additional object.
+    """This class is similar to OwlEnum except that can have additional object.
 
     Use case example:
         class Animal(OwlObjectEnum):
             DOG = ("dog", {"cry": "bow-wow"})
             CAT = ("cat", {"cry": "mewing"})
 
         def cry(self):
```

## owlmixin/owloption.py

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 
-from typing import Generic, TypeVar, Callable
+from typing import Callable, Generic, TypeVar
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class TOption(Generic[T]):
     def __init__(self, value):
@@ -85,15 +85,17 @@
         """
         return TOption(None) if self.is_none() else TOption(func(self.value).get())
 
     def __repr__(self):
         return f"Option --> {self.get()}"
 
     def __raise_no_conditional_expression(self, expression_name):
-        raise NotImplementedError(f"No expression `{expression_name}` in TOption instance")
+        raise NotImplementedError(
+            f"No expression `{expression_name}` in TOption instance"
+        )
 
     def __add__(self, other):
         self.__raise_no_conditional_expression("__add__")
 
     def __and__(self, other):
         self.__raise_no_conditional_expression("__and__")
```

## owlmixin/transformers.py

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-from typing import List, Sequence, Iterator, Optional, Any
+from typing import Any, Iterator, List, Optional, Sequence
 
 from owlmixin import util
 from owlmixin.owloption import TOption
 
 
 class ValueTransformer:
     def to_value(self, ignore_none, force_value):
@@ -22,23 +22,32 @@
 
 def traverse(value, ignore_none=True, force_value=False, ignore_empty=False):
     # pylint: disable=too-many-return-statements
     if force_value and isinstance(value, ValueTransformer):
         return value.to_value(ignore_none, force_value)
     if isinstance(value, TOption):
         return traverse(
-            value.get(), ignore_none=ignore_none, force_value=force_value, ignore_empty=ignore_empty
+            value.get(),
+            ignore_none=ignore_none,
+            force_value=force_value,
+            ignore_empty=ignore_empty,
         )
     if isinstance(value, dict):
         return traverse_dict(
-            value, ignore_none=ignore_none, force_value=force_value, ignore_empty=ignore_empty
+            value,
+            ignore_none=ignore_none,
+            force_value=force_value,
+            ignore_empty=ignore_empty,
         )
     if isinstance(value, list):
         return traverse_list(
-            value, ignore_none=ignore_none, force_value=force_value, ignore_empty=ignore_empty
+            value,
+            ignore_none=ignore_none,
+            force_value=force_value,
+            ignore_empty=ignore_empty,
         )
     if isinstance(value, Iterator):
         return traverse_list(list(value), ignore_none, force_value, ignore_empty)
     if isinstance(value, DictTransformer):
         return value.to_dict(
             ignore_none=ignore_none, force_value=force_value, ignore_empty=ignore_empty
         )
@@ -62,16 +71,15 @@
         traverse(i, ignore_none, force_value, ignore_empty)
         for i in instance_list
         if not (ignore_none and is_ignore(i))
     ]
 
 
 class DictTransformer:
-    """ `@property _dict` can overridden
-    """
+    """`@property _dict` can overridden"""
 
     @property
     def _dict(self):
         return self.__dict__
 
     def str_format(self, format_: str) -> str:
         """From instance to str with formatting
@@ -91,15 +99,19 @@
             ... }
             >>> Human.from_dict(human_dict).str_format('{id}: {name}')
             '1: Tom'
         """
         return format_.format(**self.to_dict())
 
     def to_dict(
-        self, *, ignore_none: bool = True, force_value: bool = True, ignore_empty: bool = False
+        self,
+        *,
+        ignore_none: bool = True,
+        force_value: bool = True,
+        ignore_empty: bool = False,
     ) -> dict:
         """From instance to dict
 
         :param ignore_none: Properties which is None are excluded if True
         :param force_value: Transform to value using to_value (default: str()) of ValueTransformer which inherited if True
         :param ignore_empty: Properties which is empty are excluded if True
         :return: Dict
@@ -143,19 +155,22 @@
             False
 
         """
         return traverse_dict(self._dict, ignore_none, force_value, ignore_empty)
 
 
 class DictsTransformer:
-    """ `@property _dict` can overridden
-    """
+    """`@property _dict` can overridden"""
 
     def to_dicts(
-        self, *, ignore_none: bool = True, force_value: bool = True, ignore_empty: bool = False
+        self,
+        *,
+        ignore_none: bool = True,
+        force_value: bool = True,
+        ignore_empty: bool = False,
     ) -> List[dict]:
         """From instance to dict
 
         :param ignore_none: Properties which is None are excluded if True
         :param force_value: Transform to value using to_value (default: str()) of ValueTransformer which inherited if True
         :param ignore_empty: Properties which is empty are excluded if True
         :return: List[Dict]
@@ -209,19 +224,22 @@
             False
 
         """
         return traverse_list(self, ignore_none, force_value, ignore_empty)
 
 
 class JsonTransformer:
-    """ `@property _dict` can overridden
-    """
+    """`@property _dict` can overridden"""
 
     def to_json(
-        self, *, indent: int = None, ignore_none: bool = True, ignore_empty: bool = False
+        self,
+        *,
+        indent: int = None,
+        ignore_none: bool = True,
+        ignore_empty: bool = False,
     ) -> str:
         """From instance to json string
 
         :param indent: Number of indentation
         :param ignore_none: Properties which is None are excluded if True
         :param ignore_empty: Properties which is empty are excluded if True
         :return: Json string
@@ -237,15 +255,16 @@
             ...         {"name": "Orange"}
             ...     ]
             ... })
             >>> human.to_json()
             '{"favorites": [{"name": "Apple","names_by_lang": {"de": "Apfel","en": "Apple"}},{"name": "Orange"}],"id": 1,"name": "Tom"}'
         """
         return util.dump_json(
-            traverse(self, ignore_none, force_value=True, ignore_empty=ignore_empty), indent
+            traverse(self, ignore_none, force_value=True, ignore_empty=ignore_empty),
+            indent,
         )
 
     def to_jsonf(
         self,
         fpath: str,
         encoding: str = "utf8",
         *,
@@ -265,15 +284,17 @@
         return util.dump_jsonf(
             traverse(self, ignore_none, force_value=True, ignore_empty=ignore_empty),
             fpath=fpath,
             encoding=encoding,
             indent=indent,
         )
 
-    def to_pretty_json(self, *, ignore_none: bool = True, ignore_empty: bool = False) -> str:
+    def to_pretty_json(
+        self, *, ignore_none: bool = True, ignore_empty: bool = False
+    ) -> str:
         """From instance to pretty json string
 
         :param ignore_none: Properties which is None are excluded if True
         :param ignore_empty: Properties which is empty are excluded if True
         :return: Json string
 
         Usage:
@@ -301,20 +322,21 @@
                         "name": "Orange"
                     }
                 ],
                 "id": 1,
                 "name": "Tom"
             }
         """
-        return self.to_json(indent=4, ignore_none=ignore_none, ignore_empty=ignore_empty)
+        return self.to_json(
+            indent=4, ignore_none=ignore_none, ignore_empty=ignore_empty
+        )
 
 
 class YamlTransformer:
-    """ `@property _dict` can overridden
-    """
+    """`@property _dict` can overridden"""
 
     def to_yaml(self, *, ignore_none: bool = True, ignore_empty: bool = False) -> str:
         """From instance to yaml string
 
         :param ignore_none: Properties which is None are excluded if True
         :param ignore_empty: Properties which is empty are excluded if True
         :return: Yaml string
@@ -365,16 +387,15 @@
             traverse(self, ignore_none, force_value=True, ignore_empty=ignore_empty),
             fpath=fpath,
             encoding=encoding,
         )
 
 
 class CsvTransformer:
-    """ `@property _dict` can overridden
-    """
+    """`@property _dict` can overridden"""
 
     def to_csv(
         self,
         fieldnames: Sequence[str],
         *,
         with_header: bool = False,
         crlf: bool = False,
@@ -443,16 +464,15 @@
             with_header=with_header,
             crlf=crlf,
             tsv=tsv,
         )
 
 
 class TableTransformer:
-    """ `@property _dict` can overridden
-    """
+    """`@property _dict` can overridden"""
 
     def to_table(self, fieldnames: Sequence[str]) -> str:
         """From sequence of text to csv string
 
         :param fieldnames: Order of columns by property name
         :return: Table string
```

## owlmixin/util.py

```diff
@@ -4,20 +4,20 @@
 # pylint: disable=wrong-import-order,duplicate-code
 
 import codecs
 import csv
 import io
 import json
 import re
-from math import floor, ceil
-from typing import List, Dict, Union, Sequence, Iterable, Iterator, Optional
+from math import ceil, floor
+from typing import Dict, Iterable, Iterator, List, Optional, Sequence, Union
+from unicodedata import east_asian_width
 from urllib.request import urlopen
 
 import yaml
-from unicodedata import east_asian_width
 
 
 class CrLfCsvDialect(csv.Dialect):
     delimiter = ","
     quotechar = '"'
     doublequote = True
     skipinitialspace = True
@@ -92,15 +92,17 @@
 
 def to_snake(value):
     """For key of dictionary
 
     :param unicode value:
     :rtype: unicode
     """
-    return re.sub(r"((?<!^)[A-Z])", "_\\1", value.strip("<>-")).lower().replace("-", "_")
+    return (
+        re.sub(r"((?<!^)[A-Z])", "_\\1", value.strip("<>-")).lower().replace("-", "_")
+    )
 
 
 def load_json(json_str):
     """
     :param unicode json_str:
     :rtype: dict | list
     """
@@ -131,15 +133,17 @@
     :param unicode encoding:
     :rtype: dict | list
     """
     with codecs.open(fpath, encoding=encoding) as f:
         return yaml.safe_load(f)
 
 
-def load_csvf(fpath: str, fieldnames: Optional[Sequence[str]], encoding: str) -> Iterator[dict]:
+def load_csvf(
+    fpath: str, fieldnames: Optional[Sequence[str]], encoding: str
+) -> Iterator[dict]:
     """
     :param fpath:
     :param fieldnames:
     :param encoding:
     :return Iterator of dict:
     """
     with open(fpath, mode="r", encoding=encoding) as f:
@@ -180,15 +184,17 @@
 
     def force_str(v):
         # XXX: Double quotation behaves strangely... so replace (why?)
         return dump_json(v).replace('"', "'") if isinstance(v, (dict, list)) else v
 
     with io.StringIO() as sio:
         dialect = get_dialect_name(crlf, tsv)
-        writer = csv.DictWriter(sio, fieldnames=fieldnames, dialect=dialect, extrasaction="ignore")
+        writer = csv.DictWriter(
+            sio, fieldnames=fieldnames, dialect=dialect, extrasaction="ignore"
+        )
         if with_header:
             writer.writeheader()
         for x in data:
             writer.writerow({k: force_str(v) for k, v in x.items()})
         sio.seek(0)
         return sio.read()
 
@@ -216,15 +222,17 @@
 
     def force_str(v):
         # XXX: Double quotation behaves strangely... so replace (why?)
         return dump_json(v).replace('"', "'") if isinstance(v, (dict, list)) else v
 
     with codecs.open(fpath, mode="w", encoding=encoding) as f:
         dialect = get_dialect_name(crlf, tsv)
-        writer = csv.DictWriter(f, fieldnames=fieldnames, dialect=dialect, extrasaction="ignore")
+        writer = csv.DictWriter(
+            f, fieldnames=fieldnames, dialect=dialect, extrasaction="ignore"
+        )
         if with_header:
             writer.writeheader()
         for x in data:
             writer.writerow({k: force_str(v) for k, v in x.items()})
 
     return fpath
 
@@ -236,15 +244,17 @@
     :rtype: unicode
     """
     return json.dumps(
         data, indent=indent, ensure_ascii=False, sort_keys=True, separators=(",", ": ")
     )
 
 
-def dump_jsonf(data: Union[list, dict], *, fpath: str, encoding: str, indent=None) -> str:
+def dump_jsonf(
+    data: Union[list, dict], *, fpath: str, encoding: str, indent=None
+) -> str:
     """
     :param data: list | dict data
     :param fpath: write path
     :param encoding: encoding
     :param indent:
     :rtype: written path
     """
@@ -255,15 +265,20 @@
 
 def dump_yaml(data):
     """
     :param list | dict data:
     :rtype: unicode
     """
     return yaml.dump(
-        data, indent=2, encoding=None, allow_unicode=True, default_flow_style=False, Dumper=MyDumper
+        data,
+        indent=2,
+        encoding=None,
+        allow_unicode=True,
+        default_flow_style=False,
+        Dumper=MyDumper,
     )
 
 
 def dump_yamlf(data: Union[list, dict], *, fpath: str, encoding: str) -> str:
     """
     :param data: list | dict data
     :param fpath: write path
@@ -287,15 +302,15 @@
 
     width_by_col: Dict[str, int] = {
         f: min3(max([string_width(str(d.get(f))) for d in data] + [string_width(f)]))
         for f in fieldnames
     }
 
     def fill_spaces(word: str, width: int, center=False):
-        """ aaa, 4 => ' aaa  ' """
+        """aaa, 4 => ' aaa  '"""
         to_fills: int = width - string_width(word)
         return (
             f" {' ' * floor(to_fills / 2)}{word}{' ' * ceil(to_fills / 2)} "
             if center
             else f" {word}{' ' * to_fills} "
         )
```

## Comparing `owlmixin-6.1.1.dist-info/LICENSE` & `owlmixin-6.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `owlmixin-6.1.1.dist-info/METADATA` & `owlmixin-6.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: owlmixin
-Version: 6.1.1
+Version: 6.2.0
 Summary: Mixin which converts ``data class instance`` and others each other more simple.
 Home-page: https://github.com/tadashi-aikawa/owlmixin
 License: MIT
 Keywords: dict,json,yaml,parser,mixin
 Author: tadashi-aikawa
 Author-email: syou.maman@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Documentation, https://tadashi-aikawa.github.io/owlmixin/
 Project-URL: Repository, https://github.com/tadashi-aikawa/owlmixin
 Description-Content-Type: text/markdown
 
@@ -209,15 +209,16 @@
 1. Development on master and if you need branches and issues, create them
 2. Commit with prefix emoji such as "📝", and suffix issue number like "#120"
 
 ### Commands
 
 ```bash
 # Create env
-$ make init-dev
+$ poetry env use <path of python 3.8>
+$ poetry install
 
 # Build documentation and run server locally
 $ make serve-docs
 
 # Test (Doc test & Unit test)
 $ make test
 ```
```

