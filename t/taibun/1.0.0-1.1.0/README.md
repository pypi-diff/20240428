# Comparing `tmp/taibun-1.0.0.tar.gz` & `tmp/taibun-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taibun-1.0.0.tar", last modified: Thu Aug 31 11:28:53 2023, max compression
+gzip compressed data, was "taibun-1.1.0.tar", last modified: Sun Apr 28 02:27:08 2024, max compression
```

## Comparing `taibun-1.0.0.tar` & `taibun-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-31 11:28:53.746690 taibun-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 taibun-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    11807 2023-08-31 11:28:53.744995 taibun-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10703 2023-08-31 11:19:49.000000 taibun-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-31 11:28:53.747686 taibun-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-08-31 11:24:17.000000 taibun-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-31 11:28:53.664790 taibun-1.0.0/taibun/
--rw-rw-rw-   0        0        0       46 2023-08-30 07:27:59.000000 taibun-1.0.0/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-31 11:28:53.739908 taibun-1.0.0/taibun/data/
--rw-rw-rw-   0        0        0    17141 2023-07-04 08:45:02.000000 taibun-1.0.0/taibun/data/simplified.json
--rw-rw-rw-   0        0        0  1447833 2023-08-28 08:20:03.000000 taibun-1.0.0/taibun/data/words.json
--rw-rw-rw-   0        0        0    20441 2023-08-30 07:21:35.000000 taibun-1.0.0/taibun/data/zhuyin.json
--rw-rw-rw-   0        0        0    23049 2023-08-30 07:23:06.000000 taibun-1.0.0/taibun/taibun.py
-drwxrwxrwx   0        0        0        0 2023-08-31 11:28:53.713965 taibun-1.0.0/taibun.egg-info/
--rw-rw-rw-   0        0        0    11807 2023-08-31 11:28:53.000000 taibun-1.0.0/taibun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-08-31 11:28:53.000000 taibun-1.0.0/taibun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-31 11:28:53.000000 taibun-1.0.0/taibun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-31 11:28:53.000000 taibun-1.0.0/taibun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 02:27:08.258217 taibun-1.1.0/
+-rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 taibun-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    12997 2024-04-28 02:27:08.253634 taibun-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12204 2024-04-28 01:15:26.000000 taibun-1.1.0/README.md
+-rw-rw-rw-   0        0        0       50 2024-04-28 02:07:06.000000 taibun-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      875 2024-04-28 02:27:08.281891 taibun-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 02:27:08.187620 taibun-1.1.0/taibun/
+-rw-rw-rw-   0        0        0       85 2024-04-27 02:04:57.000000 taibun-1.1.0/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:27:08.235121 taibun-1.1.0/taibun/data/
+-rw-rw-rw-   0        0        0    17160 2024-04-27 02:06:10.000000 taibun-1.1.0/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0  1893344 2024-04-28 00:12:08.000000 taibun-1.1.0/taibun/data/words.json
+-rw-rw-rw-   0        0        0    25042 2024-04-28 00:18:10.000000 taibun-1.1.0/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:27:08.245254 taibun-1.1.0/taibun.egg-info/
+-rw-rw-rw-   0        0        0    12997 2024-04-28 02:27:08.000000 taibun-1.1.0/taibun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-04-28 02:27:08.000000 taibun-1.1.0/taibun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 02:27:08.000000 taibun-1.1.0/taibun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 02:27:08.000000 taibun-1.1.0/taibun.egg-info/top_level.txt
```

### Comparing `taibun-1.0.0/LICENSE` & `taibun-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taibun-1.0.0/PKG-INFO` & `taibun-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2074 6169  : 2.1..Name: tai
 00000020: 6275 6e0d 0a56 6572 7369 6f6e 3a20 312e  bun..Version: 1.
-00000030: 302e 300d 0a53 756d 6d61 7279 3a20 5461  0.0..Summary: Ta
+00000030: 312e 300d 0a53 756d 6d61 7279 3a20 5461  1.0..Summary: Ta
 00000040: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
 00000050: 5472 616e 736c 6974 6572 6174 6f72 2061  Transliterator a
 00000060: 6e64 2054 6f6b 656e 6973 6572 0d0a 486f  nd Tokeniser..Ho
 00000070: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000080: 2f67 6974 6875 622e 636f 6d2f 616e 6472  /github.com/andr
 00000090: 6569 6861 722f 7461 6962 756e 0d0a 4175  eihar/taibun..Au
 000000a0: 7468 6f72 3a20 416e 6472 6569 2048 6172  thor: Andrei Har
@@ -21,718 +21,793 @@
 00000140: 6e73 6c69 7465 7261 746f 722c 746f 6b65  nsliterator,toke
 00000150: 6e69 7a61 7469 6f6e 2c74 6f6b 656e 697a  nization,tokeniz
 00000160: 6572 0d0a 436c 6173 7369 6669 6572 3a20  er..Classifier: 
 00000170: 546f 7069 6320 3a3a 2054 6578 7420 5072  Topic :: Text Pr
 00000180: 6f63 6573 7369 6e67 203a 3a20 4c69 6e67  ocessing :: Ling
 00000190: 7569 7374 6963 0d0a 436c 6173 7369 6669  uistic..Classifi
 000001a0: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
-000001b0: 5374 6174 7573 203a 3a20 3320 2d20 416c  Status :: 3 - Al
-000001c0: 7068 610d 0a43 6c61 7373 6966 6965 723a  pha..Classifier:
-000001d0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-000001e0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-000001f0: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000220: 330d 0a43 6c61 7373 6966 6965 723a 204f  3..Classifier: O
-00000230: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000240: 3a3a 2055 6e69 780d 0a43 6c61 7373 6966  :: Unix..Classif
-00000250: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000260: 7973 7465 6d20 3a3a 204d 6163 4f53 203a  ystem :: MacOS :
-00000270: 3a20 4d61 634f 5320 580d 0a43 6c61 7373  : MacOS X..Class
-00000280: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000290: 2053 7973 7465 6d20 3a3a 204d 6963 726f   System :: Micro
-000002a0: 736f 6674 203a 3a20 5769 6e64 6f77 730d  soft :: Windows.
-000002b0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-000002c0: 3a20 3e3d 332e 370d 0a44 6573 6372 6970  : >=3.7..Descrip
-000002d0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-000002e0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-000002f0: 0d0a 4c69 6365 6e73 652d 4669 6c65 3a20  ..License-File: 
-00000300: 4c49 4345 4e53 450d 0a0d 0a0d 0a3c 212d  LICENSE......<!-
-00000310: 2d20 5052 4f4a 4543 5420 4c4f 474f 202d  - PROJECT LOGO -
-00000320: 2d3e 0d0d 0a3c 6272 202f 3e0d 0d0a 3c64  ->...<br />...<d
-00000330: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
-00000340: 223e 0d0d 0a20 203c 6120 6872 6566 3d22  ">...  <a href="
-00000350: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000360: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
-00000370: 6275 6e22 3e0d 0d0a 2020 2020 3c69 6d67  bun">...    <img
-00000380: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000390: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000003a0: 656e 742e 636f 6d2f 616e 6472 6569 6861  ent.com/andreiha
-000003b0: 722f 7461 6962 756e 2f6d 6169 6e2f 7265  r/taibun/main/re
-000003c0: 6164 6d65 2f6c 6f67 6f2e 706e 6722 2061  adme/logo.png" a
-000003d0: 6c74 3d22 4c6f 676f 2220 7769 6474 683d  lt="Logo" width=
-000003e0: 2239 3022 2068 6569 6768 743d 2238 3022  "90" height="80"
-000003f0: 3e0d 0d0a 2020 3c2f 613e 0d0d 0a20 200d  >...  </a>...  .
-00000400: 0d0a 2320 5461 6962 756e 0d0d 0a0d 0d0a  ..# Taibun......
-00000410: 0d0d 0a0d 0d0a 3c21 2d2d 2050 524f 4a45  ......<!-- PROJE
-00000420: 4354 2053 4849 454c 4453 202d 2d3e 0d0d  CT SHIELDS -->..
-00000430: 0a5b 215b 5465 7374 735d 5b74 6573 7473  .[![Tests][tests
-00000440: 2d62 6164 6765 5d5d 5b74 6573 7473 5d0d  -badge]][tests].
-00000450: 0d0a 5b21 5b43 6f6e 7472 6962 7574 6f72  ..[![Contributor
-00000460: 735d 5b63 6f6e 7472 6962 7574 6f72 732d  s][contributors-
-00000470: 6261 6467 655d 5d5b 636f 6e74 7269 6275  badge]][contribu
-00000480: 746f 7273 5d0d 0d0a 5b21 5b52 656c 6561  tors]...[![Relea
-00000490: 7365 5d5b 7265 6c65 6173 652d 6261 6467  se][release-badg
-000004a0: 655d 5d5b 7265 6c65 6173 655d 0d0d 0a5b  e]][release]...[
-000004b0: 215b 4c69 6365 6e63 655d 5b6c 6963 656e  ![Licence][licen
-000004c0: 6365 2d62 6164 6765 5d5d 5b6c 6963 656e  ce-badge]][licen
-000004d0: 6365 5d0d 0d0a 5b21 5b4c 696e 6b65 6449  ce]...[![LinkedI
-000004e0: 6e5d 5b6c 696e 6b65 6469 6e2d 6261 6467  n][linkedin-badg
-000004f0: 655d 5d5b 6c69 6e6b 6564 696e 5d0d 0d0a  e]][linkedin]...
-00000500: 0d0d 0a2a 2a54 6169 7761 6e65 7365 2048  ...**Taiwanese H
-00000510: 6f6b 6b69 656e 2054 7261 6e73 6c69 7465  okkien Translite
-00000520: 7261 746f 7220 616e 6420 546f 6b65 6e69  rator and Tokeni
-00000530: 7365 722a 2a0d 0d0a 0d0d 0a49 7420 6861  ser**......It ha
-00000540: 7320 6d65 7468 6f64 7320 7468 6174 2061  s methods that a
-00000550: 6c6c 6f77 2074 6f20 6375 7374 6f6d 6973  llow to customis
-00000560: 6520 7472 616e 736c 6974 6572 6174 696f  e transliteratio
-00000570: 6e20 616e 6420 7265 7472 6965 7665 2061  n and retrieve a
-00000580: 6e79 206e 6563 6573 7361 7279 2069 6e66  ny necessary inf
-00000590: 6f72 6d61 7469 6f6e 2061 626f 7574 2054  ormation about T
-000005a0: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
-000005b0: 2070 726f 6e75 6e63 6961 7469 6f6e 2e3c   pronunciation.<
-000005c0: 6272 202f 3e0d 0d0a 496e 636c 7564 6573  br />...Includes
-000005d0: 2077 6f72 6420 746f 6b65 6e69 7365 7220   word tokeniser 
-000005e0: 666f 7220 5461 6977 616e 6573 6520 486f  for Taiwanese Ho
-000005f0: 6b6b 6965 6e2e 0d0d 0a0d 0d0a 5b52 6570  kkien.......[Rep
-00000600: 6f72 7420 4275 675d 5b62 7567 5d20 e280  ort Bug][bug] ..
-00000610: a20d 0d0a 5b50 7950 495d 5b70 7970 695d  ....[PyPI][pypi]
-00000620: 0d0d 0a0d 0d0a 3c2f 6469 763e 0d0d 0a0d  ......</div>....
-00000630: 0d0a 0d0d 0a0d 0d0a 2d2d 2d0d 0d0a 0d0d  ........---.....
-00000640: 0a0d 0d0a 0d0d 0a3c 212d 2d20 5441 424c  .......<!-- TABL
-00000650: 4520 4f46 2043 4f4e 5445 4e54 5320 2d2d  E OF CONTENTS --
-00000660: 3e0d 0d0a 3c64 6574 6169 6c73 206f 7065  >...<details ope
-00000670: 6e3e 0d0d 0a20 203c 7375 6d6d 6172 793e  n>...  <summary>
-00000680: 5461 626c 6520 6f66 2043 6f6e 7465 6e74  Table of Content
-00000690: 733c 2f73 756d 6d61 7279 3e0d 0d0a 2020  s</summary>...  
-000006a0: 3c6f 6c3e 0d0d 0a20 2020 203c 6c69 3e3c  <ol>...    <li><
-000006b0: 6120 6872 6566 3d22 2369 6e73 7461 6c6c  a href="#install
-000006c0: 223e 496e 7374 616c 6c3c 2f61 3e3c 2f6c  ">Install</a></l
-000006d0: 693e 0d0d 0a20 2020 203c 6c69 3e0d 0d0a  i>...    <li>...
-000006e0: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
-000006f0: 7573 6167 6522 3e55 7361 6765 3c2f 613e  usage">Usage</a>
-00000700: 0d0d 0a20 2020 2020 203c 756c 3e0d 0d0a  ...      <ul>...
-00000710: 2020 2020 2020 2020 3c6c 693e 0d0d 0a20          <li>... 
-00000720: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
-00000730: 3d22 2363 6f6e 7665 7274 6572 223e 436f  ="#converter">Co
-00000740: 6e76 6572 7465 723c 2f61 3e0d 0d0a 2020  nverter</a>...  
-00000750: 2020 2020 2020 2020 3c75 6c3e 0d0d 0a20          <ul>... 
-00000760: 2020 2020 2020 2020 2020 203c 6c69 3e3c             <li><
-00000770: 6120 6872 6566 3d22 2373 7973 7465 6d22  a href="#system"
-00000780: 3e53 7973 7465 6d3c 2f61 3e3c 2f6c 693e  >System</a></li>
-00000790: 0d0d 0a20 2020 2020 2020 2020 2020 203c  ...            <
-000007a0: 6c69 3e3c 6120 6872 6566 3d22 2364 6961  li><a href="#dia
-000007b0: 6c65 6374 223e 4469 616c 6563 743c 2f61  lect">Dialect</a
-000007c0: 3e3c 2f6c 693e 0d0d 0a20 2020 2020 2020  ></li>...       
-000007d0: 2020 2020 203c 6c69 3e3c 6120 6872 6566       <li><a href
-000007e0: 3d22 2366 6f72 6d61 7422 3e46 6f72 6d61  ="#format">Forma
-000007f0: 743c 2f61 3e3c 2f6c 693e 0d0d 0a20 2020  t</a></li>...   
-00000800: 2020 2020 2020 2020 203c 6c69 3e3c 6120           <li><a 
-00000810: 6872 6566 3d22 2364 656c 696d 6974 6572  href="#delimiter
-00000820: 223e 4465 6c69 6d69 7465 723c 2f61 3e3c  ">Delimiter</a><
-00000830: 2f6c 693e 0d0d 0a20 2020 2020 2020 2020  /li>...         
-00000840: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-00000850: 2373 616e 6468 6922 3e53 616e 6468 693c  #sandhi">Sandhi<
-00000860: 2f61 3e3c 2f6c 693e 0d0d 0a20 2020 2020  /a></li>...     
-00000870: 2020 2020 2020 203c 6c69 3e3c 6120 6872         <li><a hr
-00000880: 6566 3d22 2370 756e 6374 7561 7469 6f6e  ef="#punctuation
-00000890: 223e 5075 6e63 7475 6174 696f 6e3c 2f61  ">Punctuation</a
-000008a0: 3e3c 2f6c 693e 0d0d 0a20 2020 2020 2020  ></li>...       
-000008b0: 2020 203c 2f75 6c3e 0d0d 0a20 2020 2020     </ul>...     
-000008c0: 2020 203c 2f6c 693e 0d0d 0a20 2020 2020     </li>...     
-000008d0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-000008e0: 2374 6f6b 656e 6973 6572 223e 546f 6b65  #tokeniser">Toke
-000008f0: 6e69 7365 723c 2f61 3e3c 2f6c 693e 0d0d  niser</a></li>..
-00000900: 0a20 2020 2020 203c 2f75 6c3e 0d0d 0a20  .      </ul>... 
-00000910: 2020 203c 2f6c 693e 0d0d 0a20 2020 203c     </li>...    <
-00000920: 6c69 3e3c 6120 6872 6566 3d22 2365 7861  li><a href="#exa
-00000930: 6d70 6c65 223e 4578 616d 706c 653c 2f61  mple">Example</a
-00000940: 3e3c 2f6c 693e 0d0d 0a20 2020 203c 6c69  ></li>...    <li
-00000950: 3e3c 6120 6872 6566 3d22 2364 6174 6122  ><a href="#data"
-00000960: 3e44 6174 613c 2f61 3e3c 2f6c 693e 0d0d  >Data</a></li>..
-00000970: 0a20 2020 203c 6c69 3e3c 6120 6872 6566  .    <li><a href
-00000980: 3d22 236c 6963 656e 6365 223e 4c69 6365  ="#licence">Lice
-00000990: 6e63 653c 2f61 3e3c 2f6c 693e 0d0d 0a20  nce</a></li>... 
-000009a0: 203c 2f6f 6c3e 0d0d 0a3c 2f64 6574 6169   </ol>...</detai
-000009b0: 6c73 3e0d 0d0a 0d0d 0a0d 0d0a 0d0d 0a3c  ls>............<
-000009c0: 212d 2d20 494e 5354 414c 4c20 2d2d 3e0d  !-- INSTALL -->.
-000009d0: 0d0a 2323 2049 6e73 7461 6c6c 0d0d 0a0d  ..## Install....
-000009e0: 0d0a 5461 6962 756e 2063 616e 2062 6520  ..Taibun can be 
-000009f0: 696e 7374 616c 6c65 6420 6672 6f6d 205b  installed from [
-00000a00: 7079 7069 5d5b 7079 7069 5d0d 0d0a 0d0d  pypi][pypi].....
-00000a10: 0a60 6060 6261 7368 0d0d 0a24 2070 6970  .```bash...$ pip
-00000a20: 2069 6e73 7461 6c6c 2074 6169 6275 6e0d   install taibun.
-00000a30: 0d0a 6060 600d 0d0a 0d0d 0a0d 0d0a 0d0d  ..```...........
-00000a40: 0a3c 212d 2d20 5553 4147 4520 2d2d 3e0d  .<!-- USAGE -->.
-00000a50: 0d0a 2323 2055 7361 6765 0d0d 0a0d 0d0a  ..## Usage......
-00000a60: 2323 2320 436f 6e76 6572 7465 720d 0d0a  ### Converter...
-00000a70: 0d0d 0a60 436f 6e76 6572 7465 7260 2063  ...`Converter` c
-00000a80: 6c61 7373 2074 7261 6e73 6c69 7465 7261  lass translitera
-00000a90: 7465 7320 7468 6520 4368 696e 6573 6520  tes the Chinese 
-00000aa0: 6368 6172 6163 7465 7273 2074 6f20 7468  characters to th
-00000ab0: 6520 6368 6f73 656e 2074 7261 6e73 6c69  e chosen transli
-00000ac0: 7465 7261 7469 6f6e 2073 7973 7465 6d20  teration system 
-00000ad0: 7769 7468 2070 6172 616d 6574 6572 7320  with parameters 
-00000ae0: 7370 6563 6966 6965 6420 6279 2074 6865  specified by the
-00000af0: 2064 6576 656c 6f70 6572 2e20 576f 726b   developer. Work
-00000b00: 7320 666f 7220 626f 7468 2054 7261 6469  s for both Tradi
-00000b10: 7469 6f6e 616c 2061 6e64 2053 696d 706c  tional and Simpl
-00000b20: 6966 6965 6420 6368 6172 6163 7465 7273  ified characters
-00000b30: 2e0d 0d0a 0d0d 0a60 6060 7079 7468 6f6e  .......```python
-00000b40: 0d0d 0a23 2063 6f6e 7374 7275 6374 6f72  ...# constructor
-00000b50: 0d0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
-00000b60: 2873 7973 7465 6d2c 2064 6961 6c65 6374  (system, dialect
-00000b70: 2c20 666f 726d 6174 2c20 6465 6c69 6d69  , format, delimi
-00000b80: 7465 722c 2073 616e 6468 692c 2070 756e  ter, sandhi, pun
-00000b90: 6374 7561 7469 6f6e 290d 0d0a 0d0d 0a23  ctuation)......#
-00000ba0: 2074 7261 6e73 6c69 7465 7261 7465 2043   transliterate C
-00000bb0: 6869 6e65 7365 2063 6861 7261 6374 6572  hinese character
-00000bc0: 730d 0d0a 632e 6765 7428 696e 7075 7429  s...c.get(input)
-00000bd0: 0d0d 0a0d 0d0a 2320 636f 6e76 6572 7420  ......# convert 
-00000be0: 5369 6d70 6c69 6669 6564 2043 6869 6e65  Simplified Chine
-00000bf0: 7365 2063 6861 7261 6374 6572 7320 746f  se characters to
-00000c00: 2054 7261 6469 7469 6f6e 616c 2043 6869   Traditional Chi
-00000c10: 6e65 7365 2043 6861 7261 6374 6572 730d  nese Characters.
-00000c20: 0d0a 632e 746f 5f74 7261 6469 7469 6f6e  ..c.to_tradition
-00000c30: 616c 2869 6e70 7574 290d 0d0a 6060 600d  al(input)...```.
-00000c40: 0d0a 0d0d 0a23 2323 2320 5379 7374 656d  .....#### System
-00000c50: 0d0d 0a0d 0d0a 6073 7973 7465 6d60 2053  ......`system` S
-00000c60: 7472 696e 6720 2d20 7379 7374 656d 206f  tring - system o
-00000c70: 6620 7472 616e 736c 6974 6572 6174 696f  f transliteratio
-00000c80: 6e2e 0d0d 0a0d 0d0a 2a20 6054 6169 6c6f  n.......* `Tailo
-00000c90: 6020 2864 6566 6175 6c74 2920 2d20 5b54  ` (default) - [T
-00000ca0: c3a2 692d 75c3 a26e 204c c3b4 2d6d c3a1  ..i-u..n L..-m..
-00000cb0: 2d6a c4ab 2050 6869 6e67 2d69 6d20 486f  -j.. Phing-im Ho
-00000cc0: 6e67 2dc3 a06e 5d5b 7461 696c 6f2d 7769  ng-..n][tailo-wi
-00000cd0: 6b69 5d0d 0d0a 2a20 6050 4f4a 6020 2d20  ki]...* `POJ` - 
-00000ce0: 5b50 65cc 8d68 2dc5 8d65 2d6a c4ab 5d5b  [Pe..h-..e-j..][
-00000cf0: 706f 6a2d 7769 6b69 5d0d 0d0a 2a20 605a  poj-wiki]...* `Z
-00000d00: 6875 7969 6e60 202d 205b 5461 6977 616e  huyin` - [Taiwan
-00000d10: 6573 6520 5068 6f6e 6574 6963 2053 796d  ese Phonetic Sym
-00000d20: 626f 6c73 5d5b 7a68 7579 696e 2d77 696b  bols][zhuyin-wik
-00000d30: 695d 0d0d 0a2a 2060 544c 5041 6020 2d20  i]...* `TLPA` - 
-00000d40: 5b54 6169 7761 6e65 7365 204c 616e 6775  [Taiwanese Langu
-00000d50: 6167 6520 5068 6f6e 6574 6963 2041 6c70  age Phonetic Alp
-00000d60: 6861 6265 745d 5b74 6c70 612d 7769 6b69  habet][tlpa-wiki
-00000d70: 5d0d 0d0a 2a20 6050 696e 6779 696d 6020  ]...* `Pingyim` 
-00000d80: 2d20 5b42 62c3 a16e 6cc3 a16d 2055 c493  - [Bb..nl..m U..
-00000d90: 2050 c3ac 6e67 79c4 ab6d 2048 c58d 6e67   P..ngy..m H..ng
-00000da0: 27c3 a06e 5d5b 7069 6e67 7969 6d2d 7769  '..n][pingyim-wi
-00000db0: 6b69 5d0d 0d0a 2a20 6054 6f6e 6769 6f6e  ki]...* `Tongion
-00000dc0: 6760 202d 205b 4461 c4ab 2d67 68c3 ae20  g` - [Da..-gh.. 
-00000dd0: 54c5 8d6e 672d 69c5 8d6e 6720 50c4 ab6e  T..ng-i..ng P..n
-00000de0: 672d 696d 5d5b 746f 6e67 696f 6e67 2d77  g-im][tongiong-w
-00000df0: 696b 695d 0d0d 0a0d 0d0a 7c20 7465 7874  iki]......| text
-00000e00: 207c 2054 6169 6c6f 2020 207c 2050 4f4a   | Tailo   | POJ
-00000e10: 2020 2020 207c 205a 6875 7969 6e20 2020       | Zhuyin   
-00000e20: 2020 207c 2054 4c50 4120 2020 2020 207c     | TLPA      |
-00000e30: 2050 696e 6779 696d 207c 2054 6f6e 6769   Pingyim | Tongi
-00000e40: 6f6e 6720 7c0d 0d0a 7c2d 2d2d 2d2d 2d7c  ong |...|------|
-00000e50: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
-00000e60: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00000e70: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -|-----------|--
-00000e80: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000e90: 2d2d 7c0d 0d0a 7c20 e887 bae7 81a3 207c  --|...| ...... |
-00000ea0: 2054 c3a2 692d 75c3 a26e 207c 2054 c3a2   T..i-u..n | T..
-00000eb0: 692d 6fc3 a26e 207c 20e3 8489 e384 9ecb  i-o..n | .......
-00000ec0: 8a20 e384 a8e3 84a2 cb8a 207c 2054 6169  . ........ | Tai
-00000ed0: 3520 7561 6e35 207c 2044 c3a1 6977 c3a1  5 uan5 | D..iw..
-00000ee0: 6e20 207c 2054 c481 692d 75c7 8e6e 2020  n  | T..i-u..n  
-00000ef0: 7c0d 0d0a 0d0d 0a23 2323 2320 4469 616c  |......#### Dial
-00000f00: 6563 740d 0d0a 0d0d 0a60 6469 616c 6563  ect......`dialec
-00000f10: 7460 2053 7472 696e 6720 2d20 7072 6566  t` String - pref
-00000f20: 6572 7265 6420 7072 6f6e 756e 6369 6174  erred pronunciat
-00000f30: 696f 6e2e 0d0d 0a0d 0d0a 2a20 6073 6f75  ion.......* `sou
-00000f40: 7468 6020 2864 6566 6175 6c74 2920 2d20  th` (default) - 
-00000f50: 5b5a 6861 6e67 7a68 6f75 5d5b 7a68 616e  [Zhangzhou][zhan
-00000f60: 677a 686f 752d 7769 6b69 5d2d 6c65 616e  gzhou-wiki]-lean
-00000f70: 696e 6720 7072 6f6e 756e 6369 6174 696f  ing pronunciatio
-00000f80: 6e0d 0d0a 2a20 606e 6f72 7468 6020 2d20  n...* `north` - 
-00000f90: 5b51 7561 6e7a 686f 755d 5b71 7561 6e7a  [Quanzhou][quanz
-00000fa0: 686f 752d 7769 6b69 5d2d 6c65 616e 696e  hou-wiki]-leanin
-00000fb0: 6720 7072 6f6e 756e 6369 6174 696f 6e0d  g pronunciation.
-00000fc0: 0d0a 0d0d 0a7c 2074 6578 7420 2020 7c20  .....| text   | 
-00000fd0: 736f 7574 6820 2020 2020 2020 2020 7c20  south         | 
-00000fe0: 6e6f 7274 6820 2020 2020 2020 2020 7c0d  north         |.
-00000ff0: 0d0a 7c2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  ..|--------|----
-00001000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00001010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0d0d 0a7c  -----------|...|
-00001020: 20e4 ba94 e69c 88e7 af80 207c 2047 c58d   ......... | G..
-00001030: 6f2d 6775 65cc 8d68 2d74 7365 6820 7c20  o-gue..h-tseh | 
-00001040: 47c5 8d6f 2d67 65cc 8d68 2d74 7375 6568  G..o-ge..h-tsueh
-00001050: 207c 0d0d 0a0d 0d0a 2323 2323 2046 6f72   |......#### For
-00001060: 6d61 740d 0d0a 0d0d 0a60 666f 726d 6174  mat......`format
-00001070: 6020 5374 7269 6e67 202d 2066 6f72 6d61  ` String - forma
-00001080: 7420 696e 2077 6869 6368 2074 6f6e 6573  t in which tones
-00001090: 2077 696c 6c20 6265 2072 6570 7265 7365   will be represe
-000010a0: 6e74 6564 2069 6e20 7468 6520 636f 6e76  nted in the conv
-000010b0: 6572 7465 6420 7365 6e74 656e 6365 2e0d  erted sentence..
-000010c0: 0d0a 0d0d 0a2a 2060 6d61 726b 6020 2864  .....* `mark` (d
-000010d0: 6566 6175 6c74 2920 2d20 7573 6573 2064  efault) - uses d
-000010e0: 6961 6372 6974 6963 7320 666f 7220 6561  iacritics for ea
-000010f0: 6368 2073 796c 6c61 626c 652e 204e 6f74  ch syllable. Not
-00001100: 2061 7661 696c 6162 6c65 2066 6f72 2054   available for T
-00001110: 4c50 412e 0d0d 0a2a 2060 6e75 6d62 6572  LPA....* `number
-00001120: 6020 2d20 6164 6420 6120 6e75 6d62 6572  ` - add a number
-00001130: 2077 6869 6368 2072 6570 7265 7365 6e74   which represent
-00001140: 7320 7468 6520 746f 6e65 2061 7420 7468  s the tone at th
-00001150: 6520 656e 6420 6f66 2074 6865 2073 796c  e end of the syl
-00001160: 6c61 626c 650d 0d0a 2a20 6073 7472 6970  lable...* `strip
-00001170: 6020 2d20 7265 6d6f 7665 7320 616e 7920  ` - removes any 
-00001180: 746f 6e65 206d 6172 6b69 6e67 0d0d 0a0d  tone marking....
-00001190: 0d0a 7c20 7465 7874 207c 206d 6172 6b20  ..| text | mark 
-000011a0: 2020 207c 206e 756d 6265 7220 2020 207c     | number    |
-000011b0: 2073 7472 6970 2020 207c 0d0d 0a7c 2d2d   strip   |...|--
-000011c0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d  ----|---------|-
-000011d0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-000011e0: 2d2d 2d2d 7c0d 0d0a 7c20 e887 bae7 81a3  ----|...| ......
-000011f0: 207c 2054 c3a2 692d 75c3 a26e 207c 2054   | T..i-u..n | T
-00001200: 6169 352d 7561 6e35 207c 2054 6169 2d75  ai5-uan5 | Tai-u
-00001210: 616e 207c 0d0d 0a0d 0d0a 2323 2323 2044  an |......#### D
-00001220: 656c 696d 6974 6572 0d0d 0a0d 0d0a 6064  elimiter......`d
-00001230: 656c 696d 6974 6572 6020 5374 7269 6e67  elimiter` String
-00001240: 202d 2073 6574 7320 7468 6520 6465 6c69   - sets the deli
-00001250: 6d69 7465 7220 6368 6172 6163 7465 7220  miter character 
-00001260: 7468 6174 2077 696c 6c20 6265 2070 6c61  that will be pla
-00001270: 6365 6420 696e 2062 6574 7765 656e 2073  ced in between s
-00001280: 796c 6c61 626c 6573 206f 6620 6120 776f  yllables of a wo
-00001290: 7264 2e0d 0d0a 0d0d 0a44 6566 6175 6c74  rd.......Default
-000012a0: 2076 616c 7565 2064 6570 656e 6473 206f   value depends o
-000012b0: 6e20 7468 6520 6368 6f73 656e 2060 7379  n the chosen `sy
-000012c0: 7374 656d 603a 0d0d 0a0d 0d0a 2a20 6027  stem`:......* `'
-000012d0: 2d27 6020 2d20 666f 7220 6054 6169 6c6f  -'` - for `Tailo
-000012e0: 602c 2060 504f 4a60 2c20 6054 6f6e 6769  `, `POJ`, `Tongi
-000012f0: 6f6e 6760 0d0d 0a2a 2060 2727 6020 2d20  ong`...* `''` - 
-00001300: 666f 7220 6050 696e 6779 696d 600d 0d0a  for `Pingyim`...
-00001310: 2a20 6027 2027 6020 2d20 666f 7220 605a  * `' '` - for `Z
-00001320: 6875 7969 6e60 2c20 6054 4c50 4160 0d0d  huyin`, `TLPA`..
-00001330: 0a0d 0d0a 7c20 7465 7874 207c 2027 2d27  ....| text | '-'
-00001340: 2020 2020 207c 2027 2720 2020 2020 7c20       | ''     | 
-00001350: 2720 2720 2020 2020 7c0d 0d0a 7c2d 2d2d  ' '     |...|---
-00001360: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  ---|---------|--
-00001370: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00001380: 7c0d 0d0a 7c20 e887 bae7 81a3 207c 2054  |...| ...... | T
-00001390: c3a2 692d 75c3 a26e 207c 2054 c3a2 6975  ..i-u..n | T..iu
-000013a0: c3a2 6e20 7c20 54c3 a269 2075 c3a2 6e20  ..n | T..i u..n 
-000013b0: 7c0d 0d0a 0d0d 0a23 2323 2320 5361 6e64  |......#### Sand
-000013c0: 6869 0d0d 0a0d 0d0a 6073 616e 6468 6960  hi......`sandhi`
-000013d0: 2042 6f6f 6c65 616e 202d 2061 7070 6c69   Boolean - appli
-000013e0: 6573 2074 6865 205b 7361 6e64 6869 2072  es the [sandhi r
-000013f0: 756c 6573 206f 6620 5461 6977 616e 6573  ules of Taiwanes
-00001400: 6520 486f 6b6b 6965 6e5d 5b73 616e 6468  e Hokkien][sandh
-00001410: 692d 7769 6b69 5d20 746f 2073 796c 6c61  i-wiki] to sylla
-00001420: 626c 6573 206f 6620 6120 7369 6e67 6c65  bles of a single
-00001430: 2077 6f72 642e 0d0d 0a0d 0d0a 4465 6661   word.......Defa
-00001440: 756c 7420 7661 6c75 6520 6465 7065 6e64  ult value depend
-00001450: 7320 6f6e 2074 6865 2063 686f 7365 6e20  s on the chosen 
-00001460: 6073 7973 7465 6d60 3a0d 0d0a 0d0d 0a2a  `system`:......*
-00001470: 2060 5472 7565 6020 2d20 666f 7220 6054   `True` - for `T
-00001480: 6f6e 6769 6f6e 6760 0d0d 0a2a 2060 4661  ongiong`...* `Fa
-00001490: 6c73 6560 202d 2066 6f72 2060 5461 696c  lse` - for `Tail
-000014a0: 6f60 2c20 6050 4f4a 602c 2060 5a68 7579  o`, `POJ`, `Zhuy
-000014b0: 696e 602c 2060 544c 5041 602c 2060 5069  in`, `TLPA`, `Pi
-000014c0: 6e67 7969 6d60 0d0d 0a0d 0d0a 7c20 7465  ngyim`......| te
-000014d0: 7874 2020 2020 207c 2046 616c 7365 2020  xt     | False  
-000014e0: 2020 2020 2020 7c20 5472 7565 2020 2020        | True    
-000014f0: 2020 2020 207c 0d0d 0a7c 2d2d 2d2d 2d2d       |...|------
-00001500: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-00001510: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00001520: 2d2d 7c0d 0d0a 7c20 e9a6 ace4 be86 e8a5  --|...| ........
-00001530: bfe4 ba9e 207c 204d c3a1 2d6c c3a2 692d  .... | M..-l..i-
-00001540: 7365 2d61 2020 7c20 4d61 2d6c c481 692d  se-a  | Ma-l..i-
-00001550: 73c4 932d 6120 207c 0d0d 0a0d 0d0a 5361  s..-a  |......Sa
-00001560: 6e64 6869 2072 756c 6573 2061 6c73 6f20  ndhi rules also 
-00001570: 6368 616e 6765 2064 6570 656e 6469 6e67  change depending
-00001580: 206f 6e20 7468 6520 6469 616c 6563 7420   on the dialect 
-00001590: 6368 6f73 656e 2e0d 0d0a 0d0d 0a7c 2074  chosen.......| t
-000015a0: 6578 7420 7c20 6e6f 2073 616e 6468 6920  ext | no sandhi 
-000015b0: 7c20 736f 7574 6820 2020 7c20 6e6f 7274  | south   | nort
-000015c0: 6820 2020 7c0d 0d0a 7c2d 2d2d 2d2d 2d7c  h   |...|------|
-000015d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-000015e0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d7c  -----|---------|
-000015f0: 0d0d 0a7c 20e8 87ba e781 a320 7c20 54c3  ...| ...... | T.
-00001600: a269 2d75 c3a2 6e20 2020 7c20 54c4 8169  .i-u..n   | T..i
-00001610: 2d75 c3a2 6e20 7c20 54c3 a069 2d75 c3a2  -u..n | T..i-u..
-00001620: 6e20 7c0d 0d0a 0d0d 0a4e 6f74 6520 7468  n |......Note th
-00001630: 6174 2074 6865 2066 756e 6374 696f 6e20  at the function 
-00001640: 6973 2064 6966 6665 7265 6e74 2066 726f  is different fro
-00001650: 6d20 7265 616c 2073 616e 6468 6920 7275  m real sandhi ru
-00001660: 6c65 732c 2077 6865 7265 2063 6861 6e67  les, where chang
-00001670: 6573 2061 7265 2061 7070 6c69 6564 2074  es are applied t
-00001680: 6f20 6576 6572 7920 7369 6e67 6c65 2073  o every single s
-00001690: 796c 6c61 626c 6520 6f66 2074 6865 2073  yllable of the s
-000016a0: 656e 7465 6e63 652c 206e 6f74 206a 7573  entence, not jus
-000016b0: 7420 7369 6e67 6c65 2077 6f72 6473 2e0d  t single words..
-000016c0: 0d0a 0d0d 0a2d 202a 2a54 6169 6275 6e27  .....- **Taibun'
-000016d0: 7320 7361 6e64 6869 2072 756c 6573 2a2a  s sandhi rules**
-000016e0: 3a20 5468 c3a1 692d 6b68 6f6e 6720 70c4  : Th..i-khong p.
-000016f0: ab6e 672d 69c3 ba2c 206c 696e 2d68 c3b3  .ng-i.., lin-h..
-00001700: 2120 4cc3 ad6e 2074 7369 c3a0 2d70 c3a1  ! L..n tsi..-p..
-00001710: 2062 75c4 933f 0d0d 0a2d 202a 2a41 6374   bu..?...- **Act
-00001720: 7561 6c20 7361 6e64 6869 2072 756c 6573  ual sandhi rules
-00001730: 2a2a 3a20 5468 c3a1 692d 6b68 c58d 6e67  **: Th..i-kh..ng
-00001740: 2070 c4ab 6e67 2d69 c3ba 2c20 6c69 6e2d   p..ng-i.., lin-
-00001750: 68c3 b321 204c 696e 2074 7369 c3a0 2d70  h..! Lin tsi..-p
-00001760: 6120 6275 c493 3f0d 0d0a 0d0d 0a23 2323  a bu..?......###
-00001770: 2320 5075 6e63 7475 6174 696f 6e0d 0d0a  # Punctuation...
-00001780: 0d0d 0a60 7075 6e63 7475 6174 696f 6e60  ...`punctuation`
-00001790: 2053 7472 696e 670d 0d0a 0d0d 0a2a 2060   String......* `
-000017a0: 666f 726d 6174 6020 2864 6566 6175 6c74  format` (default
-000017b0: 2920 2d20 636f 6e76 6572 7473 2043 6869  ) - converts Chi
-000017c0: 6e65 7365 2d73 7479 6c65 2070 756e 6374  nese-style punct
-000017d0: 7561 7469 6f6e 2074 6f20 4c61 7469 6e2d  uation to Latin-
-000017e0: 7374 796c 6520 7075 6e63 7475 6174 696f  style punctuatio
-000017f0: 6e20 616e 6420 6361 7069 7461 6c69 7365  n and capitalise
-00001800: 7320 776f 7264 7320 6174 2074 6865 2062  s words at the b
-00001810: 6567 696e 6e69 6e67 206f 6620 6561 6368  eginning of each
-00001820: 2073 656e 7465 6e63 652e 0d0d 0a2a 2060   sentence....* `
-00001830: 6e6f 6e65 6020 2d20 7072 6573 6572 7665  none` - preserve
-00001840: 7320 4368 696e 6573 652d 7374 796c 6520  s Chinese-style 
-00001850: 7075 6e63 7475 6174 696f 6e20 616e 6420  punctuation and 
-00001860: 646f 6573 6e27 7420 6361 7069 7461 6c69  doesn't capitali
-00001870: 7365 2077 6f72 6473 2061 7420 7468 6520  se words at the 
-00001880: 6265 6769 6e6e 696e 6720 6f66 206e 6577  beginning of new
-00001890: 2073 656e 7465 6e63 6573 2e0d 0d0a 0d0d   sentences......
-000018a0: 0a7c 2074 6578 7420 7c20 666f 726d 6174  .| text | format
-000018b0: 207c 206e 6f6e 6520 7c0d 0d0a 7c2d 7c2d   | none |...|-|-
-000018c0: 7c2d 7c0d 0d0a 7c20 e980 99e6 98af e887  |-|...| ........
-000018d0: bae5 8d97 efbc 8ce7 b0a1 e7a8 b1e3 808c  ................
-000018e0: e58d 97e3 808d efbc 88e7 99bd e8a9 b1e5  ................
-000018f0: ad97 efbc 9a54 c3a2 692d 6cc3 a26d efbc  .....T..i-l..m..
-00001900: 9be6 b3a8 e99f b3e7 aca6 e899 9fef bc9a  ................
-00001910: e384 8ae3 849e cb8a 20e3 848b e384 a2cb  ........ .......
-00001920: 8aef bc8c e59c 8be8 aa9e efbc 9a54 c3a1  .............T..
-00001930: 696e c3a1 6eef bc89 e380 8220 7c20 5473  in..n...... | Ts
-00001940: 6520 73c4 ab20 54c3 a269 2d6c c3a2 6d2c  e s.. T..i-l..m,
-00001950: 206b c3a1 6e2d 7473 6869 6e67 2022 6cc3   k..n-tshing "l.
-00001960: a26d 2220 2850 65cc 8d68 2d75 c493 2d6a  .m" (Pe..h-u..-j
-00001970: c4ab 3a20 54c3 a269 2d6c c3a2 6d3b 2074  ..: T..i-l..m; t
-00001980: 73c3 b92d 696d 2068 c3bb 2d68 c58d 3a20  s..-im h..-h..: 
-00001990: e384 8ae3 849e cb8a 20e3 848b e384 a2cb  ........ .......
-000019a0: 8a2c 206b 6f6b 2d67 c3ad 3a20 54c3 a169  ., kok-g..: T..i
-000019b0: 6ec3 a16e 292e 207c 2074 7365 2073 c4ab  n..n). | tse s..
-000019c0: 2054 c3a2 692d 6cc3 a26d efbc 8c6b c3a1   T..i-l..m...k..
-000019d0: 6e2d 7473 6869 6e67 e380 8c6c c3a2 6de3  n-tshing...l..m.
-000019e0: 808d efbc 8850 65cc 8d68 2d75 c493 2d6a  .....Pe..h-u..-j
-000019f0: c4ab efbc 9a54 c3a2 692d 6cc3 a26d efbc  .....T..i-l..m..
-00001a00: 9b74 73c3 b92d 696d 2068 c3bb 2d68 c58d  .ts..-im h..-h..
-00001a10: efbc 9ae3 848a e384 9ecb 8a20 e384 8be3  ........... ....
-00001a20: 84a2 cb8a efbc 8c6b 6f6b 2d67 c3ad efbc  .......kok-g....
-00001a30: 9a54 c3a1 696e c3a1 6eef bc89 e380 8220  .T..in..n...... 
-00001a40: 7c0d 0d0a 0d0d 0a23 2323 2054 6f6b 656e  |......### Token
-00001a50: 6973 6572 0d0d 0a0d 0d0a 6054 6f6b 656e  iser......`Token
-00001a60: 6973 6572 6020 636c 6173 7320 7065 7266  iser` class perf
-00001a70: 6f72 6d73 205b 4e4c 544b 2077 6f72 6470  orms [NLTK wordp
-00001a80: 756e 6374 5f74 6f6b 656e 697a 655d 5b6e  unct_tokenize][n
-00001a90: 6c74 6b2d 746f 6b65 6e69 7a65 5d2d 6c69  ltk-tokenize]-li
-00001aa0: 6b65 2074 6f6b 656e 6973 6174 696f 6e20  ke tokenisation 
-00001ab0: 6f66 2061 2054 6169 7761 6e65 7365 2048  of a Taiwanese H
-00001ac0: 6f6b 6b69 656e 2073 656e 7465 6e63 652e  okkien sentence.
-00001ad0: 0d0d 0a0d 0d0a 6060 6070 7974 686f 6e0d  ......```python.
-00001ae0: 0d0a 2320 636f 6e73 7472 7563 746f 720d  ..# constructor.
-00001af0: 0d0a 7420 3d20 546f 6b65 6e69 7365 7228  ..t = Tokeniser(
-00001b00: 290d 0d0a 0d0d 0a23 2074 6f6b 656e 6973  )......# tokenis
-00001b10: 6520 5461 6977 616e 6573 6520 486f 6b6b  e Taiwanese Hokk
-00001b20: 6965 6e20 7365 6e74 656e 6365 0d0d 0a74  ien sentence...t
-00001b30: 2e74 6f6b 656e 6973 6528 696e 7075 7429  .tokenise(input)
-00001b40: 0d0d 0a60 6060 0d0d 0a0d 0d0a 0d0d 0a0d  ...```..........
-00001b50: 0d0a 3c21 2d2d 2045 5841 4d50 4c45 202d  ..<!-- EXAMPLE -
-00001b60: 2d3e 0d0d 0a23 2320 4578 616d 706c 650d  ->...## Example.
-00001b70: 0d0a 0d0d 0a60 6060 7079 7468 6f6e 0d0d  .....```python..
-00001b80: 0a66 726f 6d20 7461 6962 756e 2069 6d70  .from taibun imp
-00001b90: 6f72 7420 436f 6e76 6572 7465 722c 2054  ort Converter, T
-00001ba0: 6f6b 656e 6973 6572 0d0d 0a0d 0d0a 2320  okeniser......# 
-00001bb0: 5379 7374 656d 0d0d 0a63 203d 2043 6f6e  System...c = Con
-00001bc0: 7665 7274 6572 2829 2023 2054 6169 6c6f  verter() # Tailo
-00001bd0: 2073 7973 7465 6d20 6465 6661 756c 740d   system default.
-00001be0: 0d0a 632e 6765 7428 27e5 8588 e794 9fe8  ..c.get('.......
-00001bf0: ac9b efbc 8ce5 adb8 e794 9fe6 81ac e681  ................
-00001c00: ace8 81bd e380 8227 290d 0d0a 3e3e 2053  .......')...>> S
-00001c10: 6961 6e2d 7369 6e6e 206b c3b3 6e67 2c20  ian-sinn k..ng, 
-00001c20: 6861 cc8d 6b2d 7369 6e67 2074 69c4 816d  ha..k-sing ti..m
-00001c30: 2d74 69c4 816d 2074 6869 616e 6e2e 0d0d  -ti..m thiann...
-00001c40: 0a0d 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00001c50: 7228 7379 7374 656d 3d27 5a68 7579 696e  r(system='Zhuyin
-00001c60: 2729 0d0d 0a63 2e67 6574 2827 e585 88e7  ')...c.get('....
-00001c70: 949f e8ac 9bef bc8c e5ad b8e7 949f e681  ................
-00001c80: ace6 81ac e881 bde3 8082 2729 0d0d 0a3e  ..........')...>
-00001c90: 3e20 e384 92e3 84a7 e384 a220 e384 92e3  > ......... ....
-00001ca0: 86aa 20e3 848d e386 b2cb 8b2c 20e3 848f  .. ........, ...
-00001cb0: e384 9ae3 86b6 cb99 20e3 8492 e384 a7e3  ........ .......
-00001cc0: 84a5 20e3 8489 e384 a7e3 86b0 cbab 20e3  .. ........... .
-00001cd0: 8489 e384 a7e3 86b0 cbab 20e3 848a e384  .......... .....
-00001ce0: a7e3 86a9 2e0d 0d0a 0d0d 0a23 2044 6961  ...........# Dia
-00001cf0: 6c65 6374 0d0d 0a63 203d 2043 6f6e 7665  lect...c = Conve
-00001d00: 7274 6572 2829 2023 2073 6f75 7468 2064  rter() # south d
-00001d10: 6961 6c65 6374 2064 6566 6175 6c74 0d0d  ialect default..
-00001d20: 0a63 2e67 6574 2822 e688 91e6 acb2 e794  .c.get("........
-00001d30: a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0d 0a3e  ..........")...>
-00001d40: 3e20 4775 c3a1 2062 6568 20c4 ab6e 6720  > Gu.. beh ..ng 
-00001d50: 74c4 ab20 7473 6961 cc8d 6820 68c3 ae0d  t.. tsia..h h...
-00001d60: 0d0a 0d0d 0a63 203d 2043 6f6e 7665 7274  .....c = Convert
-00001d70: 6572 2864 6961 6c65 6374 3d27 6e6f 7274  er(dialect='nort
-00001d80: 6827 290d 0d0a 632e 6765 7428 22e6 8891  h')...c.get("...
-00001d90: e6ac b2e7 94a8 e7ae b8e9 a39f e9ad 9a22  ..............."
-00001da0: 290d 0d0a 3e3e 2047 75c3 a120 6275 6568  )...>> Gu.. bueh
-00001db0: 20c4 ab6e 6720 74c5 ab20 7473 6961 cc8d   ..ng t.. tsia..
-00001dc0: 6820 68c3 bb0d 0d0a 0d0d 0a23 2046 6f72  h h........# For
-00001dd0: 6d61 740d 0d0a 6320 3d20 436f 6e76 6572  mat...c = Conver
-00001de0: 7465 7228 2920 2320 666f 7220 5461 696c  ter() # for Tail
-00001df0: 6f2c 206d 6172 6b20 6279 2064 6566 6175  o, mark by defau
-00001e00: 6c74 0d0d 0a63 2e67 6574 2822 e794 9fe6  lt...c.get("....
-00001e10: 97a5 e5bf abe6 a882 2229 0d0d 0a3e 3e20  ........")...>> 
-00001e20: 5365 6e6e 2d6a 69cc 8d74 206b 6875 c3a0  Senn-ji..t khu..
-00001e30: 692d 6c6f cc8d 6b0d 0d0a 0d0d 0a63 203d  i-lo..k......c =
-00001e40: 2043 6f6e 7665 7274 6572 2866 6f72 6d61   Converter(forma
-00001e50: 743d 276e 756d 6265 7227 290d 0d0a 632e  t='number')...c.
-00001e60: 6765 7428 22e7 949f e697 a5e5 bfab e6a8  get("...........
-00001e70: 8222 290d 0d0a 3e3e 2053 656e 6e31 2d6a  .")...>> Senn1-j
-00001e80: 6974 3820 6b68 7561 6933 2d6c 6f6b 380d  it8 khuai3-lok8.
-00001e90: 0d0a 0d0d 0a63 203d 2043 6f6e 7665 7274  .....c = Convert
-00001ea0: 6572 2866 6f72 6d61 743d 2773 7472 6970  er(format='strip
-00001eb0: 2729 0d0d 0a63 2e67 6574 2822 e794 9fe6  ')...c.get("....
-00001ec0: 97a5 e5bf abe6 a882 2229 0d0d 0a3e 3e20  ........")...>> 
-00001ed0: 5365 6e6e 2d6a 6974 206b 6875 6169 2d6c  Senn-jit khuai-l
-00001ee0: 6f6b 0d0d 0a0d 0d0a 2320 4465 6c69 6d69  ok......# Delimi
-00001ef0: 7465 720d 0d0a 6320 3d20 436f 6e76 6572  ter...c = Conver
-00001f00: 7465 7228 6465 6c69 6d69 7465 723d 2727  ter(delimiter=''
-00001f10: 290d 0d0a 632e 6765 7428 22e5 8588 e794  )...c.get(".....
-00001f20: 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6 81ac  ................
-00001f30: e681 ace8 81bd e380 8222 290d 0d0a 3e3e  .........")...>>
-00001f40: 2053 6961 6e73 696e 6e20 6bc3 b36e 672c   Siansinn k..ng,
-00001f50: 2068 61cc 8d6b 7369 6e67 2074 69c4 816d   ha..ksing ti..m
-00001f60: 7469 c481 6d20 7468 6961 6e6e 2e0d 0d0a  ti..m thiann....
-00001f70: 0d0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
-00001f80: 2873 7973 7465 6d3d 2750 696e 6779 696d  (system='Pingyim
-00001f90: 272c 2064 656c 696d 6974 6572 3d27 2d27  ', delimiter='-'
-00001fa0: 290d 0d0a 632e 6765 7428 22e5 8588 e794  )...c.get(".....
-00001fb0: 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6 81ac  ................
-00001fc0: e681 ace8 81bd e380 8222 290d 0d0a 3e3e  .........")...>>
-00001fd0: 2053 69c4 816e 2d73 6ec4 ab20 67c7 926e   Si..n-sn.. g..n
-00001fe0: 672c 2068 c3a1 672d 73c4 ab6e 6720 6469  g, h..g-s..ng di
-00001ff0: c3a2 6d2d 6469 c3a2 6d20 7469 6ec4 812e  ..m-di..m tin...
-00002000: 0d0d 0a0d 0d0a 2320 5361 6e64 6869 0d0d  ......# Sandhi..
-00002010: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
-00002020: 2023 2066 6f72 2054 6169 6c6f 2c20 7361   # for Tailo, sa
-00002030: 6e64 6869 2046 616c 7365 2062 7920 6465  ndhi False by de
-00002040: 6661 756c 740d 0d0a 632e 6765 7428 22e5  fault...c.get(".
-00002050: 8d97 e8bf b4e9 90b5 e8b7 af22 290d 0d0a  ...........")...
-00002060: 3e3e 204c c3a2 6d2d 6875 c3aa 2d74 6869  >> L..m-hu..-thi
-00002070: 682d 6cc5 8d6f 0d0d 0a0d 0d0a 6320 3d20  h-l..o......c = 
-00002080: 436f 6e76 6572 7465 7228 7361 6e64 6869  Converter(sandhi
-00002090: 3d54 7275 6529 0d0d 0a63 2e67 6574 2822  =True)...c.get("
-000020a0: e58d 97e8 bfb4 e990 b5e8 b7af 2229 0d0d  ............")..
-000020b0: 0a3e 3e20 4cc4 816d 2d68 75c4 932d 7468  .>> L..m-hu..-th
-000020c0: c3ad 2d6c c58d 6f0d 0d0a 0d0d 0a23 2050  ..-l..o......# P
-000020d0: 756e 6374 7561 7469 6f6e 0d0d 0a63 203d  unctuation...c =
-000020e0: 2043 6f6e 7665 7274 6572 2829 2023 2066   Converter() # f
-000020f0: 6f72 6d61 7420 7075 6e63 7475 6174 696f  ormat punctuatio
-00002100: 6e20 6465 6661 756c 740d 0d0a 632e 6765  n default...c.ge
-00002110: 7428 22e5 a4aa e7a9 bae6 9c8b e58f 8bef  t(".............
-00002120: bc8c e681 81e5 a5bd efbc 81e6 8181 e9a3  ................
-00002130: 9fe9 a3bd e69c aaef bc9f 2229 0d0d 0a3e  ..........")...>
-00002140: 3e20 5468 c3a0 692d 6b68 6f6e 6720 70c3  > Th..i-khong p.
-00002150: ae6e 672d 69c3 ba2c 206c c3ad 6e2d 68c3  .ng-i.., l..n-h.
-00002160: b321 204c c3ad 6e20 7473 6961 cc8d 682d  .! L..n tsia..h-
-00002170: 70c3 a120 6275 c493 3f0d 0d0a 0d0d 0a63  p.. bu..?......c
-00002180: 203d 2043 6f6e 7665 7274 6572 2870 756e   = Converter(pun
-00002190: 6374 7561 7469 6f6e 3d27 6e6f 6e65 2729  ctuation='none')
-000021a0: 0d0d 0a63 2e67 6574 2822 e5a4 aae7 a9ba  ...c.get("......
-000021b0: e69c 8be5 8f8b efbc 8ce6 8181 e5a5 bdef  ................
-000021c0: bc81 e681 81e9 a39f e9a3 bde6 9caa efbc  ................
-000021d0: 9f22 290d 0d0a 3e3e 2074 68c3 a069 2d6b  .")...>> th..i-k
-000021e0: 686f 6e67 2070 c3ae 6e67 2d69 c3ba efbc  hong p..ng-i....
-000021f0: 8c6c c3ad 6e2d 68c3 b3ef bc81 6cc3 ad6e  .l..n-h.....l..n
-00002200: 2074 7369 61cc 8d68 2d70 c3a1 2062 75c4   tsia..h-p.. bu.
-00002210: 93ef bc9f 0d0d 0a0d 0d0a 0d0d 0a23 2054  .............# T
-00002220: 6f6b 656e 6973 6572 0d0d 0a74 203d 2054  okeniser...t = T
-00002230: 6f6b 656e 6973 6572 2829 0d0d 0a74 2e74  okeniser()...t.t
-00002240: 6f6b 656e 6973 6528 22e5 a4aa e7a9 bae6  okenise(".......
-00002250: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
-00002260: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
-00002270: 2229 0d0d 0a3e 3e20 5b27 e5a4 aae7 a9ba  ")...>> ['......
-00002280: 272c 2027 e69c 8be5 8f8b 272c 2027 efbc  ', '......', '..
-00002290: 8c27 2c20 27e6 8181 e5a5 bd27 2c20 27ef  .', '......', '.
-000022a0: bc81 272c 2027 e681 8127 2c20 27e9 a39f  ..', '...', '...
-000022b0: e9a3 bd27 2c20 27e6 9caa 272c 2027 efbc  ...', '...', '..
-000022c0: 9f27 5d0d 0d0a 6060 600d 0d0a 0d0d 0a0d  .']...```.......
-000022d0: 0d0a 0d0d 0a3c 212d 2d20 4441 5441 202d  .....<!-- DATA -
-000022e0: 2d3e 0d0d 0a23 2320 4461 7461 0d0d 0a0d  ->...## Data....
-000022f0: 0d0a 2d20 5b54 6169 7761 6e65 7365 2d43  ..- [Taiwanese-C
-00002300: 6869 6e65 7365 204f 6e6c 696e 6520 4469  hinese Online Di
-00002310: 6374 696f 6e61 7279 5d5b 6f6e 6c69 6e65  ctionary][online
-00002320: 2d64 6963 7469 6f6e 6172 795d 2028 7669  -dictionary] (vi
-00002330: 6120 5b43 6868 6f65 5461 6967 695d 5b64  a [ChhoeTaigi][d
-00002340: 6174 612d 7669 615d 290d 0d0a 2d20 5b69  ata-via])...- [i
-00002350: 5461 6967 6920 4368 696e 6573 652d 5461  Taigi Chinese-Ta
-00002360: 6977 616e 6573 6520 436f 6d70 6172 6973  iwanese Comparis
-00002370: 6f6e 2044 6963 7469 6f6e 6172 795d 5b69  on Dictionary][i
-00002380: 7461 6967 692d 6469 6374 696f 6e61 7279  taigi-dictionary
-00002390: 5d20 2876 6961 205b 4368 686f 6554 6169  ] (via [ChhoeTai
-000023a0: 6769 5d5b 6461 7461 2d76 6961 5d29 0d0d  gi][data-via])..
-000023b0: 0a0d 0d0a 0d0d 0a0d 0d0a 3c21 2d2d 2041  ..........<!-- A
-000023c0: 434b 4e4f 574c 4544 4745 4d45 4e54 5320  CKNOWLEDGEMENTS 
-000023d0: 2d2d 3e0d 0d0a 2323 2041 636b 6e6f 776c  -->...## Acknowl
-000023e0: 6564 6765 6d65 6e74 730d 0d0a 0d0d 0a2d  edgements......-
-000023f0: 2053 616d 7565 6c20 4a65 6e20 285b 4769   Samuel Jen ([Gi
-00002400: 7468 7562 5d5b 7361 6d75 656c 2d67 6974  thub][samuel-git
-00002410: 6875 625d 20c2 b720 5b4c 696e 6b65 6449  hub] .. [LinkedI
-00002420: 6e5d 5b73 616d 7565 6c2d 6c69 6e6b 6564  n][samuel-linked
-00002430: 696e 5d29 202d 2054 6169 7761 6e65 7365  in]) - Taiwanese
-00002440: 2061 6e64 204d 616e 6461 7269 6e20 7472   and Mandarin tr
-00002450: 616e 736c 6174 696f 6e0d 0d0a 0d0d 0a0d  anslation.......
-00002460: 0d0a 0d0d 0a3c 212d 2d20 4c49 4345 4e43  .....<!-- LICENC
-00002470: 4520 2d2d 3e0d 0d0a 2323 204c 6963 656e  E -->...## Licen
-00002480: 6365 0d0d 0a0d 0d0a 4265 6361 7573 6520  ce......Because 
-00002490: 5461 6962 756e 2069 7320 4d49 542d 6c69  Taibun is MIT-li
-000024a0: 6365 6e73 6564 2c20 616e 7920 6465 7665  censed, any deve
-000024b0: 6c6f 7065 7220 6361 6e20 6573 7365 6e74  loper can essent
-000024c0: 6961 6c6c 7920 646f 2077 6861 7465 7665  ially do whateve
-000024d0: 7220 7468 6579 2077 616e 7420 7769 7468  r they want with
-000024e0: 2069 7420 6173 206c 6f6e 6720 6173 2074   it as long as t
-000024f0: 6865 7920 696e 636c 7564 6520 7468 6520  hey include the 
-00002500: 6f72 6967 696e 616c 2063 6f70 7972 6967  original copyrig
-00002510: 6874 2061 6e64 206c 6963 656e 6365 206e  ht and licence n
-00002520: 6f74 6963 6520 696e 2061 6e79 2063 6f70  otice in any cop
-00002530: 6965 7320 6f66 2074 6865 2073 6f75 7263  ies of the sourc
-00002540: 6520 636f 6465 2e20 4e6f 7465 2c20 7468  e code. Note, th
-00002550: 6174 2074 6865 2064 6174 6120 7573 6564  at the data used
-00002560: 2062 7920 7468 6520 7061 636b 6167 6520   by the package 
-00002570: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
-00002580: 7220 6120 6469 6666 6572 656e 7420 636f  r a different co
-00002590: 7079 7269 6768 742e 0d0d 0a0d 0d0a 5468  pyright.......Th
-000025a0: 6520 6461 7461 2069 7320 6c69 6365 6e73  e data is licens
-000025b0: 6564 2075 6e64 6572 205b 4343 2042 592d  ed under [CC BY-
-000025c0: 5341 2034 2e30 5d5b 6461 7461 2d63 635d  SA 4.0][data-cc]
-000025d0: 0d0d 0a0d 0d0a 0d0d 0a0d 0d0a 3c21 2d2d  ............<!--
-000025e0: 204d 4152 4b44 4f57 4e20 4c49 4e4b 5320   MARKDOWN LINKS 
-000025f0: 2d2d 3e0d 0d0a 5b74 6573 7473 5d3a 2068  -->...[tests]: h
-00002600: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002610: 6d2f 616e 6472 6569 6861 722f 7461 6962  m/andreihar/taib
-00002620: 756e 2f61 6374 696f 6e73 0d0d 0a5b 7465  un/actions...[te
-00002630: 7374 732d 6261 6467 655d 3a20 6874 7470  sts-badge]: http
-00002640: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00002650: 696f 2f67 6974 6875 622f 6163 7469 6f6e  io/github/action
-00002660: 732f 776f 726b 666c 6f77 2f73 7461 7475  s/workflow/statu
-00002670: 732f 616e 6472 6569 6861 722f 7461 6962  s/andreihar/taib
-00002680: 756e 2f63 692e 7961 6d6c 3f73 7479 6c65  un/ci.yaml?style
-00002690: 3d66 6f72 2d74 6865 2d62 6164 6765 0d0d  =for-the-badge..
-000026a0: 0a5b 636f 6e74 7269 6275 746f 7273 2d62  .[contributors-b
-000026b0: 6164 6765 5d3a 2068 7474 7073 3a2f 2f69  adge]: https://i
-000026c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-000026d0: 7468 7562 2f63 6f6e 7472 6962 7574 6f72  thub/contributor
-000026e0: 732f 616e 6472 6569 6861 722f 7461 6962  s/andreihar/taib
-000026f0: 756e 3f73 7479 6c65 3d66 6f72 2d74 6865  un?style=for-the
-00002700: 2d62 6164 6765 0d0d 0a5b 636f 6e74 7269  -badge...[contri
-00002710: 6275 746f 7273 5d3a 2023 7573 6167 650d  butors]: #usage.
-00002720: 0d0a 5b72 656c 6561 7365 2d62 6164 6765  ..[release-badge
-00002730: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00002740: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00002750: 2f76 2f72 656c 6561 7365 2f61 6e64 7265  /v/release/andre
-00002760: 6968 6172 2f74 6169 6275 6e3f 636f 6c6f  ihar/taibun?colo
-00002770: 723d 3338 3631 3863 2673 7479 6c65 3d66  r=38618c&style=f
-00002780: 6f72 2d74 6865 2d62 6164 6765 0d0d 0a5b  or-the-badge...[
-00002790: 7265 6c65 6173 655d 3a20 6874 7470 733a  release]: https:
-000027a0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6e64  //github.com/and
-000027b0: 7265 6968 6172 2f74 6169 6275 6e2f 7265  reihar/taibun/re
-000027c0: 6c65 6173 6573 0d0d 0a5b 6c69 6365 6e63  leases...[licenc
-000027d0: 652d 6261 6467 655d 3a20 6874 7470 733a  e-badge]: https:
-000027e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000027f0: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
-00002800: 616e 6472 6569 6861 722f 7461 6962 756e  andreihar/taibun
-00002810: 3f63 6f6c 6f72 3d30 3030 3030 3026 7374  ?color=000000&st
-00002820: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
-00002830: 650d 0d0a 5b6c 6963 656e 6365 5d3a 204c  e...[licence]: L
-00002840: 4943 454e 5345 0d0d 0a5b 6c69 6e6b 6564  ICENSE...[linked
-00002850: 696e 2d62 6164 6765 5d3a 2068 7474 7073  in-badge]: https
-00002860: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00002870: 6f2f 6261 6467 652f 4c69 6e6b 6564 496e  o/badge/LinkedIn
-00002880: 2d30 3037 3742 353f 7374 796c 653d 666f  -0077B5?style=fo
-00002890: 722d 7468 652d 6261 6467 6526 6c6f 676f  r-the-badge&logo
-000028a0: 3d6c 696e 6b65 6469 6e26 6c6f 676f 436f  =linkedin&logoCo
-000028b0: 6c6f 723d 7768 6974 650d 0d0a 5b6c 696e  lor=white...[lin
-000028c0: 6b65 6469 6e5d 3a20 6874 7470 733a 2f2f  kedin]: https://
-000028d0: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
-000028e0: 2f69 6e2f 616e 6472 6569 2d68 6172 6261  /in/andrei-harba
-000028f0: 6368 6f76 2f0d 0d0a 0d0d 0a5b 7079 7069  chov/......[pypi
-00002900: 5d3a 2068 7474 7073 3a2f 2f70 7970 692e  ]: https://pypi.
-00002910: 6f72 672f 7072 6f6a 6563 742f 7461 6962  org/project/taib
-00002920: 756e 0d0d 0a5b 6275 675d 3a20 6874 7470  un...[bug]: http
-00002930: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00002940: 6e64 7265 6968 6172 2f74 6169 6275 6e2f  ndreihar/taibun/
-00002950: 6973 7375 6573 0d0d 0a5b 6f6e 6c69 6e65  issues...[online
-00002960: 2d64 6963 7469 6f6e 6172 795d 3a20 6874  -dictionary]: ht
-00002970: 7470 3a2f 2f69 7031 3934 3039 372e 6e74  tp://ip194097.nt
-00002980: 6375 2e65 6475 2e74 772f 756e 6769 616e  cu.edu.tw/ungian
-00002990: 2f73 6f61 6e6e 7465 6e67 2f63 6869 6c2f  /soannteng/chil/
-000029a0: 5461 6968 6f61 2e61 7370 0d0d 0a5b 6974  Taihoa.asp...[it
-000029b0: 6169 6769 2d64 6963 7469 6f6e 6172 795d  aigi-dictionary]
-000029c0: 3a20 6874 7470 733a 2f2f 6974 6169 6769  : https://itaigi
-000029d0: 2e74 772f 0d0d 0a5b 6461 7461 2d76 6961  .tw/...[data-via
-000029e0: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-000029f0: 622e 636f 6d2f 4368 686f 6554 6169 6769  b.com/ChhoeTaigi
-00002a00: 2f43 6868 6f65 5461 6967 6944 6174 6162  /ChhoeTaigiDatab
-00002a10: 6173 650d 0d0a 5b64 6174 612d 6363 5d3a  ase...[data-cc]:
-00002a20: 2068 7474 7073 3a2f 2f63 7265 6174 6976   https://creativ
-00002a30: 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963  ecommons.org/lic
-00002a40: 656e 7365 732f 6279 2d73 612f 342e 302f  enses/by-sa/4.0/
-00002a50: 6465 6564 2e65 6e0d 0d0a 5b73 616d 7565  deed.en...[samue
-00002a60: 6c2d 6769 7468 7562 5d3a 2068 7474 7073  l-github]: https
-00002a70: 3a2f 2f67 6974 6875 622e 636f 6d2f 5353  ://github.com/SS
-00002a80: 5361 6d0d 0d0a 5b73 616d 7565 6c2d 6c69  Sam...[samuel-li
-00002a90: 6e6b 6564 696e 5d3a 2068 7474 7073 3a2f  nkedin]: https:/
-00002aa0: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
-00002ab0: 6d2f 696e 2f73 616d 7565 6c2d 6a65 6e2f  m/in/samuel-jen/
-00002ac0: 0d0d 0a0d 0d0a 5b74 6169 6c6f 2d77 696b  ......[tailo-wik
-00002ad0: 695d 3a20 6874 7470 733a 2f2f 656e 2e77  i]: https://en.w
-00002ae0: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00002af0: 692f 5425 4333 2541 3269 2d75 2543 3325  i/T%C3%A2i-u%C3%
-00002b00: 4132 6e5f 4c25 4333 2542 342d 6d25 4333  A2n_L%C3%B4-m%C3
-00002b10: 2541 312d 6a25 4334 2541 425f 5068 696e  %A1-j%C4%AB_Phin
-00002b20: 672d 696d 5f48 6f6e 672d 2543 3325 4130  g-im_Hong-%C3%A0
-00002b30: 6e0d 0d0a 5b70 6f6a 2d77 696b 695d 3a20  n...[poj-wiki]: 
-00002b40: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00002b50: 6564 6961 2e6f 7267 2f77 696b 692f 5065  edia.org/wiki/Pe
-00002b60: 2543 4325 3844 682d 2543 3525 3844 652d  %CC%8Dh-%C5%8De-
-00002b70: 6a25 4334 2541 420d 0d0a 5b7a 6875 7969  j%C4%AB...[zhuyi
-00002b80: 6e2d 7769 6b69 5d3a 2068 7474 7073 3a2f  n-wiki]: https:/
-00002b90: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00002ba0: 672f 7769 6b69 2f54 6169 7761 6e65 7365  g/wiki/Taiwanese
-00002bb0: 5f50 686f 6e65 7469 635f 5379 6d62 6f6c  _Phonetic_Symbol
-00002bc0: 730d 0d0a 5b74 6c70 612d 7769 6b69 5d3a  s...[tlpa-wiki]:
-00002bd0: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
-00002be0: 7065 6469 612e 6f72 672f 7769 6b69 2f54  pedia.org/wiki/T
-00002bf0: 6169 7761 6e65 7365 5f4c 616e 6775 6167  aiwanese_Languag
-00002c00: 655f 5068 6f6e 6574 6963 5f41 6c70 6861  e_Phonetic_Alpha
-00002c10: 6265 740d 0d0a 5b70 696e 6779 696d 2d77  bet...[pingyim-w
-00002c20: 696b 695d 3a20 6874 7470 733a 2f2f 656e  iki]: https://en
-00002c30: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
-00002c40: 696b 692f 4262 2543 3325 4131 6e6c 2543  iki/Bb%C3%A1nl%C
-00002c50: 3325 4131 6d5f 7025 4333 2541 436e 6779  3%A1m_p%C3%ACngy
-00002c60: 2543 3425 4142 6d0d 0d0a 5b74 6f6e 6769  %C4%ABm...[tongi
-00002c70: 6f6e 672d 7769 6b69 5d3a 2068 7474 7073  ong-wiki]: https
-00002c80: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00002c90: 6f72 672f 7769 6b69 2f44 6125 4334 2541  org/wiki/Da%C4%A
-00002ca0: 422d 6768 2543 3325 4145 5f74 2543 3525  B-gh%C3%AE_t%C5%
-00002cb0: 3844 6e67 2d69 2543 3525 3844 6e67 5f70  8Dng-i%C5%8Dng_p
-00002cc0: 2543 3425 4142 6e67 2d69 6d0d 0d0a 5b7a  %C4%ABng-im...[z
-00002cd0: 6861 6e67 7a68 6f75 2d77 696b 695d 3a20  hangzhou-wiki]: 
-00002ce0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00002cf0: 6564 6961 2e6f 7267 2f77 696b 692f 5a68  edia.org/wiki/Zh
-00002d00: 616e 677a 686f 755f 6469 616c 6563 7473  angzhou_dialects
-00002d10: 0d0d 0a5b 7175 616e 7a68 6f75 2d77 696b  ...[quanzhou-wik
-00002d20: 695d 3a20 6874 7470 733a 2f2f 656e 2e77  i]: https://en.w
-00002d30: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00002d40: 692f 5175 616e 7a68 6f75 5f64 6961 6c65  i/Quanzhou_diale
-00002d50: 6374 730d 0d0a 5b6e 6c74 6b2d 746f 6b65  cts...[nltk-toke
-00002d60: 6e69 7a65 5d3a 2068 7474 7073 3a2f 2f6e  nize]: https://n
-00002d70: 6c74 6b2e 6f72 672f 6170 692f 6e6c 746b  ltk.org/api/nltk
-00002d80: 2e74 6f6b 656e 697a 652e 6874 6d6c 0d0d  .tokenize.html..
-00002d90: 0a5b 7361 6e64 6869 2d77 696b 695d 3a20  .[sandhi-wiki]: 
-00002da0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00002db0: 6564 6961 2e6f 7267 2f77 696b 692f 5461  edia.org/wiki/Ta
-00002dc0: 6977 616e 6573 655f 486f 6b6b 6965 6e23  iwanese_Hokkien#
-00002dd0: 546f 6e65 2532 3073 616e 6468 693a 7e3a  Tone%20sandhi:~:
-00002de0: 7465 7874 3d74 686e 6725 4532 2539 4625  text=thng%E2%9F%
-00002df0: 4139 2532 3028 2532 3273 6f75 7025 3232  A9%20(%22soup%22
-00002e00: 292e 2d2c 546f 6e65 2532 3073 616e 6468  ).-,Tone%20sandh
-00002e10: 692c 2d25 3542 6564 6974 2535 440d 0a    i,-%5Bedit%5D..
+000001b0: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
+000001c0: 6f64 7563 7469 6f6e 2f53 7461 626c 650d  oduction/Stable.
+000001d0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
+000001e0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+000001f0: 3a20 4465 7665 6c6f 7065 7273 0d0a 436c  : Developers..Cl
+00000200: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000220: 3a20 5079 7468 6f6e 203a 3a20 330d 0a43  : Python :: 3..C
+00000230: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
+00000240: 7469 6e67 2053 7973 7465 6d20 3a3a 2055  ting System :: U
+00000250: 6e69 780d 0a43 6c61 7373 6966 6965 723a  nix..Classifier:
+00000260: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
+00000270: 6d20 3a3a 204d 6163 4f53 203a 3a20 4d61  m :: MacOS :: Ma
+00000280: 634f 5320 580d 0a43 6c61 7373 6966 6965  cOS X..Classifie
+00000290: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000002a0: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+000002b0: 203a 3a20 5769 6e64 6f77 730d 0a52 6571   :: Windows..Req
+000002c0: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+000002d0: 332e 380d 0a44 6573 6372 6970 7469 6f6e  3.8..Description
+000002e0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000002f0: 6578 742f 6d61 726b 646f 776e 0d0a 4c69  ext/markdown..Li
+00000300: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+00000310: 4e53 450d 0a0d 0a3c 212d 2d20 5052 4f4a  NSE....<!-- PROJ
+00000320: 4543 5420 4c4f 474f 202d 2d3e 0d0a 3c62  ECT LOGO -->..<b
+00000330: 7220 2f3e 0d0a 3c64 6976 2061 6c69 676e  r />..<div align
+00000340: 3d22 6365 6e74 6572 223e 0d0a 2020 0d0a  ="center">..  ..
+00000350: 2320 5461 6962 756e 0d0a 0d0a 0d0a 0d0a  # Taibun........
+00000360: 3c21 2d2d 2050 524f 4a45 4354 2053 4849  <!-- PROJECT SHI
+00000370: 454c 4453 202d 2d3e 0d0a 5b21 5b54 6573  ELDS -->..[![Tes
+00000380: 7473 5d5b 7465 7374 732d 6261 6467 655d  ts][tests-badge]
+00000390: 5d5b 7465 7374 735d 0d0a 5b21 5b43 6f6e  ][tests]..[![Con
+000003a0: 7472 6962 7574 6f72 735d 5b63 6f6e 7472  tributors][contr
+000003b0: 6962 7574 6f72 732d 6261 6467 655d 5d5b  ibutors-badge]][
+000003c0: 636f 6e74 7269 6275 746f 7273 5d0d 0a5b  contributors]..[
+000003d0: 215b 5265 6c65 6173 655d 5b72 656c 6561  ![Release][relea
+000003e0: 7365 2d62 6164 6765 5d5d 5b72 656c 6561  se-badge]][relea
+000003f0: 7365 5d0d 0a5b 215b 4c69 6365 6e63 655d  se]..[![Licence]
+00000400: 5b6c 6963 656e 6365 2d62 6164 6765 5d5d  [licence-badge]]
+00000410: 5b6c 6963 656e 6365 5d0d 0a5b 215b 4c69  [licence]..[![Li
+00000420: 6e6b 6564 496e 5d5b 6c69 6e6b 6564 696e  nkedIn][linkedin
+00000430: 2d62 6164 6765 5d5d 5b6c 696e 6b65 6469  -badge]][linkedi
+00000440: 6e5d 0d0a 0d0a 2a2a 5461 6977 616e 6573  n]....**Taiwanes
+00000450: 6520 486f 6b6b 6965 6e20 5472 616e 736c  e Hokkien Transl
+00000460: 6974 6572 6174 6f72 2061 6e64 2054 6f6b  iterator and Tok
+00000470: 656e 6973 6572 2a2a 0d0a 0d0a 4974 2068  eniser**....It h
+00000480: 6173 206d 6574 686f 6473 2074 6861 7420  as methods that 
+00000490: 616c 6c6f 7720 746f 2063 7573 746f 6d69  allow to customi
+000004a0: 7365 2074 7261 6e73 6c69 7465 7261 7469  se transliterati
+000004b0: 6f6e 2061 6e64 2072 6574 7269 6576 6520  on and retrieve 
+000004c0: 616e 7920 6e65 6365 7373 6172 7920 696e  any necessary in
+000004d0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+000004e0: 5461 6977 616e 6573 6520 486f 6b6b 6965  Taiwanese Hokkie
+000004f0: 6e20 7072 6f6e 756e 6369 6174 696f 6e2e  n pronunciation.
+00000500: 3c62 7220 2f3e 0d0a 496e 636c 7564 6573  <br />..Includes
+00000510: 2077 6f72 6420 746f 6b65 6e69 7365 7220   word tokeniser 
+00000520: 666f 7220 5461 6977 616e 6573 6520 486f  for Taiwanese Ho
+00000530: 6b6b 6965 6e2e 0d0a 0d0a 5b52 6570 6f72  kkien.....[Repor
+00000540: 7420 4275 675d 5b62 7567 5d20 e280 a20d  t Bug][bug] ....
+00000550: 0a5b 5079 5049 5d5b 7079 7069 5d0d 0a0d  .[PyPI][pypi]...
+00000560: 0a3c 2f64 6976 3e0d 0a0d 0a0d 0a0d 0a2d  .</div>........-
+00000570: 2d2d 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2049  --........<!-- I
+00000580: 4e53 5441 4c4c 202d 2d3e 0d0a 2323 2049  NSTALL -->..## I
+00000590: 6e73 7461 6c6c 0d0a 0d0a 5461 6962 756e  nstall....Taibun
+000005a0: 2063 616e 2062 6520 696e 7374 616c 6c65   can be installe
+000005b0: 6420 6672 6f6d 205b 7079 7069 5d5b 7079  d from [pypi][py
+000005c0: 7069 5d0d 0a0d 0a60 6060 6261 7368 0d0a  pi]....```bash..
+000005d0: 2420 7069 7020 696e 7374 616c 6c20 7461  $ pip install ta
+000005e0: 6962 756e 0d0a 6060 600d 0a0d 0a0d 0a0d  ibun..```.......
+000005f0: 0a3c 212d 2d20 5553 4147 4520 2d2d 3e0d  .<!-- USAGE -->.
+00000600: 0a23 2320 5573 6167 650d 0a0d 0a23 2323  .## Usage....###
+00000610: 2043 6f6e 7665 7274 6572 0d0a 0d0a 6043   Converter....`C
+00000620: 6f6e 7665 7274 6572 6020 636c 6173 7320  onverter` class 
+00000630: 7472 616e 736c 6974 6572 6174 6573 2074  transliterates t
+00000640: 6865 2043 6869 6e65 7365 2063 6861 7261  he Chinese chara
+00000650: 6374 6572 7320 746f 2074 6865 2063 686f  cters to the cho
+00000660: 7365 6e20 7472 616e 736c 6974 6572 6174  sen transliterat
+00000670: 696f 6e20 7379 7374 656d 2077 6974 6820  ion system with 
+00000680: 7061 7261 6d65 7465 7273 2073 7065 6369  parameters speci
+00000690: 6669 6564 2062 7920 7468 6520 6465 7665  fied by the deve
+000006a0: 6c6f 7065 722e 2057 6f72 6b73 2066 6f72  loper. Works for
+000006b0: 2062 6f74 6820 5472 6164 6974 696f 6e61   both Traditiona
+000006c0: 6c20 616e 6420 5369 6d70 6c69 6669 6564  l and Simplified
+000006d0: 2063 6861 7261 6374 6572 732e 0d0a 0d0a   characters.....
+000006e0: 6060 6070 7974 686f 6e0d 0a23 2063 6f6e  ```python..# con
+000006f0: 7374 7275 6374 6f72 0d0a 6320 3d20 436f  structor..c = Co
+00000700: 6e76 6572 7465 7228 7379 7374 656d 2c20  nverter(system, 
+00000710: 6469 616c 6563 742c 2066 6f72 6d61 742c  dialect, format,
+00000720: 2064 656c 696d 6974 6572 2c20 7361 6e64   delimiter, sand
+00000730: 6869 2c20 7075 6e63 7475 6174 696f 6e2c  hi, punctuation,
+00000740: 2063 6f6e 7665 7274 5f6e 6f6e 5f63 6a6b   convert_non_cjk
+00000750: 290d 0a0d 0a23 2074 7261 6e73 6c69 7465  )....# translite
+00000760: 7261 7465 2043 6869 6e65 7365 2063 6861  rate Chinese cha
+00000770: 7261 6374 6572 730d 0a63 2e67 6574 2869  racters..c.get(i
+00000780: 6e70 7574 290d 0a60 6060 0d0a 0d0a 2323  nput)..```....##
+00000790: 2323 2053 7973 7465 6d0d 0a0d 0a60 7379  ## System....`sy
+000007a0: 7374 656d 6020 5374 7269 6e67 202d 2073  stem` String - s
+000007b0: 7973 7465 6d20 6f66 2074 7261 6e73 6c69  ystem of transli
+000007c0: 7465 7261 7469 6f6e 2e0d 0a0d 0a2a 2060  teration.....* `
+000007d0: 5461 696c 6f60 2028 6465 6661 756c 7429  Tailo` (default)
+000007e0: 202d 205b 54c3 a269 2d75 c3a2 6e20 4cc3   - [T..i-u..n L.
+000007f0: b42d 6dc3 a12d 6ac4 ab20 5068 696e 672d  .-m..-j.. Phing-
+00000800: 696d 2048 6f6e 672d c3a0 6e5d 5b74 6169  im Hong-..n][tai
+00000810: 6c6f 2d77 696b 695d 0d0a 2a20 6050 4f4a  lo-wiki]..* `POJ
+00000820: 6020 2d20 5b50 65cc 8d68 2dc5 8d65 2d6a  ` - [Pe..h-..e-j
+00000830: c4ab 5d5b 706f 6a2d 7769 6b69 5d0d 0a2a  ..][poj-wiki]..*
+00000840: 2060 5a68 7579 696e 6020 2d20 5b54 6169   `Zhuyin` - [Tai
+00000850: 7761 6e65 7365 2050 686f 6e65 7469 6320  wanese Phonetic 
+00000860: 5379 6d62 6f6c 735d 5b7a 6875 7969 6e2d  Symbols][zhuyin-
+00000870: 7769 6b69 5d0d 0a2a 2060 544c 5041 6020  wiki]..* `TLPA` 
+00000880: 2d20 5b54 6169 7761 6e65 7365 204c 616e  - [Taiwanese Lan
+00000890: 6775 6167 6520 5068 6f6e 6574 6963 2041  guage Phonetic A
+000008a0: 6c70 6861 6265 745d 5b74 6c70 612d 7769  lphabet][tlpa-wi
+000008b0: 6b69 5d0d 0a2a 2060 5069 6e67 7969 6d60  ki]..* `Pingyim`
+000008c0: 202d 205b 4262 c3a1 6e6c c3a1 6d20 55c4   - [Bb..nl..m U.
+000008d0: 9320 50c3 ac6e 6779 c4ab 6d20 48c5 8d6e  . P..ngy..m H..n
+000008e0: 6727 c3a0 6e5d 5b70 696e 6779 696d 2d77  g'..n][pingyim-w
+000008f0: 696b 695d 0d0a 2a20 6054 6f6e 6769 6f6e  iki]..* `Tongion
+00000900: 6760 202d 205b 4461 c4ab 2d67 68c3 ae20  g` - [Da..-gh.. 
+00000910: 54c5 8d6e 672d 69c5 8d6e 6720 50c4 ab6e  T..ng-i..ng P..n
+00000920: 672d 696d 5d5b 746f 6e67 696f 6e67 2d77  g-im][tongiong-w
+00000930: 696b 695d 0d0a 2a20 6049 5041 6020 2d20  iki]..* `IPA` - 
+00000940: 5b49 6e74 6572 6e61 7469 6f6e 616c 2050  [International P
+00000950: 686f 6e65 7469 6320 416c 7068 6162 6574  honetic Alphabet
+00000960: 5d5b 6970 612d 7769 6b69 5d0d 0a0d 0a7c  ][ipa-wiki]....|
+00000970: 2074 6578 7420 7c20 5461 696c 6f20 2020   text | Tailo   
+00000980: 7c20 504f 4a20 2020 2020 7c20 5a68 7579  | POJ     | Zhuy
+00000990: 696e 2020 2020 2020 7c20 544c 5041 2020  in      | TLPA  
+000009a0: 2020 2020 7c20 5069 6e67 7969 6d20 7c20      | Pingyim | 
+000009b0: 546f 6e67 696f 6e67 207c 2049 5041 2020  Tongiong | IPA  
+000009c0: 2020 2020 2020 207c 0d0a 7c20 2d2d 2d2d         |..| ----
+000009d0: 207c 202d 2d2d 2d2d 2d2d 207c 202d 2d2d   | ------- | ---
+000009e0: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+000009f0: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 207c  -- | --------- |
+00000a00: 202d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d   ------- | -----
+00000a10: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00000a20: 2d20 7c0d 0a7c 20e5 8fb0 e781 a320 7c20  - |..| ...... | 
+00000a30: 54c3 a269 2d75 c3a2 6e20 7c20 54c3 a269  T..i-u..n | T..i
+00000a40: 2d6f c3a2 6e20 7c20 e384 89e3 849e cb8a  -o..n | ........
+00000a50: 20e3 84a8 e384 a2cb 8a20 7c20 5461 6935   ........ | Tai5
+00000a60: 2075 616e 3520 7c20 44c3 a169 77c3 a16e   uan5 | D..iw..n
+00000a70: 2020 7c20 54c4 8169 2d75 c78e 6e20 207c    | T..i-u..n  |
+00000a80: 2054 6169 c2b2 e281 b520 7561 6ec2 b2e2   Tai..... uan...
+00000a90: 81b5 207c 0d0a 0d0a 2323 2323 2044 6961  .. |....#### Dia
+00000aa0: 6c65 6374 0d0a 0d0a 6064 6961 6c65 6374  lect....`dialect
+00000ab0: 6020 5374 7269 6e67 202d 2070 7265 6665  ` String - prefe
+00000ac0: 7272 6564 2070 726f 6e75 6e63 6961 7469  rred pronunciati
+00000ad0: 6f6e 2e0d 0a0d 0a2a 2060 736f 7574 6860  on.....* `south`
+00000ae0: 2028 6465 6661 756c 7429 202d 205b 5a68   (default) - [Zh
+00000af0: 616e 677a 686f 755d 5b7a 6861 6e67 7a68  angzhou][zhangzh
+00000b00: 6f75 2d77 696b 695d 2d6c 6561 6e69 6e67  ou-wiki]-leaning
+00000b10: 2070 726f 6e75 6e63 6961 7469 6f6e 0d0a   pronunciation..
+00000b20: 2a20 606e 6f72 7468 6020 2d20 5b51 7561  * `north` - [Qua
+00000b30: 6e7a 686f 755d 5b71 7561 6e7a 686f 752d  nzhou][quanzhou-
+00000b40: 7769 6b69 5d2d 6c65 616e 696e 6720 7072  wiki]-leaning pr
+00000b50: 6f6e 756e 6369 6174 696f 6e0d 0a0d 0a7c  onunciation....|
+00000b60: 2074 6578 7420 2020 7c20 736f 7574 6820   text   | south 
+00000b70: 2020 2020 2020 2020 7c20 6e6f 7274 6820          | north 
+00000b80: 2020 2020 2020 2020 7c0d 0a7c 202d 2d2d          |..| ---
+00000b90: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00000ba0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00000bb0: 2d2d 2d20 7c0d 0a7c 20e4 ba94 e69c 88e7  --- |..| .......
+00000bc0: af80 207c 2047 c58d 6f2d 6775 65cc 8d68  .. | G..o-gue..h
+00000bd0: 2d74 7365 6820 7c20 47c5 8d6f 2d67 65cc  -tseh | G..o-ge.
+00000be0: 8d68 2d74 7375 6568 207c 0d0a 0d0a 2323  .h-tsueh |....##
+00000bf0: 2323 2046 6f72 6d61 740d 0a0d 0a60 666f  ## Format....`fo
+00000c00: 726d 6174 6020 5374 7269 6e67 202d 2066  rmat` String - f
+00000c10: 6f72 6d61 7420 696e 2077 6869 6368 2074  ormat in which t
+00000c20: 6f6e 6573 2077 696c 6c20 6265 2072 6570  ones will be rep
+00000c30: 7265 7365 6e74 6564 2069 6e20 7468 6520  resented in the 
+00000c40: 636f 6e76 6572 7465 6420 7365 6e74 656e  converted senten
+00000c50: 6365 2e0d 0a0d 0a2a 2060 6d61 726b 6020  ce.....* `mark` 
+00000c60: 2864 6566 6175 6c74 2920 2d20 7573 6573  (default) - uses
+00000c70: 2064 6961 6372 6974 6963 7320 666f 7220   diacritics for 
+00000c80: 6561 6368 2073 796c 6c61 626c 652e 204e  each syllable. N
+00000c90: 6f74 2061 7661 696c 6162 6c65 2066 6f72  ot available for
+00000ca0: 2054 4c50 412e 0d0a 2a20 606e 756d 6265   TLPA...* `numbe
+00000cb0: 7260 202d 2061 6464 2061 206e 756d 6265  r` - add a numbe
+00000cc0: 7220 7768 6963 6820 7265 7072 6573 656e  r which represen
+00000cd0: 7473 2074 6865 2074 6f6e 6520 6174 2074  ts the tone at t
+00000ce0: 6865 2065 6e64 206f 6620 7468 6520 7379  he end of the sy
+00000cf0: 6c6c 6162 6c65 0d0a 2a20 6073 7472 6970  llable..* `strip
+00000d00: 6020 2d20 7265 6d6f 7665 7320 616e 7920  ` - removes any 
+00000d10: 746f 6e65 206d 6172 6b69 6e67 0d0a 0d0a  tone marking....
+00000d20: 7c20 7465 7874 207c 206d 6172 6b20 2020  | text | mark   
+00000d30: 207c 206e 756d 6265 7220 2020 207c 2073   | number    | s
+00000d40: 7472 6970 2020 207c 0d0a 7c20 2d2d 2d2d  trip   |..| ----
+00000d50: 207c 202d 2d2d 2d2d 2d2d 207c 202d 2d2d   | ------- | ---
+00000d60: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00000d70: 207c 0d0a 7c20 e58f b0e7 81a3 207c 2054   |..| ...... | T
+00000d80: c3a2 692d 75c3 a26e 207c 2054 6169 352d  ..i-u..n | Tai5-
+00000d90: 7561 6e35 207c 2054 6169 2d75 616e 207c  uan5 | Tai-uan |
+00000da0: 0d0a 0d0a 2323 2323 2044 656c 696d 6974  ....#### Delimit
+00000db0: 6572 0d0a 0d0a 6064 656c 696d 6974 6572  er....`delimiter
+00000dc0: 6020 5374 7269 6e67 202d 2073 6574 7320  ` String - sets 
+00000dd0: 7468 6520 6465 6c69 6d69 7465 7220 6368  the delimiter ch
+00000de0: 6172 6163 7465 7220 7468 6174 2077 696c  aracter that wil
+00000df0: 6c20 6265 2070 6c61 6365 6420 696e 2062  l be placed in b
+00000e00: 6574 7765 656e 2073 796c 6c61 626c 6573  etween syllables
+00000e10: 206f 6620 6120 776f 7264 2e0d 0a0d 0a44   of a word.....D
+00000e20: 6566 6175 6c74 2076 616c 7565 2064 6570  efault value dep
+00000e30: 656e 6473 206f 6e20 7468 6520 6368 6f73  ends on the chos
+00000e40: 656e 2060 7379 7374 656d 603a 0d0a 0d0a  en `system`:....
+00000e50: 2a20 6027 2d27 6020 2d20 666f 7220 6054  * `'-'` - for `T
+00000e60: 6169 6c6f 602c 2060 504f 4a60 2c20 6054  ailo`, `POJ`, `T
+00000e70: 6f6e 6769 6f6e 6760 0d0a 2a20 6027 2760  ongiong`..* `''`
+00000e80: 202d 2066 6f72 2060 5069 6e67 7969 6d60   - for `Pingyim`
+00000e90: 0d0a 2a20 6027 2027 6020 2d20 666f 7220  ..* `' '` - for 
+00000ea0: 605a 6875 7969 6e60 2c20 6054 4c50 4160  `Zhuyin`, `TLPA`
+00000eb0: 2c20 6049 5041 600d 0a0d 0a7c 2074 6578  , `IPA`....| tex
+00000ec0: 7420 7c20 272d 2720 2020 2020 7c20 2727  t | '-'     | ''
+00000ed0: 2020 2020 207c 2027 2027 2020 2020 207c       | ' '     |
+00000ee0: 0d0a 7c20 2d2d 2d2d 207c 202d 2d2d 2d2d  ..| ---- | -----
+00000ef0: 2d2d 207c 202d 2d2d 2d2d 2d20 7c20 2d2d  -- | ------ | --
+00000f00: 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0 e781  ----- |..| .....
+00000f10: a320 7c20 54c3 a269 2d75 c3a2 6e20 7c20  . | T..i-u..n | 
+00000f20: 54c3 a269 75c3 a26e 207c 2054 c3a2 6920  T..iu..n | T..i 
+00000f30: 75c3 a26e 207c 0d0a 0d0a 2323 2323 2053  u..n |....#### S
+00000f40: 616e 6468 690d 0a0d 0a60 7361 6e64 6869  andhi....`sandhi
+00000f50: 6020 5374 7269 6e67 202d 2061 7070 6c69  ` String - appli
+00000f60: 6573 2074 6865 205b 7361 6e64 6869 2072  es the [sandhi r
+00000f70: 756c 6573 206f 6620 5461 6977 616e 6573  ules of Taiwanes
+00000f80: 6520 486f 6b6b 6965 6e5d 5b73 616e 6468  e Hokkien][sandh
+00000f90: 692d 7769 6b69 5d20 746f 2073 796c 6c61  i-wiki] to sylla
+00000fa0: 626c 6573 206f 6620 6120 7369 6e67 6c65  bles of a single
+00000fb0: 2077 6f72 642e 0d0a 0d0a 5369 6e63 6520   word.....Since 
+00000fc0: 6974 2773 2064 6966 6669 6375 6c74 2074  it's difficult t
+00000fd0: 6f20 656e 636f 6465 2061 6c6c 2073 616e  o encode all san
+00000fe0: 6468 6920 7275 6c65 732c 2054 6169 6275  dhi rules, Taibu
+00000ff0: 6e20 7072 6f76 6964 6573 206d 756c 7469  n provides multi
+00001000: 706c 6520 6d6f 6465 7320 666f 7220 7361  ple modes for sa
+00001010: 6e64 6869 2063 6f6e 7665 7273 696f 6e20  ndhi conversion 
+00001020: 746f 2061 6c6c 6f77 2066 6f72 2063 7573  to allow for cus
+00001030: 746f 6d69 7365 6420 7361 6e64 6869 2068  tomised sandhi h
+00001040: 616e 646c 696e 672e 0d0a 0d0a 2a20 606e  andling.....* `n
+00001050: 6f6e 6560 202d 2064 6f65 736e 2774 2070  one` - doesn't p
+00001060: 6572 666f 726d 2061 6e79 2074 6f6e 6520  erform any tone 
+00001070: 7361 6e64 6869 0d0a 2a20 6061 7574 6f60  sandhi..* `auto`
+00001080: 202d 2063 6c6f 7365 7374 2061 7070 726f   - closest appro
+00001090: 7869 6d61 7469 6f6e 2074 6f20 6675 6c6c  ximation to full
+000010a0: 2063 6f72 7265 6374 2074 6f6e 6520 7361   correct tone sa
+000010b0: 6e64 6869 206f 6620 5461 6977 616e 6573  ndhi of Taiwanes
+000010c0: 652c 2077 6974 6820 7072 6f70 6572 2073  e, with proper s
+000010d0: 616e 6468 6920 6f66 2070 726f 6e6f 756e  andhi of pronoun
+000010e0: 732c 2073 7566 6669 7865 732c 2061 6e64  s, suffixes, and
+000010f0: 2077 6f72 6473 2077 6974 6820 e4bb 940d   words with ....
+00001100: 0a2a 2060 6578 635f 6c61 7374 6020 2d20  .* `exc_last` - 
+00001110: 6368 616e 6765 7320 746f 6e65 2066 6f72  changes tone for
+00001120: 2065 7665 7279 2073 796c 6c61 626c 6520   every syllable 
+00001130: 6578 6365 7074 2066 6f72 2074 6865 206c  except for the l
+00001140: 6173 7420 6f6e 650d 0a2a 2060 696e 636c  ast one..* `incl
+00001150: 5f6c 6173 7460 202d 2063 6861 6e67 6573  _last` - changes
+00001160: 2074 6f6e 6520 666f 7220 6576 6572 7920   tone for every 
+00001170: 7379 6c6c 6162 6c65 2069 6e63 6c75 6469  syllable includi
+00001180: 6e67 2074 6865 206c 6173 7420 6f6e 650d  ng the last one.
+00001190: 0a0d 0a44 6566 6175 6c74 2076 616c 7565  ...Default value
+000011a0: 2064 6570 656e 6473 206f 6e20 7468 6520   depends on the 
+000011b0: 6368 6f73 656e 2060 7379 7374 656d 603a  chosen `system`:
+000011c0: 0d0a 0d0a 2a20 6061 7574 6f60 202d 2066  ....* `auto` - f
+000011d0: 6f72 2060 546f 6e67 696f 6e67 600d 0a2a  or `Tongiong`..*
+000011e0: 2060 6e6f 6e65 6020 2d20 666f 7220 6054   `none` - for `T
+000011f0: 6169 6c6f 602c 2060 504f 4a60 2c20 605a  ailo`, `POJ`, `Z
+00001200: 6875 7969 6e60 2c20 6054 4c50 4160 2c20  huyin`, `TLPA`, 
+00001210: 6050 696e 6779 696d 602c 2060 4950 4160  `Pingyim`, `IPA`
+00001220: 0d0a 0d0a 7c20 7465 7874 2020 2020 2020  ....| text      
+00001230: 2020 207c 206e 6f6e 6520 2020 2020 2020     | none       
+00001240: 2020 2020 2020 2020 2020 7c20 6175 746f            | auto
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 207c 2065 7863 5f6c 6173 7420 2020 2020   | exc_last     
+00001270: 2020 2020 2020 2020 7c20 696e 636c 5f6c          | incl_l
+00001280: 6173 7420 2020 2020 2020 2020 2020 207c  ast            |
+00001290: 0d0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..| ------------
+000012a0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+000012b0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+000012c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+000012d0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000012e0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+000012f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a  ------------ |..
+00001300: 7c20 e980 99e6 98af e58f b0e7 81a3 e59b  | ..............
+00001310: a1e4 bb94 207c 2054 7365 2073 c4ab 2054  .... | Tse s.. T
+00001320: c3a2 692d 75c3 a26e 2067 c3ad 6e2d c3a1  ..i-u..n g..n-..
+00001330: 207c 2054 7365 2073 c3ac 2054 c481 692d   | Tse s.. T..i-
+00001340: 75c4 816e 2067 696e 2dc3 a120 7c20 5473  u..n gin-.. | Ts
+00001350: c493 2073 c3ac 2054 c481 692d 75c4 816e  .. s.. T..i-u..n
+00001360: 2067 696e 2dc3 a120 7c20 5473 c493 2073   gin-.. | Ts.. s
+00001370: c3ac 2054 c481 692d 75c4 816e 2067 696e  .. T..i-u..n gin
+00001380: 2d61 207c 0d0a 0d0a 5361 6e64 6869 2072  -a |....Sandhi r
+00001390: 756c 6573 2061 6c73 6f20 6368 616e 6765  ules also change
+000013a0: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
+000013b0: 6520 6469 616c 6563 7420 6368 6f73 656e  e dialect chosen
+000013c0: 2e0d 0a0d 0a7c 2074 6578 7420 7c20 6e6f  .....| text | no
+000013d0: 2073 616e 6468 6920 7c20 736f 7574 6820   sandhi | south 
+000013e0: 2020 7c20 6e6f 7274 6820 2020 7c0d 0a7c    | north   |..|
+000013f0: 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d   ---- | --------
+00001400: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
+00001410: 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0 e781  ----- |..| .....
+00001420: a320 7c20 54c3 a269 2d75 c3a2 6e20 2020  . | T..i-u..n   
+00001430: 7c20 54c4 8169 2d75 c3a2 6e20 7c20 54c3  | T..i-u..n | T.
+00001440: a069 2d75 c3a2 6e20 7c0d 0a0d 0a23 2323  .i-u..n |....###
+00001450: 2320 5075 6e63 7475 6174 696f 6e0d 0a0d  # Punctuation...
+00001460: 0a60 7075 6e63 7475 6174 696f 6e60 2053  .`punctuation` S
+00001470: 7472 696e 670d 0a0d 0a2a 2060 666f 726d  tring....* `form
+00001480: 6174 6020 2864 6566 6175 6c74 2920 2d20  at` (default) - 
+00001490: 636f 6e76 6572 7473 2043 6869 6e65 7365  converts Chinese
+000014a0: 2d73 7479 6c65 2070 756e 6374 7561 7469  -style punctuati
+000014b0: 6f6e 2074 6f20 4c61 7469 6e2d 7374 796c  on to Latin-styl
+000014c0: 6520 7075 6e63 7475 6174 696f 6e20 616e  e punctuation an
+000014d0: 6420 6361 7069 7461 6c69 7365 7320 776f  d capitalises wo
+000014e0: 7264 7320 6174 2074 6865 2062 6567 696e  rds at the begin
+000014f0: 6e69 6e67 206f 6620 6561 6368 2073 656e  ning of each sen
+00001500: 7465 6e63 652e 0d0a 2a20 606e 6f6e 6560  tence...* `none`
+00001510: 202d 2070 7265 7365 7276 6573 2043 6869   - preserves Chi
+00001520: 6e65 7365 2d73 7479 6c65 2070 756e 6374  nese-style punct
+00001530: 7561 7469 6f6e 2061 6e64 2064 6f65 736e  uation and doesn
+00001540: 2774 2063 6170 6974 616c 6973 6520 776f  't capitalise wo
+00001550: 7264 7320 6174 2074 6865 2062 6567 696e  rds at the begin
+00001560: 6e69 6e67 206f 6620 6e65 7720 7365 6e74  ning of new sent
+00001570: 656e 6365 732e 0d0a 0d0a 7c20 7465 7874  ences.....| text
+00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2020 2020 2020 2020 207c 2066 6f72             | for
+000015d0: 6d61 7420 2020 2020 2020 2020 2020 2020  mat             
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001630: 206e 6f6e 6520 2020 2020 2020 2020 2020   none           
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001690: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
+000016a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016e0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
+000016f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+00001750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017b0: 2d2d 2d2d 207c 0d0a 7c20 e980 99e6 98af  ---- |..| ......
+000017c0: e887 bae5 8d97 efbc 8ce7 b0a1 e7a8 b1e3  ................
+000017d0: 808c e58d 97e3 808d efbc 88e7 99bd e8a9  ................
+000017e0: b1e5 ad97 efbc 9a54 c3a2 692d 6cc3 a26d  .......T..i-l..m
+000017f0: efbc 9be6 b3a8 e99f b3e7 aca6 e899 9fef  ................
+00001800: bc9a e384 8ae3 849e cb8a 20e3 848b e384  .......... .....
+00001810: a2cb 8aef bc8c e59c 8be8 aa9e efbc 9a54  ...............T
+00001820: c3a1 696e c3a1 6eef bc89 e380 8220 7c20  ..in..n...... | 
+00001830: 5473 6520 73c4 ab20 54c3 a269 2d6c c3a2  Tse s.. T..i-l..
+00001840: 6d2c 206b c3a1 6e2d 7473 6869 6e67 2022  m, k..n-tshing "
+00001850: 6cc3 a26d 2220 2850 65cc 8d68 2d75 c493  l..m" (Pe..h-u..
+00001860: 2d6a c4ab 3a20 54c3 a269 2d6c c3a2 6d3b  -j..: T..i-l..m;
+00001870: 2074 73c3 b92d 696d 2068 c3bb 2d68 c58d   ts..-im h..-h..
+00001880: 3a20 e384 8ae3 849e cb8a 20e3 848b e384  : ........ .....
+00001890: a2cb 8a2c 206b 6f6b 2d67 c3ad 3a20 54c3  ..., kok-g..: T.
+000018a0: a169 6ec3 a16e 292e 207c 2074 7365 2073  .in..n). | tse s
+000018b0: c4ab 2054 c3a2 692d 6cc3 a26d efbc 8c6b  .. T..i-l..m...k
+000018c0: c3a1 6e2d 7473 6869 6e67 e380 8c6c c3a2  ..n-tshing...l..
+000018d0: 6de3 808d efbc 8850 65cc 8d68 2d75 c493  m......Pe..h-u..
+000018e0: 2d6a c4ab efbc 9a54 c3a2 692d 6cc3 a26d  -j.....T..i-l..m
+000018f0: efbc 9b74 73c3 b92d 696d 2068 c3bb 2d68  ...ts..-im h..-h
+00001900: c58d efbc 9ae3 848a e384 9ecb 8a20 e384  ............. ..
+00001910: 8be3 84a2 cb8a efbc 8c6b 6f6b 2d67 c3ad  .........kok-g..
+00001920: efbc 9a54 c3a1 696e c3a1 6eef bc89 e380  ...T..in..n.....
+00001930: 8220 7c0d 0a0d 0a23 2323 2320 436f 6e76  . |....#### Conv
+00001940: 6572 7420 6e6f 6e2d 434a 4b0d 0a0d 0a60  ert non-CJK....`
+00001950: 636f 6e76 6572 745f 6e6f 6e5f 636a 6b60  convert_non_cjk`
+00001960: 2042 6f6f 6c65 616e 202d 2064 6566 696e   Boolean - defin
+00001970: 6573 2077 6865 7468 6572 206f 7220 6e6f  es whether or no
+00001980: 7420 746f 2063 6f6e 7665 7274 206e 6f6e  t to convert non
+00001990: 2d43 6869 6e65 7365 2077 6f72 6473 2e20  -Chinese words. 
+000019a0: 4361 6e20 6265 2075 7365 6420 746f 2063  Can be used to c
+000019b0: 6f6e 7665 7274 2054 6169 6c6f 2074 6f20  onvert Tailo to 
+000019c0: 616e 6f74 6865 7220 726f 6d61 6e69 7361  another romanisa
+000019d0: 7469 6f6e 2073 7973 7465 6d2e 0d0a 0d0a  tion system.....
+000019e0: 2a20 6054 7275 6560 202d 2063 6f6e 7665  * `True` - conve
+000019f0: 7274 206e 6f6e 2d43 6869 6e65 7365 2063  rt non-Chinese c
+00001a00: 6861 7261 6374 6572 2077 6f72 6473 0d0a  haracter words..
+00001a10: 2a20 6046 616c 7365 6020 2864 6566 6175  * `False` (defau
+00001a20: 6c74 2920 2d20 636f 6e76 6572 7420 6f6e  lt) - convert on
+00001a30: 6c79 2043 6869 6e65 7365 2063 6861 7261  ly Chinese chara
+00001a40: 6374 6572 2077 6f72 6473 0d0a 0d0a 7c20  cter words....| 
+00001a50: 7465 7874 2020 2020 2020 7c20 4661 6c73  text      | Fals
+00001a60: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00001a70: 2020 2020 7c20 5472 7565 2020 2020 2020      | True      
+00001a80: 2020 2020 2020 2020 2020 2020 2020 7c0d                |.
+00001a90: 0a7c 202d 2d2d 2d2d 2d2d 2d2d 207c 202d  .| --------- | -
+00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ab0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ad0: 207c 0d0a 7c20 e688 91e9 a39f 7068 c3a1   |..| ......ph..
+00001ae0: 6e67 207c 20e3 86a3 e384 a8e3 849a cb8b  ng | ...........
+00001af0: 20e3 8490 e384 a7e3 849a e386 b7cb 9920   .............. 
+00001b00: 7068 c3a1 6e67 207c 20e3 86a3 e384 a8e3  ph..ng | .......
+00001b10: 849a cb8b 20e3 8490 e384 a7e3 849a e386  .... ...........
+00001b20: b7cb 9920 e384 86e3 84a4 cb8b 207c 0d0a  ... ........ |..
+00001b30: 0d0a 2323 2320 546f 6b65 6e69 7365 720d  ..### Tokeniser.
+00001b40: 0a0d 0a60 546f 6b65 6e69 7365 7260 2063  ...`Tokeniser` c
+00001b50: 6c61 7373 2070 6572 666f 726d 7320 5b4e  lass performs [N
+00001b60: 4c54 4b20 776f 7264 7075 6e63 745f 746f  LTK wordpunct_to
+00001b70: 6b65 6e69 7a65 5d5b 6e6c 746b 2d74 6f6b  kenize][nltk-tok
+00001b80: 656e 697a 655d 2d6c 696b 6520 746f 6b65  enize]-like toke
+00001b90: 6e69 7361 7469 6f6e 206f 6620 6120 5461  nisation of a Ta
+00001ba0: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
+00001bb0: 7365 6e74 656e 6365 2e0d 0a0d 0a60 6060  sentence.....```
+00001bc0: 7079 7468 6f6e 0d0a 2320 636f 6e73 7472  python..# constr
+00001bd0: 7563 746f 720d 0a74 203d 2054 6f6b 656e  uctor..t = Token
+00001be0: 6973 6572 2829 0d0a 0d0a 2320 746f 6b65  iser()....# toke
+00001bf0: 6e69 7365 2054 6169 7761 6e65 7365 2048  nise Taiwanese H
+00001c00: 6f6b 6b69 656e 2073 656e 7465 6e63 650d  okkien sentence.
+00001c10: 0a74 2e74 6f6b 656e 6973 6528 696e 7075  .t.tokenise(inpu
+00001c20: 7429 0d0a 6060 600d 0a0d 0a23 2323 204f  t)..```....### O
+00001c30: 7468 6572 2046 756e 6374 696f 6e73 0d0a  ther Functions..
+00001c40: 0d0a 6060 6070 7974 686f 6e0d 0a23 2043  ..```python..# C
+00001c50: 6f6e 7665 7274 2074 6f20 5472 6164 6974  onvert to Tradit
+00001c60: 696f 6e61 6c0d 0a74 6f5f 7472 6164 6974  ional..to_tradit
+00001c70: 696f 6e61 6c28 696e 7075 7429 0d0a 0d0a  ional(input)....
+00001c80: 2320 436f 6e76 6572 7420 746f 2053 696d  # Convert to Sim
+00001c90: 706c 6966 6965 640d 0a74 6f5f 7369 6d70  plified..to_simp
+00001ca0: 6c69 6669 6564 2869 6e70 7574 290d 0a0d  lified(input)...
+00001cb0: 0a23 2043 6865 636b 2069 6620 7468 6520  .# Check if the 
+00001cc0: 7374 7269 6e67 2069 7320 6675 6c6c 7920  string is fully 
+00001cd0: 636f 6d70 6f73 6564 206f 6620 4368 696e  composed of Chin
+00001ce0: 6573 6520 6368 6172 6163 7465 7273 0d0a  ese characters..
+00001cf0: 6973 5f63 6a6b 2869 6e70 7574 290d 0a60  is_cjk(input)..`
+00001d00: 6060 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2045  ``........<!-- E
+00001d10: 5841 4d50 4c45 202d 2d3e 0d0a 2323 2045  XAMPLE -->..## E
+00001d20: 7861 6d70 6c65 0d0a 0d0a 6060 6070 7974  xample....```pyt
+00001d30: 686f 6e0d 0a23 2043 6f6e 7665 7274 6572  hon..# Converter
+00001d40: 0d0a 6672 6f6d 2074 6169 6275 6e20 696d  ..from taibun im
+00001d50: 706f 7274 2043 6f6e 7665 7274 6572 0d0a  port Converter..
+00001d60: 0d0a 2323 2053 7973 7465 6d0d 0a63 203d  ..## System..c =
+00001d70: 2043 6f6e 7665 7274 6572 2829 2023 2054   Converter() # T
+00001d80: 6169 6c6f 2073 7973 7465 6d20 6465 6661  ailo system defa
+00001d90: 756c 740d 0a63 2e67 6574 2827 e585 88e7  ult..c.get('....
+00001da0: 949f e8ac 9bef bc8c e5ad b8e7 949f e681  ................
+00001db0: ace6 81ac e881 bde3 8082 2729 0d0a 3e3e  ..........')..>>
+00001dc0: 2053 6961 6e2d 7369 6e6e 206b c3b3 6e67   Sian-sinn k..ng
+00001dd0: 2c20 6861 cc8d 6b2d 7369 6e67 2074 69c4  , ha..k-sing ti.
+00001de0: 816d 2d74 69c4 816d 2074 6869 616e 6e2e  .m-ti..m thiann.
+00001df0: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00001e00: 7228 7379 7374 656d 3d27 5a68 7579 696e  r(system='Zhuyin
+00001e10: 2729 0d0a 632e 6765 7428 27e5 8588 e794  ')..c.get('.....
+00001e20: 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6 81ac  ................
+00001e30: e681 ace8 81bd e380 8227 290d 0a3e 3e20  .........')..>> 
+00001e40: e384 92e3 84a7 e384 a220 e384 92e3 86aa  ......... ......
+00001e50: 20e3 848d e386 b2cb 8b2c 20e3 848f e384   ........, .....
+00001e60: 9ae3 86b6 cb99 20e3 8492 e384 a7e3 84a5  ...... .........
+00001e70: 20e3 8489 e384 a7e3 86b0 cbab 20e3 8489   ........... ...
+00001e80: e384 a7e3 86b0 cbab 20e3 848a e384 a7e3  ........ .......
+00001e90: 86a9 2e0d 0a0d 0a23 2320 4469 616c 6563  .......## Dialec
+00001ea0: 740d 0a63 203d 2043 6f6e 7665 7274 6572  t..c = Converter
+00001eb0: 2829 2023 2073 6f75 7468 2064 6961 6c65  () # south diale
+00001ec0: 6374 2064 6566 6175 6c74 0d0a 632e 6765  ct default..c.ge
+00001ed0: 7428 22e6 8891 e6ac b2e7 94a8 e7ae b8e9  t(".............
+00001ee0: a39f e9ad 9a22 290d 0a3e 3e20 4775 c3a1  .....")..>> Gu..
+00001ef0: 2062 6568 20c4 ab6e 6720 74c4 ab20 7473   beh ..ng t.. ts
+00001f00: 6961 cc8d 6820 68c3 ae0d 0a0d 0a63 203d  ia..h h......c =
+00001f10: 2043 6f6e 7665 7274 6572 2864 6961 6c65   Converter(diale
+00001f20: 6374 3d27 6e6f 7274 6827 290d 0a63 2e67  ct='north')..c.g
+00001f30: 6574 2822 e688 91e6 acb2 e794 a8e7 aeb8  et("............
+00001f40: e9a3 9fe9 ad9a 2229 0d0a 3e3e 2047 75c3  ......")..>> Gu.
+00001f50: a120 6275 6568 20c4 ab6e 6720 74c5 ab20  . bueh ..ng t.. 
+00001f60: 7473 6961 cc8d 6820 68c3 bb0d 0a0d 0a23  tsia..h h......#
+00001f70: 2320 466f 726d 6174 0d0a 6320 3d20 436f  # Format..c = Co
+00001f80: 6e76 6572 7465 7228 2920 2320 666f 7220  nverter() # for 
+00001f90: 5461 696c 6f2c 206d 6172 6b20 6279 2064  Tailo, mark by d
+00001fa0: 6566 6175 6c74 0d0a 632e 6765 7428 22e7  efault..c.get(".
+00001fb0: 949f e697 a5e5 bfab e6a8 8222 290d 0a3e  ...........")..>
+00001fc0: 3e20 5365 6e6e 2d6a 69cc 8d74 206b 6875  > Senn-ji..t khu
+00001fd0: c3a0 692d 6c6f cc8d 6b0d 0a0d 0a63 203d  ..i-lo..k....c =
+00001fe0: 2043 6f6e 7665 7274 6572 2866 6f72 6d61   Converter(forma
+00001ff0: 743d 276e 756d 6265 7227 290d 0a63 2e67  t='number')..c.g
+00002000: 6574 2822 e794 9fe6 97a5 e5bf abe6 a882  et("............
+00002010: 2229 0d0a 3e3e 2053 656e 6e31 2d6a 6974  ")..>> Senn1-jit
+00002020: 3820 6b68 7561 6933 2d6c 6f6b 380d 0a0d  8 khuai3-lok8...
+00002030: 0a63 203d 2043 6f6e 7665 7274 6572 2866  .c = Converter(f
+00002040: 6f72 6d61 743d 2773 7472 6970 2729 0d0a  ormat='strip')..
+00002050: 632e 6765 7428 22e7 949f e697 a5e5 bfab  c.get(".........
+00002060: e6a8 8222 290d 0a3e 3e20 5365 6e6e 2d6a  ...")..>> Senn-j
+00002070: 6974 206b 6875 6169 2d6c 6f6b 0d0a 0d0a  it khuai-lok....
+00002080: 2323 2044 656c 696d 6974 6572 0d0a 6320  ## Delimiter..c 
+00002090: 3d20 436f 6e76 6572 7465 7228 6465 6c69  = Converter(deli
+000020a0: 6d69 7465 723d 2727 290d 0a63 2e67 6574  miter='')..c.get
+000020b0: 2822 e585 88e7 949f e8ac 9bef bc8c e5ad  ("..............
+000020c0: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
+000020d0: 2229 0d0a 3e3e 2053 6961 6e73 696e 6e20  ")..>> Siansinn 
+000020e0: 6bc3 b36e 672c 2068 61cc 8d6b 7369 6e67  k..ng, ha..ksing
+000020f0: 2074 69c4 816d 7469 c481 6d20 7468 6961   ti..mti..m thia
+00002100: 6e6e 2e0d 0a0d 0a63 203d 2043 6f6e 7665  nn.....c = Conve
+00002110: 7274 6572 2873 7973 7465 6d3d 2750 696e  rter(system='Pin
+00002120: 6779 696d 272c 2064 656c 696d 6974 6572  gyim', delimiter
+00002130: 3d27 2d27 290d 0a63 2e67 6574 2822 e585  ='-')..c.get("..
+00002140: 88e7 949f e8ac 9bef bc8c e5ad b8e7 949f  ................
+00002150: e681 ace6 81ac e881 bde3 8082 2229 0d0a  ............")..
+00002160: 3e3e 2053 69c4 816e 2d73 6ec4 ab20 67c7  >> Si..n-sn.. g.
+00002170: 926e 672c 2068 c3a1 672d 73c4 ab6e 6720  .ng, h..g-s..ng 
+00002180: 6469 c3a2 6d2d 6469 c3a2 6d20 7469 6ec4  di..m-di..m tin.
+00002190: 812e 0d0a 0d0a 2323 2053 616e 6468 690d  ......## Sandhi.
+000021a0: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
+000021b0: 2023 2066 6f72 2054 6169 6c6f 2c20 7361   # for Tailo, sa
+000021c0: 6e64 6869 206e 6f6e 6520 6279 2064 6566  ndhi none by def
+000021d0: 6175 6c74 0d0a 632e 6765 7428 22e9 8099  ault..c.get("...
+000021e0: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+000021f0: 290d 0a3e 3e20 5473 6520 73c4 ab20 54c3  )..>> Tse s.. T.
+00002200: a269 2d75 c3a2 6e20 67c3 ad6e 2dc3 a10d  .i-u..n g..n-...
+00002210: 0a0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
+00002220: 2873 616e 6468 693d 2761 7574 6f27 290d  (sandhi='auto').
+00002230: 0a63 2e67 6574 2822 e980 99e6 98af e58f  .c.get("........
+00002240: b0e7 81a3 e59b a1e4 bb94 2229 0d0a 3e3e  ..........")..>>
+00002250: 2054 7365 2073 c3ac 2054 c481 692d 75c4   Tse s.. T..i-u.
+00002260: 816e 2067 696e 2dc3 a10d 0a0d 0a63 203d  .n gin-......c =
+00002270: 2043 6f6e 7665 7274 6572 2873 616e 6468   Converter(sandh
+00002280: 693d 2765 7863 5f6c 6173 7427 290d 0a63  i='exc_last')..c
+00002290: 2e67 6574 2822 e980 99e6 98af e58f b0e7  .get("..........
+000022a0: 81a3 e59b a1e4 bb94 2229 0d0a 3e3e 2054  ........")..>> T
+000022b0: 73c4 9320 73c3 ac20 54c4 8169 2d75 c481  s.. s.. T..i-u..
+000022c0: 6e20 6769 6e2d c3a1 0d0a 0d0a 6320 3d20  n gin-......c = 
+000022d0: 436f 6e76 6572 7465 7228 7361 6e64 6869  Converter(sandhi
+000022e0: 3d27 696e 636c 5f6c 6173 7427 290d 0a63  ='incl_last')..c
+000022f0: 2e67 6574 2822 e980 99e6 98af e58f b0e7  .get("..........
+00002300: 81a3 e59b a1e4 bb94 2229 0d0a 3e3e 2054  ........")..>> T
+00002310: 73c4 9320 73c3 ac20 54c4 8169 2d75 c481  s.. s.. T..i-u..
+00002320: 6e20 6769 6e2d 610d 0a0d 0a23 2320 5075  n gin-a....## Pu
+00002330: 6e63 7475 6174 696f 6e0d 0a63 203d 2043  nctuation..c = C
+00002340: 6f6e 7665 7274 6572 2829 2023 2066 6f72  onverter() # for
+00002350: 6d61 7420 7075 6e63 7475 6174 696f 6e20  mat punctuation 
+00002360: 6465 6661 756c 740d 0a63 2e67 6574 2822  default..c.get("
+00002370: e5a4 aae7 a9ba e69c 8be5 8f8b efbc 8ce6  ................
+00002380: 8181 e5a5 bdef bc81 e681 81e9 a39f e9a3  ................
+00002390: bde6 9caa efbc 9f22 290d 0a3e 3e20 5468  .......")..>> Th
+000023a0: c3a0 692d 6b68 6f6e 6720 70c3 ae6e 672d  ..i-khong p..ng-
+000023b0: 69c3 ba2c 206c c3ad 6e2d 68c3 b321 204c  i.., l..n-h..! L
+000023c0: c3ad 6e20 7473 6961 cc8d 682d 70c3 a120  ..n tsia..h-p.. 
+000023d0: 6275 c493 3f0d 0a0d 0a63 203d 2043 6f6e  bu..?....c = Con
+000023e0: 7665 7274 6572 2870 756e 6374 7561 7469  verter(punctuati
+000023f0: 6f6e 3d27 6e6f 6e65 2729 0d0a 632e 6765  on='none')..c.ge
+00002400: 7428 22e5 a4aa e7a9 bae6 9c8b e58f 8bef  t(".............
+00002410: bc8c e681 81e5 a5bd efbc 81e6 8181 e9a3  ................
+00002420: 9fe9 a3bd e69c aaef bc9f 2229 0d0a 3e3e  ..........")..>>
+00002430: 2074 68c3 a069 2d6b 686f 6e67 2070 c3ae   th..i-khong p..
+00002440: 6e67 2d69 c3ba efbc 8c6c c3ad 6e2d 68c3  ng-i.....l..n-h.
+00002450: b3ef bc81 6cc3 ad6e 2074 7369 61cc 8d68  ....l..n tsia..h
+00002460: 2d70 c3a1 2062 75c4 93ef bc9f 0d0a 0d0a  -p.. bu.........
+00002470: 2323 2043 6f6e 7665 7274 206e 6f6e 2d43  ## Convert non-C
+00002480: 4a4b 0d0a 6320 3d20 436f 6e76 6572 7428  JK..c = Convert(
+00002490: 7379 7374 656d 3d27 5a68 7579 696e 2729  system='Zhuyin')
+000024a0: 2023 2046 616c 7365 2063 6f6e 7665 7274   # False convert
+000024b0: 5f6e 6f6e 5f63 6a6b 2064 6566 6175 6c74  _non_cjk default
+000024c0: 0d0a 632e 6765 7428 22e6 8891 e9a3 9f70  ..c.get("......p
+000024d0: 68c3 a16e 6722 290d 0a3e 3e20 e386 a3e3  h..ng")..>> ....
+000024e0: 84a8 e384 9acb 8b20 e384 90e3 84a7 e384  ....... ........
+000024f0: 9ae3 86b7 cb99 2070 68c3 a16e 670d 0a0d  ...... ph..ng...
+00002500: 0a63 203d 2043 6f6e 7665 7274 2873 7973  .c = Convert(sys
+00002510: 7465 6d3d 275a 6875 7969 6e27 2c20 636f  tem='Zhuyin', co
+00002520: 6e76 6572 745f 6e6f 6e5f 636a 6b3d 5472  nvert_non_cjk=Tr
+00002530: 7565 290d 0a63 2e67 6574 2822 e688 91e9  ue)..c.get("....
+00002540: a39f 7068 c3a1 6e67 2229 0d0a 3e3e 20e3  ..ph..ng")..>> .
+00002550: 86a3 e384 a8e3 849a cb8b 20e3 8490 e384  .......... .....
+00002560: a7e3 849a e386 b7cb 9920 e384 86e3 84a4  ......... ......
+00002570: cb8b 0d0a 0d0a 0d0a 2320 546f 6b65 6e69  ........# Tokeni
+00002580: 7365 720d 0a66 726f 6d20 7461 6962 756e  ser..from taibun
+00002590: 2069 6d70 6f72 7420 546f 6b65 6e69 7365   import Tokenise
+000025a0: 720d 0a0d 0a74 203d 2054 6f6b 656e 6973  r....t = Tokenis
+000025b0: 6572 2829 0d0a 742e 746f 6b65 6e69 7365  er()..t.tokenise
+000025c0: 2822 e5a4 aae7 a9ba e69c 8be5 8f8b efbc  ("..............
+000025d0: 8ce6 8181 e5a5 bdef bc81 e681 81e9 a39f  ................
+000025e0: e9a3 bde6 9caa efbc 9f22 290d 0a3e 3e20  .........")..>> 
+000025f0: 5b27 e5a4 aae7 a9ba 272c 2027 e69c 8be5  ['......', '....
+00002600: 8f8b 272c 2027 efbc 8c27 2c20 27e6 8181  ..', '...', '...
+00002610: e5a5 bd27 2c20 27ef bc81 272c 2027 e681  ...', '...', '..
+00002620: 8127 2c20 27e9 a39f e9a3 bd27 2c20 27e6  .', '......', '.
+00002630: 9caa 272c 2027 efbc 9f27 5d0d 0a0d 0a0d  ..', '...'].....
+00002640: 0a23 204f 7468 6572 2046 756e 6374 696f  .# Other Functio
+00002650: 6e73 0d0a 6672 6f6d 2074 6169 6275 6e20  ns..from taibun 
+00002660: 696d 706f 7274 2074 6f5f 7472 6164 6974  import to_tradit
+00002670: 696f 6e61 6c2c 2074 6f5f 7369 6d70 6c69  ional, to_simpli
+00002680: 6669 6564 2c20 6973 5f63 6a6b 0d0a 0d0a  fied, is_cjk....
+00002690: 746f 5f74 7261 6469 7469 6f6e 616c 2822  to_traditional("
+000026a0: e688 91e5 90ac e697 a0e5 8fb0 e6b9 bee8  ................
+000026b0: af9d 2229 0d0a 3e3e 20e6 8891 e881 bde7  ..")..>> .......
+000026c0: 84a1 e58f b0e7 81a3 e8a9 b10d 0a0d 0a74  ...............t
+000026d0: 6f5f 7369 6d70 6c69 6669 6564 2822 e688  o_simplified("..
+000026e0: 91e8 81bd e784 a1e8 87ba e781 a3e8 a9b1  ................
+000026f0: 2229 0d0a 3e3e 20e6 8891 e590 ace6 97a0  ")..>> .........
+00002700: e58f b0e6 b9be e8af 9d0d 0a0d 0a69 735f  .............is_
+00002710: 636a 6b28 27e6 8891 e9a3 9fe9 baad 2729  cjk('.........')
+00002720: 0d0a 3e3e 2054 7275 650d 0a0d 0a69 735f  ..>> True....is_
+00002730: 636a 6b28 27e6 8891 e9a3 9f70 68c3 a16e  cjk('......ph..n
+00002740: 6727 290d 0a3e 3e20 4661 6c73 650d 0a60  g')..>> False..`
+00002750: 6060 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2044  ``........<!-- D
+00002760: 4154 4120 2d2d 3e0d 0a23 2320 4461 7461  ATA -->..## Data
+00002770: 0d0a 0d0a 2d20 5b54 6169 7761 6e65 7365  ....- [Taiwanese
+00002780: 2d43 6869 6e65 7365 204f 6e6c 696e 6520  -Chinese Online 
+00002790: 4469 6374 696f 6e61 7279 5d5b 6f6e 6c69  Dictionary][onli
+000027a0: 6e65 2d64 6963 7469 6f6e 6172 795d 2028  ne-dictionary] (
+000027b0: 7669 6120 5b43 6868 6f65 5461 6967 695d  via [ChhoeTaigi]
+000027c0: 5b64 6174 612d 7669 615d 290d 0a2d 205b  [data-via])..- [
+000027d0: 6954 6169 6769 2043 6869 6e65 7365 2d54  iTaigi Chinese-T
+000027e0: 6169 7761 6e65 7365 2043 6f6d 7061 7269  aiwanese Compari
+000027f0: 736f 6e20 4469 6374 696f 6e61 7279 5d5b  son Dictionary][
+00002800: 6974 6169 6769 2d64 6963 7469 6f6e 6172  itaigi-dictionar
+00002810: 795d 2028 7669 6120 5b43 6868 6f65 5461  y] (via [ChhoeTa
+00002820: 6967 695d 5b64 6174 612d 7669 615d 290d  igi][data-via]).
+00002830: 0a0d 0a0d 0a0d 0a3c 212d 2d20 4143 4b4e  .......<!-- ACKN
+00002840: 4f57 4c45 4447 454d 454e 5453 202d 2d3e  OWLEDGEMENTS -->
+00002850: 0d0a 2323 2041 636b 6e6f 776c 6564 6765  ..## Acknowledge
+00002860: 6d65 6e74 730d 0a0d 0a2d 2053 616d 7565  ments....- Samue
+00002870: 6c20 4a65 6e20 285b 4769 7468 7562 5d5b  l Jen ([Github][
+00002880: 7361 6d75 656c 2d67 6974 6875 625d 20c2  samuel-github] .
+00002890: b720 5b4c 696e 6b65 6449 6e5d 5b73 616d  . [LinkedIn][sam
+000028a0: 7565 6c2d 6c69 6e6b 6564 696e 5d29 202d  uel-linkedin]) -
+000028b0: 2054 6169 7761 6e65 7365 2061 6e64 204d   Taiwanese and M
+000028c0: 616e 6461 7269 6e20 7472 616e 736c 6174  andarin translat
+000028d0: 696f 6e0d 0a0d 0a0d 0a0d 0a3c 212d 2d20  ion........<!-- 
+000028e0: 4c49 4345 4e43 4520 2d2d 3e0d 0a23 2320  LICENCE -->..## 
+000028f0: 4c69 6365 6e63 650d 0a0d 0a42 6563 6175  Licence....Becau
+00002900: 7365 2054 6169 6275 6e20 6973 204d 4954  se Taibun is MIT
+00002910: 2d6c 6963 656e 7365 642c 2061 6e79 2064  -licensed, any d
+00002920: 6576 656c 6f70 6572 2063 616e 2065 7373  eveloper can ess
+00002930: 656e 7469 616c 6c79 2064 6f20 7768 6174  entially do what
+00002940: 6576 6572 2074 6865 7920 7761 6e74 2077  ever they want w
+00002950: 6974 6820 6974 2061 7320 6c6f 6e67 2061  ith it as long a
+00002960: 7320 7468 6579 2069 6e63 6c75 6465 2074  s they include t
+00002970: 6865 206f 7269 6769 6e61 6c20 636f 7079  he original copy
+00002980: 7269 6768 7420 616e 6420 6c69 6365 6e63  right and licenc
+00002990: 6520 6e6f 7469 6365 2069 6e20 616e 7920  e notice in any 
+000029a0: 636f 7069 6573 206f 6620 7468 6520 736f  copies of the so
+000029b0: 7572 6365 2063 6f64 652e 204e 6f74 652c  urce code. Note,
+000029c0: 2074 6861 7420 7468 6520 6461 7461 2075   that the data u
+000029d0: 7365 6420 6279 2074 6865 2070 6163 6b61  sed by the packa
+000029e0: 6765 2069 7320 6c69 6365 6e73 6564 2075  ge is licensed u
+000029f0: 6e64 6572 2061 2064 6966 6665 7265 6e74  nder a different
+00002a00: 2063 6f70 7972 6967 6874 2e0d 0a0d 0a54   copyright.....T
+00002a10: 6865 2064 6174 6120 6973 206c 6963 656e  he data is licen
+00002a20: 7365 6420 756e 6465 7220 5b43 4320 4259  sed under [CC BY
+00002a30: 2d53 4120 342e 305d 5b64 6174 612d 6363  -SA 4.0][data-cc
+00002a40: 5d0d 0a0d 0a0d 0a0d 0a3c 212d 2d20 4d41  ]........<!-- MA
+00002a50: 524b 444f 574e 204c 494e 4b53 202d 2d3e  RKDOWN LINKS -->
+00002a60: 0d0a 5b74 6573 7473 5d3a 2068 7474 7073  ..[tests]: https
+00002a70: 3a2f 2f67 6974 6875 622e 636f 6d2f 616e  ://github.com/an
+00002a80: 6472 6569 6861 722f 7461 6962 756e 2f61  dreihar/taibun/a
+00002a90: 6374 696f 6e73 0d0a 5b74 6573 7473 2d62  ctions..[tests-b
+00002aa0: 6164 6765 5d3a 2068 7474 7073 3a2f 2f69  adge]: https://i
+00002ab0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00002ac0: 7468 7562 2f61 6374 696f 6e73 2f77 6f72  thub/actions/wor
+00002ad0: 6b66 6c6f 772f 7374 6174 7573 2f61 6e64  kflow/status/and
+00002ae0: 7265 6968 6172 2f74 6169 6275 6e2f 6369  reihar/taibun/ci
+00002af0: 2e79 616d 6c3f 7374 796c 653d 666f 722d  .yaml?style=for-
+00002b00: 7468 652d 6261 6467 6526 6c6f 676f 3d67  the-badge&logo=g
+00002b10: 6974 6875 620d 0a5b 636f 6e74 7269 6275  ithub..[contribu
+00002b20: 746f 7273 2d62 6164 6765 5d3a 2068 7474  tors-badge]: htt
+00002b30: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00002b40: 2e69 6f2f 6769 7468 7562 2f63 6f6e 7472  .io/github/contr
+00002b50: 6962 7574 6f72 732f 616e 6472 6569 6861  ibutors/andreiha
+00002b60: 722f 7461 6962 756e 3f73 7479 6c65 3d66  r/taibun?style=f
+00002b70: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b63  or-the-badge..[c
+00002b80: 6f6e 7472 6962 7574 6f72 735d 3a20 2375  ontributors]: #u
+00002b90: 7361 6765 0d0a 5b72 656c 6561 7365 2d62  sage..[release-b
+00002ba0: 6164 6765 5d3a 2068 7474 7073 3a2f 2f69  adge]: https://i
+00002bb0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00002bc0: 7468 7562 2f76 2f72 656c 6561 7365 2f61  thub/v/release/a
+00002bd0: 6e64 7265 6968 6172 2f74 6169 6275 6e3f  ndreihar/taibun?
+00002be0: 636f 6c6f 723d 3338 3631 3863 2673 7479  color=38618c&sty
+00002bf0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00002c00: 0d0a 5b72 656c 6561 7365 5d3a 2068 7474  ..[release]: htt
+00002c10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002c20: 616e 6472 6569 6861 722f 7461 6962 756e  andreihar/taibun
+00002c30: 2f72 656c 6561 7365 730d 0a5b 6c69 6365  /releases..[lice
+00002c40: 6e63 652d 6261 6467 655d 3a20 6874 7470  nce-badge]: http
+00002c50: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00002c60: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+00002c70: 652f 616e 6472 6569 6861 722f 7461 6962  e/andreihar/taib
+00002c80: 756e 3f63 6f6c 6f72 3d30 3030 3030 3026  un?color=000000&
+00002c90: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
+00002ca0: 6467 650d 0a5b 6c69 6365 6e63 655d 3a20  dge..[licence]: 
+00002cb0: 4c49 4345 4e53 450d 0a5b 6c69 6e6b 6564  LICENSE..[linked
+00002cc0: 696e 2d62 6164 6765 5d3a 2068 7474 7073  in-badge]: https
+00002cd0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00002ce0: 6f2f 6261 6467 652f 4c69 6e6b 6564 496e  o/badge/LinkedIn
+00002cf0: 2d30 3037 3742 353f 7374 796c 653d 666f  -0077B5?style=fo
+00002d00: 722d 7468 652d 6261 6467 6526 6c6f 676f  r-the-badge&logo
+00002d10: 3d6c 696e 6b65 6469 6e26 6c6f 676f 436f  =linkedin&logoCo
+00002d20: 6c6f 723d 7768 6974 650d 0a5b 6c69 6e6b  lor=white..[link
+00002d30: 6564 696e 5d3a 2068 7474 7073 3a2f 2f77  edin]: https://w
+00002d40: 7777 2e6c 696e 6b65 6469 6e2e 636f 6d2f  ww.linkedin.com/
+00002d50: 696e 2f61 6e64 7265 692d 6861 7262 6163  in/andrei-harbac
+00002d60: 686f 762f 0d0a 0d0a 5b70 7970 695d 3a20  hov/....[pypi]: 
+00002d70: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00002d80: 2f70 726f 6a65 6374 2f74 6169 6275 6e0d  /project/taibun.
+00002d90: 0a5b 6275 675d 3a20 6874 7470 733a 2f2f  .[bug]: https://
+00002da0: 6769 7468 7562 2e63 6f6d 2f61 6e64 7265  github.com/andre
+00002db0: 6968 6172 2f74 6169 6275 6e2f 6973 7375  ihar/taibun/issu
+00002dc0: 6573 0d0a 5b6f 6e6c 696e 652d 6469 6374  es..[online-dict
+00002dd0: 696f 6e61 7279 5d3a 2068 7474 703a 2f2f  ionary]: http://
+00002de0: 6970 3139 3430 3937 2e6e 7463 752e 6564  ip194097.ntcu.ed
+00002df0: 752e 7477 2f75 6e67 6961 6e2f 736f 616e  u.tw/ungian/soan
+00002e00: 6e74 656e 672f 6368 696c 2f54 6169 686f  nteng/chil/Taiho
+00002e10: 612e 6173 700d 0a5b 6974 6169 6769 2d64  a.asp..[itaigi-d
+00002e20: 6963 7469 6f6e 6172 795d 3a20 6874 7470  ictionary]: http
+00002e30: 733a 2f2f 6974 6169 6769 2e74 772f 0d0a  s://itaigi.tw/..
+00002e40: 5b64 6174 612d 7669 615d 3a20 6874 7470  [data-via]: http
+00002e50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f43  s://github.com/C
+00002e60: 6868 6f65 5461 6967 692f 4368 686f 6554  hhoeTaigi/ChhoeT
+00002e70: 6169 6769 4461 7461 6261 7365 0d0a 5b64  aigiDatabase..[d
+00002e80: 6174 612d 6363 5d3a 2068 7474 7073 3a2f  ata-cc]: https:/
+00002e90: 2f63 7265 6174 6976 6563 6f6d 6d6f 6e73  /creativecommons
+00002ea0: 2e6f 7267 2f6c 6963 656e 7365 732f 6279  .org/licenses/by
+00002eb0: 2d73 612f 342e 302f 6465 6564 2e65 6e0d  -sa/4.0/deed.en.
+00002ec0: 0a5b 7361 6d75 656c 2d67 6974 6875 625d  .[samuel-github]
+00002ed0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00002ee0: 2e63 6f6d 2f53 5353 616d 0d0a 5b73 616d  .com/SSSam..[sam
+00002ef0: 7565 6c2d 6c69 6e6b 6564 696e 5d3a 2068  uel-linkedin]: h
+00002f00: 7474 7073 3a2f 2f77 7777 2e6c 696e 6b65  ttps://www.linke
+00002f10: 6469 6e2e 636f 6d2f 696e 2f73 616d 7565  din.com/in/samue
+00002f20: 6c2d 6a65 6e2f 0d0a 0d0a 5b74 6169 6c6f  l-jen/....[tailo
+00002f30: 2d77 696b 695d 3a20 6874 7470 733a 2f2f  -wiki]: https://
+00002f40: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+00002f50: 2f77 696b 692f 5425 4333 2541 3269 2d75  /wiki/T%C3%A2i-u
+00002f60: 2543 3325 4132 6e5f 4c25 4333 2542 342d  %C3%A2n_L%C3%B4-
+00002f70: 6d25 4333 2541 312d 6a25 4334 2541 425f  m%C3%A1-j%C4%AB_
+00002f80: 5068 696e 672d 696d 5f48 6f6e 672d 2543  Phing-im_Hong-%C
+00002f90: 3325 4130 6e0d 0a5b 706f 6a2d 7769 6b69  3%A0n..[poj-wiki
+00002fa0: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
+00002fb0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00002fc0: 2f50 6525 4343 2538 4468 2d25 4335 2538  /Pe%CC%8Dh-%C5%8
+00002fd0: 4465 2d6a 2543 3425 4142 0d0a 5b7a 6875  De-j%C4%AB..[zhu
+00002fe0: 7969 6e2d 7769 6b69 5d3a 2068 7474 7073  yin-wiki]: https
+00002ff0: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00003000: 6f72 672f 7769 6b69 2f54 6169 7761 6e65  org/wiki/Taiwane
+00003010: 7365 5f50 686f 6e65 7469 635f 5379 6d62  se_Phonetic_Symb
+00003020: 6f6c 730d 0a5b 746c 7061 2d77 696b 695d  ols..[tlpa-wiki]
+00003030: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
+00003040: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00003050: 5461 6977 616e 6573 655f 4c61 6e67 7561  Taiwanese_Langua
+00003060: 6765 5f50 686f 6e65 7469 635f 416c 7068  ge_Phonetic_Alph
+00003070: 6162 6574 0d0a 5b70 696e 6779 696d 2d77  abet..[pingyim-w
+00003080: 696b 695d 3a20 6874 7470 733a 2f2f 656e  iki]: https://en
+00003090: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+000030a0: 696b 692f 4262 2543 3325 4131 6e6c 2543  iki/Bb%C3%A1nl%C
+000030b0: 3325 4131 6d5f 7025 4333 2541 436e 6779  3%A1m_p%C3%ACngy
+000030c0: 2543 3425 4142 6d0d 0a5b 746f 6e67 696f  %C4%ABm..[tongio
+000030d0: 6e67 2d77 696b 695d 3a20 6874 7470 733a  ng-wiki]: https:
+000030e0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+000030f0: 7267 2f77 696b 692f 4461 2543 3425 4142  rg/wiki/Da%C4%AB
+00003100: 2d67 6825 4333 2541 455f 7425 4335 2538  -gh%C3%AE_t%C5%8
+00003110: 446e 672d 6925 4335 2538 446e 675f 7025  Dng-i%C5%8Dng_p%
+00003120: 4334 2541 426e 672d 696d 0d0a 5b69 7061  C4%ABng-im..[ipa
+00003130: 2d77 696b 695d 3a20 6874 7470 733a 2f2f  -wiki]: https://
+00003140: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+00003150: 2f77 696b 692f 496e 7465 726e 6174 696f  /wiki/Internatio
+00003160: 6e61 6c5f 5068 6f6e 6574 6963 5f41 6c70  nal_Phonetic_Alp
+00003170: 6861 6265 740d 0a5b 7a68 616e 677a 686f  habet..[zhangzho
+00003180: 752d 7769 6b69 5d3a 2068 7474 7073 3a2f  u-wiki]: https:/
+00003190: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+000031a0: 672f 7769 6b69 2f5a 6861 6e67 7a68 6f75  g/wiki/Zhangzhou
+000031b0: 5f64 6961 6c65 6374 730d 0a5b 7175 616e  _dialects..[quan
+000031c0: 7a68 6f75 2d77 696b 695d 3a20 6874 7470  zhou-wiki]: http
+000031d0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+000031e0: 2e6f 7267 2f77 696b 692f 5175 616e 7a68  .org/wiki/Quanzh
+000031f0: 6f75 5f64 6961 6c65 6374 730d 0a5b 6e6c  ou_dialects..[nl
+00003200: 746b 2d74 6f6b 656e 697a 655d 3a20 6874  tk-tokenize]: ht
+00003210: 7470 733a 2f2f 6e6c 746b 2e6f 7267 2f61  tps://nltk.org/a
+00003220: 7069 2f6e 6c74 6b2e 746f 6b65 6e69 7a65  pi/nltk.tokenize
+00003230: 2e68 746d 6c0d 0a5b 7361 6e64 6869 2d77  .html..[sandhi-w
+00003240: 696b 695d 3a20 6874 7470 733a 2f2f 656e  iki]: https://en
+00003250: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00003260: 696b 692f 5461 6977 616e 6573 655f 486f  iki/Taiwanese_Ho
+00003270: 6b6b 6965 6e23 546f 6e65 2532 3073 616e  kkien#Tone%20san
+00003280: 6468 693a 7e3a 7465 7874 3d74 686e 6725  dhi:~:text=thng%
+00003290: 4532 2539 4625 4139 2532 3028 2532 3273  E2%9F%A9%20(%22s
+000032a0: 6f75 7025 3232 292e 2d2c 546f 6e65 2532  oup%22).-,Tone%2
+000032b0: 3073 616e 6468 692c 2d25 3542 6564 6974  0sandhi,-%5Bedit
+000032c0: 2535 440d 0a                             %5D..
```

### Comparing `taibun-1.0.0/README.md` & `taibun-1.1.0/taibun.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,669 +1,813 @@
-00000000: 3c21 2d2d 2050 524f 4a45 4354 204c 4f47  <!-- PROJECT LOG
-00000010: 4f20 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c  O -->..<br />..<
-00000020: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00000030: 7222 3e0d 0a20 203c 6120 6872 6566 3d22  r">..  <a href="
-00000040: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000050: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
-00000060: 6275 6e22 3e0d 0a20 2020 203c 696d 6720  bun">..    <img 
-00000070: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000080: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000090: 6e74 2e63 6f6d 2f61 6e64 7265 6968 6172  nt.com/andreihar
-000000a0: 2f74 6169 6275 6e2f 6d61 696e 2f72 6561  /taibun/main/rea
-000000b0: 646d 652f 6c6f 676f 2e70 6e67 2220 616c  dme/logo.png" al
-000000c0: 743d 224c 6f67 6f22 2077 6964 7468 3d22  t="Logo" width="
-000000d0: 3930 2220 6865 6967 6874 3d22 3830 223e  90" height="80">
-000000e0: 0d0a 2020 3c2f 613e 0d0a 2020 0d0a 2320  ..  </a>..  ..# 
-000000f0: 5461 6962 756e 0d0a 0d0a 0d0a 0d0a 3c21  Taibun........<!
-00000100: 2d2d 2050 524f 4a45 4354 2053 4849 454c  -- PROJECT SHIEL
-00000110: 4453 202d 2d3e 0d0a 5b21 5b54 6573 7473  DS -->..[![Tests
-00000120: 5d5b 7465 7374 732d 6261 6467 655d 5d5b  ][tests-badge]][
-00000130: 7465 7374 735d 0d0a 5b21 5b43 6f6e 7472  tests]..[![Contr
-00000140: 6962 7574 6f72 735d 5b63 6f6e 7472 6962  ibutors][contrib
-00000150: 7574 6f72 732d 6261 6467 655d 5d5b 636f  utors-badge]][co
-00000160: 6e74 7269 6275 746f 7273 5d0d 0a5b 215b  ntributors]..[![
-00000170: 5265 6c65 6173 655d 5b72 656c 6561 7365  Release][release
-00000180: 2d62 6164 6765 5d5d 5b72 656c 6561 7365  -badge]][release
-00000190: 5d0d 0a5b 215b 4c69 6365 6e63 655d 5b6c  ]..[![Licence][l
-000001a0: 6963 656e 6365 2d62 6164 6765 5d5d 5b6c  icence-badge]][l
-000001b0: 6963 656e 6365 5d0d 0a5b 215b 4c69 6e6b  icence]..[![Link
-000001c0: 6564 496e 5d5b 6c69 6e6b 6564 696e 2d62  edIn][linkedin-b
-000001d0: 6164 6765 5d5d 5b6c 696e 6b65 6469 6e5d  adge]][linkedin]
-000001e0: 0d0a 0d0a 2a2a 5461 6977 616e 6573 6520  ....**Taiwanese 
-000001f0: 486f 6b6b 6965 6e20 5472 616e 736c 6974  Hokkien Translit
-00000200: 6572 6174 6f72 2061 6e64 2054 6f6b 656e  erator and Token
-00000210: 6973 6572 2a2a 0d0a 0d0a 4974 2068 6173  iser**....It has
-00000220: 206d 6574 686f 6473 2074 6861 7420 616c   methods that al
-00000230: 6c6f 7720 746f 2063 7573 746f 6d69 7365  low to customise
-00000240: 2074 7261 6e73 6c69 7465 7261 7469 6f6e   transliteration
-00000250: 2061 6e64 2072 6574 7269 6576 6520 616e   and retrieve an
-00000260: 7920 6e65 6365 7373 6172 7920 696e 666f  y necessary info
-00000270: 726d 6174 696f 6e20 6162 6f75 7420 5461  rmation about Ta
-00000280: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
-00000290: 7072 6f6e 756e 6369 6174 696f 6e2e 3c62  pronunciation.<b
-000002a0: 7220 2f3e 0d0a 496e 636c 7564 6573 2077  r />..Includes w
-000002b0: 6f72 6420 746f 6b65 6e69 7365 7220 666f  ord tokeniser fo
-000002c0: 7220 5461 6977 616e 6573 6520 486f 6b6b  r Taiwanese Hokk
-000002d0: 6965 6e2e 0d0a 0d0a 5b52 6570 6f72 7420  ien.....[Report 
-000002e0: 4275 675d 5b62 7567 5d20 e280 a20d 0a5b  Bug][bug] .....[
-000002f0: 5079 5049 5d5b 7079 7069 5d0d 0a0d 0a3c  PyPI][pypi]....<
-00000300: 2f64 6976 3e0d 0a0d 0a0d 0a0d 0a2d 2d2d  /div>........---
-00000310: 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2054 4142  ........<!-- TAB
-00000320: 4c45 204f 4620 434f 4e54 454e 5453 202d  LE OF CONTENTS -
-00000330: 2d3e 0d0a 3c64 6574 6169 6c73 206f 7065  ->..<details ope
-00000340: 6e3e 0d0a 2020 3c73 756d 6d61 7279 3e54  n>..  <summary>T
-00000350: 6162 6c65 206f 6620 436f 6e74 656e 7473  able of Contents
-00000360: 3c2f 7375 6d6d 6172 793e 0d0a 2020 3c6f  </summary>..  <o
-00000370: 6c3e 0d0a 2020 2020 3c6c 693e 3c61 2068  l>..    <li><a h
-00000380: 7265 663d 2223 696e 7374 616c 6c22 3e49  ref="#install">I
-00000390: 6e73 7461 6c6c 3c2f 613e 3c2f 6c69 3e0d  nstall</a></li>.
-000003a0: 0a20 2020 203c 6c69 3e0d 0a20 2020 2020  .    <li>..     
-000003b0: 203c 6120 6872 6566 3d22 2375 7361 6765   <a href="#usage
-000003c0: 223e 5573 6167 653c 2f61 3e0d 0a20 2020  ">Usage</a>..   
-000003d0: 2020 203c 756c 3e0d 0a20 2020 2020 2020     <ul>..       
-000003e0: 203c 6c69 3e0d 0a20 2020 2020 2020 2020   <li>..         
-000003f0: 203c 6120 6872 6566 3d22 2363 6f6e 7665   <a href="#conve
-00000400: 7274 6572 223e 436f 6e76 6572 7465 723c  rter">Converter<
-00000410: 2f61 3e0d 0a20 2020 2020 2020 2020 203c  /a>..          <
-00000420: 756c 3e0d 0a20 2020 2020 2020 2020 2020  ul>..           
-00000430: 203c 6c69 3e3c 6120 6872 6566 3d22 2373   <li><a href="#s
-00000440: 7973 7465 6d22 3e53 7973 7465 6d3c 2f61  ystem">System</a
-00000450: 3e3c 2f6c 693e 0d0a 2020 2020 2020 2020  ></li>..        
-00000460: 2020 2020 3c6c 693e 3c61 2068 7265 663d      <li><a href=
-00000470: 2223 6469 616c 6563 7422 3e44 6961 6c65  "#dialect">Diale
-00000480: 6374 3c2f 613e 3c2f 6c69 3e0d 0a20 2020  ct</a></li>..   
-00000490: 2020 2020 2020 2020 203c 6c69 3e3c 6120           <li><a 
-000004a0: 6872 6566 3d22 2366 6f72 6d61 7422 3e46  href="#format">F
-000004b0: 6f72 6d61 743c 2f61 3e3c 2f6c 693e 0d0a  ormat</a></li>..
-000004c0: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
-000004d0: 3c61 2068 7265 663d 2223 6465 6c69 6d69  <a href="#delimi
-000004e0: 7465 7222 3e44 656c 696d 6974 6572 3c2f  ter">Delimiter</
-000004f0: 613e 3c2f 6c69 3e0d 0a20 2020 2020 2020  a></li>..       
-00000500: 2020 2020 203c 6c69 3e3c 6120 6872 6566       <li><a href
-00000510: 3d22 2373 616e 6468 6922 3e53 616e 6468  ="#sandhi">Sandh
-00000520: 693c 2f61 3e3c 2f6c 693e 0d0a 2020 2020  i</a></li>..    
-00000530: 2020 2020 2020 2020 3c6c 693e 3c61 2068          <li><a h
-00000540: 7265 663d 2223 7075 6e63 7475 6174 696f  ref="#punctuatio
-00000550: 6e22 3e50 756e 6374 7561 7469 6f6e 3c2f  n">Punctuation</
-00000560: 613e 3c2f 6c69 3e0d 0a20 2020 2020 2020  a></li>..       
-00000570: 2020 203c 2f75 6c3e 0d0a 2020 2020 2020     </ul>..      
-00000580: 2020 3c2f 6c69 3e0d 0a20 2020 2020 2020    </li>..       
-00000590: 203c 6c69 3e3c 6120 6872 6566 3d22 2374   <li><a href="#t
-000005a0: 6f6b 656e 6973 6572 223e 546f 6b65 6e69  okeniser">Tokeni
-000005b0: 7365 723c 2f61 3e3c 2f6c 693e 0d0a 2020  ser</a></li>..  
-000005c0: 2020 2020 3c2f 756c 3e0d 0a20 2020 203c      </ul>..    <
-000005d0: 2f6c 693e 0d0a 2020 2020 3c6c 693e 3c61  /li>..    <li><a
-000005e0: 2068 7265 663d 2223 6578 616d 706c 6522   href="#example"
-000005f0: 3e45 7861 6d70 6c65 3c2f 613e 3c2f 6c69  >Example</a></li
-00000600: 3e0d 0a20 2020 203c 6c69 3e3c 6120 6872  >..    <li><a hr
-00000610: 6566 3d22 2364 6174 6122 3e44 6174 613c  ef="#data">Data<
-00000620: 2f61 3e3c 2f6c 693e 0d0a 2020 2020 3c6c  /a></li>..    <l
-00000630: 693e 3c61 2068 7265 663d 2223 6c69 6365  i><a href="#lice
-00000640: 6e63 6522 3e4c 6963 656e 6365 3c2f 613e  nce">Licence</a>
-00000650: 3c2f 6c69 3e0d 0a20 203c 2f6f 6c3e 0d0a  </li>..  </ol>..
-00000660: 3c2f 6465 7461 696c 733e 0d0a 0d0a 0d0a  </details>......
-00000670: 0d0a 3c21 2d2d 2049 4e53 5441 4c4c 202d  ..<!-- INSTALL -
-00000680: 2d3e 0d0a 2323 2049 6e73 7461 6c6c 0d0a  ->..## Install..
-00000690: 0d0a 5461 6962 756e 2063 616e 2062 6520  ..Taibun can be 
-000006a0: 696e 7374 616c 6c65 6420 6672 6f6d 205b  installed from [
-000006b0: 7079 7069 5d5b 7079 7069 5d0d 0a0d 0a60  pypi][pypi]....`
-000006c0: 6060 6261 7368 0d0a 2420 7069 7020 696e  ``bash..$ pip in
-000006d0: 7374 616c 6c20 7461 6962 756e 0d0a 6060  stall taibun..``
-000006e0: 600d 0a0d 0a0d 0a0d 0a3c 212d 2d20 5553  `........<!-- US
-000006f0: 4147 4520 2d2d 3e0d 0a23 2320 5573 6167  AGE -->..## Usag
-00000700: 650d 0a0d 0a23 2323 2043 6f6e 7665 7274  e....### Convert
-00000710: 6572 0d0a 0d0a 6043 6f6e 7665 7274 6572  er....`Converter
-00000720: 6020 636c 6173 7320 7472 616e 736c 6974  ` class translit
-00000730: 6572 6174 6573 2074 6865 2043 6869 6e65  erates the Chine
-00000740: 7365 2063 6861 7261 6374 6572 7320 746f  se characters to
-00000750: 2074 6865 2063 686f 7365 6e20 7472 616e   the chosen tran
-00000760: 736c 6974 6572 6174 696f 6e20 7379 7374  sliteration syst
-00000770: 656d 2077 6974 6820 7061 7261 6d65 7465  em with paramete
-00000780: 7273 2073 7065 6369 6669 6564 2062 7920  rs specified by 
-00000790: 7468 6520 6465 7665 6c6f 7065 722e 2057  the developer. W
-000007a0: 6f72 6b73 2066 6f72 2062 6f74 6820 5472  orks for both Tr
-000007b0: 6164 6974 696f 6e61 6c20 616e 6420 5369  aditional and Si
-000007c0: 6d70 6c69 6669 6564 2063 6861 7261 6374  mplified charact
-000007d0: 6572 732e 0d0a 0d0a 6060 6070 7974 686f  ers.....```pytho
-000007e0: 6e0d 0a23 2063 6f6e 7374 7275 6374 6f72  n..# constructor
-000007f0: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
-00000800: 7379 7374 656d 2c20 6469 616c 6563 742c  system, dialect,
-00000810: 2066 6f72 6d61 742c 2064 656c 696d 6974   format, delimit
-00000820: 6572 2c20 7361 6e64 6869 2c20 7075 6e63  er, sandhi, punc
-00000830: 7475 6174 696f 6e29 0d0a 0d0a 2320 7472  tuation)....# tr
-00000840: 616e 736c 6974 6572 6174 6520 4368 696e  ansliterate Chin
-00000850: 6573 6520 6368 6172 6163 7465 7273 0d0a  ese characters..
-00000860: 632e 6765 7428 696e 7075 7429 0d0a 0d0a  c.get(input)....
-00000870: 2320 636f 6e76 6572 7420 5369 6d70 6c69  # convert Simpli
-00000880: 6669 6564 2043 6869 6e65 7365 2063 6861  fied Chinese cha
-00000890: 7261 6374 6572 7320 746f 2054 7261 6469  racters to Tradi
-000008a0: 7469 6f6e 616c 2043 6869 6e65 7365 2043  tional Chinese C
-000008b0: 6861 7261 6374 6572 730d 0a63 2e74 6f5f  haracters..c.to_
-000008c0: 7472 6164 6974 696f 6e61 6c28 696e 7075  traditional(inpu
-000008d0: 7429 0d0a 6060 600d 0a0d 0a23 2323 2320  t)..```....#### 
-000008e0: 5379 7374 656d 0d0a 0d0a 6073 7973 7465  System....`syste
-000008f0: 6d60 2053 7472 696e 6720 2d20 7379 7374  m` String - syst
-00000900: 656d 206f 6620 7472 616e 736c 6974 6572  em of transliter
-00000910: 6174 696f 6e2e 0d0a 0d0a 2a20 6054 6169  ation.....* `Tai
-00000920: 6c6f 6020 2864 6566 6175 6c74 2920 2d20  lo` (default) - 
-00000930: 5b54 c3a2 692d 75c3 a26e 204c c3b4 2d6d  [T..i-u..n L..-m
-00000940: c3a1 2d6a c4ab 2050 6869 6e67 2d69 6d20  ..-j.. Phing-im 
-00000950: 486f 6e67 2dc3 a06e 5d5b 7461 696c 6f2d  Hong-..n][tailo-
-00000960: 7769 6b69 5d0d 0a2a 2060 504f 4a60 202d  wiki]..* `POJ` -
-00000970: 205b 5065 cc8d 682d c58d 652d 6ac4 ab5d   [Pe..h-..e-j..]
-00000980: 5b70 6f6a 2d77 696b 695d 0d0a 2a20 605a  [poj-wiki]..* `Z
-00000990: 6875 7969 6e60 202d 205b 5461 6977 616e  huyin` - [Taiwan
-000009a0: 6573 6520 5068 6f6e 6574 6963 2053 796d  ese Phonetic Sym
-000009b0: 626f 6c73 5d5b 7a68 7579 696e 2d77 696b  bols][zhuyin-wik
-000009c0: 695d 0d0a 2a20 6054 4c50 4160 202d 205b  i]..* `TLPA` - [
-000009d0: 5461 6977 616e 6573 6520 4c61 6e67 7561  Taiwanese Langua
-000009e0: 6765 2050 686f 6e65 7469 6320 416c 7068  ge Phonetic Alph
-000009f0: 6162 6574 5d5b 746c 7061 2d77 696b 695d  abet][tlpa-wiki]
-00000a00: 0d0a 2a20 6050 696e 6779 696d 6020 2d20  ..* `Pingyim` - 
-00000a10: 5b42 62c3 a16e 6cc3 a16d 2055 c493 2050  [Bb..nl..m U.. P
-00000a20: c3ac 6e67 79c4 ab6d 2048 c58d 6e67 27c3  ..ngy..m H..ng'.
-00000a30: a06e 5d5b 7069 6e67 7969 6d2d 7769 6b69  .n][pingyim-wiki
-00000a40: 5d0d 0a2a 2060 546f 6e67 696f 6e67 6020  ]..* `Tongiong` 
-00000a50: 2d20 5b44 61c4 ab2d 6768 c3ae 2054 c58d  - [Da..-gh.. T..
-00000a60: 6e67 2d69 c58d 6e67 2050 c4ab 6e67 2d69  ng-i..ng P..ng-i
-00000a70: 6d5d 5b74 6f6e 6769 6f6e 672d 7769 6b69  m][tongiong-wiki
-00000a80: 5d0d 0a0d 0a7c 2074 6578 7420 7c20 5461  ]....| text | Ta
-00000a90: 696c 6f20 2020 7c20 504f 4a20 2020 2020  ilo   | POJ     
-00000aa0: 7c20 5a68 7579 696e 2020 2020 2020 7c20  | Zhuyin      | 
-00000ab0: 544c 5041 2020 2020 2020 7c20 5069 6e67  TLPA      | Ping
-00000ac0: 7969 6d20 7c20 546f 6e67 696f 6e67 207c  yim | Tongiong |
-00000ad0: 0d0a 7c2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ..|------|------
-00000ae0: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  ---|---------|--
-00000af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00000b00: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000b10: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d 0a7c  -|----------|..|
-00000b20: 20e8 87ba e781 a320 7c20 54c3 a269 2d75   ...... | T..i-u
-00000b30: c3a2 6e20 7c20 54c3 a269 2d6f c3a2 6e20  ..n | T..i-o..n 
-00000b40: 7c20 e384 89e3 849e cb8a 20e3 84a8 e384  | ........ .....
-00000b50: a2cb 8a20 7c20 5461 6935 2075 616e 3520  ... | Tai5 uan5 
-00000b60: 7c20 44c3 a169 77c3 a16e 2020 7c20 54c4  | D..iw..n  | T.
-00000b70: 8169 2d75 c78e 6e20 207c 0d0a 0d0a 2323  .i-u..n  |....##
-00000b80: 2323 2044 6961 6c65 6374 0d0a 0d0a 6064  ## Dialect....`d
-00000b90: 6961 6c65 6374 6020 5374 7269 6e67 202d  ialect` String -
-00000ba0: 2070 7265 6665 7272 6564 2070 726f 6e75   preferred pronu
-00000bb0: 6e63 6961 7469 6f6e 2e0d 0a0d 0a2a 2060  nciation.....* `
-00000bc0: 736f 7574 6860 2028 6465 6661 756c 7429  south` (default)
-00000bd0: 202d 205b 5a68 616e 677a 686f 755d 5b7a   - [Zhangzhou][z
-00000be0: 6861 6e67 7a68 6f75 2d77 696b 695d 2d6c  hangzhou-wiki]-l
-00000bf0: 6561 6e69 6e67 2070 726f 6e75 6e63 6961  eaning pronuncia
-00000c00: 7469 6f6e 0d0a 2a20 606e 6f72 7468 6020  tion..* `north` 
-00000c10: 2d20 5b51 7561 6e7a 686f 755d 5b71 7561  - [Quanzhou][qua
-00000c20: 6e7a 686f 752d 7769 6b69 5d2d 6c65 616e  nzhou-wiki]-lean
-00000c30: 696e 6720 7072 6f6e 756e 6369 6174 696f  ing pronunciatio
-00000c40: 6e0d 0a0d 0a7c 2074 6578 7420 2020 7c20  n....| text   | 
-00000c50: 736f 7574 6820 2020 2020 2020 2020 7c20  south         | 
-00000c60: 6e6f 7274 6820 2020 2020 2020 2020 7c0d  north         |.
-00000c70: 0a7c 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  .|--------|-----
-00000c80: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-00000c90: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d 0a7c 20e4  ----------|..| .
-00000ca0: ba94 e69c 88e7 af80 207c 2047 c58d 6f2d  ........ | G..o-
-00000cb0: 6775 65cc 8d68 2d74 7365 6820 7c20 47c5  gue..h-tseh | G.
-00000cc0: 8d6f 2d67 65cc 8d68 2d74 7375 6568 207c  .o-ge..h-tsueh |
-00000cd0: 0d0a 0d0a 2323 2323 2046 6f72 6d61 740d  ....#### Format.
-00000ce0: 0a0d 0a60 666f 726d 6174 6020 5374 7269  ...`format` Stri
-00000cf0: 6e67 202d 2066 6f72 6d61 7420 696e 2077  ng - format in w
-00000d00: 6869 6368 2074 6f6e 6573 2077 696c 6c20  hich tones will 
-00000d10: 6265 2072 6570 7265 7365 6e74 6564 2069  be represented i
-00000d20: 6e20 7468 6520 636f 6e76 6572 7465 6420  n the converted 
-00000d30: 7365 6e74 656e 6365 2e0d 0a0d 0a2a 2060  sentence.....* `
-00000d40: 6d61 726b 6020 2864 6566 6175 6c74 2920  mark` (default) 
-00000d50: 2d20 7573 6573 2064 6961 6372 6974 6963  - uses diacritic
-00000d60: 7320 666f 7220 6561 6368 2073 796c 6c61  s for each sylla
-00000d70: 626c 652e 204e 6f74 2061 7661 696c 6162  ble. Not availab
-00000d80: 6c65 2066 6f72 2054 4c50 412e 0d0a 2a20  le for TLPA...* 
-00000d90: 606e 756d 6265 7260 202d 2061 6464 2061  `number` - add a
-00000da0: 206e 756d 6265 7220 7768 6963 6820 7265   number which re
-00000db0: 7072 6573 656e 7473 2074 6865 2074 6f6e  presents the ton
-00000dc0: 6520 6174 2074 6865 2065 6e64 206f 6620  e at the end of 
-00000dd0: 7468 6520 7379 6c6c 6162 6c65 0d0a 2a20  the syllable..* 
-00000de0: 6073 7472 6970 6020 2d20 7265 6d6f 7665  `strip` - remove
-00000df0: 7320 616e 7920 746f 6e65 206d 6172 6b69  s any tone marki
-00000e00: 6e67 0d0a 0d0a 7c20 7465 7874 207c 206d  ng....| text | m
-00000e10: 6172 6b20 2020 207c 206e 756d 6265 7220  ark    | number 
-00000e20: 2020 207c 2073 7472 6970 2020 207c 0d0a     | strip   |..
-00000e30: 7c2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  |------|--------
-00000e40: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -|-----------|--
-00000e50: 2d2d 2d2d 2d2d 2d7c 0d0a 7c20 e887 bae7  -------|..| ....
-00000e60: 81a3 207c 2054 c3a2 692d 75c3 a26e 207c  .. | T..i-u..n |
-00000e70: 2054 6169 352d 7561 6e35 207c 2054 6169   Tai5-uan5 | Tai
-00000e80: 2d75 616e 207c 0d0a 0d0a 2323 2323 2044  -uan |....#### D
-00000e90: 656c 696d 6974 6572 0d0a 0d0a 6064 656c  elimiter....`del
-00000ea0: 696d 6974 6572 6020 5374 7269 6e67 202d  imiter` String -
-00000eb0: 2073 6574 7320 7468 6520 6465 6c69 6d69   sets the delimi
-00000ec0: 7465 7220 6368 6172 6163 7465 7220 7468  ter character th
-00000ed0: 6174 2077 696c 6c20 6265 2070 6c61 6365  at will be place
-00000ee0: 6420 696e 2062 6574 7765 656e 2073 796c  d in between syl
-00000ef0: 6c61 626c 6573 206f 6620 6120 776f 7264  lables of a word
-00000f00: 2e0d 0a0d 0a44 6566 6175 6c74 2076 616c  .....Default val
-00000f10: 7565 2064 6570 656e 6473 206f 6e20 7468  ue depends on th
-00000f20: 6520 6368 6f73 656e 2060 7379 7374 656d  e chosen `system
-00000f30: 603a 0d0a 0d0a 2a20 6027 2d27 6020 2d20  `:....* `'-'` - 
-00000f40: 666f 7220 6054 6169 6c6f 602c 2060 504f  for `Tailo`, `PO
-00000f50: 4a60 2c20 6054 6f6e 6769 6f6e 6760 0d0a  J`, `Tongiong`..
-00000f60: 2a20 6027 2760 202d 2066 6f72 2060 5069  * `''` - for `Pi
-00000f70: 6e67 7969 6d60 0d0a 2a20 6027 2027 6020  ngyim`..* `' '` 
-00000f80: 2d20 666f 7220 605a 6875 7969 6e60 2c20  - for `Zhuyin`, 
-00000f90: 6054 4c50 4160 0d0a 0d0a 7c20 7465 7874  `TLPA`....| text
-00000fa0: 207c 2027 2d27 2020 2020 207c 2027 2720   | '-'     | '' 
-00000fb0: 2020 2020 7c20 2720 2720 2020 2020 7c0d      | ' '     |.
-00000fc0: 0a7c 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  .|------|-------
-00000fd0: 2d2d 7c2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  --|--------|----
-00000fe0: 2d2d 2d2d 2d7c 0d0a 7c20 e887 bae7 81a3  -----|..| ......
-00000ff0: 207c 2054 c3a2 692d 75c3 a26e 207c 2054   | T..i-u..n | T
-00001000: c3a2 6975 c3a2 6e20 7c20 54c3 a269 2075  ..iu..n | T..i u
-00001010: c3a2 6e20 7c0d 0a0d 0a23 2323 2320 5361  ..n |....#### Sa
-00001020: 6e64 6869 0d0a 0d0a 6073 616e 6468 6960  ndhi....`sandhi`
-00001030: 2042 6f6f 6c65 616e 202d 2061 7070 6c69   Boolean - appli
-00001040: 6573 2074 6865 205b 7361 6e64 6869 2072  es the [sandhi r
-00001050: 756c 6573 206f 6620 5461 6977 616e 6573  ules of Taiwanes
-00001060: 6520 486f 6b6b 6965 6e5d 5b73 616e 6468  e Hokkien][sandh
-00001070: 692d 7769 6b69 5d20 746f 2073 796c 6c61  i-wiki] to sylla
-00001080: 626c 6573 206f 6620 6120 7369 6e67 6c65  bles of a single
-00001090: 2077 6f72 642e 0d0a 0d0a 4465 6661 756c   word.....Defaul
-000010a0: 7420 7661 6c75 6520 6465 7065 6e64 7320  t value depends 
-000010b0: 6f6e 2074 6865 2063 686f 7365 6e20 6073  on the chosen `s
-000010c0: 7973 7465 6d60 3a0d 0a0d 0a2a 2060 5472  ystem`:....* `Tr
-000010d0: 7565 6020 2d20 666f 7220 6054 6f6e 6769  ue` - for `Tongi
-000010e0: 6f6e 6760 0d0a 2a20 6046 616c 7365 6020  ong`..* `False` 
-000010f0: 2d20 666f 7220 6054 6169 6c6f 602c 2060  - for `Tailo`, `
-00001100: 504f 4a60 2c20 605a 6875 7969 6e60 2c20  POJ`, `Zhuyin`, 
-00001110: 6054 4c50 4160 2c20 6050 696e 6779 696d  `TLPA`, `Pingyim
-00001120: 600d 0a0d 0a7c 2074 6578 7420 2020 2020  `....| text     
-00001130: 7c20 4661 6c73 6520 2020 2020 2020 207c  | False        |
-00001140: 2054 7275 6520 2020 2020 2020 2020 7c0d   True         |.
-00001150: 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  .|----------|---
-00001160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00001170: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d 0a7c 20e9  ----------|..| .
-00001180: a6ac e4be 86e8 a5bf e4ba 9e20 7c20 4dc3  ........... | M.
-00001190: a12d 6cc3 a269 2d73 652d 6120 207c 204d  .-l..i-se-a  | M
-000011a0: 612d 6cc4 8169 2d73 c493 2d61 2020 7c0d  a-l..i-s..-a  |.
-000011b0: 0a0d 0a53 616e 6468 6920 7275 6c65 7320  ...Sandhi rules 
-000011c0: 616c 736f 2063 6861 6e67 6520 6465 7065  also change depe
-000011d0: 6e64 696e 6720 6f6e 2074 6865 2064 6961  nding on the dia
-000011e0: 6c65 6374 2063 686f 7365 6e2e 0d0a 0d0a  lect chosen.....
-000011f0: 7c20 7465 7874 207c 206e 6f20 7361 6e64  | text | no sand
-00001200: 6869 207c 2073 6f75 7468 2020 207c 206e  hi | south   | n
-00001210: 6f72 7468 2020 207c 0d0a 7c2d 2d2d 2d2d  orth   |..|-----
-00001220: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -|-----------|--
-00001230: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00001240: 2d7c 0d0a 7c20 e887 bae7 81a3 207c 2054  -|..| ...... | T
-00001250: c3a2 692d 75c3 a26e 2020 207c 2054 c481  ..i-u..n   | T..
-00001260: 692d 75c3 a26e 207c 2054 c3a0 692d 75c3  i-u..n | T..i-u.
-00001270: a26e 207c 0d0a 0d0a 4e6f 7465 2074 6861  .n |....Note tha
-00001280: 7420 7468 6520 6675 6e63 7469 6f6e 2069  t the function i
-00001290: 7320 6469 6666 6572 656e 7420 6672 6f6d  s different from
-000012a0: 2072 6561 6c20 7361 6e64 6869 2072 756c   real sandhi rul
-000012b0: 6573 2c20 7768 6572 6520 6368 616e 6765  es, where change
-000012c0: 7320 6172 6520 6170 706c 6965 6420 746f  s are applied to
-000012d0: 2065 7665 7279 2073 696e 676c 6520 7379   every single sy
-000012e0: 6c6c 6162 6c65 206f 6620 7468 6520 7365  llable of the se
-000012f0: 6e74 656e 6365 2c20 6e6f 7420 6a75 7374  ntence, not just
-00001300: 2073 696e 676c 6520 776f 7264 732e 0d0a   single words...
-00001310: 0d0a 2d20 2a2a 5461 6962 756e 2773 2073  ..- **Taibun's s
-00001320: 616e 6468 6920 7275 6c65 732a 2a3a 2054  andhi rules**: T
-00001330: 68c3 a169 2d6b 686f 6e67 2070 c4ab 6e67  h..i-khong p..ng
-00001340: 2d69 c3ba 2c20 6c69 6e2d 68c3 b321 204c  -i.., lin-h..! L
-00001350: c3ad 6e20 7473 69c3 a02d 70c3 a120 6275  ..n tsi..-p.. bu
-00001360: c493 3f0d 0a2d 202a 2a41 6374 7561 6c20  ..?..- **Actual 
-00001370: 7361 6e64 6869 2072 756c 6573 2a2a 3a20  sandhi rules**: 
-00001380: 5468 c3a1 692d 6b68 c58d 6e67 2070 c4ab  Th..i-kh..ng p..
-00001390: 6e67 2d69 c3ba 2c20 6c69 6e2d 68c3 b321  ng-i.., lin-h..!
-000013a0: 204c 696e 2074 7369 c3a0 2d70 6120 6275   Lin tsi..-pa bu
-000013b0: c493 3f0d 0a0d 0a23 2323 2320 5075 6e63  ..?....#### Punc
-000013c0: 7475 6174 696f 6e0d 0a0d 0a60 7075 6e63  tuation....`punc
-000013d0: 7475 6174 696f 6e60 2053 7472 696e 670d  tuation` String.
-000013e0: 0a0d 0a2a 2060 666f 726d 6174 6020 2864  ...* `format` (d
-000013f0: 6566 6175 6c74 2920 2d20 636f 6e76 6572  efault) - conver
-00001400: 7473 2043 6869 6e65 7365 2d73 7479 6c65  ts Chinese-style
-00001410: 2070 756e 6374 7561 7469 6f6e 2074 6f20   punctuation to 
-00001420: 4c61 7469 6e2d 7374 796c 6520 7075 6e63  Latin-style punc
-00001430: 7475 6174 696f 6e20 616e 6420 6361 7069  tuation and capi
-00001440: 7461 6c69 7365 7320 776f 7264 7320 6174  talises words at
-00001450: 2074 6865 2062 6567 696e 6e69 6e67 206f   the beginning o
-00001460: 6620 6561 6368 2073 656e 7465 6e63 652e  f each sentence.
-00001470: 0d0a 2a20 606e 6f6e 6560 202d 2070 7265  ..* `none` - pre
-00001480: 7365 7276 6573 2043 6869 6e65 7365 2d73  serves Chinese-s
-00001490: 7479 6c65 2070 756e 6374 7561 7469 6f6e  tyle punctuation
-000014a0: 2061 6e64 2064 6f65 736e 2774 2063 6170   and doesn't cap
-000014b0: 6974 616c 6973 6520 776f 7264 7320 6174  italise words at
-000014c0: 2074 6865 2062 6567 696e 6e69 6e67 206f   the beginning o
-000014d0: 6620 6e65 7720 7365 6e74 656e 6365 732e  f new sentences.
-000014e0: 0d0a 0d0a 7c20 7465 7874 207c 2066 6f72  ....| text | for
-000014f0: 6d61 7420 7c20 6e6f 6e65 207c 0d0a 7c2d  mat | none |..|-
-00001500: 7c2d 7c2d 7c0d 0a7c 20e9 8099 e698 afe8  |-|-|..| .......
-00001510: 87ba e58d 97ef bc8c e7b0 a1e7 a8b1 e380  ................
-00001520: 8ce5 8d97 e380 8def bc88 e799 bde8 a9b1  ................
-00001530: e5ad 97ef bc9a 54c3 a269 2d6c c3a2 6def  ......T..i-l..m.
-00001540: bc9b e6b3 a8e9 9fb3 e7ac a6e8 999f efbc  ................
-00001550: 9ae3 848a e384 9ecb 8a20 e384 8be3 84a2  ......... ......
-00001560: cb8a efbc 8ce5 9c8b e8aa 9eef bc9a 54c3  ..............T.
-00001570: a169 6ec3 a16e efbc 89e3 8082 207c 2054  .in..n...... | T
-00001580: 7365 2073 c4ab 2054 c3a2 692d 6cc3 a26d  se s.. T..i-l..m
-00001590: 2c20 6bc3 a16e 2d74 7368 696e 6720 226c  , k..n-tshing "l
-000015a0: c3a2 6d22 2028 5065 cc8d 682d 75c4 932d  ..m" (Pe..h-u..-
-000015b0: 6ac4 ab3a 2054 c3a2 692d 6cc3 a26d 3b20  j..: T..i-l..m; 
-000015c0: 7473 c3b9 2d69 6d20 68c3 bb2d 68c5 8d3a  ts..-im h..-h..:
-000015d0: 20e3 848a e384 9ecb 8a20 e384 8be3 84a2   ........ ......
-000015e0: cb8a 2c20 6b6f 6b2d 67c3 ad3a 2054 c3a1  .., kok-g..: T..
-000015f0: 696e c3a1 6e29 2e20 7c20 7473 6520 73c4  in..n). | tse s.
-00001600: ab20 54c3 a269 2d6c c3a2 6def bc8c 6bc3  . T..i-l..m...k.
-00001610: a16e 2d74 7368 696e 67e3 808c 6cc3 a26d  .n-tshing...l..m
-00001620: e380 8def bc88 5065 cc8d 682d 75c4 932d  ......Pe..h-u..-
-00001630: 6ac4 abef bc9a 54c3 a269 2d6c c3a2 6def  j.....T..i-l..m.
-00001640: bc9b 7473 c3b9 2d69 6d20 68c3 bb2d 68c5  ..ts..-im h..-h.
-00001650: 8def bc9a e384 8ae3 849e cb8a 20e3 848b  ............ ...
-00001660: e384 a2cb 8aef bc8c 6b6f 6b2d 67c3 adef  ........kok-g...
-00001670: bc9a 54c3 a169 6ec3 a16e efbc 89e3 8082  ..T..in..n......
-00001680: 207c 0d0a 0d0a 2323 2320 546f 6b65 6e69   |....### Tokeni
-00001690: 7365 720d 0a0d 0a60 546f 6b65 6e69 7365  ser....`Tokenise
-000016a0: 7260 2063 6c61 7373 2070 6572 666f 726d  r` class perform
-000016b0: 7320 5b4e 4c54 4b20 776f 7264 7075 6e63  s [NLTK wordpunc
-000016c0: 745f 746f 6b65 6e69 7a65 5d5b 6e6c 746b  t_tokenize][nltk
-000016d0: 2d74 6f6b 656e 697a 655d 2d6c 696b 6520  -tokenize]-like 
-000016e0: 746f 6b65 6e69 7361 7469 6f6e 206f 6620  tokenisation of 
-000016f0: 6120 5461 6977 616e 6573 6520 486f 6b6b  a Taiwanese Hokk
-00001700: 6965 6e20 7365 6e74 656e 6365 2e0d 0a0d  ien sentence....
-00001710: 0a60 6060 7079 7468 6f6e 0d0a 2320 636f  .```python..# co
-00001720: 6e73 7472 7563 746f 720d 0a74 203d 2054  nstructor..t = T
-00001730: 6f6b 656e 6973 6572 2829 0d0a 0d0a 2320  okeniser()....# 
-00001740: 746f 6b65 6e69 7365 2054 6169 7761 6e65  tokenise Taiwane
-00001750: 7365 2048 6f6b 6b69 656e 2073 656e 7465  se Hokkien sente
-00001760: 6e63 650d 0a74 2e74 6f6b 656e 6973 6528  nce..t.tokenise(
-00001770: 696e 7075 7429 0d0a 6060 600d 0a0d 0a0d  input)..```.....
-00001780: 0a0d 0a3c 212d 2d20 4558 414d 504c 4520  ...<!-- EXAMPLE 
-00001790: 2d2d 3e0d 0a23 2320 4578 616d 706c 650d  -->..## Example.
-000017a0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-000017b0: 6f6d 2074 6169 6275 6e20 696d 706f 7274  om taibun import
-000017c0: 2043 6f6e 7665 7274 6572 2c20 546f 6b65   Converter, Toke
-000017d0: 6e69 7365 720d 0a0d 0a23 2053 7973 7465  niser....# Syste
-000017e0: 6d0d 0a63 203d 2043 6f6e 7665 7274 6572  m..c = Converter
-000017f0: 2829 2023 2054 6169 6c6f 2073 7973 7465  () # Tailo syste
-00001800: 6d20 6465 6661 756c 740d 0a63 2e67 6574  m default..c.get
-00001810: 2827 e585 88e7 949f e8ac 9bef bc8c e5ad  ('..............
-00001820: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
-00001830: 2729 0d0a 3e3e 2053 6961 6e2d 7369 6e6e  ')..>> Sian-sinn
-00001840: 206b c3b3 6e67 2c20 6861 cc8d 6b2d 7369   k..ng, ha..k-si
-00001850: 6e67 2074 69c4 816d 2d74 69c4 816d 2074  ng ti..m-ti..m t
-00001860: 6869 616e 6e2e 0d0a 0d0a 6320 3d20 436f  hiann.....c = Co
-00001870: 6e76 6572 7465 7228 7379 7374 656d 3d27  nverter(system='
-00001880: 5a68 7579 696e 2729 0d0a 632e 6765 7428  Zhuyin')..c.get(
-00001890: 27e5 8588 e794 9fe8 ac9b efbc 8ce5 adb8  '...............
-000018a0: e794 9fe6 81ac e681 ace8 81bd e380 8227  ...............'
-000018b0: 290d 0a3e 3e20 e384 92e3 84a7 e384 a220  )..>> ......... 
-000018c0: e384 92e3 86aa 20e3 848d e386 b2cb 8b2c  ...... ........,
-000018d0: 20e3 848f e384 9ae3 86b6 cb99 20e3 8492   ........... ...
-000018e0: e384 a7e3 84a5 20e3 8489 e384 a7e3 86b0  ...... .........
-000018f0: cbab 20e3 8489 e384 a7e3 86b0 cbab 20e3  .. ........... .
-00001900: 848a e384 a7e3 86a9 2e0d 0a0d 0a23 2044  .............# D
-00001910: 6961 6c65 6374 0d0a 6320 3d20 436f 6e76  ialect..c = Conv
-00001920: 6572 7465 7228 2920 2320 736f 7574 6820  erter() # south 
-00001930: 6469 616c 6563 7420 6465 6661 756c 740d  dialect default.
-00001940: 0a63 2e67 6574 2822 e688 91e6 acb2 e794  .c.get("........
-00001950: a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a 3e3e  ..........")..>>
-00001960: 2047 75c3 a120 6265 6820 c4ab 6e67 2074   Gu.. beh ..ng t
-00001970: c4ab 2074 7369 61cc 8d68 2068 c3ae 0d0a  .. tsia..h h....
-00001980: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
-00001990: 6469 616c 6563 743d 276e 6f72 7468 2729  dialect='north')
-000019a0: 0d0a 632e 6765 7428 22e6 8891 e6ac b2e7  ..c.get(".......
-000019b0: 94a8 e7ae b8e9 a39f e9ad 9a22 290d 0a3e  ...........")..>
-000019c0: 3e20 4775 c3a1 2062 7565 6820 c4ab 6e67  > Gu.. bueh ..ng
-000019d0: 2074 c5ab 2074 7369 61cc 8d68 2068 c3bb   t.. tsia..h h..
-000019e0: 0d0a 0d0a 2320 466f 726d 6174 0d0a 6320  ....# Format..c 
-000019f0: 3d20 436f 6e76 6572 7465 7228 2920 2320  = Converter() # 
-00001a00: 666f 7220 5461 696c 6f2c 206d 6172 6b20  for Tailo, mark 
-00001a10: 6279 2064 6566 6175 6c74 0d0a 632e 6765  by default..c.ge
-00001a20: 7428 22e7 949f e697 a5e5 bfab e6a8 8222  t("............"
-00001a30: 290d 0a3e 3e20 5365 6e6e 2d6a 69cc 8d74  )..>> Senn-ji..t
-00001a40: 206b 6875 c3a0 692d 6c6f cc8d 6b0d 0a0d   khu..i-lo..k...
-00001a50: 0a63 203d 2043 6f6e 7665 7274 6572 2866  .c = Converter(f
-00001a60: 6f72 6d61 743d 276e 756d 6265 7227 290d  ormat='number').
-00001a70: 0a63 2e67 6574 2822 e794 9fe6 97a5 e5bf  .c.get("........
-00001a80: abe6 a882 2229 0d0a 3e3e 2053 656e 6e31  ....")..>> Senn1
-00001a90: 2d6a 6974 3820 6b68 7561 6933 2d6c 6f6b  -jit8 khuai3-lok
-00001aa0: 380d 0a0d 0a63 203d 2043 6f6e 7665 7274  8....c = Convert
-00001ab0: 6572 2866 6f72 6d61 743d 2773 7472 6970  er(format='strip
-00001ac0: 2729 0d0a 632e 6765 7428 22e7 949f e697  ')..c.get(".....
-00001ad0: a5e5 bfab e6a8 8222 290d 0a3e 3e20 5365  .......")..>> Se
-00001ae0: 6e6e 2d6a 6974 206b 6875 6169 2d6c 6f6b  nn-jit khuai-lok
-00001af0: 0d0a 0d0a 2320 4465 6c69 6d69 7465 720d  ....# Delimiter.
-00001b00: 0a63 203d 2043 6f6e 7665 7274 6572 2864  .c = Converter(d
-00001b10: 656c 696d 6974 6572 3d27 2729 0d0a 632e  elimiter='')..c.
-00001b20: 6765 7428 22e5 8588 e794 9fe8 ac9b efbc  get("...........
-00001b30: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
-00001b40: e380 8222 290d 0a3e 3e20 5369 616e 7369  ...")..>> Siansi
-00001b50: 6e6e 206b c3b3 6e67 2c20 6861 cc8d 6b73  nn k..ng, ha..ks
-00001b60: 696e 6720 7469 c481 6d74 69c4 816d 2074  ing ti..mti..m t
-00001b70: 6869 616e 6e2e 0d0a 0d0a 6320 3d20 436f  hiann.....c = Co
-00001b80: 6e76 6572 7465 7228 7379 7374 656d 3d27  nverter(system='
-00001b90: 5069 6e67 7969 6d27 2c20 6465 6c69 6d69  Pingyim', delimi
-00001ba0: 7465 723d 272d 2729 0d0a 632e 6765 7428  ter='-')..c.get(
-00001bb0: 22e5 8588 e794 9fe8 ac9b efbc 8ce5 adb8  "...............
-00001bc0: e794 9fe6 81ac e681 ace8 81bd e380 8222  ..............."
-00001bd0: 290d 0a3e 3e20 5369 c481 6e2d 736e c4ab  )..>> Si..n-sn..
-00001be0: 2067 c792 6e67 2c20 68c3 a167 2d73 c4ab   g..ng, h..g-s..
-00001bf0: 6e67 2064 69c3 a26d 2d64 69c3 a26d 2074  ng di..m-di..m t
-00001c00: 696e c481 2e0d 0a0d 0a23 2053 616e 6468  in.......# Sandh
-00001c10: 690d 0a63 203d 2043 6f6e 7665 7274 6572  i..c = Converter
-00001c20: 2829 2023 2066 6f72 2054 6169 6c6f 2c20  () # for Tailo, 
-00001c30: 7361 6e64 6869 2046 616c 7365 2062 7920  sandhi False by 
-00001c40: 6465 6661 756c 740d 0a63 2e67 6574 2822  default..c.get("
-00001c50: e58d 97e8 bfb4 e990 b5e8 b7af 2229 0d0a  ............")..
-00001c60: 3e3e 204c c3a2 6d2d 6875 c3aa 2d74 6869  >> L..m-hu..-thi
-00001c70: 682d 6cc5 8d6f 0d0a 0d0a 6320 3d20 436f  h-l..o....c = Co
-00001c80: 6e76 6572 7465 7228 7361 6e64 6869 3d54  nverter(sandhi=T
-00001c90: 7275 6529 0d0a 632e 6765 7428 22e5 8d97  rue)..c.get("...
-00001ca0: e8bf b4e9 90b5 e8b7 af22 290d 0a3e 3e20  .........")..>> 
-00001cb0: 4cc4 816d 2d68 75c4 932d 7468 c3ad 2d6c  L..m-hu..-th..-l
-00001cc0: c58d 6f0d 0a0d 0a23 2050 756e 6374 7561  ..o....# Punctua
-00001cd0: 7469 6f6e 0d0a 6320 3d20 436f 6e76 6572  tion..c = Conver
-00001ce0: 7465 7228 2920 2320 666f 726d 6174 2070  ter() # format p
-00001cf0: 756e 6374 7561 7469 6f6e 2064 6566 6175  unctuation defau
-00001d00: 6c74 0d0a 632e 6765 7428 22e5 a4aa e7a9  lt..c.get(".....
-00001d10: bae6 9c8b e58f 8bef bc8c e681 81e5 a5bd  ................
-00001d20: efbc 81e6 8181 e9a3 9fe9 a3bd e69c aaef  ................
-00001d30: bc9f 2229 0d0a 3e3e 2054 68c3 a069 2d6b  ..")..>> Th..i-k
-00001d40: 686f 6e67 2070 c3ae 6e67 2d69 c3ba 2c20  hong p..ng-i.., 
-00001d50: 6cc3 ad6e 2d68 c3b3 2120 4cc3 ad6e 2074  l..n-h..! L..n t
-00001d60: 7369 61cc 8d68 2d70 c3a1 2062 75c4 933f  sia..h-p.. bu..?
-00001d70: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00001d80: 7228 7075 6e63 7475 6174 696f 6e3d 276e  r(punctuation='n
-00001d90: 6f6e 6527 290d 0a63 2e67 6574 2822 e5a4  one')..c.get("..
-00001da0: aae7 a9ba e69c 8be5 8f8b efbc 8ce6 8181  ................
-00001db0: e5a5 bdef bc81 e681 81e9 a39f e9a3 bde6  ................
-00001dc0: 9caa efbc 9f22 290d 0a3e 3e20 7468 c3a0  .....")..>> th..
-00001dd0: 692d 6b68 6f6e 6720 70c3 ae6e 672d 69c3  i-khong p..ng-i.
-00001de0: baef bc8c 6cc3 ad6e 2d68 c3b3 efbc 816c  ....l..n-h.....l
-00001df0: c3ad 6e20 7473 6961 cc8d 682d 70c3 a120  ..n tsia..h-p.. 
-00001e00: 6275 c493 efbc 9f0d 0a0d 0a0d 0a23 2054  bu...........# T
-00001e10: 6f6b 656e 6973 6572 0d0a 7420 3d20 546f  okeniser..t = To
-00001e20: 6b65 6e69 7365 7228 290d 0a74 2e74 6f6b  keniser()..t.tok
-00001e30: 656e 6973 6528 22e5 a4aa e7a9 bae6 9c8b  enise(".........
-00001e40: e58f 8bef bc8c e681 81e5 a5bd efbc 81e6  ................
-00001e50: 8181 e9a3 9fe9 a3bd e69c aaef bc9f 2229  ..............")
-00001e60: 0d0a 3e3e 205b 27e5 a4aa e7a9 ba27 2c20  ..>> ['......', 
-00001e70: 27e6 9c8b e58f 8b27 2c20 27ef bc8c 272c  '......', '...',
-00001e80: 2027 e681 81e5 a5bd 272c 2027 efbc 8127   '......', '...'
-00001e90: 2c20 27e6 8181 272c 2027 e9a3 9fe9 a3bd  , '...', '......
-00001ea0: 272c 2027 e69c aa27 2c20 27ef bc9f 275d  ', '...', '...']
-00001eb0: 0d0a 6060 600d 0a0d 0a0d 0a0d 0a3c 212d  ..```........<!-
-00001ec0: 2d20 4441 5441 202d 2d3e 0d0a 2323 2044  - DATA -->..## D
-00001ed0: 6174 610d 0a0d 0a2d 205b 5461 6977 616e  ata....- [Taiwan
-00001ee0: 6573 652d 4368 696e 6573 6520 4f6e 6c69  ese-Chinese Onli
-00001ef0: 6e65 2044 6963 7469 6f6e 6172 795d 5b6f  ne Dictionary][o
-00001f00: 6e6c 696e 652d 6469 6374 696f 6e61 7279  nline-dictionary
-00001f10: 5d20 2876 6961 205b 4368 686f 6554 6169  ] (via [ChhoeTai
-00001f20: 6769 5d5b 6461 7461 2d76 6961 5d29 0d0a  gi][data-via])..
-00001f30: 2d20 5b69 5461 6967 6920 4368 696e 6573  - [iTaigi Chines
-00001f40: 652d 5461 6977 616e 6573 6520 436f 6d70  e-Taiwanese Comp
-00001f50: 6172 6973 6f6e 2044 6963 7469 6f6e 6172  arison Dictionar
-00001f60: 795d 5b69 7461 6967 692d 6469 6374 696f  y][itaigi-dictio
-00001f70: 6e61 7279 5d20 2876 6961 205b 4368 686f  nary] (via [Chho
-00001f80: 6554 6169 6769 5d5b 6461 7461 2d76 6961  eTaigi][data-via
-00001f90: 5d29 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2041  ])........<!-- A
-00001fa0: 434b 4e4f 574c 4544 4745 4d45 4e54 5320  CKNOWLEDGEMENTS 
-00001fb0: 2d2d 3e0d 0a23 2320 4163 6b6e 6f77 6c65  -->..## Acknowle
-00001fc0: 6467 656d 656e 7473 0d0a 0d0a 2d20 5361  dgements....- Sa
-00001fd0: 6d75 656c 204a 656e 2028 5b47 6974 6875  muel Jen ([Githu
-00001fe0: 625d 5b73 616d 7565 6c2d 6769 7468 7562  b][samuel-github
-00001ff0: 5d20 c2b7 205b 4c69 6e6b 6564 496e 5d5b  ] .. [LinkedIn][
-00002000: 7361 6d75 656c 2d6c 696e 6b65 6469 6e5d  samuel-linkedin]
-00002010: 2920 2d20 5461 6977 616e 6573 6520 616e  ) - Taiwanese an
-00002020: 6420 4d61 6e64 6172 696e 2074 7261 6e73  d Mandarin trans
-00002030: 6c61 7469 6f6e 0d0a 0d0a 0d0a 0d0a 3c21  lation........<!
-00002040: 2d2d 204c 4943 454e 4345 202d 2d3e 0d0a  -- LICENCE -->..
-00002050: 2323 204c 6963 656e 6365 0d0a 0d0a 4265  ## Licence....Be
-00002060: 6361 7573 6520 5461 6962 756e 2069 7320  cause Taibun is 
-00002070: 4d49 542d 6c69 6365 6e73 6564 2c20 616e  MIT-licensed, an
-00002080: 7920 6465 7665 6c6f 7065 7220 6361 6e20  y developer can 
-00002090: 6573 7365 6e74 6961 6c6c 7920 646f 2077  essentially do w
-000020a0: 6861 7465 7665 7220 7468 6579 2077 616e  hatever they wan
-000020b0: 7420 7769 7468 2069 7420 6173 206c 6f6e  t with it as lon
-000020c0: 6720 6173 2074 6865 7920 696e 636c 7564  g as they includ
-000020d0: 6520 7468 6520 6f72 6967 696e 616c 2063  e the original c
-000020e0: 6f70 7972 6967 6874 2061 6e64 206c 6963  opyright and lic
-000020f0: 656e 6365 206e 6f74 6963 6520 696e 2061  ence notice in a
-00002100: 6e79 2063 6f70 6965 7320 6f66 2074 6865  ny copies of the
-00002110: 2073 6f75 7263 6520 636f 6465 2e20 4e6f   source code. No
-00002120: 7465 2c20 7468 6174 2074 6865 2064 6174  te, that the dat
-00002130: 6120 7573 6564 2062 7920 7468 6520 7061  a used by the pa
-00002140: 636b 6167 6520 6973 206c 6963 656e 7365  ckage is license
-00002150: 6420 756e 6465 7220 6120 6469 6666 6572  d under a differ
-00002160: 656e 7420 636f 7079 7269 6768 742e 0d0a  ent copyright...
-00002170: 0d0a 5468 6520 6461 7461 2069 7320 6c69  ..The data is li
-00002180: 6365 6e73 6564 2075 6e64 6572 205b 4343  censed under [CC
-00002190: 2042 592d 5341 2034 2e30 5d5b 6461 7461   BY-SA 4.0][data
-000021a0: 2d63 635d 0d0a 0d0a 0d0a 0d0a 3c21 2d2d  -cc]........<!--
-000021b0: 204d 4152 4b44 4f57 4e20 4c49 4e4b 5320   MARKDOWN LINKS 
-000021c0: 2d2d 3e0d 0a5b 7465 7374 735d 3a20 6874  -->..[tests]: ht
-000021d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000021e0: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
-000021f0: 6e2f 6163 7469 6f6e 730d 0a5b 7465 7374  n/actions..[test
-00002200: 732d 6261 6467 655d 3a20 6874 7470 733a  s-badge]: https:
-00002210: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00002220: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
-00002230: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
-00002240: 616e 6472 6569 6861 722f 7461 6962 756e  andreihar/taibun
-00002250: 2f63 692e 7961 6d6c 3f73 7479 6c65 3d66  /ci.yaml?style=f
-00002260: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b63  or-the-badge..[c
-00002270: 6f6e 7472 6962 7574 6f72 732d 6261 6467  ontributors-badg
-00002280: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
-00002290: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-000022a0: 622f 636f 6e74 7269 6275 746f 7273 2f61  b/contributors/a
-000022b0: 6e64 7265 6968 6172 2f74 6169 6275 6e3f  ndreihar/taibun?
-000022c0: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-000022d0: 6467 650d 0a5b 636f 6e74 7269 6275 746f  dge..[contributo
-000022e0: 7273 5d3a 2023 7573 6167 650d 0a5b 7265  rs]: #usage..[re
-000022f0: 6c65 6173 652d 6261 6467 655d 3a20 6874  lease-badge]: ht
-00002300: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00002310: 732e 696f 2f67 6974 6875 622f 762f 7265  s.io/github/v/re
-00002320: 6c65 6173 652f 616e 6472 6569 6861 722f  lease/andreihar/
-00002330: 7461 6962 756e 3f63 6f6c 6f72 3d33 3836  taibun?color=386
-00002340: 3138 6326 7374 796c 653d 666f 722d 7468  18c&style=for-th
-00002350: 652d 6261 6467 650d 0a5b 7265 6c65 6173  e-badge..[releas
-00002360: 655d 3a20 6874 7470 733a 2f2f 6769 7468  e]: https://gith
-00002370: 7562 2e63 6f6d 2f61 6e64 7265 6968 6172  ub.com/andreihar
-00002380: 2f74 6169 6275 6e2f 7265 6c65 6173 6573  /taibun/releases
-00002390: 0d0a 5b6c 6963 656e 6365 2d62 6164 6765  ..[licence-badge
-000023a0: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-000023b0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-000023c0: 2f6c 6963 656e 7365 2f61 6e64 7265 6968  /license/andreih
-000023d0: 6172 2f74 6169 6275 6e3f 636f 6c6f 723d  ar/taibun?color=
-000023e0: 3030 3030 3030 2673 7479 6c65 3d66 6f72  000000&style=for
-000023f0: 2d74 6865 2d62 6164 6765 0d0a 5b6c 6963  -the-badge..[lic
-00002400: 656e 6365 5d3a 204c 4943 454e 5345 0d0a  ence]: LICENSE..
-00002410: 5b6c 696e 6b65 6469 6e2d 6261 6467 655d  [linkedin-badge]
-00002420: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00002430: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
-00002440: 696e 6b65 6449 6e2d 3030 3737 4235 3f73  inkedIn-0077B5?s
-00002450: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
-00002460: 6765 266c 6f67 6f3d 6c69 6e6b 6564 696e  ge&logo=linkedin
-00002470: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
-00002480: 0d0a 5b6c 696e 6b65 6469 6e5d 3a20 6874  ..[linkedin]: ht
-00002490: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
-000024a0: 696e 2e63 6f6d 2f69 6e2f 616e 6472 6569  in.com/in/andrei
-000024b0: 2d68 6172 6261 6368 6f76 2f0d 0a0d 0a5b  -harbachov/....[
-000024c0: 7079 7069 5d3a 2068 7474 7073 3a2f 2f70  pypi]: https://p
-000024d0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-000024e0: 7461 6962 756e 0d0a 5b62 7567 5d3a 2068  taibun..[bug]: h
-000024f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002500: 6d2f 616e 6472 6569 6861 722f 7461 6962  m/andreihar/taib
-00002510: 756e 2f69 7373 7565 730d 0a5b 6f6e 6c69  un/issues..[onli
-00002520: 6e65 2d64 6963 7469 6f6e 6172 795d 3a20  ne-dictionary]: 
-00002530: 6874 7470 3a2f 2f69 7031 3934 3039 372e  http://ip194097.
-00002540: 6e74 6375 2e65 6475 2e74 772f 756e 6769  ntcu.edu.tw/ungi
-00002550: 616e 2f73 6f61 6e6e 7465 6e67 2f63 6869  an/soannteng/chi
-00002560: 6c2f 5461 6968 6f61 2e61 7370 0d0a 5b69  l/Taihoa.asp..[i
-00002570: 7461 6967 692d 6469 6374 696f 6e61 7279  taigi-dictionary
-00002580: 5d3a 2068 7474 7073 3a2f 2f69 7461 6967  ]: https://itaig
-00002590: 692e 7477 2f0d 0a5b 6461 7461 2d76 6961  i.tw/..[data-via
-000025a0: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-000025b0: 622e 636f 6d2f 4368 686f 6554 6169 6769  b.com/ChhoeTaigi
-000025c0: 2f43 6868 6f65 5461 6967 6944 6174 6162  /ChhoeTaigiDatab
-000025d0: 6173 650d 0a5b 6461 7461 2d63 635d 3a20  ase..[data-cc]: 
-000025e0: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
-000025f0: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
-00002600: 6e73 6573 2f62 792d 7361 2f34 2e30 2f64  nses/by-sa/4.0/d
-00002610: 6565 642e 656e 0d0a 5b73 616d 7565 6c2d  eed.en..[samuel-
-00002620: 6769 7468 7562 5d3a 2068 7474 7073 3a2f  github]: https:/
-00002630: 2f67 6974 6875 622e 636f 6d2f 5353 5361  /github.com/SSSa
-00002640: 6d0d 0a5b 7361 6d75 656c 2d6c 696e 6b65  m..[samuel-linke
-00002650: 6469 6e5d 3a20 6874 7470 733a 2f2f 7777  din]: https://ww
-00002660: 772e 6c69 6e6b 6564 696e 2e63 6f6d 2f69  w.linkedin.com/i
-00002670: 6e2f 7361 6d75 656c 2d6a 656e 2f0d 0a0d  n/samuel-jen/...
-00002680: 0a5b 7461 696c 6f2d 7769 6b69 5d3a 2068  .[tailo-wiki]: h
-00002690: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-000026a0: 6469 612e 6f72 672f 7769 6b69 2f54 2543  dia.org/wiki/T%C
-000026b0: 3325 4132 692d 7525 4333 2541 326e 5f4c  3%A2i-u%C3%A2n_L
-000026c0: 2543 3325 4234 2d6d 2543 3325 4131 2d6a  %C3%B4-m%C3%A1-j
-000026d0: 2543 3425 4142 5f50 6869 6e67 2d69 6d5f  %C4%AB_Phing-im_
-000026e0: 486f 6e67 2d25 4333 2541 306e 0d0a 5b70  Hong-%C3%A0n..[p
-000026f0: 6f6a 2d77 696b 695d 3a20 6874 7470 733a  oj-wiki]: https:
-00002700: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002710: 7267 2f77 696b 692f 5065 2543 4325 3844  rg/wiki/Pe%CC%8D
-00002720: 682d 2543 3525 3844 652d 6a25 4334 2541  h-%C5%8De-j%C4%A
-00002730: 420d 0a5b 7a68 7579 696e 2d77 696b 695d  B..[zhuyin-wiki]
-00002740: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
-00002750: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00002760: 5461 6977 616e 6573 655f 5068 6f6e 6574  Taiwanese_Phonet
-00002770: 6963 5f53 796d 626f 6c73 0d0a 5b74 6c70  ic_Symbols..[tlp
-00002780: 612d 7769 6b69 5d3a 2068 7474 7073 3a2f  a-wiki]: https:/
-00002790: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-000027a0: 672f 7769 6b69 2f54 6169 7761 6e65 7365  g/wiki/Taiwanese
-000027b0: 5f4c 616e 6775 6167 655f 5068 6f6e 6574  _Language_Phonet
-000027c0: 6963 5f41 6c70 6861 6265 740d 0a5b 7069  ic_Alphabet..[pi
-000027d0: 6e67 7969 6d2d 7769 6b69 5d3a 2068 7474  ngyim-wiki]: htt
-000027e0: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-000027f0: 612e 6f72 672f 7769 6b69 2f42 6225 4333  a.org/wiki/Bb%C3
-00002800: 2541 316e 6c25 4333 2541 316d 5f70 2543  %A1nl%C3%A1m_p%C
-00002810: 3325 4143 6e67 7925 4334 2541 426d 0d0a  3%ACngy%C4%ABm..
-00002820: 5b74 6f6e 6769 6f6e 672d 7769 6b69 5d3a  [tongiong-wiki]:
-00002830: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
-00002840: 7065 6469 612e 6f72 672f 7769 6b69 2f44  pedia.org/wiki/D
-00002850: 6125 4334 2541 422d 6768 2543 3325 4145  a%C4%AB-gh%C3%AE
-00002860: 5f74 2543 3525 3844 6e67 2d69 2543 3525  _t%C5%8Dng-i%C5%
-00002870: 3844 6e67 5f70 2543 3425 4142 6e67 2d69  8Dng_p%C4%ABng-i
-00002880: 6d0d 0a5b 7a68 616e 677a 686f 752d 7769  m..[zhangzhou-wi
-00002890: 6b69 5d3a 2068 7474 7073 3a2f 2f65 6e2e  ki]: https://en.
-000028a0: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-000028b0: 6b69 2f5a 6861 6e67 7a68 6f75 5f64 6961  ki/Zhangzhou_dia
-000028c0: 6c65 6374 730d 0a5b 7175 616e 7a68 6f75  lects..[quanzhou
-000028d0: 2d77 696b 695d 3a20 6874 7470 733a 2f2f  -wiki]: https://
-000028e0: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
-000028f0: 2f77 696b 692f 5175 616e 7a68 6f75 5f64  /wiki/Quanzhou_d
-00002900: 6961 6c65 6374 730d 0a5b 6e6c 746b 2d74  ialects..[nltk-t
-00002910: 6f6b 656e 697a 655d 3a20 6874 7470 733a  okenize]: https:
-00002920: 2f2f 6e6c 746b 2e6f 7267 2f61 7069 2f6e  //nltk.org/api/n
-00002930: 6c74 6b2e 746f 6b65 6e69 7a65 2e68 746d  ltk.tokenize.htm
-00002940: 6c0d 0a5b 7361 6e64 6869 2d77 696b 695d  l..[sandhi-wiki]
-00002950: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
-00002960: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00002970: 5461 6977 616e 6573 655f 486f 6b6b 6965  Taiwanese_Hokkie
-00002980: 6e23 546f 6e65 2532 3073 616e 6468 693a  n#Tone%20sandhi:
-00002990: 7e3a 7465 7874 3d74 686e 6725 4532 2539  ~:text=thng%E2%9
-000029a0: 4625 4139 2532 3028 2532 3273 6f75 7025  F%A9%20(%22soup%
-000029b0: 3232 292e 2d2c 546f 6e65 2532 3073 616e  22).-,Tone%20san
-000029c0: 6468 692c 2d25 3542 6564 6974 2535 44    dhi,-%5Bedit%5D
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 2074 6169  : 2.1..Name: tai
+00000020: 6275 6e0d 0a56 6572 7369 6f6e 3a20 312e  bun..Version: 1.
+00000030: 312e 300d 0a53 756d 6d61 7279 3a20 5461  1.0..Summary: Ta
+00000040: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
+00000050: 5472 616e 736c 6974 6572 6174 6f72 2061  Transliterator a
+00000060: 6e64 2054 6f6b 656e 6973 6572 0d0a 486f  nd Tokeniser..Ho
+00000070: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000080: 2f67 6974 6875 622e 636f 6d2f 616e 6472  /github.com/andr
+00000090: 6569 6861 722f 7461 6962 756e 0d0a 4175  eihar/taibun..Au
+000000a0: 7468 6f72 3a20 416e 6472 6569 2048 6172  thor: Andrei Har
+000000b0: 6261 6368 6f76 0d0a 4175 7468 6f72 2d65  bachov..Author-e
+000000c0: 6d61 696c 3a20 616e 6472 6569 2e68 6172  mail: andrei.har
+000000d0: 6261 6368 6f76 4067 6d61 696c 2e63 6f6d  bachov@gmail.com
+000000e0: 0d0a 4c69 6365 6e73 653a 204d 4954 0d0a  ..License: MIT..
+000000f0: 4b65 7977 6f72 6473 3a20 7079 7468 6f6e  Keywords: python
+00000100: 2c74 6169 7761 6e2c 7461 6977 616e 6573  ,taiwan,taiwanes
+00000110: 652c 7461 6967 692c 686f 6b6b 6965 6e2c  e,taigi,hokkien,
+00000120: 726f 6d61 6e69 7a61 7469 6f6e 2c74 7261  romanization,tra
+00000130: 6e73 6c69 7465 7261 7469 6f6e 2c74 7261  nsliteration,tra
+00000140: 6e73 6c69 7465 7261 746f 722c 746f 6b65  nsliterator,toke
+00000150: 6e69 7a61 7469 6f6e 2c74 6f6b 656e 697a  nization,tokeniz
+00000160: 6572 0d0a 436c 6173 7369 6669 6572 3a20  er..Classifier: 
+00000170: 546f 7069 6320 3a3a 2054 6578 7420 5072  Topic :: Text Pr
+00000180: 6f63 6573 7369 6e67 203a 3a20 4c69 6e67  ocessing :: Ling
+00000190: 7569 7374 6963 0d0a 436c 6173 7369 6669  uistic..Classifi
+000001a0: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
+000001b0: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
+000001c0: 6f64 7563 7469 6f6e 2f53 7461 626c 650d  oduction/Stable.
+000001d0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
+000001e0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+000001f0: 3a20 4465 7665 6c6f 7065 7273 0d0a 436c  : Developers..Cl
+00000200: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000220: 3a20 5079 7468 6f6e 203a 3a20 330d 0a43  : Python :: 3..C
+00000230: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
+00000240: 7469 6e67 2053 7973 7465 6d20 3a3a 2055  ting System :: U
+00000250: 6e69 780d 0a43 6c61 7373 6966 6965 723a  nix..Classifier:
+00000260: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
+00000270: 6d20 3a3a 204d 6163 4f53 203a 3a20 4d61  m :: MacOS :: Ma
+00000280: 634f 5320 580d 0a43 6c61 7373 6966 6965  cOS X..Classifie
+00000290: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000002a0: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+000002b0: 203a 3a20 5769 6e64 6f77 730d 0a52 6571   :: Windows..Req
+000002c0: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+000002d0: 332e 380d 0a44 6573 6372 6970 7469 6f6e  3.8..Description
+000002e0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000002f0: 6578 742f 6d61 726b 646f 776e 0d0a 4c69  ext/markdown..Li
+00000300: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+00000310: 4e53 450d 0a0d 0a3c 212d 2d20 5052 4f4a  NSE....<!-- PROJ
+00000320: 4543 5420 4c4f 474f 202d 2d3e 0d0a 3c62  ECT LOGO -->..<b
+00000330: 7220 2f3e 0d0a 3c64 6976 2061 6c69 676e  r />..<div align
+00000340: 3d22 6365 6e74 6572 223e 0d0a 2020 0d0a  ="center">..  ..
+00000350: 2320 5461 6962 756e 0d0a 0d0a 0d0a 0d0a  # Taibun........
+00000360: 3c21 2d2d 2050 524f 4a45 4354 2053 4849  <!-- PROJECT SHI
+00000370: 454c 4453 202d 2d3e 0d0a 5b21 5b54 6573  ELDS -->..[![Tes
+00000380: 7473 5d5b 7465 7374 732d 6261 6467 655d  ts][tests-badge]
+00000390: 5d5b 7465 7374 735d 0d0a 5b21 5b43 6f6e  ][tests]..[![Con
+000003a0: 7472 6962 7574 6f72 735d 5b63 6f6e 7472  tributors][contr
+000003b0: 6962 7574 6f72 732d 6261 6467 655d 5d5b  ibutors-badge]][
+000003c0: 636f 6e74 7269 6275 746f 7273 5d0d 0a5b  contributors]..[
+000003d0: 215b 5265 6c65 6173 655d 5b72 656c 6561  ![Release][relea
+000003e0: 7365 2d62 6164 6765 5d5d 5b72 656c 6561  se-badge]][relea
+000003f0: 7365 5d0d 0a5b 215b 4c69 6365 6e63 655d  se]..[![Licence]
+00000400: 5b6c 6963 656e 6365 2d62 6164 6765 5d5d  [licence-badge]]
+00000410: 5b6c 6963 656e 6365 5d0d 0a5b 215b 4c69  [licence]..[![Li
+00000420: 6e6b 6564 496e 5d5b 6c69 6e6b 6564 696e  nkedIn][linkedin
+00000430: 2d62 6164 6765 5d5d 5b6c 696e 6b65 6469  -badge]][linkedi
+00000440: 6e5d 0d0a 0d0a 2a2a 5461 6977 616e 6573  n]....**Taiwanes
+00000450: 6520 486f 6b6b 6965 6e20 5472 616e 736c  e Hokkien Transl
+00000460: 6974 6572 6174 6f72 2061 6e64 2054 6f6b  iterator and Tok
+00000470: 656e 6973 6572 2a2a 0d0a 0d0a 4974 2068  eniser**....It h
+00000480: 6173 206d 6574 686f 6473 2074 6861 7420  as methods that 
+00000490: 616c 6c6f 7720 746f 2063 7573 746f 6d69  allow to customi
+000004a0: 7365 2074 7261 6e73 6c69 7465 7261 7469  se transliterati
+000004b0: 6f6e 2061 6e64 2072 6574 7269 6576 6520  on and retrieve 
+000004c0: 616e 7920 6e65 6365 7373 6172 7920 696e  any necessary in
+000004d0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+000004e0: 5461 6977 616e 6573 6520 486f 6b6b 6965  Taiwanese Hokkie
+000004f0: 6e20 7072 6f6e 756e 6369 6174 696f 6e2e  n pronunciation.
+00000500: 3c62 7220 2f3e 0d0a 496e 636c 7564 6573  <br />..Includes
+00000510: 2077 6f72 6420 746f 6b65 6e69 7365 7220   word tokeniser 
+00000520: 666f 7220 5461 6977 616e 6573 6520 486f  for Taiwanese Ho
+00000530: 6b6b 6965 6e2e 0d0a 0d0a 5b52 6570 6f72  kkien.....[Repor
+00000540: 7420 4275 675d 5b62 7567 5d20 e280 a20d  t Bug][bug] ....
+00000550: 0a5b 5079 5049 5d5b 7079 7069 5d0d 0a0d  .[PyPI][pypi]...
+00000560: 0a3c 2f64 6976 3e0d 0a0d 0a0d 0a0d 0a2d  .</div>........-
+00000570: 2d2d 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2049  --........<!-- I
+00000580: 4e53 5441 4c4c 202d 2d3e 0d0a 2323 2049  NSTALL -->..## I
+00000590: 6e73 7461 6c6c 0d0a 0d0a 5461 6962 756e  nstall....Taibun
+000005a0: 2063 616e 2062 6520 696e 7374 616c 6c65   can be installe
+000005b0: 6420 6672 6f6d 205b 7079 7069 5d5b 7079  d from [pypi][py
+000005c0: 7069 5d0d 0a0d 0a60 6060 6261 7368 0d0a  pi]....```bash..
+000005d0: 2420 7069 7020 696e 7374 616c 6c20 7461  $ pip install ta
+000005e0: 6962 756e 0d0a 6060 600d 0a0d 0a0d 0a0d  ibun..```.......
+000005f0: 0a3c 212d 2d20 5553 4147 4520 2d2d 3e0d  .<!-- USAGE -->.
+00000600: 0a23 2320 5573 6167 650d 0a0d 0a23 2323  .## Usage....###
+00000610: 2043 6f6e 7665 7274 6572 0d0a 0d0a 6043   Converter....`C
+00000620: 6f6e 7665 7274 6572 6020 636c 6173 7320  onverter` class 
+00000630: 7472 616e 736c 6974 6572 6174 6573 2074  transliterates t
+00000640: 6865 2043 6869 6e65 7365 2063 6861 7261  he Chinese chara
+00000650: 6374 6572 7320 746f 2074 6865 2063 686f  cters to the cho
+00000660: 7365 6e20 7472 616e 736c 6974 6572 6174  sen transliterat
+00000670: 696f 6e20 7379 7374 656d 2077 6974 6820  ion system with 
+00000680: 7061 7261 6d65 7465 7273 2073 7065 6369  parameters speci
+00000690: 6669 6564 2062 7920 7468 6520 6465 7665  fied by the deve
+000006a0: 6c6f 7065 722e 2057 6f72 6b73 2066 6f72  loper. Works for
+000006b0: 2062 6f74 6820 5472 6164 6974 696f 6e61   both Traditiona
+000006c0: 6c20 616e 6420 5369 6d70 6c69 6669 6564  l and Simplified
+000006d0: 2063 6861 7261 6374 6572 732e 0d0a 0d0a   characters.....
+000006e0: 6060 6070 7974 686f 6e0d 0a23 2063 6f6e  ```python..# con
+000006f0: 7374 7275 6374 6f72 0d0a 6320 3d20 436f  structor..c = Co
+00000700: 6e76 6572 7465 7228 7379 7374 656d 2c20  nverter(system, 
+00000710: 6469 616c 6563 742c 2066 6f72 6d61 742c  dialect, format,
+00000720: 2064 656c 696d 6974 6572 2c20 7361 6e64   delimiter, sand
+00000730: 6869 2c20 7075 6e63 7475 6174 696f 6e2c  hi, punctuation,
+00000740: 2063 6f6e 7665 7274 5f6e 6f6e 5f63 6a6b   convert_non_cjk
+00000750: 290d 0a0d 0a23 2074 7261 6e73 6c69 7465  )....# translite
+00000760: 7261 7465 2043 6869 6e65 7365 2063 6861  rate Chinese cha
+00000770: 7261 6374 6572 730d 0a63 2e67 6574 2869  racters..c.get(i
+00000780: 6e70 7574 290d 0a60 6060 0d0a 0d0a 2323  nput)..```....##
+00000790: 2323 2053 7973 7465 6d0d 0a0d 0a60 7379  ## System....`sy
+000007a0: 7374 656d 6020 5374 7269 6e67 202d 2073  stem` String - s
+000007b0: 7973 7465 6d20 6f66 2074 7261 6e73 6c69  ystem of transli
+000007c0: 7465 7261 7469 6f6e 2e0d 0a0d 0a2a 2060  teration.....* `
+000007d0: 5461 696c 6f60 2028 6465 6661 756c 7429  Tailo` (default)
+000007e0: 202d 205b 54c3 a269 2d75 c3a2 6e20 4cc3   - [T..i-u..n L.
+000007f0: b42d 6dc3 a12d 6ac4 ab20 5068 696e 672d  .-m..-j.. Phing-
+00000800: 696d 2048 6f6e 672d c3a0 6e5d 5b74 6169  im Hong-..n][tai
+00000810: 6c6f 2d77 696b 695d 0d0a 2a20 6050 4f4a  lo-wiki]..* `POJ
+00000820: 6020 2d20 5b50 65cc 8d68 2dc5 8d65 2d6a  ` - [Pe..h-..e-j
+00000830: c4ab 5d5b 706f 6a2d 7769 6b69 5d0d 0a2a  ..][poj-wiki]..*
+00000840: 2060 5a68 7579 696e 6020 2d20 5b54 6169   `Zhuyin` - [Tai
+00000850: 7761 6e65 7365 2050 686f 6e65 7469 6320  wanese Phonetic 
+00000860: 5379 6d62 6f6c 735d 5b7a 6875 7969 6e2d  Symbols][zhuyin-
+00000870: 7769 6b69 5d0d 0a2a 2060 544c 5041 6020  wiki]..* `TLPA` 
+00000880: 2d20 5b54 6169 7761 6e65 7365 204c 616e  - [Taiwanese Lan
+00000890: 6775 6167 6520 5068 6f6e 6574 6963 2041  guage Phonetic A
+000008a0: 6c70 6861 6265 745d 5b74 6c70 612d 7769  lphabet][tlpa-wi
+000008b0: 6b69 5d0d 0a2a 2060 5069 6e67 7969 6d60  ki]..* `Pingyim`
+000008c0: 202d 205b 4262 c3a1 6e6c c3a1 6d20 55c4   - [Bb..nl..m U.
+000008d0: 9320 50c3 ac6e 6779 c4ab 6d20 48c5 8d6e  . P..ngy..m H..n
+000008e0: 6727 c3a0 6e5d 5b70 696e 6779 696d 2d77  g'..n][pingyim-w
+000008f0: 696b 695d 0d0a 2a20 6054 6f6e 6769 6f6e  iki]..* `Tongion
+00000900: 6760 202d 205b 4461 c4ab 2d67 68c3 ae20  g` - [Da..-gh.. 
+00000910: 54c5 8d6e 672d 69c5 8d6e 6720 50c4 ab6e  T..ng-i..ng P..n
+00000920: 672d 696d 5d5b 746f 6e67 696f 6e67 2d77  g-im][tongiong-w
+00000930: 696b 695d 0d0a 2a20 6049 5041 6020 2d20  iki]..* `IPA` - 
+00000940: 5b49 6e74 6572 6e61 7469 6f6e 616c 2050  [International P
+00000950: 686f 6e65 7469 6320 416c 7068 6162 6574  honetic Alphabet
+00000960: 5d5b 6970 612d 7769 6b69 5d0d 0a0d 0a7c  ][ipa-wiki]....|
+00000970: 2074 6578 7420 7c20 5461 696c 6f20 2020   text | Tailo   
+00000980: 7c20 504f 4a20 2020 2020 7c20 5a68 7579  | POJ     | Zhuy
+00000990: 696e 2020 2020 2020 7c20 544c 5041 2020  in      | TLPA  
+000009a0: 2020 2020 7c20 5069 6e67 7969 6d20 7c20      | Pingyim | 
+000009b0: 546f 6e67 696f 6e67 207c 2049 5041 2020  Tongiong | IPA  
+000009c0: 2020 2020 2020 207c 0d0a 7c20 2d2d 2d2d         |..| ----
+000009d0: 207c 202d 2d2d 2d2d 2d2d 207c 202d 2d2d   | ------- | ---
+000009e0: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+000009f0: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 207c  -- | --------- |
+00000a00: 202d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d   ------- | -----
+00000a10: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00000a20: 2d20 7c0d 0a7c 20e5 8fb0 e781 a320 7c20  - |..| ...... | 
+00000a30: 54c3 a269 2d75 c3a2 6e20 7c20 54c3 a269  T..i-u..n | T..i
+00000a40: 2d6f c3a2 6e20 7c20 e384 89e3 849e cb8a  -o..n | ........
+00000a50: 20e3 84a8 e384 a2cb 8a20 7c20 5461 6935   ........ | Tai5
+00000a60: 2075 616e 3520 7c20 44c3 a169 77c3 a16e   uan5 | D..iw..n
+00000a70: 2020 7c20 54c4 8169 2d75 c78e 6e20 207c    | T..i-u..n  |
+00000a80: 2054 6169 c2b2 e281 b520 7561 6ec2 b2e2   Tai..... uan...
+00000a90: 81b5 207c 0d0a 0d0a 2323 2323 2044 6961  .. |....#### Dia
+00000aa0: 6c65 6374 0d0a 0d0a 6064 6961 6c65 6374  lect....`dialect
+00000ab0: 6020 5374 7269 6e67 202d 2070 7265 6665  ` String - prefe
+00000ac0: 7272 6564 2070 726f 6e75 6e63 6961 7469  rred pronunciati
+00000ad0: 6f6e 2e0d 0a0d 0a2a 2060 736f 7574 6860  on.....* `south`
+00000ae0: 2028 6465 6661 756c 7429 202d 205b 5a68   (default) - [Zh
+00000af0: 616e 677a 686f 755d 5b7a 6861 6e67 7a68  angzhou][zhangzh
+00000b00: 6f75 2d77 696b 695d 2d6c 6561 6e69 6e67  ou-wiki]-leaning
+00000b10: 2070 726f 6e75 6e63 6961 7469 6f6e 0d0a   pronunciation..
+00000b20: 2a20 606e 6f72 7468 6020 2d20 5b51 7561  * `north` - [Qua
+00000b30: 6e7a 686f 755d 5b71 7561 6e7a 686f 752d  nzhou][quanzhou-
+00000b40: 7769 6b69 5d2d 6c65 616e 696e 6720 7072  wiki]-leaning pr
+00000b50: 6f6e 756e 6369 6174 696f 6e0d 0a0d 0a7c  onunciation....|
+00000b60: 2074 6578 7420 2020 7c20 736f 7574 6820   text   | south 
+00000b70: 2020 2020 2020 2020 7c20 6e6f 7274 6820          | north 
+00000b80: 2020 2020 2020 2020 7c0d 0a7c 202d 2d2d          |..| ---
+00000b90: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00000ba0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00000bb0: 2d2d 2d20 7c0d 0a7c 20e4 ba94 e69c 88e7  --- |..| .......
+00000bc0: af80 207c 2047 c58d 6f2d 6775 65cc 8d68  .. | G..o-gue..h
+00000bd0: 2d74 7365 6820 7c20 47c5 8d6f 2d67 65cc  -tseh | G..o-ge.
+00000be0: 8d68 2d74 7375 6568 207c 0d0a 0d0a 2323  .h-tsueh |....##
+00000bf0: 2323 2046 6f72 6d61 740d 0a0d 0a60 666f  ## Format....`fo
+00000c00: 726d 6174 6020 5374 7269 6e67 202d 2066  rmat` String - f
+00000c10: 6f72 6d61 7420 696e 2077 6869 6368 2074  ormat in which t
+00000c20: 6f6e 6573 2077 696c 6c20 6265 2072 6570  ones will be rep
+00000c30: 7265 7365 6e74 6564 2069 6e20 7468 6520  resented in the 
+00000c40: 636f 6e76 6572 7465 6420 7365 6e74 656e  converted senten
+00000c50: 6365 2e0d 0a0d 0a2a 2060 6d61 726b 6020  ce.....* `mark` 
+00000c60: 2864 6566 6175 6c74 2920 2d20 7573 6573  (default) - uses
+00000c70: 2064 6961 6372 6974 6963 7320 666f 7220   diacritics for 
+00000c80: 6561 6368 2073 796c 6c61 626c 652e 204e  each syllable. N
+00000c90: 6f74 2061 7661 696c 6162 6c65 2066 6f72  ot available for
+00000ca0: 2054 4c50 412e 0d0a 2a20 606e 756d 6265   TLPA...* `numbe
+00000cb0: 7260 202d 2061 6464 2061 206e 756d 6265  r` - add a numbe
+00000cc0: 7220 7768 6963 6820 7265 7072 6573 656e  r which represen
+00000cd0: 7473 2074 6865 2074 6f6e 6520 6174 2074  ts the tone at t
+00000ce0: 6865 2065 6e64 206f 6620 7468 6520 7379  he end of the sy
+00000cf0: 6c6c 6162 6c65 0d0a 2a20 6073 7472 6970  llable..* `strip
+00000d00: 6020 2d20 7265 6d6f 7665 7320 616e 7920  ` - removes any 
+00000d10: 746f 6e65 206d 6172 6b69 6e67 0d0a 0d0a  tone marking....
+00000d20: 7c20 7465 7874 207c 206d 6172 6b20 2020  | text | mark   
+00000d30: 207c 206e 756d 6265 7220 2020 207c 2073   | number    | s
+00000d40: 7472 6970 2020 207c 0d0a 7c20 2d2d 2d2d  trip   |..| ----
+00000d50: 207c 202d 2d2d 2d2d 2d2d 207c 202d 2d2d   | ------- | ---
+00000d60: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00000d70: 207c 0d0a 7c20 e58f b0e7 81a3 207c 2054   |..| ...... | T
+00000d80: c3a2 692d 75c3 a26e 207c 2054 6169 352d  ..i-u..n | Tai5-
+00000d90: 7561 6e35 207c 2054 6169 2d75 616e 207c  uan5 | Tai-uan |
+00000da0: 0d0a 0d0a 2323 2323 2044 656c 696d 6974  ....#### Delimit
+00000db0: 6572 0d0a 0d0a 6064 656c 696d 6974 6572  er....`delimiter
+00000dc0: 6020 5374 7269 6e67 202d 2073 6574 7320  ` String - sets 
+00000dd0: 7468 6520 6465 6c69 6d69 7465 7220 6368  the delimiter ch
+00000de0: 6172 6163 7465 7220 7468 6174 2077 696c  aracter that wil
+00000df0: 6c20 6265 2070 6c61 6365 6420 696e 2062  l be placed in b
+00000e00: 6574 7765 656e 2073 796c 6c61 626c 6573  etween syllables
+00000e10: 206f 6620 6120 776f 7264 2e0d 0a0d 0a44   of a word.....D
+00000e20: 6566 6175 6c74 2076 616c 7565 2064 6570  efault value dep
+00000e30: 656e 6473 206f 6e20 7468 6520 6368 6f73  ends on the chos
+00000e40: 656e 2060 7379 7374 656d 603a 0d0a 0d0a  en `system`:....
+00000e50: 2a20 6027 2d27 6020 2d20 666f 7220 6054  * `'-'` - for `T
+00000e60: 6169 6c6f 602c 2060 504f 4a60 2c20 6054  ailo`, `POJ`, `T
+00000e70: 6f6e 6769 6f6e 6760 0d0a 2a20 6027 2760  ongiong`..* `''`
+00000e80: 202d 2066 6f72 2060 5069 6e67 7969 6d60   - for `Pingyim`
+00000e90: 0d0a 2a20 6027 2027 6020 2d20 666f 7220  ..* `' '` - for 
+00000ea0: 605a 6875 7969 6e60 2c20 6054 4c50 4160  `Zhuyin`, `TLPA`
+00000eb0: 2c20 6049 5041 600d 0a0d 0a7c 2074 6578  , `IPA`....| tex
+00000ec0: 7420 7c20 272d 2720 2020 2020 7c20 2727  t | '-'     | ''
+00000ed0: 2020 2020 207c 2027 2027 2020 2020 207c       | ' '     |
+00000ee0: 0d0a 7c20 2d2d 2d2d 207c 202d 2d2d 2d2d  ..| ---- | -----
+00000ef0: 2d2d 207c 202d 2d2d 2d2d 2d20 7c20 2d2d  -- | ------ | --
+00000f00: 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0 e781  ----- |..| .....
+00000f10: a320 7c20 54c3 a269 2d75 c3a2 6e20 7c20  . | T..i-u..n | 
+00000f20: 54c3 a269 75c3 a26e 207c 2054 c3a2 6920  T..iu..n | T..i 
+00000f30: 75c3 a26e 207c 0d0a 0d0a 2323 2323 2053  u..n |....#### S
+00000f40: 616e 6468 690d 0a0d 0a60 7361 6e64 6869  andhi....`sandhi
+00000f50: 6020 5374 7269 6e67 202d 2061 7070 6c69  ` String - appli
+00000f60: 6573 2074 6865 205b 7361 6e64 6869 2072  es the [sandhi r
+00000f70: 756c 6573 206f 6620 5461 6977 616e 6573  ules of Taiwanes
+00000f80: 6520 486f 6b6b 6965 6e5d 5b73 616e 6468  e Hokkien][sandh
+00000f90: 692d 7769 6b69 5d20 746f 2073 796c 6c61  i-wiki] to sylla
+00000fa0: 626c 6573 206f 6620 6120 7369 6e67 6c65  bles of a single
+00000fb0: 2077 6f72 642e 0d0a 0d0a 5369 6e63 6520   word.....Since 
+00000fc0: 6974 2773 2064 6966 6669 6375 6c74 2074  it's difficult t
+00000fd0: 6f20 656e 636f 6465 2061 6c6c 2073 616e  o encode all san
+00000fe0: 6468 6920 7275 6c65 732c 2054 6169 6275  dhi rules, Taibu
+00000ff0: 6e20 7072 6f76 6964 6573 206d 756c 7469  n provides multi
+00001000: 706c 6520 6d6f 6465 7320 666f 7220 7361  ple modes for sa
+00001010: 6e64 6869 2063 6f6e 7665 7273 696f 6e20  ndhi conversion 
+00001020: 746f 2061 6c6c 6f77 2066 6f72 2063 7573  to allow for cus
+00001030: 746f 6d69 7365 6420 7361 6e64 6869 2068  tomised sandhi h
+00001040: 616e 646c 696e 672e 0d0a 0d0a 2a20 606e  andling.....* `n
+00001050: 6f6e 6560 202d 2064 6f65 736e 2774 2070  one` - doesn't p
+00001060: 6572 666f 726d 2061 6e79 2074 6f6e 6520  erform any tone 
+00001070: 7361 6e64 6869 0d0a 2a20 6061 7574 6f60  sandhi..* `auto`
+00001080: 202d 2063 6c6f 7365 7374 2061 7070 726f   - closest appro
+00001090: 7869 6d61 7469 6f6e 2074 6f20 6675 6c6c  ximation to full
+000010a0: 2063 6f72 7265 6374 2074 6f6e 6520 7361   correct tone sa
+000010b0: 6e64 6869 206f 6620 5461 6977 616e 6573  ndhi of Taiwanes
+000010c0: 652c 2077 6974 6820 7072 6f70 6572 2073  e, with proper s
+000010d0: 616e 6468 6920 6f66 2070 726f 6e6f 756e  andhi of pronoun
+000010e0: 732c 2073 7566 6669 7865 732c 2061 6e64  s, suffixes, and
+000010f0: 2077 6f72 6473 2077 6974 6820 e4bb 940d   words with ....
+00001100: 0a2a 2060 6578 635f 6c61 7374 6020 2d20  .* `exc_last` - 
+00001110: 6368 616e 6765 7320 746f 6e65 2066 6f72  changes tone for
+00001120: 2065 7665 7279 2073 796c 6c61 626c 6520   every syllable 
+00001130: 6578 6365 7074 2066 6f72 2074 6865 206c  except for the l
+00001140: 6173 7420 6f6e 650d 0a2a 2060 696e 636c  ast one..* `incl
+00001150: 5f6c 6173 7460 202d 2063 6861 6e67 6573  _last` - changes
+00001160: 2074 6f6e 6520 666f 7220 6576 6572 7920   tone for every 
+00001170: 7379 6c6c 6162 6c65 2069 6e63 6c75 6469  syllable includi
+00001180: 6e67 2074 6865 206c 6173 7420 6f6e 650d  ng the last one.
+00001190: 0a0d 0a44 6566 6175 6c74 2076 616c 7565  ...Default value
+000011a0: 2064 6570 656e 6473 206f 6e20 7468 6520   depends on the 
+000011b0: 6368 6f73 656e 2060 7379 7374 656d 603a  chosen `system`:
+000011c0: 0d0a 0d0a 2a20 6061 7574 6f60 202d 2066  ....* `auto` - f
+000011d0: 6f72 2060 546f 6e67 696f 6e67 600d 0a2a  or `Tongiong`..*
+000011e0: 2060 6e6f 6e65 6020 2d20 666f 7220 6054   `none` - for `T
+000011f0: 6169 6c6f 602c 2060 504f 4a60 2c20 605a  ailo`, `POJ`, `Z
+00001200: 6875 7969 6e60 2c20 6054 4c50 4160 2c20  huyin`, `TLPA`, 
+00001210: 6050 696e 6779 696d 602c 2060 4950 4160  `Pingyim`, `IPA`
+00001220: 0d0a 0d0a 7c20 7465 7874 2020 2020 2020  ....| text      
+00001230: 2020 207c 206e 6f6e 6520 2020 2020 2020     | none       
+00001240: 2020 2020 2020 2020 2020 7c20 6175 746f            | auto
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 207c 2065 7863 5f6c 6173 7420 2020 2020   | exc_last     
+00001270: 2020 2020 2020 2020 7c20 696e 636c 5f6c          | incl_l
+00001280: 6173 7420 2020 2020 2020 2020 2020 207c  ast            |
+00001290: 0d0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..| ------------
+000012a0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+000012b0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+000012c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+000012d0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000012e0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+000012f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a  ------------ |..
+00001300: 7c20 e980 99e6 98af e58f b0e7 81a3 e59b  | ..............
+00001310: a1e4 bb94 207c 2054 7365 2073 c4ab 2054  .... | Tse s.. T
+00001320: c3a2 692d 75c3 a26e 2067 c3ad 6e2d c3a1  ..i-u..n g..n-..
+00001330: 207c 2054 7365 2073 c3ac 2054 c481 692d   | Tse s.. T..i-
+00001340: 75c4 816e 2067 696e 2dc3 a120 7c20 5473  u..n gin-.. | Ts
+00001350: c493 2073 c3ac 2054 c481 692d 75c4 816e  .. s.. T..i-u..n
+00001360: 2067 696e 2dc3 a120 7c20 5473 c493 2073   gin-.. | Ts.. s
+00001370: c3ac 2054 c481 692d 75c4 816e 2067 696e  .. T..i-u..n gin
+00001380: 2d61 207c 0d0a 0d0a 5361 6e64 6869 2072  -a |....Sandhi r
+00001390: 756c 6573 2061 6c73 6f20 6368 616e 6765  ules also change
+000013a0: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
+000013b0: 6520 6469 616c 6563 7420 6368 6f73 656e  e dialect chosen
+000013c0: 2e0d 0a0d 0a7c 2074 6578 7420 7c20 6e6f  .....| text | no
+000013d0: 2073 616e 6468 6920 7c20 736f 7574 6820   sandhi | south 
+000013e0: 2020 7c20 6e6f 7274 6820 2020 7c0d 0a7c    | north   |..|
+000013f0: 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d   ---- | --------
+00001400: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
+00001410: 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0 e781  ----- |..| .....
+00001420: a320 7c20 54c3 a269 2d75 c3a2 6e20 2020  . | T..i-u..n   
+00001430: 7c20 54c4 8169 2d75 c3a2 6e20 7c20 54c3  | T..i-u..n | T.
+00001440: a069 2d75 c3a2 6e20 7c0d 0a0d 0a23 2323  .i-u..n |....###
+00001450: 2320 5075 6e63 7475 6174 696f 6e0d 0a0d  # Punctuation...
+00001460: 0a60 7075 6e63 7475 6174 696f 6e60 2053  .`punctuation` S
+00001470: 7472 696e 670d 0a0d 0a2a 2060 666f 726d  tring....* `form
+00001480: 6174 6020 2864 6566 6175 6c74 2920 2d20  at` (default) - 
+00001490: 636f 6e76 6572 7473 2043 6869 6e65 7365  converts Chinese
+000014a0: 2d73 7479 6c65 2070 756e 6374 7561 7469  -style punctuati
+000014b0: 6f6e 2074 6f20 4c61 7469 6e2d 7374 796c  on to Latin-styl
+000014c0: 6520 7075 6e63 7475 6174 696f 6e20 616e  e punctuation an
+000014d0: 6420 6361 7069 7461 6c69 7365 7320 776f  d capitalises wo
+000014e0: 7264 7320 6174 2074 6865 2062 6567 696e  rds at the begin
+000014f0: 6e69 6e67 206f 6620 6561 6368 2073 656e  ning of each sen
+00001500: 7465 6e63 652e 0d0a 2a20 606e 6f6e 6560  tence...* `none`
+00001510: 202d 2070 7265 7365 7276 6573 2043 6869   - preserves Chi
+00001520: 6e65 7365 2d73 7479 6c65 2070 756e 6374  nese-style punct
+00001530: 7561 7469 6f6e 2061 6e64 2064 6f65 736e  uation and doesn
+00001540: 2774 2063 6170 6974 616c 6973 6520 776f  't capitalise wo
+00001550: 7264 7320 6174 2074 6865 2062 6567 696e  rds at the begin
+00001560: 6e69 6e67 206f 6620 6e65 7720 7365 6e74  ning of new sent
+00001570: 656e 6365 732e 0d0a 0d0a 7c20 7465 7874  ences.....| text
+00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2020 2020 2020 2020 207c 2066 6f72             | for
+000015d0: 6d61 7420 2020 2020 2020 2020 2020 2020  mat             
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001630: 206e 6f6e 6520 2020 2020 2020 2020 2020   none           
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001690: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
+000016a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016e0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
+000016f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+00001750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017b0: 2d2d 2d2d 207c 0d0a 7c20 e980 99e6 98af  ---- |..| ......
+000017c0: e887 bae5 8d97 efbc 8ce7 b0a1 e7a8 b1e3  ................
+000017d0: 808c e58d 97e3 808d efbc 88e7 99bd e8a9  ................
+000017e0: b1e5 ad97 efbc 9a54 c3a2 692d 6cc3 a26d  .......T..i-l..m
+000017f0: efbc 9be6 b3a8 e99f b3e7 aca6 e899 9fef  ................
+00001800: bc9a e384 8ae3 849e cb8a 20e3 848b e384  .......... .....
+00001810: a2cb 8aef bc8c e59c 8be8 aa9e efbc 9a54  ...............T
+00001820: c3a1 696e c3a1 6eef bc89 e380 8220 7c20  ..in..n...... | 
+00001830: 5473 6520 73c4 ab20 54c3 a269 2d6c c3a2  Tse s.. T..i-l..
+00001840: 6d2c 206b c3a1 6e2d 7473 6869 6e67 2022  m, k..n-tshing "
+00001850: 6cc3 a26d 2220 2850 65cc 8d68 2d75 c493  l..m" (Pe..h-u..
+00001860: 2d6a c4ab 3a20 54c3 a269 2d6c c3a2 6d3b  -j..: T..i-l..m;
+00001870: 2074 73c3 b92d 696d 2068 c3bb 2d68 c58d   ts..-im h..-h..
+00001880: 3a20 e384 8ae3 849e cb8a 20e3 848b e384  : ........ .....
+00001890: a2cb 8a2c 206b 6f6b 2d67 c3ad 3a20 54c3  ..., kok-g..: T.
+000018a0: a169 6ec3 a16e 292e 207c 2074 7365 2073  .in..n). | tse s
+000018b0: c4ab 2054 c3a2 692d 6cc3 a26d efbc 8c6b  .. T..i-l..m...k
+000018c0: c3a1 6e2d 7473 6869 6e67 e380 8c6c c3a2  ..n-tshing...l..
+000018d0: 6de3 808d efbc 8850 65cc 8d68 2d75 c493  m......Pe..h-u..
+000018e0: 2d6a c4ab efbc 9a54 c3a2 692d 6cc3 a26d  -j.....T..i-l..m
+000018f0: efbc 9b74 73c3 b92d 696d 2068 c3bb 2d68  ...ts..-im h..-h
+00001900: c58d efbc 9ae3 848a e384 9ecb 8a20 e384  ............. ..
+00001910: 8be3 84a2 cb8a efbc 8c6b 6f6b 2d67 c3ad  .........kok-g..
+00001920: efbc 9a54 c3a1 696e c3a1 6eef bc89 e380  ...T..in..n.....
+00001930: 8220 7c0d 0a0d 0a23 2323 2320 436f 6e76  . |....#### Conv
+00001940: 6572 7420 6e6f 6e2d 434a 4b0d 0a0d 0a60  ert non-CJK....`
+00001950: 636f 6e76 6572 745f 6e6f 6e5f 636a 6b60  convert_non_cjk`
+00001960: 2042 6f6f 6c65 616e 202d 2064 6566 696e   Boolean - defin
+00001970: 6573 2077 6865 7468 6572 206f 7220 6e6f  es whether or no
+00001980: 7420 746f 2063 6f6e 7665 7274 206e 6f6e  t to convert non
+00001990: 2d43 6869 6e65 7365 2077 6f72 6473 2e20  -Chinese words. 
+000019a0: 4361 6e20 6265 2075 7365 6420 746f 2063  Can be used to c
+000019b0: 6f6e 7665 7274 2054 6169 6c6f 2074 6f20  onvert Tailo to 
+000019c0: 616e 6f74 6865 7220 726f 6d61 6e69 7361  another romanisa
+000019d0: 7469 6f6e 2073 7973 7465 6d2e 0d0a 0d0a  tion system.....
+000019e0: 2a20 6054 7275 6560 202d 2063 6f6e 7665  * `True` - conve
+000019f0: 7274 206e 6f6e 2d43 6869 6e65 7365 2063  rt non-Chinese c
+00001a00: 6861 7261 6374 6572 2077 6f72 6473 0d0a  haracter words..
+00001a10: 2a20 6046 616c 7365 6020 2864 6566 6175  * `False` (defau
+00001a20: 6c74 2920 2d20 636f 6e76 6572 7420 6f6e  lt) - convert on
+00001a30: 6c79 2043 6869 6e65 7365 2063 6861 7261  ly Chinese chara
+00001a40: 6374 6572 2077 6f72 6473 0d0a 0d0a 7c20  cter words....| 
+00001a50: 7465 7874 2020 2020 2020 7c20 4661 6c73  text      | Fals
+00001a60: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00001a70: 2020 2020 7c20 5472 7565 2020 2020 2020      | True      
+00001a80: 2020 2020 2020 2020 2020 2020 2020 7c0d                |.
+00001a90: 0a7c 202d 2d2d 2d2d 2d2d 2d2d 207c 202d  .| --------- | -
+00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ab0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ad0: 207c 0d0a 7c20 e688 91e9 a39f 7068 c3a1   |..| ......ph..
+00001ae0: 6e67 207c 20e3 86a3 e384 a8e3 849a cb8b  ng | ...........
+00001af0: 20e3 8490 e384 a7e3 849a e386 b7cb 9920   .............. 
+00001b00: 7068 c3a1 6e67 207c 20e3 86a3 e384 a8e3  ph..ng | .......
+00001b10: 849a cb8b 20e3 8490 e384 a7e3 849a e386  .... ...........
+00001b20: b7cb 9920 e384 86e3 84a4 cb8b 207c 0d0a  ... ........ |..
+00001b30: 0d0a 2323 2320 546f 6b65 6e69 7365 720d  ..### Tokeniser.
+00001b40: 0a0d 0a60 546f 6b65 6e69 7365 7260 2063  ...`Tokeniser` c
+00001b50: 6c61 7373 2070 6572 666f 726d 7320 5b4e  lass performs [N
+00001b60: 4c54 4b20 776f 7264 7075 6e63 745f 746f  LTK wordpunct_to
+00001b70: 6b65 6e69 7a65 5d5b 6e6c 746b 2d74 6f6b  kenize][nltk-tok
+00001b80: 656e 697a 655d 2d6c 696b 6520 746f 6b65  enize]-like toke
+00001b90: 6e69 7361 7469 6f6e 206f 6620 6120 5461  nisation of a Ta
+00001ba0: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
+00001bb0: 7365 6e74 656e 6365 2e0d 0a0d 0a60 6060  sentence.....```
+00001bc0: 7079 7468 6f6e 0d0a 2320 636f 6e73 7472  python..# constr
+00001bd0: 7563 746f 720d 0a74 203d 2054 6f6b 656e  uctor..t = Token
+00001be0: 6973 6572 2829 0d0a 0d0a 2320 746f 6b65  iser()....# toke
+00001bf0: 6e69 7365 2054 6169 7761 6e65 7365 2048  nise Taiwanese H
+00001c00: 6f6b 6b69 656e 2073 656e 7465 6e63 650d  okkien sentence.
+00001c10: 0a74 2e74 6f6b 656e 6973 6528 696e 7075  .t.tokenise(inpu
+00001c20: 7429 0d0a 6060 600d 0a0d 0a23 2323 204f  t)..```....### O
+00001c30: 7468 6572 2046 756e 6374 696f 6e73 0d0a  ther Functions..
+00001c40: 0d0a 6060 6070 7974 686f 6e0d 0a23 2043  ..```python..# C
+00001c50: 6f6e 7665 7274 2074 6f20 5472 6164 6974  onvert to Tradit
+00001c60: 696f 6e61 6c0d 0a74 6f5f 7472 6164 6974  ional..to_tradit
+00001c70: 696f 6e61 6c28 696e 7075 7429 0d0a 0d0a  ional(input)....
+00001c80: 2320 436f 6e76 6572 7420 746f 2053 696d  # Convert to Sim
+00001c90: 706c 6966 6965 640d 0a74 6f5f 7369 6d70  plified..to_simp
+00001ca0: 6c69 6669 6564 2869 6e70 7574 290d 0a0d  lified(input)...
+00001cb0: 0a23 2043 6865 636b 2069 6620 7468 6520  .# Check if the 
+00001cc0: 7374 7269 6e67 2069 7320 6675 6c6c 7920  string is fully 
+00001cd0: 636f 6d70 6f73 6564 206f 6620 4368 696e  composed of Chin
+00001ce0: 6573 6520 6368 6172 6163 7465 7273 0d0a  ese characters..
+00001cf0: 6973 5f63 6a6b 2869 6e70 7574 290d 0a60  is_cjk(input)..`
+00001d00: 6060 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2045  ``........<!-- E
+00001d10: 5841 4d50 4c45 202d 2d3e 0d0a 2323 2045  XAMPLE -->..## E
+00001d20: 7861 6d70 6c65 0d0a 0d0a 6060 6070 7974  xample....```pyt
+00001d30: 686f 6e0d 0a23 2043 6f6e 7665 7274 6572  hon..# Converter
+00001d40: 0d0a 6672 6f6d 2074 6169 6275 6e20 696d  ..from taibun im
+00001d50: 706f 7274 2043 6f6e 7665 7274 6572 0d0a  port Converter..
+00001d60: 0d0a 2323 2053 7973 7465 6d0d 0a63 203d  ..## System..c =
+00001d70: 2043 6f6e 7665 7274 6572 2829 2023 2054   Converter() # T
+00001d80: 6169 6c6f 2073 7973 7465 6d20 6465 6661  ailo system defa
+00001d90: 756c 740d 0a63 2e67 6574 2827 e585 88e7  ult..c.get('....
+00001da0: 949f e8ac 9bef bc8c e5ad b8e7 949f e681  ................
+00001db0: ace6 81ac e881 bde3 8082 2729 0d0a 3e3e  ..........')..>>
+00001dc0: 2053 6961 6e2d 7369 6e6e 206b c3b3 6e67   Sian-sinn k..ng
+00001dd0: 2c20 6861 cc8d 6b2d 7369 6e67 2074 69c4  , ha..k-sing ti.
+00001de0: 816d 2d74 69c4 816d 2074 6869 616e 6e2e  .m-ti..m thiann.
+00001df0: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00001e00: 7228 7379 7374 656d 3d27 5a68 7579 696e  r(system='Zhuyin
+00001e10: 2729 0d0a 632e 6765 7428 27e5 8588 e794  ')..c.get('.....
+00001e20: 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6 81ac  ................
+00001e30: e681 ace8 81bd e380 8227 290d 0a3e 3e20  .........')..>> 
+00001e40: e384 92e3 84a7 e384 a220 e384 92e3 86aa  ......... ......
+00001e50: 20e3 848d e386 b2cb 8b2c 20e3 848f e384   ........, .....
+00001e60: 9ae3 86b6 cb99 20e3 8492 e384 a7e3 84a5  ...... .........
+00001e70: 20e3 8489 e384 a7e3 86b0 cbab 20e3 8489   ........... ...
+00001e80: e384 a7e3 86b0 cbab 20e3 848a e384 a7e3  ........ .......
+00001e90: 86a9 2e0d 0a0d 0a23 2320 4469 616c 6563  .......## Dialec
+00001ea0: 740d 0a63 203d 2043 6f6e 7665 7274 6572  t..c = Converter
+00001eb0: 2829 2023 2073 6f75 7468 2064 6961 6c65  () # south diale
+00001ec0: 6374 2064 6566 6175 6c74 0d0a 632e 6765  ct default..c.ge
+00001ed0: 7428 22e6 8891 e6ac b2e7 94a8 e7ae b8e9  t(".............
+00001ee0: a39f e9ad 9a22 290d 0a3e 3e20 4775 c3a1  .....")..>> Gu..
+00001ef0: 2062 6568 20c4 ab6e 6720 74c4 ab20 7473   beh ..ng t.. ts
+00001f00: 6961 cc8d 6820 68c3 ae0d 0a0d 0a63 203d  ia..h h......c =
+00001f10: 2043 6f6e 7665 7274 6572 2864 6961 6c65   Converter(diale
+00001f20: 6374 3d27 6e6f 7274 6827 290d 0a63 2e67  ct='north')..c.g
+00001f30: 6574 2822 e688 91e6 acb2 e794 a8e7 aeb8  et("............
+00001f40: e9a3 9fe9 ad9a 2229 0d0a 3e3e 2047 75c3  ......")..>> Gu.
+00001f50: a120 6275 6568 20c4 ab6e 6720 74c5 ab20  . bueh ..ng t.. 
+00001f60: 7473 6961 cc8d 6820 68c3 bb0d 0a0d 0a23  tsia..h h......#
+00001f70: 2320 466f 726d 6174 0d0a 6320 3d20 436f  # Format..c = Co
+00001f80: 6e76 6572 7465 7228 2920 2320 666f 7220  nverter() # for 
+00001f90: 5461 696c 6f2c 206d 6172 6b20 6279 2064  Tailo, mark by d
+00001fa0: 6566 6175 6c74 0d0a 632e 6765 7428 22e7  efault..c.get(".
+00001fb0: 949f e697 a5e5 bfab e6a8 8222 290d 0a3e  ...........")..>
+00001fc0: 3e20 5365 6e6e 2d6a 69cc 8d74 206b 6875  > Senn-ji..t khu
+00001fd0: c3a0 692d 6c6f cc8d 6b0d 0a0d 0a63 203d  ..i-lo..k....c =
+00001fe0: 2043 6f6e 7665 7274 6572 2866 6f72 6d61   Converter(forma
+00001ff0: 743d 276e 756d 6265 7227 290d 0a63 2e67  t='number')..c.g
+00002000: 6574 2822 e794 9fe6 97a5 e5bf abe6 a882  et("............
+00002010: 2229 0d0a 3e3e 2053 656e 6e31 2d6a 6974  ")..>> Senn1-jit
+00002020: 3820 6b68 7561 6933 2d6c 6f6b 380d 0a0d  8 khuai3-lok8...
+00002030: 0a63 203d 2043 6f6e 7665 7274 6572 2866  .c = Converter(f
+00002040: 6f72 6d61 743d 2773 7472 6970 2729 0d0a  ormat='strip')..
+00002050: 632e 6765 7428 22e7 949f e697 a5e5 bfab  c.get(".........
+00002060: e6a8 8222 290d 0a3e 3e20 5365 6e6e 2d6a  ...")..>> Senn-j
+00002070: 6974 206b 6875 6169 2d6c 6f6b 0d0a 0d0a  it khuai-lok....
+00002080: 2323 2044 656c 696d 6974 6572 0d0a 6320  ## Delimiter..c 
+00002090: 3d20 436f 6e76 6572 7465 7228 6465 6c69  = Converter(deli
+000020a0: 6d69 7465 723d 2727 290d 0a63 2e67 6574  miter='')..c.get
+000020b0: 2822 e585 88e7 949f e8ac 9bef bc8c e5ad  ("..............
+000020c0: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
+000020d0: 2229 0d0a 3e3e 2053 6961 6e73 696e 6e20  ")..>> Siansinn 
+000020e0: 6bc3 b36e 672c 2068 61cc 8d6b 7369 6e67  k..ng, ha..ksing
+000020f0: 2074 69c4 816d 7469 c481 6d20 7468 6961   ti..mti..m thia
+00002100: 6e6e 2e0d 0a0d 0a63 203d 2043 6f6e 7665  nn.....c = Conve
+00002110: 7274 6572 2873 7973 7465 6d3d 2750 696e  rter(system='Pin
+00002120: 6779 696d 272c 2064 656c 696d 6974 6572  gyim', delimiter
+00002130: 3d27 2d27 290d 0a63 2e67 6574 2822 e585  ='-')..c.get("..
+00002140: 88e7 949f e8ac 9bef bc8c e5ad b8e7 949f  ................
+00002150: e681 ace6 81ac e881 bde3 8082 2229 0d0a  ............")..
+00002160: 3e3e 2053 69c4 816e 2d73 6ec4 ab20 67c7  >> Si..n-sn.. g.
+00002170: 926e 672c 2068 c3a1 672d 73c4 ab6e 6720  .ng, h..g-s..ng 
+00002180: 6469 c3a2 6d2d 6469 c3a2 6d20 7469 6ec4  di..m-di..m tin.
+00002190: 812e 0d0a 0d0a 2323 2053 616e 6468 690d  ......## Sandhi.
+000021a0: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
+000021b0: 2023 2066 6f72 2054 6169 6c6f 2c20 7361   # for Tailo, sa
+000021c0: 6e64 6869 206e 6f6e 6520 6279 2064 6566  ndhi none by def
+000021d0: 6175 6c74 0d0a 632e 6765 7428 22e9 8099  ault..c.get("...
+000021e0: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+000021f0: 290d 0a3e 3e20 5473 6520 73c4 ab20 54c3  )..>> Tse s.. T.
+00002200: a269 2d75 c3a2 6e20 67c3 ad6e 2dc3 a10d  .i-u..n g..n-...
+00002210: 0a0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
+00002220: 2873 616e 6468 693d 2761 7574 6f27 290d  (sandhi='auto').
+00002230: 0a63 2e67 6574 2822 e980 99e6 98af e58f  .c.get("........
+00002240: b0e7 81a3 e59b a1e4 bb94 2229 0d0a 3e3e  ..........")..>>
+00002250: 2054 7365 2073 c3ac 2054 c481 692d 75c4   Tse s.. T..i-u.
+00002260: 816e 2067 696e 2dc3 a10d 0a0d 0a63 203d  .n gin-......c =
+00002270: 2043 6f6e 7665 7274 6572 2873 616e 6468   Converter(sandh
+00002280: 693d 2765 7863 5f6c 6173 7427 290d 0a63  i='exc_last')..c
+00002290: 2e67 6574 2822 e980 99e6 98af e58f b0e7  .get("..........
+000022a0: 81a3 e59b a1e4 bb94 2229 0d0a 3e3e 2054  ........")..>> T
+000022b0: 73c4 9320 73c3 ac20 54c4 8169 2d75 c481  s.. s.. T..i-u..
+000022c0: 6e20 6769 6e2d c3a1 0d0a 0d0a 6320 3d20  n gin-......c = 
+000022d0: 436f 6e76 6572 7465 7228 7361 6e64 6869  Converter(sandhi
+000022e0: 3d27 696e 636c 5f6c 6173 7427 290d 0a63  ='incl_last')..c
+000022f0: 2e67 6574 2822 e980 99e6 98af e58f b0e7  .get("..........
+00002300: 81a3 e59b a1e4 bb94 2229 0d0a 3e3e 2054  ........")..>> T
+00002310: 73c4 9320 73c3 ac20 54c4 8169 2d75 c481  s.. s.. T..i-u..
+00002320: 6e20 6769 6e2d 610d 0a0d 0a23 2320 5075  n gin-a....## Pu
+00002330: 6e63 7475 6174 696f 6e0d 0a63 203d 2043  nctuation..c = C
+00002340: 6f6e 7665 7274 6572 2829 2023 2066 6f72  onverter() # for
+00002350: 6d61 7420 7075 6e63 7475 6174 696f 6e20  mat punctuation 
+00002360: 6465 6661 756c 740d 0a63 2e67 6574 2822  default..c.get("
+00002370: e5a4 aae7 a9ba e69c 8be5 8f8b efbc 8ce6  ................
+00002380: 8181 e5a5 bdef bc81 e681 81e9 a39f e9a3  ................
+00002390: bde6 9caa efbc 9f22 290d 0a3e 3e20 5468  .......")..>> Th
+000023a0: c3a0 692d 6b68 6f6e 6720 70c3 ae6e 672d  ..i-khong p..ng-
+000023b0: 69c3 ba2c 206c c3ad 6e2d 68c3 b321 204c  i.., l..n-h..! L
+000023c0: c3ad 6e20 7473 6961 cc8d 682d 70c3 a120  ..n tsia..h-p.. 
+000023d0: 6275 c493 3f0d 0a0d 0a63 203d 2043 6f6e  bu..?....c = Con
+000023e0: 7665 7274 6572 2870 756e 6374 7561 7469  verter(punctuati
+000023f0: 6f6e 3d27 6e6f 6e65 2729 0d0a 632e 6765  on='none')..c.ge
+00002400: 7428 22e5 a4aa e7a9 bae6 9c8b e58f 8bef  t(".............
+00002410: bc8c e681 81e5 a5bd efbc 81e6 8181 e9a3  ................
+00002420: 9fe9 a3bd e69c aaef bc9f 2229 0d0a 3e3e  ..........")..>>
+00002430: 2074 68c3 a069 2d6b 686f 6e67 2070 c3ae   th..i-khong p..
+00002440: 6e67 2d69 c3ba efbc 8c6c c3ad 6e2d 68c3  ng-i.....l..n-h.
+00002450: b3ef bc81 6cc3 ad6e 2074 7369 61cc 8d68  ....l..n tsia..h
+00002460: 2d70 c3a1 2062 75c4 93ef bc9f 0d0a 0d0a  -p.. bu.........
+00002470: 2323 2043 6f6e 7665 7274 206e 6f6e 2d43  ## Convert non-C
+00002480: 4a4b 0d0a 6320 3d20 436f 6e76 6572 7428  JK..c = Convert(
+00002490: 7379 7374 656d 3d27 5a68 7579 696e 2729  system='Zhuyin')
+000024a0: 2023 2046 616c 7365 2063 6f6e 7665 7274   # False convert
+000024b0: 5f6e 6f6e 5f63 6a6b 2064 6566 6175 6c74  _non_cjk default
+000024c0: 0d0a 632e 6765 7428 22e6 8891 e9a3 9f70  ..c.get("......p
+000024d0: 68c3 a16e 6722 290d 0a3e 3e20 e386 a3e3  h..ng")..>> ....
+000024e0: 84a8 e384 9acb 8b20 e384 90e3 84a7 e384  ....... ........
+000024f0: 9ae3 86b7 cb99 2070 68c3 a16e 670d 0a0d  ...... ph..ng...
+00002500: 0a63 203d 2043 6f6e 7665 7274 2873 7973  .c = Convert(sys
+00002510: 7465 6d3d 275a 6875 7969 6e27 2c20 636f  tem='Zhuyin', co
+00002520: 6e76 6572 745f 6e6f 6e5f 636a 6b3d 5472  nvert_non_cjk=Tr
+00002530: 7565 290d 0a63 2e67 6574 2822 e688 91e9  ue)..c.get("....
+00002540: a39f 7068 c3a1 6e67 2229 0d0a 3e3e 20e3  ..ph..ng")..>> .
+00002550: 86a3 e384 a8e3 849a cb8b 20e3 8490 e384  .......... .....
+00002560: a7e3 849a e386 b7cb 9920 e384 86e3 84a4  ......... ......
+00002570: cb8b 0d0a 0d0a 0d0a 2320 546f 6b65 6e69  ........# Tokeni
+00002580: 7365 720d 0a66 726f 6d20 7461 6962 756e  ser..from taibun
+00002590: 2069 6d70 6f72 7420 546f 6b65 6e69 7365   import Tokenise
+000025a0: 720d 0a0d 0a74 203d 2054 6f6b 656e 6973  r....t = Tokenis
+000025b0: 6572 2829 0d0a 742e 746f 6b65 6e69 7365  er()..t.tokenise
+000025c0: 2822 e5a4 aae7 a9ba e69c 8be5 8f8b efbc  ("..............
+000025d0: 8ce6 8181 e5a5 bdef bc81 e681 81e9 a39f  ................
+000025e0: e9a3 bde6 9caa efbc 9f22 290d 0a3e 3e20  .........")..>> 
+000025f0: 5b27 e5a4 aae7 a9ba 272c 2027 e69c 8be5  ['......', '....
+00002600: 8f8b 272c 2027 efbc 8c27 2c20 27e6 8181  ..', '...', '...
+00002610: e5a5 bd27 2c20 27ef bc81 272c 2027 e681  ...', '...', '..
+00002620: 8127 2c20 27e9 a39f e9a3 bd27 2c20 27e6  .', '......', '.
+00002630: 9caa 272c 2027 efbc 9f27 5d0d 0a0d 0a0d  ..', '...'].....
+00002640: 0a23 204f 7468 6572 2046 756e 6374 696f  .# Other Functio
+00002650: 6e73 0d0a 6672 6f6d 2074 6169 6275 6e20  ns..from taibun 
+00002660: 696d 706f 7274 2074 6f5f 7472 6164 6974  import to_tradit
+00002670: 696f 6e61 6c2c 2074 6f5f 7369 6d70 6c69  ional, to_simpli
+00002680: 6669 6564 2c20 6973 5f63 6a6b 0d0a 0d0a  fied, is_cjk....
+00002690: 746f 5f74 7261 6469 7469 6f6e 616c 2822  to_traditional("
+000026a0: e688 91e5 90ac e697 a0e5 8fb0 e6b9 bee8  ................
+000026b0: af9d 2229 0d0a 3e3e 20e6 8891 e881 bde7  ..")..>> .......
+000026c0: 84a1 e58f b0e7 81a3 e8a9 b10d 0a0d 0a74  ...............t
+000026d0: 6f5f 7369 6d70 6c69 6669 6564 2822 e688  o_simplified("..
+000026e0: 91e8 81bd e784 a1e8 87ba e781 a3e8 a9b1  ................
+000026f0: 2229 0d0a 3e3e 20e6 8891 e590 ace6 97a0  ")..>> .........
+00002700: e58f b0e6 b9be e8af 9d0d 0a0d 0a69 735f  .............is_
+00002710: 636a 6b28 27e6 8891 e9a3 9fe9 baad 2729  cjk('.........')
+00002720: 0d0a 3e3e 2054 7275 650d 0a0d 0a69 735f  ..>> True....is_
+00002730: 636a 6b28 27e6 8891 e9a3 9f70 68c3 a16e  cjk('......ph..n
+00002740: 6727 290d 0a3e 3e20 4661 6c73 650d 0a60  g')..>> False..`
+00002750: 6060 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2044  ``........<!-- D
+00002760: 4154 4120 2d2d 3e0d 0a23 2320 4461 7461  ATA -->..## Data
+00002770: 0d0a 0d0a 2d20 5b54 6169 7761 6e65 7365  ....- [Taiwanese
+00002780: 2d43 6869 6e65 7365 204f 6e6c 696e 6520  -Chinese Online 
+00002790: 4469 6374 696f 6e61 7279 5d5b 6f6e 6c69  Dictionary][onli
+000027a0: 6e65 2d64 6963 7469 6f6e 6172 795d 2028  ne-dictionary] (
+000027b0: 7669 6120 5b43 6868 6f65 5461 6967 695d  via [ChhoeTaigi]
+000027c0: 5b64 6174 612d 7669 615d 290d 0a2d 205b  [data-via])..- [
+000027d0: 6954 6169 6769 2043 6869 6e65 7365 2d54  iTaigi Chinese-T
+000027e0: 6169 7761 6e65 7365 2043 6f6d 7061 7269  aiwanese Compari
+000027f0: 736f 6e20 4469 6374 696f 6e61 7279 5d5b  son Dictionary][
+00002800: 6974 6169 6769 2d64 6963 7469 6f6e 6172  itaigi-dictionar
+00002810: 795d 2028 7669 6120 5b43 6868 6f65 5461  y] (via [ChhoeTa
+00002820: 6967 695d 5b64 6174 612d 7669 615d 290d  igi][data-via]).
+00002830: 0a0d 0a0d 0a0d 0a3c 212d 2d20 4143 4b4e  .......<!-- ACKN
+00002840: 4f57 4c45 4447 454d 454e 5453 202d 2d3e  OWLEDGEMENTS -->
+00002850: 0d0a 2323 2041 636b 6e6f 776c 6564 6765  ..## Acknowledge
+00002860: 6d65 6e74 730d 0a0d 0a2d 2053 616d 7565  ments....- Samue
+00002870: 6c20 4a65 6e20 285b 4769 7468 7562 5d5b  l Jen ([Github][
+00002880: 7361 6d75 656c 2d67 6974 6875 625d 20c2  samuel-github] .
+00002890: b720 5b4c 696e 6b65 6449 6e5d 5b73 616d  . [LinkedIn][sam
+000028a0: 7565 6c2d 6c69 6e6b 6564 696e 5d29 202d  uel-linkedin]) -
+000028b0: 2054 6169 7761 6e65 7365 2061 6e64 204d   Taiwanese and M
+000028c0: 616e 6461 7269 6e20 7472 616e 736c 6174  andarin translat
+000028d0: 696f 6e0d 0a0d 0a0d 0a0d 0a3c 212d 2d20  ion........<!-- 
+000028e0: 4c49 4345 4e43 4520 2d2d 3e0d 0a23 2320  LICENCE -->..## 
+000028f0: 4c69 6365 6e63 650d 0a0d 0a42 6563 6175  Licence....Becau
+00002900: 7365 2054 6169 6275 6e20 6973 204d 4954  se Taibun is MIT
+00002910: 2d6c 6963 656e 7365 642c 2061 6e79 2064  -licensed, any d
+00002920: 6576 656c 6f70 6572 2063 616e 2065 7373  eveloper can ess
+00002930: 656e 7469 616c 6c79 2064 6f20 7768 6174  entially do what
+00002940: 6576 6572 2074 6865 7920 7761 6e74 2077  ever they want w
+00002950: 6974 6820 6974 2061 7320 6c6f 6e67 2061  ith it as long a
+00002960: 7320 7468 6579 2069 6e63 6c75 6465 2074  s they include t
+00002970: 6865 206f 7269 6769 6e61 6c20 636f 7079  he original copy
+00002980: 7269 6768 7420 616e 6420 6c69 6365 6e63  right and licenc
+00002990: 6520 6e6f 7469 6365 2069 6e20 616e 7920  e notice in any 
+000029a0: 636f 7069 6573 206f 6620 7468 6520 736f  copies of the so
+000029b0: 7572 6365 2063 6f64 652e 204e 6f74 652c  urce code. Note,
+000029c0: 2074 6861 7420 7468 6520 6461 7461 2075   that the data u
+000029d0: 7365 6420 6279 2074 6865 2070 6163 6b61  sed by the packa
+000029e0: 6765 2069 7320 6c69 6365 6e73 6564 2075  ge is licensed u
+000029f0: 6e64 6572 2061 2064 6966 6665 7265 6e74  nder a different
+00002a00: 2063 6f70 7972 6967 6874 2e0d 0a0d 0a54   copyright.....T
+00002a10: 6865 2064 6174 6120 6973 206c 6963 656e  he data is licen
+00002a20: 7365 6420 756e 6465 7220 5b43 4320 4259  sed under [CC BY
+00002a30: 2d53 4120 342e 305d 5b64 6174 612d 6363  -SA 4.0][data-cc
+00002a40: 5d0d 0a0d 0a0d 0a0d 0a3c 212d 2d20 4d41  ]........<!-- MA
+00002a50: 524b 444f 574e 204c 494e 4b53 202d 2d3e  RKDOWN LINKS -->
+00002a60: 0d0a 5b74 6573 7473 5d3a 2068 7474 7073  ..[tests]: https
+00002a70: 3a2f 2f67 6974 6875 622e 636f 6d2f 616e  ://github.com/an
+00002a80: 6472 6569 6861 722f 7461 6962 756e 2f61  dreihar/taibun/a
+00002a90: 6374 696f 6e73 0d0a 5b74 6573 7473 2d62  ctions..[tests-b
+00002aa0: 6164 6765 5d3a 2068 7474 7073 3a2f 2f69  adge]: https://i
+00002ab0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00002ac0: 7468 7562 2f61 6374 696f 6e73 2f77 6f72  thub/actions/wor
+00002ad0: 6b66 6c6f 772f 7374 6174 7573 2f61 6e64  kflow/status/and
+00002ae0: 7265 6968 6172 2f74 6169 6275 6e2f 6369  reihar/taibun/ci
+00002af0: 2e79 616d 6c3f 7374 796c 653d 666f 722d  .yaml?style=for-
+00002b00: 7468 652d 6261 6467 6526 6c6f 676f 3d67  the-badge&logo=g
+00002b10: 6974 6875 620d 0a5b 636f 6e74 7269 6275  ithub..[contribu
+00002b20: 746f 7273 2d62 6164 6765 5d3a 2068 7474  tors-badge]: htt
+00002b30: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00002b40: 2e69 6f2f 6769 7468 7562 2f63 6f6e 7472  .io/github/contr
+00002b50: 6962 7574 6f72 732f 616e 6472 6569 6861  ibutors/andreiha
+00002b60: 722f 7461 6962 756e 3f73 7479 6c65 3d66  r/taibun?style=f
+00002b70: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b63  or-the-badge..[c
+00002b80: 6f6e 7472 6962 7574 6f72 735d 3a20 2375  ontributors]: #u
+00002b90: 7361 6765 0d0a 5b72 656c 6561 7365 2d62  sage..[release-b
+00002ba0: 6164 6765 5d3a 2068 7474 7073 3a2f 2f69  adge]: https://i
+00002bb0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00002bc0: 7468 7562 2f76 2f72 656c 6561 7365 2f61  thub/v/release/a
+00002bd0: 6e64 7265 6968 6172 2f74 6169 6275 6e3f  ndreihar/taibun?
+00002be0: 636f 6c6f 723d 3338 3631 3863 2673 7479  color=38618c&sty
+00002bf0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00002c00: 0d0a 5b72 656c 6561 7365 5d3a 2068 7474  ..[release]: htt
+00002c10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002c20: 616e 6472 6569 6861 722f 7461 6962 756e  andreihar/taibun
+00002c30: 2f72 656c 6561 7365 730d 0a5b 6c69 6365  /releases..[lice
+00002c40: 6e63 652d 6261 6467 655d 3a20 6874 7470  nce-badge]: http
+00002c50: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00002c60: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+00002c70: 652f 616e 6472 6569 6861 722f 7461 6962  e/andreihar/taib
+00002c80: 756e 3f63 6f6c 6f72 3d30 3030 3030 3026  un?color=000000&
+00002c90: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
+00002ca0: 6467 650d 0a5b 6c69 6365 6e63 655d 3a20  dge..[licence]: 
+00002cb0: 4c49 4345 4e53 450d 0a5b 6c69 6e6b 6564  LICENSE..[linked
+00002cc0: 696e 2d62 6164 6765 5d3a 2068 7474 7073  in-badge]: https
+00002cd0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00002ce0: 6f2f 6261 6467 652f 4c69 6e6b 6564 496e  o/badge/LinkedIn
+00002cf0: 2d30 3037 3742 353f 7374 796c 653d 666f  -0077B5?style=fo
+00002d00: 722d 7468 652d 6261 6467 6526 6c6f 676f  r-the-badge&logo
+00002d10: 3d6c 696e 6b65 6469 6e26 6c6f 676f 436f  =linkedin&logoCo
+00002d20: 6c6f 723d 7768 6974 650d 0a5b 6c69 6e6b  lor=white..[link
+00002d30: 6564 696e 5d3a 2068 7474 7073 3a2f 2f77  edin]: https://w
+00002d40: 7777 2e6c 696e 6b65 6469 6e2e 636f 6d2f  ww.linkedin.com/
+00002d50: 696e 2f61 6e64 7265 692d 6861 7262 6163  in/andrei-harbac
+00002d60: 686f 762f 0d0a 0d0a 5b70 7970 695d 3a20  hov/....[pypi]: 
+00002d70: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00002d80: 2f70 726f 6a65 6374 2f74 6169 6275 6e0d  /project/taibun.
+00002d90: 0a5b 6275 675d 3a20 6874 7470 733a 2f2f  .[bug]: https://
+00002da0: 6769 7468 7562 2e63 6f6d 2f61 6e64 7265  github.com/andre
+00002db0: 6968 6172 2f74 6169 6275 6e2f 6973 7375  ihar/taibun/issu
+00002dc0: 6573 0d0a 5b6f 6e6c 696e 652d 6469 6374  es..[online-dict
+00002dd0: 696f 6e61 7279 5d3a 2068 7474 703a 2f2f  ionary]: http://
+00002de0: 6970 3139 3430 3937 2e6e 7463 752e 6564  ip194097.ntcu.ed
+00002df0: 752e 7477 2f75 6e67 6961 6e2f 736f 616e  u.tw/ungian/soan
+00002e00: 6e74 656e 672f 6368 696c 2f54 6169 686f  nteng/chil/Taiho
+00002e10: 612e 6173 700d 0a5b 6974 6169 6769 2d64  a.asp..[itaigi-d
+00002e20: 6963 7469 6f6e 6172 795d 3a20 6874 7470  ictionary]: http
+00002e30: 733a 2f2f 6974 6169 6769 2e74 772f 0d0a  s://itaigi.tw/..
+00002e40: 5b64 6174 612d 7669 615d 3a20 6874 7470  [data-via]: http
+00002e50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f43  s://github.com/C
+00002e60: 6868 6f65 5461 6967 692f 4368 686f 6554  hhoeTaigi/ChhoeT
+00002e70: 6169 6769 4461 7461 6261 7365 0d0a 5b64  aigiDatabase..[d
+00002e80: 6174 612d 6363 5d3a 2068 7474 7073 3a2f  ata-cc]: https:/
+00002e90: 2f63 7265 6174 6976 6563 6f6d 6d6f 6e73  /creativecommons
+00002ea0: 2e6f 7267 2f6c 6963 656e 7365 732f 6279  .org/licenses/by
+00002eb0: 2d73 612f 342e 302f 6465 6564 2e65 6e0d  -sa/4.0/deed.en.
+00002ec0: 0a5b 7361 6d75 656c 2d67 6974 6875 625d  .[samuel-github]
+00002ed0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00002ee0: 2e63 6f6d 2f53 5353 616d 0d0a 5b73 616d  .com/SSSam..[sam
+00002ef0: 7565 6c2d 6c69 6e6b 6564 696e 5d3a 2068  uel-linkedin]: h
+00002f00: 7474 7073 3a2f 2f77 7777 2e6c 696e 6b65  ttps://www.linke
+00002f10: 6469 6e2e 636f 6d2f 696e 2f73 616d 7565  din.com/in/samue
+00002f20: 6c2d 6a65 6e2f 0d0a 0d0a 5b74 6169 6c6f  l-jen/....[tailo
+00002f30: 2d77 696b 695d 3a20 6874 7470 733a 2f2f  -wiki]: https://
+00002f40: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+00002f50: 2f77 696b 692f 5425 4333 2541 3269 2d75  /wiki/T%C3%A2i-u
+00002f60: 2543 3325 4132 6e5f 4c25 4333 2542 342d  %C3%A2n_L%C3%B4-
+00002f70: 6d25 4333 2541 312d 6a25 4334 2541 425f  m%C3%A1-j%C4%AB_
+00002f80: 5068 696e 672d 696d 5f48 6f6e 672d 2543  Phing-im_Hong-%C
+00002f90: 3325 4130 6e0d 0a5b 706f 6a2d 7769 6b69  3%A0n..[poj-wiki
+00002fa0: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
+00002fb0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00002fc0: 2f50 6525 4343 2538 4468 2d25 4335 2538  /Pe%CC%8Dh-%C5%8
+00002fd0: 4465 2d6a 2543 3425 4142 0d0a 5b7a 6875  De-j%C4%AB..[zhu
+00002fe0: 7969 6e2d 7769 6b69 5d3a 2068 7474 7073  yin-wiki]: https
+00002ff0: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00003000: 6f72 672f 7769 6b69 2f54 6169 7761 6e65  org/wiki/Taiwane
+00003010: 7365 5f50 686f 6e65 7469 635f 5379 6d62  se_Phonetic_Symb
+00003020: 6f6c 730d 0a5b 746c 7061 2d77 696b 695d  ols..[tlpa-wiki]
+00003030: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
+00003040: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00003050: 5461 6977 616e 6573 655f 4c61 6e67 7561  Taiwanese_Langua
+00003060: 6765 5f50 686f 6e65 7469 635f 416c 7068  ge_Phonetic_Alph
+00003070: 6162 6574 0d0a 5b70 696e 6779 696d 2d77  abet..[pingyim-w
+00003080: 696b 695d 3a20 6874 7470 733a 2f2f 656e  iki]: https://en
+00003090: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+000030a0: 696b 692f 4262 2543 3325 4131 6e6c 2543  iki/Bb%C3%A1nl%C
+000030b0: 3325 4131 6d5f 7025 4333 2541 436e 6779  3%A1m_p%C3%ACngy
+000030c0: 2543 3425 4142 6d0d 0a5b 746f 6e67 696f  %C4%ABm..[tongio
+000030d0: 6e67 2d77 696b 695d 3a20 6874 7470 733a  ng-wiki]: https:
+000030e0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+000030f0: 7267 2f77 696b 692f 4461 2543 3425 4142  rg/wiki/Da%C4%AB
+00003100: 2d67 6825 4333 2541 455f 7425 4335 2538  -gh%C3%AE_t%C5%8
+00003110: 446e 672d 6925 4335 2538 446e 675f 7025  Dng-i%C5%8Dng_p%
+00003120: 4334 2541 426e 672d 696d 0d0a 5b69 7061  C4%ABng-im..[ipa
+00003130: 2d77 696b 695d 3a20 6874 7470 733a 2f2f  -wiki]: https://
+00003140: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+00003150: 2f77 696b 692f 496e 7465 726e 6174 696f  /wiki/Internatio
+00003160: 6e61 6c5f 5068 6f6e 6574 6963 5f41 6c70  nal_Phonetic_Alp
+00003170: 6861 6265 740d 0a5b 7a68 616e 677a 686f  habet..[zhangzho
+00003180: 752d 7769 6b69 5d3a 2068 7474 7073 3a2f  u-wiki]: https:/
+00003190: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+000031a0: 672f 7769 6b69 2f5a 6861 6e67 7a68 6f75  g/wiki/Zhangzhou
+000031b0: 5f64 6961 6c65 6374 730d 0a5b 7175 616e  _dialects..[quan
+000031c0: 7a68 6f75 2d77 696b 695d 3a20 6874 7470  zhou-wiki]: http
+000031d0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+000031e0: 2e6f 7267 2f77 696b 692f 5175 616e 7a68  .org/wiki/Quanzh
+000031f0: 6f75 5f64 6961 6c65 6374 730d 0a5b 6e6c  ou_dialects..[nl
+00003200: 746b 2d74 6f6b 656e 697a 655d 3a20 6874  tk-tokenize]: ht
+00003210: 7470 733a 2f2f 6e6c 746b 2e6f 7267 2f61  tps://nltk.org/a
+00003220: 7069 2f6e 6c74 6b2e 746f 6b65 6e69 7a65  pi/nltk.tokenize
+00003230: 2e68 746d 6c0d 0a5b 7361 6e64 6869 2d77  .html..[sandhi-w
+00003240: 696b 695d 3a20 6874 7470 733a 2f2f 656e  iki]: https://en
+00003250: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00003260: 696b 692f 5461 6977 616e 6573 655f 486f  iki/Taiwanese_Ho
+00003270: 6b6b 6965 6e23 546f 6e65 2532 3073 616e  kkien#Tone%20san
+00003280: 6468 693a 7e3a 7465 7874 3d74 686e 6725  dhi:~:text=thng%
+00003290: 4532 2539 4625 4139 2532 3028 2532 3273  E2%9F%A9%20(%22s
+000032a0: 6f75 7025 3232 292e 2d2c 546f 6e65 2532  oup%22).-,Tone%2
+000032b0: 3073 616e 6468 692c 2d25 3542 6564 6974  0sandhi,-%5Bedit
+000032c0: 2535 440d 0a                             %5D..
```

### Comparing `taibun-1.0.0/taibun/data/simplified.json` & `taibun-1.1.0/taibun/data/simplified.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988925802879292%*

 * *Differences: {"'学'": "'學'"}*

```diff
@@ -182,14 +182,15 @@
     "\u5986": "\u599d",
     "\u5987": "\u5a66",
     "\u5988": "\u5abd",
     "\u5a07": "\u5b0c",
     "\u5a31": "\u5a1b",
     "\u5a74": "\u5b30",
     "\u5b59": "\u5b6b",
+    "\u5b66": "\u5b78",
     "\u5b81": "\u5be7",
     "\u5b9d": "\u5bf6",
     "\u5b9e": "\u5be6",
     "\u5ba0": "\u5bf5",
     "\u5ba1": "\u5be9",
     "\u5baa": "\u61b2",
     "\u5bab": "\u5bae",
```

### Comparing `taibun-1.0.0/taibun.egg-info/PKG-INFO` & `taibun-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,738 +1,763 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2074 6169  : 2.1..Name: tai
-00000020: 6275 6e0d 0a56 6572 7369 6f6e 3a20 312e  bun..Version: 1.
-00000030: 302e 300d 0a53 756d 6d61 7279 3a20 5461  0.0..Summary: Ta
-00000040: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
-00000050: 5472 616e 736c 6974 6572 6174 6f72 2061  Transliterator a
-00000060: 6e64 2054 6f6b 656e 6973 6572 0d0a 486f  nd Tokeniser..Ho
-00000070: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-00000080: 2f67 6974 6875 622e 636f 6d2f 616e 6472  /github.com/andr
-00000090: 6569 6861 722f 7461 6962 756e 0d0a 4175  eihar/taibun..Au
-000000a0: 7468 6f72 3a20 416e 6472 6569 2048 6172  thor: Andrei Har
-000000b0: 6261 6368 6f76 0d0a 4175 7468 6f72 2d65  bachov..Author-e
-000000c0: 6d61 696c 3a20 616e 6472 6569 2e68 6172  mail: andrei.har
-000000d0: 6261 6368 6f76 4067 6d61 696c 2e63 6f6d  bachov@gmail.com
-000000e0: 0d0a 4c69 6365 6e73 653a 204d 4954 0d0a  ..License: MIT..
-000000f0: 4b65 7977 6f72 6473 3a20 7079 7468 6f6e  Keywords: python
-00000100: 2c74 6169 7761 6e2c 7461 6977 616e 6573  ,taiwan,taiwanes
-00000110: 652c 7461 6967 692c 686f 6b6b 6965 6e2c  e,taigi,hokkien,
-00000120: 726f 6d61 6e69 7a61 7469 6f6e 2c74 7261  romanization,tra
-00000130: 6e73 6c69 7465 7261 7469 6f6e 2c74 7261  nsliteration,tra
-00000140: 6e73 6c69 7465 7261 746f 722c 746f 6b65  nsliterator,toke
-00000150: 6e69 7a61 7469 6f6e 2c74 6f6b 656e 697a  nization,tokeniz
-00000160: 6572 0d0a 436c 6173 7369 6669 6572 3a20  er..Classifier: 
-00000170: 546f 7069 6320 3a3a 2054 6578 7420 5072  Topic :: Text Pr
-00000180: 6f63 6573 7369 6e67 203a 3a20 4c69 6e67  ocessing :: Ling
-00000190: 7569 7374 6963 0d0a 436c 6173 7369 6669  uistic..Classifi
-000001a0: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
-000001b0: 5374 6174 7573 203a 3a20 3320 2d20 416c  Status :: 3 - Al
-000001c0: 7068 610d 0a43 6c61 7373 6966 6965 723a  pha..Classifier:
-000001d0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-000001e0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-000001f0: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000220: 330d 0a43 6c61 7373 6966 6965 723a 204f  3..Classifier: O
-00000230: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000240: 3a3a 2055 6e69 780d 0a43 6c61 7373 6966  :: Unix..Classif
-00000250: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000260: 7973 7465 6d20 3a3a 204d 6163 4f53 203a  ystem :: MacOS :
-00000270: 3a20 4d61 634f 5320 580d 0a43 6c61 7373  : MacOS X..Class
-00000280: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000290: 2053 7973 7465 6d20 3a3a 204d 6963 726f   System :: Micro
-000002a0: 736f 6674 203a 3a20 5769 6e64 6f77 730d  soft :: Windows.
-000002b0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-000002c0: 3a20 3e3d 332e 370d 0a44 6573 6372 6970  : >=3.7..Descrip
-000002d0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-000002e0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-000002f0: 0d0a 4c69 6365 6e73 652d 4669 6c65 3a20  ..License-File: 
-00000300: 4c49 4345 4e53 450d 0a0d 0a0d 0a3c 212d  LICENSE......<!-
-00000310: 2d20 5052 4f4a 4543 5420 4c4f 474f 202d  - PROJECT LOGO -
-00000320: 2d3e 0d0d 0a3c 6272 202f 3e0d 0d0a 3c64  ->...<br />...<d
-00000330: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
-00000340: 223e 0d0d 0a20 203c 6120 6872 6566 3d22  ">...  <a href="
-00000350: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000360: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
-00000370: 6275 6e22 3e0d 0d0a 2020 2020 3c69 6d67  bun">...    <img
-00000380: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000390: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000003a0: 656e 742e 636f 6d2f 616e 6472 6569 6861  ent.com/andreiha
-000003b0: 722f 7461 6962 756e 2f6d 6169 6e2f 7265  r/taibun/main/re
-000003c0: 6164 6d65 2f6c 6f67 6f2e 706e 6722 2061  adme/logo.png" a
-000003d0: 6c74 3d22 4c6f 676f 2220 7769 6474 683d  lt="Logo" width=
-000003e0: 2239 3022 2068 6569 6768 743d 2238 3022  "90" height="80"
-000003f0: 3e0d 0d0a 2020 3c2f 613e 0d0d 0a20 200d  >...  </a>...  .
-00000400: 0d0a 2320 5461 6962 756e 0d0d 0a0d 0d0a  ..# Taibun......
-00000410: 0d0d 0a0d 0d0a 3c21 2d2d 2050 524f 4a45  ......<!-- PROJE
-00000420: 4354 2053 4849 454c 4453 202d 2d3e 0d0d  CT SHIELDS -->..
-00000430: 0a5b 215b 5465 7374 735d 5b74 6573 7473  .[![Tests][tests
-00000440: 2d62 6164 6765 5d5d 5b74 6573 7473 5d0d  -badge]][tests].
-00000450: 0d0a 5b21 5b43 6f6e 7472 6962 7574 6f72  ..[![Contributor
-00000460: 735d 5b63 6f6e 7472 6962 7574 6f72 732d  s][contributors-
-00000470: 6261 6467 655d 5d5b 636f 6e74 7269 6275  badge]][contribu
-00000480: 746f 7273 5d0d 0d0a 5b21 5b52 656c 6561  tors]...[![Relea
-00000490: 7365 5d5b 7265 6c65 6173 652d 6261 6467  se][release-badg
-000004a0: 655d 5d5b 7265 6c65 6173 655d 0d0d 0a5b  e]][release]...[
-000004b0: 215b 4c69 6365 6e63 655d 5b6c 6963 656e  ![Licence][licen
-000004c0: 6365 2d62 6164 6765 5d5d 5b6c 6963 656e  ce-badge]][licen
-000004d0: 6365 5d0d 0d0a 5b21 5b4c 696e 6b65 6449  ce]...[![LinkedI
-000004e0: 6e5d 5b6c 696e 6b65 6469 6e2d 6261 6467  n][linkedin-badg
-000004f0: 655d 5d5b 6c69 6e6b 6564 696e 5d0d 0d0a  e]][linkedin]...
-00000500: 0d0d 0a2a 2a54 6169 7761 6e65 7365 2048  ...**Taiwanese H
-00000510: 6f6b 6b69 656e 2054 7261 6e73 6c69 7465  okkien Translite
-00000520: 7261 746f 7220 616e 6420 546f 6b65 6e69  rator and Tokeni
-00000530: 7365 722a 2a0d 0d0a 0d0d 0a49 7420 6861  ser**......It ha
-00000540: 7320 6d65 7468 6f64 7320 7468 6174 2061  s methods that a
-00000550: 6c6c 6f77 2074 6f20 6375 7374 6f6d 6973  llow to customis
-00000560: 6520 7472 616e 736c 6974 6572 6174 696f  e transliteratio
-00000570: 6e20 616e 6420 7265 7472 6965 7665 2061  n and retrieve a
-00000580: 6e79 206e 6563 6573 7361 7279 2069 6e66  ny necessary inf
-00000590: 6f72 6d61 7469 6f6e 2061 626f 7574 2054  ormation about T
-000005a0: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
-000005b0: 2070 726f 6e75 6e63 6961 7469 6f6e 2e3c   pronunciation.<
-000005c0: 6272 202f 3e0d 0d0a 496e 636c 7564 6573  br />...Includes
-000005d0: 2077 6f72 6420 746f 6b65 6e69 7365 7220   word tokeniser 
-000005e0: 666f 7220 5461 6977 616e 6573 6520 486f  for Taiwanese Ho
-000005f0: 6b6b 6965 6e2e 0d0d 0a0d 0d0a 5b52 6570  kkien.......[Rep
-00000600: 6f72 7420 4275 675d 5b62 7567 5d20 e280  ort Bug][bug] ..
-00000610: a20d 0d0a 5b50 7950 495d 5b70 7970 695d  ....[PyPI][pypi]
-00000620: 0d0d 0a0d 0d0a 3c2f 6469 763e 0d0d 0a0d  ......</div>....
-00000630: 0d0a 0d0d 0a0d 0d0a 2d2d 2d0d 0d0a 0d0d  ........---.....
-00000640: 0a0d 0d0a 0d0d 0a3c 212d 2d20 5441 424c  .......<!-- TABL
-00000650: 4520 4f46 2043 4f4e 5445 4e54 5320 2d2d  E OF CONTENTS --
-00000660: 3e0d 0d0a 3c64 6574 6169 6c73 206f 7065  >...<details ope
-00000670: 6e3e 0d0d 0a20 203c 7375 6d6d 6172 793e  n>...  <summary>
-00000680: 5461 626c 6520 6f66 2043 6f6e 7465 6e74  Table of Content
-00000690: 733c 2f73 756d 6d61 7279 3e0d 0d0a 2020  s</summary>...  
-000006a0: 3c6f 6c3e 0d0d 0a20 2020 203c 6c69 3e3c  <ol>...    <li><
-000006b0: 6120 6872 6566 3d22 2369 6e73 7461 6c6c  a href="#install
-000006c0: 223e 496e 7374 616c 6c3c 2f61 3e3c 2f6c  ">Install</a></l
-000006d0: 693e 0d0d 0a20 2020 203c 6c69 3e0d 0d0a  i>...    <li>...
-000006e0: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
-000006f0: 7573 6167 6522 3e55 7361 6765 3c2f 613e  usage">Usage</a>
-00000700: 0d0d 0a20 2020 2020 203c 756c 3e0d 0d0a  ...      <ul>...
-00000710: 2020 2020 2020 2020 3c6c 693e 0d0d 0a20          <li>... 
-00000720: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
-00000730: 3d22 2363 6f6e 7665 7274 6572 223e 436f  ="#converter">Co
-00000740: 6e76 6572 7465 723c 2f61 3e0d 0d0a 2020  nverter</a>...  
-00000750: 2020 2020 2020 2020 3c75 6c3e 0d0d 0a20          <ul>... 
-00000760: 2020 2020 2020 2020 2020 203c 6c69 3e3c             <li><
-00000770: 6120 6872 6566 3d22 2373 7973 7465 6d22  a href="#system"
-00000780: 3e53 7973 7465 6d3c 2f61 3e3c 2f6c 693e  >System</a></li>
-00000790: 0d0d 0a20 2020 2020 2020 2020 2020 203c  ...            <
-000007a0: 6c69 3e3c 6120 6872 6566 3d22 2364 6961  li><a href="#dia
-000007b0: 6c65 6374 223e 4469 616c 6563 743c 2f61  lect">Dialect</a
-000007c0: 3e3c 2f6c 693e 0d0d 0a20 2020 2020 2020  ></li>...       
-000007d0: 2020 2020 203c 6c69 3e3c 6120 6872 6566       <li><a href
-000007e0: 3d22 2366 6f72 6d61 7422 3e46 6f72 6d61  ="#format">Forma
-000007f0: 743c 2f61 3e3c 2f6c 693e 0d0d 0a20 2020  t</a></li>...   
-00000800: 2020 2020 2020 2020 203c 6c69 3e3c 6120           <li><a 
-00000810: 6872 6566 3d22 2364 656c 696d 6974 6572  href="#delimiter
-00000820: 223e 4465 6c69 6d69 7465 723c 2f61 3e3c  ">Delimiter</a><
-00000830: 2f6c 693e 0d0d 0a20 2020 2020 2020 2020  /li>...         
-00000840: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-00000850: 2373 616e 6468 6922 3e53 616e 6468 693c  #sandhi">Sandhi<
-00000860: 2f61 3e3c 2f6c 693e 0d0d 0a20 2020 2020  /a></li>...     
-00000870: 2020 2020 2020 203c 6c69 3e3c 6120 6872         <li><a hr
-00000880: 6566 3d22 2370 756e 6374 7561 7469 6f6e  ef="#punctuation
-00000890: 223e 5075 6e63 7475 6174 696f 6e3c 2f61  ">Punctuation</a
-000008a0: 3e3c 2f6c 693e 0d0d 0a20 2020 2020 2020  ></li>...       
-000008b0: 2020 203c 2f75 6c3e 0d0d 0a20 2020 2020     </ul>...     
-000008c0: 2020 203c 2f6c 693e 0d0d 0a20 2020 2020     </li>...     
-000008d0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-000008e0: 2374 6f6b 656e 6973 6572 223e 546f 6b65  #tokeniser">Toke
-000008f0: 6e69 7365 723c 2f61 3e3c 2f6c 693e 0d0d  niser</a></li>..
-00000900: 0a20 2020 2020 203c 2f75 6c3e 0d0d 0a20  .      </ul>... 
-00000910: 2020 203c 2f6c 693e 0d0d 0a20 2020 203c     </li>...    <
-00000920: 6c69 3e3c 6120 6872 6566 3d22 2365 7861  li><a href="#exa
-00000930: 6d70 6c65 223e 4578 616d 706c 653c 2f61  mple">Example</a
-00000940: 3e3c 2f6c 693e 0d0d 0a20 2020 203c 6c69  ></li>...    <li
-00000950: 3e3c 6120 6872 6566 3d22 2364 6174 6122  ><a href="#data"
-00000960: 3e44 6174 613c 2f61 3e3c 2f6c 693e 0d0d  >Data</a></li>..
-00000970: 0a20 2020 203c 6c69 3e3c 6120 6872 6566  .    <li><a href
-00000980: 3d22 236c 6963 656e 6365 223e 4c69 6365  ="#licence">Lice
-00000990: 6e63 653c 2f61 3e3c 2f6c 693e 0d0d 0a20  nce</a></li>... 
-000009a0: 203c 2f6f 6c3e 0d0d 0a3c 2f64 6574 6169   </ol>...</detai
-000009b0: 6c73 3e0d 0d0a 0d0d 0a0d 0d0a 0d0d 0a3c  ls>............<
-000009c0: 212d 2d20 494e 5354 414c 4c20 2d2d 3e0d  !-- INSTALL -->.
-000009d0: 0d0a 2323 2049 6e73 7461 6c6c 0d0d 0a0d  ..## Install....
-000009e0: 0d0a 5461 6962 756e 2063 616e 2062 6520  ..Taibun can be 
-000009f0: 696e 7374 616c 6c65 6420 6672 6f6d 205b  installed from [
-00000a00: 7079 7069 5d5b 7079 7069 5d0d 0d0a 0d0d  pypi][pypi].....
-00000a10: 0a60 6060 6261 7368 0d0d 0a24 2070 6970  .```bash...$ pip
-00000a20: 2069 6e73 7461 6c6c 2074 6169 6275 6e0d   install taibun.
-00000a30: 0d0a 6060 600d 0d0a 0d0d 0a0d 0d0a 0d0d  ..```...........
-00000a40: 0a3c 212d 2d20 5553 4147 4520 2d2d 3e0d  .<!-- USAGE -->.
-00000a50: 0d0a 2323 2055 7361 6765 0d0d 0a0d 0d0a  ..## Usage......
-00000a60: 2323 2320 436f 6e76 6572 7465 720d 0d0a  ### Converter...
-00000a70: 0d0d 0a60 436f 6e76 6572 7465 7260 2063  ...`Converter` c
-00000a80: 6c61 7373 2074 7261 6e73 6c69 7465 7261  lass translitera
-00000a90: 7465 7320 7468 6520 4368 696e 6573 6520  tes the Chinese 
-00000aa0: 6368 6172 6163 7465 7273 2074 6f20 7468  characters to th
-00000ab0: 6520 6368 6f73 656e 2074 7261 6e73 6c69  e chosen transli
-00000ac0: 7465 7261 7469 6f6e 2073 7973 7465 6d20  teration system 
-00000ad0: 7769 7468 2070 6172 616d 6574 6572 7320  with parameters 
-00000ae0: 7370 6563 6966 6965 6420 6279 2074 6865  specified by the
-00000af0: 2064 6576 656c 6f70 6572 2e20 576f 726b   developer. Work
-00000b00: 7320 666f 7220 626f 7468 2054 7261 6469  s for both Tradi
-00000b10: 7469 6f6e 616c 2061 6e64 2053 696d 706c  tional and Simpl
-00000b20: 6966 6965 6420 6368 6172 6163 7465 7273  ified characters
-00000b30: 2e0d 0d0a 0d0d 0a60 6060 7079 7468 6f6e  .......```python
-00000b40: 0d0d 0a23 2063 6f6e 7374 7275 6374 6f72  ...# constructor
-00000b50: 0d0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
-00000b60: 2873 7973 7465 6d2c 2064 6961 6c65 6374  (system, dialect
-00000b70: 2c20 666f 726d 6174 2c20 6465 6c69 6d69  , format, delimi
-00000b80: 7465 722c 2073 616e 6468 692c 2070 756e  ter, sandhi, pun
-00000b90: 6374 7561 7469 6f6e 290d 0d0a 0d0d 0a23  ctuation)......#
-00000ba0: 2074 7261 6e73 6c69 7465 7261 7465 2043   transliterate C
-00000bb0: 6869 6e65 7365 2063 6861 7261 6374 6572  hinese character
-00000bc0: 730d 0d0a 632e 6765 7428 696e 7075 7429  s...c.get(input)
-00000bd0: 0d0d 0a0d 0d0a 2320 636f 6e76 6572 7420  ......# convert 
-00000be0: 5369 6d70 6c69 6669 6564 2043 6869 6e65  Simplified Chine
-00000bf0: 7365 2063 6861 7261 6374 6572 7320 746f  se characters to
-00000c00: 2054 7261 6469 7469 6f6e 616c 2043 6869   Traditional Chi
-00000c10: 6e65 7365 2043 6861 7261 6374 6572 730d  nese Characters.
-00000c20: 0d0a 632e 746f 5f74 7261 6469 7469 6f6e  ..c.to_tradition
-00000c30: 616c 2869 6e70 7574 290d 0d0a 6060 600d  al(input)...```.
-00000c40: 0d0a 0d0d 0a23 2323 2320 5379 7374 656d  .....#### System
-00000c50: 0d0d 0a0d 0d0a 6073 7973 7465 6d60 2053  ......`system` S
-00000c60: 7472 696e 6720 2d20 7379 7374 656d 206f  tring - system o
-00000c70: 6620 7472 616e 736c 6974 6572 6174 696f  f transliteratio
-00000c80: 6e2e 0d0d 0a0d 0d0a 2a20 6054 6169 6c6f  n.......* `Tailo
-00000c90: 6020 2864 6566 6175 6c74 2920 2d20 5b54  ` (default) - [T
-00000ca0: c3a2 692d 75c3 a26e 204c c3b4 2d6d c3a1  ..i-u..n L..-m..
-00000cb0: 2d6a c4ab 2050 6869 6e67 2d69 6d20 486f  -j.. Phing-im Ho
-00000cc0: 6e67 2dc3 a06e 5d5b 7461 696c 6f2d 7769  ng-..n][tailo-wi
-00000cd0: 6b69 5d0d 0d0a 2a20 6050 4f4a 6020 2d20  ki]...* `POJ` - 
-00000ce0: 5b50 65cc 8d68 2dc5 8d65 2d6a c4ab 5d5b  [Pe..h-..e-j..][
-00000cf0: 706f 6a2d 7769 6b69 5d0d 0d0a 2a20 605a  poj-wiki]...* `Z
-00000d00: 6875 7969 6e60 202d 205b 5461 6977 616e  huyin` - [Taiwan
-00000d10: 6573 6520 5068 6f6e 6574 6963 2053 796d  ese Phonetic Sym
-00000d20: 626f 6c73 5d5b 7a68 7579 696e 2d77 696b  bols][zhuyin-wik
-00000d30: 695d 0d0d 0a2a 2060 544c 5041 6020 2d20  i]...* `TLPA` - 
-00000d40: 5b54 6169 7761 6e65 7365 204c 616e 6775  [Taiwanese Langu
-00000d50: 6167 6520 5068 6f6e 6574 6963 2041 6c70  age Phonetic Alp
-00000d60: 6861 6265 745d 5b74 6c70 612d 7769 6b69  habet][tlpa-wiki
-00000d70: 5d0d 0d0a 2a20 6050 696e 6779 696d 6020  ]...* `Pingyim` 
-00000d80: 2d20 5b42 62c3 a16e 6cc3 a16d 2055 c493  - [Bb..nl..m U..
-00000d90: 2050 c3ac 6e67 79c4 ab6d 2048 c58d 6e67   P..ngy..m H..ng
-00000da0: 27c3 a06e 5d5b 7069 6e67 7969 6d2d 7769  '..n][pingyim-wi
-00000db0: 6b69 5d0d 0d0a 2a20 6054 6f6e 6769 6f6e  ki]...* `Tongion
-00000dc0: 6760 202d 205b 4461 c4ab 2d67 68c3 ae20  g` - [Da..-gh.. 
-00000dd0: 54c5 8d6e 672d 69c5 8d6e 6720 50c4 ab6e  T..ng-i..ng P..n
-00000de0: 672d 696d 5d5b 746f 6e67 696f 6e67 2d77  g-im][tongiong-w
-00000df0: 696b 695d 0d0d 0a0d 0d0a 7c20 7465 7874  iki]......| text
-00000e00: 207c 2054 6169 6c6f 2020 207c 2050 4f4a   | Tailo   | POJ
-00000e10: 2020 2020 207c 205a 6875 7969 6e20 2020       | Zhuyin   
-00000e20: 2020 207c 2054 4c50 4120 2020 2020 207c     | TLPA      |
-00000e30: 2050 696e 6779 696d 207c 2054 6f6e 6769   Pingyim | Tongi
-00000e40: 6f6e 6720 7c0d 0d0a 7c2d 2d2d 2d2d 2d7c  ong |...|------|
-00000e50: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
-00000e60: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00000e70: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -|-----------|--
-00000e80: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000e90: 2d2d 7c0d 0d0a 7c20 e887 bae7 81a3 207c  --|...| ...... |
-00000ea0: 2054 c3a2 692d 75c3 a26e 207c 2054 c3a2   T..i-u..n | T..
-00000eb0: 692d 6fc3 a26e 207c 20e3 8489 e384 9ecb  i-o..n | .......
-00000ec0: 8a20 e384 a8e3 84a2 cb8a 207c 2054 6169  . ........ | Tai
-00000ed0: 3520 7561 6e35 207c 2044 c3a1 6977 c3a1  5 uan5 | D..iw..
-00000ee0: 6e20 207c 2054 c481 692d 75c7 8e6e 2020  n  | T..i-u..n  
-00000ef0: 7c0d 0d0a 0d0d 0a23 2323 2320 4469 616c  |......#### Dial
-00000f00: 6563 740d 0d0a 0d0d 0a60 6469 616c 6563  ect......`dialec
-00000f10: 7460 2053 7472 696e 6720 2d20 7072 6566  t` String - pref
-00000f20: 6572 7265 6420 7072 6f6e 756e 6369 6174  erred pronunciat
-00000f30: 696f 6e2e 0d0d 0a0d 0d0a 2a20 6073 6f75  ion.......* `sou
-00000f40: 7468 6020 2864 6566 6175 6c74 2920 2d20  th` (default) - 
-00000f50: 5b5a 6861 6e67 7a68 6f75 5d5b 7a68 616e  [Zhangzhou][zhan
-00000f60: 677a 686f 752d 7769 6b69 5d2d 6c65 616e  gzhou-wiki]-lean
-00000f70: 696e 6720 7072 6f6e 756e 6369 6174 696f  ing pronunciatio
-00000f80: 6e0d 0d0a 2a20 606e 6f72 7468 6020 2d20  n...* `north` - 
-00000f90: 5b51 7561 6e7a 686f 755d 5b71 7561 6e7a  [Quanzhou][quanz
-00000fa0: 686f 752d 7769 6b69 5d2d 6c65 616e 696e  hou-wiki]-leanin
-00000fb0: 6720 7072 6f6e 756e 6369 6174 696f 6e0d  g pronunciation.
-00000fc0: 0d0a 0d0d 0a7c 2074 6578 7420 2020 7c20  .....| text   | 
-00000fd0: 736f 7574 6820 2020 2020 2020 2020 7c20  south         | 
-00000fe0: 6e6f 7274 6820 2020 2020 2020 2020 7c0d  north         |.
-00000ff0: 0d0a 7c2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  ..|--------|----
-00001000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00001010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0d0d 0a7c  -----------|...|
-00001020: 20e4 ba94 e69c 88e7 af80 207c 2047 c58d   ......... | G..
-00001030: 6f2d 6775 65cc 8d68 2d74 7365 6820 7c20  o-gue..h-tseh | 
-00001040: 47c5 8d6f 2d67 65cc 8d68 2d74 7375 6568  G..o-ge..h-tsueh
-00001050: 207c 0d0d 0a0d 0d0a 2323 2323 2046 6f72   |......#### For
-00001060: 6d61 740d 0d0a 0d0d 0a60 666f 726d 6174  mat......`format
-00001070: 6020 5374 7269 6e67 202d 2066 6f72 6d61  ` String - forma
-00001080: 7420 696e 2077 6869 6368 2074 6f6e 6573  t in which tones
-00001090: 2077 696c 6c20 6265 2072 6570 7265 7365   will be represe
-000010a0: 6e74 6564 2069 6e20 7468 6520 636f 6e76  nted in the conv
-000010b0: 6572 7465 6420 7365 6e74 656e 6365 2e0d  erted sentence..
-000010c0: 0d0a 0d0d 0a2a 2060 6d61 726b 6020 2864  .....* `mark` (d
-000010d0: 6566 6175 6c74 2920 2d20 7573 6573 2064  efault) - uses d
-000010e0: 6961 6372 6974 6963 7320 666f 7220 6561  iacritics for ea
-000010f0: 6368 2073 796c 6c61 626c 652e 204e 6f74  ch syllable. Not
-00001100: 2061 7661 696c 6162 6c65 2066 6f72 2054   available for T
-00001110: 4c50 412e 0d0d 0a2a 2060 6e75 6d62 6572  LPA....* `number
-00001120: 6020 2d20 6164 6420 6120 6e75 6d62 6572  ` - add a number
-00001130: 2077 6869 6368 2072 6570 7265 7365 6e74   which represent
-00001140: 7320 7468 6520 746f 6e65 2061 7420 7468  s the tone at th
-00001150: 6520 656e 6420 6f66 2074 6865 2073 796c  e end of the syl
-00001160: 6c61 626c 650d 0d0a 2a20 6073 7472 6970  lable...* `strip
-00001170: 6020 2d20 7265 6d6f 7665 7320 616e 7920  ` - removes any 
-00001180: 746f 6e65 206d 6172 6b69 6e67 0d0d 0a0d  tone marking....
-00001190: 0d0a 7c20 7465 7874 207c 206d 6172 6b20  ..| text | mark 
-000011a0: 2020 207c 206e 756d 6265 7220 2020 207c     | number    |
-000011b0: 2073 7472 6970 2020 207c 0d0d 0a7c 2d2d   strip   |...|--
-000011c0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d  ----|---------|-
-000011d0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-000011e0: 2d2d 2d2d 7c0d 0d0a 7c20 e887 bae7 81a3  ----|...| ......
-000011f0: 207c 2054 c3a2 692d 75c3 a26e 207c 2054   | T..i-u..n | T
-00001200: 6169 352d 7561 6e35 207c 2054 6169 2d75  ai5-uan5 | Tai-u
-00001210: 616e 207c 0d0d 0a0d 0d0a 2323 2323 2044  an |......#### D
-00001220: 656c 696d 6974 6572 0d0d 0a0d 0d0a 6064  elimiter......`d
-00001230: 656c 696d 6974 6572 6020 5374 7269 6e67  elimiter` String
-00001240: 202d 2073 6574 7320 7468 6520 6465 6c69   - sets the deli
-00001250: 6d69 7465 7220 6368 6172 6163 7465 7220  miter character 
-00001260: 7468 6174 2077 696c 6c20 6265 2070 6c61  that will be pla
-00001270: 6365 6420 696e 2062 6574 7765 656e 2073  ced in between s
-00001280: 796c 6c61 626c 6573 206f 6620 6120 776f  yllables of a wo
-00001290: 7264 2e0d 0d0a 0d0d 0a44 6566 6175 6c74  rd.......Default
-000012a0: 2076 616c 7565 2064 6570 656e 6473 206f   value depends o
-000012b0: 6e20 7468 6520 6368 6f73 656e 2060 7379  n the chosen `sy
-000012c0: 7374 656d 603a 0d0d 0a0d 0d0a 2a20 6027  stem`:......* `'
-000012d0: 2d27 6020 2d20 666f 7220 6054 6169 6c6f  -'` - for `Tailo
-000012e0: 602c 2060 504f 4a60 2c20 6054 6f6e 6769  `, `POJ`, `Tongi
-000012f0: 6f6e 6760 0d0d 0a2a 2060 2727 6020 2d20  ong`...* `''` - 
-00001300: 666f 7220 6050 696e 6779 696d 600d 0d0a  for `Pingyim`...
-00001310: 2a20 6027 2027 6020 2d20 666f 7220 605a  * `' '` - for `Z
-00001320: 6875 7969 6e60 2c20 6054 4c50 4160 0d0d  huyin`, `TLPA`..
-00001330: 0a0d 0d0a 7c20 7465 7874 207c 2027 2d27  ....| text | '-'
-00001340: 2020 2020 207c 2027 2720 2020 2020 7c20       | ''     | 
-00001350: 2720 2720 2020 2020 7c0d 0d0a 7c2d 2d2d  ' '     |...|---
-00001360: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  ---|---------|--
-00001370: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00001380: 7c0d 0d0a 7c20 e887 bae7 81a3 207c 2054  |...| ...... | T
-00001390: c3a2 692d 75c3 a26e 207c 2054 c3a2 6975  ..i-u..n | T..iu
-000013a0: c3a2 6e20 7c20 54c3 a269 2075 c3a2 6e20  ..n | T..i u..n 
-000013b0: 7c0d 0d0a 0d0d 0a23 2323 2320 5361 6e64  |......#### Sand
-000013c0: 6869 0d0d 0a0d 0d0a 6073 616e 6468 6960  hi......`sandhi`
-000013d0: 2042 6f6f 6c65 616e 202d 2061 7070 6c69   Boolean - appli
-000013e0: 6573 2074 6865 205b 7361 6e64 6869 2072  es the [sandhi r
-000013f0: 756c 6573 206f 6620 5461 6977 616e 6573  ules of Taiwanes
-00001400: 6520 486f 6b6b 6965 6e5d 5b73 616e 6468  e Hokkien][sandh
-00001410: 692d 7769 6b69 5d20 746f 2073 796c 6c61  i-wiki] to sylla
-00001420: 626c 6573 206f 6620 6120 7369 6e67 6c65  bles of a single
-00001430: 2077 6f72 642e 0d0d 0a0d 0d0a 4465 6661   word.......Defa
-00001440: 756c 7420 7661 6c75 6520 6465 7065 6e64  ult value depend
-00001450: 7320 6f6e 2074 6865 2063 686f 7365 6e20  s on the chosen 
-00001460: 6073 7973 7465 6d60 3a0d 0d0a 0d0d 0a2a  `system`:......*
-00001470: 2060 5472 7565 6020 2d20 666f 7220 6054   `True` - for `T
-00001480: 6f6e 6769 6f6e 6760 0d0d 0a2a 2060 4661  ongiong`...* `Fa
-00001490: 6c73 6560 202d 2066 6f72 2060 5461 696c  lse` - for `Tail
-000014a0: 6f60 2c20 6050 4f4a 602c 2060 5a68 7579  o`, `POJ`, `Zhuy
-000014b0: 696e 602c 2060 544c 5041 602c 2060 5069  in`, `TLPA`, `Pi
-000014c0: 6e67 7969 6d60 0d0d 0a0d 0d0a 7c20 7465  ngyim`......| te
-000014d0: 7874 2020 2020 207c 2046 616c 7365 2020  xt     | False  
-000014e0: 2020 2020 2020 7c20 5472 7565 2020 2020        | True    
-000014f0: 2020 2020 207c 0d0d 0a7c 2d2d 2d2d 2d2d       |...|------
-00001500: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-00001510: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00001520: 2d2d 7c0d 0d0a 7c20 e9a6 ace4 be86 e8a5  --|...| ........
-00001530: bfe4 ba9e 207c 204d c3a1 2d6c c3a2 692d  .... | M..-l..i-
-00001540: 7365 2d61 2020 7c20 4d61 2d6c c481 692d  se-a  | Ma-l..i-
-00001550: 73c4 932d 6120 207c 0d0d 0a0d 0d0a 5361  s..-a  |......Sa
-00001560: 6e64 6869 2072 756c 6573 2061 6c73 6f20  ndhi rules also 
-00001570: 6368 616e 6765 2064 6570 656e 6469 6e67  change depending
-00001580: 206f 6e20 7468 6520 6469 616c 6563 7420   on the dialect 
-00001590: 6368 6f73 656e 2e0d 0d0a 0d0d 0a7c 2074  chosen.......| t
-000015a0: 6578 7420 7c20 6e6f 2073 616e 6468 6920  ext | no sandhi 
-000015b0: 7c20 736f 7574 6820 2020 7c20 6e6f 7274  | south   | nort
-000015c0: 6820 2020 7c0d 0d0a 7c2d 2d2d 2d2d 2d7c  h   |...|------|
-000015d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-000015e0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d7c  -----|---------|
-000015f0: 0d0d 0a7c 20e8 87ba e781 a320 7c20 54c3  ...| ...... | T.
-00001600: a269 2d75 c3a2 6e20 2020 7c20 54c4 8169  .i-u..n   | T..i
-00001610: 2d75 c3a2 6e20 7c20 54c3 a069 2d75 c3a2  -u..n | T..i-u..
-00001620: 6e20 7c0d 0d0a 0d0d 0a4e 6f74 6520 7468  n |......Note th
-00001630: 6174 2074 6865 2066 756e 6374 696f 6e20  at the function 
-00001640: 6973 2064 6966 6665 7265 6e74 2066 726f  is different fro
-00001650: 6d20 7265 616c 2073 616e 6468 6920 7275  m real sandhi ru
-00001660: 6c65 732c 2077 6865 7265 2063 6861 6e67  les, where chang
-00001670: 6573 2061 7265 2061 7070 6c69 6564 2074  es are applied t
-00001680: 6f20 6576 6572 7920 7369 6e67 6c65 2073  o every single s
-00001690: 796c 6c61 626c 6520 6f66 2074 6865 2073  yllable of the s
-000016a0: 656e 7465 6e63 652c 206e 6f74 206a 7573  entence, not jus
-000016b0: 7420 7369 6e67 6c65 2077 6f72 6473 2e0d  t single words..
-000016c0: 0d0a 0d0d 0a2d 202a 2a54 6169 6275 6e27  .....- **Taibun'
-000016d0: 7320 7361 6e64 6869 2072 756c 6573 2a2a  s sandhi rules**
-000016e0: 3a20 5468 c3a1 692d 6b68 6f6e 6720 70c4  : Th..i-khong p.
-000016f0: ab6e 672d 69c3 ba2c 206c 696e 2d68 c3b3  .ng-i.., lin-h..
-00001700: 2120 4cc3 ad6e 2074 7369 c3a0 2d70 c3a1  ! L..n tsi..-p..
-00001710: 2062 75c4 933f 0d0d 0a2d 202a 2a41 6374   bu..?...- **Act
-00001720: 7561 6c20 7361 6e64 6869 2072 756c 6573  ual sandhi rules
-00001730: 2a2a 3a20 5468 c3a1 692d 6b68 c58d 6e67  **: Th..i-kh..ng
-00001740: 2070 c4ab 6e67 2d69 c3ba 2c20 6c69 6e2d   p..ng-i.., lin-
-00001750: 68c3 b321 204c 696e 2074 7369 c3a0 2d70  h..! Lin tsi..-p
-00001760: 6120 6275 c493 3f0d 0d0a 0d0d 0a23 2323  a bu..?......###
-00001770: 2320 5075 6e63 7475 6174 696f 6e0d 0d0a  # Punctuation...
-00001780: 0d0d 0a60 7075 6e63 7475 6174 696f 6e60  ...`punctuation`
-00001790: 2053 7472 696e 670d 0d0a 0d0d 0a2a 2060   String......* `
-000017a0: 666f 726d 6174 6020 2864 6566 6175 6c74  format` (default
-000017b0: 2920 2d20 636f 6e76 6572 7473 2043 6869  ) - converts Chi
-000017c0: 6e65 7365 2d73 7479 6c65 2070 756e 6374  nese-style punct
-000017d0: 7561 7469 6f6e 2074 6f20 4c61 7469 6e2d  uation to Latin-
-000017e0: 7374 796c 6520 7075 6e63 7475 6174 696f  style punctuatio
-000017f0: 6e20 616e 6420 6361 7069 7461 6c69 7365  n and capitalise
-00001800: 7320 776f 7264 7320 6174 2074 6865 2062  s words at the b
-00001810: 6567 696e 6e69 6e67 206f 6620 6561 6368  eginning of each
-00001820: 2073 656e 7465 6e63 652e 0d0d 0a2a 2060   sentence....* `
-00001830: 6e6f 6e65 6020 2d20 7072 6573 6572 7665  none` - preserve
-00001840: 7320 4368 696e 6573 652d 7374 796c 6520  s Chinese-style 
-00001850: 7075 6e63 7475 6174 696f 6e20 616e 6420  punctuation and 
-00001860: 646f 6573 6e27 7420 6361 7069 7461 6c69  doesn't capitali
-00001870: 7365 2077 6f72 6473 2061 7420 7468 6520  se words at the 
-00001880: 6265 6769 6e6e 696e 6720 6f66 206e 6577  beginning of new
-00001890: 2073 656e 7465 6e63 6573 2e0d 0d0a 0d0d   sentences......
-000018a0: 0a7c 2074 6578 7420 7c20 666f 726d 6174  .| text | format
-000018b0: 207c 206e 6f6e 6520 7c0d 0d0a 7c2d 7c2d   | none |...|-|-
-000018c0: 7c2d 7c0d 0d0a 7c20 e980 99e6 98af e887  |-|...| ........
-000018d0: bae5 8d97 efbc 8ce7 b0a1 e7a8 b1e3 808c  ................
-000018e0: e58d 97e3 808d efbc 88e7 99bd e8a9 b1e5  ................
-000018f0: ad97 efbc 9a54 c3a2 692d 6cc3 a26d efbc  .....T..i-l..m..
-00001900: 9be6 b3a8 e99f b3e7 aca6 e899 9fef bc9a  ................
-00001910: e384 8ae3 849e cb8a 20e3 848b e384 a2cb  ........ .......
-00001920: 8aef bc8c e59c 8be8 aa9e efbc 9a54 c3a1  .............T..
-00001930: 696e c3a1 6eef bc89 e380 8220 7c20 5473  in..n...... | Ts
-00001940: 6520 73c4 ab20 54c3 a269 2d6c c3a2 6d2c  e s.. T..i-l..m,
-00001950: 206b c3a1 6e2d 7473 6869 6e67 2022 6cc3   k..n-tshing "l.
-00001960: a26d 2220 2850 65cc 8d68 2d75 c493 2d6a  .m" (Pe..h-u..-j
-00001970: c4ab 3a20 54c3 a269 2d6c c3a2 6d3b 2074  ..: T..i-l..m; t
-00001980: 73c3 b92d 696d 2068 c3bb 2d68 c58d 3a20  s..-im h..-h..: 
-00001990: e384 8ae3 849e cb8a 20e3 848b e384 a2cb  ........ .......
-000019a0: 8a2c 206b 6f6b 2d67 c3ad 3a20 54c3 a169  ., kok-g..: T..i
-000019b0: 6ec3 a16e 292e 207c 2074 7365 2073 c4ab  n..n). | tse s..
-000019c0: 2054 c3a2 692d 6cc3 a26d efbc 8c6b c3a1   T..i-l..m...k..
-000019d0: 6e2d 7473 6869 6e67 e380 8c6c c3a2 6de3  n-tshing...l..m.
-000019e0: 808d efbc 8850 65cc 8d68 2d75 c493 2d6a  .....Pe..h-u..-j
-000019f0: c4ab efbc 9a54 c3a2 692d 6cc3 a26d efbc  .....T..i-l..m..
-00001a00: 9b74 73c3 b92d 696d 2068 c3bb 2d68 c58d  .ts..-im h..-h..
-00001a10: efbc 9ae3 848a e384 9ecb 8a20 e384 8be3  ........... ....
-00001a20: 84a2 cb8a efbc 8c6b 6f6b 2d67 c3ad efbc  .......kok-g....
-00001a30: 9a54 c3a1 696e c3a1 6eef bc89 e380 8220  .T..in..n...... 
-00001a40: 7c0d 0d0a 0d0d 0a23 2323 2054 6f6b 656e  |......### Token
-00001a50: 6973 6572 0d0d 0a0d 0d0a 6054 6f6b 656e  iser......`Token
-00001a60: 6973 6572 6020 636c 6173 7320 7065 7266  iser` class perf
-00001a70: 6f72 6d73 205b 4e4c 544b 2077 6f72 6470  orms [NLTK wordp
-00001a80: 756e 6374 5f74 6f6b 656e 697a 655d 5b6e  unct_tokenize][n
-00001a90: 6c74 6b2d 746f 6b65 6e69 7a65 5d2d 6c69  ltk-tokenize]-li
-00001aa0: 6b65 2074 6f6b 656e 6973 6174 696f 6e20  ke tokenisation 
-00001ab0: 6f66 2061 2054 6169 7761 6e65 7365 2048  of a Taiwanese H
-00001ac0: 6f6b 6b69 656e 2073 656e 7465 6e63 652e  okkien sentence.
-00001ad0: 0d0d 0a0d 0d0a 6060 6070 7974 686f 6e0d  ......```python.
-00001ae0: 0d0a 2320 636f 6e73 7472 7563 746f 720d  ..# constructor.
-00001af0: 0d0a 7420 3d20 546f 6b65 6e69 7365 7228  ..t = Tokeniser(
-00001b00: 290d 0d0a 0d0d 0a23 2074 6f6b 656e 6973  )......# tokenis
-00001b10: 6520 5461 6977 616e 6573 6520 486f 6b6b  e Taiwanese Hokk
-00001b20: 6965 6e20 7365 6e74 656e 6365 0d0d 0a74  ien sentence...t
-00001b30: 2e74 6f6b 656e 6973 6528 696e 7075 7429  .tokenise(input)
-00001b40: 0d0d 0a60 6060 0d0d 0a0d 0d0a 0d0d 0a0d  ...```..........
-00001b50: 0d0a 3c21 2d2d 2045 5841 4d50 4c45 202d  ..<!-- EXAMPLE -
-00001b60: 2d3e 0d0d 0a23 2320 4578 616d 706c 650d  ->...## Example.
-00001b70: 0d0a 0d0d 0a60 6060 7079 7468 6f6e 0d0d  .....```python..
-00001b80: 0a66 726f 6d20 7461 6962 756e 2069 6d70  .from taibun imp
-00001b90: 6f72 7420 436f 6e76 6572 7465 722c 2054  ort Converter, T
-00001ba0: 6f6b 656e 6973 6572 0d0d 0a0d 0d0a 2320  okeniser......# 
-00001bb0: 5379 7374 656d 0d0d 0a63 203d 2043 6f6e  System...c = Con
-00001bc0: 7665 7274 6572 2829 2023 2054 6169 6c6f  verter() # Tailo
-00001bd0: 2073 7973 7465 6d20 6465 6661 756c 740d   system default.
-00001be0: 0d0a 632e 6765 7428 27e5 8588 e794 9fe8  ..c.get('.......
-00001bf0: ac9b efbc 8ce5 adb8 e794 9fe6 81ac e681  ................
-00001c00: ace8 81bd e380 8227 290d 0d0a 3e3e 2053  .......')...>> S
-00001c10: 6961 6e2d 7369 6e6e 206b c3b3 6e67 2c20  ian-sinn k..ng, 
-00001c20: 6861 cc8d 6b2d 7369 6e67 2074 69c4 816d  ha..k-sing ti..m
-00001c30: 2d74 69c4 816d 2074 6869 616e 6e2e 0d0d  -ti..m thiann...
-00001c40: 0a0d 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00001c50: 7228 7379 7374 656d 3d27 5a68 7579 696e  r(system='Zhuyin
-00001c60: 2729 0d0d 0a63 2e67 6574 2827 e585 88e7  ')...c.get('....
-00001c70: 949f e8ac 9bef bc8c e5ad b8e7 949f e681  ................
-00001c80: ace6 81ac e881 bde3 8082 2729 0d0d 0a3e  ..........')...>
-00001c90: 3e20 e384 92e3 84a7 e384 a220 e384 92e3  > ......... ....
-00001ca0: 86aa 20e3 848d e386 b2cb 8b2c 20e3 848f  .. ........, ...
-00001cb0: e384 9ae3 86b6 cb99 20e3 8492 e384 a7e3  ........ .......
-00001cc0: 84a5 20e3 8489 e384 a7e3 86b0 cbab 20e3  .. ........... .
-00001cd0: 8489 e384 a7e3 86b0 cbab 20e3 848a e384  .......... .....
-00001ce0: a7e3 86a9 2e0d 0d0a 0d0d 0a23 2044 6961  ...........# Dia
-00001cf0: 6c65 6374 0d0d 0a63 203d 2043 6f6e 7665  lect...c = Conve
-00001d00: 7274 6572 2829 2023 2073 6f75 7468 2064  rter() # south d
-00001d10: 6961 6c65 6374 2064 6566 6175 6c74 0d0d  ialect default..
-00001d20: 0a63 2e67 6574 2822 e688 91e6 acb2 e794  .c.get("........
-00001d30: a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0d 0a3e  ..........")...>
-00001d40: 3e20 4775 c3a1 2062 6568 20c4 ab6e 6720  > Gu.. beh ..ng 
-00001d50: 74c4 ab20 7473 6961 cc8d 6820 68c3 ae0d  t.. tsia..h h...
-00001d60: 0d0a 0d0d 0a63 203d 2043 6f6e 7665 7274  .....c = Convert
-00001d70: 6572 2864 6961 6c65 6374 3d27 6e6f 7274  er(dialect='nort
-00001d80: 6827 290d 0d0a 632e 6765 7428 22e6 8891  h')...c.get("...
-00001d90: e6ac b2e7 94a8 e7ae b8e9 a39f e9ad 9a22  ..............."
-00001da0: 290d 0d0a 3e3e 2047 75c3 a120 6275 6568  )...>> Gu.. bueh
-00001db0: 20c4 ab6e 6720 74c5 ab20 7473 6961 cc8d   ..ng t.. tsia..
-00001dc0: 6820 68c3 bb0d 0d0a 0d0d 0a23 2046 6f72  h h........# For
-00001dd0: 6d61 740d 0d0a 6320 3d20 436f 6e76 6572  mat...c = Conver
-00001de0: 7465 7228 2920 2320 666f 7220 5461 696c  ter() # for Tail
-00001df0: 6f2c 206d 6172 6b20 6279 2064 6566 6175  o, mark by defau
-00001e00: 6c74 0d0d 0a63 2e67 6574 2822 e794 9fe6  lt...c.get("....
-00001e10: 97a5 e5bf abe6 a882 2229 0d0d 0a3e 3e20  ........")...>> 
-00001e20: 5365 6e6e 2d6a 69cc 8d74 206b 6875 c3a0  Senn-ji..t khu..
-00001e30: 692d 6c6f cc8d 6b0d 0d0a 0d0d 0a63 203d  i-lo..k......c =
-00001e40: 2043 6f6e 7665 7274 6572 2866 6f72 6d61   Converter(forma
-00001e50: 743d 276e 756d 6265 7227 290d 0d0a 632e  t='number')...c.
-00001e60: 6765 7428 22e7 949f e697 a5e5 bfab e6a8  get("...........
-00001e70: 8222 290d 0d0a 3e3e 2053 656e 6e31 2d6a  .")...>> Senn1-j
-00001e80: 6974 3820 6b68 7561 6933 2d6c 6f6b 380d  it8 khuai3-lok8.
-00001e90: 0d0a 0d0d 0a63 203d 2043 6f6e 7665 7274  .....c = Convert
-00001ea0: 6572 2866 6f72 6d61 743d 2773 7472 6970  er(format='strip
-00001eb0: 2729 0d0d 0a63 2e67 6574 2822 e794 9fe6  ')...c.get("....
-00001ec0: 97a5 e5bf abe6 a882 2229 0d0d 0a3e 3e20  ........")...>> 
-00001ed0: 5365 6e6e 2d6a 6974 206b 6875 6169 2d6c  Senn-jit khuai-l
-00001ee0: 6f6b 0d0d 0a0d 0d0a 2320 4465 6c69 6d69  ok......# Delimi
-00001ef0: 7465 720d 0d0a 6320 3d20 436f 6e76 6572  ter...c = Conver
-00001f00: 7465 7228 6465 6c69 6d69 7465 723d 2727  ter(delimiter=''
-00001f10: 290d 0d0a 632e 6765 7428 22e5 8588 e794  )...c.get(".....
-00001f20: 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6 81ac  ................
-00001f30: e681 ace8 81bd e380 8222 290d 0d0a 3e3e  .........")...>>
-00001f40: 2053 6961 6e73 696e 6e20 6bc3 b36e 672c   Siansinn k..ng,
-00001f50: 2068 61cc 8d6b 7369 6e67 2074 69c4 816d   ha..ksing ti..m
-00001f60: 7469 c481 6d20 7468 6961 6e6e 2e0d 0d0a  ti..m thiann....
-00001f70: 0d0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
-00001f80: 2873 7973 7465 6d3d 2750 696e 6779 696d  (system='Pingyim
-00001f90: 272c 2064 656c 696d 6974 6572 3d27 2d27  ', delimiter='-'
-00001fa0: 290d 0d0a 632e 6765 7428 22e5 8588 e794  )...c.get(".....
-00001fb0: 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6 81ac  ................
-00001fc0: e681 ace8 81bd e380 8222 290d 0d0a 3e3e  .........")...>>
-00001fd0: 2053 69c4 816e 2d73 6ec4 ab20 67c7 926e   Si..n-sn.. g..n
-00001fe0: 672c 2068 c3a1 672d 73c4 ab6e 6720 6469  g, h..g-s..ng di
-00001ff0: c3a2 6d2d 6469 c3a2 6d20 7469 6ec4 812e  ..m-di..m tin...
-00002000: 0d0d 0a0d 0d0a 2320 5361 6e64 6869 0d0d  ......# Sandhi..
-00002010: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
-00002020: 2023 2066 6f72 2054 6169 6c6f 2c20 7361   # for Tailo, sa
-00002030: 6e64 6869 2046 616c 7365 2062 7920 6465  ndhi False by de
-00002040: 6661 756c 740d 0d0a 632e 6765 7428 22e5  fault...c.get(".
-00002050: 8d97 e8bf b4e9 90b5 e8b7 af22 290d 0d0a  ...........")...
-00002060: 3e3e 204c c3a2 6d2d 6875 c3aa 2d74 6869  >> L..m-hu..-thi
-00002070: 682d 6cc5 8d6f 0d0d 0a0d 0d0a 6320 3d20  h-l..o......c = 
-00002080: 436f 6e76 6572 7465 7228 7361 6e64 6869  Converter(sandhi
-00002090: 3d54 7275 6529 0d0d 0a63 2e67 6574 2822  =True)...c.get("
-000020a0: e58d 97e8 bfb4 e990 b5e8 b7af 2229 0d0d  ............")..
-000020b0: 0a3e 3e20 4cc4 816d 2d68 75c4 932d 7468  .>> L..m-hu..-th
-000020c0: c3ad 2d6c c58d 6f0d 0d0a 0d0d 0a23 2050  ..-l..o......# P
-000020d0: 756e 6374 7561 7469 6f6e 0d0d 0a63 203d  unctuation...c =
-000020e0: 2043 6f6e 7665 7274 6572 2829 2023 2066   Converter() # f
-000020f0: 6f72 6d61 7420 7075 6e63 7475 6174 696f  ormat punctuatio
-00002100: 6e20 6465 6661 756c 740d 0d0a 632e 6765  n default...c.ge
-00002110: 7428 22e5 a4aa e7a9 bae6 9c8b e58f 8bef  t(".............
-00002120: bc8c e681 81e5 a5bd efbc 81e6 8181 e9a3  ................
-00002130: 9fe9 a3bd e69c aaef bc9f 2229 0d0d 0a3e  ..........")...>
-00002140: 3e20 5468 c3a0 692d 6b68 6f6e 6720 70c3  > Th..i-khong p.
-00002150: ae6e 672d 69c3 ba2c 206c c3ad 6e2d 68c3  .ng-i.., l..n-h.
-00002160: b321 204c c3ad 6e20 7473 6961 cc8d 682d  .! L..n tsia..h-
-00002170: 70c3 a120 6275 c493 3f0d 0d0a 0d0d 0a63  p.. bu..?......c
-00002180: 203d 2043 6f6e 7665 7274 6572 2870 756e   = Converter(pun
-00002190: 6374 7561 7469 6f6e 3d27 6e6f 6e65 2729  ctuation='none')
-000021a0: 0d0d 0a63 2e67 6574 2822 e5a4 aae7 a9ba  ...c.get("......
-000021b0: e69c 8be5 8f8b efbc 8ce6 8181 e5a5 bdef  ................
-000021c0: bc81 e681 81e9 a39f e9a3 bde6 9caa efbc  ................
-000021d0: 9f22 290d 0d0a 3e3e 2074 68c3 a069 2d6b  .")...>> th..i-k
-000021e0: 686f 6e67 2070 c3ae 6e67 2d69 c3ba efbc  hong p..ng-i....
-000021f0: 8c6c c3ad 6e2d 68c3 b3ef bc81 6cc3 ad6e  .l..n-h.....l..n
-00002200: 2074 7369 61cc 8d68 2d70 c3a1 2062 75c4   tsia..h-p.. bu.
-00002210: 93ef bc9f 0d0d 0a0d 0d0a 0d0d 0a23 2054  .............# T
-00002220: 6f6b 656e 6973 6572 0d0d 0a74 203d 2054  okeniser...t = T
-00002230: 6f6b 656e 6973 6572 2829 0d0d 0a74 2e74  okeniser()...t.t
-00002240: 6f6b 656e 6973 6528 22e5 a4aa e7a9 bae6  okenise(".......
-00002250: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
-00002260: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
-00002270: 2229 0d0d 0a3e 3e20 5b27 e5a4 aae7 a9ba  ")...>> ['......
-00002280: 272c 2027 e69c 8be5 8f8b 272c 2027 efbc  ', '......', '..
-00002290: 8c27 2c20 27e6 8181 e5a5 bd27 2c20 27ef  .', '......', '.
-000022a0: bc81 272c 2027 e681 8127 2c20 27e9 a39f  ..', '...', '...
-000022b0: e9a3 bd27 2c20 27e6 9caa 272c 2027 efbc  ...', '...', '..
-000022c0: 9f27 5d0d 0d0a 6060 600d 0d0a 0d0d 0a0d  .']...```.......
-000022d0: 0d0a 0d0d 0a3c 212d 2d20 4441 5441 202d  .....<!-- DATA -
-000022e0: 2d3e 0d0d 0a23 2320 4461 7461 0d0d 0a0d  ->...## Data....
-000022f0: 0d0a 2d20 5b54 6169 7761 6e65 7365 2d43  ..- [Taiwanese-C
-00002300: 6869 6e65 7365 204f 6e6c 696e 6520 4469  hinese Online Di
-00002310: 6374 696f 6e61 7279 5d5b 6f6e 6c69 6e65  ctionary][online
-00002320: 2d64 6963 7469 6f6e 6172 795d 2028 7669  -dictionary] (vi
-00002330: 6120 5b43 6868 6f65 5461 6967 695d 5b64  a [ChhoeTaigi][d
-00002340: 6174 612d 7669 615d 290d 0d0a 2d20 5b69  ata-via])...- [i
-00002350: 5461 6967 6920 4368 696e 6573 652d 5461  Taigi Chinese-Ta
-00002360: 6977 616e 6573 6520 436f 6d70 6172 6973  iwanese Comparis
-00002370: 6f6e 2044 6963 7469 6f6e 6172 795d 5b69  on Dictionary][i
-00002380: 7461 6967 692d 6469 6374 696f 6e61 7279  taigi-dictionary
-00002390: 5d20 2876 6961 205b 4368 686f 6554 6169  ] (via [ChhoeTai
-000023a0: 6769 5d5b 6461 7461 2d76 6961 5d29 0d0d  gi][data-via])..
-000023b0: 0a0d 0d0a 0d0d 0a0d 0d0a 3c21 2d2d 2041  ..........<!-- A
-000023c0: 434b 4e4f 574c 4544 4745 4d45 4e54 5320  CKNOWLEDGEMENTS 
-000023d0: 2d2d 3e0d 0d0a 2323 2041 636b 6e6f 776c  -->...## Acknowl
-000023e0: 6564 6765 6d65 6e74 730d 0d0a 0d0d 0a2d  edgements......-
-000023f0: 2053 616d 7565 6c20 4a65 6e20 285b 4769   Samuel Jen ([Gi
-00002400: 7468 7562 5d5b 7361 6d75 656c 2d67 6974  thub][samuel-git
-00002410: 6875 625d 20c2 b720 5b4c 696e 6b65 6449  hub] .. [LinkedI
-00002420: 6e5d 5b73 616d 7565 6c2d 6c69 6e6b 6564  n][samuel-linked
-00002430: 696e 5d29 202d 2054 6169 7761 6e65 7365  in]) - Taiwanese
-00002440: 2061 6e64 204d 616e 6461 7269 6e20 7472   and Mandarin tr
-00002450: 616e 736c 6174 696f 6e0d 0d0a 0d0d 0a0d  anslation.......
-00002460: 0d0a 0d0d 0a3c 212d 2d20 4c49 4345 4e43  .....<!-- LICENC
-00002470: 4520 2d2d 3e0d 0d0a 2323 204c 6963 656e  E -->...## Licen
-00002480: 6365 0d0d 0a0d 0d0a 4265 6361 7573 6520  ce......Because 
-00002490: 5461 6962 756e 2069 7320 4d49 542d 6c69  Taibun is MIT-li
-000024a0: 6365 6e73 6564 2c20 616e 7920 6465 7665  censed, any deve
-000024b0: 6c6f 7065 7220 6361 6e20 6573 7365 6e74  loper can essent
-000024c0: 6961 6c6c 7920 646f 2077 6861 7465 7665  ially do whateve
-000024d0: 7220 7468 6579 2077 616e 7420 7769 7468  r they want with
-000024e0: 2069 7420 6173 206c 6f6e 6720 6173 2074   it as long as t
-000024f0: 6865 7920 696e 636c 7564 6520 7468 6520  hey include the 
-00002500: 6f72 6967 696e 616c 2063 6f70 7972 6967  original copyrig
-00002510: 6874 2061 6e64 206c 6963 656e 6365 206e  ht and licence n
-00002520: 6f74 6963 6520 696e 2061 6e79 2063 6f70  otice in any cop
-00002530: 6965 7320 6f66 2074 6865 2073 6f75 7263  ies of the sourc
-00002540: 6520 636f 6465 2e20 4e6f 7465 2c20 7468  e code. Note, th
-00002550: 6174 2074 6865 2064 6174 6120 7573 6564  at the data used
-00002560: 2062 7920 7468 6520 7061 636b 6167 6520   by the package 
-00002570: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
-00002580: 7220 6120 6469 6666 6572 656e 7420 636f  r a different co
-00002590: 7079 7269 6768 742e 0d0d 0a0d 0d0a 5468  pyright.......Th
-000025a0: 6520 6461 7461 2069 7320 6c69 6365 6e73  e data is licens
-000025b0: 6564 2075 6e64 6572 205b 4343 2042 592d  ed under [CC BY-
-000025c0: 5341 2034 2e30 5d5b 6461 7461 2d63 635d  SA 4.0][data-cc]
-000025d0: 0d0d 0a0d 0d0a 0d0d 0a0d 0d0a 3c21 2d2d  ............<!--
-000025e0: 204d 4152 4b44 4f57 4e20 4c49 4e4b 5320   MARKDOWN LINKS 
-000025f0: 2d2d 3e0d 0d0a 5b74 6573 7473 5d3a 2068  -->...[tests]: h
-00002600: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002610: 6d2f 616e 6472 6569 6861 722f 7461 6962  m/andreihar/taib
-00002620: 756e 2f61 6374 696f 6e73 0d0d 0a5b 7465  un/actions...[te
-00002630: 7374 732d 6261 6467 655d 3a20 6874 7470  sts-badge]: http
-00002640: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00002650: 696f 2f67 6974 6875 622f 6163 7469 6f6e  io/github/action
-00002660: 732f 776f 726b 666c 6f77 2f73 7461 7475  s/workflow/statu
-00002670: 732f 616e 6472 6569 6861 722f 7461 6962  s/andreihar/taib
-00002680: 756e 2f63 692e 7961 6d6c 3f73 7479 6c65  un/ci.yaml?style
-00002690: 3d66 6f72 2d74 6865 2d62 6164 6765 0d0d  =for-the-badge..
-000026a0: 0a5b 636f 6e74 7269 6275 746f 7273 2d62  .[contributors-b
-000026b0: 6164 6765 5d3a 2068 7474 7073 3a2f 2f69  adge]: https://i
-000026c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-000026d0: 7468 7562 2f63 6f6e 7472 6962 7574 6f72  thub/contributor
-000026e0: 732f 616e 6472 6569 6861 722f 7461 6962  s/andreihar/taib
-000026f0: 756e 3f73 7479 6c65 3d66 6f72 2d74 6865  un?style=for-the
-00002700: 2d62 6164 6765 0d0d 0a5b 636f 6e74 7269  -badge...[contri
-00002710: 6275 746f 7273 5d3a 2023 7573 6167 650d  butors]: #usage.
-00002720: 0d0a 5b72 656c 6561 7365 2d62 6164 6765  ..[release-badge
-00002730: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00002740: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00002750: 2f76 2f72 656c 6561 7365 2f61 6e64 7265  /v/release/andre
-00002760: 6968 6172 2f74 6169 6275 6e3f 636f 6c6f  ihar/taibun?colo
-00002770: 723d 3338 3631 3863 2673 7479 6c65 3d66  r=38618c&style=f
-00002780: 6f72 2d74 6865 2d62 6164 6765 0d0d 0a5b  or-the-badge...[
-00002790: 7265 6c65 6173 655d 3a20 6874 7470 733a  release]: https:
-000027a0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6e64  //github.com/and
-000027b0: 7265 6968 6172 2f74 6169 6275 6e2f 7265  reihar/taibun/re
-000027c0: 6c65 6173 6573 0d0d 0a5b 6c69 6365 6e63  leases...[licenc
-000027d0: 652d 6261 6467 655d 3a20 6874 7470 733a  e-badge]: https:
-000027e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000027f0: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
-00002800: 616e 6472 6569 6861 722f 7461 6962 756e  andreihar/taibun
-00002810: 3f63 6f6c 6f72 3d30 3030 3030 3026 7374  ?color=000000&st
-00002820: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
-00002830: 650d 0d0a 5b6c 6963 656e 6365 5d3a 204c  e...[licence]: L
-00002840: 4943 454e 5345 0d0d 0a5b 6c69 6e6b 6564  ICENSE...[linked
-00002850: 696e 2d62 6164 6765 5d3a 2068 7474 7073  in-badge]: https
-00002860: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00002870: 6f2f 6261 6467 652f 4c69 6e6b 6564 496e  o/badge/LinkedIn
-00002880: 2d30 3037 3742 353f 7374 796c 653d 666f  -0077B5?style=fo
-00002890: 722d 7468 652d 6261 6467 6526 6c6f 676f  r-the-badge&logo
-000028a0: 3d6c 696e 6b65 6469 6e26 6c6f 676f 436f  =linkedin&logoCo
-000028b0: 6c6f 723d 7768 6974 650d 0d0a 5b6c 696e  lor=white...[lin
-000028c0: 6b65 6469 6e5d 3a20 6874 7470 733a 2f2f  kedin]: https://
-000028d0: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
-000028e0: 2f69 6e2f 616e 6472 6569 2d68 6172 6261  /in/andrei-harba
-000028f0: 6368 6f76 2f0d 0d0a 0d0d 0a5b 7079 7069  chov/......[pypi
-00002900: 5d3a 2068 7474 7073 3a2f 2f70 7970 692e  ]: https://pypi.
-00002910: 6f72 672f 7072 6f6a 6563 742f 7461 6962  org/project/taib
-00002920: 756e 0d0d 0a5b 6275 675d 3a20 6874 7470  un...[bug]: http
-00002930: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00002940: 6e64 7265 6968 6172 2f74 6169 6275 6e2f  ndreihar/taibun/
-00002950: 6973 7375 6573 0d0d 0a5b 6f6e 6c69 6e65  issues...[online
-00002960: 2d64 6963 7469 6f6e 6172 795d 3a20 6874  -dictionary]: ht
-00002970: 7470 3a2f 2f69 7031 3934 3039 372e 6e74  tp://ip194097.nt
-00002980: 6375 2e65 6475 2e74 772f 756e 6769 616e  cu.edu.tw/ungian
-00002990: 2f73 6f61 6e6e 7465 6e67 2f63 6869 6c2f  /soannteng/chil/
-000029a0: 5461 6968 6f61 2e61 7370 0d0d 0a5b 6974  Taihoa.asp...[it
-000029b0: 6169 6769 2d64 6963 7469 6f6e 6172 795d  aigi-dictionary]
-000029c0: 3a20 6874 7470 733a 2f2f 6974 6169 6769  : https://itaigi
-000029d0: 2e74 772f 0d0d 0a5b 6461 7461 2d76 6961  .tw/...[data-via
-000029e0: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-000029f0: 622e 636f 6d2f 4368 686f 6554 6169 6769  b.com/ChhoeTaigi
-00002a00: 2f43 6868 6f65 5461 6967 6944 6174 6162  /ChhoeTaigiDatab
-00002a10: 6173 650d 0d0a 5b64 6174 612d 6363 5d3a  ase...[data-cc]:
-00002a20: 2068 7474 7073 3a2f 2f63 7265 6174 6976   https://creativ
-00002a30: 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963  ecommons.org/lic
-00002a40: 656e 7365 732f 6279 2d73 612f 342e 302f  enses/by-sa/4.0/
-00002a50: 6465 6564 2e65 6e0d 0d0a 5b73 616d 7565  deed.en...[samue
-00002a60: 6c2d 6769 7468 7562 5d3a 2068 7474 7073  l-github]: https
-00002a70: 3a2f 2f67 6974 6875 622e 636f 6d2f 5353  ://github.com/SS
-00002a80: 5361 6d0d 0d0a 5b73 616d 7565 6c2d 6c69  Sam...[samuel-li
-00002a90: 6e6b 6564 696e 5d3a 2068 7474 7073 3a2f  nkedin]: https:/
-00002aa0: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
-00002ab0: 6d2f 696e 2f73 616d 7565 6c2d 6a65 6e2f  m/in/samuel-jen/
-00002ac0: 0d0d 0a0d 0d0a 5b74 6169 6c6f 2d77 696b  ......[tailo-wik
-00002ad0: 695d 3a20 6874 7470 733a 2f2f 656e 2e77  i]: https://en.w
-00002ae0: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00002af0: 692f 5425 4333 2541 3269 2d75 2543 3325  i/T%C3%A2i-u%C3%
-00002b00: 4132 6e5f 4c25 4333 2542 342d 6d25 4333  A2n_L%C3%B4-m%C3
-00002b10: 2541 312d 6a25 4334 2541 425f 5068 696e  %A1-j%C4%AB_Phin
-00002b20: 672d 696d 5f48 6f6e 672d 2543 3325 4130  g-im_Hong-%C3%A0
-00002b30: 6e0d 0d0a 5b70 6f6a 2d77 696b 695d 3a20  n...[poj-wiki]: 
-00002b40: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00002b50: 6564 6961 2e6f 7267 2f77 696b 692f 5065  edia.org/wiki/Pe
-00002b60: 2543 4325 3844 682d 2543 3525 3844 652d  %CC%8Dh-%C5%8De-
-00002b70: 6a25 4334 2541 420d 0d0a 5b7a 6875 7969  j%C4%AB...[zhuyi
-00002b80: 6e2d 7769 6b69 5d3a 2068 7474 7073 3a2f  n-wiki]: https:/
-00002b90: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00002ba0: 672f 7769 6b69 2f54 6169 7761 6e65 7365  g/wiki/Taiwanese
-00002bb0: 5f50 686f 6e65 7469 635f 5379 6d62 6f6c  _Phonetic_Symbol
-00002bc0: 730d 0d0a 5b74 6c70 612d 7769 6b69 5d3a  s...[tlpa-wiki]:
-00002bd0: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
-00002be0: 7065 6469 612e 6f72 672f 7769 6b69 2f54  pedia.org/wiki/T
-00002bf0: 6169 7761 6e65 7365 5f4c 616e 6775 6167  aiwanese_Languag
-00002c00: 655f 5068 6f6e 6574 6963 5f41 6c70 6861  e_Phonetic_Alpha
-00002c10: 6265 740d 0d0a 5b70 696e 6779 696d 2d77  bet...[pingyim-w
-00002c20: 696b 695d 3a20 6874 7470 733a 2f2f 656e  iki]: https://en
-00002c30: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
-00002c40: 696b 692f 4262 2543 3325 4131 6e6c 2543  iki/Bb%C3%A1nl%C
-00002c50: 3325 4131 6d5f 7025 4333 2541 436e 6779  3%A1m_p%C3%ACngy
-00002c60: 2543 3425 4142 6d0d 0d0a 5b74 6f6e 6769  %C4%ABm...[tongi
-00002c70: 6f6e 672d 7769 6b69 5d3a 2068 7474 7073  ong-wiki]: https
-00002c80: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00002c90: 6f72 672f 7769 6b69 2f44 6125 4334 2541  org/wiki/Da%C4%A
-00002ca0: 422d 6768 2543 3325 4145 5f74 2543 3525  B-gh%C3%AE_t%C5%
-00002cb0: 3844 6e67 2d69 2543 3525 3844 6e67 5f70  8Dng-i%C5%8Dng_p
-00002cc0: 2543 3425 4142 6e67 2d69 6d0d 0d0a 5b7a  %C4%ABng-im...[z
-00002cd0: 6861 6e67 7a68 6f75 2d77 696b 695d 3a20  hangzhou-wiki]: 
-00002ce0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00002cf0: 6564 6961 2e6f 7267 2f77 696b 692f 5a68  edia.org/wiki/Zh
-00002d00: 616e 677a 686f 755f 6469 616c 6563 7473  angzhou_dialects
-00002d10: 0d0d 0a5b 7175 616e 7a68 6f75 2d77 696b  ...[quanzhou-wik
-00002d20: 695d 3a20 6874 7470 733a 2f2f 656e 2e77  i]: https://en.w
-00002d30: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00002d40: 692f 5175 616e 7a68 6f75 5f64 6961 6c65  i/Quanzhou_diale
-00002d50: 6374 730d 0d0a 5b6e 6c74 6b2d 746f 6b65  cts...[nltk-toke
-00002d60: 6e69 7a65 5d3a 2068 7474 7073 3a2f 2f6e  nize]: https://n
-00002d70: 6c74 6b2e 6f72 672f 6170 692f 6e6c 746b  ltk.org/api/nltk
-00002d80: 2e74 6f6b 656e 697a 652e 6874 6d6c 0d0d  .tokenize.html..
-00002d90: 0a5b 7361 6e64 6869 2d77 696b 695d 3a20  .[sandhi-wiki]: 
-00002da0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00002db0: 6564 6961 2e6f 7267 2f77 696b 692f 5461  edia.org/wiki/Ta
-00002dc0: 6977 616e 6573 655f 486f 6b6b 6965 6e23  iwanese_Hokkien#
-00002dd0: 546f 6e65 2532 3073 616e 6468 693a 7e3a  Tone%20sandhi:~:
-00002de0: 7465 7874 3d74 686e 6725 4532 2539 4625  text=thng%E2%9F%
-00002df0: 4139 2532 3028 2532 3273 6f75 7025 3232  A9%20(%22soup%22
-00002e00: 292e 2d2c 546f 6e65 2532 3073 616e 6468  ).-,Tone%20sandh
-00002e10: 692c 2d25 3542 6564 6974 2535 440d 0a    i,-%5Bedit%5D..
+00000000: 3c21 2d2d 2050 524f 4a45 4354 204c 4f47  <!-- PROJECT LOG
+00000010: 4f20 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c  O -->..<br />..<
+00000020: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00000030: 7222 3e0d 0a20 200d 0a23 2054 6169 6275  r">..  ..# Taibu
+00000040: 6e0d 0a0d 0a0d 0a0d 0a3c 212d 2d20 5052  n........<!-- PR
+00000050: 4f4a 4543 5420 5348 4945 4c44 5320 2d2d  OJECT SHIELDS --
+00000060: 3e0d 0a5b 215b 5465 7374 735d 5b74 6573  >..[![Tests][tes
+00000070: 7473 2d62 6164 6765 5d5d 5b74 6573 7473  ts-badge]][tests
+00000080: 5d0d 0a5b 215b 436f 6e74 7269 6275 746f  ]..[![Contributo
+00000090: 7273 5d5b 636f 6e74 7269 6275 746f 7273  rs][contributors
+000000a0: 2d62 6164 6765 5d5d 5b63 6f6e 7472 6962  -badge]][contrib
+000000b0: 7574 6f72 735d 0d0a 5b21 5b52 656c 6561  utors]..[![Relea
+000000c0: 7365 5d5b 7265 6c65 6173 652d 6261 6467  se][release-badg
+000000d0: 655d 5d5b 7265 6c65 6173 655d 0d0a 5b21  e]][release]..[!
+000000e0: 5b4c 6963 656e 6365 5d5b 6c69 6365 6e63  [Licence][licenc
+000000f0: 652d 6261 6467 655d 5d5b 6c69 6365 6e63  e-badge]][licenc
+00000100: 655d 0d0a 5b21 5b4c 696e 6b65 6449 6e5d  e]..[![LinkedIn]
+00000110: 5b6c 696e 6b65 6469 6e2d 6261 6467 655d  [linkedin-badge]
+00000120: 5d5b 6c69 6e6b 6564 696e 5d0d 0a0d 0a2a  ][linkedin]....*
+00000130: 2a54 6169 7761 6e65 7365 2048 6f6b 6b69  *Taiwanese Hokki
+00000140: 656e 2054 7261 6e73 6c69 7465 7261 746f  en Transliterato
+00000150: 7220 616e 6420 546f 6b65 6e69 7365 722a  r and Tokeniser*
+00000160: 2a0d 0a0d 0a49 7420 6861 7320 6d65 7468  *....It has meth
+00000170: 6f64 7320 7468 6174 2061 6c6c 6f77 2074  ods that allow t
+00000180: 6f20 6375 7374 6f6d 6973 6520 7472 616e  o customise tran
+00000190: 736c 6974 6572 6174 696f 6e20 616e 6420  sliteration and 
+000001a0: 7265 7472 6965 7665 2061 6e79 206e 6563  retrieve any nec
+000001b0: 6573 7361 7279 2069 6e66 6f72 6d61 7469  essary informati
+000001c0: 6f6e 2061 626f 7574 2054 6169 7761 6e65  on about Taiwane
+000001d0: 7365 2048 6f6b 6b69 656e 2070 726f 6e75  se Hokkien pronu
+000001e0: 6e63 6961 7469 6f6e 2e3c 6272 202f 3e0d  nciation.<br />.
+000001f0: 0a49 6e63 6c75 6465 7320 776f 7264 2074  .Includes word t
+00000200: 6f6b 656e 6973 6572 2066 6f72 2054 6169  okeniser for Tai
+00000210: 7761 6e65 7365 2048 6f6b 6b69 656e 2e0d  wanese Hokkien..
+00000220: 0a0d 0a5b 5265 706f 7274 2042 7567 5d5b  ...[Report Bug][
+00000230: 6275 675d 20e2 80a2 0d0a 5b50 7950 495d  bug] .....[PyPI]
+00000240: 5b70 7970 695d 0d0a 0d0a 3c2f 6469 763e  [pypi]....</div>
+00000250: 0d0a 0d0a 0d0a 0d0a 2d2d 2d0d 0a0d 0a0d  ........---.....
+00000260: 0a0d 0a3c 212d 2d20 494e 5354 414c 4c20  ...<!-- INSTALL 
+00000270: 2d2d 3e0d 0a23 2320 496e 7374 616c 6c0d  -->..## Install.
+00000280: 0a0d 0a54 6169 6275 6e20 6361 6e20 6265  ...Taibun can be
+00000290: 2069 6e73 7461 6c6c 6564 2066 726f 6d20   installed from 
+000002a0: 5b70 7970 695d 5b70 7970 695d 0d0a 0d0a  [pypi][pypi]....
+000002b0: 6060 6062 6173 680d 0a24 2070 6970 2069  ```bash..$ pip i
+000002c0: 6e73 7461 6c6c 2074 6169 6275 6e0d 0a60  nstall taibun..`
+000002d0: 6060 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2055  ``........<!-- U
+000002e0: 5341 4745 202d 2d3e 0d0a 2323 2055 7361  SAGE -->..## Usa
+000002f0: 6765 0d0a 0d0a 2323 2320 436f 6e76 6572  ge....### Conver
+00000300: 7465 720d 0a0d 0a60 436f 6e76 6572 7465  ter....`Converte
+00000310: 7260 2063 6c61 7373 2074 7261 6e73 6c69  r` class transli
+00000320: 7465 7261 7465 7320 7468 6520 4368 696e  terates the Chin
+00000330: 6573 6520 6368 6172 6163 7465 7273 2074  ese characters t
+00000340: 6f20 7468 6520 6368 6f73 656e 2074 7261  o the chosen tra
+00000350: 6e73 6c69 7465 7261 7469 6f6e 2073 7973  nsliteration sys
+00000360: 7465 6d20 7769 7468 2070 6172 616d 6574  tem with paramet
+00000370: 6572 7320 7370 6563 6966 6965 6420 6279  ers specified by
+00000380: 2074 6865 2064 6576 656c 6f70 6572 2e20   the developer. 
+00000390: 576f 726b 7320 666f 7220 626f 7468 2054  Works for both T
+000003a0: 7261 6469 7469 6f6e 616c 2061 6e64 2053  raditional and S
+000003b0: 696d 706c 6966 6965 6420 6368 6172 6163  implified charac
+000003c0: 7465 7273 2e0d 0a0d 0a60 6060 7079 7468  ters.....```pyth
+000003d0: 6f6e 0d0a 2320 636f 6e73 7472 7563 746f  on..# constructo
+000003e0: 720d 0a63 203d 2043 6f6e 7665 7274 6572  r..c = Converter
+000003f0: 2873 7973 7465 6d2c 2064 6961 6c65 6374  (system, dialect
+00000400: 2c20 666f 726d 6174 2c20 6465 6c69 6d69  , format, delimi
+00000410: 7465 722c 2073 616e 6468 692c 2070 756e  ter, sandhi, pun
+00000420: 6374 7561 7469 6f6e 2c20 636f 6e76 6572  ctuation, conver
+00000430: 745f 6e6f 6e5f 636a 6b29 0d0a 0d0a 2320  t_non_cjk)....# 
+00000440: 7472 616e 736c 6974 6572 6174 6520 4368  transliterate Ch
+00000450: 696e 6573 6520 6368 6172 6163 7465 7273  inese characters
+00000460: 0d0a 632e 6765 7428 696e 7075 7429 0d0a  ..c.get(input)..
+00000470: 6060 600d 0a0d 0a23 2323 2320 5379 7374  ```....#### Syst
+00000480: 656d 0d0a 0d0a 6073 7973 7465 6d60 2053  em....`system` S
+00000490: 7472 696e 6720 2d20 7379 7374 656d 206f  tring - system o
+000004a0: 6620 7472 616e 736c 6974 6572 6174 696f  f transliteratio
+000004b0: 6e2e 0d0a 0d0a 2a20 6054 6169 6c6f 6020  n.....* `Tailo` 
+000004c0: 2864 6566 6175 6c74 2920 2d20 5b54 c3a2  (default) - [T..
+000004d0: 692d 75c3 a26e 204c c3b4 2d6d c3a1 2d6a  i-u..n L..-m..-j
+000004e0: c4ab 2050 6869 6e67 2d69 6d20 486f 6e67  .. Phing-im Hong
+000004f0: 2dc3 a06e 5d5b 7461 696c 6f2d 7769 6b69  -..n][tailo-wiki
+00000500: 5d0d 0a2a 2060 504f 4a60 202d 205b 5065  ]..* `POJ` - [Pe
+00000510: cc8d 682d c58d 652d 6ac4 ab5d 5b70 6f6a  ..h-..e-j..][poj
+00000520: 2d77 696b 695d 0d0a 2a20 605a 6875 7969  -wiki]..* `Zhuyi
+00000530: 6e60 202d 205b 5461 6977 616e 6573 6520  n` - [Taiwanese 
+00000540: 5068 6f6e 6574 6963 2053 796d 626f 6c73  Phonetic Symbols
+00000550: 5d5b 7a68 7579 696e 2d77 696b 695d 0d0a  ][zhuyin-wiki]..
+00000560: 2a20 6054 4c50 4160 202d 205b 5461 6977  * `TLPA` - [Taiw
+00000570: 616e 6573 6520 4c61 6e67 7561 6765 2050  anese Language P
+00000580: 686f 6e65 7469 6320 416c 7068 6162 6574  honetic Alphabet
+00000590: 5d5b 746c 7061 2d77 696b 695d 0d0a 2a20  ][tlpa-wiki]..* 
+000005a0: 6050 696e 6779 696d 6020 2d20 5b42 62c3  `Pingyim` - [Bb.
+000005b0: a16e 6cc3 a16d 2055 c493 2050 c3ac 6e67  .nl..m U.. P..ng
+000005c0: 79c4 ab6d 2048 c58d 6e67 27c3 a06e 5d5b  y..m H..ng'..n][
+000005d0: 7069 6e67 7969 6d2d 7769 6b69 5d0d 0a2a  pingyim-wiki]..*
+000005e0: 2060 546f 6e67 696f 6e67 6020 2d20 5b44   `Tongiong` - [D
+000005f0: 61c4 ab2d 6768 c3ae 2054 c58d 6e67 2d69  a..-gh.. T..ng-i
+00000600: c58d 6e67 2050 c4ab 6e67 2d69 6d5d 5b74  ..ng P..ng-im][t
+00000610: 6f6e 6769 6f6e 672d 7769 6b69 5d0d 0a2a  ongiong-wiki]..*
+00000620: 2060 4950 4160 202d 205b 496e 7465 726e   `IPA` - [Intern
+00000630: 6174 696f 6e61 6c20 5068 6f6e 6574 6963  ational Phonetic
+00000640: 2041 6c70 6861 6265 745d 5b69 7061 2d77   Alphabet][ipa-w
+00000650: 696b 695d 0d0a 0d0a 7c20 7465 7874 207c  iki]....| text |
+00000660: 2054 6169 6c6f 2020 207c 2050 4f4a 2020   Tailo   | POJ  
+00000670: 2020 207c 205a 6875 7969 6e20 2020 2020     | Zhuyin     
+00000680: 207c 2054 4c50 4120 2020 2020 207c 2050   | TLPA      | P
+00000690: 696e 6779 696d 207c 2054 6f6e 6769 6f6e  ingyim | Tongion
+000006a0: 6720 7c20 4950 4120 2020 2020 2020 2020  g | IPA         
+000006b0: 7c0d 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d  |..| ---- | ----
+000006c0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20  --- | ------- | 
+000006d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+000006e0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+000006f0: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 207c 202d  - | -------- | -
+00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20  ---------- |..| 
+00000710: e58f b0e7 81a3 207c 2054 c3a2 692d 75c3  ...... | T..i-u.
+00000720: a26e 207c 2054 c3a2 692d 6fc3 a26e 207c  .n | T..i-o..n |
+00000730: 20e3 8489 e384 9ecb 8a20 e384 a8e3 84a2   ........ ......
+00000740: cb8a 207c 2054 6169 3520 7561 6e35 207c  .. | Tai5 uan5 |
+00000750: 2044 c3a1 6977 c3a1 6e20 207c 2054 c481   D..iw..n  | T..
+00000760: 692d 75c7 8e6e 2020 7c20 5461 69c2 b2e2  i-u..n  | Tai...
+00000770: 81b5 2075 616e c2b2 e281 b520 7c0d 0a0d  .. uan..... |...
+00000780: 0a23 2323 2320 4469 616c 6563 740d 0a0d  .#### Dialect...
+00000790: 0a60 6469 616c 6563 7460 2053 7472 696e  .`dialect` Strin
+000007a0: 6720 2d20 7072 6566 6572 7265 6420 7072  g - preferred pr
+000007b0: 6f6e 756e 6369 6174 696f 6e2e 0d0a 0d0a  onunciation.....
+000007c0: 2a20 6073 6f75 7468 6020 2864 6566 6175  * `south` (defau
+000007d0: 6c74 2920 2d20 5b5a 6861 6e67 7a68 6f75  lt) - [Zhangzhou
+000007e0: 5d5b 7a68 616e 677a 686f 752d 7769 6b69  ][zhangzhou-wiki
+000007f0: 5d2d 6c65 616e 696e 6720 7072 6f6e 756e  ]-leaning pronun
+00000800: 6369 6174 696f 6e0d 0a2a 2060 6e6f 7274  ciation..* `nort
+00000810: 6860 202d 205b 5175 616e 7a68 6f75 5d5b  h` - [Quanzhou][
+00000820: 7175 616e 7a68 6f75 2d77 696b 695d 2d6c  quanzhou-wiki]-l
+00000830: 6561 6e69 6e67 2070 726f 6e75 6e63 6961  eaning pronuncia
+00000840: 7469 6f6e 0d0a 0d0a 7c20 7465 7874 2020  tion....| text  
+00000850: 207c 2073 6f75 7468 2020 2020 2020 2020   | south        
+00000860: 207c 206e 6f72 7468 2020 2020 2020 2020   | north        
+00000870: 207c 0d0a 7c20 2d2d 2d2d 2d2d 207c 202d   |..| ------ | -
+00000880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
+00000890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a  ------------ |..
+000008a0: 7c20 e4ba 94e6 9c88 e7af 8020 7c20 47c5  | ......... | G.
+000008b0: 8d6f 2d67 7565 cc8d 682d 7473 6568 207c  .o-gue..h-tseh |
+000008c0: 2047 c58d 6f2d 6765 cc8d 682d 7473 7565   G..o-ge..h-tsue
+000008d0: 6820 7c0d 0a0d 0a23 2323 2320 466f 726d  h |....#### Form
+000008e0: 6174 0d0a 0d0a 6066 6f72 6d61 7460 2053  at....`format` S
+000008f0: 7472 696e 6720 2d20 666f 726d 6174 2069  tring - format i
+00000900: 6e20 7768 6963 6820 746f 6e65 7320 7769  n which tones wi
+00000910: 6c6c 2062 6520 7265 7072 6573 656e 7465  ll be represente
+00000920: 6420 696e 2074 6865 2063 6f6e 7665 7274  d in the convert
+00000930: 6564 2073 656e 7465 6e63 652e 0d0a 0d0a  ed sentence.....
+00000940: 2a20 606d 6172 6b60 2028 6465 6661 756c  * `mark` (defaul
+00000950: 7429 202d 2075 7365 7320 6469 6163 7269  t) - uses diacri
+00000960: 7469 6373 2066 6f72 2065 6163 6820 7379  tics for each sy
+00000970: 6c6c 6162 6c65 2e20 4e6f 7420 6176 6169  llable. Not avai
+00000980: 6c61 626c 6520 666f 7220 544c 5041 2e0d  lable for TLPA..
+00000990: 0a2a 2060 6e75 6d62 6572 6020 2d20 6164  .* `number` - ad
+000009a0: 6420 6120 6e75 6d62 6572 2077 6869 6368  d a number which
+000009b0: 2072 6570 7265 7365 6e74 7320 7468 6520   represents the 
+000009c0: 746f 6e65 2061 7420 7468 6520 656e 6420  tone at the end 
+000009d0: 6f66 2074 6865 2073 796c 6c61 626c 650d  of the syllable.
+000009e0: 0a2a 2060 7374 7269 7060 202d 2072 656d  .* `strip` - rem
+000009f0: 6f76 6573 2061 6e79 2074 6f6e 6520 6d61  oves any tone ma
+00000a00: 726b 696e 670d 0a0d 0a7c 2074 6578 7420  rking....| text 
+00000a10: 7c20 6d61 726b 2020 2020 7c20 6e75 6d62  | mark    | numb
+00000a20: 6572 2020 2020 7c20 7374 7269 7020 2020  er    | strip   
+00000a30: 7c0d 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d  |..| ---- | ----
+00000a40: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d20  --- | --------- 
+00000a50: 7c20 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e5  | ------- |..| .
+00000a60: 8fb0 e781 a320 7c20 54c3 a269 2d75 c3a2  ..... | T..i-u..
+00000a70: 6e20 7c20 5461 6935 2d75 616e 3520 7c20  n | Tai5-uan5 | 
+00000a80: 5461 692d 7561 6e20 7c0d 0a0d 0a23 2323  Tai-uan |....###
+00000a90: 2320 4465 6c69 6d69 7465 720d 0a0d 0a60  # Delimiter....`
+00000aa0: 6465 6c69 6d69 7465 7260 2053 7472 696e  delimiter` Strin
+00000ab0: 6720 2d20 7365 7473 2074 6865 2064 656c  g - sets the del
+00000ac0: 696d 6974 6572 2063 6861 7261 6374 6572  imiter character
+00000ad0: 2074 6861 7420 7769 6c6c 2062 6520 706c   that will be pl
+00000ae0: 6163 6564 2069 6e20 6265 7477 6565 6e20  aced in between 
+00000af0: 7379 6c6c 6162 6c65 7320 6f66 2061 2077  syllables of a w
+00000b00: 6f72 642e 0d0a 0d0a 4465 6661 756c 7420  ord.....Default 
+00000b10: 7661 6c75 6520 6465 7065 6e64 7320 6f6e  value depends on
+00000b20: 2074 6865 2063 686f 7365 6e20 6073 7973   the chosen `sys
+00000b30: 7465 6d60 3a0d 0a0d 0a2a 2060 272d 2760  tem`:....* `'-'`
+00000b40: 202d 2066 6f72 2060 5461 696c 6f60 2c20   - for `Tailo`, 
+00000b50: 6050 4f4a 602c 2060 546f 6e67 696f 6e67  `POJ`, `Tongiong
+00000b60: 600d 0a2a 2060 2727 6020 2d20 666f 7220  `..* `''` - for 
+00000b70: 6050 696e 6779 696d 600d 0a2a 2060 2720  `Pingyim`..* `' 
+00000b80: 2760 202d 2066 6f72 2060 5a68 7579 696e  '` - for `Zhuyin
+00000b90: 602c 2060 544c 5041 602c 2060 4950 4160  `, `TLPA`, `IPA`
+00000ba0: 0d0a 0d0a 7c20 7465 7874 207c 2027 2d27  ....| text | '-'
+00000bb0: 2020 2020 207c 2027 2720 2020 2020 7c20       | ''     | 
+00000bc0: 2720 2720 2020 2020 7c0d 0a7c 202d 2d2d  ' '     |..| ---
+00000bd0: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
+00000be0: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 207c  ---- | ------- |
+00000bf0: 0d0a 7c20 e58f b0e7 81a3 207c 2054 c3a2  ..| ...... | T..
+00000c00: 692d 75c3 a26e 207c 2054 c3a2 6975 c3a2  i-u..n | T..iu..
+00000c10: 6e20 7c20 54c3 a269 2075 c3a2 6e20 7c0d  n | T..i u..n |.
+00000c20: 0a0d 0a23 2323 2320 5361 6e64 6869 0d0a  ...#### Sandhi..
+00000c30: 0d0a 6073 616e 6468 6960 2053 7472 696e  ..`sandhi` Strin
+00000c40: 6720 2d20 6170 706c 6965 7320 7468 6520  g - applies the 
+00000c50: 5b73 616e 6468 6920 7275 6c65 7320 6f66  [sandhi rules of
+00000c60: 2054 6169 7761 6e65 7365 2048 6f6b 6b69   Taiwanese Hokki
+00000c70: 656e 5d5b 7361 6e64 6869 2d77 696b 695d  en][sandhi-wiki]
+00000c80: 2074 6f20 7379 6c6c 6162 6c65 7320 6f66   to syllables of
+00000c90: 2061 2073 696e 676c 6520 776f 7264 2e0d   a single word..
+00000ca0: 0a0d 0a53 696e 6365 2069 7427 7320 6469  ...Since it's di
+00000cb0: 6666 6963 756c 7420 746f 2065 6e63 6f64  fficult to encod
+00000cc0: 6520 616c 6c20 7361 6e64 6869 2072 756c  e all sandhi rul
+00000cd0: 6573 2c20 5461 6962 756e 2070 726f 7669  es, Taibun provi
+00000ce0: 6465 7320 6d75 6c74 6970 6c65 206d 6f64  des multiple mod
+00000cf0: 6573 2066 6f72 2073 616e 6468 6920 636f  es for sandhi co
+00000d00: 6e76 6572 7369 6f6e 2074 6f20 616c 6c6f  nversion to allo
+00000d10: 7720 666f 7220 6375 7374 6f6d 6973 6564  w for customised
+00000d20: 2073 616e 6468 6920 6861 6e64 6c69 6e67   sandhi handling
+00000d30: 2e0d 0a0d 0a2a 2060 6e6f 6e65 6020 2d20  .....* `none` - 
+00000d40: 646f 6573 6e27 7420 7065 7266 6f72 6d20  doesn't perform 
+00000d50: 616e 7920 746f 6e65 2073 616e 6468 690d  any tone sandhi.
+00000d60: 0a2a 2060 6175 746f 6020 2d20 636c 6f73  .* `auto` - clos
+00000d70: 6573 7420 6170 7072 6f78 696d 6174 696f  est approximatio
+00000d80: 6e20 746f 2066 756c 6c20 636f 7272 6563  n to full correc
+00000d90: 7420 746f 6e65 2073 616e 6468 6920 6f66  t tone sandhi of
+00000da0: 2054 6169 7761 6e65 7365 2c20 7769 7468   Taiwanese, with
+00000db0: 2070 726f 7065 7220 7361 6e64 6869 206f   proper sandhi o
+00000dc0: 6620 7072 6f6e 6f75 6e73 2c20 7375 6666  f pronouns, suff
+00000dd0: 6978 6573 2c20 616e 6420 776f 7264 7320  ixes, and words 
+00000de0: 7769 7468 20e4 bb94 0d0a 2a20 6065 7863  with .....* `exc
+00000df0: 5f6c 6173 7460 202d 2063 6861 6e67 6573  _last` - changes
+00000e00: 2074 6f6e 6520 666f 7220 6576 6572 7920   tone for every 
+00000e10: 7379 6c6c 6162 6c65 2065 7863 6570 7420  syllable except 
+00000e20: 666f 7220 7468 6520 6c61 7374 206f 6e65  for the last one
+00000e30: 0d0a 2a20 6069 6e63 6c5f 6c61 7374 6020  ..* `incl_last` 
+00000e40: 2d20 6368 616e 6765 7320 746f 6e65 2066  - changes tone f
+00000e50: 6f72 2065 7665 7279 2073 796c 6c61 626c  or every syllabl
+00000e60: 6520 696e 636c 7564 696e 6720 7468 6520  e including the 
+00000e70: 6c61 7374 206f 6e65 0d0a 0d0a 4465 6661  last one....Defa
+00000e80: 756c 7420 7661 6c75 6520 6465 7065 6e64  ult value depend
+00000e90: 7320 6f6e 2074 6865 2063 686f 7365 6e20  s on the chosen 
+00000ea0: 6073 7973 7465 6d60 3a0d 0a0d 0a2a 2060  `system`:....* `
+00000eb0: 6175 746f 6020 2d20 666f 7220 6054 6f6e  auto` - for `Ton
+00000ec0: 6769 6f6e 6760 0d0a 2a20 606e 6f6e 6560  giong`..* `none`
+00000ed0: 202d 2066 6f72 2060 5461 696c 6f60 2c20   - for `Tailo`, 
+00000ee0: 6050 4f4a 602c 2060 5a68 7579 696e 602c  `POJ`, `Zhuyin`,
+00000ef0: 2060 544c 5041 602c 2060 5069 6e67 7969   `TLPA`, `Pingyi
+00000f00: 6d60 2c20 6049 5041 600d 0a0d 0a7c 2074  m`, `IPA`....| t
+00000f10: 6578 7420 2020 2020 2020 2020 7c20 6e6f  ext         | no
+00000f20: 6e65 2020 2020 2020 2020 2020 2020 2020  ne              
+00000f30: 2020 207c 2061 7574 6f20 2020 2020 2020     | auto       
+00000f40: 2020 2020 2020 2020 2020 7c20 6578 635f            | exc_
+00000f50: 6c61 7374 2020 2020 2020 2020 2020 2020  last            
+00000f60: 207c 2069 6e63 6c5f 6c61 7374 2020 2020   | incl_last    
+00000f70: 2020 2020 2020 2020 7c0d 0a7c 202d 2d2d          |..| ---
+00000f80: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
+00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000fa0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00000fb0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+00000fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+00000fd0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00000fe0: 2d2d 2d2d 2d20 7c0d 0a7c 20e9 8099 e698  ----- |..| .....
+00000ff0: afe5 8fb0 e781 a3e5 9ba1 e4bb 9420 7c20  ............. | 
+00001000: 5473 6520 73c4 ab20 54c3 a269 2d75 c3a2  Tse s.. T..i-u..
+00001010: 6e20 67c3 ad6e 2dc3 a120 7c20 5473 6520  n g..n-.. | Tse 
+00001020: 73c3 ac20 54c4 8169 2d75 c481 6e20 6769  s.. T..i-u..n gi
+00001030: 6e2d c3a1 207c 2054 73c4 9320 73c3 ac20  n-.. | Ts.. s.. 
+00001040: 54c4 8169 2d75 c481 6e20 6769 6e2d c3a1  T..i-u..n gin-..
+00001050: 207c 2054 73c4 9320 73c3 ac20 54c4 8169   | Ts.. s.. T..i
+00001060: 2d75 c481 6e20 6769 6e2d 6120 7c0d 0a0d  -u..n gin-a |...
+00001070: 0a53 616e 6468 6920 7275 6c65 7320 616c  .Sandhi rules al
+00001080: 736f 2063 6861 6e67 6520 6465 7065 6e64  so change depend
+00001090: 696e 6720 6f6e 2074 6865 2064 6961 6c65  ing on the diale
+000010a0: 6374 2063 686f 7365 6e2e 0d0a 0d0a 7c20  ct chosen.....| 
+000010b0: 7465 7874 207c 206e 6f20 7361 6e64 6869  text | no sandhi
+000010c0: 207c 2073 6f75 7468 2020 207c 206e 6f72   | south   | nor
+000010d0: 7468 2020 207c 0d0a 7c20 2d2d 2d2d 207c  th   |..| ---- |
+000010e0: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
+000010f0: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 207c  ---- | ------- |
+00001100: 0d0a 7c20 e58f b0e7 81a3 207c 2054 c3a2  ..| ...... | T..
+00001110: 692d 75c3 a26e 2020 207c 2054 c481 692d  i-u..n   | T..i-
+00001120: 75c3 a26e 207c 2054 c3a0 692d 75c3 a26e  u..n | T..i-u..n
+00001130: 207c 0d0a 0d0a 2323 2323 2050 756e 6374   |....#### Punct
+00001140: 7561 7469 6f6e 0d0a 0d0a 6070 756e 6374  uation....`punct
+00001150: 7561 7469 6f6e 6020 5374 7269 6e67 0d0a  uation` String..
+00001160: 0d0a 2a20 6066 6f72 6d61 7460 2028 6465  ..* `format` (de
+00001170: 6661 756c 7429 202d 2063 6f6e 7665 7274  fault) - convert
+00001180: 7320 4368 696e 6573 652d 7374 796c 6520  s Chinese-style 
+00001190: 7075 6e63 7475 6174 696f 6e20 746f 204c  punctuation to L
+000011a0: 6174 696e 2d73 7479 6c65 2070 756e 6374  atin-style punct
+000011b0: 7561 7469 6f6e 2061 6e64 2063 6170 6974  uation and capit
+000011c0: 616c 6973 6573 2077 6f72 6473 2061 7420  alises words at 
+000011d0: 7468 6520 6265 6769 6e6e 696e 6720 6f66  the beginning of
+000011e0: 2065 6163 6820 7365 6e74 656e 6365 2e0d   each sentence..
+000011f0: 0a2a 2060 6e6f 6e65 6020 2d20 7072 6573  .* `none` - pres
+00001200: 6572 7665 7320 4368 696e 6573 652d 7374  erves Chinese-st
+00001210: 796c 6520 7075 6e63 7475 6174 696f 6e20  yle punctuation 
+00001220: 616e 6420 646f 6573 6e27 7420 6361 7069  and doesn't capi
+00001230: 7461 6c69 7365 2077 6f72 6473 2061 7420  talise words at 
+00001240: 7468 6520 6265 6769 6e6e 696e 6720 6f66  the beginning of
+00001250: 206e 6577 2073 656e 7465 6e63 6573 2e0d   new sentences..
+00001260: 0a0d 0a7c 2074 6578 7420 2020 2020 2020  ...| text       
+00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012b0: 2020 2020 7c20 666f 726d 6174 2020 2020      | format    
+000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001310: 2020 2020 2020 2020 7c20 6e6f 6e65 2020          | none  
+00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001370: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001380: 0d0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..| ------------
+00001390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013d0: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
+000013e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001430: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d  ------------- |.
+000014a0: 0a7c 20e9 8099 e698 afe8 87ba e58d 97ef  .| .............
+000014b0: bc8c e7b0 a1e7 a8b1 e380 8ce5 8d97 e380  ................
+000014c0: 8def bc88 e799 bde8 a9b1 e5ad 97ef bc9a  ................
+000014d0: 54c3 a269 2d6c c3a2 6def bc9b e6b3 a8e9  T..i-l..m.......
+000014e0: 9fb3 e7ac a6e8 999f efbc 9ae3 848a e384  ................
+000014f0: 9ecb 8a20 e384 8be3 84a2 cb8a efbc 8ce5  ... ............
+00001500: 9c8b e8aa 9eef bc9a 54c3 a169 6ec3 a16e  ........T..in..n
+00001510: efbc 89e3 8082 207c 2054 7365 2073 c4ab  ...... | Tse s..
+00001520: 2054 c3a2 692d 6cc3 a26d 2c20 6bc3 a16e   T..i-l..m, k..n
+00001530: 2d74 7368 696e 6720 226c c3a2 6d22 2028  -tshing "l..m" (
+00001540: 5065 cc8d 682d 75c4 932d 6ac4 ab3a 2054  Pe..h-u..-j..: T
+00001550: c3a2 692d 6cc3 a26d 3b20 7473 c3b9 2d69  ..i-l..m; ts..-i
+00001560: 6d20 68c3 bb2d 68c5 8d3a 20e3 848a e384  m h..-h..: .....
+00001570: 9ecb 8a20 e384 8be3 84a2 cb8a 2c20 6b6f  ... ........, ko
+00001580: 6b2d 67c3 ad3a 2054 c3a1 696e c3a1 6e29  k-g..: T..in..n)
+00001590: 2e20 7c20 7473 6520 73c4 ab20 54c3 a269  . | tse s.. T..i
+000015a0: 2d6c c3a2 6def bc8c 6bc3 a16e 2d74 7368  -l..m...k..n-tsh
+000015b0: 696e 67e3 808c 6cc3 a26d e380 8def bc88  ing...l..m......
+000015c0: 5065 cc8d 682d 75c4 932d 6ac4 abef bc9a  Pe..h-u..-j.....
+000015d0: 54c3 a269 2d6c c3a2 6def bc9b 7473 c3b9  T..i-l..m...ts..
+000015e0: 2d69 6d20 68c3 bb2d 68c5 8def bc9a e384  -im h..-h.......
+000015f0: 8ae3 849e cb8a 20e3 848b e384 a2cb 8aef  ...... .........
+00001600: bc8c 6b6f 6b2d 67c3 adef bc9a 54c3 a169  ..kok-g.....T..i
+00001610: 6ec3 a16e efbc 89e3 8082 207c 0d0a 0d0a  n..n...... |....
+00001620: 2323 2323 2043 6f6e 7665 7274 206e 6f6e  #### Convert non
+00001630: 2d43 4a4b 0d0a 0d0a 6063 6f6e 7665 7274  -CJK....`convert
+00001640: 5f6e 6f6e 5f63 6a6b 6020 426f 6f6c 6561  _non_cjk` Boolea
+00001650: 6e20 2d20 6465 6669 6e65 7320 7768 6574  n - defines whet
+00001660: 6865 7220 6f72 206e 6f74 2074 6f20 636f  her or not to co
+00001670: 6e76 6572 7420 6e6f 6e2d 4368 696e 6573  nvert non-Chines
+00001680: 6520 776f 7264 732e 2043 616e 2062 6520  e words. Can be 
+00001690: 7573 6564 2074 6f20 636f 6e76 6572 7420  used to convert 
+000016a0: 5461 696c 6f20 746f 2061 6e6f 7468 6572  Tailo to another
+000016b0: 2072 6f6d 616e 6973 6174 696f 6e20 7379   romanisation sy
+000016c0: 7374 656d 2e0d 0a0d 0a2a 2060 5472 7565  stem.....* `True
+000016d0: 6020 2d20 636f 6e76 6572 7420 6e6f 6e2d  ` - convert non-
+000016e0: 4368 696e 6573 6520 6368 6172 6163 7465  Chinese characte
+000016f0: 7220 776f 7264 730d 0a2a 2060 4661 6c73  r words..* `Fals
+00001700: 6560 2028 6465 6661 756c 7429 202d 2063  e` (default) - c
+00001710: 6f6e 7665 7274 206f 6e6c 7920 4368 696e  onvert only Chin
+00001720: 6573 6520 6368 6172 6163 7465 7220 776f  ese character wo
+00001730: 7264 730d 0a0d 0a7c 2074 6578 7420 2020  rds....| text   
+00001740: 2020 207c 2046 616c 7365 2020 2020 2020     | False      
+00001750: 2020 2020 2020 2020 2020 2020 207c 2054               | T
+00001760: 7275 6520 2020 2020 2020 2020 2020 2020  rue             
+00001770: 2020 2020 2020 207c 0d0a 7c20 2d2d 2d2d         |..| ----
+00001780: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
+000017a0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
+000017b0: 2d2d 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e6  --------- |..| .
+000017c0: 8891 e9a3 9f70 68c3 a16e 6720 7c20 e386  .....ph..ng | ..
+000017d0: a3e3 84a8 e384 9acb 8b20 e384 90e3 84a7  ......... ......
+000017e0: e384 9ae3 86b7 cb99 2070 68c3 a16e 6720  ........ ph..ng 
+000017f0: 7c20 e386 a3e3 84a8 e384 9acb 8b20 e384  | ........... ..
+00001800: 90e3 84a7 e384 9ae3 86b7 cb99 20e3 8486  ............ ...
+00001810: e384 a4cb 8b20 7c0d 0a0d 0a23 2323 2054  ..... |....### T
+00001820: 6f6b 656e 6973 6572 0d0a 0d0a 6054 6f6b  okeniser....`Tok
+00001830: 656e 6973 6572 6020 636c 6173 7320 7065  eniser` class pe
+00001840: 7266 6f72 6d73 205b 4e4c 544b 2077 6f72  rforms [NLTK wor
+00001850: 6470 756e 6374 5f74 6f6b 656e 697a 655d  dpunct_tokenize]
+00001860: 5b6e 6c74 6b2d 746f 6b65 6e69 7a65 5d2d  [nltk-tokenize]-
+00001870: 6c69 6b65 2074 6f6b 656e 6973 6174 696f  like tokenisatio
+00001880: 6e20 6f66 2061 2054 6169 7761 6e65 7365  n of a Taiwanese
+00001890: 2048 6f6b 6b69 656e 2073 656e 7465 6e63   Hokkien sentenc
+000018a0: 652e 0d0a 0d0a 6060 6070 7974 686f 6e0d  e.....```python.
+000018b0: 0a23 2063 6f6e 7374 7275 6374 6f72 0d0a  .# constructor..
+000018c0: 7420 3d20 546f 6b65 6e69 7365 7228 290d  t = Tokeniser().
+000018d0: 0a0d 0a23 2074 6f6b 656e 6973 6520 5461  ...# tokenise Ta
+000018e0: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
+000018f0: 7365 6e74 656e 6365 0d0a 742e 746f 6b65  sentence..t.toke
+00001900: 6e69 7365 2869 6e70 7574 290d 0a60 6060  nise(input)..```
+00001910: 0d0a 0d0a 2323 2320 4f74 6865 7220 4675  ....### Other Fu
+00001920: 6e63 7469 6f6e 730d 0a0d 0a60 6060 7079  nctions....```py
+00001930: 7468 6f6e 0d0a 2320 436f 6e76 6572 7420  thon..# Convert 
+00001940: 746f 2054 7261 6469 7469 6f6e 616c 0d0a  to Traditional..
+00001950: 746f 5f74 7261 6469 7469 6f6e 616c 2869  to_traditional(i
+00001960: 6e70 7574 290d 0a0d 0a23 2043 6f6e 7665  nput)....# Conve
+00001970: 7274 2074 6f20 5369 6d70 6c69 6669 6564  rt to Simplified
+00001980: 0d0a 746f 5f73 696d 706c 6966 6965 6428  ..to_simplified(
+00001990: 696e 7075 7429 0d0a 0d0a 2320 4368 6563  input)....# Chec
+000019a0: 6b20 6966 2074 6865 2073 7472 696e 6720  k if the string 
+000019b0: 6973 2066 756c 6c79 2063 6f6d 706f 7365  is fully compose
+000019c0: 6420 6f66 2043 6869 6e65 7365 2063 6861  d of Chinese cha
+000019d0: 7261 6374 6572 730d 0a69 735f 636a 6b28  racters..is_cjk(
+000019e0: 696e 7075 7429 0d0a 6060 600d 0a0d 0a0d  input)..```.....
+000019f0: 0a0d 0a3c 212d 2d20 4558 414d 504c 4520  ...<!-- EXAMPLE 
+00001a00: 2d2d 3e0d 0a23 2320 4578 616d 706c 650d  -->..## Example.
+00001a10: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 2320  ...```python..# 
+00001a20: 436f 6e76 6572 7465 720d 0a66 726f 6d20  Converter..from 
+00001a30: 7461 6962 756e 2069 6d70 6f72 7420 436f  taibun import Co
+00001a40: 6e76 6572 7465 720d 0a0d 0a23 2320 5379  nverter....## Sy
+00001a50: 7374 656d 0d0a 6320 3d20 436f 6e76 6572  stem..c = Conver
+00001a60: 7465 7228 2920 2320 5461 696c 6f20 7379  ter() # Tailo sy
+00001a70: 7374 656d 2064 6566 6175 6c74 0d0a 632e  stem default..c.
+00001a80: 6765 7428 27e5 8588 e794 9fe8 ac9b efbc  get('...........
+00001a90: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
+00001aa0: e380 8227 290d 0a3e 3e20 5369 616e 2d73  ...')..>> Sian-s
+00001ab0: 696e 6e20 6bc3 b36e 672c 2068 61cc 8d6b  inn k..ng, ha..k
+00001ac0: 2d73 696e 6720 7469 c481 6d2d 7469 c481  -sing ti..m-ti..
+00001ad0: 6d20 7468 6961 6e6e 2e0d 0a0d 0a63 203d  m thiann.....c =
+00001ae0: 2043 6f6e 7665 7274 6572 2873 7973 7465   Converter(syste
+00001af0: 6d3d 275a 6875 7969 6e27 290d 0a63 2e67  m='Zhuyin')..c.g
+00001b00: 6574 2827 e585 88e7 949f e8ac 9bef bc8c  et('............
+00001b10: e5ad b8e7 949f e681 ace6 81ac e881 bde3  ................
+00001b20: 8082 2729 0d0a 3e3e 20e3 8492 e384 a7e3  ..')..>> .......
+00001b30: 84a2 20e3 8492 e386 aa20 e384 8de3 86b2  .. ...... ......
+00001b40: cb8b 2c20 e384 8fe3 849a e386 b6cb 9920  .., ........... 
+00001b50: e384 92e3 84a7 e384 a520 e384 89e3 84a7  ......... ......
+00001b60: e386 b0cb ab20 e384 89e3 84a7 e386 b0cb  ..... ..........
+00001b70: ab20 e384 8ae3 84a7 e386 a92e 0d0a 0d0a  . ..............
+00001b80: 2323 2044 6961 6c65 6374 0d0a 6320 3d20  ## Dialect..c = 
+00001b90: 436f 6e76 6572 7465 7228 2920 2320 736f  Converter() # so
+00001ba0: 7574 6820 6469 616c 6563 7420 6465 6661  uth dialect defa
+00001bb0: 756c 740d 0a63 2e67 6574 2822 e688 91e6  ult..c.get("....
+00001bc0: acb2 e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229  ..............")
+00001bd0: 0d0a 3e3e 2047 75c3 a120 6265 6820 c4ab  ..>> Gu.. beh ..
+00001be0: 6e67 2074 c4ab 2074 7369 61cc 8d68 2068  ng t.. tsia..h h
+00001bf0: c3ae 0d0a 0d0a 6320 3d20 436f 6e76 6572  ......c = Conver
+00001c00: 7465 7228 6469 616c 6563 743d 276e 6f72  ter(dialect='nor
+00001c10: 7468 2729 0d0a 632e 6765 7428 22e6 8891  th')..c.get("...
+00001c20: e6ac b2e7 94a8 e7ae b8e9 a39f e9ad 9a22  ..............."
+00001c30: 290d 0a3e 3e20 4775 c3a1 2062 7565 6820  )..>> Gu.. bueh 
+00001c40: c4ab 6e67 2074 c5ab 2074 7369 61cc 8d68  ..ng t.. tsia..h
+00001c50: 2068 c3bb 0d0a 0d0a 2323 2046 6f72 6d61   h......## Forma
+00001c60: 740d 0a63 203d 2043 6f6e 7665 7274 6572  t..c = Converter
+00001c70: 2829 2023 2066 6f72 2054 6169 6c6f 2c20  () # for Tailo, 
+00001c80: 6d61 726b 2062 7920 6465 6661 756c 740d  mark by default.
+00001c90: 0a63 2e67 6574 2822 e794 9fe6 97a5 e5bf  .c.get("........
+00001ca0: abe6 a882 2229 0d0a 3e3e 2053 656e 6e2d  ....")..>> Senn-
+00001cb0: 6a69 cc8d 7420 6b68 75c3 a069 2d6c 6fcc  ji..t khu..i-lo.
+00001cc0: 8d6b 0d0a 0d0a 6320 3d20 436f 6e76 6572  .k....c = Conver
+00001cd0: 7465 7228 666f 726d 6174 3d27 6e75 6d62  ter(format='numb
+00001ce0: 6572 2729 0d0a 632e 6765 7428 22e7 949f  er')..c.get("...
+00001cf0: e697 a5e5 bfab e6a8 8222 290d 0a3e 3e20  .........")..>> 
+00001d00: 5365 6e6e 312d 6a69 7438 206b 6875 6169  Senn1-jit8 khuai
+00001d10: 332d 6c6f 6b38 0d0a 0d0a 6320 3d20 436f  3-lok8....c = Co
+00001d20: 6e76 6572 7465 7228 666f 726d 6174 3d27  nverter(format='
+00001d30: 7374 7269 7027 290d 0a63 2e67 6574 2822  strip')..c.get("
+00001d40: e794 9fe6 97a5 e5bf abe6 a882 2229 0d0a  ............")..
+00001d50: 3e3e 2053 656e 6e2d 6a69 7420 6b68 7561  >> Senn-jit khua
+00001d60: 692d 6c6f 6b0d 0a0d 0a23 2320 4465 6c69  i-lok....## Deli
+00001d70: 6d69 7465 720d 0a63 203d 2043 6f6e 7665  miter..c = Conve
+00001d80: 7274 6572 2864 656c 696d 6974 6572 3d27  rter(delimiter='
+00001d90: 2729 0d0a 632e 6765 7428 22e5 8588 e794  ')..c.get(".....
+00001da0: 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6 81ac  ................
+00001db0: e681 ace8 81bd e380 8222 290d 0a3e 3e20  .........")..>> 
+00001dc0: 5369 616e 7369 6e6e 206b c3b3 6e67 2c20  Siansinn k..ng, 
+00001dd0: 6861 cc8d 6b73 696e 6720 7469 c481 6d74  ha..ksing ti..mt
+00001de0: 69c4 816d 2074 6869 616e 6e2e 0d0a 0d0a  i..m thiann.....
+00001df0: 6320 3d20 436f 6e76 6572 7465 7228 7379  c = Converter(sy
+00001e00: 7374 656d 3d27 5069 6e67 7969 6d27 2c20  stem='Pingyim', 
+00001e10: 6465 6c69 6d69 7465 723d 272d 2729 0d0a  delimiter='-')..
+00001e20: 632e 6765 7428 22e5 8588 e794 9fe8 ac9b  c.get(".........
+00001e30: efbc 8ce5 adb8 e794 9fe6 81ac e681 ace8  ................
+00001e40: 81bd e380 8222 290d 0a3e 3e20 5369 c481  .....")..>> Si..
+00001e50: 6e2d 736e c4ab 2067 c792 6e67 2c20 68c3  n-sn.. g..ng, h.
+00001e60: a167 2d73 c4ab 6e67 2064 69c3 a26d 2d64  .g-s..ng di..m-d
+00001e70: 69c3 a26d 2074 696e c481 2e0d 0a0d 0a23  i..m tin.......#
+00001e80: 2320 5361 6e64 6869 0d0a 6320 3d20 436f  # Sandhi..c = Co
+00001e90: 6e76 6572 7465 7228 2920 2320 666f 7220  nverter() # for 
+00001ea0: 5461 696c 6f2c 2073 616e 6468 6920 6e6f  Tailo, sandhi no
+00001eb0: 6e65 2062 7920 6465 6661 756c 740d 0a63  ne by default..c
+00001ec0: 2e67 6574 2822 e980 99e6 98af e58f b0e7  .get("..........
+00001ed0: 81a3 e59b a1e4 bb94 2229 0d0a 3e3e 2054  ........")..>> T
+00001ee0: 7365 2073 c4ab 2054 c3a2 692d 75c3 a26e  se s.. T..i-u..n
+00001ef0: 2067 c3ad 6e2d c3a1 0d0a 0d0a 6320 3d20   g..n-......c = 
+00001f00: 436f 6e76 6572 7465 7228 7361 6e64 6869  Converter(sandhi
+00001f10: 3d27 6175 746f 2729 0d0a 632e 6765 7428  ='auto')..c.get(
+00001f20: 22e9 8099 e698 afe5 8fb0 e781 a3e5 9ba1  "...............
+00001f30: e4bb 9422 290d 0a3e 3e20 5473 6520 73c3  ...")..>> Tse s.
+00001f40: ac20 54c4 8169 2d75 c481 6e20 6769 6e2d  . T..i-u..n gin-
+00001f50: c3a1 0d0a 0d0a 6320 3d20 436f 6e76 6572  ......c = Conver
+00001f60: 7465 7228 7361 6e64 6869 3d27 6578 635f  ter(sandhi='exc_
+00001f70: 6c61 7374 2729 0d0a 632e 6765 7428 22e9  last')..c.get(".
+00001f80: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
+00001f90: 9422 290d 0a3e 3e20 5473 c493 2073 c3ac  .")..>> Ts.. s..
+00001fa0: 2054 c481 692d 75c4 816e 2067 696e 2dc3   T..i-u..n gin-.
+00001fb0: a10d 0a0d 0a63 203d 2043 6f6e 7665 7274  .....c = Convert
+00001fc0: 6572 2873 616e 6468 693d 2769 6e63 6c5f  er(sandhi='incl_
+00001fd0: 6c61 7374 2729 0d0a 632e 6765 7428 22e9  last')..c.get(".
+00001fe0: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
+00001ff0: 9422 290d 0a3e 3e20 5473 c493 2073 c3ac  .")..>> Ts.. s..
+00002000: 2054 c481 692d 75c4 816e 2067 696e 2d61   T..i-u..n gin-a
+00002010: 0d0a 0d0a 2323 2050 756e 6374 7561 7469  ....## Punctuati
+00002020: 6f6e 0d0a 6320 3d20 436f 6e76 6572 7465  on..c = Converte
+00002030: 7228 2920 2320 666f 726d 6174 2070 756e  r() # format pun
+00002040: 6374 7561 7469 6f6e 2064 6566 6175 6c74  ctuation default
+00002050: 0d0a 632e 6765 7428 22e5 a4aa e7a9 bae6  ..c.get(".......
+00002060: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
+00002070: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
+00002080: 2229 0d0a 3e3e 2054 68c3 a069 2d6b 686f  ")..>> Th..i-kho
+00002090: 6e67 2070 c3ae 6e67 2d69 c3ba 2c20 6cc3  ng p..ng-i.., l.
+000020a0: ad6e 2d68 c3b3 2120 4cc3 ad6e 2074 7369  .n-h..! L..n tsi
+000020b0: 61cc 8d68 2d70 c3a1 2062 75c4 933f 0d0a  a..h-p.. bu..?..
+000020c0: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+000020d0: 7075 6e63 7475 6174 696f 6e3d 276e 6f6e  punctuation='non
+000020e0: 6527 290d 0a63 2e67 6574 2822 e5a4 aae7  e')..c.get("....
+000020f0: a9ba e69c 8be5 8f8b efbc 8ce6 8181 e5a5  ................
+00002100: bdef bc81 e681 81e9 a39f e9a3 bde6 9caa  ................
+00002110: efbc 9f22 290d 0a3e 3e20 7468 c3a0 692d  ...")..>> th..i-
+00002120: 6b68 6f6e 6720 70c3 ae6e 672d 69c3 baef  khong p..ng-i...
+00002130: bc8c 6cc3 ad6e 2d68 c3b3 efbc 816c c3ad  ..l..n-h.....l..
+00002140: 6e20 7473 6961 cc8d 682d 70c3 a120 6275  n tsia..h-p.. bu
+00002150: c493 efbc 9f0d 0a0d 0a23 2320 436f 6e76  .........## Conv
+00002160: 6572 7420 6e6f 6e2d 434a 4b0d 0a63 203d  ert non-CJK..c =
+00002170: 2043 6f6e 7665 7274 2873 7973 7465 6d3d   Convert(system=
+00002180: 275a 6875 7969 6e27 2920 2320 4661 6c73  'Zhuyin') # Fals
+00002190: 6520 636f 6e76 6572 745f 6e6f 6e5f 636a  e convert_non_cj
+000021a0: 6b20 6465 6661 756c 740d 0a63 2e67 6574  k default..c.get
+000021b0: 2822 e688 91e9 a39f 7068 c3a1 6e67 2229  ("......ph..ng")
+000021c0: 0d0a 3e3e 20e3 86a3 e384 a8e3 849a cb8b  ..>> ...........
+000021d0: 20e3 8490 e384 a7e3 849a e386 b7cb 9920   .............. 
+000021e0: 7068 c3a1 6e67 0d0a 0d0a 6320 3d20 436f  ph..ng....c = Co
+000021f0: 6e76 6572 7428 7379 7374 656d 3d27 5a68  nvert(system='Zh
+00002200: 7579 696e 272c 2063 6f6e 7665 7274 5f6e  uyin', convert_n
+00002210: 6f6e 5f63 6a6b 3d54 7275 6529 0d0a 632e  on_cjk=True)..c.
+00002220: 6765 7428 22e6 8891 e9a3 9f70 68c3 a16e  get("......ph..n
+00002230: 6722 290d 0a3e 3e20 e386 a3e3 84a8 e384  g")..>> ........
+00002240: 9acb 8b20 e384 90e3 84a7 e384 9ae3 86b7  ... ............
+00002250: cb99 20e3 8486 e384 a4cb 8b0d 0a0d 0a0d  .. .............
+00002260: 0a23 2054 6f6b 656e 6973 6572 0d0a 6672  .# Tokeniser..fr
+00002270: 6f6d 2074 6169 6275 6e20 696d 706f 7274  om taibun import
+00002280: 2054 6f6b 656e 6973 6572 0d0a 0d0a 7420   Tokeniser....t 
+00002290: 3d20 546f 6b65 6e69 7365 7228 290d 0a74  = Tokeniser()..t
+000022a0: 2e74 6f6b 656e 6973 6528 22e5 a4aa e7a9  .tokenise(".....
+000022b0: bae6 9c8b e58f 8bef bc8c e681 81e5 a5bd  ................
+000022c0: efbc 81e6 8181 e9a3 9fe9 a3bd e69c aaef  ................
+000022d0: bc9f 2229 0d0a 3e3e 205b 27e5 a4aa e7a9  ..")..>> ['.....
+000022e0: ba27 2c20 27e6 9c8b e58f 8b27 2c20 27ef  .', '......', '.
+000022f0: bc8c 272c 2027 e681 81e5 a5bd 272c 2027  ..', '......', '
+00002300: efbc 8127 2c20 27e6 8181 272c 2027 e9a3  ...', '...', '..
+00002310: 9fe9 a3bd 272c 2027 e69c aa27 2c20 27ef  ....', '...', '.
+00002320: bc9f 275d 0d0a 0d0a 0d0a 2320 4f74 6865  ..']......# Othe
+00002330: 7220 4675 6e63 7469 6f6e 730d 0a66 726f  r Functions..fro
+00002340: 6d20 7461 6962 756e 2069 6d70 6f72 7420  m taibun import 
+00002350: 746f 5f74 7261 6469 7469 6f6e 616c 2c20  to_traditional, 
+00002360: 746f 5f73 696d 706c 6966 6965 642c 2069  to_simplified, i
+00002370: 735f 636a 6b0d 0a0d 0a74 6f5f 7472 6164  s_cjk....to_trad
+00002380: 6974 696f 6e61 6c28 22e6 8891 e590 ace6  itional(".......
+00002390: 97a0 e58f b0e6 b9be e8af 9d22 290d 0a3e  ...........")..>
+000023a0: 3e20 e688 91e8 81bd e784 a1e5 8fb0 e781  > ..............
+000023b0: a3e8 a9b1 0d0a 0d0a 746f 5f73 696d 706c  ........to_simpl
+000023c0: 6966 6965 6428 22e6 8891 e881 bde7 84a1  ified(".........
+000023d0: e887 bae7 81a3 e8a9 b122 290d 0a3e 3e20  .........")..>> 
+000023e0: e688 91e5 90ac e697 a0e5 8fb0 e6b9 bee8  ................
+000023f0: af9d 0d0a 0d0a 6973 5f63 6a6b 2827 e688  ......is_cjk('..
+00002400: 91e9 a39f e9ba ad27 290d 0a3e 3e20 5472  .......')..>> Tr
+00002410: 7565 0d0a 0d0a 6973 5f63 6a6b 2827 e688  ue....is_cjk('..
+00002420: 91e9 a39f 7068 c3a1 6e67 2729 0d0a 3e3e  ....ph..ng')..>>
+00002430: 2046 616c 7365 0d0a 6060 600d 0a0d 0a0d   False..```.....
+00002440: 0a0d 0a3c 212d 2d20 4441 5441 202d 2d3e  ...<!-- DATA -->
+00002450: 0d0a 2323 2044 6174 610d 0a0d 0a2d 205b  ..## Data....- [
+00002460: 5461 6977 616e 6573 652d 4368 696e 6573  Taiwanese-Chines
+00002470: 6520 4f6e 6c69 6e65 2044 6963 7469 6f6e  e Online Diction
+00002480: 6172 795d 5b6f 6e6c 696e 652d 6469 6374  ary][online-dict
+00002490: 696f 6e61 7279 5d20 2876 6961 205b 4368  ionary] (via [Ch
+000024a0: 686f 6554 6169 6769 5d5b 6461 7461 2d76  hoeTaigi][data-v
+000024b0: 6961 5d29 0d0a 2d20 5b69 5461 6967 6920  ia])..- [iTaigi 
+000024c0: 4368 696e 6573 652d 5461 6977 616e 6573  Chinese-Taiwanes
+000024d0: 6520 436f 6d70 6172 6973 6f6e 2044 6963  e Comparison Dic
+000024e0: 7469 6f6e 6172 795d 5b69 7461 6967 692d  tionary][itaigi-
+000024f0: 6469 6374 696f 6e61 7279 5d20 2876 6961  dictionary] (via
+00002500: 205b 4368 686f 6554 6169 6769 5d5b 6461   [ChhoeTaigi][da
+00002510: 7461 2d76 6961 5d29 0d0a 0d0a 0d0a 0d0a  ta-via])........
+00002520: 3c21 2d2d 2041 434b 4e4f 574c 4544 4745  <!-- ACKNOWLEDGE
+00002530: 4d45 4e54 5320 2d2d 3e0d 0a23 2320 4163  MENTS -->..## Ac
+00002540: 6b6e 6f77 6c65 6467 656d 656e 7473 0d0a  knowledgements..
+00002550: 0d0a 2d20 5361 6d75 656c 204a 656e 2028  ..- Samuel Jen (
+00002560: 5b47 6974 6875 625d 5b73 616d 7565 6c2d  [Github][samuel-
+00002570: 6769 7468 7562 5d20 c2b7 205b 4c69 6e6b  github] .. [Link
+00002580: 6564 496e 5d5b 7361 6d75 656c 2d6c 696e  edIn][samuel-lin
+00002590: 6b65 6469 6e5d 2920 2d20 5461 6977 616e  kedin]) - Taiwan
+000025a0: 6573 6520 616e 6420 4d61 6e64 6172 696e  ese and Mandarin
+000025b0: 2074 7261 6e73 6c61 7469 6f6e 0d0a 0d0a   translation....
+000025c0: 0d0a 0d0a 3c21 2d2d 204c 4943 454e 4345  ....<!-- LICENCE
+000025d0: 202d 2d3e 0d0a 2323 204c 6963 656e 6365   -->..## Licence
+000025e0: 0d0a 0d0a 4265 6361 7573 6520 5461 6962  ....Because Taib
+000025f0: 756e 2069 7320 4d49 542d 6c69 6365 6e73  un is MIT-licens
+00002600: 6564 2c20 616e 7920 6465 7665 6c6f 7065  ed, any develope
+00002610: 7220 6361 6e20 6573 7365 6e74 6961 6c6c  r can essentiall
+00002620: 7920 646f 2077 6861 7465 7665 7220 7468  y do whatever th
+00002630: 6579 2077 616e 7420 7769 7468 2069 7420  ey want with it 
+00002640: 6173 206c 6f6e 6720 6173 2074 6865 7920  as long as they 
+00002650: 696e 636c 7564 6520 7468 6520 6f72 6967  include the orig
+00002660: 696e 616c 2063 6f70 7972 6967 6874 2061  inal copyright a
+00002670: 6e64 206c 6963 656e 6365 206e 6f74 6963  nd licence notic
+00002680: 6520 696e 2061 6e79 2063 6f70 6965 7320  e in any copies 
+00002690: 6f66 2074 6865 2073 6f75 7263 6520 636f  of the source co
+000026a0: 6465 2e20 4e6f 7465 2c20 7468 6174 2074  de. Note, that t
+000026b0: 6865 2064 6174 6120 7573 6564 2062 7920  he data used by 
+000026c0: 7468 6520 7061 636b 6167 6520 6973 206c  the package is l
+000026d0: 6963 656e 7365 6420 756e 6465 7220 6120  icensed under a 
+000026e0: 6469 6666 6572 656e 7420 636f 7079 7269  different copyri
+000026f0: 6768 742e 0d0a 0d0a 5468 6520 6461 7461  ght.....The data
+00002700: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
+00002710: 6572 205b 4343 2042 592d 5341 2034 2e30  er [CC BY-SA 4.0
+00002720: 5d5b 6461 7461 2d63 635d 0d0a 0d0a 0d0a  ][data-cc]......
+00002730: 0d0a 3c21 2d2d 204d 4152 4b44 4f57 4e20  ..<!-- MARKDOWN 
+00002740: 4c49 4e4b 5320 2d2d 3e0d 0a5b 7465 7374  LINKS -->..[test
+00002750: 735d 3a20 6874 7470 733a 2f2f 6769 7468  s]: https://gith
+00002760: 7562 2e63 6f6d 2f61 6e64 7265 6968 6172  ub.com/andreihar
+00002770: 2f74 6169 6275 6e2f 6163 7469 6f6e 730d  /taibun/actions.
+00002780: 0a5b 7465 7374 732d 6261 6467 655d 3a20  .[tests-badge]: 
+00002790: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000027a0: 6c64 732e 696f 2f67 6974 6875 622f 6163  lds.io/github/ac
+000027b0: 7469 6f6e 732f 776f 726b 666c 6f77 2f73  tions/workflow/s
+000027c0: 7461 7475 732f 616e 6472 6569 6861 722f  tatus/andreihar/
+000027d0: 7461 6962 756e 2f63 692e 7961 6d6c 3f73  taibun/ci.yaml?s
+000027e0: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+000027f0: 6765 266c 6f67 6f3d 6769 7468 7562 0d0a  ge&logo=github..
+00002800: 5b63 6f6e 7472 6962 7574 6f72 732d 6261  [contributors-ba
+00002810: 6467 655d 3a20 6874 7470 733a 2f2f 696d  dge]: https://im
+00002820: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00002830: 6875 622f 636f 6e74 7269 6275 746f 7273  hub/contributors
+00002840: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
+00002850: 6e3f 7374 796c 653d 666f 722d 7468 652d  n?style=for-the-
+00002860: 6261 6467 650d 0a5b 636f 6e74 7269 6275  badge..[contribu
+00002870: 746f 7273 5d3a 2023 7573 6167 650d 0a5b  tors]: #usage..[
+00002880: 7265 6c65 6173 652d 6261 6467 655d 3a20  release-badge]: 
+00002890: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000028a0: 6c64 732e 696f 2f67 6974 6875 622f 762f  lds.io/github/v/
+000028b0: 7265 6c65 6173 652f 616e 6472 6569 6861  release/andreiha
+000028c0: 722f 7461 6962 756e 3f63 6f6c 6f72 3d33  r/taibun?color=3
+000028d0: 3836 3138 6326 7374 796c 653d 666f 722d  8618c&style=for-
+000028e0: 7468 652d 6261 6467 650d 0a5b 7265 6c65  the-badge..[rele
+000028f0: 6173 655d 3a20 6874 7470 733a 2f2f 6769  ase]: https://gi
+00002900: 7468 7562 2e63 6f6d 2f61 6e64 7265 6968  thub.com/andreih
+00002910: 6172 2f74 6169 6275 6e2f 7265 6c65 6173  ar/taibun/releas
+00002920: 6573 0d0a 5b6c 6963 656e 6365 2d62 6164  es..[licence-bad
+00002930: 6765 5d3a 2068 7474 7073 3a2f 2f69 6d67  ge]: https://img
+00002940: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00002950: 7562 2f6c 6963 656e 7365 2f61 6e64 7265  ub/license/andre
+00002960: 6968 6172 2f74 6169 6275 6e3f 636f 6c6f  ihar/taibun?colo
+00002970: 723d 3030 3030 3030 2673 7479 6c65 3d66  r=000000&style=f
+00002980: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b6c  or-the-badge..[l
+00002990: 6963 656e 6365 5d3a 204c 4943 454e 5345  icence]: LICENSE
+000029a0: 0d0a 5b6c 696e 6b65 6469 6e2d 6261 6467  ..[linkedin-badg
+000029b0: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
+000029c0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000029d0: 2f4c 696e 6b65 6449 6e2d 3030 3737 4235  /LinkedIn-0077B5
+000029e0: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+000029f0: 6164 6765 266c 6f67 6f3d 6c69 6e6b 6564  adge&logo=linked
+00002a00: 696e 266c 6f67 6f43 6f6c 6f72 3d77 6869  in&logoColor=whi
+00002a10: 7465 0d0a 5b6c 696e 6b65 6469 6e5d 3a20  te..[linkedin]: 
+00002a20: 6874 7470 733a 2f2f 7777 772e 6c69 6e6b  https://www.link
+00002a30: 6564 696e 2e63 6f6d 2f69 6e2f 616e 6472  edin.com/in/andr
+00002a40: 6569 2d68 6172 6261 6368 6f76 2f0d 0a0d  ei-harbachov/...
+00002a50: 0a5b 7079 7069 5d3a 2068 7474 7073 3a2f  .[pypi]: https:/
+00002a60: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00002a70: 742f 7461 6962 756e 0d0a 5b62 7567 5d3a  t/taibun..[bug]:
+00002a80: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002a90: 636f 6d2f 616e 6472 6569 6861 722f 7461  com/andreihar/ta
+00002aa0: 6962 756e 2f69 7373 7565 730d 0a5b 6f6e  ibun/issues..[on
+00002ab0: 6c69 6e65 2d64 6963 7469 6f6e 6172 795d  line-dictionary]
+00002ac0: 3a20 6874 7470 3a2f 2f69 7031 3934 3039  : http://ip19409
+00002ad0: 372e 6e74 6375 2e65 6475 2e74 772f 756e  7.ntcu.edu.tw/un
+00002ae0: 6769 616e 2f73 6f61 6e6e 7465 6e67 2f63  gian/soannteng/c
+00002af0: 6869 6c2f 5461 6968 6f61 2e61 7370 0d0a  hil/Taihoa.asp..
+00002b00: 5b69 7461 6967 692d 6469 6374 696f 6e61  [itaigi-dictiona
+00002b10: 7279 5d3a 2068 7474 7073 3a2f 2f69 7461  ry]: https://ita
+00002b20: 6967 692e 7477 2f0d 0a5b 6461 7461 2d76  igi.tw/..[data-v
+00002b30: 6961 5d3a 2068 7474 7073 3a2f 2f67 6974  ia]: https://git
+00002b40: 6875 622e 636f 6d2f 4368 686f 6554 6169  hub.com/ChhoeTai
+00002b50: 6769 2f43 6868 6f65 5461 6967 6944 6174  gi/ChhoeTaigiDat
+00002b60: 6162 6173 650d 0a5b 6461 7461 2d63 635d  abase..[data-cc]
+00002b70: 3a20 6874 7470 733a 2f2f 6372 6561 7469  : https://creati
+00002b80: 7665 636f 6d6d 6f6e 732e 6f72 672f 6c69  vecommons.org/li
+00002b90: 6365 6e73 6573 2f62 792d 7361 2f34 2e30  censes/by-sa/4.0
+00002ba0: 2f64 6565 642e 656e 0d0a 5b73 616d 7565  /deed.en..[samue
+00002bb0: 6c2d 6769 7468 7562 5d3a 2068 7474 7073  l-github]: https
+00002bc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5353  ://github.com/SS
+00002bd0: 5361 6d0d 0a5b 7361 6d75 656c 2d6c 696e  Sam..[samuel-lin
+00002be0: 6b65 6469 6e5d 3a20 6874 7470 733a 2f2f  kedin]: https://
+00002bf0: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
+00002c00: 2f69 6e2f 7361 6d75 656c 2d6a 656e 2f0d  /in/samuel-jen/.
+00002c10: 0a0d 0a5b 7461 696c 6f2d 7769 6b69 5d3a  ...[tailo-wiki]:
+00002c20: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+00002c30: 7065 6469 612e 6f72 672f 7769 6b69 2f54  pedia.org/wiki/T
+00002c40: 2543 3325 4132 692d 7525 4333 2541 326e  %C3%A2i-u%C3%A2n
+00002c50: 5f4c 2543 3325 4234 2d6d 2543 3325 4131  _L%C3%B4-m%C3%A1
+00002c60: 2d6a 2543 3425 4142 5f50 6869 6e67 2d69  -j%C4%AB_Phing-i
+00002c70: 6d5f 486f 6e67 2d25 4333 2541 306e 0d0a  m_Hong-%C3%A0n..
+00002c80: 5b70 6f6a 2d77 696b 695d 3a20 6874 7470  [poj-wiki]: http
+00002c90: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+00002ca0: 2e6f 7267 2f77 696b 692f 5065 2543 4325  .org/wiki/Pe%CC%
+00002cb0: 3844 682d 2543 3525 3844 652d 6a25 4334  8Dh-%C5%8De-j%C4
+00002cc0: 2541 420d 0a5b 7a68 7579 696e 2d77 696b  %AB..[zhuyin-wik
+00002cd0: 695d 3a20 6874 7470 733a 2f2f 656e 2e77  i]: https://en.w
+00002ce0: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00002cf0: 692f 5461 6977 616e 6573 655f 5068 6f6e  i/Taiwanese_Phon
+00002d00: 6574 6963 5f53 796d 626f 6c73 0d0a 5b74  etic_Symbols..[t
+00002d10: 6c70 612d 7769 6b69 5d3a 2068 7474 7073  lpa-wiki]: https
+00002d20: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00002d30: 6f72 672f 7769 6b69 2f54 6169 7761 6e65  org/wiki/Taiwane
+00002d40: 7365 5f4c 616e 6775 6167 655f 5068 6f6e  se_Language_Phon
+00002d50: 6574 6963 5f41 6c70 6861 6265 740d 0a5b  etic_Alphabet..[
+00002d60: 7069 6e67 7969 6d2d 7769 6b69 5d3a 2068  pingyim-wiki]: h
+00002d70: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00002d80: 6469 612e 6f72 672f 7769 6b69 2f42 6225  dia.org/wiki/Bb%
+00002d90: 4333 2541 316e 6c25 4333 2541 316d 5f70  C3%A1nl%C3%A1m_p
+00002da0: 2543 3325 4143 6e67 7925 4334 2541 426d  %C3%ACngy%C4%ABm
+00002db0: 0d0a 5b74 6f6e 6769 6f6e 672d 7769 6b69  ..[tongiong-wiki
+00002dc0: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
+00002dd0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00002de0: 2f44 6125 4334 2541 422d 6768 2543 3325  /Da%C4%AB-gh%C3%
+00002df0: 4145 5f74 2543 3525 3844 6e67 2d69 2543  AE_t%C5%8Dng-i%C
+00002e00: 3525 3844 6e67 5f70 2543 3425 4142 6e67  5%8Dng_p%C4%ABng
+00002e10: 2d69 6d0d 0a5b 6970 612d 7769 6b69 5d3a  -im..[ipa-wiki]:
+00002e20: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+00002e30: 7065 6469 612e 6f72 672f 7769 6b69 2f49  pedia.org/wiki/I
+00002e40: 6e74 6572 6e61 7469 6f6e 616c 5f50 686f  nternational_Pho
+00002e50: 6e65 7469 635f 416c 7068 6162 6574 0d0a  netic_Alphabet..
+00002e60: 5b7a 6861 6e67 7a68 6f75 2d77 696b 695d  [zhangzhou-wiki]
+00002e70: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
+00002e80: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00002e90: 5a68 616e 677a 686f 755f 6469 616c 6563  Zhangzhou_dialec
+00002ea0: 7473 0d0a 5b71 7561 6e7a 686f 752d 7769  ts..[quanzhou-wi
+00002eb0: 6b69 5d3a 2068 7474 7073 3a2f 2f65 6e2e  ki]: https://en.
+00002ec0: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
+00002ed0: 6b69 2f51 7561 6e7a 686f 755f 6469 616c  ki/Quanzhou_dial
+00002ee0: 6563 7473 0d0a 5b6e 6c74 6b2d 746f 6b65  ects..[nltk-toke
+00002ef0: 6e69 7a65 5d3a 2068 7474 7073 3a2f 2f6e  nize]: https://n
+00002f00: 6c74 6b2e 6f72 672f 6170 692f 6e6c 746b  ltk.org/api/nltk
+00002f10: 2e74 6f6b 656e 697a 652e 6874 6d6c 0d0a  .tokenize.html..
+00002f20: 5b73 616e 6468 692d 7769 6b69 5d3a 2068  [sandhi-wiki]: h
+00002f30: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00002f40: 6469 612e 6f72 672f 7769 6b69 2f54 6169  dia.org/wiki/Tai
+00002f50: 7761 6e65 7365 5f48 6f6b 6b69 656e 2354  wanese_Hokkien#T
+00002f60: 6f6e 6525 3230 7361 6e64 6869 3a7e 3a74  one%20sandhi:~:t
+00002f70: 6578 743d 7468 6e67 2545 3225 3946 2541  ext=thng%E2%9F%A
+00002f80: 3925 3230 2825 3232 736f 7570 2532 3229  9%20(%22soup%22)
+00002f90: 2e2d 2c54 6f6e 6525 3230 7361 6e64 6869  .-,Tone%20sandhi
+00002fa0: 2c2d 2535 4265 6469 7425 3544            ,-%5Bedit%5D
```

