# Comparing `tmp/aiocsv-1.3.1.tar.gz` & `tmp/aiocsv-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocsv-1.3.1.tar", last modified: Tue Feb 27 17:18:11 2024, max compression
+gzip compressed data, was "aiocsv-1.3.2.tar", last modified: Sun Apr 28 10:30:03 2024, max compression
```

## Comparing `aiocsv-1.3.1.tar` & `aiocsv-1.3.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2024-02-27 17:18:11.286908 aiocsv-1.3.1/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1065 2024-02-21 11:42:01.000000 aiocsv-1.3.1/LICENSE
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7384 2024-02-27 17:18:11.283574 aiocsv-1.3.1/PKG-INFO
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2024-02-27 17:18:11.280241 aiocsv-1.3.1/aiocsv/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      697 2024-02-27 17:17:50.000000 aiocsv-1.3.1/aiocsv/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    32263 2024-02-27 14:39:22.000000 aiocsv-1.3.1/aiocsv/_parser.c
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      505 2024-02-21 18:10:22.000000 aiocsv-1.3.1/aiocsv/_parser.pyi
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10640 2024-02-27 14:17:45.000000 aiocsv-1.3.1/aiocsv/parser.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      477 2024-02-21 18:10:39.000000 aiocsv-1.3.1/aiocsv/protocols.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        0 2023-11-07 09:57:21.000000 aiocsv-1.3.1/aiocsv/py.typed
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3664 2024-02-21 18:10:47.000000 aiocsv-1.3.1/aiocsv/readers.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3662 2024-02-21 18:11:15.000000 aiocsv-1.3.1/aiocsv/writers.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2024-02-27 17:18:11.283574 aiocsv-1.3.1/aiocsv.egg-info/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7384 2024-02-27 17:18:11.000000 aiocsv-1.3.1/aiocsv.egg-info/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      441 2024-02-27 17:18:11.000000 aiocsv-1.3.1/aiocsv.egg-info/SOURCES.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2024-02-27 17:18:11.000000 aiocsv-1.3.1/aiocsv.egg-info/dependency_links.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2024-02-21 17:56:51.000000 aiocsv-1.3.1/aiocsv.egg-info/not-zip-safe
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        7 2024-02-27 17:18:11.000000 aiocsv-1.3.1/aiocsv.egg-info/top_level.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      777 2024-02-21 18:07:57.000000 aiocsv-1.3.1/pyproject.toml
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6885 2024-02-21 11:50:38.000000 aiocsv-1.3.1/readme.md
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2024-02-27 17:18:11.286908 aiocsv-1.3.1/setup.cfg
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      126 2024-02-21 11:42:01.000000 aiocsv-1.3.1/setup.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2024-02-27 17:18:11.283574 aiocsv-1.3.1/tests/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1431 2023-11-07 09:57:21.000000 aiocsv-1.3.1/tests/test_dialects.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2407 2024-02-21 11:42:01.000000 aiocsv-1.3.1/tests/test_dict.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1048 2024-02-19 19:15:23.000000 aiocsv-1.3.1/tests/test_newlines.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11973 2024-02-27 14:13:59.000000 aiocsv-1.3.1/tests/test_parser.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1699 2024-02-21 11:42:01.000000 aiocsv-1.3.1/tests/test_simple.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2024-04-28 10:30:03.977237 aiocsv-1.3.2/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1065 2024-02-21 11:42:01.000000 aiocsv-1.3.2/LICENSE
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    12892 2024-04-28 10:30:03.973903 aiocsv-1.3.2/PKG-INFO
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2024-04-28 10:30:03.973903 aiocsv-1.3.2/aiocsv/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      569 2024-04-28 10:29:16.000000 aiocsv-1.3.2/aiocsv/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    32290 2024-04-28 09:00:26.000000 aiocsv-1.3.2/aiocsv/_parser.c
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      503 2024-04-28 09:00:24.000000 aiocsv-1.3.2/aiocsv/_parser.pyi
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10619 2024-04-28 09:00:23.000000 aiocsv-1.3.2/aiocsv/parser.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      984 2024-04-28 09:23:10.000000 aiocsv-1.3.2/aiocsv/protocols.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        0 2023-11-07 09:57:21.000000 aiocsv-1.3.2/aiocsv/py.typed
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4015 2024-04-28 09:33:00.000000 aiocsv-1.3.2/aiocsv/readers.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3921 2024-04-28 10:08:29.000000 aiocsv-1.3.2/aiocsv/writers.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2024-04-28 10:30:03.973903 aiocsv-1.3.2/aiocsv.egg-info/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    12892 2024-04-28 10:30:03.000000 aiocsv-1.3.2/aiocsv.egg-info/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      470 2024-04-28 10:30:03.000000 aiocsv-1.3.2/aiocsv.egg-info/SOURCES.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2024-04-28 10:30:03.000000 aiocsv-1.3.2/aiocsv.egg-info/dependency_links.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2024-02-21 17:56:51.000000 aiocsv-1.3.2/aiocsv.egg-info/not-zip-safe
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       18 2024-04-28 10:30:03.000000 aiocsv-1.3.2/aiocsv.egg-info/requires.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        7 2024-04-28 10:30:03.000000 aiocsv-1.3.2/aiocsv.egg-info/top_level.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      944 2024-04-28 09:11:14.000000 aiocsv-1.3.2/pyproject.toml
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    12360 2024-04-28 10:17:01.000000 aiocsv-1.3.2/readme.md
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2024-04-28 10:30:03.977237 aiocsv-1.3.2/setup.cfg
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      125 2024-04-28 09:07:21.000000 aiocsv-1.3.2/setup.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2024-04-28 10:30:03.973903 aiocsv-1.3.2/tests/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1434 2024-04-28 10:21:31.000000 aiocsv-1.3.2/tests/test_dialects.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2550 2024-04-28 10:22:16.000000 aiocsv-1.3.2/tests/test_dict.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1113 2024-04-28 10:22:24.000000 aiocsv-1.3.2/tests/test_newlines.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    12422 2024-04-28 10:28:06.000000 aiocsv-1.3.2/tests/test_parser.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1682 2024-04-28 09:07:03.000000 aiocsv-1.3.2/tests/test_simple.py
```

### Comparing `aiocsv-1.3.1/LICENSE` & `aiocsv-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocsv-1.3.1/aiocsv/_parser.c` & `aiocsv-1.3.2/aiocsv/_parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -792,14 +792,15 @@
         record = Parser_try_parse(self);
         if (PyErr_Occurred()) return NULL;
     }
 
     // Generate a row or stop iteration altogether
     if (record) {
         PyErr_SetObject(PyExc_StopIteration, record);
+        Py_DECREF(record);
     } else {
         PyErr_SetNone(PyExc_StopAsyncIteration);
     }
     return NULL;
 }
 
 // *** Type Specification ***
```

### Comparing `aiocsv-1.3.1/aiocsv/parser.py` & `aiocsv-1.3.2/aiocsv/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # © Copyright 2020-2024 Mikołaj Kuranowski
 # SPDX-License-Identifier: MIT
 
+import csv
 from enum import IntEnum, auto
 from typing import Any, AsyncIterator, Awaitable, Generator, List, Optional, Sequence, Union
-import csv
 
 from .protocols import DialectLike, WithAsyncRead
 
 
 class ParserState(IntEnum):
     START_RECORD = auto()
     START_FIELD = auto()
@@ -213,15 +213,15 @@
         self.add_char(c)
         self.state = ParserState.IN_QUOTED_FIELD
         return Decision.CONTINUE
 
     def process_char_in_quote_in_quoted(self, c: str) -> Decision:
         if c == self.dialect.quotechar and self.dialect.quoting != QUOTE_NONE:
             # XXX: Is this check for quoting necessary?
-            self.add_char(c)  # type: ignore | wtf
+            self.add_char(c)
             self.state = ParserState.IN_QUOTED_FIELD
         elif c == self.dialect.delimiter:
             self.save_field()
             self.state = ParserState.START_FIELD
         elif c == "\r":
             self.save_field()
             self.state = ParserState.EAT_NEWLINE
@@ -246,15 +246,15 @@
         if len(self.field_so_far) == self.field_limit:
             raise csv.Error(f"field larger than field limit ({self.field_limit})")
         self.field_so_far.append(c)
 
     def save_field(self) -> None:
         field: Union[str, float, None]
         if self.dialect.skipinitialspace:
-            field = "".join(self.field_so_far[self.find_first_non_space(self.field_so_far):])
+            field = "".join(self.field_so_far[self.find_first_non_space(self.field_so_far) :])
         else:
             field = "".join(self.field_so_far)
 
         # Convert to float if QUOTE_NONNUMERIC
         if self.dialect.quoting == QUOTE_NONNUMERIC and field and self.field_was_numeric:
             self.field_was_numeric = False
             field = float(field)
```

### Comparing `aiocsv-1.3.1/aiocsv/readers.py` & `aiocsv-1.3.2/aiocsv/readers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 # © Copyright 2020-2024 Mikołaj Kuranowski
 # SPDX-License-Identifier: MIT
 
+# cSpell: words asyncfile restkey restval
+
 import csv
-from warnings import warn
 from typing import Dict, List, Optional, Sequence
-from .protocols import WithAsyncRead
+from warnings import warn
+
+from typing_extensions import Unpack
+
+from .protocols import CsvDialectArg, CsvDialectKwargs, WithAsyncRead
 
 try:
     from ._parser import Parser
 except ImportError:
     warn("using slow, pure-Python parser")
     from .parser import Parser
 
 
 class AsyncReader:
     """An object that iterates over lines in given asynchronous file.
     Additional keyword arguments are passed to the underlying csv.reader instance.
     Iterating over this object returns parsed CSV rows (List[str]).
     """
-    def __init__(self, asyncfile: WithAsyncRead, **csvreaderparams) -> None:
+
+    def __init__(
+        self,
+        asyncfile: WithAsyncRead,
+        dialect: CsvDialectArg = "excel",
+        **csv_dialect_kwargs: Unpack[CsvDialectKwargs],
+    ) -> None:
         self._file = asyncfile
 
         # csv.Dialect isn't a class, instead it's a weird proxy
         # (at least in CPython) to _csv.Dialect. Instead of figuring how
         # this shit works, just let `csv` figure the dialects out.
-        self._dialect = csv.reader("", **csvreaderparams).dialect
+        self._dialect = csv.reader("", dialect=dialect, **csv_dialect_kwargs).dialect
 
         self._parser = Parser(self._file, self._dialect)
 
     @property
     def dialect(self) -> csv.Dialect:
         return self._dialect
 
@@ -46,22 +57,29 @@
 class AsyncDictReader:
     """An object that iterates over lines in given asynchronous file.
     Additional keyword arguments are passed to the underlying csv.DictReader instance.
     If given csv file has no header, provide a 'fieldnames' keyword argument,
     like you would to csv.DictReader.
     Iterating over this object returns parsed CSV rows (Dict[str, str]).
     """
-    def __init__(self, asyncfile: WithAsyncRead, fieldnames: Optional[Sequence[str]] = None,
-                 restkey: Optional[str] = None, restval: Optional[str] = None,
-                 **csvreaderparams) -> None:
+
+    def __init__(
+        self,
+        asyncfile: WithAsyncRead,
+        fieldnames: Optional[Sequence[str]] = None,
+        restkey: Optional[str] = None,
+        restval: Optional[str] = None,
+        dialect: CsvDialectArg = "excel",
+        **csv_dialect_kwargs: Unpack[CsvDialectKwargs],
+    ) -> None:
 
         self.fieldnames: Optional[List[str]] = list(fieldnames) if fieldnames else None
         self.restkey: Optional[str] = restkey
         self.restval: Optional[str] = restval
-        self.reader = AsyncReader(asyncfile, **csvreaderparams)
+        self.reader = AsyncReader(asyncfile, dialect=dialect, **csv_dialect_kwargs)
 
     @property
     def dialect(self) -> csv.Dialect:
         return self.reader.dialect
 
     @property
     def line_num(self) -> int:
```

### Comparing `aiocsv-1.3.1/tests/test_dialects.py` & `aiocsv-1.3.2/tests/test_dialects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,43 @@
+import os
 from tempfile import NamedTemporaryFile
+
 import aiofiles
 import pytest
-import os
 
 from aiocsv import AsyncReader, AsyncWriter
 
 FILENAME = "tests/eu_cities_unix.csv"
-PARAMS = {"dialect": "unix"}
+DIALECT = "unix"
 VALUES = [
     ["Berlin", "Germany"],
     ["Madrid", "Spain"],
     ["Rome", "Italy"],
     ["Bucharest", "Romania"],
     ["Paris", "France"],
 ]
 
 
 @pytest.mark.asyncio
 async def test_dialect_read():
     async with aiofiles.open(FILENAME, mode="r", encoding="ascii", newline="") as afp:
-        read_rows = [i async for i in AsyncReader(afp, **PARAMS)]
+        read_rows = [i async for i in AsyncReader(afp, dialect=DIALECT)]
         assert read_rows == VALUES
 
 
 @pytest.mark.asyncio
 async def test_dialect_write():
     # Create a TempFile to direct writer to
     with NamedTemporaryFile(mode="w+", suffix=".csv", delete=False) as tf:
         target_name = tf.name
 
     try:
         # Write rows
         async with aiofiles.open(target_name, mode="w", encoding="ascii", newline="") as afp:
-            writer = AsyncWriter(afp, **PARAMS)
+            writer = AsyncWriter(afp, dialect=DIALECT)
             await writer.writerow(VALUES[0])
             await writer.writerows(VALUES[1:])
 
         # Read original and created files
         with open(target_name, mode="r", encoding="ascii") as created_f:
             created = created_f.read()
```

### Comparing `aiocsv-1.3.1/tests/test_dict.py` & `aiocsv-1.3.2/tests/test_dict.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,52 @@
+import csv
+import os
 from tempfile import NamedTemporaryFile
+
 import aiofiles
 import pytest
-import csv
-import os
 
 from aiocsv import AsyncDictReader, AsyncDictWriter
+from aiocsv.protocols import CsvDialectKwargs
 
 FILENAME = "tests/metro_systems.tsv"
-PARAMS = {"delimiter": "\t", "quotechar": "'", "quoting": csv.QUOTE_ALL}
+DIALECT_PARAMS: CsvDialectKwargs = {"delimiter": "\t", "quotechar": "'", "quoting": csv.QUOTE_ALL}
 HEADER = ["City", "Stations", "System Length"]
-VALUES = [dict(zip(HEADER, i)) for i in [
-    ["New York", "424", "380"],
-    ["Shanghai", "345", "676"],
-    ["Seoul", "331", "353"],
-    ["Beijing", "326", "690"],
-    ["Paris", "302", "214"],
-    ["London", "270", "402"],
-]]
+VALUES = [
+    dict(zip(HEADER, i))
+    for i in [
+        ["New York", "424", "380"],
+        ["Shanghai", "345", "676"],
+        ["Seoul", "331", "353"],
+        ["Beijing", "326", "690"],
+        ["Paris", "302", "214"],
+        ["London", "270", "402"],
+    ]
+]
 
 
 @pytest.mark.asyncio
 async def test_dict_read():
     async with aiofiles.open(FILENAME, mode="r", encoding="ascii", newline="") as afp:
-        read_rows = [i async for i in AsyncDictReader(afp, **PARAMS)]
+        read_rows = [i async for i in AsyncDictReader(afp, **DIALECT_PARAMS)]
         assert read_rows == VALUES
 
 
 @pytest.mark.asyncio
 async def test_dict_read_line_nums():
     async with aiofiles.open(FILENAME, mode="r", encoding="ascii", newline="") as afp:
-        r = AsyncDictReader(afp, **PARAMS)
+        r = AsyncDictReader(afp, **DIALECT_PARAMS)
         read_rows = [(row, r.line_num) async for row in r]
         assert read_rows == [(row, i) for i, row in enumerate(VALUES, start=2)]
 
 
 @pytest.mark.asyncio
 async def test_dict_read_get_fieldnames():
     async with aiofiles.open(FILENAME, mode="r", encoding="ascii", newline="") as afp:
-        reader = AsyncDictReader(afp, **PARAMS)
+        reader = AsyncDictReader(afp, **DIALECT_PARAMS)
 
         assert reader.fieldnames is None
         assert await reader.get_fieldnames() == ["City", "Stations", "System Length"]
         assert reader.fieldnames == ["City", "Stations", "System Length"]
 
 
 @pytest.mark.asyncio
@@ -49,15 +54,15 @@
     # Create a TempFile to direct writer to
     with NamedTemporaryFile(mode="w+", suffix=".csv", delete=False) as tf:
         target_name = tf.name
 
     try:
         # Write rows
         async with aiofiles.open(target_name, mode="w", encoding="ascii", newline="") as afp:
-            writer = AsyncDictWriter(afp, HEADER, **PARAMS)
+            writer = AsyncDictWriter(afp, HEADER, **DIALECT_PARAMS)
             await writer.writeheader()
             await writer.writerow(VALUES[0])
             await writer.writerows(VALUES[1:])
 
         # Read original and created files
         with open(target_name, mode="r", encoding="ascii") as created_f:
             created = created_f.read()
```

### Comparing `aiocsv-1.3.1/tests/test_parser.py` & `aiocsv-1.3.2/tests/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import AsyncIterator, Callable, List, Protocol, Type
-import pytest
 import csv
 import io
+from typing import AsyncIterator, Callable, List, Protocol, Type
+
+import pytest
 
-from aiocsv.parser import Parser as PyParser
 from aiocsv._parser import Parser as CParser
-from aiocsv.protocols import WithAsyncRead, DialectLike
+from aiocsv.parser import Parser as PyParser
+from aiocsv.protocols import DialectLike, WithAsyncRead
 
 
 class Parser(Protocol):
     def __aiter__(self) -> AsyncIterator[List[str]]: ...
     @property
     def line_num(self) -> int: ...
 
@@ -34,15 +35,15 @@
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_simple(parser: Type[Parser]):
     data = 'abc,"def",ghi\r\n' '"j""k""l",mno,pqr\r\n' 'stu,vwx,"yz"\r\n'
 
     csv_result = list(csv.reader(io.StringIO(data, newline="")))
     custom_result = [
-        r async for r in parser(AsyncStringIO(data), csv.get_dialect("excel"))
+        r async for r in parser(AsyncStringIO(data), csv.get_dialect("excel"))  # type: ignore
     ]
 
     assert csv_result == custom_result
     assert custom_result == [
         ["abc", "def", "ghi"],
         ['j"k"l', "mno", "pqr"],
         ["stu", "vwx", "yz"],
@@ -51,45 +52,49 @@
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_escapes(parser: Type[Parser]):
     data = 'ab$"c,de$\nf\r\n' '"$"",$$gh$"\r\n' '"i\nj",k$,\r\n'
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$", strict=True)
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
 
     assert csv_result == custom_result
     assert custom_result == [['ab"c', "de\nf"], ['"', '$gh"'], ["i\nj", "k,"]]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_empty(parser: Type[Parser]):
     data = "\r\n  a,,\r\n,\r\n  "
 
-    csv_parser = csv.reader(
-        io.StringIO(data, newline=""), skipinitialspace=True, strict=True
-    )
+    csv_parser = csv.reader(io.StringIO(data, newline=""), skipinitialspace=True, strict=True)
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
 
     assert csv_result == custom_result
     assert custom_result == [[], ["a", "", ""], ["", ""], [""]]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_nonnumeric(parser: Type[Parser]):
     data = '1,2\n"a",,3.14'
 
     csv_parser = csv.reader(
         io.StringIO(data, newline=""), quoting=csv.QUOTE_NONNUMERIC, strict=True
     )
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
 
     assert csv_result == custom_result
     assert custom_result == [[1.0, 2.0], ["a", "", 3.14]]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
@@ -100,40 +105,42 @@
         io.StringIO(data, newline=""), quoting=csv.QUOTE_NONNUMERIC, strict=True
     )
 
     with pytest.raises(ValueError):
         list(csv_parser)
 
     with pytest.raises(ValueError):
-        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]  # type: ignore
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_none_quoting(parser: Type[Parser]):
     data = '1" hello,"2\na","3.14"'
 
-    csv_parser = csv.reader(
-        io.StringIO(data, newline=""), quoting=csv.QUOTE_NONE, strict=True
-    )
+    csv_parser = csv.reader(io.StringIO(data, newline=""), quoting=csv.QUOTE_NONE, strict=True)
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
 
     assert csv_result == custom_result
     assert custom_result == [['1" hello', '"2'], ['a"', '"3.14"']]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_weird_quotes(parser: Type[Parser]):
     data = 'a"b,$"cd"\r\n' '"ef"g",\r\n' '"$"""","e"$f"\r\n'
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$", strict=False)
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
 
     assert csv_result == custom_result
     assert custom_result == [['a"b', '"cd"'], ['efg"', ""], ['""', 'e$f"']]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
@@ -142,100 +149,110 @@
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), strict=True)
 
     with pytest.raises(csv.Error, match="',' expected after '\"'"):
         list(csv_parser)
 
     with pytest.raises(csv.Error, match="',' expected after '\"'"):
-        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]  # type: ignore
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_weird_quotes_nonnumeric(parser: Type[Parser]):
     data = '3.0,\r\n"1."5,"15"\r\n$2,"-4".5\r\n-5$.2,-11'
 
     csv_parser = csv.reader(
         io.StringIO(data, newline=""),
         quoting=csv.QUOTE_NONNUMERIC,
         escapechar="$",
         strict=False,
     )
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
 
     assert csv_result == custom_result
     assert custom_result == [[3.0, ""], ["1.5", "15"], ["2", "-4.5"], [-5.2, -11.0]]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_escape_after_quote_in_quoted(parser: Type[Parser]):
     data = '"fo"$o\r\n'
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$")
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
     expected_result = [["fo$o"]]
 
     assert csv_result == expected_result
     assert custom_result == expected_result
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_escaped_crlf(parser: Type[Parser]):
     data = "foo$\r\nbar\r\n"
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$")
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
     expected_result = [["foo\r"], ["bar"]]
 
     assert csv_result == expected_result
     assert custom_result == expected_result
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_escaped_crlf_in_quoted(parser: Type[Parser]):
     data = '"foo$\r\n",bar\r\n'
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$")
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
     expected_result = [["foo\r\n", "bar"]]
 
     assert csv_result == expected_result
     assert custom_result == expected_result
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_consecutive_newlines(parser: Type[Parser]):
     data = "foo\r\rbar\n\rbaz\n\nspam\r\n\neggs"
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$")
     csv_result = list(csv_parser)
-    custom_result = [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+    custom_result = [
+        r async for r in parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
+    ]
     expected_result = [["foo"], [], ["bar"], [], ["baz"], [], ["spam"], [], ["eggs"]]
 
     assert csv_result == expected_result
     assert custom_result == expected_result
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_line_num(parser: Type[Parser]):
     data = 'foo,bar,baz\r\nspam,"egg\reggs",milk\r\n'
 
     csv_parser = csv.reader(io.StringIO(data, newline=""))
     csv_result = [(csv_parser.line_num, line) for line in csv_parser]
 
-    custom_parser = parser(AsyncStringIO(data), csv_parser.dialect)
+    custom_parser = parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
     custom_result = [(custom_parser.line_num, line) async for line in custom_parser]
 
     expected_result = [
         (1, ["foo", "bar", "baz"]),
         (3, ["spam", "egg\reggs", "milk"]),
     ]
 
@@ -252,71 +269,71 @@
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), strict=True)
 
     with pytest.raises(csv.Error, match=r"field larger than field limit \(64\)"):
         list(csv_parser)
 
     with pytest.raises(csv.Error, match=r"field larger than field limit \(64\)"):
-        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]  # type: ignore
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_unterminated_quote(parser: Type[Parser]):
     data = '"abc\r\n'
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), strict=True)
 
     with pytest.raises(csv.Error, match=r"unexpected end of data"):
         list(csv_parser)
 
     with pytest.raises(csv.Error, match=r"unexpected end of data"):
-        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]  # type: ignore
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_unterminated_quote_non_strict(parser: Type[Parser]):
     data = '"abc\r\n'
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), strict=False)
     csv_result = list(csv_parser)
 
-    custom_parser = parser(AsyncStringIO(data), csv_parser.dialect)
+    custom_parser = parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
     custom_result = [line async for line in custom_parser]
 
     expected_result = [["abc\r\n"]]
 
     assert csv_result == expected_result
     assert custom_result == expected_result
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_eof_in_escape(parser: Type[Parser]):
-    data = 'a$'
+    data = "a$"
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$", strict=True)
 
     with pytest.raises(csv.Error, match=r"unexpected end of data"):
         list(csv_parser)
 
     with pytest.raises(csv.Error, match=r"unexpected end of data"):
-        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]  # type: ignore
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_eof_in_escape_non_strict(parser: Type[Parser]):
-    data = 'a$'
+    data = "a$"
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$", strict=False)
     csv_result = list(csv_parser)
 
-    custom_parser = parser(AsyncStringIO(data), csv_parser.dialect)
+    custom_parser = parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
     custom_result = [line async for line in custom_parser]
 
     expected_result = [["a\n"]]
 
     assert csv_result == expected_result
     assert custom_result == expected_result
 
@@ -328,25 +345,25 @@
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$", strict=True)
 
     with pytest.raises(csv.Error, match=r"unexpected end of data"):
         list(csv_parser)
 
     with pytest.raises(csv.Error, match=r"unexpected end of data"):
-        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]
+        [r async for r in parser(AsyncStringIO(data), csv_parser.dialect)]  # type: ignore
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("parser", PARSERS, ids=PARSER_NAMES)
 async def test_parsing_eof_in_quoted_escape_non_strict(parser: Type[Parser]):
     data = '"a$'
 
     csv_parser = csv.reader(io.StringIO(data, newline=""), escapechar="$", strict=False)
     csv_result = list(csv_parser)
 
-    custom_parser = parser(AsyncStringIO(data), csv_parser.dialect)
+    custom_parser = parser(AsyncStringIO(data), csv_parser.dialect)  # type: ignore
     custom_result = [line async for line in custom_parser]
 
     expected_result = [["a\n"]]
 
     assert csv_result == expected_result
     assert custom_result == expected_result
```

### Comparing `aiocsv-1.3.1/tests/test_simple.py` & `aiocsv-1.3.2/tests/test_simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,18 @@
+import os
 from tempfile import NamedTemporaryFile
+
 import aiofiles
 import pytest
-import os
 
 from aiocsv import AsyncReader, AsyncWriter
 
 FILENAME = "tests/math_constants.csv"
 HEADER = ["name", "value"]
-VALUES = [
-    ["pi", "3.1416"],
-    ["sqrt2", "1.4142"],
-    ["phi", "1.618"],
-    ["e", "2.7183"]
-]
+VALUES = [["pi", "3.1416"], ["sqrt2", "1.4142"], ["phi", "1.618"], ["e", "2.7183"]]
 
 
 @pytest.mark.asyncio
 async def test_simple_read():
     async with aiofiles.open(FILENAME, mode="r", encoding="ascii", newline="") as af:
         read_rows = [i async for i in AsyncReader(af)]
         assert read_rows == VALUES
```

