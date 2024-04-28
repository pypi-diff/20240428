# Comparing `tmp/refparse-0.3.0.tar.gz` & `tmp/refparse-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refparse-0.3.0.tar", last modified: Tue Mar 19 15:14:27 2024, max compression
+gzip compressed data, was "refparse-0.4.0.tar", last modified: Sun Apr 28 04:39:03 2024, max compression
```

## Comparing `refparse-0.3.0.tar` & `refparse-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:14:27.064110 refparse-0.3.0/
--rw-rw-rw-   0        0        0     1085 2024-03-10 02:36:50.000000 refparse-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      989 2024-03-19 15:14:27.064110 refparse-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       54 2024-03-10 02:36:50.000000 refparse-0.3.0/README.md
--rw-rw-rw-   0        0        0     1186 2024-03-10 02:36:50.000000 refparse-0.3.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-19 15:14:27.029960 refparse-0.3.0/refparse/
--rw-rw-rw-   0        0        0       23 2024-03-19 03:54:59.000000 refparse-0.3.0/refparse/__init__.py
--rw-rw-rw-   0        0        0     7292 2024-03-10 02:36:50.000000 refparse-0.3.0/refparse/cssci.py
--rw-rw-rw-   0        0        0     9964 2024-03-19 14:25:47.000000 refparse-0.3.0/refparse/scopus.py
--rw-rw-rw-   0        0        0     6558 2024-03-10 02:36:50.000000 refparse-0.3.0/refparse/wos.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:14:27.063109 refparse-0.3.0/refparse.egg-info/
--rw-rw-rw-   0        0        0      989 2024-03-19 15:14:26.000000 refparse-0.3.0/refparse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-03-19 15:14:27.000000 refparse-0.3.0/refparse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:14:26.000000 refparse-0.3.0/refparse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-19 15:14:26.000000 refparse-0.3.0/refparse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 15:14:27.065112 refparse-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-19 15:14:27.061103 refparse-0.3.0/tests/
--rw-rw-rw-   0        0        0    13549 2024-03-18 17:38:27.000000 refparse-0.3.0/tests/test_cssci.py
--rw-rw-rw-   0        0        0    12465 2024-03-19 14:31:11.000000 refparse-0.3.0/tests/test_scopus.py
--rw-rw-rw-   0        0        0     7678 2024-03-19 02:26:05.000000 refparse-0.3.0/tests/test_wos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:39:03.654750 refparse-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 04:38:54.000000 refparse-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-28 04:39:03.654750 refparse-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-28 04:38:54.000000 refparse-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-28 04:38:54.000000 refparse-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:39:03.654750 refparse-0.4.0/refparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-28 04:38:54.000000 refparse-0.4.0/refparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-28 04:38:54.000000 refparse-0.4.0/refparse/cssci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-28 04:38:54.000000 refparse-0.4.0/refparse/scopus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-28 04:38:54.000000 refparse-0.4.0/refparse/wos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:39:03.654750 refparse-0.4.0/refparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-28 04:39:03.000000 refparse-0.4.0/refparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-28 04:39:03.000000 refparse-0.4.0/refparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:39:03.000000 refparse-0.4.0/refparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 04:39:03.000000 refparse-0.4.0/refparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:39:03.654750 refparse-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:39:03.654750 refparse-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-04-28 04:38:54.000000 refparse-0.4.0/tests/test_cssci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-04-28 04:38:54.000000 refparse-0.4.0/tests/test_scopus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-28 04:38:54.000000 refparse-0.4.0/tests/test_wos.py
```

### Comparing `refparse-0.3.0/LICENSE` & `refparse-0.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Wang K2
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Wang K2
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `refparse-0.3.0/pyproject.toml` & `refparse-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,72 @@
-00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
-00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
-00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
-00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
-00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
-00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
-00000060: 0a6e 616d 6520 3d20 2272 6566 7061 7273  .name = "refpars
-00000070: 6522 0d0a 6175 7468 6f72 7320 3d20 5b7b  e"..authors = [{
-00000080: 6e61 6d65 203d 2022 5761 6e67 4b32 222c  name = "WangK2",
-00000090: 2065 6d61 696c 203d 2022 6b77 3232 3132   email = "kw2212
-000000a0: 3235 4067 6d61 696c 2e63 6f6d 227d 5d0d  25@gmail.com"}].
-000000b0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
-000000c0: 4120 5079 7468 6f6e 206c 6962 7261 7279  A Python library
-000000d0: 2074 6f20 7061 7273 6520 6269 626c 696f   to parse biblio
-000000e0: 6772 6170 6869 6320 7265 6665 7265 6e63  graphic referenc
-000000f0: 6573 220d 0a6c 6963 656e 7365 203d 207b  es"..license = {
-00000100: 7465 7874 203d 2022 4d49 5422 7d0d 0a72  text = "MIT"}..r
-00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
-00000120: 6d64 220d 0a72 6571 7569 7265 732d 7079  md"..requires-py
-00000130: 7468 6f6e 203d 2022 3e3d 332e 3922 0d0a  thon = ">=3.9"..
-00000140: 636c 6173 7369 6669 6572 7320 3d20 5b0d  classifiers = [.
-00000150: 0a20 2020 2022 4465 7665 6c6f 706d 656e  .    "Developmen
-00000160: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
-00000170: 416c 7068 6122 2c0d 0a20 2020 2022 496e  Alpha",..    "In
-00000180: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000190: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
-000001a0: 7263 6822 2c0d 0a20 2020 2022 4c69 6365  rch",..    "Lice
-000001b0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001c0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-000001d0: 7365 222c 0d0a 2020 2020 2250 726f 6772  se",..    "Progr
-000001e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 222c  :: Python :: 3",
-00000200: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
-00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000220: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
-00000230: 6c79 222c 0d0a 2020 2020 2250 726f 6772  ly",..    "Progr
-00000240: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000250: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-00000260: 222c 0d0a 2020 2020 2250 726f 6772 616d  ",..    "Program
-00000270: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000280: 2050 7974 686f 6e20 3a3a 2033 2e31 3022   Python :: 3.10"
-00000290: 2c0d 0a20 2020 2022 5072 6f67 7261 6d6d  ,..    "Programm
-000002a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002b0: 5079 7468 6f6e 203a 3a20 332e 3131 222c  Python :: 3.11",
-000002c0: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
-000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002e0: 7974 686f 6e20 3a3a 2033 2e31 3222 2c0d  ython :: 3.12",.
-000002f0: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
-00000300: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000310: 6570 656e 6465 6e74 222c 0d0a 2020 2020  ependent",..    
-00000320: 2254 6f70 6963 203a 3a20 5363 6965 6e74  "Topic :: Scient
-00000330: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
-00000340: 203a 3a20 496e 666f 726d 6174 696f 6e20   :: Information 
-00000350: 416e 616c 7973 6973 222c 0d0a 2020 2020  Analysis",..    
-00000360: 2254 7970 696e 6720 3a3a 2054 7970 6564  "Typing :: Typed
-00000370: 222c 0d0a 2020 2020 5d0d 0a64 796e 616d  ",..    ]..dynam
-00000380: 6963 203d 205b 2276 6572 7369 6f6e 225d  ic = ["version"]
-00000390: 0d0a 0d0a 5b70 726f 6a65 6374 2e75 726c  ....[project.url
-000003a0: 735d 0d0a 5265 706f 7369 746f 7279 203d  s]..Repository =
-000003b0: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-000003c0: 2e63 6f6d 2f64 6f75 626c 6573 7361 792f  .com/doublessay/
-000003d0: 7265 6670 6172 7365 220d 0a0d 0a5b 746f  refparse"....[to
-000003e0: 6f6c 2e73 6574 7570 746f 6f6c 735d 0d0a  ol.setuptools]..
-000003f0: 7061 636b 6167 6573 203d 205b 2272 6566  packages = ["ref
-00000400: 7061 7273 6522 5d0d 0a0d 0a5b 746f 6f6c  parse"]....[tool
-00000410: 2e73 6574 7570 746f 6f6c 732e 6479 6e61  .setuptools.dyna
-00000420: 6d69 635d 0d0a 7665 7273 696f 6e20 3d20  mic]..version = 
-00000430: 7b61 7474 7220 3d20 2272 6566 7061 7273  {attr = "refpars
-00000440: 652e 5f5f 7665 7273 696f 6e5f 5f22 7d0d  e.__version__"}.
-00000450: 0a0d 0a5b 746f 6f6c 2e62 6c61 636b 5d0d  ...[tool.black].
-00000460: 0a6c 696e 652d 6c65 6e67 7468 203d 2031  .line-length = 1
-00000470: 3230 0d0a 0d0a 5b74 6f6f 6c2e 636f 7665  20....[tool.cove
-00000480: 7261 6765 2e72 756e 5d0d 0a73 6f75 7263  rage.run]..sourc
-00000490: 6520 3d20 5b22 7265 6670 6172 7365 225d  e = ["refparse"]
-000004a0: 0d0a                                     ..
+00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0a72  [build-system].r
+00000010: 6571 7569 7265 7320 3d20 5b22 7365 7475  equires = ["setu
+00000020: 7074 6f6f 6c73 225d 0a62 7569 6c64 2d62  ptools"].build-b
+00000030: 6163 6b65 6e64 203d 2022 7365 7475 7074  ackend = "setupt
+00000040: 6f6f 6c73 2e62 7569 6c64 5f6d 6574 6122  ools.build_meta"
+00000050: 0a0a 5b70 726f 6a65 6374 5d0a 6e61 6d65  ..[project].name
+00000060: 203d 2022 7265 6670 6172 7365 220a 6175   = "refparse".au
+00000070: 7468 6f72 7320 3d20 5b7b 6e61 6d65 203d  thors = [{name =
+00000080: 2022 5761 6e67 4b32 222c 2065 6d61 696c   "WangK2", email
+00000090: 203d 2022 6b77 3232 3132 3235 4067 6d61   = "kw221225@gma
+000000a0: 696c 2e63 6f6d 227d 5d0a 6465 7363 7269  il.com"}].descri
+000000b0: 7074 696f 6e20 3d20 2241 2050 7974 686f  ption = "A Pytho
+000000c0: 6e20 6c69 6272 6172 7920 746f 2070 6172  n library to par
+000000d0: 7365 2062 6962 6c69 6f67 7261 7068 6963  se bibliographic
+000000e0: 2072 6566 6572 656e 6365 7322 0a6c 6963   references".lic
+000000f0: 656e 7365 203d 207b 7465 7874 203d 2022  ense = {text = "
+00000100: 4d49 5422 7d0a 7265 6164 6d65 203d 2022  MIT"}.readme = "
+00000110: 5245 4144 4d45 2e6d 6422 0a72 6571 7569  README.md".requi
+00000120: 7265 732d 7079 7468 6f6e 203d 2022 3e3d  res-python = ">=
+00000130: 332e 3922 0a63 6c61 7373 6966 6965 7273  3.9".classifiers
+00000140: 203d 205b 0a20 2020 2022 4465 7665 6c6f   = [.    "Develo
+00000150: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+00000160: 3320 2d20 416c 7068 6122 2c0a 2020 2020  3 - Alpha",.    
+00000170: 2249 6e74 656e 6465 6420 4175 6469 656e  "Intended Audien
+00000180: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
+00000190: 7365 6172 6368 222c 0a20 2020 2022 4c69  search",.    "Li
+000001a0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000001b0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+000001c0: 656e 7365 222c 0a20 2020 2022 5072 6f67  ense",.    "Prog
+000001d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001e0: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
+000001f0: 2c0a 2020 2020 2250 726f 6772 616d 6d69  ,.    "Programmi
+00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000210: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
+00000220: 6c79 222c 0a20 2020 2022 5072 6f67 7261  ly",.    "Progra
+00000230: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000240: 3a20 5079 7468 6f6e 203a 3a20 332e 3922  : Python :: 3.9"
+00000250: 2c0a 2020 2020 2250 726f 6772 616d 6d69  ,.    "Programmi
+00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000270: 7974 686f 6e20 3a3a 2033 2e31 3022 2c0a  ython :: 3.10",.
+00000280: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
+00000290: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002a0: 686f 6e20 3a3a 2033 2e31 3122 2c0a 2020  hon :: 3.11",.  
+000002b0: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
+000002c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002d0: 6e20 3a3a 2033 2e31 3222 2c0a 2020 2020  n :: 3.12",.    
+000002e0: 224f 7065 7261 7469 6e67 2053 7973 7465  "Operating Syste
+000002f0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000300: 656e 7422 2c0a 2020 2020 2254 6f70 6963  ent",.    "Topic
+00000310: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
+00000320: 6e67 696e 6565 7269 6e67 203a 3a20 496e  ngineering :: In
+00000330: 666f 726d 6174 696f 6e20 416e 616c 7973  formation Analys
+00000340: 6973 222c 0a20 2020 2022 5479 7069 6e67  is",.    "Typing
+00000350: 203a 3a20 5479 7065 6422 2c0a 2020 2020   :: Typed",.    
+00000360: 5d0a 6479 6e61 6d69 6320 3d20 5b22 7665  ].dynamic = ["ve
+00000370: 7273 696f 6e22 5d0a 0a5b 7072 6f6a 6563  rsion"]..[projec
+00000380: 742e 7572 6c73 5d0a 5265 706f 7369 746f  t.urls].Reposito
+00000390: 7279 203d 2022 6874 7470 733a 2f2f 6769  ry = "https://gi
+000003a0: 7468 7562 2e63 6f6d 2f64 6f75 626c 6573  thub.com/doubles
+000003b0: 7361 792f 7265 6670 6172 7365 220a 0a5b  say/refparse"..[
+000003c0: 746f 6f6c 2e73 6574 7570 746f 6f6c 735d  tool.setuptools]
+000003d0: 0a70 6163 6b61 6765 7320 3d20 5b22 7265  .packages = ["re
+000003e0: 6670 6172 7365 225d 0a0a 5b74 6f6f 6c2e  fparse"]..[tool.
+000003f0: 7365 7475 7074 6f6f 6c73 2e64 796e 616d  setuptools.dynam
+00000400: 6963 5d0a 7665 7273 696f 6e20 3d20 7b61  ic].version = {a
+00000410: 7474 7220 3d20 2272 6566 7061 7273 652e  ttr = "refparse.
+00000420: 5f5f 7665 7273 696f 6e5f 5f22 7d0a 0a5b  __version__"}..[
+00000430: 746f 6f6c 2e62 6c61 636b 5d0a 6c69 6e65  tool.black].line
+00000440: 2d6c 656e 6774 6820 3d20 3132 300a 0a5b  -length = 120..[
+00000450: 746f 6f6c 2e63 6f76 6572 6167 652e 7275  tool.coverage.ru
+00000460: 6e5d 0a73 6f75 7263 6520 3d20 5b22 7265  n].source = ["re
+00000470: 6670 6172 7365 225d 0a                   fparse"].
```

### Comparing `refparse-0.3.0/refparse/wos.py` & `refparse-0.4.0/refparse/wos.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,173 +1,135 @@
-import re
-from typing import Optional
-
-
-class ParseWos:
-    def __init__(self, ref: str, keep_one_doi: bool = True, keep_eng_result: bool = True):
-        self.ref = self.clean(ref)
-        self.keep_one_doi = keep_one_doi
-        self.keep_eng_result = keep_eng_result
-
-    @staticmethod
-    def clean(ref: str) -> str:
-        # Remove duplicated commas. e.g. ForeRunner3D,, 2020, DOES HP MULTIJET FUS
-        ref = re.sub(r",{2,}", ",", ref)
-
-        # Remove blank spaces before commas.
-        # e.g. Afshinmanesh F, 2005, EUROCON 2005: THE INTERNATIONAL CONFERENCE ON COMPUTER AS A TOOL, VOL 1 AND 2 , PROCEEDINGS, P217
-        ref = re.sub(r" ,", ",", ref)
-        return ref
-
-    def parse(self):
-        if self.ref.startswith("[Anonymous]"):
-            return None
-        elif "Patent No." in self.ref:
-            return self.parse_patent()
-        elif re.search(r"\d{4}, \[", self.ref):
-            return self.parse_bilingual()
-        else:
-            return self.parse_general()
-
-    @staticmethod
-    def extract_doi(entry: str) -> Optional[str]:
-        """Extract DOI from a reference entry."""
-        if ", DOI [" in entry:
-            doi_part = re.split(r", DOI (?=\[)", entry, maxsplit=1)[1]
-            doi_list = doi_part.strip("[]").split(", ")
-            doi_set = set(doi.replace("DOI ", "").lower() for doi in doi_list)
-            if len(doi_set) == 1:
-                doi = doi_set.pop()
-            elif len(doi_set) > 1:
-                doi = "; ".join(doi_set)
-        elif ", DOI " in entry:
-            doi_match = re.search(r"DOI (10\..*)$", entry)
-            if doi_match:
-                doi = doi_match.group(1).lower()
-        else:
-            doi = None
-        return doi
-
-    @staticmethod
-    def extract_page(entry: str) -> Optional[str]:
-        """Extract page number from a reference entry."""
-        page_match = re.search(r", p([A-Za-z\d]+)(?=, DOI|$)", entry, flags=re.I)
-        page = page_match.group(1) if page_match else None
-        return page
-
-    @staticmethod
-    def extract_volume(entry: str) -> Optional[str]:
-        """Extract volume number from a reference entry."""
-        if re.search(", vol", entry, flags=re.I):
-            volume_match = re.search(r"vol[s\.]? ([\w\-: ]+)(?=, |$)", entry, flags=re.I)
-        elif re.search(", vvolume", entry, flags=re.I):
-            volume_match = re.search(r", vvolume (\d+)(?=, |$)", entry, flags=re.I)
-        else:
-            volume_match = re.search(r", v([\w\-\. ]+)(?=(, |$))", entry, flags=re.I)
-        return volume_match.group(1) if volume_match else None
-
-    def parse_general(self) -> dict[str, Optional[str]]:
-        if re.search(r", \d{4}, ", self.ref):
-            parts = self.ref.split(", ", maxsplit=3)
-            author = parts[0]
-            year = parts[1]
-            source = parts[2]
-        else:
-            parts = self.ref.split(", ", maxsplit=2)
-            author = parts[0]
-            year = None
-            source = parts[1]
-        volume = self.extract_volume(self.ref)
-        page = self.extract_page(self.ref)
-        doi = self.extract_doi(self.ref)
-        if self.keep_one_doi is True:
-            if doi is not None and "; " in doi:
-                doi = doi.split("; ")[0]
-        return {
-            "author": author,
-            "year": year,
-            "source": source,
-            "volume": volume,
-            "page": page,
-            "doi": doi,
-        }
-
-    def parse_bilingual(self) -> dict[str, Optional[str]]:
-        fields = re.split(r", (?![^\[]*\])", self.ref)
-        author = fields[0]
-        year = fields[1]
-        source = fields[2]
-        if author.startswith("["):
-            if re.search(r"\[[A-Za-z]+ ", author):
-                author_eng, author_non_eng = re.split(r" (?=[^A-Za-z]+)", author.strip("[]"), maxsplit=1)
-            else:
-                author_non_eng, author_eng = re.split(r"(?=[^A-Za-z]+) (?=[A-Za-z]+ )", author.strip("[]"), maxsplit=1)
-        else:
-            author_eng, author_non_eng = None, None
-            if re.search(r"^[A-Za-z]+ ", author):
-                author_eng = author
-            else:
-                author_non_eng = author
-
-        if re.search(r"\[[A-Za-z]+ ", source):
-            source_eng, source_non_eng = re.split(r", (?=[^A-Za-z]+)", source.strip("[]"), maxsplit=1)
-        else:
-            source_non_eng, source_eng = re.split(r"(?=[^A-Za-z]+), (?=[A-Za-z]+)", source.strip("[]"), maxsplit=1)
-        volume = self.extract_volume(self.ref)
-        page = self.extract_page(self.ref)
-        doi = self.extract_doi(self.ref)
-        if self.keep_eng_result is True:
-            return {
-                "author": author_eng,
-                "year": year,
-                "source": source_eng,
-                "volume": volume,
-                "page": page,
-                "doi": doi,
-            }
-        else:
-            return {
-                "author": author_non_eng,
-                "year": year,
-                "source": source_non_eng,
-                "volume": volume,
-                "page": page,
-                "doi": doi,
-            }
-
-    def parse_patent(self) -> dict[str, Optional[str]]:
-        """Parse a patent reference from Web of Science."""
-        first_part, patent_num_part = self.ref.split(", Patent No. ")
-        if patent_num_part.startswith("["):
-            patent_number_str = patent_num_part.strip("[]")
-            patent_number_list = patent_number_str.split(", ")
-            patent_number_set = set(i.replace(",", "") for i in patent_number_list)
-            patent_number = "; ".join(patent_number_set)
-        else:
-            patent_number = patent_num_part
-
-        fields = first_part.split(", ", maxsplit=2)
-        author = fields[0]
-        year = fields[1]
-
-        try:
-            # Fan P., 2011, PT, Patent No. 2011163640
-            if fields[2] == "PT":
-                title = None
-
-            # Redlich R. M., 2006, U. S. Patent, Patent No. [7,103,915, 7103915]
-            elif fields[2].endswith("Patent"):
-                title = None
-
-            else:
-                title = fields[2]
-
-        except IndexError:
-            # Pingchen Fan PZ, 2017, Patent No. [US9745268B2, 9745268]
-            title = None
-
-        return {
-            "author": author,
-            "year": year,
-            "title": title,
-            "identifier": patent_number,
-        }
+import re
+from typing import Optional
+
+
+class ParseWos:
+    def __init__(self, ref: str, keep_one_doi: bool = True, keep_eng_result: bool = True):
+        self.ref = self.clean(ref)
+        self.keep_one_doi = keep_one_doi
+        self.keep_eng_result = keep_eng_result
+
+    @staticmethod
+    def clean(ref: str) -> str:
+        # Remove duplicated commas. e.g. ForeRunner3D,, 2020, DOES HP MULTIJET FUS
+        ref = re.sub(r",{2,}", ",", ref)
+
+        # Remove blank spaces before commas.
+        # e.g. Afshinmanesh F, 2005, EUROCON 2005: THE INTERNATIONAL CONFERENCE ON COMPUTER AS A TOOL, VOL 1 AND 2 , PROCEEDINGS, P217
+        ref = re.sub(r" ,", ",", ref)
+        return ref
+
+    def parse(self):
+        if self.ref.startswith("[Anonymous]"):
+            return None
+        elif "Patent No." in self.ref:
+            return None
+        elif re.search(r"\d{4}, \[", self.ref):
+            return self.parse_bilingual()
+        else:
+            return self.parse_general()
+
+    @staticmethod
+    def extract_doi(entry: str) -> Optional[str]:
+        """Extract DOI from a reference entry."""
+        if ", DOI [" in entry:
+            doi_part = re.split(r", DOI (?=\[)", entry, maxsplit=1)[1]
+            doi_list = doi_part.strip("[]").split(", ")
+            doi_set = set(doi.replace("DOI ", "").lower() for doi in doi_list)
+            if len(doi_set) == 1:
+                doi = doi_set.pop()
+            elif len(doi_set) > 1:
+                doi = "; ".join(doi_set)
+        elif ", DOI " in entry:
+            doi_match = re.search(r"DOI (10\..*)$", entry)
+            if doi_match:
+                doi = doi_match.group(1).lower()
+        else:
+            doi = None
+        return doi
+
+    @staticmethod
+    def extract_page(entry: str) -> Optional[str]:
+        """Extract page number from a reference entry."""
+        page_match = re.search(r", p([A-Za-z\d]+)(?=, DOI|$)", entry, flags=re.I)
+        page = page_match.group(1) if page_match else None
+        return page
+
+    @staticmethod
+    def extract_volume(entry: str) -> Optional[str]:
+        """Extract volume number from a reference entry."""
+        if re.search(", vol", entry, flags=re.I):
+            volume_match = re.search(r"vol[s\.]? ([\w\-: ]+)(?=, |$)", entry, flags=re.I)
+        elif re.search(", vvolume", entry, flags=re.I):
+            volume_match = re.search(r", vvolume (\d+)(?=, |$)", entry, flags=re.I)
+        else:
+            volume_match = re.search(r", v([\w\-\. ]+)(?=(, |$))", entry, flags=re.I)
+        return volume_match.group(1) if volume_match else None
+
+    def parse_general(self) -> dict[str, Optional[str]]:
+        if re.search(r", \d{4}, ", self.ref):
+            parts = self.ref.split(", ", maxsplit=3)
+            author = parts[0]
+            year = parts[1]
+            source = parts[2]
+        else:
+            parts = self.ref.split(", ", maxsplit=2)
+            author = parts[0]
+            year = None
+            source = parts[1]
+        volume = self.extract_volume(self.ref)
+        page = self.extract_page(self.ref)
+        doi = self.extract_doi(self.ref)
+        if self.keep_one_doi is True:
+            if doi is not None and "; " in doi:
+                doi = doi.split("; ")[0]
+        return {
+            "author": author,
+            "year": year,
+            "source": source,
+            "volume": volume,
+            "page": page,
+            "doi": doi,
+        }
+
+    def parse_bilingual(self) -> dict[str, Optional[str]]:
+        fields = re.split(r", (?![^\[]*\])", self.ref)
+        author = fields[0]
+        year = fields[1]
+        source = fields[2]
+        if author.startswith("["):
+            if re.search(r"\[[A-Za-z]+ ", author):
+                author_eng, author_non_eng = re.split(r" (?=[^A-Za-z]+)", author.strip("[]"), maxsplit=1)
+            else:
+                author_non_eng, author_eng = re.split(r"(?=[^A-Za-z]+) (?=[A-Za-z]+ )", author.strip("[]"), maxsplit=1)
+        else:
+            author_eng, author_non_eng = None, None
+            if re.search(r"^[A-Za-z]+ ", author):
+                author_eng = author
+            else:
+                author_non_eng = author
+
+        if re.search(r"\[[A-Za-z]+ ", source):
+            source_eng, source_non_eng = re.split(r", (?=[^A-Za-z]+)", source.strip("[]"), maxsplit=1)
+        else:
+            source_non_eng, source_eng = re.split(r"(?=[^A-Za-z]+), (?=[A-Za-z]+)", source.strip("[]"), maxsplit=1)
+        volume = self.extract_volume(self.ref)
+        page = self.extract_page(self.ref)
+        doi = self.extract_doi(self.ref)
+        if self.keep_eng_result is True:
+            return {
+                "author": author_eng,
+                "year": year,
+                "source": source_eng,
+                "volume": volume,
+                "page": page,
+                "doi": doi,
+            }
+        else:
+            return {
+                "author": author_non_eng,
+                "year": year,
+                "source": source_non_eng,
+                "volume": volume,
+                "page": page,
+                "doi": doi,
+            }
```

### Comparing `refparse-0.3.0/tests/test_cssci.py` & `refparse-0.4.0/tests/test_cssci.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,421 +1,421 @@
-import pytest
-
-from refparse.cssci import ParseCssci
-
-test_clean_data = [
-    (
-        "1.康德.纯粹理性批判.北京:人民出版社",
-        "康德.纯粹理性批判.北京:人民出版社",
-    ),
-    (
-        "7..中华人民共和国公共图书馆法.2021",
-        ".中华人民共和国公共图书馆法.2021",
-    ),
-]
-
-test_web_data = [
-    (
-        "8.Google.Analytics.js.2021",
-        {
-            "type": "web",
-            "author": "Google",
-            "title": "Analytics.js",
-            "year": "2021",
-        },
-    ),
-    (
-        "9..CNNIC:微博用户达2.5亿，近半数网民使用.2012",
-        {
-            "type": "web",
-            "author": None,
-            "title": "CNNIC:微博用户达25亿，近半数网民使用2012",
-            "year": "2012",
-        },
-    ),
-    (
-        "22.IFLA.IFLA STRATEGY 2019-2024.2019",
-        {
-            "type": "web",
-            "author": "IFLA",
-            "title": "IFLA STRATEGY 2019-2024",
-            "year": "2019",
-        },
-    ),
-]
-
-test_standard_data = [
-    (
-        "8..GB/T37043-2018，智慧城市术语.北京:中国标准出版社",
-        {
-            "type": "standard",
-            "author": None,
-            "title": "智慧城市术语",
-            "source": "北京:中国标准出版社",
-            "year": None,
-            "identifier": "GB/T37043-2018",
-        },
-    ),
-    (
-        "17.全国信息技术标准化技术委员会教育技术分会.GB/T 36342-2018,智慧校园总体框架,2018",
-        {
-            "type": "standard",
-            "author": "全国信息技术标准化技术委员会教育技术分会",
-            "title": "智慧校园总体框架",
-            "source": None,
-            "year": "2018",
-            "identifier": "GB/T 36342-2018",
-        },
-    ),
-    (
-        "30.全国信息技术标准化技术委员会.智慧城市，数据融合，第5部分:市政基础设施数据元素:GB/T 36625.5-2019.北京:中国标准出版社",
-        {
-            "type": "standard",
-            "author": "全国信息技术标准化技术委员会",
-            "title": "智慧城市，数据融合，第5部分:市政基础设施数据元素",
-            "source": "北京:中国标准出版社",
-            "year": None,
-            "identifier": "GB/T 36625.5-2019",
-        },
-    ),
-]
-
-test_book_data = [
-    (
-        "14.吴建中.21世纪图书馆新论.上海:上海科学技术文献出版社",
-        {
-            "type": "book",
-            "author": "吴建中",
-            "title": "21世纪图书馆新论",
-            "source": "上海:上海科学技术文献出版社",
-        },
-    ),
-    (
-        "3.金元浦.中国文化概论.北京:首都师范大学出版社",
-        {
-            "type": "book",
-            "author": "金元浦",
-            "title": "中国文化概论",
-            "source": "北京:首都师范大学出版社",
-        },
-    ),
-]
-
-test_thesis_data = [
-    (
-        "21.郑怿昕.智慧图书馆环境下馆员核心能力研究:学位论文.南京:南京农业大学,2015:27-31",
-        {
-            "type": "thesis",
-            "author": "郑怿昕",
-            "title": "智慧图书馆环境下馆员核心能力研究",
-            "source": "南京:南京农业大学",
-            "year": "2015",
-        },
-    ),
-    (
-        "17.段美珍.智慧图书馆建设评价模型与应用研究:学位论文.北京:中国科学院大学,2020",
-        {
-            "type": "thesis",
-            "author": "段美珍",
-            "title": "智慧图书馆建设评价模型与应用研究",
-            "source": "北京:中国科学院大学",
-            "year": "2020",
-        },
-    ),
-]
-
-test_newspaper_data = [
-    (
-        "6..习近平在第二届世界互联网大会开幕式上的讲话.人民日报.12.17(2)",
-        {
-            "type": "newspaper",
-            "author": None,
-            "title": "习近平在第二届世界互联网大会开幕式上的讲话",
-            "source": "人民日报",
-            "date": "12.17",
-        },
-    ),
-    (
-        "25.曹磊.大数据:数字世界的智慧基因.文汇报.11.8(12)",
-        {
-            "type": "newspaper",
-            "author": "曹磊",
-            "title": "大数据:数字世界的智慧基因",
-            "source": "文汇报",
-            "date": "11.8",
-        },
-    ),
-    (
-        "65..图书馆来了机器人管理员.宁波日报.1.8",
-        {
-            "type": "newspaper",
-            "author": None,
-            "title": "图书馆来了机器人管理员",
-            "source": "宁波日报",
-            "date": "1.8",
-        },
-    ),
-]
-
-test_patent1_data = [
-    (
-        "26.图书上下架机器人.CN102152293A",
-        {
-            "type": "patent",
-            "title": "图书上下架机器人",
-            "identifier": "CN102152293A",
-        },
-    )
-]
-test_patent2_data = [
-    (
-        "9.一种基于RFID技术的自动式图书智能盘点机器人:201620075212.0.2016-01-25",
-        {
-            "type": "patent",
-            "title": "一种基于RFID技术的自动式图书智能盘点机器人",
-            "identifier": "201620075212.0",
-        },
-    ),
-    (
-        "39.一种基于区块链的金融安全存证平台系统及方法:中国，201910838935. X(2019-09-05)",
-        {
-            "type": "patent",
-            "title": "一种基于区块链的金融安全存证平台系统及方法",
-            "identifier": "201910838935",
-        },
-    ),
-]
-
-
-test_journal_data = [
-    (
-        "2.严栋.基于物联网的智慧图书馆.图书馆学刊.2010.32(7)",
-        {
-            "type": "journal",
-            "author": "严栋",
-            "title": "基于物联网的智慧图书馆",
-            "source": "图书馆学刊",
-            "year": "2010",
-            "volume": "32",
-            "issue": "7",
-        },
-    ),
-    (
-        "39.刘炜.5G与智慧图书馆建设.中国图书馆学报.2019.45(5)",
-        {
-            "type": "journal",
-            "author": "刘炜",
-            "title": "5G与智慧图书馆建设",
-            "source": "中国图书馆学报",
-            "year": "2019",
-            "volume": "45",
-            "issue": "5",
-        },
-    ),
-]
-
-test_english_data = [
-    (
-        "20.Alexei,P..Rite of passage.USA:Galaxy Publishing Co",
-        {
-            "type": "english-book",
-            "author": "Alexei,P.",
-            "title": "Rite of passage",
-            "source": "USA:Galaxy Publishing Co",
-            "year": None,
-            "page": None,
-        },
-    ),
-    (
-        "8.Sohail,S S.Book recommendation system using opinion mining technique:IEEE,2013:1609-1614",
-        {
-            "type": "english-book",
-            "author": "Sohail,S S",
-            "title": "Book recommendation system using opinion mining technique",
-            "source": "IEEE",
-            "year": "2013",
-            "page": "1609-1614",
-        },
-    ),
-    (
-        "7.Vaz,P C.Improving a hybrid literary book recommendation system through author ranking.New York:Association for Computing Machinery,2012:387-388",
-        {
-            "type": "english-book",
-            "author": "Vaz,P C",
-            "title": "Improving a hybrid literary book recommendation system through author ranking",
-            "source": "New York:Association for Computing Machinery",
-            "year": "2012",
-            "page": "387-388",
-        },
-    ),
-    (
-        "7.Hunzaker,M.B. Fallin.Mapping Cultural Schemas: From Theory to Method.American Sociological Review.2019.84(5)",
-        {
-            "type": "english-paper",
-            "author": "Hunzaker,M.B. Fallin",
-            "title": "Mapping Cultural Schemas: From Theory to Method",
-            "source": "American Sociological Review",
-            "year": "2019",
-            "volume": "84",
-            "issue": "5",
-        },
-    ),
-    (
-        "1.Aittola,M..Smart Library: Location-Aware Mobile Library Service.International Symposium on Human Computer Interaction with Mobile Devices and Services.2003.(5)",
-        {
-            "type": "english-paper",
-            "author": "Aittola,M.",
-            "title": "Smart Library: Location-Aware Mobile Library Service",
-            "source": "International Symposium on Human Computer Interaction with Mobile Devices and Services",
-            "year": "2003",
-            "volume": None,
-            "issue": "5",
-        },
-    ),
-]
-
-test_parse_data = [
-    (
-        "3..2021第五届中国未来智慧图书馆发展论坛.2021",
-        {
-            "type": "web",
-            "author": None,
-            "title": "2021第五届中国未来智慧图书馆发展论坛",
-            "year": "2021",
-        },
-    ),
-    (
-        "10..GB/T 35273-2020，信息安全技术个人信息安全规范",
-        {
-            "type": "standard",
-            "author": None,
-            "title": "信息安全技术个人信息安全规范",
-            "source": None,
-            "year": None,
-            "identifier": "GB/T 35273-2020",
-        },
-    ),
-    (
-        "14.吴慰慈.图书馆学概论.北京:北京图书馆出版社",
-        {
-            "type": "book",
-            "author": "吴慰慈",
-            "title": "图书馆学概论",
-            "source": "北京:北京图书馆出版社",
-        },
-    ),
-    (
-        "37.潘星.智慧图书馆联盟建设策略研究:学位论文.扬州:扬州大学,2021",
-        {
-            "type": "thesis",
-            "author": "潘星",
-            "title": "智慧图书馆联盟建设策略研究",
-            "source": "扬州:扬州大学",
-            "year": "2021",
-        },
-    ),
-    (
-        "12.王伟健.一个来了还想再来的图书馆.人民日报.1.7(11)",
-        {
-            "type": "newspaper",
-            "author": "王伟健",
-            "title": "一个来了还想再来的图书馆",
-            "source": "人民日报",
-            "date": "1.7",
-        },
-    ),
-    (
-        "25.一种用于图书馆机器人的书本上架装置.CN202880264U",
-        {
-            "type": "patent",
-            "title": "一种用于图书馆机器人的书本上架装置",
-            "identifier": "CN202880264U",
-        },
-    ),
-    (
-        "10.一种基于RFID标签RSSI信号值的图书排序方法:201610050963.1.2016-01-25",
-        {
-            "type": "patent",
-            "title": "一种基于RFID标签RSSI信号值的图书排序方法",
-            "identifier": "201610050963.1",
-        },
-    ),
-    (
-        "33.司莉.科学数据的标准规范体系框架研究.图书馆.2016.(5)",
-        {
-            "type": "journal",
-            "author": "司莉",
-            "title": "科学数据的标准规范体系框架研究",
-            "source": "图书馆",
-            "year": "2016",
-            "volume": None,
-            "issue": "5",
-        },
-    ),
-    (
-        "18.Ahirwar,J..Five Laws of Library Science and Information Economics.Informatics Studies.2021.7(1)",
-        {
-            "type": "english-paper",
-            "author": "Ahirwar,J.",
-            "title": "Five Laws of Library Science and Information Economics",
-            "source": "Informatics Studies",
-            "year": "2021",
-            "volume": "7",
-            "issue": "1",
-        },
-    ),
-]
-
-
-@pytest.mark.parametrize("input, expected", test_clean_data)
-def test_clean(input, expected):
-    assert ParseCssci.clean(input) == expected
-
-
-@pytest.mark.parametrize("input, expected", test_web_data)
-def test_parse_web(input, expected):
-    assert ParseCssci(input).parse_web() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_standard_data)
-def test_parse_standard(input, expected):
-    assert ParseCssci(input).parse_standard() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_book_data)
-def test_parse_book(input, expected):
-    assert ParseCssci(input).parse_book() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_thesis_data)
-def test_parse_thesis(input, expected):
-    assert ParseCssci(input).parse_thesis() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_newspaper_data)
-def test_parse_newspaper(input, expected):
-    assert ParseCssci(input).parse_newspaper() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_patent1_data)
-def test_parse_patent1(input, expected):
-    assert ParseCssci(input).parse_patent1() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_patent2_data)
-def test_parse_patent2(input, expected):
-    assert ParseCssci(input).parse_patent2() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_journal_data)
-def test_parse_journal(input, expected):
-    assert ParseCssci(input).parse_journal() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_english_data)
-def test_parse_english(input, expected):
-    assert ParseCssci(input).parse_english() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_parse_data)
-def test_parse_parse(input, expected):
-    assert ParseCssci(input).parse() == expected
+import pytest
+
+from refparse.cssci import ParseCssci
+
+test_clean_data = [
+    (
+        "1.康德.纯粹理性批判.北京:人民出版社",
+        "康德.纯粹理性批判.北京:人民出版社",
+    ),
+    (
+        "7..中华人民共和国公共图书馆法.2021",
+        ".中华人民共和国公共图书馆法.2021",
+    ),
+]
+
+test_web_data = [
+    (
+        "8.Google.Analytics.js.2021",
+        {
+            "type": "web",
+            "author": "Google",
+            "title": "Analytics.js",
+            "year": "2021",
+        },
+    ),
+    (
+        "9..CNNIC:微博用户达2.5亿，近半数网民使用.2012",
+        {
+            "type": "web",
+            "author": None,
+            "title": "CNNIC:微博用户达25亿，近半数网民使用2012",
+            "year": "2012",
+        },
+    ),
+    (
+        "22.IFLA.IFLA STRATEGY 2019-2024.2019",
+        {
+            "type": "web",
+            "author": "IFLA",
+            "title": "IFLA STRATEGY 2019-2024",
+            "year": "2019",
+        },
+    ),
+]
+
+test_standard_data = [
+    (
+        "8..GB/T37043-2018，智慧城市术语.北京:中国标准出版社",
+        {
+            "type": "standard",
+            "author": None,
+            "title": "智慧城市术语",
+            "source": "北京:中国标准出版社",
+            "year": None,
+            "identifier": "GB/T37043-2018",
+        },
+    ),
+    (
+        "17.全国信息技术标准化技术委员会教育技术分会.GB/T 36342-2018,智慧校园总体框架,2018",
+        {
+            "type": "standard",
+            "author": "全国信息技术标准化技术委员会教育技术分会",
+            "title": "智慧校园总体框架",
+            "source": None,
+            "year": "2018",
+            "identifier": "GB/T 36342-2018",
+        },
+    ),
+    (
+        "30.全国信息技术标准化技术委员会.智慧城市，数据融合，第5部分:市政基础设施数据元素:GB/T 36625.5-2019.北京:中国标准出版社",
+        {
+            "type": "standard",
+            "author": "全国信息技术标准化技术委员会",
+            "title": "智慧城市，数据融合，第5部分:市政基础设施数据元素",
+            "source": "北京:中国标准出版社",
+            "year": None,
+            "identifier": "GB/T 36625.5-2019",
+        },
+    ),
+]
+
+test_book_data = [
+    (
+        "14.吴建中.21世纪图书馆新论.上海:上海科学技术文献出版社",
+        {
+            "type": "book",
+            "author": "吴建中",
+            "title": "21世纪图书馆新论",
+            "source": "上海:上海科学技术文献出版社",
+        },
+    ),
+    (
+        "3.金元浦.中国文化概论.北京:首都师范大学出版社",
+        {
+            "type": "book",
+            "author": "金元浦",
+            "title": "中国文化概论",
+            "source": "北京:首都师范大学出版社",
+        },
+    ),
+]
+
+test_thesis_data = [
+    (
+        "21.郑怿昕.智慧图书馆环境下馆员核心能力研究:学位论文.南京:南京农业大学,2015:27-31",
+        {
+            "type": "thesis",
+            "author": "郑怿昕",
+            "title": "智慧图书馆环境下馆员核心能力研究",
+            "source": "南京:南京农业大学",
+            "year": "2015",
+        },
+    ),
+    (
+        "17.段美珍.智慧图书馆建设评价模型与应用研究:学位论文.北京:中国科学院大学,2020",
+        {
+            "type": "thesis",
+            "author": "段美珍",
+            "title": "智慧图书馆建设评价模型与应用研究",
+            "source": "北京:中国科学院大学",
+            "year": "2020",
+        },
+    ),
+]
+
+test_newspaper_data = [
+    (
+        "6..习近平在第二届世界互联网大会开幕式上的讲话.人民日报.12.17(2)",
+        {
+            "type": "newspaper",
+            "author": None,
+            "title": "习近平在第二届世界互联网大会开幕式上的讲话",
+            "source": "人民日报",
+            "date": "12.17",
+        },
+    ),
+    (
+        "25.曹磊.大数据:数字世界的智慧基因.文汇报.11.8(12)",
+        {
+            "type": "newspaper",
+            "author": "曹磊",
+            "title": "大数据:数字世界的智慧基因",
+            "source": "文汇报",
+            "date": "11.8",
+        },
+    ),
+    (
+        "65..图书馆来了机器人管理员.宁波日报.1.8",
+        {
+            "type": "newspaper",
+            "author": None,
+            "title": "图书馆来了机器人管理员",
+            "source": "宁波日报",
+            "date": "1.8",
+        },
+    ),
+]
+
+test_patent1_data = [
+    (
+        "26.图书上下架机器人.CN102152293A",
+        {
+            "type": "patent",
+            "title": "图书上下架机器人",
+            "identifier": "CN102152293A",
+        },
+    )
+]
+test_patent2_data = [
+    (
+        "9.一种基于RFID技术的自动式图书智能盘点机器人:201620075212.0.2016-01-25",
+        {
+            "type": "patent",
+            "title": "一种基于RFID技术的自动式图书智能盘点机器人",
+            "identifier": "201620075212.0",
+        },
+    ),
+    (
+        "39.一种基于区块链的金融安全存证平台系统及方法:中国，201910838935. X(2019-09-05)",
+        {
+            "type": "patent",
+            "title": "一种基于区块链的金融安全存证平台系统及方法",
+            "identifier": "201910838935",
+        },
+    ),
+]
+
+
+test_paper_data = [
+    (
+        "2.严栋.基于物联网的智慧图书馆.图书馆学刊.2010.32(7)",
+        {
+            "type": "paper",
+            "author": "严栋",
+            "title": "基于物联网的智慧图书馆",
+            "source": "图书馆学刊",
+            "year": "2010",
+            "volume": "32",
+            "issue": "7",
+        },
+    ),
+    (
+        "39.刘炜.5G与智慧图书馆建设.中国图书馆学报.2019.45(5)",
+        {
+            "type": "paper",
+            "author": "刘炜",
+            "title": "5G与智慧图书馆建设",
+            "source": "中国图书馆学报",
+            "year": "2019",
+            "volume": "45",
+            "issue": "5",
+        },
+    ),
+]
+
+test_english_data = [
+    (
+        "20.Alexei,P..Rite of passage.USA:Galaxy Publishing Co",
+        {
+            "type": "english-book",
+            "author": "Alexei,P.",
+            "title": "Rite of passage",
+            "source": "USA:Galaxy Publishing Co",
+            "year": None,
+            "page": None,
+        },
+    ),
+    (
+        "8.Sohail,S S.Book recommendation system using opinion mining technique:IEEE,2013:1609-1614",
+        {
+            "type": "english-book",
+            "author": "Sohail,S S",
+            "title": "Book recommendation system using opinion mining technique",
+            "source": "IEEE",
+            "year": "2013",
+            "page": "1609-1614",
+        },
+    ),
+    (
+        "7.Vaz,P C.Improving a hybrid literary book recommendation system through author ranking.New York:Association for Computing Machinery,2012:387-388",
+        {
+            "type": "english-book",
+            "author": "Vaz,P C",
+            "title": "Improving a hybrid literary book recommendation system through author ranking",
+            "source": "New York:Association for Computing Machinery",
+            "year": "2012",
+            "page": "387-388",
+        },
+    ),
+    (
+        "7.Hunzaker,M.B. Fallin.Mapping Cultural Schemas: From Theory to Method.American Sociological Review.2019.84(5)",
+        {
+            "type": "english-paper",
+            "author": "Hunzaker,M.B. Fallin",
+            "title": "Mapping Cultural Schemas: From Theory to Method",
+            "source": "American Sociological Review",
+            "year": "2019",
+            "volume": "84",
+            "issue": "5",
+        },
+    ),
+    (
+        "1.Aittola,M..Smart Library: Location-Aware Mobile Library Service.International Symposium on Human Computer Interaction with Mobile Devices and Services.2003.(5)",
+        {
+            "type": "english-paper",
+            "author": "Aittola,M.",
+            "title": "Smart Library: Location-Aware Mobile Library Service",
+            "source": "International Symposium on Human Computer Interaction with Mobile Devices and Services",
+            "year": "2003",
+            "volume": None,
+            "issue": "5",
+        },
+    ),
+]
+
+test_parse_data = [
+    (
+        "3..2021第五届中国未来智慧图书馆发展论坛.2021",
+        {
+            "type": "web",
+            "author": None,
+            "title": "2021第五届中国未来智慧图书馆发展论坛",
+            "year": "2021",
+        },
+    ),
+    (
+        "10..GB/T 35273-2020，信息安全技术个人信息安全规范",
+        {
+            "type": "standard",
+            "author": None,
+            "title": "信息安全技术个人信息安全规范",
+            "source": None,
+            "year": None,
+            "identifier": "GB/T 35273-2020",
+        },
+    ),
+    (
+        "14.吴慰慈.图书馆学概论.北京:北京图书馆出版社",
+        {
+            "type": "book",
+            "author": "吴慰慈",
+            "title": "图书馆学概论",
+            "source": "北京:北京图书馆出版社",
+        },
+    ),
+    (
+        "37.潘星.智慧图书馆联盟建设策略研究:学位论文.扬州:扬州大学,2021",
+        {
+            "type": "thesis",
+            "author": "潘星",
+            "title": "智慧图书馆联盟建设策略研究",
+            "source": "扬州:扬州大学",
+            "year": "2021",
+        },
+    ),
+    (
+        "12.王伟健.一个来了还想再来的图书馆.人民日报.1.7(11)",
+        {
+            "type": "newspaper",
+            "author": "王伟健",
+            "title": "一个来了还想再来的图书馆",
+            "source": "人民日报",
+            "date": "1.7",
+        },
+    ),
+    (
+        "25.一种用于图书馆机器人的书本上架装置.CN202880264U",
+        {
+            "type": "patent",
+            "title": "一种用于图书馆机器人的书本上架装置",
+            "identifier": "CN202880264U",
+        },
+    ),
+    (
+        "10.一种基于RFID标签RSSI信号值的图书排序方法:201610050963.1.2016-01-25",
+        {
+            "type": "patent",
+            "title": "一种基于RFID标签RSSI信号值的图书排序方法",
+            "identifier": "201610050963.1",
+        },
+    ),
+    (
+        "33.司莉.科学数据的标准规范体系框架研究.图书馆.2016.(5)",
+        {
+            "type": "paper",
+            "author": "司莉",
+            "title": "科学数据的标准规范体系框架研究",
+            "source": "图书馆",
+            "year": "2016",
+            "volume": None,
+            "issue": "5",
+        },
+    ),
+    (
+        "18.Ahirwar,J..Five Laws of Library Science and Information Economics.Informatics Studies.2021.7(1)",
+        {
+            "type": "english-paper",
+            "author": "Ahirwar,J.",
+            "title": "Five Laws of Library Science and Information Economics",
+            "source": "Informatics Studies",
+            "year": "2021",
+            "volume": "7",
+            "issue": "1",
+        },
+    ),
+]
+
+
+@pytest.mark.parametrize("input, expected", test_clean_data)
+def test_clean(input, expected):
+    assert ParseCssci.clean(input) == expected
+
+
+@pytest.mark.parametrize("input, expected", test_web_data)
+def test_parse_web(input, expected):
+    assert ParseCssci(input).parse_web() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_standard_data)
+def test_parse_standard(input, expected):
+    assert ParseCssci(input).parse_standard() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_book_data)
+def test_parse_book(input, expected):
+    assert ParseCssci(input).parse_book() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_thesis_data)
+def test_parse_thesis(input, expected):
+    assert ParseCssci(input).parse_thesis() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_newspaper_data)
+def test_parse_newspaper(input, expected):
+    assert ParseCssci(input).parse_newspaper() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_patent1_data)
+def test_parse_patent1(input, expected):
+    assert ParseCssci(input).parse_patent1() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_patent2_data)
+def test_parse_patent2(input, expected):
+    assert ParseCssci(input).parse_patent2() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_paper_data)
+def test_parse_paper(input, expected):
+    assert ParseCssci(input).parse_paper() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_english_data)
+def test_parse_english(input, expected):
+    assert ParseCssci(input).parse_english() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_parse_data)
+def test_parse_parse(input, expected):
+    assert ParseCssci(input).parse() == expected
```

### Comparing `refparse-0.3.0/tests/test_wos.py` & `refparse-0.4.0/tests/test_wos.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,275 +1,270 @@
-import pytest
-
-from refparse.wos import ParseWos
-
-test_doi_data = [
-    (
-        "Yao J, 2008, SCIENCE, V321, P930, DOI 10.1126/science.1157566",
-        "10.1126/science.1157566",
-    ),
-    (
-        "Jiang HM, 2017, NAT CHEM BIOL, V13, P994, DOI [10.1038/NCHEMBIO.2442, 10.1038/nchembio.2442]",
-        "10.1038/nchembio.2442",
-    ),
-    (
-        "Du K-K., 2013, J CHINA U POSTS TELE, V20, P96, DOI DOI 10.1016/S1005-8885(13)60240-X",
-        "10.1016/s1005-8885(13)60240-x",
-    ),
-]
-
-test_page_data = [
-    (
-        "Habibi M, 2017, BIOINFORMATICS, V33, pI37, DOI 10.1093/bioinformatics/btx228",
-        "I37",
-    ),
-    (
-        "Vaswani A., 2017, ADV NEURAL INFORM PR, P30",
-        "30",
-    ),
-]
-
-test_volume_data = [
-    (
-        "Habibi M, 2017, BIOINFORMATICS, V33, pI37, DOI 10.1093/bioinformatics/btx228",
-        "33",
-    ),
-    (
-        "Krallinger M., 2015, J CHEMINFORM, V7",
-        "7",
-    ),
-    (
-        "Berg B.L., 2009, QUALITATIVE RES METH, V7th",
-        "7th",
-    ),
-    (
-        "Lefebvre C., 2019, COCHRANE HDB SYSTEMA, V2nd ed., P67",
-        "2nd ed.",
-    ),
-    (
-        "Schmidt V., 1979, SEPM (Soc. Sediment. Geol.) Spec. Publ., VVolume 26, P175",
-        "26",
-    ),
-    (
-        "WILLIAMS RS, 1995, ANNALS OF GLACIOLOGY, VOL 21, 1995, P284",
-        "21",
-    ),
-]
-
-test_general_data = [
-    (
-        "Morin F., AISTATS 2005",
-        {
-            "author": "Morin F.",
-            "year": None,
-            "source": "AISTATS 2005",
-            "volume": None,
-            "page": None,
-            "doi": None,
-        },
-    ),
-    (
-        "Boden Mikael, 2001, DALLAS PROJECT",
-        {
-            "author": "Boden Mikael",
-            "year": "2001",
-            "source": "DALLAS PROJECT",
-            "volume": None,
-            "page": None,
-            "doi": None,
-        },
-    ),
-    (
-        "Bengio Yoshua, IEEE T NEURAL NETWOR, V5, P157",
-        {
-            "author": "Bengio Yoshua",
-            "year": None,
-            "source": "IEEE T NEURAL NETWOR",
-            "volume": "5",
-            "page": "157",
-            "doi": None,
-        },
-    ),
-    (
-        "Rajpurkar P., 2016, PROC C EMPIRICAL MET, V2016, P2383, DOI DOI 10.18653/V1/D16-1264",
-        {
-            "author": "Rajpurkar P.",
-            "year": "2016",
-            "source": "PROC C EMPIRICAL MET",
-            "volume": "2016",
-            "page": "2383",
-            "doi": "10.18653/v1/d16-1264",
-        },
-    ),
-]
-
-test_bilingual_data = [
-    (
-        {
-            "ref": "Poggio Tomaso, 2017, [International Journal of Automation and Computing, 国际自动化与计算杂志], V14, P503"
-        },
-        {
-            "author": "Poggio Tomaso",
-            "year": "2017",
-            "source": "International Journal of Automation and Computing",
-            "volume": "14",
-            "page": "503",
-            "doi": None,
-        },
-    ),
-    (
-        {
-            "ref": "Kim Kyung Ja, 2019, [English Teaching, 영어교육], V74, P249",
-        },
-        {
-            "author": "Kim Kyung Ja",
-            "year": "2019",
-            "source": "English Teaching",
-            "volume": "74",
-            "page": "249",
-            "doi": None,
-        },
-    ),
-    (
-        {
-            "ref": "[Fang Tiegang 方铁钢], 2017, [汽车安全与节能学报, Journal of Automotive Safety and Energy], V8, P226",
-        },
-        {
-            "author": "Fang Tiegang",
-            "year": "2017",
-            "source": "Journal of Automotive Safety and Energy",
-            "volume": "8",
-            "page": "226",
-            "doi": None,
-        },
-    ),
-    (
-        {
-            "ref": "张海亭, 2009, [计算机系统应用, Computer Systems & Applications], V18, P1",
-        },
-        {
-            "author": None,
-            "year": "2009",
-            "source": "Computer Systems & Applications",
-            "volume": "18",
-            "page": "1",
-            "doi": None,
-        },
-    ),
-    (
-        {
-            "ref": "[赵丽晓 Zhao Lixiao], 2014, [作物杂志, Crops], P6",
-            "keep_eng_result": False,
-        },
-        {
-            "author": "赵丽晓",
-            "year": "2014",
-            "source": "作物杂志",
-            "volume": None,
-            "page": "6",
-            "doi": None,
-        },
-    ),
-]
-
-test_patent_data = [
-    (
-        "Fan P., 2011, PT, Patent No. 2011163640",
-        {
-            "author": "Fan P.",
-            "year": "2011",
-            "title": None,
-            "identifier": "2011163640",
-        },
-    ),
-    (
-        "Redlich R. M., 2006, U. S. Patent, Patent No. [7,103,915, 7103915]",
-        {
-            "author": "Redlich R. M.",
-            "year": "2006",
-            "title": None,
-            "identifier": "7103915",
-        },
-    ),
-    (
-        "Watanabe K., 1995, Low calorie foodstuff, aqueous paste composition, as well as production process thereof, Patent No. 5690981A",
-        {
-            "author": "Watanabe K.",
-            "year": "1995",
-            "title": "Low calorie foodstuff, aqueous paste composition, as well as production process thereof",
-            "identifier": "5690981A",
-        },
-    ),
-]
-
-test_parse_data = [
-    (
-        "[Anonymous], 2017, NATURE, DOI DOI 10.1038/NATURE.2017.22094",
-        None,
-    ),
-    (
-        "Dodd SK., 2013, Patent No. 2013/171639 A1",
-        {
-            "author": "Dodd SK.",
-            "identifier": "2013/171639 A1",
-            "title": None,
-            "year": "2013",
-        },
-    ),
-    (
-        "[张铁华 Zhang Tiehua], 2011, [吉林大学学报. 工学版, Journal of Jilin University. Engineering and Technology Edition], V41, P882",
-        {
-            "author": "Zhang Tiehua",
-            "year": "2011",
-            "source": "Journal of Jilin University. Engineering and Technology Edition",
-            "volume": "41",
-            "page": "882",
-            "doi": None,
-        },
-    ),
-    (
-        "Wang X, 2019, BIOINFORMATICS, V35, P1745, DOI 10.1093/bioinformatics/bty869",
-        {
-            "author": "Wang X",
-            "year": "2019",
-            "source": "BIOINFORMATICS",
-            "volume": "35",
-            "page": "1745",
-            "doi": "10.1093/bioinformatics/bty869",
-        },
-    ),
-]
-
-
-@pytest.mark.parametrize("input, expected", test_doi_data)
-def test_extract_doi(input, expected):
-    assert ParseWos.extract_doi(input) == expected
-
-
-@pytest.mark.parametrize("input, expected", test_page_data)
-def test_extract_page(input, expected):
-    assert ParseWos.extract_page(input) == expected
-
-
-@pytest.mark.parametrize("input, expected", test_volume_data)
-def test_extract_volume(input, expected):
-    assert ParseWos.extract_volume(input) == expected
-
-
-@pytest.mark.parametrize("input, expected", test_general_data)
-def test_parse_general(input, expected):
-    assert ParseWos(input).parse_general() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_bilingual_data)
-def test_parse_bilingual(input, expected):
-    assert ParseWos(**input).parse_bilingual() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_patent_data)
-def test_parse_patent(input, expected):
-    assert ParseWos(input).parse_patent() == expected
-
-
-@pytest.mark.parametrize("input, expected", test_parse_data)
-def test_parse(input, expected):
-    assert ParseWos(input).parse() == expected
+import pytest
+
+from refparse.wos import ParseWos
+
+test_doi_data = [
+    (
+        "Yao J, 2008, SCIENCE, V321, P930, DOI 10.1126/science.1157566",
+        "10.1126/science.1157566",
+    ),
+    (
+        "Jiang HM, 2017, NAT CHEM BIOL, V13, P994, DOI [10.1038/NCHEMBIO.2442, 10.1038/nchembio.2442]",
+        "10.1038/nchembio.2442",
+    ),
+    (
+        "Du K-K., 2013, J CHINA U POSTS TELE, V20, P96, DOI DOI 10.1016/S1005-8885(13)60240-X",
+        "10.1016/s1005-8885(13)60240-x",
+    ),
+]
+
+test_page_data = [
+    (
+        "Habibi M, 2017, BIOINFORMATICS, V33, pI37, DOI 10.1093/bioinformatics/btx228",
+        "I37",
+    ),
+    (
+        "Vaswani A., 2017, ADV NEURAL INFORM PR, P30",
+        "30",
+    ),
+]
+
+test_volume_data = [
+    (
+        "Habibi M, 2017, BIOINFORMATICS, V33, pI37, DOI 10.1093/bioinformatics/btx228",
+        "33",
+    ),
+    (
+        "Krallinger M., 2015, J CHEMINFORM, V7",
+        "7",
+    ),
+    (
+        "Berg B.L., 2009, QUALITATIVE RES METH, V7th",
+        "7th",
+    ),
+    (
+        "Lefebvre C., 2019, COCHRANE HDB SYSTEMA, V2nd ed., P67",
+        "2nd ed.",
+    ),
+    (
+        "Schmidt V., 1979, SEPM (Soc. Sediment. Geol.) Spec. Publ., VVolume 26, P175",
+        "26",
+    ),
+    (
+        "WILLIAMS RS, 1995, ANNALS OF GLACIOLOGY, VOL 21, 1995, P284",
+        "21",
+    ),
+]
+
+test_general_data = [
+    (
+        "Morin F., AISTATS 2005",
+        {
+            "author": "Morin F.",
+            "year": None,
+            "source": "AISTATS 2005",
+            "volume": None,
+            "page": None,
+            "doi": None,
+        },
+    ),
+    (
+        "Boden Mikael, 2001, DALLAS PROJECT",
+        {
+            "author": "Boden Mikael",
+            "year": "2001",
+            "source": "DALLAS PROJECT",
+            "volume": None,
+            "page": None,
+            "doi": None,
+        },
+    ),
+    (
+        "Bengio Yoshua, IEEE T NEURAL NETWOR, V5, P157",
+        {
+            "author": "Bengio Yoshua",
+            "year": None,
+            "source": "IEEE T NEURAL NETWOR",
+            "volume": "5",
+            "page": "157",
+            "doi": None,
+        },
+    ),
+    (
+        "Rajpurkar P., 2016, PROC C EMPIRICAL MET, V2016, P2383, DOI DOI 10.18653/V1/D16-1264",
+        {
+            "author": "Rajpurkar P.",
+            "year": "2016",
+            "source": "PROC C EMPIRICAL MET",
+            "volume": "2016",
+            "page": "2383",
+            "doi": "10.18653/v1/d16-1264",
+        },
+    ),
+]
+
+test_bilingual_data = [
+    (
+        {
+            "ref": "Poggio Tomaso, 2017, [International Journal of Automation and Computing, 国际自动化与计算杂志], V14, P503"
+        },
+        {
+            "author": "Poggio Tomaso",
+            "year": "2017",
+            "source": "International Journal of Automation and Computing",
+            "volume": "14",
+            "page": "503",
+            "doi": None,
+        },
+    ),
+    (
+        {
+            "ref": "Kim Kyung Ja, 2019, [English Teaching, 영어교육], V74, P249",
+        },
+        {
+            "author": "Kim Kyung Ja",
+            "year": "2019",
+            "source": "English Teaching",
+            "volume": "74",
+            "page": "249",
+            "doi": None,
+        },
+    ),
+    (
+        {
+            "ref": "[Fang Tiegang 方铁钢], 2017, [汽车安全与节能学报, Journal of Automotive Safety and Energy], V8, P226",
+        },
+        {
+            "author": "Fang Tiegang",
+            "year": "2017",
+            "source": "Journal of Automotive Safety and Energy",
+            "volume": "8",
+            "page": "226",
+            "doi": None,
+        },
+    ),
+    (
+        {
+            "ref": "张海亭, 2009, [计算机系统应用, Computer Systems & Applications], V18, P1",
+        },
+        {
+            "author": None,
+            "year": "2009",
+            "source": "Computer Systems & Applications",
+            "volume": "18",
+            "page": "1",
+            "doi": None,
+        },
+    ),
+    (
+        {
+            "ref": "[赵丽晓 Zhao Lixiao], 2014, [作物杂志, Crops], P6",
+            "keep_eng_result": False,
+        },
+        {
+            "author": "赵丽晓",
+            "year": "2014",
+            "source": "作物杂志",
+            "volume": None,
+            "page": "6",
+            "doi": None,
+        },
+    ),
+]
+
+test_patent_data = [
+    (
+        "Fan P., 2011, PT, Patent No. 2011163640",
+        {
+            "author": "Fan P.",
+            "year": "2011",
+            "title": None,
+            "identifier": "2011163640",
+        },
+    ),
+    (
+        "Redlich R. M., 2006, U. S. Patent, Patent No. [7,103,915, 7103915]",
+        {
+            "author": "Redlich R. M.",
+            "year": "2006",
+            "title": None,
+            "identifier": "7103915",
+        },
+    ),
+    (
+        "Watanabe K., 1995, Low calorie foodstuff, aqueous paste composition, as well as production process thereof, Patent No. 5690981A",
+        {
+            "author": "Watanabe K.",
+            "year": "1995",
+            "title": "Low calorie foodstuff, aqueous paste composition, as well as production process thereof",
+            "identifier": "5690981A",
+        },
+    ),
+]
+
+test_parse_data = [
+    (
+        "[Anonymous], 2017, NATURE, DOI DOI 10.1038/NATURE.2017.22094",
+        None,
+    ),
+    (
+        "Dodd SK., 2013, Patent No. 2013/171639 A1",
+        None,
+    ),
+    (
+        "[张铁华 Zhang Tiehua], 2011, [吉林大学学报. 工学版, Journal of Jilin University. Engineering and Technology Edition], V41, P882",
+        {
+            "author": "Zhang Tiehua",
+            "year": "2011",
+            "source": "Journal of Jilin University. Engineering and Technology Edition",
+            "volume": "41",
+            "page": "882",
+            "doi": None,
+        },
+    ),
+    (
+        "Wang X, 2019, BIOINFORMATICS, V35, P1745, DOI 10.1093/bioinformatics/bty869",
+        {
+            "author": "Wang X",
+            "year": "2019",
+            "source": "BIOINFORMATICS",
+            "volume": "35",
+            "page": "1745",
+            "doi": "10.1093/bioinformatics/bty869",
+        },
+    ),
+]
+
+
+@pytest.mark.parametrize("input, expected", test_doi_data)
+def test_extract_doi(input, expected):
+    assert ParseWos.extract_doi(input) == expected
+
+
+@pytest.mark.parametrize("input, expected", test_page_data)
+def test_extract_page(input, expected):
+    assert ParseWos.extract_page(input) == expected
+
+
+@pytest.mark.parametrize("input, expected", test_volume_data)
+def test_extract_volume(input, expected):
+    assert ParseWos.extract_volume(input) == expected
+
+
+@pytest.mark.parametrize("input, expected", test_general_data)
+def test_parse_general(input, expected):
+    assert ParseWos(input).parse_general() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_bilingual_data)
+def test_parse_bilingual(input, expected):
+    assert ParseWos(**input).parse_bilingual() == expected
+
+
+# @pytest.mark.parametrize("input, expected", test_patent_data)
+# def test_parse_patent(input, expected):
+#     assert ParseWos(input).parse_patent() == expected
+
+
+@pytest.mark.parametrize("input, expected", test_parse_data)
+def test_parse(input, expected):
+    assert ParseWos(input).parse() == expected
```

