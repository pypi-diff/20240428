# Comparing `tmp/thread-2.0.0.tar.gz` & `tmp/thread-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thread-2.0.0.tar", max compression
+gzip compressed data, was "thread-2.0.1.tar", max compression
```

## Comparing `thread-2.0.0.tar` & `thread-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1496 2024-04-21 04:10:29.955723 thread-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     5329 2024-04-21 04:10:29.955723 thread-2.0.0/README.md
--rw-r--r--   0        0        0     1625 2024-04-21 04:10:29.955723 thread-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      657 2024-04-21 04:10:29.955723 thread-2.0.0/src/thread/__init__.py
--rw-r--r--   0        0        0      139 2024-04-21 04:10:29.955723 thread-2.0.0/src/thread/__main__.py
--rw-r--r--   0        0        0     1522 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/_types.py
--rw-r--r--   0        0        0      272 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/cli.py
--rw-r--r--   0        0        0       93 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/decorators/__init__.py
--rw-r--r--   0        0        0     4846 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/decorators/_processor.py
--rw-r--r--   0        0        0     3889 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/decorators/_threaded.py
--rw-r--r--   0        0        0     2196 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/py.typed
--rw-r--r--   0        0        0    22008 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/thread.py
--rw-r--r--   0        0        0      123 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/utils/__init__.py
--rw-r--r--   0        0        0     1381 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/utils/algorithm.py
--rw-r--r--   0        0        0     4527 2024-04-21 04:10:29.959723 thread-2.0.0/src/thread/utils/config.py
--rw-r--r--   0        0        0       50 2024-04-21 04:10:29.959723 thread-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0       65 2024-04-21 04:10:29.959723 thread-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1144 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_algorithm.py
--rw-r--r--   0        0        0     1820 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_concurrentprocessing.py
--rw-r--r--   0        0        0     9471 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_dataframe_compatibility.py
--rw-r--r--   0        0        0     2118 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_decorator.py
--rw-r--r--   0        0        0     3409 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_thread.py
--rw-r--r--   0        0        0     1484 2024-04-21 04:10:29.959723 thread-2.0.0/tests/test_verbosity.py
--rw-r--r--   0        0        0     6715 1970-01-01 00:00:00.000000 thread-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-04-28 08:08:00.664454 thread-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4657 2024-04-28 08:08:00.664454 thread-2.0.1/README.md
+-rw-r--r--   0        0        0     1625 2024-04-28 08:08:00.664454 thread-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      657 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/__main__.py
+-rw-r--r--   0        0        0     1522 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/_types.py
+-rw-r--r--   0        0        0      272 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/cli.py
+-rw-r--r--   0        0        0       93 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/decorators/__init__.py
+-rw-r--r--   0        0        0     4846 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/decorators/_processor.py
+-rw-r--r--   0        0        0     3889 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/decorators/_threaded.py
+-rw-r--r--   0        0        0     2196 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/py.typed
+-rw-r--r--   0        0        0    22008 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/thread.py
+-rw-r--r--   0        0        0      123 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/utils/__init__.py
+-rw-r--r--   0        0        0     1385 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/utils/algorithm.py
+-rw-r--r--   0        0        0     4527 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/utils/config.py
+-rw-r--r--   0        0        0       61 2024-04-28 08:08:00.668455 thread-2.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     1232 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_algorithm.py
+-rw-r--r--   0        0        0     1816 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_concurrentprocessing.py
+-rw-r--r--   0        0        0     9467 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_dataframe_compatibility.py
+-rw-r--r--   0        0        0     2114 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_decorator.py
+-rw-r--r--   0        0        0     3405 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_thread.py
+-rw-r--r--   0        0        0     1480 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_verbosity.py
+-rw-r--r--   0        0        0     6043 1970-01-01 00:00:00.000000 thread-2.0.1/PKG-INFO
```

### Comparing `thread-2.0.0/LICENSE.txt` & `thread-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thread-2.0.0/README.md` & `thread-2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -82,38 +82,14 @@
    from thread import Thread, ConcurrentProcessing
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
-<!-- DOCS -->
-## Documentation
-
-Our docs are [here!](https://thread.ngjx.org)
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- ROADMAP -->
-## Roadmap
-
-- [x] v2.0.0 Release
-- [ ] Bug fixes
-- [ ] New features
-- [ ] Testing
-- [ ] Next release...
-
-See the [open issues](https://github.com/python-thread/thread/issues) for a full list of proposed features (and known issues).
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- CONTRIBUTING -->
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**. ( ˶ˆᗜˆ˵ )
 
 If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
 Don't forget to give the project a star! Thanks again!
@@ -138,18 +114,14 @@
 
 
 <!-- CONTACT -->
 ## Contact
 
 Alex - [contact@thread.ngjx.org](mailto:contact@thread.ngjx.org)
 
-Project Board: [https://github.com/orgs/python-thread/projects/2](https://github.com/orgs/python-thread/projects/2)
-
-Project Link: [https://github.com/python-thread/thread](https://github.com/python-thread/thread)
-
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- ACKNOWLEDGMENTS -->
 ## Acknowledgments
```

#### html2text {}

```diff
@@ -21,37 +21,28 @@
 ## Getting Started This is an example of how you can set up your project
 locally. To get a local copy up and running follow these simple example steps.
 ### Prerequisites * Python 3.9+ ### Installation _Below is an example of how
 you can install and use thread._ 1. Install the package ```sh pip install -
 U thread ``` 2. Import thread into your library! ```py import thread from
 thread import Thread, ConcurrentProcessing ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Documentation Our docs are [here!](https://thread.ngjx.org)
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [x] v2.0.0 Release - [ ] Bug fixes - [ ] New features - [ ]
-Testing - [ ] Next release... See the [open issues](https://github.com/python-
-thread/thread/issues) for a full list of proposed features (and known issues).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. ( Ë¶ËáËËµ ) If you have a suggestion that would
 make this better, please fork the repo and create a pull request. You can also
 simply open an issue with the tag "enhancement". Don't forget to give the
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
 -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the BSD-3-Clause License. See [LICENSE.txt](./
 LICENSE.txt) for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact Alex - [contact@thread.ngjx.org](mailto:contact@thread.ngjx.org)
-Project Board: [https://github.com/orgs/python-thread/projects/2](https://
-github.com/orgs/python-thread/projects/2) Project Link: [https://github.com/
-python-thread/thread](https://github.com/python-thread/thread)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Acknowledgments * [Choose an Open Source License](https://
 choosealicense.com) * [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/
 tools/emoji-cheat-sheet) * [Malven's Flexbox Cheatsheet](https://
 flexbox.malven.co/) * [Malven's Grid Cheatsheet](https://grid.malven.co/) *
 [Img Shields](https://shields.io)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `thread-2.0.0/pyproject.toml` & `thread-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thread"
-version = "2.0.0"
+version = "2.0.1"
 description = "Threading module extension"
 authors = ["Alex <contact@ngjx.org>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [
   { include = "thread", from = "src" },
   { include = "thread/py.typed", from = "src" },
@@ -26,15 +26,15 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: Implementation :: CPython",
   "Typing :: Typed",
 ]
 
 [tool.poetry.urls]
 Homepage = "https://thread.ngjx.org"
-Documentation = "https://thread.ngjx.org/docs/v2.0.0"
+Documentation = "https://thread.ngjx.org/docs/v2.0.1"
 Source = "https://github.com/python-thread/thread"
 Download = "https://pypi.org/project/thread/#files"
 "Release Notes" = "https://github.com/python-thread/thread/releases"
 "Bug Tracker" = "https://github.com/python-thread/thread/issues"
 
 [tool.poetry.scripts]
 thread = "thread.__main__:app"
```

### Comparing `thread-2.0.0/src/thread/__init__.py` & `thread-2.0.1/src/thread/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ## Thread Library
-Documentation at https://thread.ngjx.org/docs/2.0.0
+Documentation at https://thread.ngjx.org/docs/2.0.1
 
 
 ---
 
 Released under the BSD-3 License
 
 Copyright (c) thread.ngjx.org, All rights reserved
@@ -14,15 +14,15 @@
 This file contains the exports to
 ```py
 import thread
 ```
 """
 
 
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 
 
 # Export Core
 from .thread import Thread, ConcurrentProcessing
 
 
 from . import _types as types, exceptions
```

### Comparing `thread-2.0.0/src/thread/_types.py` & `thread-2.0.1/src/thread/_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ## Types
 
-Documentation: https://thread.ngjx.org/docs/v2.0.0
+Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 from typing import Any, Literal, Callable, Union, Sized
 from typing_extensions import (
     ParamSpec,
     TypeVar,
     Concatenate,
```

### Comparing `thread-2.0.0/src/thread/decorators/_processor.py` & `thread-2.0.1/src/thread/decorators/_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ## Processor
 
-Documentation: https://thread.ngjx.org/docs/v2.0.0
+Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 from functools import wraps
 from ..thread import ConcurrentProcessing
 
 from .._types import (
     Overflow_In,
```

### Comparing `thread-2.0.0/src/thread/decorators/_threaded.py` & `thread-2.0.1/src/thread/decorators/_threaded.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ## Threaded
 
-Documentation: https://thread.ngjx.org/docs/v2.0.0
+Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 from functools import wraps
 from ..thread import Thread
 
 from .._types import Overflow_In, Data_In
 from typing import Callable, Mapping, Sequence, Optional, Union, overload
```

### Comparing `thread-2.0.0/src/thread/exceptions.py` & `thread-2.0.1/src/thread/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ## Thread Exceptions
 
-Documentation: https://thread.ngjx.org/docs/v2.0.0
+Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 import traceback
 from typing import Any, Optional, Sequence, Tuple
 
 
 class ErrorBase(Exception):
```

### Comparing `thread-2.0.0/src/thread/thread.py` & `thread-2.0.1/src/thread/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ```py
 class Thread: ...
 
 
 class ConcurrentProcessing: ...
 ```
 
-Documentation: https://thread.ngjx.org/docs/v2.0.0
+Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 import sys
 import time
 import ctypes
 import signal
 import threading
```

### Comparing `thread-2.0.0/src/thread/utils/algorithm.py` & `thread-2.0.1/src/thread/utils/algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 If it gets too dense, we could consider splitting it into a library import
 |_ algorithm/
   |_ __init__.py
   |_ a.py
   |_ b.py
 """
 
-from typing import List, Tuple
+from typing import Tuple, Generator
 
 
-def chunk_split(dataset_length: int, number_of_chunks: int) -> List[Tuple[int, int]]:
+def chunk_split(
+    dataset_length: int, number_of_chunks: int
+) -> Generator[Tuple[int, int], None, None]:
     """
     Splits a dataset into balanced chunks
 
     If the size of the dataset is not fully divisible by the number of chunks, it is split like this
       > `[ [n+1], [n+1], [n+1], [n], [n], [n] ]`
 
 
@@ -23,31 +25,28 @@
     ----------
     :param dataset_length: This should be the length of the dataset you want to split into chunks
     :param number_of_chunks: The should be the number of chunks it will attempt to split into
 
 
     Returns
     -------
-    :returns list[tuple[int, int]]: The chunked dataset slices
+    :returns Generator[tuple[int, int], None, None]: The chunked dataset slices
 
     Raises
     ------
     AssertionError: The number of chunks specified is larger than the dataset size
     """
     assert (
         dataset_length >= number_of_chunks
     ), 'The number of chunks specified is larger than the dataset size'
 
     chunk_count = dataset_length // number_of_chunks
     overflow = dataset_length % number_of_chunks
 
     i = 0
-    split = []
     while i < dataset_length:
         chunk_length = chunk_count + int(overflow > 0)
         b = i + chunk_length
 
-        split.append((i, b))
+        yield (i, b)
         overflow -= 1
         i = b
-
-    return split
```

### Comparing `thread-2.0.0/src/thread/utils/config.py` & `thread-2.0.1/src/thread/utils/config.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.0/tests/test_algorithm.py` & `thread-2.0.1/tests/test_algorithm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import random
-from src.thread.utils import algorithm
+from typing import Generator
+
+from thread.utils import algorithm
+
+
+def test_type():
+    assert isinstance(algorithm.chunk_split(5, 1), Generator)
 
 
 def test_chunking_1():
-    assert algorithm.chunk_split(5, 1) == [(0, 5)]
+    assert list(algorithm.chunk_split(5, 1)) == [(0, 5)]
 
 
 def test_chunking_2():
-    assert algorithm.chunk_split(5, 2) == [(0, 3), (3, 5)]
+    assert list(algorithm.chunk_split(5, 2)) == [(0, 3), (3, 5)]
 
 
 def test_chunking_3():
-    assert algorithm.chunk_split(100, 8) == [
+    assert list(algorithm.chunk_split(100, 8)) == [
         (0, 13),
         (13, 26),
         (26, 39),
         (39, 52),
         (52, 64),
         (64, 76),
         (76, 88),
@@ -27,19 +33,17 @@
     dataset_length = random.randint(400, int(10e6))
     thread_count = random.randint(2, 100)
 
     expected_chunk_length_low = dataset_length // thread_count
     expected_chunk_high = dataset_length % thread_count
 
     i = 0
-    heap = []
+    gen = algorithm.chunk_split(dataset_length, thread_count)
     while i < dataset_length:
         chunk_length = expected_chunk_length_low + int(expected_chunk_high > 0)
         b = i + chunk_length
 
-        heap.append((i, b))
+        assert (
+            next(gen) == (i, b)
+        ), f'\nIndex: {i}\nLength: {dataset_length}\nThreads: {thread_count}\nExpected: {(i, b)}\nActual: {next(gen)}'
         expected_chunk_high -= 1
         i = b
-
-    assert (
-        algorithm.chunk_split(dataset_length, thread_count) == heap
-    ), f'\nLength: {dataset_length}\nThreads: {thread_count}\nExpected: {heap}\nActual: {algorithm.chunk_split(dataset_length, thread_count)}'
```

### Comparing `thread-2.0.0/tests/test_concurrentprocessing.py` & `thread-2.0.1/tests/test_concurrentprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import pytest
-from src.thread import ConcurrentProcessing, exceptions
+from thread import ConcurrentProcessing, exceptions
 
 
 # >>>>>>>>>> Dummy Functions <<<<<<<<<< #
 def _dummy_dataProcessor(data_in: int, delay: float = 0) -> int:
     time.sleep(delay)
     return data_in
```

### Comparing `thread-2.0.0/tests/test_dataframe_compatibility.py` & `thread-2.0.1/tests/test_dataframe_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 import pytest
-from src.thread import ConcurrentProcessing
+from thread import ConcurrentProcessing
 
 
 class DummyLengthOnly:
     length: typing.Any
 
     def __init__(self, length: typing.Any):
         self.length = length
```

### Comparing `thread-2.0.0/tests/test_decorator.py` & `thread-2.0.1/tests/test_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from src.thread import threaded, processor
+from thread import threaded, processor
 
 
 # >>>>>>>>>> Dummy Functions <<<<<<<<<< #
 def _dummy_target_raiseToPower(x: float, power: float, delay: float = 0):
     time.sleep(delay)
     return x**power
```

### Comparing `thread-2.0.0/tests/test_thread.py` & `thread-2.0.1/tests/test_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import pytest
-from src.thread import Thread, exceptions
+from thread import Thread, exceptions
 
 
 # >>>>>>>>>> Dummy Functions <<<<<<<<<< #
 def _dummy_target_raiseToPower(x: float, power: float, delay: float = 0):
     time.sleep(delay)
     return x**power
```

### Comparing `thread-2.0.0/tests/test_verbosity.py` & `thread-2.0.1/tests/test_verbosity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from src.thread.utils.config import Verbosity
+from thread.utils.config import Verbosity
 
 
 # >>>>>>>>>> General Use <<<<<<<<<< #
 def test_eqTrue():
     assert Verbosity(0) == 0
     assert Verbosity(0) == 'quiet'
     assert Verbosity(1) == 'normal'
```

### Comparing `thread-2.0.0/PKG-INFO` & `thread-2.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thread
-Version: 2.0.0
+Version: 2.0.1
 Summary: Threading module extension
 License: BSD-3-Clause
 Keywords: thread,threading,extension,multiprocessing
 Author: Alex
 Author-email: contact@ngjx.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/python-thread/thread/issues
-Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.0
+Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.1
 Project-URL: Download, https://pypi.org/project/thread/#files
 Project-URL: Homepage, https://thread.ngjx.org
 Project-URL: Release Notes, https://github.com/python-thread/thread/releases
 Project-URL: Source, https://github.com/python-thread/thread
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
@@ -114,38 +114,14 @@
    from thread import Thread, ConcurrentProcessing
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
-<!-- DOCS -->
-## Documentation
-
-Our docs are [here!](https://thread.ngjx.org)
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- ROADMAP -->
-## Roadmap
-
-- [x] v2.0.0 Release
-- [ ] Bug fixes
-- [ ] New features
-- [ ] Testing
-- [ ] Next release...
-
-See the [open issues](https://github.com/python-thread/thread/issues) for a full list of proposed features (and known issues).
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!-- CONTRIBUTING -->
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**. ( ˶ˆᗜˆ˵ )
 
 If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
 Don't forget to give the project a star! Thanks again!
@@ -170,18 +146,14 @@
 
 
 <!-- CONTACT -->
 ## Contact
 
 Alex - [contact@thread.ngjx.org](mailto:contact@thread.ngjx.org)
 
-Project Board: [https://github.com/orgs/python-thread/projects/2](https://github.com/orgs/python-thread/projects/2)
-
-Project Link: [https://github.com/python-thread/thread](https://github.com/python-thread/thread)
-
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- ACKNOWLEDGMENTS -->
 ## Acknowledgments
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: thread Version: 2.0.0 Summary: Threading module
+Metadata-Version: 2.1 Name: thread Version: 2.0.1 Summary: Threading module
 extension License: BSD-3-Clause Keywords:
 thread,threading,extension,multiprocessing Author: Alex Author-email:
 contact@ngjx.org Requires-Python: >=3.9,<4.0 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Software Development
 Classifier: Typing :: Typed Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/python-thread/thread/issues
-Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.0 Project-URL:
+Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.1 Project-URL:
 Download, https://pypi.org/project/thread/#files Project-URL: Homepage, https:/
 /thread.ngjx.org Project-URL: Release Notes, https://github.com/python-thread/
 thread/releases Project-URL: Source, https://github.com/python-thread/thread
 Description-Content-Type: text/markdown
  _[_!_[_P_Y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_v_e_r_s_i_o_n_-_s_h_i_e_l_d_]_]_[_p_y_p_i_-_u_r_l_] _[_!_[_P_Y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_d_o_w_n_l_o_a_d_s_-
  _s_h_i_e_l_d_]_]_[_p_y_p_i_-_u_r_l_] _[_!_[_F_o_r_k_s_]_[_f_o_r_k_s_-_s_h_i_e_l_d_]_]_[_f_o_r_k_s_-_u_r_l_] _[_!_[_S_t_a_r_g_a_z_e_r_s_]_[_s_t_a_r_s_-
   _s_h_i_e_l_d_]_]_[_s_t_a_r_s_-_u_r_l_] _[_!_[_B_S_D_-_3_-_C_l_a_u_s_e_ _L_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_-_s_h_i_e_l_d_]_]_[_l_i_c_e_n_s_e_-_u_r_l_]
@@ -40,37 +40,28 @@
 ## Getting Started This is an example of how you can set up your project
 locally. To get a local copy up and running follow these simple example steps.
 ### Prerequisites * Python 3.9+ ### Installation _Below is an example of how
 you can install and use thread._ 1. Install the package ```sh pip install -
 U thread ``` 2. Import thread into your library! ```py import thread from
 thread import Thread, ConcurrentProcessing ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Documentation Our docs are [here!](https://thread.ngjx.org)
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [x] v2.0.0 Release - [ ] Bug fixes - [ ] New features - [ ]
-Testing - [ ] Next release... See the [open issues](https://github.com/python-
-thread/thread/issues) for a full list of proposed features (and known issues).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. ( Ë¶ËáËËµ ) If you have a suggestion that would
 make this better, please fork the repo and create a pull request. You can also
 simply open an issue with the tag "enhancement". Don't forget to give the
 project a star! Thanks again! 1. Fork the Project 2. Create your Feature Branch
 (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
 -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the BSD-3-Clause License. See [LICENSE.txt](./
 LICENSE.txt) for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact Alex - [contact@thread.ngjx.org](mailto:contact@thread.ngjx.org)
-Project Board: [https://github.com/orgs/python-thread/projects/2](https://
-github.com/orgs/python-thread/projects/2) Project Link: [https://github.com/
-python-thread/thread](https://github.com/python-thread/thread)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Acknowledgments * [Choose an Open Source License](https://
 choosealicense.com) * [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/
 tools/emoji-cheat-sheet) * [Malven's Flexbox Cheatsheet](https://
 flexbox.malven.co/) * [Malven's Grid Cheatsheet](https://grid.malven.co/) *
 [Img Shields](https://shields.io)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

