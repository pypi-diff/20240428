# Comparing `tmp/example990420-0.0.7.tar.gz` & `tmp/example990420-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example990420-0.0.7.tar", last modified: Tue Jul  4 09:07:43 2023, max compression
+gzip compressed data, was "example990420-1.1.0.tar", last modified: Sun Apr 28 02:17:08 2024, max compression
```

## Comparing `example990420-0.0.7.tar` & `example990420-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 09:07:43.105015 example990420-0.0.7/
--rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 example990420-0.0.7/LICENSE
--rw-rw-rw-   0        0        0    10953 2023-07-04 09:07:43.103025 example990420-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9927 2023-07-04 09:04:02.000000 example990420-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 09:07:43.073749 example990420-0.0.7/example990420.egg-info/
--rw-rw-rw-   0        0        0    10953 2023-07-04 09:07:42.000000 example990420-0.0.7/example990420.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-07-04 09:07:42.000000 example990420-0.0.7/example990420.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 09:07:42.000000 example990420-0.0.7/example990420.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 09:07:42.000000 example990420-0.0.7/example990420.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 09:07:43.106011 example990420-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-07-04 09:07:33.000000 example990420-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:07:43.082872 example990420-0.0.7/taibun/
--rw-rw-rw-   0        0        0       46 2023-07-04 07:50:30.000000 example990420-0.0.7/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:07:43.092714 example990420-0.0.7/taibun/data/
--rw-rw-rw-   0        0        0    17141 2023-06-17 08:58:24.000000 example990420-0.0.7/taibun/data/simplified.json
--rw-rw-rw-   0        0        0   645595 2023-07-03 18:29:04.000000 example990420-0.0.7/taibun/data/words.json
--rw-rw-rw-   0        0        0    19967 2023-07-04 08:47:50.000000 example990420-0.0.7/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:17:08.012819 example990420-1.1.0/
+-rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 example990420-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    13004 2024-04-28 02:17:08.011634 example990420-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12204 2024-04-28 01:15:26.000000 example990420-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 02:17:08.006224 example990420-1.1.0/example990420.egg-info/
+-rw-rw-rw-   0        0        0    13004 2024-04-28 02:17:07.000000 example990420-1.1.0/example990420.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-28 02:17:07.000000 example990420-1.1.0/example990420.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 02:17:07.000000 example990420-1.1.0/example990420.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 02:17:07.000000 example990420-1.1.0/example990420.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       50 2024-04-28 02:07:06.000000 example990420-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      882 2024-04-28 02:17:08.018963 example990420-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 02:17:07.982112 example990420-1.1.0/taibun/
+-rw-rw-rw-   0        0        0       85 2024-04-27 02:04:57.000000 example990420-1.1.0/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:17:07.992912 example990420-1.1.0/taibun/data/
+-rw-rw-rw-   0        0        0    17160 2024-04-27 02:06:10.000000 example990420-1.1.0/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0  1893344 2024-04-28 00:12:08.000000 example990420-1.1.0/taibun/data/words.json
+-rw-rw-rw-   0        0        0    25042 2024-04-28 00:18:10.000000 example990420-1.1.0/taibun/taibun.py
```

### Comparing `example990420-0.0.7/LICENSE` & `example990420-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `example990420-0.0.7/PKG-INFO` & `example990420-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,685 +1,813 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2065 7861  : 2.1..Name: exa
 00000020: 6d70 6c65 3939 3034 3230 0d0a 5665 7273  mple990420..Vers
-00000030: 696f 6e3a 2030 2e30 2e37 0d0a 5375 6d6d  ion: 0.0.7..Summ
-00000040: 6172 793a 2043 6f6e 7665 7274 2043 6869  ary: Convert Chi
-00000050: 6e65 7365 2063 6861 7261 6374 6572 7320  nese characters 
-00000060: 746f 2054 6169 7761 6e65 7365 0d0a 486f  to Taiwanese..Ho
-00000070: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-00000080: 2f67 6974 6875 622e 636f 6d2f 616e 6472  /github.com/andr
-00000090: 6569 6861 722f 7461 6962 756e 0d0a 4175  eihar/taibun..Au
-000000a0: 7468 6f72 3a20 416e 6472 6569 2048 6172  thor: Andrei Har
-000000b0: 6261 6368 6f76 0d0a 4175 7468 6f72 2d65  bachov..Author-e
-000000c0: 6d61 696c 3a20 3c61 6e64 7265 692e 6861  mail: <andrei.ha
-000000d0: 7262 6163 686f 7640 676d 6169 6c2e 636f  rbachov@gmail.co
-000000e0: 6d3e 0d0a 4c69 6365 6e73 653a 204d 4954  m>..License: MIT
-000000f0: 0d0a 4b65 7977 6f72 6473 3a20 7079 7468  ..Keywords: pyth
-00000100: 6f6e 2c74 6169 7761 6e2c 7461 6977 616e  on,taiwan,taiwan
-00000110: 6573 652c 7461 6967 692c 686f 6b6b 6965  ese,taigi,hokkie
-00000120: 6e2c 726f 6d61 6e69 7a61 7469 6f6e 2c74  n,romanization,t
-00000130: 7261 6e73 6c69 7465 7261 7469 6f6e 0d0a  ransliteration..
-00000140: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-00000150: 6320 3a3a 2054 6578 7420 5072 6f63 6573  c :: Text Proces
-00000160: 7369 6e67 203a 3a20 4c69 6e67 7569 7374  sing :: Linguist
-00000170: 6963 0d0a 436c 6173 7369 6669 6572 3a20  ic..Classifier: 
-00000180: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000190: 7573 203a 3a20 3220 2d20 5072 652d 416c  us :: 2 - Pre-Al
-000001a0: 7068 610d 0a43 6c61 7373 6966 6965 723a  pha..Classifier:
-000001b0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-000001c0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-000001d0: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000200: 330d 0a43 6c61 7373 6966 6965 723a 204f  3..Classifier: O
-00000210: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000220: 3a3a 2055 6e69 780d 0a43 6c61 7373 6966  :: Unix..Classif
-00000230: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000240: 7973 7465 6d20 3a3a 204d 6163 4f53 203a  ystem :: MacOS :
-00000250: 3a20 4d61 634f 5320 580d 0a43 6c61 7373  : MacOS X..Class
-00000260: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000270: 2053 7973 7465 6d20 3a3a 204d 6963 726f   System :: Micro
-00000280: 736f 6674 203a 3a20 5769 6e64 6f77 730d  soft :: Windows.
-00000290: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000002a0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-000002b0: 6d61 726b 646f 776e 0d0a 4c69 6365 6e73  markdown..Licens
-000002c0: 652d 4669 6c65 3a20 4c49 4345 4e53 450d  e-File: LICENSE.
-000002d0: 0a0d 0a0d 0a3c 212d 2d20 5052 4f4a 4543  .....<!-- PROJEC
-000002e0: 5420 4c4f 474f 202d 2d3e 0d0d 0a3c 6469  T LOGO -->...<di
-000002f0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00000300: 3e0d 0d0a 0d0d 0a23 20e5 8fb0 e696 8720  >......# ...... 
-00000310: 7c20 54c3 a269 2d62 c3bb 6e0d 0d0a 0d0d  | T..i-b..n.....
-00000320: 0a3c 212d 2d20 5052 4f4a 4543 5420 5348  .<!-- PROJECT SH
-00000330: 4945 4c44 5320 2d2d 3e0d 0d0a 5b21 5b43  IELDS -->...[![C
-00000340: 6f6e 7472 6962 7574 6f72 735d 5b63 6f6e  ontributors][con
-00000350: 7472 6962 7574 6f72 732d 6261 6467 655d  tributors-badge]
-00000360: 5d5b 636f 6e74 7269 6275 746f 7273 5d0d  ][contributors].
-00000370: 0d0a 5b21 5b52 656c 6561 7365 5d5b 7265  ..[![Release][re
-00000380: 6c65 6173 652d 6261 6467 655d 5d5b 7265  lease-badge]][re
-00000390: 6c65 6173 655d 0d0d 0a5b 215b 4c69 6365  lease]...[![Lice
-000003a0: 6e63 655d 5b6c 6963 656e 6365 2d62 6164  nce][licence-bad
-000003b0: 6765 5d5d 5b6c 6963 656e 6365 5d0d 0d0a  ge]][licence]...
-000003c0: 5b21 5b4c 696e 6b65 6449 6e5d 5b6c 696e  [![LinkedIn][lin
-000003d0: 6b65 6469 6e2d 6261 6467 655d 5d5b 6c69  kedin-badge]][li
-000003e0: 6e6b 6564 696e 5d0d 0d0a 0d0d 0a2a 2a54  nkedin]......**T
-000003f0: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
-00000400: 2074 7261 6e73 6c69 7465 7261 746f 7220   transliterator 
-00000410: 6672 6f6d 2043 6869 6e65 7365 2063 6861  from Chinese cha
-00000420: 7261 6374 6572 732a 2a0d 0d0a 0d0d 0a49  racters**......I
-00000430: 7420 6861 7320 6d65 7468 6f64 7320 7468  t has methods th
-00000440: 6174 2061 6c6c 6f77 2074 6f20 6375 7374  at allow to cust
-00000450: 6f6d 6973 6520 7472 616e 736c 6974 6572  omise transliter
-00000460: 6174 696f 6e20 616e 6420 7265 7472 6965  ation and retrie
-00000470: 7665 2061 6e79 206e 6563 6573 7361 7279  ve any necessary
-00000480: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-00000490: 7574 2054 6169 7761 6e65 7365 2048 6f6b  ut Taiwanese Hok
-000004a0: 6b69 656e 2070 726f 6e75 6e63 6961 7469  kien pronunciati
-000004b0: 6f6e 2e3c 6272 202f 3e0d 0d0a 496e 636c  on.<br />...Incl
-000004c0: 7564 6573 2077 6f72 6420 746f 6b65 6e69  udes word tokeni
-000004d0: 7365 7220 666f 7220 5461 6977 616e 6573  ser for Taiwanes
-000004e0: 6520 486f 6b6b 6965 6e2e 0d0d 0a0d 0d0a  e Hokkien.......
-000004f0: 5b52 6570 6f72 7420 4275 675d 5b62 7567  [Report Bug][bug
-00000500: 5d20 e280 a20d 0d0a 5b50 7950 495d 5b70  ] ......[PyPI][p
-00000510: 7970 695d 0d0d 0a0d 0d0a 3c2f 6469 763e  ypi]......</div>
-00000520: 0d0d 0a0d 0d0a 0d0d 0a2d 2d2d 0d0d 0a0d  .........---....
-00000530: 0d0a 0d0d 0a3c 212d 2d20 5441 424c 4520  .....<!-- TABLE 
-00000540: 4f46 2043 4f4e 5445 4e54 5320 2d2d 3e0d  OF CONTENTS -->.
-00000550: 0d0a 3c64 6574 6169 6c73 206f 7065 6e3e  ..<details open>
-00000560: 0d0d 0a20 203c 7375 6d6d 6172 793e 5461  ...  <summary>Ta
-00000570: 626c 6520 6f66 2043 6f6e 7465 6e74 733c  ble of Contents<
-00000580: 2f73 756d 6d61 7279 3e0d 0d0a 2020 3c6f  /summary>...  <o
-00000590: 6c3e 0d0d 0a20 2020 203c 6c69 3e3c 6120  l>...    <li><a 
-000005a0: 6872 6566 3d22 2369 6e73 7461 6c6c 223e  href="#install">
-000005b0: 496e 7374 616c 6c3c 2f61 3e3c 2f6c 693e  Install</a></li>
-000005c0: 0d0d 0a20 2020 203c 6c69 3e0d 0d0a 2020  ...    <li>...  
-000005d0: 2020 2020 3c61 2068 7265 663d 2223 7573      <a href="#us
-000005e0: 6167 6522 3e55 7361 6765 3c2f 613e 0d0d  age">Usage</a>..
-000005f0: 0a20 2020 2020 203c 756c 3e0d 0d0a 2020  .      <ul>...  
-00000600: 2020 2020 2020 3c6c 693e 0d0d 0a20 2020        <li>...   
-00000610: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
-00000620: 2363 6f6e 7665 7274 6572 223e 436f 6e76  #converter">Conv
-00000630: 6572 7465 723c 2f61 3e0d 0d0a 2020 2020  erter</a>...    
-00000640: 2020 2020 2020 3c75 6c3e 0d0d 0a20 2020        <ul>...   
-00000650: 2020 2020 2020 2020 203c 6c69 3e3c 6120           <li><a 
-00000660: 6872 6566 3d22 2373 7973 7465 6d22 3e53  href="#system">S
-00000670: 7973 7465 6d3c 2f61 3e3c 2f6c 693e 0d0d  ystem</a></li>..
-00000680: 0a20 2020 2020 2020 2020 2020 203c 6c69  .            <li
-00000690: 3e3c 6120 6872 6566 3d22 2364 6961 6c65  ><a href="#diale
-000006a0: 6374 223e 4469 616c 6563 743c 2f61 3e3c  ct">Dialect</a><
-000006b0: 2f6c 693e 0d0d 0a20 2020 2020 2020 2020  /li>...         
-000006c0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-000006d0: 2366 6f72 6d61 7422 3e46 6f72 6d61 743c  #format">Format<
-000006e0: 2f61 3e3c 2f6c 693e 0d0d 0a20 2020 2020  /a></li>...     
-000006f0: 2020 2020 2020 203c 6c69 3e3c 6120 6872         <li><a hr
-00000700: 6566 3d22 2364 656c 696d 6974 6572 223e  ef="#delimiter">
-00000710: 4465 6c69 6d69 7465 723c 2f61 3e3c 2f6c  Delimiter</a></l
-00000720: 693e 0d0d 0a20 2020 2020 2020 2020 2020  i>...           
-00000730: 203c 6c69 3e3c 6120 6872 6566 3d22 2373   <li><a href="#s
-00000740: 616e 6468 6922 3e53 616e 6468 693c 2f61  andhi">Sandhi</a
-00000750: 3e3c 2f6c 693e 0d0d 0a20 2020 2020 2020  ></li>...       
-00000760: 2020 2020 203c 6c69 3e3c 6120 6872 6566       <li><a href
-00000770: 3d22 2370 756e 6374 7561 7469 6f6e 223e  ="#punctuation">
-00000780: 5075 6e63 7475 6174 696f 6e3c 2f61 3e3c  Punctuation</a><
-00000790: 2f6c 693e 0d0d 0a20 2020 2020 2020 2020  /li>...         
-000007a0: 203c 2f75 6c3e 0d0d 0a20 2020 2020 2020   </ul>...       
-000007b0: 203c 2f6c 693e 0d0d 0a20 2020 2020 2020   </li>...       
-000007c0: 203c 6c69 3e3c 6120 6872 6566 3d22 2374   <li><a href="#t
-000007d0: 6f6b 656e 6973 6572 223e 546f 6b65 6e69  okeniser">Tokeni
-000007e0: 7365 723c 2f61 3e3c 2f6c 693e 0d0d 0a20  ser</a></li>... 
-000007f0: 2020 2020 203c 2f75 6c3e 0d0d 0a20 2020       </ul>...   
-00000800: 203c 2f6c 693e 0d0d 0a20 2020 203c 6c69   </li>...    <li
-00000810: 3e3c 6120 6872 6566 3d22 2365 7861 6d70  ><a href="#examp
-00000820: 6c65 223e 4578 616d 706c 653c 2f61 3e3c  le">Example</a><
-00000830: 2f6c 693e 0d0d 0a20 2020 203c 6c69 3e3c  /li>...    <li><
-00000840: 6120 6872 6566 3d22 2364 6174 6122 3e44  a href="#data">D
-00000850: 6174 613c 2f61 3e3c 2f6c 693e 0d0d 0a20  ata</a></li>... 
-00000860: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-00000870: 236c 6963 656e 6365 223e 4c69 6365 6e63  #licence">Licenc
-00000880: 653c 2f61 3e3c 2f6c 693e 0d0d 0a20 203c  e</a></li>...  <
-00000890: 2f6f 6c3e 0d0d 0a3c 2f64 6574 6169 6c73  /ol>...</details
-000008a0: 3e0d 0d0a 0d0d 0a0d 0d0a 3c21 2d2d 2049  >.........<!-- I
-000008b0: 4e53 5441 4c4c 202d 2d3e 0d0d 0a23 2320  NSTALL -->...## 
-000008c0: 496e 7374 616c 6c0d 0d0a 0d0d 0a54 6169  Install......Tai
-000008d0: 6275 6e20 6361 6e20 6265 2069 6e73 7461  bun can be insta
-000008e0: 6c6c 6564 2066 726f 6d20 5b70 7970 695d  lled from [pypi]
-000008f0: 5b70 7970 695d 0d0d 0a0d 0d0a 6060 6062  [pypi]......```b
-00000900: 6173 680d 0d0a 2420 7069 7020 696e 7374  ash...$ pip inst
-00000910: 616c 6c20 7461 6962 756e 0d0d 0a60 6060  all taibun...```
-00000920: 0d0d 0a0d 0d0a 0d0d 0a3c 212d 2d20 5553  .........<!-- US
-00000930: 4147 4520 2d2d 3e0d 0d0a 2323 2055 7361  AGE -->...## Usa
-00000940: 6765 0d0d 0a0d 0d0a 2323 2320 436f 6e76  ge......### Conv
-00000950: 6572 7465 720d 0d0a 0d0d 0a60 436f 6e76  erter......`Conv
-00000960: 6572 7465 7260 2063 6c61 7373 2074 7261  erter` class tra
-00000970: 6e73 6c69 7465 7261 7465 7320 7468 6520  nsliterates the 
-00000980: 4368 696e 6573 6520 6368 6172 6163 7465  Chinese characte
-00000990: 7273 2074 6f20 7468 6520 6368 6f73 656e  rs to the chosen
-000009a0: 2074 7261 6e73 6c69 7465 7261 7469 6f6e   transliteration
-000009b0: 2073 7973 7465 6d20 7769 7468 2070 6172   system with par
-000009c0: 616d 6574 6572 7320 7370 6563 6966 6965  ameters specifie
-000009d0: 6420 6279 2074 6865 2064 6576 656c 6f70  d by the develop
-000009e0: 6572 2e20 576f 726b 7320 666f 7220 626f  er. Works for bo
-000009f0: 7468 2054 7261 6469 7469 6f6e 616c 2061  th Traditional a
-00000a00: 6e64 2053 696d 706c 6966 6965 6420 6368  nd Simplified ch
-00000a10: 6172 6163 7465 7273 2e0d 0d0a 0d0d 0a60  aracters.......`
-00000a20: 6060 7079 7468 6f6e 0d0d 0a23 2063 6f6e  ``python...# con
-00000a30: 7374 7275 6374 6f72 0d0d 0a63 203d 2043  structor...c = C
-00000a40: 6f6e 7665 7274 6572 2873 7973 7465 6d2c  onverter(system,
-00000a50: 2064 6961 6c65 6374 2c20 666f 726d 6174   dialect, format
-00000a60: 2c20 6465 6c69 6d69 7465 722c 2073 616e  , delimiter, san
-00000a70: 6468 692c 2070 756e 6374 7561 7469 6f6e  dhi, punctuation
-00000a80: 290d 0d0a 0d0d 0a23 2074 7261 6e73 6c69  )......# transli
-00000a90: 7465 7261 7465 2043 6869 6e65 7365 2063  terate Chinese c
-00000aa0: 6861 7261 6374 6572 730d 0d0a 632e 6765  haracters...c.ge
-00000ab0: 7428 696e 7075 7429 0d0d 0a0d 0d0a 2320  t(input)......# 
-00000ac0: 636f 6e76 6572 7420 5369 6d70 6c69 6669  convert Simplifi
-00000ad0: 6564 2043 6869 6e65 7365 2063 6861 7261  ed Chinese chara
-00000ae0: 6374 6572 7320 746f 2054 7261 6469 7469  cters to Traditi
-00000af0: 6f6e 616c 2043 6869 6e65 7365 2043 6861  onal Chinese Cha
-00000b00: 7261 6374 6572 730d 0d0a 632e 746f 5f74  racters...c.to_t
-00000b10: 7261 6469 7469 6f6e 616c 2869 6e70 7574  raditional(input
-00000b20: 290d 0d0a 6060 600d 0d0a 0d0d 0a23 2323  )...```......###
-00000b30: 2320 5379 7374 656d 0d0d 0a0d 0d0a 6073  # System......`s
-00000b40: 7973 7465 6d60 2053 7472 696e 6720 2d20  ystem` String - 
-00000b50: 7379 7374 656d 206f 6620 7472 616e 736c  system of transl
-00000b60: 6974 6572 6174 696f 6e2e 0d0d 0a0d 0d0a  iteration.......
-00000b70: 2a20 6054 6169 6c6f 6020 2864 6566 6175  * `Tailo` (defau
-00000b80: 6c74 2920 2d20 5b54 c3a2 692d 75c3 a26e  lt) - [T..i-u..n
-00000b90: 204c c3b4 2d6d c3a1 2d6a c4ab 2050 6869   L..-m..-j.. Phi
-00000ba0: 6e67 2d69 6d20 486f 6e67 2dc3 a06e 5d5b  ng-im Hong-..n][
-00000bb0: 7461 696c 6f2d 7769 6b69 5d0d 0d0a 2a20  tailo-wiki]...* 
-00000bc0: 6050 4f4a 6020 2d20 5b50 65cc 8d68 2dc5  `POJ` - [Pe..h-.
-00000bd0: 8d65 2d6a c4ab 5d5b 706f 6a2d 7769 6b69  .e-j..][poj-wiki
-00000be0: 5d0d 0d0a 2a20 605a 6875 7969 6e60 202d  ]...* `Zhuyin` -
-00000bf0: 205b 5461 6977 616e 6573 6520 5068 6f6e   [Taiwanese Phon
-00000c00: 6574 6963 2053 796d 626f 6c73 5d5b 7a68  etic Symbols][zh
-00000c10: 7579 696e 2d77 696b 695d 0d0d 0a2a 2060  uyin-wiki]...* `
-00000c20: 544c 5041 6020 2d20 5b54 6169 7761 6e65  TLPA` - [Taiwane
-00000c30: 7365 204c 616e 6775 6167 6520 5068 6f6e  se Language Phon
-00000c40: 6574 6963 2041 6c70 6861 6265 745d 5b74  etic Alphabet][t
-00000c50: 6c70 612d 7769 6b69 5d0d 0d0a 2a20 6050  lpa-wiki]...* `P
-00000c60: 696e 6779 696d 6020 2d20 5b42 62c3 a16e  ingyim` - [Bb..n
-00000c70: 6cc3 a16d 2055 c493 2050 c3ac 6e67 79c4  l..m U.. P..ngy.
-00000c80: ab6d 2048 c58d 6e67 27c3 a06e 5d5b 7069  .m H..ng'..n][pi
-00000c90: 6e67 7969 6d2d 7769 6b69 5d0d 0d0a 2a20  ngyim-wiki]...* 
-00000ca0: 6054 6f6e 6769 6f6e 6760 202d 205b 4461  `Tongiong` - [Da
-00000cb0: c4ab 2d67 68c3 ae20 54c5 8d6e 672d 69c5  ..-gh.. T..ng-i.
-00000cc0: 8d6e 6720 50c4 ab6e 672d 696d 5d5b 746f  .ng P..ng-im][to
-00000cd0: 6e67 696f 6e67 2d77 696b 695d 0d0d 0a0d  ngiong-wiki]....
-00000ce0: 0d0a 7c20 7465 7874 207c 2054 6169 6c6f  ..| text | Tailo
-00000cf0: 2020 207c 2050 4f4a 2020 2020 207c 205a     | POJ     | Z
-00000d00: 6875 7969 6e20 2020 2020 207c 2054 4c50  huyin      | TLP
-00000d10: 4120 2020 2020 207c 2050 696e 6779 696d  A      | Pingyim
-00000d20: 207c 2054 6f6e 6769 6f6e 6720 7c0d 0d0a   | Tongiong |...
-00000d30: 7c2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  |------|--------
-00000d40: 2d7c 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -|---------|----
-00000d50: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
-00000d60: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d7c  -----|---------|
-00000d70: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d 0d0a 7c20  ----------|...| 
-00000d80: e887 bae7 81a3 207c 2054 c3a2 692d 75c3  ...... | T..i-u.
-00000d90: a26e 207c 2054 c3a2 692d 6fc3 a26e 207c  .n | T..i-o..n |
-00000da0: 20e3 8489 e384 9ecb 8a20 e384 a8e3 84a2   ........ ......
-00000db0: cb8a 207c 2054 6169 3520 7561 6e35 207c  .. | Tai5 uan5 |
-00000dc0: 2044 c3a1 6977 c3a1 6e20 207c 2054 c481   D..iw..n  | T..
-00000dd0: 692d 75c7 8e6e 2020 7c0d 0d0a 0d0d 0a0d  i-u..n  |.......
-00000de0: 0d0a 2323 2323 2044 6961 6c65 6374 0d0d  ..#### Dialect..
-00000df0: 0a0d 0d0a 6064 6961 6c65 6374 6020 5374  ....`dialect` St
-00000e00: 7269 6e67 202d 2070 7265 6665 7272 6564  ring - preferred
-00000e10: 2070 726f 6e75 6e63 6961 7469 6f6e 2e0d   pronunciation..
-00000e20: 0d0a 0d0d 0a2a 2060 736f 7574 6860 2028  .....* `south` (
-00000e30: 6465 6661 756c 7429 202d 205b 5a68 616e  default) - [Zhan
-00000e40: 677a 686f 755d 5b7a 6861 6e67 7a68 6f75  gzhou][zhangzhou
-00000e50: 2d77 696b 695d 2d6c 6561 6e69 6e67 2070  -wiki]-leaning p
-00000e60: 726f 6e75 6e63 6961 7469 6f6e 0d0d 0a2a  ronunciation...*
-00000e70: 2060 6e6f 7274 6860 202d 205b 5175 616e   `north` - [Quan
-00000e80: 7a68 6f75 5d5b 7175 616e 7a68 6f75 2d77  zhou][quanzhou-w
-00000e90: 696b 695d 2d6c 6561 6e69 6e67 2070 726f  iki]-leaning pro
-00000ea0: 6e75 6e63 6961 7469 6f6e 0d0d 0a0d 0d0a  nunciation......
-00000eb0: 7c20 7465 7874 2020 207c 2073 6f75 7468  | text   | south
-00000ec0: 2020 2020 2020 2020 207c 206e 6f72 7468           | north
-00000ed0: 2020 2020 2020 2020 207c 0d0d 0a7c 2d2d           |...|--
-00000ee0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000ef0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000f00: 2d2d 2d2d 2d2d 7c0d 0d0a 7c20 e4ba 94e6  ------|...| ....
-00000f10: 9c88 e7af 8020 7c20 47c5 8d6f 2d67 7565  ..... | G..o-gue
-00000f20: cc8d 682d 7473 6568 207c 2047 c58d 6f2d  ..h-tseh | G..o-
-00000f30: 6765 cc8d 682d 7473 7565 6820 7c0d 0d0a  ge..h-tsueh |...
-00000f40: 0d0d 0a0d 0d0a 2323 2323 2046 6f72 6d61  ......#### Forma
-00000f50: 740d 0d0a 0d0d 0a60 666f 726d 6174 6020  t......`format` 
-00000f60: 5374 7269 6e67 202d 2066 6f72 6d61 7420  String - format 
-00000f70: 696e 2077 6869 6368 2074 6f6e 6573 2077  in which tones w
-00000f80: 696c 6c20 6265 2072 6570 7265 7365 6e74  ill be represent
-00000f90: 6564 2069 6e20 7468 6520 636f 6e76 6572  ed in the conver
-00000fa0: 7465 6420 7365 6e74 656e 6365 2e0d 0d0a  ted sentence....
-00000fb0: 0d0d 0a2a 2060 6d61 726b 6020 2864 6566  ...* `mark` (def
-00000fc0: 6175 6c74 2920 2d20 7573 6573 2064 6961  ault) - uses dia
-00000fd0: 6372 6974 6963 7320 666f 7220 6561 6368  critics for each
-00000fe0: 2073 796c 6c61 626c 652e 204e 6f74 2061   syllable. Not a
-00000ff0: 7661 696c 6162 6c65 2066 6f72 2054 4c50  vailable for TLP
-00001000: 412e 0d0d 0a2a 2060 6e75 6d62 6572 6020  A....* `number` 
-00001010: 2d20 6164 6420 6120 6e75 6d62 6572 2077  - add a number w
-00001020: 6869 6368 2072 6570 7265 7365 6e74 7320  hich represents 
-00001030: 7468 6520 746f 6e65 2061 7420 7468 6520  the tone at the 
-00001040: 656e 6420 6f66 2074 6865 2073 796c 6c61  end of the sylla
-00001050: 626c 650d 0d0a 2a20 6073 7472 6970 6020  ble...* `strip` 
-00001060: 2d20 7265 6d6f 7665 7320 616e 7920 746f  - removes any to
-00001070: 6e65 206d 6172 6b69 6e67 0d0d 0a0d 0d0a  ne marking......
-00001080: 7c20 7465 7874 207c 206d 6172 6b20 2020  | text | mark   
-00001090: 207c 206e 756d 6265 7220 2020 207c 2073   | number    | s
-000010a0: 7472 6970 2020 207c 0d0d 0a7c 2d2d 2d2d  trip   |...|----
-000010b0: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  --|---------|---
-000010c0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-000010d0: 2d2d 7c0d 0d0a 7c20 e887 bae7 81a3 207c  --|...| ...... |
-000010e0: 2054 c3a2 692d 75c3 a26e 207c 2054 6169   T..i-u..n | Tai
-000010f0: 352d 7561 6e35 207c 2054 6169 2d75 616e  5-uan5 | Tai-uan
-00001100: 207c 0d0d 0a0d 0d0a 0d0d 0a23 2323 2320   |.........#### 
-00001110: 4465 6c69 6d69 7465 720d 0d0a 0d0d 0a60  Delimiter......`
-00001120: 6465 6c69 6d69 7465 7260 2053 7472 696e  delimiter` Strin
-00001130: 6720 2d20 7365 7473 2074 6865 2064 656c  g - sets the del
-00001140: 696d 6974 6572 2063 6861 7261 6374 6572  imiter character
-00001150: 2074 6861 7420 7769 6c6c 2062 6520 706c   that will be pl
-00001160: 6163 6564 2069 6e20 6265 7477 6565 6e20  aced in between 
-00001170: 7379 6c6c 6162 6c65 7320 6f66 2061 2077  syllables of a w
-00001180: 6f72 642e 0d0d 0a0d 0d0a 4465 6661 756c  ord.......Defaul
-00001190: 7420 7661 6c75 6520 6465 7065 6e64 7320  t value depends 
-000011a0: 6f6e 2074 6865 2063 686f 7365 6e20 6073  on the chosen `s
-000011b0: 7973 7465 6d60 3a0d 0d0a 0d0d 0a2a 2060  ystem`:......* `
-000011c0: 272d 2760 202d 2066 6f72 2060 5461 696c  '-'` - for `Tail
-000011d0: 6f60 2c20 6050 4f4a 602c 2060 546f 6e67  o`, `POJ`, `Tong
-000011e0: 696f 6e67 600d 0d0a 2a20 6027 2760 202d  iong`...* `''` -
-000011f0: 2066 6f72 2060 5069 6e67 7969 6d60 0d0d   for `Pingyim`..
-00001200: 0a2a 2060 2720 2760 202d 2066 6f72 2060  .* `' '` - for `
-00001210: 5a68 7579 696e 602c 2060 544c 5041 600d  Zhuyin`, `TLPA`.
-00001220: 0d0a 0d0d 0a7c 2074 6578 7420 7c20 272d  .....| text | '-
-00001230: 2720 2020 2020 7c20 2727 2020 2020 207c  '     | ''     |
-00001240: 2027 2027 2020 2020 207c 0d0d 0a7c 2d2d   ' '     |...|--
-00001250: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d  ----|---------|-
-00001260: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00001270: 2d7c 0d0d 0a7c 20e8 87ba e781 a320 7c20  -|...| ...... | 
-00001280: 54c3 a269 2d75 c3a2 6e20 7c20 54c3 a269  T..i-u..n | T..i
-00001290: 75c3 a26e 207c 2054 c3a2 6920 75c3 a26e  u..n | T..i u..n
-000012a0: 207c 0d0d 0a0d 0d0a 0d0d 0a23 2323 2320   |.........#### 
-000012b0: 5361 6e64 6869 0d0d 0a0d 0d0a 6073 616e  Sandhi......`san
-000012c0: 6468 6960 2042 6f6f 6c65 616e 202d 2061  dhi` Boolean - a
-000012d0: 7070 6c69 6573 2074 6865 205b 7361 6e64  pplies the [sand
-000012e0: 6869 2072 756c 6573 206f 6620 5461 6977  hi rules of Taiw
-000012f0: 616e 6573 6520 486f 6b6b 6965 6e5d 5b73  anese Hokkien][s
-00001300: 616e 6468 692d 7769 6b69 5d20 746f 2073  andhi-wiki] to s
-00001310: 796c 6c61 626c 6573 206f 6620 6120 7369  yllables of a si
-00001320: 6e67 6c65 2077 6f72 642e 0d0d 0a0d 0d0a  ngle word.......
-00001330: 4465 6661 756c 7420 7661 6c75 6520 6465  Default value de
-00001340: 7065 6e64 7320 6f6e 2074 6865 2063 686f  pends on the cho
-00001350: 7365 6e20 6073 7973 7465 6d60 3a0d 0d0a  sen `system`:...
-00001360: 0d0d 0a2a 2060 5472 7565 6020 2d20 666f  ...* `True` - fo
-00001370: 7220 6054 6f6e 6769 6f6e 6760 0d0d 0a2a  r `Tongiong`...*
-00001380: 2060 4661 6c73 6560 202d 2066 6f72 2060   `False` - for `
-00001390: 5461 696c 6f60 2c20 6050 4f4a 602c 2060  Tailo`, `POJ`, `
-000013a0: 5a68 7579 696e 602c 2060 544c 5041 602c  Zhuyin`, `TLPA`,
-000013b0: 2060 5069 6e67 7969 6d60 0d0d 0a0d 0d0a   `Pingyim`......
-000013c0: 7c20 7465 7874 2020 2020 207c 2046 616c  | text     | Fal
-000013d0: 7365 2020 2020 2020 2020 7c20 5472 7565  se        | True
-000013e0: 2020 2020 2020 2020 207c 0d0d 0a7c 2d2d           |...|--
-000013f0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00001400: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00001410: 2d2d 2d2d 2d2d 7c0d 0d0a 7c20 e882 b2e5  ------|...| ....
-00001420: 9ba1 e4bb 94e6 ad8c 207c 2049 6f2d 67c3  ........ | Io-g.
-00001430: ad6e 2dc3 a12d 6b75 6120 7c20 49c5 8d2d  .n-..-kua | I..-
-00001440: 6769 6e2d 612d 6b75 6120 7c0d 0d0a 0d0d  gin-a-kua |.....
-00001450: 0a53 616e 6468 6920 7275 6c65 7320 616c  .Sandhi rules al
-00001460: 736f 2063 6861 6e67 6520 6465 7065 6e64  so change depend
-00001470: 696e 6720 6f6e 2074 6865 2064 6961 6c65  ing on the diale
-00001480: 6374 2063 686f 7365 6e2e 0d0d 0a0d 0d0a  ct chosen.......
-00001490: 7c20 7465 7874 207c 206e 6f20 7361 6e64  | text | no sand
-000014a0: 6869 207c 2073 6f75 7468 2020 207c 206e  hi | south   | n
-000014b0: 6f72 7468 2020 207c 0d0d 0a7c 2d2d 2d2d  orth   |...|----
-000014c0: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --|-----------|-
-000014d0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-000014e0: 2d2d 7c0d 0d0a 7c20 e887 bae7 81a3 207c  --|...| ...... |
-000014f0: 2054 c3a2 692d 75c3 a26e 2020 207c 2054   T..i-u..n   | T
-00001500: c481 692d 75c3 a26e 207c 2054 c3a0 692d  ..i-u..n | T..i-
-00001510: 75c3 a26e 207c 0d0d 0a0d 0d0a 4e6f 7465  u..n |......Note
-00001520: 2074 6861 7420 7468 6520 6675 6e63 7469   that the functi
-00001530: 6f6e 2069 7320 6469 6666 6572 656e 7420  on is different 
-00001540: 6672 6f6d 2072 6561 6c20 7361 6e64 6869  from real sandhi
-00001550: 2072 756c 6573 2c20 7768 6572 6520 6368   rules, where ch
-00001560: 616e 6765 7320 6172 6520 6170 706c 6965  anges are applie
-00001570: 6420 746f 2065 7665 7279 2073 696e 676c  d to every singl
-00001580: 6520 7379 6c6c 6162 6c65 206f 6620 7468  e syllable of th
-00001590: 6520 7365 6e74 656e 6365 2c20 6e6f 7420  e sentence, not 
-000015a0: 6a75 7374 2073 696e 676c 6520 776f 7264  just single word
-000015b0: 732e 0d0d 0a0d 0d0a 2d20 2a2a 5461 6962  s.......- **Taib
-000015c0: 756e 2773 2073 616e 6468 6920 7275 6c65  un's sandhi rule
-000015d0: 732a 2a3a 2054 68c3 a169 2d6b 686f 6e67  s**: Th..i-khong
-000015e0: 2070 c4ab 6e67 2d69 c3ba 2c20 6cc3 ad6e   p..ng-i.., l..n
-000015f0: 2068 c3b3 2120 4cc3 ad6e 2074 7369 c3a0   h..! L..n tsi..
-00001600: 2d70 c3a1 2062 75c4 933f 0d0d 0a2d 202a  -p.. bu..?...- *
-00001610: 2a41 6374 7561 6c20 7361 6e64 6869 2072  *Actual sandhi r
-00001620: 756c 6573 2a2a 3a20 5468 c3a1 692d 6b68  ules**: Th..i-kh
-00001630: c58d 6e67 2070 c4ab 6e67 2d69 c3ba 2c20  ..ng p..ng-i.., 
-00001640: 6c69 6e20 68c3 b321 204c 696e 2074 7369  lin h..! Lin tsi
-00001650: c3a0 2d70 6120 6275 c493 3f0d 0d0a 0d0d  ..-pa bu..?.....
-00001660: 0a0d 0d0a 2323 2323 2050 756e 6374 7561  ....#### Punctua
-00001670: 7469 6f6e 0d0d 0a0d 0d0a 6070 756e 6374  tion......`punct
-00001680: 7561 7469 6f6e 6020 5374 7269 6e67 0d0d  uation` String..
-00001690: 0a0d 0d0a 2a20 6066 6f72 6d61 7460 2028  ....* `format` (
-000016a0: 6465 6661 756c 7429 202d 2063 6f6e 7665  default) - conve
-000016b0: 7274 7320 4368 696e 6573 652d 7374 796c  rts Chinese-styl
-000016c0: 6520 7075 6e63 7475 6174 696f 6e20 746f  e punctuation to
-000016d0: 204c 6174 696e 2d73 7479 6c65 2070 756e   Latin-style pun
-000016e0: 6374 7561 7469 6f6e 2061 6e64 2063 6170  ctuation and cap
-000016f0: 6974 616c 6973 6573 2077 6f72 6473 2061  italises words a
-00001700: 7420 7468 6520 6265 6769 6e6e 696e 6720  t the beginning 
-00001710: 6f66 2065 6163 6820 7365 6e74 656e 6365  of each sentence
-00001720: 2e0d 0d0a 2a20 606e 6f6e 6560 202d 2070  ....* `none` - p
-00001730: 7265 7365 7276 6573 2043 6869 6e65 7365  reserves Chinese
-00001740: 2d73 7479 6c65 2070 756e 6374 7561 7469  -style punctuati
-00001750: 6f6e 2061 6e64 2064 6f65 736e 2774 2063  on and doesn't c
-00001760: 6170 6974 616c 6973 6520 776f 7264 7320  apitalise words 
-00001770: 6174 2074 6865 2062 6567 696e 6e69 6e67  at the beginning
-00001780: 206f 6620 6e65 7720 7365 6e74 656e 6365   of new sentence
-00001790: 732e 0d0d 0a0d 0d0a 7c20 7465 7874 207c  s.......| text |
-000017a0: 2066 6f72 6d61 7420 7c20 6e6f 6e65 207c   format | none |
-000017b0: 0d0d 0a7c 2d7c 2d7c 2d7c 0d0d 0a7c 20e9  ...|-|-|-|...| .
-000017c0: 8099 e698 afe8 87ba e58d 97ef bc8c e7b0  ................
-000017d0: a1e7 a8b1 e380 8ce5 8d97 e380 8def bc88  ................
-000017e0: e799 bde8 a9b1 e5ad 97ef bc9a 54c3 a269  ............T..i
-000017f0: 2d6c c3a2 6def bc9b e6b3 a8e9 9fb3 e7ac  -l..m...........
-00001800: a6e8 999f efbc 9ae3 848a e384 9ecb 8a20  ............... 
-00001810: e384 8be3 84a2 cb8a efbc 8ce5 9c8b e8aa  ................
-00001820: 9eef bc9a 54c3 a169 6ec3 a16e efbc 89e3  ....T..in..n....
-00001830: 8082 207c 2054 7365 2073 c4ab 2054 c3a2  .. | Tse s.. T..
-00001840: 692d 6cc3 a26d 2c20 6bc3 a16e 2d74 7368  i-l..m, k..n-tsh
-00001850: 696e 6720 226c c3a2 6d22 2028 5065 cc8d  ing "l..m" (Pe..
-00001860: 682d 75c4 932d 6ac4 ab3a 2054 c3a2 692d  h-u..-j..: T..i-
-00001870: 6cc3 a26d 3b20 7473 c3b9 2d69 6d20 68c3  l..m; ts..-im h.
-00001880: bb2d 68c5 8d3a 20e3 848a e384 9ecb 8a20  .-h..: ........ 
-00001890: e384 8be3 84a2 cb8a 2c20 6b6f 6b2d 67c3  ........, kok-g.
-000018a0: ad3a 2054 c3a1 696e c3a1 6e29 2e20 7c20  .: T..in..n). | 
-000018b0: 7473 6520 73c4 ab20 54c3 a269 2d6c c3a2  tse s.. T..i-l..
-000018c0: 6def bc8c 6bc3 a16e 2d74 7368 696e 67e3  m...k..n-tshing.
-000018d0: 808c 6cc3 a26d e380 8def bc88 5065 cc8d  ..l..m......Pe..
-000018e0: 682d 75c4 932d 6ac4 abef bc9a 54c3 a269  h-u..-j.....T..i
-000018f0: 2d6c c3a2 6def bc9b 7473 c3b9 2d69 6d20  -l..m...ts..-im 
-00001900: 68c3 bb2d 68c5 8def bc9a e384 8ae3 849e  h..-h...........
-00001910: cb8a 20e3 848b e384 a2cb 8aef bc8c 6b6f  .. ...........ko
-00001920: 6b2d 67c3 adef bc9a 54c3 a169 6ec3 a16e  k-g.....T..in..n
-00001930: efbc 89e3 8082 207c 0d0d 0a0d 0d0a 2323  ...... |......##
-00001940: 2320 546f 6b65 6e69 7365 720d 0d0a 0d0d  # Tokeniser.....
-00001950: 0a60 546f 6b65 6e69 7365 7260 2063 6c61  .`Tokeniser` cla
-00001960: 7373 2070 6572 666f 726d 7320 5b4e 4c54  ss performs [NLT
-00001970: 4b20 776f 7264 7075 6e63 745f 746f 6b65  K wordpunct_toke
-00001980: 6e69 7a65 5d5b 6e6c 746b 2d74 6f6b 656e  nize][nltk-token
-00001990: 697a 655d 2d6c 696b 6520 746f 6b65 6e69  ize]-like tokeni
-000019a0: 7361 7469 6f6e 206f 6620 6120 5461 6977  sation of a Taiw
-000019b0: 616e 6573 6520 486f 6b6b 6965 6e20 7365  anese Hokkien se
-000019c0: 6e74 656e 6365 2e0d 0d0a 0d0d 0a60 6060  ntence.......```
-000019d0: 7079 7468 6f6e 0d0d 0a23 2063 6f6e 7374  python...# const
-000019e0: 7275 6374 6f72 0d0d 0a74 203d 2054 6f6b  ructor...t = Tok
-000019f0: 656e 6973 6572 2829 0d0d 0a0d 0d0a 2320  eniser()......# 
-00001a00: 746f 6b65 6e69 7365 2054 6169 7761 6e65  tokenise Taiwane
-00001a10: 7365 2048 6f6b 6b69 656e 2073 656e 7465  se Hokkien sente
-00001a20: 6e63 650d 0d0a 742e 746f 6b65 6e69 7365  nce...t.tokenise
-00001a30: 2869 6e70 7574 290d 0d0a 6060 600d 0d0a  (input)...```...
-00001a40: 0d0d 0a0d 0d0a 3c21 2d2d 2045 5841 4d50  ......<!-- EXAMP
-00001a50: 4c45 202d 2d3e 0d0d 0a23 2320 4578 616d  LE -->...## Exam
-00001a60: 706c 650d 0d0a 0d0d 0a60 6060 7079 7468  ple......```pyth
-00001a70: 6f6e 0d0d 0a66 726f 6d20 7461 6962 756e  on...from taibun
-00001a80: 2069 6d70 6f72 7420 436f 6e76 6572 7465   import Converte
-00001a90: 722c 2054 6f6b 656e 6973 6572 0d0d 0a0d  r, Tokeniser....
-00001aa0: 0d0a 2320 5379 7374 656d 0d0d 0a63 203d  ..# System...c =
-00001ab0: 2043 6f6e 7665 7274 6572 2829 2023 2054   Converter() # T
-00001ac0: 6169 6c6f 2073 7973 7465 6d20 6465 6661  ailo system defa
-00001ad0: 756c 740d 0d0a 632e 6765 7428 27e5 8588  ult...c.get('...
-00001ae0: e794 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6  ................
-00001af0: 81ac e681 ace8 81bd e380 8227 290d 0d0a  ...........')...
-00001b00: 3e3e 2053 6961 6e2d 7369 6e6e 206b c3b3  >> Sian-sinn k..
-00001b10: 6e67 2c20 6861 cc8d 6b2d 7369 6e67 2074  ng, ha..k-sing t
-00001b20: 69c4 816d 2d74 69c4 816d 2074 6869 616e  i..m-ti..m thian
-00001b30: 6e2e 0d0d 0a0d 0d0a 6320 3d20 436f 6e76  n.......c = Conv
-00001b40: 6572 7465 7228 7379 7374 656d 3d27 5a68  erter(system='Zh
-00001b50: 7579 696e 2729 0d0d 0a63 2e67 6574 2827  uyin')...c.get('
-00001b60: e585 88e7 949f e8ac 9bef bc8c e5ad b8e7  ................
-00001b70: 949f e681 ace6 81ac e881 bde3 8082 2729  ..............')
-00001b80: 0d0d 0a3e 3e20 e384 92e3 84a7 e384 a220  ...>> ......... 
-00001b90: e384 92e3 86aa 20e3 848d e386 b2cb 8b2c  ...... ........,
-00001ba0: 20e3 848f e384 9ae3 848d 20e3 8492 e384   ......... .....
-00001bb0: a7e3 84a5 20e3 8489 e384 a7e3 86b0 cbab  .... ...........
-00001bc0: 20e3 8489 e384 a7e3 86b0 cbab 20e3 848a   ........... ...
-00001bd0: e384 a7e3 86a9 2e0d 0d0a 0d0d 0a23 2044  .............# D
-00001be0: 6961 6c65 6374 0d0d 0a63 203d 2043 6f6e  ialect...c = Con
-00001bf0: 7665 7274 6572 2829 2023 2073 6f75 7468  verter() # south
-00001c00: 2064 6961 6c65 6374 2064 6566 6175 6c74   dialect default
-00001c10: 0d0d 0a63 2e67 6574 2822 e688 91e6 acb2  ...c.get("......
-00001c20: e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0d  ............")..
-00001c30: 0a3e 3e20 4775 c3a1 2062 6568 20c4 ab6e  .>> Gu.. beh ..n
-00001c40: 6720 74c4 ab20 7473 6961 cc8d 6820 68c3  g t.. tsia..h h.
-00001c50: ae0d 0d0a 0d0d 0a63 203d 2043 6f6e 7665  .......c = Conve
-00001c60: 7274 6572 2864 6961 6c65 6374 3d27 6e6f  rter(dialect='no
-00001c70: 7274 6827 290d 0d0a 632e 6765 7428 22e6  rth')...c.get(".
-00001c80: 8891 e6ac b2e7 94a8 e7ae b8e9 a39f e9ad  ................
-00001c90: 9a22 290d 0d0a 3e3e 2047 75c3 a120 6275  .")...>> Gu.. bu
-00001ca0: 6568 20c4 ab6e 6720 74c5 ab20 7473 6961  eh ..ng t.. tsia
-00001cb0: cc8d 6820 68c3 bb0d 0d0a 0d0d 0a23 2046  ..h h........# F
-00001cc0: 6f72 6d61 740d 0d0a 6320 3d20 436f 6e76  ormat...c = Conv
-00001cd0: 6572 7465 7228 2920 2320 666f 7220 5461  erter() # for Ta
-00001ce0: 696c 6f2c 206d 6172 6b20 6279 2064 6566  ilo, mark by def
-00001cf0: 6175 6c74 0d0d 0a63 2e67 6574 2822 e794  ault...c.get("..
-00001d00: 9fe6 97a5 e5bf abe6 a882 2229 0d0d 0a3e  ..........")...>
-00001d10: 3e20 5365 6e6e 2d6a 69cc 8d74 206b 6875  > Senn-ji..t khu
-00001d20: c3a0 692d 6c6f cc8d 6b0d 0d0a 0d0d 0a63  ..i-lo..k......c
-00001d30: 203d 2043 6f6e 7665 7274 6572 2866 6f72   = Converter(for
-00001d40: 6d61 743d 276e 756d 6265 7227 290d 0d0a  mat='number')...
-00001d50: 632e 6765 7428 22e7 949f e697 a5e5 bfab  c.get(".........
-00001d60: e6a8 8222 290d 0d0a 3e3e 2053 656e 6e31  ...")...>> Senn1
-00001d70: 2d6a 6974 3820 6b68 7561 6933 2d6c 6f6b  -jit8 khuai3-lok
-00001d80: 380d 0d0a 0d0d 0a63 203d 2043 6f6e 7665  8......c = Conve
-00001d90: 7274 6572 2866 6f72 6d61 743d 2773 7472  rter(format='str
-00001da0: 6970 2729 0d0d 0a63 2e67 6574 2822 e794  ip')...c.get("..
-00001db0: 9fe6 97a5 e5bf abe6 a882 2229 0d0d 0a3e  ..........")...>
-00001dc0: 3e20 5365 6e6e 2d6a 6974 206b 6875 6169  > Senn-jit khuai
-00001dd0: 2d6c 6f6b 0d0d 0a0d 0d0a 2320 4465 6c69  -lok......# Deli
-00001de0: 6d69 7465 720d 0d0a 6320 3d20 436f 6e76  miter...c = Conv
-00001df0: 6572 7465 7228 6465 6c69 6d69 7465 723d  erter(delimiter=
-00001e00: 2727 290d 0d0a 632e 6765 7428 22e5 8588  '')...c.get("...
-00001e10: e794 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6  ................
-00001e20: 81ac e681 ace8 81bd e380 8222 290d 0d0a  ...........")...
-00001e30: 3e3e 2053 6961 6e73 696e 6e20 6bc3 b36e  >> Siansinn k..n
-00001e40: 672c 2068 61cc 8d6b 7369 6e67 2074 69c4  g, ha..ksing ti.
-00001e50: 816d 7469 c481 6d20 7468 6961 6e6e 2e0d  .mti..m thiann..
-00001e60: 0d0a 0d0d 0a63 203d 2043 6f6e 7665 7274  .....c = Convert
-00001e70: 6572 2873 7973 7465 6d3d 2750 696e 6779  er(system='Pingy
-00001e80: 696d 272c 2064 656c 696d 6974 6572 3d27  im', delimiter='
-00001e90: 2d27 290d 0d0a 632e 6765 7428 22e5 8588  -')...c.get("...
-00001ea0: e794 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6  ................
-00001eb0: 81ac e681 ace8 81bd e380 8222 290d 0d0a  ...........")...
-00001ec0: 3e3e 2053 69c4 816e 2d73 6ec4 ab20 67c7  >> Si..n-sn.. g.
-00001ed0: 926e 672c 2068 c3a1 672d 73c4 ab6e 6720  .ng, h..g-s..ng 
-00001ee0: 6469 c3a2 6d2d 6469 c3a2 6d20 7469 6ec4  di..m-di..m tin.
-00001ef0: 812e 0d0d 0a0d 0d0a 2320 5361 6e64 6869  ........# Sandhi
-00001f00: 0d0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
-00001f10: 2829 2023 2066 6f72 2054 6169 6c6f 2c20  () # for Tailo, 
-00001f20: 7361 6e64 6869 2046 616c 7365 2062 7920  sandhi False by 
-00001f30: 6465 6661 756c 740d 0d0a 632e 6765 7428  default...c.get(
-00001f40: 22e5 8d97 e8bf b4e9 90b5 e8b7 af22 290d  "............").
-00001f50: 0d0a 3e3e 204c c3a2 6d2d 6875 c3aa 2d74  ..>> L..m-hu..-t
-00001f60: 6869 682d 6cc5 8d6f 0d0d 0a0d 0d0a 6320  hih-l..o......c 
-00001f70: 3d20 436f 6e76 6572 7465 7228 7361 6e64  = Converter(sand
-00001f80: 6869 3d54 7275 6529 0d0d 0a63 2e67 6574  hi=True)...c.get
-00001f90: 2822 e58d 97e8 bfb4 e990 b5e8 b7af 2229  ("............")
-00001fa0: 0d0d 0a3e 3e20 4cc4 816d 2d68 75c4 932d  ...>> L..m-hu..-
-00001fb0: 7468 c3ad 2d6c c58d 6f0d 0d0a 0d0d 0a23  th..-l..o......#
-00001fc0: 2050 756e 6374 7561 7469 6f6e 0d0d 0a63   Punctuation...c
-00001fd0: 203d 2043 6f6e 7665 7274 6572 2829 2023   = Converter() #
-00001fe0: 2066 6f72 6d61 7420 7075 6e63 7475 6174   format punctuat
-00001ff0: 696f 6e20 6465 6661 756c 740d 0d0a 632e  ion default...c.
-00002000: 6765 7428 22e5 a4aa e7a9 bae6 9c8b e58f  get("...........
-00002010: 8bef bc8c e681 81e5 a5bd efbc 81e6 8181  ................
-00002020: e9a3 9fe9 a3bd e69c aaef bc9f 2229 0d0d  ............")..
-00002030: 0a3e 3e20 5468 c3a0 692d 6b68 6f6e 6720  .>> Th..i-khong 
-00002040: 70c3 ae6e 672d 69c3 ba2c 206c c3ad 6e20  p..ng-i.., l..n 
-00002050: 68c3 b321 204c c3ad 6e20 7473 6961 cc8d  h..! L..n tsia..
-00002060: 682d 70c3 a120 6275 c493 3f0d 0d0a 0d0d  h-p.. bu..?.....
-00002070: 0a63 203d 2043 6f6e 7665 7274 6572 2870  .c = Converter(p
-00002080: 756e 6374 7561 7469 6f6e 3d27 6e6f 6e65  unctuation='none
-00002090: 2729 0d0d 0a63 2e67 6574 2822 e5a4 aae7  ')...c.get("....
-000020a0: a9ba e69c 8be5 8f8b efbc 8ce6 8181 e5a5  ................
-000020b0: bdef bc81 e681 81e9 a39f e9a3 bde6 9caa  ................
-000020c0: efbc 9f22 290d 0d0a 3e3e 2074 68c3 a069  ...")...>> th..i
-000020d0: 2d6b 686f 6e67 2070 c3ae 6e67 2d69 c3ba  -khong p..ng-i..
-000020e0: efbc 8c6c c3ad 6e20 68c3 b3ef bc81 6cc3  ...l..n h.....l.
-000020f0: ad6e 2074 7369 61cc 8d68 2d70 c3a1 2062  .n tsia..h-p.. b
-00002100: 75c4 93ef bc9f 0d0d 0a0d 0d0a 0d0d 0a23  u..............#
-00002110: 2054 6f6b 656e 6973 6572 0d0d 0a74 203d   Tokeniser...t =
-00002120: 2054 6f6b 656e 6973 6572 2829 0d0d 0a74   Tokeniser()...t
-00002130: 2e74 6f6b 656e 6973 6528 22e5 a4aa e7a9  .tokenise(".....
-00002140: bae6 9c8b e58f 8bef bc8c e681 81e5 a5bd  ................
-00002150: efbc 81e6 8181 e9a3 9fe9 a3bd e69c aaef  ................
-00002160: bc9f 2229 0d0d 0a3e 3e20 5b27 e5a4 aae7  ..")...>> ['....
-00002170: a9ba 272c 2027 e69c 8be5 8f8b 272c 2027  ..', '......', '
-00002180: efbc 8c27 2c20 27e6 8181 272c 2027 e5a5  ...', '...', '..
-00002190: bd27 2c20 27ef bc81 272c 2027 e681 8127  .', '...', '...'
-000021a0: 2c20 27e9 a39f e9a3 bd27 2c20 27e6 9caa  , '......', '...
-000021b0: 272c 2027 efbc 9f27 5d0d 0d0a 6060 600d  ', '...']...```.
-000021c0: 0d0a 0d0d 0a0d 0d0a 3c21 2d2d 2044 4154  ........<!-- DAT
-000021d0: 4120 2d2d 3e0d 0d0a 2323 2044 6174 610d  A -->...## Data.
-000021e0: 0d0a 0d0d 0a2d 205b 4469 6374 696f 6e61  .....- [Dictiona
-000021f0: 7279 206f 6620 4672 6571 7565 6e74 6c79  ry of Frequently
-00002200: 2d55 7365 6420 5461 6977 616e 204d 696e  -Used Taiwan Min
-00002210: 6e61 6e5d 5b64 6963 7469 6f6e 6172 795d  nan][dictionary]
-00002220: 2028 7669 6120 5b6d 6f65 6469 6374 2d64   (via [moedict-d
-00002230: 6174 612d 7477 626c 675d 5b64 6963 7469  ata-twblg][dicti
-00002240: 6f6e 6172 792d 7669 615d 290d 0d0a 0d0d  onary-via]).....
-00002250: 0a0d 0d0a 3c21 2d2d 204c 4943 454e 4345  ....<!-- LICENCE
-00002260: 202d 2d3e 0d0d 0a23 2320 4c69 6365 6e63   -->...## Licenc
-00002270: 650d 0d0a 0d0d 0a42 6563 6175 7365 2054  e......Because T
-00002280: 6169 6275 6e20 6973 204d 4954 2d6c 6963  aibun is MIT-lic
-00002290: 656e 7365 642c 2061 6e79 2064 6576 656c  ensed, any devel
-000022a0: 6f70 6572 2063 616e 2065 7373 656e 7469  oper can essenti
-000022b0: 616c 6c79 2064 6f20 7768 6174 6576 6572  ally do whatever
-000022c0: 2074 6865 7920 7761 6e74 2077 6974 6820   they want with 
-000022d0: 6974 2061 7320 6c6f 6e67 2061 7320 7468  it as long as th
-000022e0: 6579 2069 6e63 6c75 6465 2074 6865 206f  ey include the o
-000022f0: 7269 6769 6e61 6c20 636f 7079 7269 6768  riginal copyrigh
-00002300: 7420 616e 6420 6c69 6365 6e63 6520 6e6f  t and licence no
-00002310: 7469 6365 2069 6e20 616e 7920 636f 7069  tice in any copi
-00002320: 6573 206f 6620 7468 6520 736f 7572 6365  es of the source
-00002330: 2063 6f64 652e 204e 6f74 652c 2074 6861   code. Note, tha
-00002340: 7420 7468 6520 6461 7461 2075 7365 6420  t the data used 
-00002350: 6279 2074 6865 2070 6163 6b61 6765 2069  by the package i
-00002360: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
-00002370: 2061 2064 6966 6665 7265 6e74 2063 6f70   a different cop
-00002380: 7972 6967 6874 2e0d 0d0a 0d0d 0a54 6865  yright.......The
-00002390: 2064 6174 6120 6973 206c 6963 656e 7365   data is license
-000023a0: 6420 756e 6465 7220 5b43 4320 4259 2d4e  d under [CC BY-N
-000023b0: 4420 332e 3020 5457 5d5b 6469 7374 696f  D 3.0 TW][distio
-000023c0: 6e61 7279 2d63 635d 0d0d 0a0d 0d0a 0d0d  nary-cc]........
-000023d0: 0a0d 0d0a 3c21 2d2d 204d 4152 4b44 4f57  ....<!-- MARKDOW
-000023e0: 4e20 4c49 4e4b 5320 2d2d 3e0d 0d0a 5b63  N LINKS -->...[c
-000023f0: 6f6e 7472 6962 7574 6f72 732d 6261 6467  ontributors-badg
-00002400: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
-00002410: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00002420: 622f 636f 6e74 7269 6275 746f 7273 2f61  b/contributors/a
-00002430: 6e64 7265 6968 6172 2f74 6169 6275 6e3f  ndreihar/taibun?
-00002440: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-00002450: 6467 650d 0d0a 5b63 6f6e 7472 6962 7574  dge...[contribut
-00002460: 6f72 735d 3a20 2375 7361 6765 0d0d 0a5b  ors]: #usage...[
-00002470: 7265 6c65 6173 652d 6261 6467 655d 3a20  release-badge]: 
-00002480: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00002490: 6c64 732e 696f 2f67 6974 6875 622f 762f  lds.io/github/v/
-000024a0: 7265 6c65 6173 652f 616e 6472 6569 6861  release/andreiha
-000024b0: 722f 7461 6962 756e 3f63 6f6c 6f72 3d33  r/taibun?color=3
-000024c0: 3836 3138 6326 7374 796c 653d 666f 722d  8618c&style=for-
-000024d0: 7468 652d 6261 6467 650d 0d0a 5b72 656c  the-badge...[rel
-000024e0: 6561 7365 5d3a 2068 7474 7073 3a2f 2f67  ease]: https://g
-000024f0: 6974 6875 622e 636f 6d2f 616e 6472 6569  ithub.com/andrei
-00002500: 6861 722f 7461 6962 756e 2f72 656c 6561  har/taibun/relea
-00002510: 7365 730d 0d0a 5b6c 6963 656e 6365 2d62  ses...[licence-b
-00002520: 6164 6765 5d3a 2068 7474 7073 3a2f 2f69  adge]: https://i
-00002530: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00002540: 7468 7562 2f6c 6963 656e 7365 2f61 6e64  thub/license/and
-00002550: 7265 6968 6172 2f74 6169 6275 6e2e 7376  reihar/taibun.sv
-00002560: 673f 636f 6c6f 723d 3030 3030 3030 2673  g?color=000000&s
-00002570: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
-00002580: 6765 0d0d 0a5b 6c69 6365 6e63 655d 3a20  ge...[licence]: 
-00002590: 4c49 4345 4e53 450d 0d0a 5b6c 696e 6b65  LICENSE...[linke
-000025a0: 6469 6e2d 6261 6467 655d 3a20 6874 7470  din-badge]: http
-000025b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000025c0: 696f 2f62 6164 6765 2f4c 696e 6b65 6449  io/badge/LinkedI
-000025d0: 6e2d 3030 3737 4235 3f73 7479 6c65 3d66  n-0077B5?style=f
-000025e0: 6f72 2d74 6865 2d62 6164 6765 266c 6f67  or-the-badge&log
-000025f0: 6f3d 6c69 6e6b 6564 696e 266c 6f67 6f43  o=linkedin&logoC
-00002600: 6f6c 6f72 3d77 6869 7465 0d0d 0a5b 6c69  olor=white...[li
-00002610: 6e6b 6564 696e 5d3a 2068 7474 7073 3a2f  nkedin]: https:/
-00002620: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
-00002630: 6d2f 696e 2f61 6e64 7265 692d 6861 7262  m/in/andrei-harb
-00002640: 6163 686f 762f 0d0d 0a0d 0d0a 5b70 7970  achov/......[pyp
-00002650: 695d 3a20 6874 7470 733a 2f2f 7079 7069  i]: https://pypi
-00002660: 2e6f 7267 2f70 726f 6a65 6374 2f74 6169  .org/project/tai
-00002670: 6275 6e0d 0d0a 5b62 7567 5d3a 2068 7474  bun...[bug]: htt
-00002680: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002690: 616e 6472 6569 6861 722f 7461 6962 756e  andreihar/taibun
-000026a0: 2f69 7373 7565 730d 0d0a 5b64 6963 7469  /issues...[dicti
-000026b0: 6f6e 6172 795d 3a20 6874 7470 733a 2f2f  onary]: https://
-000026c0: 7477 626c 672e 6469 6374 2e65 6475 2e74  twblg.dict.edu.t
-000026d0: 772f 686f 6c6f 6469 6374 5f6e 6577 2f0d  w/holodict_new/.
-000026e0: 0d0a 5b64 6963 7469 6f6e 6172 792d 7669  ..[dictionary-vi
-000026f0: 615d 3a20 6874 7470 733a 2f2f 6769 7468  a]: https://gith
-00002700: 7562 2e63 6f6d 2f67 3076 2f6d 6f65 6469  ub.com/g0v/moedi
-00002710: 6374 2d64 6174 612d 7477 626c 670d 0d0a  ct-data-twblg...
-00002720: 5b64 6973 7469 6f6e 6172 792d 6363 5d3a  [distionary-cc]:
-00002730: 2068 7474 7073 3a2f 2f63 7265 6174 6976   https://creativ
-00002740: 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963  ecommons.org/lic
-00002750: 656e 7365 732f 6279 2d6e 642f 332e 302f  enses/by-nd/3.0/
-00002760: 7477 2f64 6565 642e 656e 0d0d 0a0d 0d0a  tw/deed.en......
-00002770: 5b74 6169 6c6f 2d77 696b 695d 3a20 6874  [tailo-wiki]: ht
-00002780: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
-00002790: 6961 2e6f 7267 2f77 696b 692f 5425 4333  ia.org/wiki/T%C3
-000027a0: 2541 3269 2d75 2543 3325 4132 6e5f 4c25  %A2i-u%C3%A2n_L%
-000027b0: 4333 2542 342d 6d25 4333 2541 312d 6a25  C3%B4-m%C3%A1-j%
-000027c0: 4334 2541 425f 5068 696e 672d 696d 5f48  C4%AB_Phing-im_H
-000027d0: 6f6e 672d 2543 3325 4130 6e0d 0d0a 5b70  ong-%C3%A0n...[p
-000027e0: 6f6a 2d77 696b 695d 3a20 6874 7470 733a  oj-wiki]: https:
-000027f0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002800: 7267 2f77 696b 692f 5065 2543 4325 3844  rg/wiki/Pe%CC%8D
-00002810: 682d 2543 3525 3844 652d 6a25 4334 2541  h-%C5%8De-j%C4%A
-00002820: 420d 0d0a 5b7a 6875 7969 6e2d 7769 6b69  B...[zhuyin-wiki
-00002830: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
-00002840: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00002850: 2f54 6169 7761 6e65 7365 5f50 686f 6e65  /Taiwanese_Phone
-00002860: 7469 635f 5379 6d62 6f6c 730d 0d0a 5b74  tic_Symbols...[t
-00002870: 6c70 612d 7769 6b69 5d3a 2068 7474 7073  lpa-wiki]: https
-00002880: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00002890: 6f72 672f 7769 6b69 2f54 6169 7761 6e65  org/wiki/Taiwane
-000028a0: 7365 5f4c 616e 6775 6167 655f 5068 6f6e  se_Language_Phon
-000028b0: 6574 6963 5f41 6c70 6861 6265 740d 0d0a  etic_Alphabet...
-000028c0: 5b70 696e 6779 696d 2d77 696b 695d 3a20  [pingyim-wiki]: 
-000028d0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000028e0: 6564 6961 2e6f 7267 2f77 696b 692f 4262  edia.org/wiki/Bb
-000028f0: 2543 3325 4131 6e6c 2543 3325 4131 6d5f  %C3%A1nl%C3%A1m_
-00002900: 7025 4333 2541 436e 6779 2543 3425 4142  p%C3%ACngy%C4%AB
-00002910: 6d0d 0d0a 5b74 6f6e 6769 6f6e 672d 7769  m...[tongiong-wi
-00002920: 6b69 5d3a 2068 7474 7073 3a2f 2f65 6e2e  ki]: https://en.
-00002930: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-00002940: 6b69 2f44 6125 4334 2541 422d 6768 2543  ki/Da%C4%AB-gh%C
-00002950: 3325 4145 5f74 2543 3525 3844 6e67 2d69  3%AE_t%C5%8Dng-i
-00002960: 2543 3525 3844 6e67 5f70 2543 3425 4142  %C5%8Dng_p%C4%AB
-00002970: 6e67 2d69 6d0d 0d0a 5b7a 6861 6e67 7a68  ng-im...[zhangzh
-00002980: 6f75 2d77 696b 695d 3a20 6874 7470 733a  ou-wiki]: https:
-00002990: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-000029a0: 7267 2f77 696b 692f 5a68 616e 677a 686f  rg/wiki/Zhangzho
-000029b0: 755f 6469 616c 6563 7473 0d0d 0a5b 7175  u_dialects...[qu
-000029c0: 616e 7a68 6f75 2d77 696b 695d 3a20 6874  anzhou-wiki]: ht
-000029d0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
-000029e0: 6961 2e6f 7267 2f77 696b 692f 5175 616e  ia.org/wiki/Quan
-000029f0: 7a68 6f75 5f64 6961 6c65 6374 730d 0d0a  zhou_dialects...
-00002a00: 5b6e 6c74 6b2d 746f 6b65 6e69 7a65 5d3a  [nltk-tokenize]:
-00002a10: 2068 7474 7073 3a2f 2f6e 6c74 6b2e 6f72   https://nltk.or
-00002a20: 672f 6170 692f 6e6c 746b 2e74 6f6b 656e  g/api/nltk.token
-00002a30: 697a 652e 6874 6d6c 0d0d 0a5b 7361 6e64  ize.html...[sand
-00002a40: 6869 2d77 696b 695d 3a20 6874 7470 733a  hi-wiki]: https:
-00002a50: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002a60: 7267 2f77 696b 692f 5461 6977 616e 6573  rg/wiki/Taiwanes
-00002a70: 655f 486f 6b6b 6965 6e23 546f 6e65 2532  e_Hokkien#Tone%2
-00002a80: 3073 616e 6468 693a 7e3a 7465 7874 3d74  0sandhi:~:text=t
-00002a90: 686e 6725 4532 2539 4625 4139 2532 3028  hng%E2%9F%A9%20(
-00002aa0: 2532 3273 6f75 7025 3232 292e 2d2c 546f  %22soup%22).-,To
-00002ab0: 6e65 2532 3073 616e 6468 692c 2d25 3542  ne%20sandhi,-%5B
-00002ac0: 6564 6974 2535 440d 0a                   edit%5D..
+00000030: 696f 6e3a 2031 2e31 2e30 0d0a 5375 6d6d  ion: 1.1.0..Summ
+00000040: 6172 793a 2054 6169 7761 6e65 7365 2048  ary: Taiwanese H
+00000050: 6f6b 6b69 656e 2054 7261 6e73 6c69 7465  okkien Translite
+00000060: 7261 746f 7220 616e 6420 546f 6b65 6e69  rator and Tokeni
+00000070: 7365 720d 0a48 6f6d 652d 7061 6765 3a20  ser..Home-page: 
+00000080: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000090: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
+000000a0: 6275 6e0d 0a41 7574 686f 723a 2041 6e64  bun..Author: And
+000000b0: 7265 6920 4861 7262 6163 686f 760d 0a41  rei Harbachov..A
+000000c0: 7574 686f 722d 656d 6169 6c3a 2061 6e64  uthor-email: and
+000000d0: 7265 692e 6861 7262 6163 686f 7640 676d  rei.harbachov@gm
+000000e0: 6169 6c2e 636f 6d0d 0a4c 6963 656e 7365  ail.com..License
+000000f0: 3a20 4d49 540d 0a4b 6579 776f 7264 733a  : MIT..Keywords:
+00000100: 2070 7974 686f 6e2c 7461 6977 616e 2c74   python,taiwan,t
+00000110: 6169 7761 6e65 7365 2c74 6169 6769 2c68  aiwanese,taigi,h
+00000120: 6f6b 6b69 656e 2c72 6f6d 616e 697a 6174  okkien,romanizat
+00000130: 696f 6e2c 7472 616e 736c 6974 6572 6174  ion,transliterat
+00000140: 696f 6e2c 7472 616e 736c 6974 6572 6174  ion,transliterat
+00000150: 6f72 2c74 6f6b 656e 697a 6174 696f 6e2c  or,tokenization,
+00000160: 746f 6b65 6e69 7a65 720d 0a43 6c61 7373  tokenizer..Class
+00000170: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+00000180: 5465 7874 2050 726f 6365 7373 696e 6720  Text Processing 
+00000190: 3a3a 204c 696e 6775 6973 7469 630d 0a43  :: Linguistic..C
+000001a0: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
+000001b0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+000001c0: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
+000001d0: 5374 6162 6c65 0d0a 436c 6173 7369 6669  Stable..Classifi
+000001e0: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+000001f0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000200: 6572 730d 0a43 6c61 7373 6966 6965 723a  ers..Classifier:
+00000210: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000230: 3a3a 2033 0d0a 436c 6173 7369 6669 6572  :: 3..Classifier
+00000240: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000250: 656d 203a 3a20 556e 6978 0d0a 436c 6173  em :: Unix..Clas
+00000260: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+00000270: 6720 5379 7374 656d 203a 3a20 4d61 634f  g System :: MacO
+00000280: 5320 3a3a 204d 6163 4f53 2058 0d0a 436c  S :: MacOS X..Cl
+00000290: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+000002a0: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
+000002b0: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
+000002c0: 7773 0d0a 5265 7175 6972 6573 2d50 7974  ws..Requires-Pyt
+000002d0: 686f 6e3a 203e 3d33 2e38 0d0a 4465 7363  hon: >=3.8..Desc
+000002e0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+000002f0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000300: 6f77 6e0d 0a4c 6963 656e 7365 2d46 696c  own..License-Fil
+00000310: 653a 204c 4943 454e 5345 0d0a 0d0a 3c21  e: LICENSE....<!
+00000320: 2d2d 2050 524f 4a45 4354 204c 4f47 4f20  -- PROJECT LOGO 
+00000330: 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c 6469  -->..<br />..<di
+00000340: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00000350: 3e0d 0a20 200d 0a23 2054 6169 6275 6e0d  >..  ..# Taibun.
+00000360: 0a0d 0a0d 0a0d 0a3c 212d 2d20 5052 4f4a  .......<!-- PROJ
+00000370: 4543 5420 5348 4945 4c44 5320 2d2d 3e0d  ECT SHIELDS -->.
+00000380: 0a5b 215b 5465 7374 735d 5b74 6573 7473  .[![Tests][tests
+00000390: 2d62 6164 6765 5d5d 5b74 6573 7473 5d0d  -badge]][tests].
+000003a0: 0a5b 215b 436f 6e74 7269 6275 746f 7273  .[![Contributors
+000003b0: 5d5b 636f 6e74 7269 6275 746f 7273 2d62  ][contributors-b
+000003c0: 6164 6765 5d5d 5b63 6f6e 7472 6962 7574  adge]][contribut
+000003d0: 6f72 735d 0d0a 5b21 5b52 656c 6561 7365  ors]..[![Release
+000003e0: 5d5b 7265 6c65 6173 652d 6261 6467 655d  ][release-badge]
+000003f0: 5d5b 7265 6c65 6173 655d 0d0a 5b21 5b4c  ][release]..[![L
+00000400: 6963 656e 6365 5d5b 6c69 6365 6e63 652d  icence][licence-
+00000410: 6261 6467 655d 5d5b 6c69 6365 6e63 655d  badge]][licence]
+00000420: 0d0a 5b21 5b4c 696e 6b65 6449 6e5d 5b6c  ..[![LinkedIn][l
+00000430: 696e 6b65 6469 6e2d 6261 6467 655d 5d5b  inkedin-badge]][
+00000440: 6c69 6e6b 6564 696e 5d0d 0a0d 0a2a 2a54  linkedin]....**T
+00000450: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
+00000460: 2054 7261 6e73 6c69 7465 7261 746f 7220   Transliterator 
+00000470: 616e 6420 546f 6b65 6e69 7365 722a 2a0d  and Tokeniser**.
+00000480: 0a0d 0a49 7420 6861 7320 6d65 7468 6f64  ...It has method
+00000490: 7320 7468 6174 2061 6c6c 6f77 2074 6f20  s that allow to 
+000004a0: 6375 7374 6f6d 6973 6520 7472 616e 736c  customise transl
+000004b0: 6974 6572 6174 696f 6e20 616e 6420 7265  iteration and re
+000004c0: 7472 6965 7665 2061 6e79 206e 6563 6573  trieve any neces
+000004d0: 7361 7279 2069 6e66 6f72 6d61 7469 6f6e  sary information
+000004e0: 2061 626f 7574 2054 6169 7761 6e65 7365   about Taiwanese
+000004f0: 2048 6f6b 6b69 656e 2070 726f 6e75 6e63   Hokkien pronunc
+00000500: 6961 7469 6f6e 2e3c 6272 202f 3e0d 0a49  iation.<br />..I
+00000510: 6e63 6c75 6465 7320 776f 7264 2074 6f6b  ncludes word tok
+00000520: 656e 6973 6572 2066 6f72 2054 6169 7761  eniser for Taiwa
+00000530: 6e65 7365 2048 6f6b 6b69 656e 2e0d 0a0d  nese Hokkien....
+00000540: 0a5b 5265 706f 7274 2042 7567 5d5b 6275  .[Report Bug][bu
+00000550: 675d 20e2 80a2 0d0a 5b50 7950 495d 5b70  g] .....[PyPI][p
+00000560: 7970 695d 0d0a 0d0a 3c2f 6469 763e 0d0a  ypi]....</div>..
+00000570: 0d0a 0d0a 0d0a 2d2d 2d0d 0a0d 0a0d 0a0d  ......---.......
+00000580: 0a3c 212d 2d20 494e 5354 414c 4c20 2d2d  .<!-- INSTALL --
+00000590: 3e0d 0a23 2320 496e 7374 616c 6c0d 0a0d  >..## Install...
+000005a0: 0a54 6169 6275 6e20 6361 6e20 6265 2069  .Taibun can be i
+000005b0: 6e73 7461 6c6c 6564 2066 726f 6d20 5b70  nstalled from [p
+000005c0: 7970 695d 5b70 7970 695d 0d0a 0d0a 6060  ypi][pypi]....``
+000005d0: 6062 6173 680d 0a24 2070 6970 2069 6e73  `bash..$ pip ins
+000005e0: 7461 6c6c 2074 6169 6275 6e0d 0a60 6060  tall taibun..```
+000005f0: 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2055 5341  ........<!-- USA
+00000600: 4745 202d 2d3e 0d0a 2323 2055 7361 6765  GE -->..## Usage
+00000610: 0d0a 0d0a 2323 2320 436f 6e76 6572 7465  ....### Converte
+00000620: 720d 0a0d 0a60 436f 6e76 6572 7465 7260  r....`Converter`
+00000630: 2063 6c61 7373 2074 7261 6e73 6c69 7465   class translite
+00000640: 7261 7465 7320 7468 6520 4368 696e 6573  rates the Chines
+00000650: 6520 6368 6172 6163 7465 7273 2074 6f20  e characters to 
+00000660: 7468 6520 6368 6f73 656e 2074 7261 6e73  the chosen trans
+00000670: 6c69 7465 7261 7469 6f6e 2073 7973 7465  literation syste
+00000680: 6d20 7769 7468 2070 6172 616d 6574 6572  m with parameter
+00000690: 7320 7370 6563 6966 6965 6420 6279 2074  s specified by t
+000006a0: 6865 2064 6576 656c 6f70 6572 2e20 576f  he developer. Wo
+000006b0: 726b 7320 666f 7220 626f 7468 2054 7261  rks for both Tra
+000006c0: 6469 7469 6f6e 616c 2061 6e64 2053 696d  ditional and Sim
+000006d0: 706c 6966 6965 6420 6368 6172 6163 7465  plified characte
+000006e0: 7273 2e0d 0a0d 0a60 6060 7079 7468 6f6e  rs.....```python
+000006f0: 0d0a 2320 636f 6e73 7472 7563 746f 720d  ..# constructor.
+00000700: 0a63 203d 2043 6f6e 7665 7274 6572 2873  .c = Converter(s
+00000710: 7973 7465 6d2c 2064 6961 6c65 6374 2c20  ystem, dialect, 
+00000720: 666f 726d 6174 2c20 6465 6c69 6d69 7465  format, delimite
+00000730: 722c 2073 616e 6468 692c 2070 756e 6374  r, sandhi, punct
+00000740: 7561 7469 6f6e 2c20 636f 6e76 6572 745f  uation, convert_
+00000750: 6e6f 6e5f 636a 6b29 0d0a 0d0a 2320 7472  non_cjk)....# tr
+00000760: 616e 736c 6974 6572 6174 6520 4368 696e  ansliterate Chin
+00000770: 6573 6520 6368 6172 6163 7465 7273 0d0a  ese characters..
+00000780: 632e 6765 7428 696e 7075 7429 0d0a 6060  c.get(input)..``
+00000790: 600d 0a0d 0a23 2323 2320 5379 7374 656d  `....#### System
+000007a0: 0d0a 0d0a 6073 7973 7465 6d60 2053 7472  ....`system` Str
+000007b0: 696e 6720 2d20 7379 7374 656d 206f 6620  ing - system of 
+000007c0: 7472 616e 736c 6974 6572 6174 696f 6e2e  transliteration.
+000007d0: 0d0a 0d0a 2a20 6054 6169 6c6f 6020 2864  ....* `Tailo` (d
+000007e0: 6566 6175 6c74 2920 2d20 5b54 c3a2 692d  efault) - [T..i-
+000007f0: 75c3 a26e 204c c3b4 2d6d c3a1 2d6a c4ab  u..n L..-m..-j..
+00000800: 2050 6869 6e67 2d69 6d20 486f 6e67 2dc3   Phing-im Hong-.
+00000810: a06e 5d5b 7461 696c 6f2d 7769 6b69 5d0d  .n][tailo-wiki].
+00000820: 0a2a 2060 504f 4a60 202d 205b 5065 cc8d  .* `POJ` - [Pe..
+00000830: 682d c58d 652d 6ac4 ab5d 5b70 6f6a 2d77  h-..e-j..][poj-w
+00000840: 696b 695d 0d0a 2a20 605a 6875 7969 6e60  iki]..* `Zhuyin`
+00000850: 202d 205b 5461 6977 616e 6573 6520 5068   - [Taiwanese Ph
+00000860: 6f6e 6574 6963 2053 796d 626f 6c73 5d5b  onetic Symbols][
+00000870: 7a68 7579 696e 2d77 696b 695d 0d0a 2a20  zhuyin-wiki]..* 
+00000880: 6054 4c50 4160 202d 205b 5461 6977 616e  `TLPA` - [Taiwan
+00000890: 6573 6520 4c61 6e67 7561 6765 2050 686f  ese Language Pho
+000008a0: 6e65 7469 6320 416c 7068 6162 6574 5d5b  netic Alphabet][
+000008b0: 746c 7061 2d77 696b 695d 0d0a 2a20 6050  tlpa-wiki]..* `P
+000008c0: 696e 6779 696d 6020 2d20 5b42 62c3 a16e  ingyim` - [Bb..n
+000008d0: 6cc3 a16d 2055 c493 2050 c3ac 6e67 79c4  l..m U.. P..ngy.
+000008e0: ab6d 2048 c58d 6e67 27c3 a06e 5d5b 7069  .m H..ng'..n][pi
+000008f0: 6e67 7969 6d2d 7769 6b69 5d0d 0a2a 2060  ngyim-wiki]..* `
+00000900: 546f 6e67 696f 6e67 6020 2d20 5b44 61c4  Tongiong` - [Da.
+00000910: ab2d 6768 c3ae 2054 c58d 6e67 2d69 c58d  .-gh.. T..ng-i..
+00000920: 6e67 2050 c4ab 6e67 2d69 6d5d 5b74 6f6e  ng P..ng-im][ton
+00000930: 6769 6f6e 672d 7769 6b69 5d0d 0a2a 2060  giong-wiki]..* `
+00000940: 4950 4160 202d 205b 496e 7465 726e 6174  IPA` - [Internat
+00000950: 696f 6e61 6c20 5068 6f6e 6574 6963 2041  ional Phonetic A
+00000960: 6c70 6861 6265 745d 5b69 7061 2d77 696b  lphabet][ipa-wik
+00000970: 695d 0d0a 0d0a 7c20 7465 7874 207c 2054  i]....| text | T
+00000980: 6169 6c6f 2020 207c 2050 4f4a 2020 2020  ailo   | POJ    
+00000990: 207c 205a 6875 7969 6e20 2020 2020 207c   | Zhuyin      |
+000009a0: 2054 4c50 4120 2020 2020 207c 2050 696e   TLPA      | Pin
+000009b0: 6779 696d 207c 2054 6f6e 6769 6f6e 6720  gyim | Tongiong 
+000009c0: 7c20 4950 4120 2020 2020 2020 2020 7c0d  | IPA         |.
+000009d0: 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  .| ---- | ------
+000009e0: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
+000009f0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
+00000a00: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d20  ----- | ------- 
+00000a10: 7c20 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  | -------- | ---
+00000a20: 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20 e58f  -------- |..| ..
+00000a30: b0e7 81a3 207c 2054 c3a2 692d 75c3 a26e  .... | T..i-u..n
+00000a40: 207c 2054 c3a2 692d 6fc3 a26e 207c 20e3   | T..i-o..n | .
+00000a50: 8489 e384 9ecb 8a20 e384 a8e3 84a2 cb8a  ....... ........
+00000a60: 207c 2054 6169 3520 7561 6e35 207c 2044   | Tai5 uan5 | D
+00000a70: c3a1 6977 c3a1 6e20 207c 2054 c481 692d  ..iw..n  | T..i-
+00000a80: 75c7 8e6e 2020 7c20 5461 69c2 b2e2 81b5  u..n  | Tai.....
+00000a90: 2075 616e c2b2 e281 b520 7c0d 0a0d 0a23   uan..... |....#
+00000aa0: 2323 2320 4469 616c 6563 740d 0a0d 0a60  ### Dialect....`
+00000ab0: 6469 616c 6563 7460 2053 7472 696e 6720  dialect` String 
+00000ac0: 2d20 7072 6566 6572 7265 6420 7072 6f6e  - preferred pron
+00000ad0: 756e 6369 6174 696f 6e2e 0d0a 0d0a 2a20  unciation.....* 
+00000ae0: 6073 6f75 7468 6020 2864 6566 6175 6c74  `south` (default
+00000af0: 2920 2d20 5b5a 6861 6e67 7a68 6f75 5d5b  ) - [Zhangzhou][
+00000b00: 7a68 616e 677a 686f 752d 7769 6b69 5d2d  zhangzhou-wiki]-
+00000b10: 6c65 616e 696e 6720 7072 6f6e 756e 6369  leaning pronunci
+00000b20: 6174 696f 6e0d 0a2a 2060 6e6f 7274 6860  ation..* `north`
+00000b30: 202d 205b 5175 616e 7a68 6f75 5d5b 7175   - [Quanzhou][qu
+00000b40: 616e 7a68 6f75 2d77 696b 695d 2d6c 6561  anzhou-wiki]-lea
+00000b50: 6e69 6e67 2070 726f 6e75 6e63 6961 7469  ning pronunciati
+00000b60: 6f6e 0d0a 0d0a 7c20 7465 7874 2020 207c  on....| text   |
+00000b70: 2073 6f75 7468 2020 2020 2020 2020 207c   south         |
+00000b80: 206e 6f72 7468 2020 2020 2020 2020 207c   north         |
+00000b90: 0d0a 7c20 2d2d 2d2d 2d2d 207c 202d 2d2d  ..| ------ | ---
+00000ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
+00000bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20  ---------- |..| 
+00000bc0: e4ba 94e6 9c88 e7af 8020 7c20 47c5 8d6f  ......... | G..o
+00000bd0: 2d67 7565 cc8d 682d 7473 6568 207c 2047  -gue..h-tseh | G
+00000be0: c58d 6f2d 6765 cc8d 682d 7473 7565 6820  ..o-ge..h-tsueh 
+00000bf0: 7c0d 0a0d 0a23 2323 2320 466f 726d 6174  |....#### Format
+00000c00: 0d0a 0d0a 6066 6f72 6d61 7460 2053 7472  ....`format` Str
+00000c10: 696e 6720 2d20 666f 726d 6174 2069 6e20  ing - format in 
+00000c20: 7768 6963 6820 746f 6e65 7320 7769 6c6c  which tones will
+00000c30: 2062 6520 7265 7072 6573 656e 7465 6420   be represented 
+00000c40: 696e 2074 6865 2063 6f6e 7665 7274 6564  in the converted
+00000c50: 2073 656e 7465 6e63 652e 0d0a 0d0a 2a20   sentence.....* 
+00000c60: 606d 6172 6b60 2028 6465 6661 756c 7429  `mark` (default)
+00000c70: 202d 2075 7365 7320 6469 6163 7269 7469   - uses diacriti
+00000c80: 6373 2066 6f72 2065 6163 6820 7379 6c6c  cs for each syll
+00000c90: 6162 6c65 2e20 4e6f 7420 6176 6169 6c61  able. Not availa
+00000ca0: 626c 6520 666f 7220 544c 5041 2e0d 0a2a  ble for TLPA...*
+00000cb0: 2060 6e75 6d62 6572 6020 2d20 6164 6420   `number` - add 
+00000cc0: 6120 6e75 6d62 6572 2077 6869 6368 2072  a number which r
+00000cd0: 6570 7265 7365 6e74 7320 7468 6520 746f  epresents the to
+00000ce0: 6e65 2061 7420 7468 6520 656e 6420 6f66  ne at the end of
+00000cf0: 2074 6865 2073 796c 6c61 626c 650d 0a2a   the syllable..*
+00000d00: 2060 7374 7269 7060 202d 2072 656d 6f76   `strip` - remov
+00000d10: 6573 2061 6e79 2074 6f6e 6520 6d61 726b  es any tone mark
+00000d20: 696e 670d 0a0d 0a7c 2074 6578 7420 7c20  ing....| text | 
+00000d30: 6d61 726b 2020 2020 7c20 6e75 6d62 6572  mark    | number
+00000d40: 2020 2020 7c20 7374 7269 7020 2020 7c0d      | strip   |.
+00000d50: 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  .| ---- | ------
+00000d60: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d20 7c20  - | --------- | 
+00000d70: 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0  ------- |..| ...
+00000d80: e781 a320 7c20 54c3 a269 2d75 c3a2 6e20  ... | T..i-u..n 
+00000d90: 7c20 5461 6935 2d75 616e 3520 7c20 5461  | Tai5-uan5 | Ta
+00000da0: 692d 7561 6e20 7c0d 0a0d 0a23 2323 2320  i-uan |....#### 
+00000db0: 4465 6c69 6d69 7465 720d 0a0d 0a60 6465  Delimiter....`de
+00000dc0: 6c69 6d69 7465 7260 2053 7472 696e 6720  limiter` String 
+00000dd0: 2d20 7365 7473 2074 6865 2064 656c 696d  - sets the delim
+00000de0: 6974 6572 2063 6861 7261 6374 6572 2074  iter character t
+00000df0: 6861 7420 7769 6c6c 2062 6520 706c 6163  hat will be plac
+00000e00: 6564 2069 6e20 6265 7477 6565 6e20 7379  ed in between sy
+00000e10: 6c6c 6162 6c65 7320 6f66 2061 2077 6f72  llables of a wor
+00000e20: 642e 0d0a 0d0a 4465 6661 756c 7420 7661  d.....Default va
+00000e30: 6c75 6520 6465 7065 6e64 7320 6f6e 2074  lue depends on t
+00000e40: 6865 2063 686f 7365 6e20 6073 7973 7465  he chosen `syste
+00000e50: 6d60 3a0d 0a0d 0a2a 2060 272d 2760 202d  m`:....* `'-'` -
+00000e60: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
+00000e70: 4f4a 602c 2060 546f 6e67 696f 6e67 600d  OJ`, `Tongiong`.
+00000e80: 0a2a 2060 2727 6020 2d20 666f 7220 6050  .* `''` - for `P
+00000e90: 696e 6779 696d 600d 0a2a 2060 2720 2760  ingyim`..* `' '`
+00000ea0: 202d 2066 6f72 2060 5a68 7579 696e 602c   - for `Zhuyin`,
+00000eb0: 2060 544c 5041 602c 2060 4950 4160 0d0a   `TLPA`, `IPA`..
+00000ec0: 0d0a 7c20 7465 7874 207c 2027 2d27 2020  ..| text | '-'  
+00000ed0: 2020 207c 2027 2720 2020 2020 7c20 2720     | ''     | ' 
+00000ee0: 2720 2020 2020 7c0d 0a7c 202d 2d2d 2d20  '     |..| ---- 
+00000ef0: 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  | ------- | ----
+00000f00: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
+00000f10: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
+00000f20: 75c3 a26e 207c 2054 c3a2 6975 c3a2 6e20  u..n | T..iu..n 
+00000f30: 7c20 54c3 a269 2075 c3a2 6e20 7c0d 0a0d  | T..i u..n |...
+00000f40: 0a23 2323 2320 5361 6e64 6869 0d0a 0d0a  .#### Sandhi....
+00000f50: 6073 616e 6468 6960 2053 7472 696e 6720  `sandhi` String 
+00000f60: 2d20 6170 706c 6965 7320 7468 6520 5b73  - applies the [s
+00000f70: 616e 6468 6920 7275 6c65 7320 6f66 2054  andhi rules of T
+00000f80: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
+00000f90: 5d5b 7361 6e64 6869 2d77 696b 695d 2074  ][sandhi-wiki] t
+00000fa0: 6f20 7379 6c6c 6162 6c65 7320 6f66 2061  o syllables of a
+00000fb0: 2073 696e 676c 6520 776f 7264 2e0d 0a0d   single word....
+00000fc0: 0a53 696e 6365 2069 7427 7320 6469 6666  .Since it's diff
+00000fd0: 6963 756c 7420 746f 2065 6e63 6f64 6520  icult to encode 
+00000fe0: 616c 6c20 7361 6e64 6869 2072 756c 6573  all sandhi rules
+00000ff0: 2c20 5461 6962 756e 2070 726f 7669 6465  , Taibun provide
+00001000: 7320 6d75 6c74 6970 6c65 206d 6f64 6573  s multiple modes
+00001010: 2066 6f72 2073 616e 6468 6920 636f 6e76   for sandhi conv
+00001020: 6572 7369 6f6e 2074 6f20 616c 6c6f 7720  ersion to allow 
+00001030: 666f 7220 6375 7374 6f6d 6973 6564 2073  for customised s
+00001040: 616e 6468 6920 6861 6e64 6c69 6e67 2e0d  andhi handling..
+00001050: 0a0d 0a2a 2060 6e6f 6e65 6020 2d20 646f  ...* `none` - do
+00001060: 6573 6e27 7420 7065 7266 6f72 6d20 616e  esn't perform an
+00001070: 7920 746f 6e65 2073 616e 6468 690d 0a2a  y tone sandhi..*
+00001080: 2060 6175 746f 6020 2d20 636c 6f73 6573   `auto` - closes
+00001090: 7420 6170 7072 6f78 696d 6174 696f 6e20  t approximation 
+000010a0: 746f 2066 756c 6c20 636f 7272 6563 7420  to full correct 
+000010b0: 746f 6e65 2073 616e 6468 6920 6f66 2054  tone sandhi of T
+000010c0: 6169 7761 6e65 7365 2c20 7769 7468 2070  aiwanese, with p
+000010d0: 726f 7065 7220 7361 6e64 6869 206f 6620  roper sandhi of 
+000010e0: 7072 6f6e 6f75 6e73 2c20 7375 6666 6978  pronouns, suffix
+000010f0: 6573 2c20 616e 6420 776f 7264 7320 7769  es, and words wi
+00001100: 7468 20e4 bb94 0d0a 2a20 6065 7863 5f6c  th .....* `exc_l
+00001110: 6173 7460 202d 2063 6861 6e67 6573 2074  ast` - changes t
+00001120: 6f6e 6520 666f 7220 6576 6572 7920 7379  one for every sy
+00001130: 6c6c 6162 6c65 2065 7863 6570 7420 666f  llable except fo
+00001140: 7220 7468 6520 6c61 7374 206f 6e65 0d0a  r the last one..
+00001150: 2a20 6069 6e63 6c5f 6c61 7374 6020 2d20  * `incl_last` - 
+00001160: 6368 616e 6765 7320 746f 6e65 2066 6f72  changes tone for
+00001170: 2065 7665 7279 2073 796c 6c61 626c 6520   every syllable 
+00001180: 696e 636c 7564 696e 6720 7468 6520 6c61  including the la
+00001190: 7374 206f 6e65 0d0a 0d0a 4465 6661 756c  st one....Defaul
+000011a0: 7420 7661 6c75 6520 6465 7065 6e64 7320  t value depends 
+000011b0: 6f6e 2074 6865 2063 686f 7365 6e20 6073  on the chosen `s
+000011c0: 7973 7465 6d60 3a0d 0a0d 0a2a 2060 6175  ystem`:....* `au
+000011d0: 746f 6020 2d20 666f 7220 6054 6f6e 6769  to` - for `Tongi
+000011e0: 6f6e 6760 0d0a 2a20 606e 6f6e 6560 202d  ong`..* `none` -
+000011f0: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
+00001200: 4f4a 602c 2060 5a68 7579 696e 602c 2060  OJ`, `Zhuyin`, `
+00001210: 544c 5041 602c 2060 5069 6e67 7969 6d60  TLPA`, `Pingyim`
+00001220: 2c20 6049 5041 600d 0a0d 0a7c 2074 6578  , `IPA`....| tex
+00001230: 7420 2020 2020 2020 2020 7c20 6e6f 6e65  t         | none
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 207c 2061 7574 6f20 2020 2020 2020 2020   | auto         
+00001260: 2020 2020 2020 2020 7c20 6578 635f 6c61          | exc_la
+00001270: 7374 2020 2020 2020 2020 2020 2020 207c  st             |
+00001280: 2069 6e63 6c5f 6c61 7374 2020 2020 2020   incl_last      
+00001290: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
+000012a0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+000012b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+000012c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000012d0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+000012e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
+000012f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001300: 2d2d 2d20 7c0d 0a7c 20e9 8099 e698 afe5  --- |..| .......
+00001310: 8fb0 e781 a3e5 9ba1 e4bb 9420 7c20 5473  ........... | Ts
+00001320: 6520 73c4 ab20 54c3 a269 2d75 c3a2 6e20  e s.. T..i-u..n 
+00001330: 67c3 ad6e 2dc3 a120 7c20 5473 6520 73c3  g..n-.. | Tse s.
+00001340: ac20 54c4 8169 2d75 c481 6e20 6769 6e2d  . T..i-u..n gin-
+00001350: c3a1 207c 2054 73c4 9320 73c3 ac20 54c4  .. | Ts.. s.. T.
+00001360: 8169 2d75 c481 6e20 6769 6e2d c3a1 207c  .i-u..n gin-.. |
+00001370: 2054 73c4 9320 73c3 ac20 54c4 8169 2d75   Ts.. s.. T..i-u
+00001380: c481 6e20 6769 6e2d 6120 7c0d 0a0d 0a53  ..n gin-a |....S
+00001390: 616e 6468 6920 7275 6c65 7320 616c 736f  andhi rules also
+000013a0: 2063 6861 6e67 6520 6465 7065 6e64 696e   change dependin
+000013b0: 6720 6f6e 2074 6865 2064 6961 6c65 6374  g on the dialect
+000013c0: 2063 686f 7365 6e2e 0d0a 0d0a 7c20 7465   chosen.....| te
+000013d0: 7874 207c 206e 6f20 7361 6e64 6869 207c  xt | no sandhi |
+000013e0: 2073 6f75 7468 2020 207c 206e 6f72 7468   south   | north
+000013f0: 2020 207c 0d0a 7c20 2d2d 2d2d 207c 202d     |..| ---- | -
+00001400: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
+00001410: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
+00001420: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
+00001430: 75c3 a26e 2020 207c 2054 c481 692d 75c3  u..n   | T..i-u.
+00001440: a26e 207c 2054 c3a0 692d 75c3 a26e 207c  .n | T..i-u..n |
+00001450: 0d0a 0d0a 2323 2323 2050 756e 6374 7561  ....#### Punctua
+00001460: 7469 6f6e 0d0a 0d0a 6070 756e 6374 7561  tion....`punctua
+00001470: 7469 6f6e 6020 5374 7269 6e67 0d0a 0d0a  tion` String....
+00001480: 2a20 6066 6f72 6d61 7460 2028 6465 6661  * `format` (defa
+00001490: 756c 7429 202d 2063 6f6e 7665 7274 7320  ult) - converts 
+000014a0: 4368 696e 6573 652d 7374 796c 6520 7075  Chinese-style pu
+000014b0: 6e63 7475 6174 696f 6e20 746f 204c 6174  nctuation to Lat
+000014c0: 696e 2d73 7479 6c65 2070 756e 6374 7561  in-style punctua
+000014d0: 7469 6f6e 2061 6e64 2063 6170 6974 616c  tion and capital
+000014e0: 6973 6573 2077 6f72 6473 2061 7420 7468  ises words at th
+000014f0: 6520 6265 6769 6e6e 696e 6720 6f66 2065  e beginning of e
+00001500: 6163 6820 7365 6e74 656e 6365 2e0d 0a2a  ach sentence...*
+00001510: 2060 6e6f 6e65 6020 2d20 7072 6573 6572   `none` - preser
+00001520: 7665 7320 4368 696e 6573 652d 7374 796c  ves Chinese-styl
+00001530: 6520 7075 6e63 7475 6174 696f 6e20 616e  e punctuation an
+00001540: 6420 646f 6573 6e27 7420 6361 7069 7461  d doesn't capita
+00001550: 6c69 7365 2077 6f72 6473 2061 7420 7468  lise words at th
+00001560: 6520 6265 6769 6e6e 696e 6720 6f66 206e  e beginning of n
+00001570: 6577 2073 656e 7465 6e63 6573 2e0d 0a0d  ew sentences....
+00001580: 0a7c 2074 6578 7420 2020 2020 2020 2020  .| text         
+00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015d0: 2020 7c20 666f 726d 6174 2020 2020 2020    | format      
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2020 2020 2020 7c20 6e6f 6e65 2020 2020        | none    
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001690: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
+000016a0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
+000016b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016f0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00001700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001750: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d 0a7c  ----------- |..|
+000017c0: 20e9 8099 e698 afe8 87ba e58d 97ef bc8c   ...............
+000017d0: e7b0 a1e7 a8b1 e380 8ce5 8d97 e380 8def  ................
+000017e0: bc88 e799 bde8 a9b1 e5ad 97ef bc9a 54c3  ..............T.
+000017f0: a269 2d6c c3a2 6def bc9b e6b3 a8e9 9fb3  .i-l..m.........
+00001800: e7ac a6e8 999f efbc 9ae3 848a e384 9ecb  ................
+00001810: 8a20 e384 8be3 84a2 cb8a efbc 8ce5 9c8b  . ..............
+00001820: e8aa 9eef bc9a 54c3 a169 6ec3 a16e efbc  ......T..in..n..
+00001830: 89e3 8082 207c 2054 7365 2073 c4ab 2054  .... | Tse s.. T
+00001840: c3a2 692d 6cc3 a26d 2c20 6bc3 a16e 2d74  ..i-l..m, k..n-t
+00001850: 7368 696e 6720 226c c3a2 6d22 2028 5065  shing "l..m" (Pe
+00001860: cc8d 682d 75c4 932d 6ac4 ab3a 2054 c3a2  ..h-u..-j..: T..
+00001870: 692d 6cc3 a26d 3b20 7473 c3b9 2d69 6d20  i-l..m; ts..-im 
+00001880: 68c3 bb2d 68c5 8d3a 20e3 848a e384 9ecb  h..-h..: .......
+00001890: 8a20 e384 8be3 84a2 cb8a 2c20 6b6f 6b2d  . ........, kok-
+000018a0: 67c3 ad3a 2054 c3a1 696e c3a1 6e29 2e20  g..: T..in..n). 
+000018b0: 7c20 7473 6520 73c4 ab20 54c3 a269 2d6c  | tse s.. T..i-l
+000018c0: c3a2 6def bc8c 6bc3 a16e 2d74 7368 696e  ..m...k..n-tshin
+000018d0: 67e3 808c 6cc3 a26d e380 8def bc88 5065  g...l..m......Pe
+000018e0: cc8d 682d 75c4 932d 6ac4 abef bc9a 54c3  ..h-u..-j.....T.
+000018f0: a269 2d6c c3a2 6def bc9b 7473 c3b9 2d69  .i-l..m...ts..-i
+00001900: 6d20 68c3 bb2d 68c5 8def bc9a e384 8ae3  m h..-h.........
+00001910: 849e cb8a 20e3 848b e384 a2cb 8aef bc8c  .... ...........
+00001920: 6b6f 6b2d 67c3 adef bc9a 54c3 a169 6ec3  kok-g.....T..in.
+00001930: a16e efbc 89e3 8082 207c 0d0a 0d0a 2323  .n...... |....##
+00001940: 2323 2043 6f6e 7665 7274 206e 6f6e 2d43  ## Convert non-C
+00001950: 4a4b 0d0a 0d0a 6063 6f6e 7665 7274 5f6e  JK....`convert_n
+00001960: 6f6e 5f63 6a6b 6020 426f 6f6c 6561 6e20  on_cjk` Boolean 
+00001970: 2d20 6465 6669 6e65 7320 7768 6574 6865  - defines whethe
+00001980: 7220 6f72 206e 6f74 2074 6f20 636f 6e76  r or not to conv
+00001990: 6572 7420 6e6f 6e2d 4368 696e 6573 6520  ert non-Chinese 
+000019a0: 776f 7264 732e 2043 616e 2062 6520 7573  words. Can be us
+000019b0: 6564 2074 6f20 636f 6e76 6572 7420 5461  ed to convert Ta
+000019c0: 696c 6f20 746f 2061 6e6f 7468 6572 2072  ilo to another r
+000019d0: 6f6d 616e 6973 6174 696f 6e20 7379 7374  omanisation syst
+000019e0: 656d 2e0d 0a0d 0a2a 2060 5472 7565 6020  em.....* `True` 
+000019f0: 2d20 636f 6e76 6572 7420 6e6f 6e2d 4368  - convert non-Ch
+00001a00: 696e 6573 6520 6368 6172 6163 7465 7220  inese character 
+00001a10: 776f 7264 730d 0a2a 2060 4661 6c73 6560  words..* `False`
+00001a20: 2028 6465 6661 756c 7429 202d 2063 6f6e   (default) - con
+00001a30: 7665 7274 206f 6e6c 7920 4368 696e 6573  vert only Chines
+00001a40: 6520 6368 6172 6163 7465 7220 776f 7264  e character word
+00001a50: 730d 0a0d 0a7c 2074 6578 7420 2020 2020  s....| text     
+00001a60: 207c 2046 616c 7365 2020 2020 2020 2020   | False        
+00001a70: 2020 2020 2020 2020 2020 207c 2054 7275             | Tru
+00001a80: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00001a90: 2020 2020 207c 0d0a 7c20 2d2d 2d2d 2d2d       |..| ------
+00001aa0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ad0: 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e6 8891  ------- |..| ...
+00001ae0: e9a3 9f70 68c3 a16e 6720 7c20 e386 a3e3  ...ph..ng | ....
+00001af0: 84a8 e384 9acb 8b20 e384 90e3 84a7 e384  ....... ........
+00001b00: 9ae3 86b7 cb99 2070 68c3 a16e 6720 7c20  ...... ph..ng | 
+00001b10: e386 a3e3 84a8 e384 9acb 8b20 e384 90e3  ........... ....
+00001b20: 84a7 e384 9ae3 86b7 cb99 20e3 8486 e384  .......... .....
+00001b30: a4cb 8b20 7c0d 0a0d 0a23 2323 2054 6f6b  ... |....### Tok
+00001b40: 656e 6973 6572 0d0a 0d0a 6054 6f6b 656e  eniser....`Token
+00001b50: 6973 6572 6020 636c 6173 7320 7065 7266  iser` class perf
+00001b60: 6f72 6d73 205b 4e4c 544b 2077 6f72 6470  orms [NLTK wordp
+00001b70: 756e 6374 5f74 6f6b 656e 697a 655d 5b6e  unct_tokenize][n
+00001b80: 6c74 6b2d 746f 6b65 6e69 7a65 5d2d 6c69  ltk-tokenize]-li
+00001b90: 6b65 2074 6f6b 656e 6973 6174 696f 6e20  ke tokenisation 
+00001ba0: 6f66 2061 2054 6169 7761 6e65 7365 2048  of a Taiwanese H
+00001bb0: 6f6b 6b69 656e 2073 656e 7465 6e63 652e  okkien sentence.
+00001bc0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a23  ....```python..#
+00001bd0: 2063 6f6e 7374 7275 6374 6f72 0d0a 7420   constructor..t 
+00001be0: 3d20 546f 6b65 6e69 7365 7228 290d 0a0d  = Tokeniser()...
+00001bf0: 0a23 2074 6f6b 656e 6973 6520 5461 6977  .# tokenise Taiw
+00001c00: 616e 6573 6520 486f 6b6b 6965 6e20 7365  anese Hokkien se
+00001c10: 6e74 656e 6365 0d0a 742e 746f 6b65 6e69  ntence..t.tokeni
+00001c20: 7365 2869 6e70 7574 290d 0a60 6060 0d0a  se(input)..```..
+00001c30: 0d0a 2323 2320 4f74 6865 7220 4675 6e63  ..### Other Func
+00001c40: 7469 6f6e 730d 0a0d 0a60 6060 7079 7468  tions....```pyth
+00001c50: 6f6e 0d0a 2320 436f 6e76 6572 7420 746f  on..# Convert to
+00001c60: 2054 7261 6469 7469 6f6e 616c 0d0a 746f   Traditional..to
+00001c70: 5f74 7261 6469 7469 6f6e 616c 2869 6e70  _traditional(inp
+00001c80: 7574 290d 0a0d 0a23 2043 6f6e 7665 7274  ut)....# Convert
+00001c90: 2074 6f20 5369 6d70 6c69 6669 6564 0d0a   to Simplified..
+00001ca0: 746f 5f73 696d 706c 6966 6965 6428 696e  to_simplified(in
+00001cb0: 7075 7429 0d0a 0d0a 2320 4368 6563 6b20  put)....# Check 
+00001cc0: 6966 2074 6865 2073 7472 696e 6720 6973  if the string is
+00001cd0: 2066 756c 6c79 2063 6f6d 706f 7365 6420   fully composed 
+00001ce0: 6f66 2043 6869 6e65 7365 2063 6861 7261  of Chinese chara
+00001cf0: 6374 6572 730d 0a69 735f 636a 6b28 696e  cters..is_cjk(in
+00001d00: 7075 7429 0d0a 6060 600d 0a0d 0a0d 0a0d  put)..```.......
+00001d10: 0a3c 212d 2d20 4558 414d 504c 4520 2d2d  .<!-- EXAMPLE --
+00001d20: 3e0d 0a23 2320 4578 616d 706c 650d 0a0d  >..## Example...
+00001d30: 0a60 6060 7079 7468 6f6e 0d0a 2320 436f  .```python..# Co
+00001d40: 6e76 6572 7465 720d 0a66 726f 6d20 7461  nverter..from ta
+00001d50: 6962 756e 2069 6d70 6f72 7420 436f 6e76  ibun import Conv
+00001d60: 6572 7465 720d 0a0d 0a23 2320 5379 7374  erter....## Syst
+00001d70: 656d 0d0a 6320 3d20 436f 6e76 6572 7465  em..c = Converte
+00001d80: 7228 2920 2320 5461 696c 6f20 7379 7374  r() # Tailo syst
+00001d90: 656d 2064 6566 6175 6c74 0d0a 632e 6765  em default..c.ge
+00001da0: 7428 27e5 8588 e794 9fe8 ac9b efbc 8ce5  t('.............
+00001db0: adb8 e794 9fe6 81ac e681 ace8 81bd e380  ................
+00001dc0: 8227 290d 0a3e 3e20 5369 616e 2d73 696e  .')..>> Sian-sin
+00001dd0: 6e20 6bc3 b36e 672c 2068 61cc 8d6b 2d73  n k..ng, ha..k-s
+00001de0: 696e 6720 7469 c481 6d2d 7469 c481 6d20  ing ti..m-ti..m 
+00001df0: 7468 6961 6e6e 2e0d 0a0d 0a63 203d 2043  thiann.....c = C
+00001e00: 6f6e 7665 7274 6572 2873 7973 7465 6d3d  onverter(system=
+00001e10: 275a 6875 7969 6e27 290d 0a63 2e67 6574  'Zhuyin')..c.get
+00001e20: 2827 e585 88e7 949f e8ac 9bef bc8c e5ad  ('..............
+00001e30: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
+00001e40: 2729 0d0a 3e3e 20e3 8492 e384 a7e3 84a2  ')..>> .........
+00001e50: 20e3 8492 e386 aa20 e384 8de3 86b2 cb8b   ...... ........
+00001e60: 2c20 e384 8fe3 849a e386 b6cb 9920 e384  , ........... ..
+00001e70: 92e3 84a7 e384 a520 e384 89e3 84a7 e386  ....... ........
+00001e80: b0cb ab20 e384 89e3 84a7 e386 b0cb ab20  ... ........... 
+00001e90: e384 8ae3 84a7 e386 a92e 0d0a 0d0a 2323  ..............##
+00001ea0: 2044 6961 6c65 6374 0d0a 6320 3d20 436f   Dialect..c = Co
+00001eb0: 6e76 6572 7465 7228 2920 2320 736f 7574  nverter() # sout
+00001ec0: 6820 6469 616c 6563 7420 6465 6661 756c  h dialect defaul
+00001ed0: 740d 0a63 2e67 6574 2822 e688 91e6 acb2  t..c.get("......
+00001ee0: e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a  ............")..
+00001ef0: 3e3e 2047 75c3 a120 6265 6820 c4ab 6e67  >> Gu.. beh ..ng
+00001f00: 2074 c4ab 2074 7369 61cc 8d68 2068 c3ae   t.. tsia..h h..
+00001f10: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00001f20: 7228 6469 616c 6563 743d 276e 6f72 7468  r(dialect='north
+00001f30: 2729 0d0a 632e 6765 7428 22e6 8891 e6ac  ')..c.get(".....
+00001f40: b2e7 94a8 e7ae b8e9 a39f e9ad 9a22 290d  .............").
+00001f50: 0a3e 3e20 4775 c3a1 2062 7565 6820 c4ab  .>> Gu.. bueh ..
+00001f60: 6e67 2074 c5ab 2074 7369 61cc 8d68 2068  ng t.. tsia..h h
+00001f70: c3bb 0d0a 0d0a 2323 2046 6f72 6d61 740d  ......## Format.
+00001f80: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
+00001f90: 2023 2066 6f72 2054 6169 6c6f 2c20 6d61   # for Tailo, ma
+00001fa0: 726b 2062 7920 6465 6661 756c 740d 0a63  rk by default..c
+00001fb0: 2e67 6574 2822 e794 9fe6 97a5 e5bf abe6  .get("..........
+00001fc0: a882 2229 0d0a 3e3e 2053 656e 6e2d 6a69  ..")..>> Senn-ji
+00001fd0: cc8d 7420 6b68 75c3 a069 2d6c 6fcc 8d6b  ..t khu..i-lo..k
+00001fe0: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00001ff0: 7228 666f 726d 6174 3d27 6e75 6d62 6572  r(format='number
+00002000: 2729 0d0a 632e 6765 7428 22e7 949f e697  ')..c.get(".....
+00002010: a5e5 bfab e6a8 8222 290d 0a3e 3e20 5365  .......")..>> Se
+00002020: 6e6e 312d 6a69 7438 206b 6875 6169 332d  nn1-jit8 khuai3-
+00002030: 6c6f 6b38 0d0a 0d0a 6320 3d20 436f 6e76  lok8....c = Conv
+00002040: 6572 7465 7228 666f 726d 6174 3d27 7374  erter(format='st
+00002050: 7269 7027 290d 0a63 2e67 6574 2822 e794  rip')..c.get("..
+00002060: 9fe6 97a5 e5bf abe6 a882 2229 0d0a 3e3e  ..........")..>>
+00002070: 2053 656e 6e2d 6a69 7420 6b68 7561 692d   Senn-jit khuai-
+00002080: 6c6f 6b0d 0a0d 0a23 2320 4465 6c69 6d69  lok....## Delimi
+00002090: 7465 720d 0a63 203d 2043 6f6e 7665 7274  ter..c = Convert
+000020a0: 6572 2864 656c 696d 6974 6572 3d27 2729  er(delimiter='')
+000020b0: 0d0a 632e 6765 7428 22e5 8588 e794 9fe8  ..c.get(".......
+000020c0: ac9b efbc 8ce5 adb8 e794 9fe6 81ac e681  ................
+000020d0: ace8 81bd e380 8222 290d 0a3e 3e20 5369  .......")..>> Si
+000020e0: 616e 7369 6e6e 206b c3b3 6e67 2c20 6861  ansinn k..ng, ha
+000020f0: cc8d 6b73 696e 6720 7469 c481 6d74 69c4  ..ksing ti..mti.
+00002100: 816d 2074 6869 616e 6e2e 0d0a 0d0a 6320  .m thiann.....c 
+00002110: 3d20 436f 6e76 6572 7465 7228 7379 7374  = Converter(syst
+00002120: 656d 3d27 5069 6e67 7969 6d27 2c20 6465  em='Pingyim', de
+00002130: 6c69 6d69 7465 723d 272d 2729 0d0a 632e  limiter='-')..c.
+00002140: 6765 7428 22e5 8588 e794 9fe8 ac9b efbc  get("...........
+00002150: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
+00002160: e380 8222 290d 0a3e 3e20 5369 c481 6e2d  ...")..>> Si..n-
+00002170: 736e c4ab 2067 c792 6e67 2c20 68c3 a167  sn.. g..ng, h..g
+00002180: 2d73 c4ab 6e67 2064 69c3 a26d 2d64 69c3  -s..ng di..m-di.
+00002190: a26d 2074 696e c481 2e0d 0a0d 0a23 2320  .m tin.......## 
+000021a0: 5361 6e64 6869 0d0a 6320 3d20 436f 6e76  Sandhi..c = Conv
+000021b0: 6572 7465 7228 2920 2320 666f 7220 5461  erter() # for Ta
+000021c0: 696c 6f2c 2073 616e 6468 6920 6e6f 6e65  ilo, sandhi none
+000021d0: 2062 7920 6465 6661 756c 740d 0a63 2e67   by default..c.g
+000021e0: 6574 2822 e980 99e6 98af e58f b0e7 81a3  et("............
+000021f0: e59b a1e4 bb94 2229 0d0a 3e3e 2054 7365  ......")..>> Tse
+00002200: 2073 c4ab 2054 c3a2 692d 75c3 a26e 2067   s.. T..i-u..n g
+00002210: c3ad 6e2d c3a1 0d0a 0d0a 6320 3d20 436f  ..n-......c = Co
+00002220: 6e76 6572 7465 7228 7361 6e64 6869 3d27  nverter(sandhi='
+00002230: 6175 746f 2729 0d0a 632e 6765 7428 22e9  auto')..c.get(".
+00002240: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
+00002250: 9422 290d 0a3e 3e20 5473 6520 73c3 ac20  .")..>> Tse s.. 
+00002260: 54c4 8169 2d75 c481 6e20 6769 6e2d c3a1  T..i-u..n gin-..
+00002270: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00002280: 7228 7361 6e64 6869 3d27 6578 635f 6c61  r(sandhi='exc_la
+00002290: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
+000022a0: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+000022b0: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
+000022c0: c481 692d 75c4 816e 2067 696e 2dc3 a10d  ..i-u..n gin-...
+000022d0: 0a0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
+000022e0: 2873 616e 6468 693d 2769 6e63 6c5f 6c61  (sandhi='incl_la
+000022f0: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
+00002300: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+00002310: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
+00002320: c481 692d 75c4 816e 2067 696e 2d61 0d0a  ..i-u..n gin-a..
+00002330: 0d0a 2323 2050 756e 6374 7561 7469 6f6e  ..## Punctuation
+00002340: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+00002350: 2920 2320 666f 726d 6174 2070 756e 6374  ) # format punct
+00002360: 7561 7469 6f6e 2064 6566 6175 6c74 0d0a  uation default..
+00002370: 632e 6765 7428 22e5 a4aa e7a9 bae6 9c8b  c.get(".........
+00002380: e58f 8bef bc8c e681 81e5 a5bd efbc 81e6  ................
+00002390: 8181 e9a3 9fe9 a3bd e69c aaef bc9f 2229  ..............")
+000023a0: 0d0a 3e3e 2054 68c3 a069 2d6b 686f 6e67  ..>> Th..i-khong
+000023b0: 2070 c3ae 6e67 2d69 c3ba 2c20 6cc3 ad6e   p..ng-i.., l..n
+000023c0: 2d68 c3b3 2120 4cc3 ad6e 2074 7369 61cc  -h..! L..n tsia.
+000023d0: 8d68 2d70 c3a1 2062 75c4 933f 0d0a 0d0a  .h-p.. bu..?....
+000023e0: 6320 3d20 436f 6e76 6572 7465 7228 7075  c = Converter(pu
+000023f0: 6e63 7475 6174 696f 6e3d 276e 6f6e 6527  nctuation='none'
+00002400: 290d 0a63 2e67 6574 2822 e5a4 aae7 a9ba  )..c.get("......
+00002410: e69c 8be5 8f8b efbc 8ce6 8181 e5a5 bdef  ................
+00002420: bc81 e681 81e9 a39f e9a3 bde6 9caa efbc  ................
+00002430: 9f22 290d 0a3e 3e20 7468 c3a0 692d 6b68  .")..>> th..i-kh
+00002440: 6f6e 6720 70c3 ae6e 672d 69c3 baef bc8c  ong p..ng-i.....
+00002450: 6cc3 ad6e 2d68 c3b3 efbc 816c c3ad 6e20  l..n-h.....l..n 
+00002460: 7473 6961 cc8d 682d 70c3 a120 6275 c493  tsia..h-p.. bu..
+00002470: efbc 9f0d 0a0d 0a23 2320 436f 6e76 6572  .......## Conver
+00002480: 7420 6e6f 6e2d 434a 4b0d 0a63 203d 2043  t non-CJK..c = C
+00002490: 6f6e 7665 7274 2873 7973 7465 6d3d 275a  onvert(system='Z
+000024a0: 6875 7969 6e27 2920 2320 4661 6c73 6520  huyin') # False 
+000024b0: 636f 6e76 6572 745f 6e6f 6e5f 636a 6b20  convert_non_cjk 
+000024c0: 6465 6661 756c 740d 0a63 2e67 6574 2822  default..c.get("
+000024d0: e688 91e9 a39f 7068 c3a1 6e67 2229 0d0a  ......ph..ng")..
+000024e0: 3e3e 20e3 86a3 e384 a8e3 849a cb8b 20e3  >> ........... .
+000024f0: 8490 e384 a7e3 849a e386 b7cb 9920 7068  ............. ph
+00002500: c3a1 6e67 0d0a 0d0a 6320 3d20 436f 6e76  ..ng....c = Conv
+00002510: 6572 7428 7379 7374 656d 3d27 5a68 7579  ert(system='Zhuy
+00002520: 696e 272c 2063 6f6e 7665 7274 5f6e 6f6e  in', convert_non
+00002530: 5f63 6a6b 3d54 7275 6529 0d0a 632e 6765  _cjk=True)..c.ge
+00002540: 7428 22e6 8891 e9a3 9f70 68c3 a16e 6722  t("......ph..ng"
+00002550: 290d 0a3e 3e20 e386 a3e3 84a8 e384 9acb  )..>> ..........
+00002560: 8b20 e384 90e3 84a7 e384 9ae3 86b7 cb99  . ..............
+00002570: 20e3 8486 e384 a4cb 8b0d 0a0d 0a0d 0a23   ..............#
+00002580: 2054 6f6b 656e 6973 6572 0d0a 6672 6f6d   Tokeniser..from
+00002590: 2074 6169 6275 6e20 696d 706f 7274 2054   taibun import T
+000025a0: 6f6b 656e 6973 6572 0d0a 0d0a 7420 3d20  okeniser....t = 
+000025b0: 546f 6b65 6e69 7365 7228 290d 0a74 2e74  Tokeniser()..t.t
+000025c0: 6f6b 656e 6973 6528 22e5 a4aa e7a9 bae6  okenise(".......
+000025d0: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
+000025e0: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
+000025f0: 2229 0d0a 3e3e 205b 27e5 a4aa e7a9 ba27  ")..>> ['......'
+00002600: 2c20 27e6 9c8b e58f 8b27 2c20 27ef bc8c  , '......', '...
+00002610: 272c 2027 e681 81e5 a5bd 272c 2027 efbc  ', '......', '..
+00002620: 8127 2c20 27e6 8181 272c 2027 e9a3 9fe9  .', '...', '....
+00002630: a3bd 272c 2027 e69c aa27 2c20 27ef bc9f  ..', '...', '...
+00002640: 275d 0d0a 0d0a 0d0a 2320 4f74 6865 7220  ']......# Other 
+00002650: 4675 6e63 7469 6f6e 730d 0a66 726f 6d20  Functions..from 
+00002660: 7461 6962 756e 2069 6d70 6f72 7420 746f  taibun import to
+00002670: 5f74 7261 6469 7469 6f6e 616c 2c20 746f  _traditional, to
+00002680: 5f73 696d 706c 6966 6965 642c 2069 735f  _simplified, is_
+00002690: 636a 6b0d 0a0d 0a74 6f5f 7472 6164 6974  cjk....to_tradit
+000026a0: 696f 6e61 6c28 22e6 8891 e590 ace6 97a0  ional(".........
+000026b0: e58f b0e6 b9be e8af 9d22 290d 0a3e 3e20  .........")..>> 
+000026c0: e688 91e8 81bd e784 a1e5 8fb0 e781 a3e8  ................
+000026d0: a9b1 0d0a 0d0a 746f 5f73 696d 706c 6966  ......to_simplif
+000026e0: 6965 6428 22e6 8891 e881 bde7 84a1 e887  ied("...........
+000026f0: bae7 81a3 e8a9 b122 290d 0a3e 3e20 e688  .......")..>> ..
+00002700: 91e5 90ac e697 a0e5 8fb0 e6b9 bee8 af9d  ................
+00002710: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
+00002720: a39f e9ba ad27 290d 0a3e 3e20 5472 7565  .....')..>> True
+00002730: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
+00002740: a39f 7068 c3a1 6e67 2729 0d0a 3e3e 2046  ..ph..ng')..>> F
+00002750: 616c 7365 0d0a 6060 600d 0a0d 0a0d 0a0d  alse..```.......
+00002760: 0a3c 212d 2d20 4441 5441 202d 2d3e 0d0a  .<!-- DATA -->..
+00002770: 2323 2044 6174 610d 0a0d 0a2d 205b 5461  ## Data....- [Ta
+00002780: 6977 616e 6573 652d 4368 696e 6573 6520  iwanese-Chinese 
+00002790: 4f6e 6c69 6e65 2044 6963 7469 6f6e 6172  Online Dictionar
+000027a0: 795d 5b6f 6e6c 696e 652d 6469 6374 696f  y][online-dictio
+000027b0: 6e61 7279 5d20 2876 6961 205b 4368 686f  nary] (via [Chho
+000027c0: 6554 6169 6769 5d5b 6461 7461 2d76 6961  eTaigi][data-via
+000027d0: 5d29 0d0a 2d20 5b69 5461 6967 6920 4368  ])..- [iTaigi Ch
+000027e0: 696e 6573 652d 5461 6977 616e 6573 6520  inese-Taiwanese 
+000027f0: 436f 6d70 6172 6973 6f6e 2044 6963 7469  Comparison Dicti
+00002800: 6f6e 6172 795d 5b69 7461 6967 692d 6469  onary][itaigi-di
+00002810: 6374 696f 6e61 7279 5d20 2876 6961 205b  ctionary] (via [
+00002820: 4368 686f 6554 6169 6769 5d5b 6461 7461  ChhoeTaigi][data
+00002830: 2d76 6961 5d29 0d0a 0d0a 0d0a 0d0a 3c21  -via])........<!
+00002840: 2d2d 2041 434b 4e4f 574c 4544 4745 4d45  -- ACKNOWLEDGEME
+00002850: 4e54 5320 2d2d 3e0d 0a23 2320 4163 6b6e  NTS -->..## Ackn
+00002860: 6f77 6c65 6467 656d 656e 7473 0d0a 0d0a  owledgements....
+00002870: 2d20 5361 6d75 656c 204a 656e 2028 5b47  - Samuel Jen ([G
+00002880: 6974 6875 625d 5b73 616d 7565 6c2d 6769  ithub][samuel-gi
+00002890: 7468 7562 5d20 c2b7 205b 4c69 6e6b 6564  thub] .. [Linked
+000028a0: 496e 5d5b 7361 6d75 656c 2d6c 696e 6b65  In][samuel-linke
+000028b0: 6469 6e5d 2920 2d20 5461 6977 616e 6573  din]) - Taiwanes
+000028c0: 6520 616e 6420 4d61 6e64 6172 696e 2074  e and Mandarin t
+000028d0: 7261 6e73 6c61 7469 6f6e 0d0a 0d0a 0d0a  ranslation......
+000028e0: 0d0a 3c21 2d2d 204c 4943 454e 4345 202d  ..<!-- LICENCE -
+000028f0: 2d3e 0d0a 2323 204c 6963 656e 6365 0d0a  ->..## Licence..
+00002900: 0d0a 4265 6361 7573 6520 5461 6962 756e  ..Because Taibun
+00002910: 2069 7320 4d49 542d 6c69 6365 6e73 6564   is MIT-licensed
+00002920: 2c20 616e 7920 6465 7665 6c6f 7065 7220  , any developer 
+00002930: 6361 6e20 6573 7365 6e74 6961 6c6c 7920  can essentially 
+00002940: 646f 2077 6861 7465 7665 7220 7468 6579  do whatever they
+00002950: 2077 616e 7420 7769 7468 2069 7420 6173   want with it as
+00002960: 206c 6f6e 6720 6173 2074 6865 7920 696e   long as they in
+00002970: 636c 7564 6520 7468 6520 6f72 6967 696e  clude the origin
+00002980: 616c 2063 6f70 7972 6967 6874 2061 6e64  al copyright and
+00002990: 206c 6963 656e 6365 206e 6f74 6963 6520   licence notice 
+000029a0: 696e 2061 6e79 2063 6f70 6965 7320 6f66  in any copies of
+000029b0: 2074 6865 2073 6f75 7263 6520 636f 6465   the source code
+000029c0: 2e20 4e6f 7465 2c20 7468 6174 2074 6865  . Note, that the
+000029d0: 2064 6174 6120 7573 6564 2062 7920 7468   data used by th
+000029e0: 6520 7061 636b 6167 6520 6973 206c 6963  e package is lic
+000029f0: 656e 7365 6420 756e 6465 7220 6120 6469  ensed under a di
+00002a00: 6666 6572 656e 7420 636f 7079 7269 6768  fferent copyrigh
+00002a10: 742e 0d0a 0d0a 5468 6520 6461 7461 2069  t.....The data i
+00002a20: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00002a30: 205b 4343 2042 592d 5341 2034 2e30 5d5b   [CC BY-SA 4.0][
+00002a40: 6461 7461 2d63 635d 0d0a 0d0a 0d0a 0d0a  data-cc]........
+00002a50: 3c21 2d2d 204d 4152 4b44 4f57 4e20 4c49  <!-- MARKDOWN LI
+00002a60: 4e4b 5320 2d2d 3e0d 0a5b 7465 7374 735d  NKS -->..[tests]
+00002a70: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00002a80: 2e63 6f6d 2f61 6e64 7265 6968 6172 2f74  .com/andreihar/t
+00002a90: 6169 6275 6e2f 6163 7469 6f6e 730d 0a5b  aibun/actions..[
+00002aa0: 7465 7374 732d 6261 6467 655d 3a20 6874  tests-badge]: ht
+00002ab0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00002ac0: 732e 696f 2f67 6974 6875 622f 6163 7469  s.io/github/acti
+00002ad0: 6f6e 732f 776f 726b 666c 6f77 2f73 7461  ons/workflow/sta
+00002ae0: 7475 732f 616e 6472 6569 6861 722f 7461  tus/andreihar/ta
+00002af0: 6962 756e 2f63 692e 7961 6d6c 3f73 7479  ibun/ci.yaml?sty
+00002b00: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00002b10: 266c 6f67 6f3d 6769 7468 7562 0d0a 5b63  &logo=github..[c
+00002b20: 6f6e 7472 6962 7574 6f72 732d 6261 6467  ontributors-badg
+00002b30: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
+00002b40: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00002b50: 622f 636f 6e74 7269 6275 746f 7273 2f61  b/contributors/a
+00002b60: 6e64 7265 6968 6172 2f74 6169 6275 6e3f  ndreihar/taibun?
+00002b70: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
+00002b80: 6467 650d 0a5b 636f 6e74 7269 6275 746f  dge..[contributo
+00002b90: 7273 5d3a 2023 7573 6167 650d 0a5b 7265  rs]: #usage..[re
+00002ba0: 6c65 6173 652d 6261 6467 655d 3a20 6874  lease-badge]: ht
+00002bb0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00002bc0: 732e 696f 2f67 6974 6875 622f 762f 7265  s.io/github/v/re
+00002bd0: 6c65 6173 652f 616e 6472 6569 6861 722f  lease/andreihar/
+00002be0: 7461 6962 756e 3f63 6f6c 6f72 3d33 3836  taibun?color=386
+00002bf0: 3138 6326 7374 796c 653d 666f 722d 7468  18c&style=for-th
+00002c00: 652d 6261 6467 650d 0a5b 7265 6c65 6173  e-badge..[releas
+00002c10: 655d 3a20 6874 7470 733a 2f2f 6769 7468  e]: https://gith
+00002c20: 7562 2e63 6f6d 2f61 6e64 7265 6968 6172  ub.com/andreihar
+00002c30: 2f74 6169 6275 6e2f 7265 6c65 6173 6573  /taibun/releases
+00002c40: 0d0a 5b6c 6963 656e 6365 2d62 6164 6765  ..[licence-badge
+00002c50: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
+00002c60: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00002c70: 2f6c 6963 656e 7365 2f61 6e64 7265 6968  /license/andreih
+00002c80: 6172 2f74 6169 6275 6e3f 636f 6c6f 723d  ar/taibun?color=
+00002c90: 3030 3030 3030 2673 7479 6c65 3d66 6f72  000000&style=for
+00002ca0: 2d74 6865 2d62 6164 6765 0d0a 5b6c 6963  -the-badge..[lic
+00002cb0: 656e 6365 5d3a 204c 4943 454e 5345 0d0a  ence]: LICENSE..
+00002cc0: 5b6c 696e 6b65 6469 6e2d 6261 6467 655d  [linkedin-badge]
+00002cd0: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
+00002ce0: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+00002cf0: 696e 6b65 6449 6e2d 3030 3737 4235 3f73  inkedIn-0077B5?s
+00002d00: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+00002d10: 6765 266c 6f67 6f3d 6c69 6e6b 6564 696e  ge&logo=linkedin
+00002d20: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
+00002d30: 0d0a 5b6c 696e 6b65 6469 6e5d 3a20 6874  ..[linkedin]: ht
+00002d40: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
+00002d50: 696e 2e63 6f6d 2f69 6e2f 616e 6472 6569  in.com/in/andrei
+00002d60: 2d68 6172 6261 6368 6f76 2f0d 0a0d 0a5b  -harbachov/....[
+00002d70: 7079 7069 5d3a 2068 7474 7073 3a2f 2f70  pypi]: https://p
+00002d80: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00002d90: 7461 6962 756e 0d0a 5b62 7567 5d3a 2068  taibun..[bug]: h
+00002da0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002db0: 6d2f 616e 6472 6569 6861 722f 7461 6962  m/andreihar/taib
+00002dc0: 756e 2f69 7373 7565 730d 0a5b 6f6e 6c69  un/issues..[onli
+00002dd0: 6e65 2d64 6963 7469 6f6e 6172 795d 3a20  ne-dictionary]: 
+00002de0: 6874 7470 3a2f 2f69 7031 3934 3039 372e  http://ip194097.
+00002df0: 6e74 6375 2e65 6475 2e74 772f 756e 6769  ntcu.edu.tw/ungi
+00002e00: 616e 2f73 6f61 6e6e 7465 6e67 2f63 6869  an/soannteng/chi
+00002e10: 6c2f 5461 6968 6f61 2e61 7370 0d0a 5b69  l/Taihoa.asp..[i
+00002e20: 7461 6967 692d 6469 6374 696f 6e61 7279  taigi-dictionary
+00002e30: 5d3a 2068 7474 7073 3a2f 2f69 7461 6967  ]: https://itaig
+00002e40: 692e 7477 2f0d 0a5b 6461 7461 2d76 6961  i.tw/..[data-via
+00002e50: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00002e60: 622e 636f 6d2f 4368 686f 6554 6169 6769  b.com/ChhoeTaigi
+00002e70: 2f43 6868 6f65 5461 6967 6944 6174 6162  /ChhoeTaigiDatab
+00002e80: 6173 650d 0a5b 6461 7461 2d63 635d 3a20  ase..[data-cc]: 
+00002e90: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
+00002ea0: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
+00002eb0: 6e73 6573 2f62 792d 7361 2f34 2e30 2f64  nses/by-sa/4.0/d
+00002ec0: 6565 642e 656e 0d0a 5b73 616d 7565 6c2d  eed.en..[samuel-
+00002ed0: 6769 7468 7562 5d3a 2068 7474 7073 3a2f  github]: https:/
+00002ee0: 2f67 6974 6875 622e 636f 6d2f 5353 5361  /github.com/SSSa
+00002ef0: 6d0d 0a5b 7361 6d75 656c 2d6c 696e 6b65  m..[samuel-linke
+00002f00: 6469 6e5d 3a20 6874 7470 733a 2f2f 7777  din]: https://ww
+00002f10: 772e 6c69 6e6b 6564 696e 2e63 6f6d 2f69  w.linkedin.com/i
+00002f20: 6e2f 7361 6d75 656c 2d6a 656e 2f0d 0a0d  n/samuel-jen/...
+00002f30: 0a5b 7461 696c 6f2d 7769 6b69 5d3a 2068  .[tailo-wiki]: h
+00002f40: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00002f50: 6469 612e 6f72 672f 7769 6b69 2f54 2543  dia.org/wiki/T%C
+00002f60: 3325 4132 692d 7525 4333 2541 326e 5f4c  3%A2i-u%C3%A2n_L
+00002f70: 2543 3325 4234 2d6d 2543 3325 4131 2d6a  %C3%B4-m%C3%A1-j
+00002f80: 2543 3425 4142 5f50 6869 6e67 2d69 6d5f  %C4%AB_Phing-im_
+00002f90: 486f 6e67 2d25 4333 2541 306e 0d0a 5b70  Hong-%C3%A0n..[p
+00002fa0: 6f6a 2d77 696b 695d 3a20 6874 7470 733a  oj-wiki]: https:
+00002fb0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00002fc0: 7267 2f77 696b 692f 5065 2543 4325 3844  rg/wiki/Pe%CC%8D
+00002fd0: 682d 2543 3525 3844 652d 6a25 4334 2541  h-%C5%8De-j%C4%A
+00002fe0: 420d 0a5b 7a68 7579 696e 2d77 696b 695d  B..[zhuyin-wiki]
+00002ff0: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
+00003000: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00003010: 5461 6977 616e 6573 655f 5068 6f6e 6574  Taiwanese_Phonet
+00003020: 6963 5f53 796d 626f 6c73 0d0a 5b74 6c70  ic_Symbols..[tlp
+00003030: 612d 7769 6b69 5d3a 2068 7474 7073 3a2f  a-wiki]: https:/
+00003040: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00003050: 672f 7769 6b69 2f54 6169 7761 6e65 7365  g/wiki/Taiwanese
+00003060: 5f4c 616e 6775 6167 655f 5068 6f6e 6574  _Language_Phonet
+00003070: 6963 5f41 6c70 6861 6265 740d 0a5b 7069  ic_Alphabet..[pi
+00003080: 6e67 7969 6d2d 7769 6b69 5d3a 2068 7474  ngyim-wiki]: htt
+00003090: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+000030a0: 612e 6f72 672f 7769 6b69 2f42 6225 4333  a.org/wiki/Bb%C3
+000030b0: 2541 316e 6c25 4333 2541 316d 5f70 2543  %A1nl%C3%A1m_p%C
+000030c0: 3325 4143 6e67 7925 4334 2541 426d 0d0a  3%ACngy%C4%ABm..
+000030d0: 5b74 6f6e 6769 6f6e 672d 7769 6b69 5d3a  [tongiong-wiki]:
+000030e0: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+000030f0: 7065 6469 612e 6f72 672f 7769 6b69 2f44  pedia.org/wiki/D
+00003100: 6125 4334 2541 422d 6768 2543 3325 4145  a%C4%AB-gh%C3%AE
+00003110: 5f74 2543 3525 3844 6e67 2d69 2543 3525  _t%C5%8Dng-i%C5%
+00003120: 3844 6e67 5f70 2543 3425 4142 6e67 2d69  8Dng_p%C4%ABng-i
+00003130: 6d0d 0a5b 6970 612d 7769 6b69 5d3a 2068  m..[ipa-wiki]: h
+00003140: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00003150: 6469 612e 6f72 672f 7769 6b69 2f49 6e74  dia.org/wiki/Int
+00003160: 6572 6e61 7469 6f6e 616c 5f50 686f 6e65  ernational_Phone
+00003170: 7469 635f 416c 7068 6162 6574 0d0a 5b7a  tic_Alphabet..[z
+00003180: 6861 6e67 7a68 6f75 2d77 696b 695d 3a20  hangzhou-wiki]: 
+00003190: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+000031a0: 6564 6961 2e6f 7267 2f77 696b 692f 5a68  edia.org/wiki/Zh
+000031b0: 616e 677a 686f 755f 6469 616c 6563 7473  angzhou_dialects
+000031c0: 0d0a 5b71 7561 6e7a 686f 752d 7769 6b69  ..[quanzhou-wiki
+000031d0: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
+000031e0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+000031f0: 2f51 7561 6e7a 686f 755f 6469 616c 6563  /Quanzhou_dialec
+00003200: 7473 0d0a 5b6e 6c74 6b2d 746f 6b65 6e69  ts..[nltk-tokeni
+00003210: 7a65 5d3a 2068 7474 7073 3a2f 2f6e 6c74  ze]: https://nlt
+00003220: 6b2e 6f72 672f 6170 692f 6e6c 746b 2e74  k.org/api/nltk.t
+00003230: 6f6b 656e 697a 652e 6874 6d6c 0d0a 5b73  okenize.html..[s
+00003240: 616e 6468 692d 7769 6b69 5d3a 2068 7474  andhi-wiki]: htt
+00003250: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00003260: 612e 6f72 672f 7769 6b69 2f54 6169 7761  a.org/wiki/Taiwa
+00003270: 6e65 7365 5f48 6f6b 6b69 656e 2354 6f6e  nese_Hokkien#Ton
+00003280: 6525 3230 7361 6e64 6869 3a7e 3a74 6578  e%20sandhi:~:tex
+00003290: 743d 7468 6e67 2545 3225 3946 2541 3925  t=thng%E2%9F%A9%
+000032a0: 3230 2825 3232 736f 7570 2532 3229 2e2d  20(%22soup%22).-
+000032b0: 2c54 6f6e 6525 3230 7361 6e64 6869 2c2d  ,Tone%20sandhi,-
+000032c0: 2535 4265 6469 7425 3544 0d0a            %5Bedit%5D..
```

### Comparing `example990420-0.0.7/README.md` & `example990420-1.1.0/example990420.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,621 +1,813 @@
-00000000: 3c21 2d2d 2050 524f 4a45 4354 204c 4f47  <!-- PROJECT LOG
-00000010: 4f20 2d2d 3e0d 0a3c 6469 7620 616c 6967  O -->..<div alig
-00000020: 6e3d 2263 656e 7465 7222 3e0d 0a0d 0a23  n="center">....#
-00000030: 20e5 8fb0 e696 8720 7c20 54c3 a269 2d62   ...... | T..i-b
-00000040: c3bb 6e0d 0a0d 0a3c 212d 2d20 5052 4f4a  ..n....<!-- PROJ
-00000050: 4543 5420 5348 4945 4c44 5320 2d2d 3e0d  ECT SHIELDS -->.
-00000060: 0a5b 215b 436f 6e74 7269 6275 746f 7273  .[![Contributors
-00000070: 5d5b 636f 6e74 7269 6275 746f 7273 2d62  ][contributors-b
-00000080: 6164 6765 5d5d 5b63 6f6e 7472 6962 7574  adge]][contribut
-00000090: 6f72 735d 0d0a 5b21 5b52 656c 6561 7365  ors]..[![Release
-000000a0: 5d5b 7265 6c65 6173 652d 6261 6467 655d  ][release-badge]
-000000b0: 5d5b 7265 6c65 6173 655d 0d0a 5b21 5b4c  ][release]..[![L
-000000c0: 6963 656e 6365 5d5b 6c69 6365 6e63 652d  icence][licence-
-000000d0: 6261 6467 655d 5d5b 6c69 6365 6e63 655d  badge]][licence]
-000000e0: 0d0a 5b21 5b4c 696e 6b65 6449 6e5d 5b6c  ..[![LinkedIn][l
-000000f0: 696e 6b65 6469 6e2d 6261 6467 655d 5d5b  inkedin-badge]][
-00000100: 6c69 6e6b 6564 696e 5d0d 0a0d 0a2a 2a54  linkedin]....**T
-00000110: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
-00000120: 2074 7261 6e73 6c69 7465 7261 746f 7220   transliterator 
-00000130: 6672 6f6d 2043 6869 6e65 7365 2063 6861  from Chinese cha
-00000140: 7261 6374 6572 732a 2a0d 0a0d 0a49 7420  racters**....It 
-00000150: 6861 7320 6d65 7468 6f64 7320 7468 6174  has methods that
-00000160: 2061 6c6c 6f77 2074 6f20 6375 7374 6f6d   allow to custom
-00000170: 6973 6520 7472 616e 736c 6974 6572 6174  ise transliterat
-00000180: 696f 6e20 616e 6420 7265 7472 6965 7665  ion and retrieve
-00000190: 2061 6e79 206e 6563 6573 7361 7279 2069   any necessary i
-000001a0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-000001b0: 2054 6169 7761 6e65 7365 2048 6f6b 6b69   Taiwanese Hokki
-000001c0: 656e 2070 726f 6e75 6e63 6961 7469 6f6e  en pronunciation
-000001d0: 2e3c 6272 202f 3e0d 0a49 6e63 6c75 6465  .<br />..Include
-000001e0: 7320 776f 7264 2074 6f6b 656e 6973 6572  s word tokeniser
-000001f0: 2066 6f72 2054 6169 7761 6e65 7365 2048   for Taiwanese H
-00000200: 6f6b 6b69 656e 2e0d 0a0d 0a5b 5265 706f  okkien.....[Repo
-00000210: 7274 2042 7567 5d5b 6275 675d 20e2 80a2  rt Bug][bug] ...
-00000220: 0d0a 5b50 7950 495d 5b70 7970 695d 0d0a  ..[PyPI][pypi]..
-00000230: 0d0a 3c2f 6469 763e 0d0a 0d0a 0d0a 2d2d  ..</div>......--
-00000240: 2d0d 0a0d 0a0d 0a3c 212d 2d20 5441 424c  -......<!-- TABL
-00000250: 4520 4f46 2043 4f4e 5445 4e54 5320 2d2d  E OF CONTENTS --
-00000260: 3e0d 0a3c 6465 7461 696c 7320 6f70 656e  >..<details open
-00000270: 3e0d 0a20 203c 7375 6d6d 6172 793e 5461  >..  <summary>Ta
-00000280: 626c 6520 6f66 2043 6f6e 7465 6e74 733c  ble of Contents<
-00000290: 2f73 756d 6d61 7279 3e0d 0a20 203c 6f6c  /summary>..  <ol
-000002a0: 3e0d 0a20 2020 203c 6c69 3e3c 6120 6872  >..    <li><a hr
-000002b0: 6566 3d22 2369 6e73 7461 6c6c 223e 496e  ef="#install">In
-000002c0: 7374 616c 6c3c 2f61 3e3c 2f6c 693e 0d0a  stall</a></li>..
-000002d0: 2020 2020 3c6c 693e 0d0a 2020 2020 2020      <li>..      
-000002e0: 3c61 2068 7265 663d 2223 7573 6167 6522  <a href="#usage"
-000002f0: 3e55 7361 6765 3c2f 613e 0d0a 2020 2020  >Usage</a>..    
-00000300: 2020 3c75 6c3e 0d0a 2020 2020 2020 2020    <ul>..        
-00000310: 3c6c 693e 0d0a 2020 2020 2020 2020 2020  <li>..          
-00000320: 3c61 2068 7265 663d 2223 636f 6e76 6572  <a href="#conver
-00000330: 7465 7222 3e43 6f6e 7665 7274 6572 3c2f  ter">Converter</
-00000340: 613e 0d0a 2020 2020 2020 2020 2020 3c75  a>..          <u
-00000350: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
-00000360: 3c6c 693e 3c61 2068 7265 663d 2223 7379  <li><a href="#sy
-00000370: 7374 656d 223e 5379 7374 656d 3c2f 613e  stem">System</a>
-00000380: 3c2f 6c69 3e0d 0a20 2020 2020 2020 2020  </li>..         
-00000390: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-000003a0: 2364 6961 6c65 6374 223e 4469 616c 6563  #dialect">Dialec
-000003b0: 743c 2f61 3e3c 2f6c 693e 0d0a 2020 2020  t</a></li>..    
-000003c0: 2020 2020 2020 2020 3c6c 693e 3c61 2068          <li><a h
-000003d0: 7265 663d 2223 666f 726d 6174 223e 466f  ref="#format">Fo
-000003e0: 726d 6174 3c2f 613e 3c2f 6c69 3e0d 0a20  rmat</a></li>.. 
-000003f0: 2020 2020 2020 2020 2020 203c 6c69 3e3c             <li><
-00000400: 6120 6872 6566 3d22 2364 656c 696d 6974  a href="#delimit
-00000410: 6572 223e 4465 6c69 6d69 7465 723c 2f61  er">Delimiter</a
-00000420: 3e3c 2f6c 693e 0d0a 2020 2020 2020 2020  ></li>..        
-00000430: 2020 2020 3c6c 693e 3c61 2068 7265 663d      <li><a href=
-00000440: 2223 7361 6e64 6869 223e 5361 6e64 6869  "#sandhi">Sandhi
-00000450: 3c2f 613e 3c2f 6c69 3e0d 0a20 2020 2020  </a></li>..     
-00000460: 2020 2020 2020 203c 6c69 3e3c 6120 6872         <li><a hr
-00000470: 6566 3d22 2370 756e 6374 7561 7469 6f6e  ef="#punctuation
-00000480: 223e 5075 6e63 7475 6174 696f 6e3c 2f61  ">Punctuation</a
-00000490: 3e3c 2f6c 693e 0d0a 2020 2020 2020 2020  ></li>..        
-000004a0: 2020 3c2f 756c 3e0d 0a20 2020 2020 2020    </ul>..       
-000004b0: 203c 2f6c 693e 0d0a 2020 2020 2020 2020   </li>..        
-000004c0: 3c6c 693e 3c61 2068 7265 663d 2223 746f  <li><a href="#to
-000004d0: 6b65 6e69 7365 7222 3e54 6f6b 656e 6973  keniser">Tokenis
-000004e0: 6572 3c2f 613e 3c2f 6c69 3e0d 0a20 2020  er</a></li>..   
-000004f0: 2020 203c 2f75 6c3e 0d0a 2020 2020 3c2f     </ul>..    </
-00000500: 6c69 3e0d 0a20 2020 203c 6c69 3e3c 6120  li>..    <li><a 
-00000510: 6872 6566 3d22 2365 7861 6d70 6c65 223e  href="#example">
-00000520: 4578 616d 706c 653c 2f61 3e3c 2f6c 693e  Example</a></li>
-00000530: 0d0a 2020 2020 3c6c 693e 3c61 2068 7265  ..    <li><a hre
-00000540: 663d 2223 6461 7461 223e 4461 7461 3c2f  f="#data">Data</
-00000550: 613e 3c2f 6c69 3e0d 0a20 2020 203c 6c69  a></li>..    <li
-00000560: 3e3c 6120 6872 6566 3d22 236c 6963 656e  ><a href="#licen
-00000570: 6365 223e 4c69 6365 6e63 653c 2f61 3e3c  ce">Licence</a><
-00000580: 2f6c 693e 0d0a 2020 3c2f 6f6c 3e0d 0a3c  /li>..  </ol>..<
-00000590: 2f64 6574 6169 6c73 3e0d 0a0d 0a0d 0a3c  /details>......<
-000005a0: 212d 2d20 494e 5354 414c 4c20 2d2d 3e0d  !-- INSTALL -->.
-000005b0: 0a23 2320 496e 7374 616c 6c0d 0a0d 0a54  .## Install....T
-000005c0: 6169 6275 6e20 6361 6e20 6265 2069 6e73  aibun can be ins
-000005d0: 7461 6c6c 6564 2066 726f 6d20 5b70 7970  talled from [pyp
-000005e0: 695d 5b70 7970 695d 0d0a 0d0a 6060 6062  i][pypi]....```b
-000005f0: 6173 680d 0a24 2070 6970 2069 6e73 7461  ash..$ pip insta
-00000600: 6c6c 2074 6169 6275 6e0d 0a60 6060 0d0a  ll taibun..```..
-00000610: 0d0a 0d0a 3c21 2d2d 2055 5341 4745 202d  ....<!-- USAGE -
-00000620: 2d3e 0d0a 2323 2055 7361 6765 0d0a 0d0a  ->..## Usage....
-00000630: 2323 2320 436f 6e76 6572 7465 720d 0a0d  ### Converter...
-00000640: 0a60 436f 6e76 6572 7465 7260 2063 6c61  .`Converter` cla
-00000650: 7373 2074 7261 6e73 6c69 7465 7261 7465  ss transliterate
-00000660: 7320 7468 6520 4368 696e 6573 6520 6368  s the Chinese ch
-00000670: 6172 6163 7465 7273 2074 6f20 7468 6520  aracters to the 
-00000680: 6368 6f73 656e 2074 7261 6e73 6c69 7465  chosen translite
-00000690: 7261 7469 6f6e 2073 7973 7465 6d20 7769  ration system wi
-000006a0: 7468 2070 6172 616d 6574 6572 7320 7370  th parameters sp
-000006b0: 6563 6966 6965 6420 6279 2074 6865 2064  ecified by the d
-000006c0: 6576 656c 6f70 6572 2e20 576f 726b 7320  eveloper. Works 
-000006d0: 666f 7220 626f 7468 2054 7261 6469 7469  for both Traditi
-000006e0: 6f6e 616c 2061 6e64 2053 696d 706c 6966  onal and Simplif
-000006f0: 6965 6420 6368 6172 6163 7465 7273 2e0d  ied characters..
-00000700: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 2320  ...```python..# 
-00000710: 636f 6e73 7472 7563 746f 720d 0a63 203d  constructor..c =
-00000720: 2043 6f6e 7665 7274 6572 2873 7973 7465   Converter(syste
-00000730: 6d2c 2064 6961 6c65 6374 2c20 666f 726d  m, dialect, form
-00000740: 6174 2c20 6465 6c69 6d69 7465 722c 2073  at, delimiter, s
-00000750: 616e 6468 692c 2070 756e 6374 7561 7469  andhi, punctuati
-00000760: 6f6e 290d 0a0d 0a23 2074 7261 6e73 6c69  on)....# transli
-00000770: 7465 7261 7465 2043 6869 6e65 7365 2063  terate Chinese c
-00000780: 6861 7261 6374 6572 730d 0a63 2e67 6574  haracters..c.get
-00000790: 2869 6e70 7574 290d 0a0d 0a23 2063 6f6e  (input)....# con
-000007a0: 7665 7274 2053 696d 706c 6966 6965 6420  vert Simplified 
-000007b0: 4368 696e 6573 6520 6368 6172 6163 7465  Chinese characte
-000007c0: 7273 2074 6f20 5472 6164 6974 696f 6e61  rs to Traditiona
-000007d0: 6c20 4368 696e 6573 6520 4368 6172 6163  l Chinese Charac
-000007e0: 7465 7273 0d0a 632e 746f 5f74 7261 6469  ters..c.to_tradi
-000007f0: 7469 6f6e 616c 2869 6e70 7574 290d 0a60  tional(input)..`
-00000800: 6060 0d0a 0d0a 2323 2323 2053 7973 7465  ``....#### Syste
-00000810: 6d0d 0a0d 0a60 7379 7374 656d 6020 5374  m....`system` St
-00000820: 7269 6e67 202d 2073 7973 7465 6d20 6f66  ring - system of
-00000830: 2074 7261 6e73 6c69 7465 7261 7469 6f6e   transliteration
-00000840: 2e0d 0a0d 0a2a 2060 5461 696c 6f60 2028  .....* `Tailo` (
-00000850: 6465 6661 756c 7429 202d 205b 54c3 a269  default) - [T..i
-00000860: 2d75 c3a2 6e20 4cc3 b42d 6dc3 a12d 6ac4  -u..n L..-m..-j.
-00000870: ab20 5068 696e 672d 696d 2048 6f6e 672d  . Phing-im Hong-
-00000880: c3a0 6e5d 5b74 6169 6c6f 2d77 696b 695d  ..n][tailo-wiki]
-00000890: 0d0a 2a20 6050 4f4a 6020 2d20 5b50 65cc  ..* `POJ` - [Pe.
-000008a0: 8d68 2dc5 8d65 2d6a c4ab 5d5b 706f 6a2d  .h-..e-j..][poj-
-000008b0: 7769 6b69 5d0d 0a2a 2060 5a68 7579 696e  wiki]..* `Zhuyin
-000008c0: 6020 2d20 5b54 6169 7761 6e65 7365 2050  ` - [Taiwanese P
-000008d0: 686f 6e65 7469 6320 5379 6d62 6f6c 735d  honetic Symbols]
-000008e0: 5b7a 6875 7969 6e2d 7769 6b69 5d0d 0a2a  [zhuyin-wiki]..*
-000008f0: 2060 544c 5041 6020 2d20 5b54 6169 7761   `TLPA` - [Taiwa
-00000900: 6e65 7365 204c 616e 6775 6167 6520 5068  nese Language Ph
-00000910: 6f6e 6574 6963 2041 6c70 6861 6265 745d  onetic Alphabet]
-00000920: 5b74 6c70 612d 7769 6b69 5d0d 0a2a 2060  [tlpa-wiki]..* `
-00000930: 5069 6e67 7969 6d60 202d 205b 4262 c3a1  Pingyim` - [Bb..
-00000940: 6e6c c3a1 6d20 55c4 9320 50c3 ac6e 6779  nl..m U.. P..ngy
-00000950: c4ab 6d20 48c5 8d6e 6727 c3a0 6e5d 5b70  ..m H..ng'..n][p
-00000960: 696e 6779 696d 2d77 696b 695d 0d0a 2a20  ingyim-wiki]..* 
-00000970: 6054 6f6e 6769 6f6e 6760 202d 205b 4461  `Tongiong` - [Da
-00000980: c4ab 2d67 68c3 ae20 54c5 8d6e 672d 69c5  ..-gh.. T..ng-i.
-00000990: 8d6e 6720 50c4 ab6e 672d 696d 5d5b 746f  .ng P..ng-im][to
-000009a0: 6e67 696f 6e67 2d77 696b 695d 0d0a 0d0a  ngiong-wiki]....
-000009b0: 7c20 7465 7874 207c 2054 6169 6c6f 2020  | text | Tailo  
-000009c0: 207c 2050 4f4a 2020 2020 207c 205a 6875   | POJ     | Zhu
-000009d0: 7969 6e20 2020 2020 207c 2054 4c50 4120  yin      | TLPA 
-000009e0: 2020 2020 207c 2050 696e 6779 696d 207c       | Pingyim |
-000009f0: 2054 6f6e 6769 6f6e 6720 7c0d 0a7c 2d2d   Tongiong |..|--
-00000a00: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d  ----|---------|-
-00000a10: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00000a20: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000a30: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  --|---------|---
-00000a40: 2d2d 2d2d 2d2d 2d7c 0d0a 7c20 e887 bae7  -------|..| ....
-00000a50: 81a3 207c 2054 c3a2 692d 75c3 a26e 207c  .. | T..i-u..n |
-00000a60: 2054 c3a2 692d 6fc3 a26e 207c 20e3 8489   T..i-o..n | ...
-00000a70: e384 9ecb 8a20 e384 a8e3 84a2 cb8a 207c  ..... ........ |
-00000a80: 2054 6169 3520 7561 6e35 207c 2044 c3a1   Tai5 uan5 | D..
-00000a90: 6977 c3a1 6e20 207c 2054 c481 692d 75c7  iw..n  | T..i-u.
-00000aa0: 8e6e 2020 7c0d 0a0d 0a0d 0a23 2323 2320  .n  |......#### 
-00000ab0: 4469 616c 6563 740d 0a0d 0a60 6469 616c  Dialect....`dial
-00000ac0: 6563 7460 2053 7472 696e 6720 2d20 7072  ect` String - pr
-00000ad0: 6566 6572 7265 6420 7072 6f6e 756e 6369  eferred pronunci
-00000ae0: 6174 696f 6e2e 0d0a 0d0a 2a20 6073 6f75  ation.....* `sou
-00000af0: 7468 6020 2864 6566 6175 6c74 2920 2d20  th` (default) - 
-00000b00: 5b5a 6861 6e67 7a68 6f75 5d5b 7a68 616e  [Zhangzhou][zhan
-00000b10: 677a 686f 752d 7769 6b69 5d2d 6c65 616e  gzhou-wiki]-lean
-00000b20: 696e 6720 7072 6f6e 756e 6369 6174 696f  ing pronunciatio
-00000b30: 6e0d 0a2a 2060 6e6f 7274 6860 202d 205b  n..* `north` - [
-00000b40: 5175 616e 7a68 6f75 5d5b 7175 616e 7a68  Quanzhou][quanzh
-00000b50: 6f75 2d77 696b 695d 2d6c 6561 6e69 6e67  ou-wiki]-leaning
-00000b60: 2070 726f 6e75 6e63 6961 7469 6f6e 0d0a   pronunciation..
-00000b70: 0d0a 7c20 7465 7874 2020 207c 2073 6f75  ..| text   | sou
-00000b80: 7468 2020 2020 2020 2020 207c 206e 6f72  th         | nor
-00000b90: 7468 2020 2020 2020 2020 207c 0d0a 7c2d  th         |..|-
-00000ba0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000bb0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000bc0: 2d2d 2d2d 2d2d 2d7c 0d0a 7c20 e4ba 94e6  -------|..| ....
-00000bd0: 9c88 e7af 8020 7c20 47c5 8d6f 2d67 7565  ..... | G..o-gue
-00000be0: cc8d 682d 7473 6568 207c 2047 c58d 6f2d  ..h-tseh | G..o-
-00000bf0: 6765 cc8d 682d 7473 7565 6820 7c0d 0a0d  ge..h-tsueh |...
-00000c00: 0a0d 0a23 2323 2320 466f 726d 6174 0d0a  ...#### Format..
-00000c10: 0d0a 6066 6f72 6d61 7460 2053 7472 696e  ..`format` Strin
-00000c20: 6720 2d20 666f 726d 6174 2069 6e20 7768  g - format in wh
-00000c30: 6963 6820 746f 6e65 7320 7769 6c6c 2062  ich tones will b
-00000c40: 6520 7265 7072 6573 656e 7465 6420 696e  e represented in
-00000c50: 2074 6865 2063 6f6e 7665 7274 6564 2073   the converted s
-00000c60: 656e 7465 6e63 652e 0d0a 0d0a 2a20 606d  entence.....* `m
-00000c70: 6172 6b60 2028 6465 6661 756c 7429 202d  ark` (default) -
-00000c80: 2075 7365 7320 6469 6163 7269 7469 6373   uses diacritics
-00000c90: 2066 6f72 2065 6163 6820 7379 6c6c 6162   for each syllab
-00000ca0: 6c65 2e20 4e6f 7420 6176 6169 6c61 626c  le. Not availabl
-00000cb0: 6520 666f 7220 544c 5041 2e0d 0a2a 2060  e for TLPA...* `
-00000cc0: 6e75 6d62 6572 6020 2d20 6164 6420 6120  number` - add a 
-00000cd0: 6e75 6d62 6572 2077 6869 6368 2072 6570  number which rep
-00000ce0: 7265 7365 6e74 7320 7468 6520 746f 6e65  resents the tone
-00000cf0: 2061 7420 7468 6520 656e 6420 6f66 2074   at the end of t
-00000d00: 6865 2073 796c 6c61 626c 650d 0a2a 2060  he syllable..* `
-00000d10: 7374 7269 7060 202d 2072 656d 6f76 6573  strip` - removes
-00000d20: 2061 6e79 2074 6f6e 6520 6d61 726b 696e   any tone markin
-00000d30: 670d 0a0d 0a7c 2074 6578 7420 7c20 6d61  g....| text | ma
-00000d40: 726b 2020 2020 7c20 6e75 6d62 6572 2020  rk    | number  
-00000d50: 2020 7c20 7374 7269 7020 2020 7c0d 0a7c    | strip   |..|
-00000d60: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000d70: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  |-----------|---
-00000d80: 2d2d 2d2d 2d2d 7c0d 0a7c 20e8 87ba e781  ------|..| .....
-00000d90: a320 7c20 54c3 a269 2d75 c3a2 6e20 7c20  . | T..i-u..n | 
-00000da0: 5461 6935 2d75 616e 3520 7c20 5461 692d  Tai5-uan5 | Tai-
-00000db0: 7561 6e20 7c0d 0a0d 0a0d 0a23 2323 2320  uan |......#### 
-00000dc0: 4465 6c69 6d69 7465 720d 0a0d 0a60 6465  Delimiter....`de
-00000dd0: 6c69 6d69 7465 7260 2053 7472 696e 6720  limiter` String 
-00000de0: 2d20 7365 7473 2074 6865 2064 656c 696d  - sets the delim
-00000df0: 6974 6572 2063 6861 7261 6374 6572 2074  iter character t
-00000e00: 6861 7420 7769 6c6c 2062 6520 706c 6163  hat will be plac
-00000e10: 6564 2069 6e20 6265 7477 6565 6e20 7379  ed in between sy
-00000e20: 6c6c 6162 6c65 7320 6f66 2061 2077 6f72  llables of a wor
-00000e30: 642e 0d0a 0d0a 4465 6661 756c 7420 7661  d.....Default va
-00000e40: 6c75 6520 6465 7065 6e64 7320 6f6e 2074  lue depends on t
-00000e50: 6865 2063 686f 7365 6e20 6073 7973 7465  he chosen `syste
-00000e60: 6d60 3a0d 0a0d 0a2a 2060 272d 2760 202d  m`:....* `'-'` -
-00000e70: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
-00000e80: 4f4a 602c 2060 546f 6e67 696f 6e67 600d  OJ`, `Tongiong`.
-00000e90: 0a2a 2060 2727 6020 2d20 666f 7220 6050  .* `''` - for `P
-00000ea0: 696e 6779 696d 600d 0a2a 2060 2720 2760  ingyim`..* `' '`
-00000eb0: 202d 2066 6f72 2060 5a68 7579 696e 602c   - for `Zhuyin`,
-00000ec0: 2060 544c 5041 600d 0a0d 0a7c 2074 6578   `TLPA`....| tex
-00000ed0: 7420 7c20 272d 2720 2020 2020 7c20 2727  t | '-'     | ''
-00000ee0: 2020 2020 207c 2027 2027 2020 2020 207c       | ' '     |
-00000ef0: 0d0a 7c2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ..|------|------
-00000f00: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ---|--------|---
-00000f10: 2d2d 2d2d 2d2d 7c0d 0a7c 20e8 87ba e781  ------|..| .....
-00000f20: a320 7c20 54c3 a269 2d75 c3a2 6e20 7c20  . | T..i-u..n | 
-00000f30: 54c3 a269 75c3 a26e 207c 2054 c3a2 6920  T..iu..n | T..i 
-00000f40: 75c3 a26e 207c 0d0a 0d0a 0d0a 2323 2323  u..n |......####
-00000f50: 2053 616e 6468 690d 0a0d 0a60 7361 6e64   Sandhi....`sand
-00000f60: 6869 6020 426f 6f6c 6561 6e20 2d20 6170  hi` Boolean - ap
-00000f70: 706c 6965 7320 7468 6520 5b73 616e 6468  plies the [sandh
-00000f80: 6920 7275 6c65 7320 6f66 2054 6169 7761  i rules of Taiwa
-00000f90: 6e65 7365 2048 6f6b 6b69 656e 5d5b 7361  nese Hokkien][sa
-00000fa0: 6e64 6869 2d77 696b 695d 2074 6f20 7379  ndhi-wiki] to sy
-00000fb0: 6c6c 6162 6c65 7320 6f66 2061 2073 696e  llables of a sin
-00000fc0: 676c 6520 776f 7264 2e0d 0a0d 0a44 6566  gle word.....Def
-00000fd0: 6175 6c74 2076 616c 7565 2064 6570 656e  ault value depen
-00000fe0: 6473 206f 6e20 7468 6520 6368 6f73 656e  ds on the chosen
-00000ff0: 2060 7379 7374 656d 603a 0d0a 0d0a 2a20   `system`:....* 
-00001000: 6054 7275 6560 202d 2066 6f72 2060 546f  `True` - for `To
-00001010: 6e67 696f 6e67 600d 0a2a 2060 4661 6c73  ngiong`..* `Fals
-00001020: 6560 202d 2066 6f72 2060 5461 696c 6f60  e` - for `Tailo`
-00001030: 2c20 6050 4f4a 602c 2060 5a68 7579 696e  , `POJ`, `Zhuyin
-00001040: 602c 2060 544c 5041 602c 2060 5069 6e67  `, `TLPA`, `Ping
-00001050: 7969 6d60 0d0a 0d0a 7c20 7465 7874 2020  yim`....| text  
-00001060: 2020 207c 2046 616c 7365 2020 2020 2020     | False      
-00001070: 2020 7c20 5472 7565 2020 2020 2020 2020    | True        
-00001080: 207c 0d0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d7c   |..|----------|
-00001090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-000010a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0d0a  -------------|..
-000010b0: 7c20 e882 b2e5 9ba1 e4bb 94e6 ad8c 207c  | ............ |
-000010c0: 2049 6f2d 67c3 ad6e 2dc3 a12d 6b75 6120   Io-g..n-..-kua 
-000010d0: 7c20 49c5 8d2d 6769 6e2d 612d 6b75 6120  | I..-gin-a-kua 
-000010e0: 7c0d 0a0d 0a53 616e 6468 6920 7275 6c65  |....Sandhi rule
-000010f0: 7320 616c 736f 2063 6861 6e67 6520 6465  s also change de
-00001100: 7065 6e64 696e 6720 6f6e 2074 6865 2064  pending on the d
-00001110: 6961 6c65 6374 2063 686f 7365 6e2e 0d0a  ialect chosen...
-00001120: 0d0a 7c20 7465 7874 207c 206e 6f20 7361  ..| text | no sa
-00001130: 6e64 6869 207c 2073 6f75 7468 2020 207c  ndhi | south   |
-00001140: 206e 6f72 7468 2020 207c 0d0a 7c2d 2d2d   north   |..|---
-00001150: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---|-----------|
-00001160: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
-00001170: 2d2d 2d7c 0d0a 7c20 e887 bae7 81a3 207c  ---|..| ...... |
-00001180: 2054 c3a2 692d 75c3 a26e 2020 207c 2054   T..i-u..n   | T
-00001190: c481 692d 75c3 a26e 207c 2054 c3a0 692d  ..i-u..n | T..i-
-000011a0: 75c3 a26e 207c 0d0a 0d0a 4e6f 7465 2074  u..n |....Note t
-000011b0: 6861 7420 7468 6520 6675 6e63 7469 6f6e  hat the function
-000011c0: 2069 7320 6469 6666 6572 656e 7420 6672   is different fr
-000011d0: 6f6d 2072 6561 6c20 7361 6e64 6869 2072  om real sandhi r
-000011e0: 756c 6573 2c20 7768 6572 6520 6368 616e  ules, where chan
-000011f0: 6765 7320 6172 6520 6170 706c 6965 6420  ges are applied 
-00001200: 746f 2065 7665 7279 2073 696e 676c 6520  to every single 
-00001210: 7379 6c6c 6162 6c65 206f 6620 7468 6520  syllable of the 
-00001220: 7365 6e74 656e 6365 2c20 6e6f 7420 6a75  sentence, not ju
-00001230: 7374 2073 696e 676c 6520 776f 7264 732e  st single words.
-00001240: 0d0a 0d0a 2d20 2a2a 5461 6962 756e 2773  ....- **Taibun's
-00001250: 2073 616e 6468 6920 7275 6c65 732a 2a3a   sandhi rules**:
-00001260: 2054 68c3 a169 2d6b 686f 6e67 2070 c4ab   Th..i-khong p..
-00001270: 6e67 2d69 c3ba 2c20 6cc3 ad6e 2068 c3b3  ng-i.., l..n h..
-00001280: 2120 4cc3 ad6e 2074 7369 c3a0 2d70 c3a1  ! L..n tsi..-p..
-00001290: 2062 75c4 933f 0d0a 2d20 2a2a 4163 7475   bu..?..- **Actu
-000012a0: 616c 2073 616e 6468 6920 7275 6c65 732a  al sandhi rules*
-000012b0: 2a3a 2054 68c3 a169 2d6b 68c5 8d6e 6720  *: Th..i-kh..ng 
-000012c0: 70c4 ab6e 672d 69c3 ba2c 206c 696e 2068  p..ng-i.., lin h
-000012d0: c3b3 2120 4c69 6e20 7473 69c3 a02d 7061  ..! Lin tsi..-pa
-000012e0: 2062 75c4 933f 0d0a 0d0a 0d0a 2323 2323   bu..?......####
-000012f0: 2050 756e 6374 7561 7469 6f6e 0d0a 0d0a   Punctuation....
-00001300: 6070 756e 6374 7561 7469 6f6e 6020 5374  `punctuation` St
-00001310: 7269 6e67 0d0a 0d0a 2a20 6066 6f72 6d61  ring....* `forma
-00001320: 7460 2028 6465 6661 756c 7429 202d 2063  t` (default) - c
-00001330: 6f6e 7665 7274 7320 4368 696e 6573 652d  onverts Chinese-
-00001340: 7374 796c 6520 7075 6e63 7475 6174 696f  style punctuatio
-00001350: 6e20 746f 204c 6174 696e 2d73 7479 6c65  n to Latin-style
-00001360: 2070 756e 6374 7561 7469 6f6e 2061 6e64   punctuation and
-00001370: 2063 6170 6974 616c 6973 6573 2077 6f72   capitalises wor
-00001380: 6473 2061 7420 7468 6520 6265 6769 6e6e  ds at the beginn
-00001390: 696e 6720 6f66 2065 6163 6820 7365 6e74  ing of each sent
-000013a0: 656e 6365 2e0d 0a2a 2060 6e6f 6e65 6020  ence...* `none` 
-000013b0: 2d20 7072 6573 6572 7665 7320 4368 696e  - preserves Chin
-000013c0: 6573 652d 7374 796c 6520 7075 6e63 7475  ese-style punctu
-000013d0: 6174 696f 6e20 616e 6420 646f 6573 6e27  ation and doesn'
-000013e0: 7420 6361 7069 7461 6c69 7365 2077 6f72  t capitalise wor
-000013f0: 6473 2061 7420 7468 6520 6265 6769 6e6e  ds at the beginn
-00001400: 696e 6720 6f66 206e 6577 2073 656e 7465  ing of new sente
-00001410: 6e63 6573 2e0d 0a0d 0a7c 2074 6578 7420  nces.....| text 
-00001420: 7c20 666f 726d 6174 207c 206e 6f6e 6520  | format | none 
-00001430: 7c0d 0a7c 2d7c 2d7c 2d7c 0d0a 7c20 e980  |..|-|-|-|..| ..
-00001440: 99e6 98af e887 bae5 8d97 efbc 8ce7 b0a1  ................
-00001450: e7a8 b1e3 808c e58d 97e3 808d efbc 88e7  ................
-00001460: 99bd e8a9 b1e5 ad97 efbc 9a54 c3a2 692d  ...........T..i-
-00001470: 6cc3 a26d efbc 9be6 b3a8 e99f b3e7 aca6  l..m............
-00001480: e899 9fef bc9a e384 8ae3 849e cb8a 20e3  .............. .
-00001490: 848b e384 a2cb 8aef bc8c e59c 8be8 aa9e  ................
-000014a0: efbc 9a54 c3a1 696e c3a1 6eef bc89 e380  ...T..in..n.....
-000014b0: 8220 7c20 5473 6520 73c4 ab20 54c3 a269  . | Tse s.. T..i
-000014c0: 2d6c c3a2 6d2c 206b c3a1 6e2d 7473 6869  -l..m, k..n-tshi
-000014d0: 6e67 2022 6cc3 a26d 2220 2850 65cc 8d68  ng "l..m" (Pe..h
-000014e0: 2d75 c493 2d6a c4ab 3a20 54c3 a269 2d6c  -u..-j..: T..i-l
-000014f0: c3a2 6d3b 2074 73c3 b92d 696d 2068 c3bb  ..m; ts..-im h..
-00001500: 2d68 c58d 3a20 e384 8ae3 849e cb8a 20e3  -h..: ........ .
-00001510: 848b e384 a2cb 8a2c 206b 6f6b 2d67 c3ad  ......., kok-g..
-00001520: 3a20 54c3 a169 6ec3 a16e 292e 207c 2074  : T..in..n). | t
-00001530: 7365 2073 c4ab 2054 c3a2 692d 6cc3 a26d  se s.. T..i-l..m
-00001540: efbc 8c6b c3a1 6e2d 7473 6869 6e67 e380  ...k..n-tshing..
-00001550: 8c6c c3a2 6de3 808d efbc 8850 65cc 8d68  .l..m......Pe..h
-00001560: 2d75 c493 2d6a c4ab efbc 9a54 c3a2 692d  -u..-j.....T..i-
-00001570: 6cc3 a26d efbc 9b74 73c3 b92d 696d 2068  l..m...ts..-im h
-00001580: c3bb 2d68 c58d efbc 9ae3 848a e384 9ecb  ..-h............
-00001590: 8a20 e384 8be3 84a2 cb8a efbc 8c6b 6f6b  . ...........kok
-000015a0: 2d67 c3ad efbc 9a54 c3a1 696e c3a1 6eef  -g.....T..in..n.
-000015b0: bc89 e380 8220 7c0d 0a0d 0a23 2323 2054  ..... |....### T
-000015c0: 6f6b 656e 6973 6572 0d0a 0d0a 6054 6f6b  okeniser....`Tok
-000015d0: 656e 6973 6572 6020 636c 6173 7320 7065  eniser` class pe
-000015e0: 7266 6f72 6d73 205b 4e4c 544b 2077 6f72  rforms [NLTK wor
-000015f0: 6470 756e 6374 5f74 6f6b 656e 697a 655d  dpunct_tokenize]
-00001600: 5b6e 6c74 6b2d 746f 6b65 6e69 7a65 5d2d  [nltk-tokenize]-
-00001610: 6c69 6b65 2074 6f6b 656e 6973 6174 696f  like tokenisatio
-00001620: 6e20 6f66 2061 2054 6169 7761 6e65 7365  n of a Taiwanese
-00001630: 2048 6f6b 6b69 656e 2073 656e 7465 6e63   Hokkien sentenc
-00001640: 652e 0d0a 0d0a 6060 6070 7974 686f 6e0d  e.....```python.
-00001650: 0a23 2063 6f6e 7374 7275 6374 6f72 0d0a  .# constructor..
-00001660: 7420 3d20 546f 6b65 6e69 7365 7228 290d  t = Tokeniser().
-00001670: 0a0d 0a23 2074 6f6b 656e 6973 6520 5461  ...# tokenise Ta
-00001680: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
-00001690: 7365 6e74 656e 6365 0d0a 742e 746f 6b65  sentence..t.toke
-000016a0: 6e69 7365 2869 6e70 7574 290d 0a60 6060  nise(input)..```
-000016b0: 0d0a 0d0a 0d0a 3c21 2d2d 2045 5841 4d50  ......<!-- EXAMP
-000016c0: 4c45 202d 2d3e 0d0a 2323 2045 7861 6d70  LE -->..## Examp
-000016d0: 6c65 0d0a 0d0a 6060 6070 7974 686f 6e0d  le....```python.
-000016e0: 0a66 726f 6d20 7461 6962 756e 2069 6d70  .from taibun imp
-000016f0: 6f72 7420 436f 6e76 6572 7465 722c 2054  ort Converter, T
-00001700: 6f6b 656e 6973 6572 0d0a 0d0a 2320 5379  okeniser....# Sy
-00001710: 7374 656d 0d0a 6320 3d20 436f 6e76 6572  stem..c = Conver
-00001720: 7465 7228 2920 2320 5461 696c 6f20 7379  ter() # Tailo sy
-00001730: 7374 656d 2064 6566 6175 6c74 0d0a 632e  stem default..c.
-00001740: 6765 7428 27e5 8588 e794 9fe8 ac9b efbc  get('...........
-00001750: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
-00001760: e380 8227 290d 0a3e 3e20 5369 616e 2d73  ...')..>> Sian-s
-00001770: 696e 6e20 6bc3 b36e 672c 2068 61cc 8d6b  inn k..ng, ha..k
-00001780: 2d73 696e 6720 7469 c481 6d2d 7469 c481  -sing ti..m-ti..
-00001790: 6d20 7468 6961 6e6e 2e0d 0a0d 0a63 203d  m thiann.....c =
-000017a0: 2043 6f6e 7665 7274 6572 2873 7973 7465   Converter(syste
-000017b0: 6d3d 275a 6875 7969 6e27 290d 0a63 2e67  m='Zhuyin')..c.g
-000017c0: 6574 2827 e585 88e7 949f e8ac 9bef bc8c  et('............
-000017d0: e5ad b8e7 949f e681 ace6 81ac e881 bde3  ................
-000017e0: 8082 2729 0d0a 3e3e 20e3 8492 e384 a7e3  ..')..>> .......
-000017f0: 84a2 20e3 8492 e386 aa20 e384 8de3 86b2  .. ...... ......
-00001800: cb8b 2c20 e384 8fe3 849a e384 8d20 e384  .., ......... ..
-00001810: 92e3 84a7 e384 a520 e384 89e3 84a7 e386  ....... ........
-00001820: b0cb ab20 e384 89e3 84a7 e386 b0cb ab20  ... ........... 
-00001830: e384 8ae3 84a7 e386 a92e 0d0a 0d0a 2320  ..............# 
-00001840: 4469 616c 6563 740d 0a63 203d 2043 6f6e  Dialect..c = Con
-00001850: 7665 7274 6572 2829 2023 2073 6f75 7468  verter() # south
-00001860: 2064 6961 6c65 6374 2064 6566 6175 6c74   dialect default
-00001870: 0d0a 632e 6765 7428 22e6 8891 e6ac b2e7  ..c.get(".......
-00001880: 94a8 e7ae b8e9 a39f e9ad 9a22 290d 0a3e  ...........")..>
-00001890: 3e20 4775 c3a1 2062 6568 20c4 ab6e 6720  > Gu.. beh ..ng 
-000018a0: 74c4 ab20 7473 6961 cc8d 6820 68c3 ae0d  t.. tsia..h h...
-000018b0: 0a0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
-000018c0: 2864 6961 6c65 6374 3d27 6e6f 7274 6827  (dialect='north'
-000018d0: 290d 0a63 2e67 6574 2822 e688 91e6 acb2  )..c.get("......
-000018e0: e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a  ............")..
-000018f0: 3e3e 2047 75c3 a120 6275 6568 20c4 ab6e  >> Gu.. bueh ..n
-00001900: 6720 74c5 ab20 7473 6961 cc8d 6820 68c3  g t.. tsia..h h.
-00001910: bb0d 0a0d 0a23 2046 6f72 6d61 740d 0a63  .....# Format..c
-00001920: 203d 2043 6f6e 7665 7274 6572 2829 2023   = Converter() #
-00001930: 2066 6f72 2054 6169 6c6f 2c20 6d61 726b   for Tailo, mark
-00001940: 2062 7920 6465 6661 756c 740d 0a63 2e67   by default..c.g
-00001950: 6574 2822 e794 9fe6 97a5 e5bf abe6 a882  et("............
-00001960: 2229 0d0a 3e3e 2053 656e 6e2d 6a69 cc8d  ")..>> Senn-ji..
-00001970: 7420 6b68 75c3 a069 2d6c 6fcc 8d6b 0d0a  t khu..i-lo..k..
-00001980: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
-00001990: 666f 726d 6174 3d27 6e75 6d62 6572 2729  format='number')
-000019a0: 0d0a 632e 6765 7428 22e7 949f e697 a5e5  ..c.get(".......
-000019b0: bfab e6a8 8222 290d 0a3e 3e20 5365 6e6e  .....")..>> Senn
-000019c0: 312d 6a69 7438 206b 6875 6169 332d 6c6f  1-jit8 khuai3-lo
-000019d0: 6b38 0d0a 0d0a 6320 3d20 436f 6e76 6572  k8....c = Conver
-000019e0: 7465 7228 666f 726d 6174 3d27 7374 7269  ter(format='stri
-000019f0: 7027 290d 0a63 2e67 6574 2822 e794 9fe6  p')..c.get("....
-00001a00: 97a5 e5bf abe6 a882 2229 0d0a 3e3e 2053  ........")..>> S
-00001a10: 656e 6e2d 6a69 7420 6b68 7561 692d 6c6f  enn-jit khuai-lo
-00001a20: 6b0d 0a0d 0a23 2044 656c 696d 6974 6572  k....# Delimiter
-00001a30: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
-00001a40: 6465 6c69 6d69 7465 723d 2727 290d 0a63  delimiter='')..c
-00001a50: 2e67 6574 2822 e585 88e7 949f e8ac 9bef  .get("..........
-00001a60: bc8c e5ad b8e7 949f e681 ace6 81ac e881  ................
-00001a70: bde3 8082 2229 0d0a 3e3e 2053 6961 6e73  ....")..>> Sians
-00001a80: 696e 6e20 6bc3 b36e 672c 2068 61cc 8d6b  inn k..ng, ha..k
-00001a90: 7369 6e67 2074 69c4 816d 7469 c481 6d20  sing ti..mti..m 
-00001aa0: 7468 6961 6e6e 2e0d 0a0d 0a63 203d 2043  thiann.....c = C
-00001ab0: 6f6e 7665 7274 6572 2873 7973 7465 6d3d  onverter(system=
-00001ac0: 2750 696e 6779 696d 272c 2064 656c 696d  'Pingyim', delim
-00001ad0: 6974 6572 3d27 2d27 290d 0a63 2e67 6574  iter='-')..c.get
-00001ae0: 2822 e585 88e7 949f e8ac 9bef bc8c e5ad  ("..............
-00001af0: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
-00001b00: 2229 0d0a 3e3e 2053 69c4 816e 2d73 6ec4  ")..>> Si..n-sn.
-00001b10: ab20 67c7 926e 672c 2068 c3a1 672d 73c4  . g..ng, h..g-s.
-00001b20: ab6e 6720 6469 c3a2 6d2d 6469 c3a2 6d20  .ng di..m-di..m 
-00001b30: 7469 6ec4 812e 0d0a 0d0a 2320 5361 6e64  tin.......# Sand
-00001b40: 6869 0d0a 6320 3d20 436f 6e76 6572 7465  hi..c = Converte
-00001b50: 7228 2920 2320 666f 7220 5461 696c 6f2c  r() # for Tailo,
-00001b60: 2073 616e 6468 6920 4661 6c73 6520 6279   sandhi False by
-00001b70: 2064 6566 6175 6c74 0d0a 632e 6765 7428   default..c.get(
-00001b80: 22e5 8d97 e8bf b4e9 90b5 e8b7 af22 290d  "............").
-00001b90: 0a3e 3e20 4cc3 a26d 2d68 75c3 aa2d 7468  .>> L..m-hu..-th
-00001ba0: 6968 2d6c c58d 6f0d 0a0d 0a63 203d 2043  ih-l..o....c = C
-00001bb0: 6f6e 7665 7274 6572 2873 616e 6468 693d  onverter(sandhi=
-00001bc0: 5472 7565 290d 0a63 2e67 6574 2822 e58d  True)..c.get("..
-00001bd0: 97e8 bfb4 e990 b5e8 b7af 2229 0d0a 3e3e  ..........")..>>
-00001be0: 204c c481 6d2d 6875 c493 2d74 68c3 ad2d   L..m-hu..-th..-
-00001bf0: 6cc5 8d6f 0d0a 0d0a 2320 5075 6e63 7475  l..o....# Punctu
-00001c00: 6174 696f 6e0d 0a63 203d 2043 6f6e 7665  ation..c = Conve
-00001c10: 7274 6572 2829 2023 2066 6f72 6d61 7420  rter() # format 
-00001c20: 7075 6e63 7475 6174 696f 6e20 6465 6661  punctuation defa
-00001c30: 756c 740d 0a63 2e67 6574 2822 e5a4 aae7  ult..c.get("....
-00001c40: a9ba e69c 8be5 8f8b efbc 8ce6 8181 e5a5  ................
-00001c50: bdef bc81 e681 81e9 a39f e9a3 bde6 9caa  ................
-00001c60: efbc 9f22 290d 0a3e 3e20 5468 c3a0 692d  ...")..>> Th..i-
-00001c70: 6b68 6f6e 6720 70c3 ae6e 672d 69c3 ba2c  khong p..ng-i..,
-00001c80: 206c c3ad 6e20 68c3 b321 204c c3ad 6e20   l..n h..! L..n 
-00001c90: 7473 6961 cc8d 682d 70c3 a120 6275 c493  tsia..h-p.. bu..
-00001ca0: 3f0d 0a0d 0a63 203d 2043 6f6e 7665 7274  ?....c = Convert
-00001cb0: 6572 2870 756e 6374 7561 7469 6f6e 3d27  er(punctuation='
-00001cc0: 6e6f 6e65 2729 0d0a 632e 6765 7428 22e5  none')..c.get(".
-00001cd0: a4aa e7a9 bae6 9c8b e58f 8bef bc8c e681  ................
-00001ce0: 81e5 a5bd efbc 81e6 8181 e9a3 9fe9 a3bd  ................
-00001cf0: e69c aaef bc9f 2229 0d0a 3e3e 2074 68c3  ......")..>> th.
-00001d00: a069 2d6b 686f 6e67 2070 c3ae 6e67 2d69  .i-khong p..ng-i
-00001d10: c3ba efbc 8c6c c3ad 6e20 68c3 b3ef bc81  .....l..n h.....
-00001d20: 6cc3 ad6e 2074 7369 61cc 8d68 2d70 c3a1  l..n tsia..h-p..
-00001d30: 2062 75c4 93ef bc9f 0d0a 0d0a 0d0a 2320   bu...........# 
-00001d40: 546f 6b65 6e69 7365 720d 0a74 203d 2054  Tokeniser..t = T
-00001d50: 6f6b 656e 6973 6572 2829 0d0a 742e 746f  okeniser()..t.to
-00001d60: 6b65 6e69 7365 2822 e5a4 aae7 a9ba e69c  kenise("........
-00001d70: 8be5 8f8b efbc 8ce6 8181 e5a5 bdef bc81  ................
-00001d80: e681 81e9 a39f e9a3 bde6 9caa efbc 9f22  ..............."
-00001d90: 290d 0a3e 3e20 5b27 e5a4 aae7 a9ba 272c  )..>> ['......',
-00001da0: 2027 e69c 8be5 8f8b 272c 2027 efbc 8c27   '......', '...'
-00001db0: 2c20 27e6 8181 272c 2027 e5a5 bd27 2c20  , '...', '...', 
-00001dc0: 27ef bc81 272c 2027 e681 8127 2c20 27e9  '...', '...', '.
-00001dd0: a39f e9a3 bd27 2c20 27e6 9caa 272c 2027  .....', '...', '
-00001de0: efbc 9f27 5d0d 0a60 6060 0d0a 0d0a 0d0a  ...']..```......
-00001df0: 3c21 2d2d 2044 4154 4120 2d2d 3e0d 0a23  <!-- DATA -->..#
-00001e00: 2320 4461 7461 0d0a 0d0a 2d20 5b44 6963  # Data....- [Dic
-00001e10: 7469 6f6e 6172 7920 6f66 2046 7265 7175  tionary of Frequ
-00001e20: 656e 746c 792d 5573 6564 2054 6169 7761  ently-Used Taiwa
-00001e30: 6e20 4d69 6e6e 616e 5d5b 6469 6374 696f  n Minnan][dictio
-00001e40: 6e61 7279 5d20 2876 6961 205b 6d6f 6564  nary] (via [moed
-00001e50: 6963 742d 6461 7461 2d74 7762 6c67 5d5b  ict-data-twblg][
-00001e60: 6469 6374 696f 6e61 7279 2d76 6961 5d29  dictionary-via])
-00001e70: 0d0a 0d0a 0d0a 3c21 2d2d 204c 4943 454e  ......<!-- LICEN
-00001e80: 4345 202d 2d3e 0d0a 2323 204c 6963 656e  CE -->..## Licen
-00001e90: 6365 0d0a 0d0a 4265 6361 7573 6520 5461  ce....Because Ta
-00001ea0: 6962 756e 2069 7320 4d49 542d 6c69 6365  ibun is MIT-lice
-00001eb0: 6e73 6564 2c20 616e 7920 6465 7665 6c6f  nsed, any develo
-00001ec0: 7065 7220 6361 6e20 6573 7365 6e74 6961  per can essentia
-00001ed0: 6c6c 7920 646f 2077 6861 7465 7665 7220  lly do whatever 
-00001ee0: 7468 6579 2077 616e 7420 7769 7468 2069  they want with i
-00001ef0: 7420 6173 206c 6f6e 6720 6173 2074 6865  t as long as the
-00001f00: 7920 696e 636c 7564 6520 7468 6520 6f72  y include the or
-00001f10: 6967 696e 616c 2063 6f70 7972 6967 6874  iginal copyright
-00001f20: 2061 6e64 206c 6963 656e 6365 206e 6f74   and licence not
-00001f30: 6963 6520 696e 2061 6e79 2063 6f70 6965  ice in any copie
-00001f40: 7320 6f66 2074 6865 2073 6f75 7263 6520  s of the source 
-00001f50: 636f 6465 2e20 4e6f 7465 2c20 7468 6174  code. Note, that
-00001f60: 2074 6865 2064 6174 6120 7573 6564 2062   the data used b
-00001f70: 7920 7468 6520 7061 636b 6167 6520 6973  y the package is
-00001f80: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
-00001f90: 6120 6469 6666 6572 656e 7420 636f 7079  a different copy
-00001fa0: 7269 6768 742e 0d0a 0d0a 5468 6520 6461  right.....The da
-00001fb0: 7461 2069 7320 6c69 6365 6e73 6564 2075  ta is licensed u
-00001fc0: 6e64 6572 205b 4343 2042 592d 4e44 2033  nder [CC BY-ND 3
-00001fd0: 2e30 2054 575d 5b64 6973 7469 6f6e 6172  .0 TW][distionar
-00001fe0: 792d 6363 5d0d 0a0d 0a0d 0a0d 0a3c 212d  y-cc]........<!-
-00001ff0: 2d20 4d41 524b 444f 574e 204c 494e 4b53  - MARKDOWN LINKS
-00002000: 202d 2d3e 0d0a 5b63 6f6e 7472 6962 7574   -->..[contribut
-00002010: 6f72 732d 6261 6467 655d 3a20 6874 7470  ors-badge]: http
-00002020: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00002030: 696f 2f67 6974 6875 622f 636f 6e74 7269  io/github/contri
-00002040: 6275 746f 7273 2f61 6e64 7265 6968 6172  butors/andreihar
-00002050: 2f74 6169 6275 6e3f 7374 796c 653d 666f  /taibun?style=fo
-00002060: 722d 7468 652d 6261 6467 650d 0a5b 636f  r-the-badge..[co
-00002070: 6e74 7269 6275 746f 7273 5d3a 2023 7573  ntributors]: #us
-00002080: 6167 650d 0a5b 7265 6c65 6173 652d 6261  age..[release-ba
-00002090: 6467 655d 3a20 6874 7470 733a 2f2f 696d  dge]: https://im
-000020a0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-000020b0: 6875 622f 762f 7265 6c65 6173 652f 616e  hub/v/release/an
-000020c0: 6472 6569 6861 722f 7461 6962 756e 3f63  dreihar/taibun?c
-000020d0: 6f6c 6f72 3d33 3836 3138 6326 7374 796c  olor=38618c&styl
-000020e0: 653d 666f 722d 7468 652d 6261 6467 650d  e=for-the-badge.
-000020f0: 0a5b 7265 6c65 6173 655d 3a20 6874 7470  .[release]: http
-00002100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00002110: 6e64 7265 6968 6172 2f74 6169 6275 6e2f  ndreihar/taibun/
-00002120: 7265 6c65 6173 6573 0d0a 5b6c 6963 656e  releases..[licen
-00002130: 6365 2d62 6164 6765 5d3a 2068 7474 7073  ce-badge]: https
-00002140: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00002150: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
-00002160: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
-00002170: 6e2e 7376 673f 636f 6c6f 723d 3030 3030  n.svg?color=0000
-00002180: 3030 2673 7479 6c65 3d66 6f72 2d74 6865  00&style=for-the
-00002190: 2d62 6164 6765 0d0a 5b6c 6963 656e 6365  -badge..[licence
-000021a0: 5d3a 204c 4943 454e 5345 0d0a 5b6c 696e  ]: LICENSE..[lin
-000021b0: 6b65 6469 6e2d 6261 6467 655d 3a20 6874  kedin-badge]: ht
-000021c0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000021d0: 732e 696f 2f62 6164 6765 2f4c 696e 6b65  s.io/badge/Linke
-000021e0: 6449 6e2d 3030 3737 4235 3f73 7479 6c65  dIn-0077B5?style
-000021f0: 3d66 6f72 2d74 6865 2d62 6164 6765 266c  =for-the-badge&l
-00002200: 6f67 6f3d 6c69 6e6b 6564 696e 266c 6f67  ogo=linkedin&log
-00002210: 6f43 6f6c 6f72 3d77 6869 7465 0d0a 5b6c  oColor=white..[l
-00002220: 696e 6b65 6469 6e5d 3a20 6874 7470 733a  inkedin]: https:
-00002230: 2f2f 7777 772e 6c69 6e6b 6564 696e 2e63  //www.linkedin.c
-00002240: 6f6d 2f69 6e2f 616e 6472 6569 2d68 6172  om/in/andrei-har
-00002250: 6261 6368 6f76 2f0d 0a0d 0a5b 7079 7069  bachov/....[pypi
-00002260: 5d3a 2068 7474 7073 3a2f 2f70 7970 692e  ]: https://pypi.
-00002270: 6f72 672f 7072 6f6a 6563 742f 7461 6962  org/project/taib
-00002280: 756e 0d0a 5b62 7567 5d3a 2068 7474 7073  un..[bug]: https
-00002290: 3a2f 2f67 6974 6875 622e 636f 6d2f 616e  ://github.com/an
-000022a0: 6472 6569 6861 722f 7461 6962 756e 2f69  dreihar/taibun/i
-000022b0: 7373 7565 730d 0a5b 6469 6374 696f 6e61  ssues..[dictiona
-000022c0: 7279 5d3a 2068 7474 7073 3a2f 2f74 7762  ry]: https://twb
-000022d0: 6c67 2e64 6963 742e 6564 752e 7477 2f68  lg.dict.edu.tw/h
-000022e0: 6f6c 6f64 6963 745f 6e65 772f 0d0a 5b64  olodict_new/..[d
-000022f0: 6963 7469 6f6e 6172 792d 7669 615d 3a20  ictionary-via]: 
-00002300: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002310: 6f6d 2f67 3076 2f6d 6f65 6469 6374 2d64  om/g0v/moedict-d
-00002320: 6174 612d 7477 626c 670d 0a5b 6469 7374  ata-twblg..[dist
-00002330: 696f 6e61 7279 2d63 635d 3a20 6874 7470  ionary-cc]: http
-00002340: 733a 2f2f 6372 6561 7469 7665 636f 6d6d  s://creativecomm
-00002350: 6f6e 732e 6f72 672f 6c69 6365 6e73 6573  ons.org/licenses
-00002360: 2f62 792d 6e64 2f33 2e30 2f74 772f 6465  /by-nd/3.0/tw/de
-00002370: 6564 2e65 6e0d 0a0d 0a5b 7461 696c 6f2d  ed.en....[tailo-
-00002380: 7769 6b69 5d3a 2068 7474 7073 3a2f 2f65  wiki]: https://e
-00002390: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-000023a0: 7769 6b69 2f54 2543 3325 4132 692d 7525  wiki/T%C3%A2i-u%
-000023b0: 4333 2541 326e 5f4c 2543 3325 4234 2d6d  C3%A2n_L%C3%B4-m
-000023c0: 2543 3325 4131 2d6a 2543 3425 4142 5f50  %C3%A1-j%C4%AB_P
-000023d0: 6869 6e67 2d69 6d5f 486f 6e67 2d25 4333  hing-im_Hong-%C3
-000023e0: 2541 306e 0d0a 5b70 6f6a 2d77 696b 695d  %A0n..[poj-wiki]
-000023f0: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
-00002400: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00002410: 5065 2543 4325 3844 682d 2543 3525 3844  Pe%CC%8Dh-%C5%8D
-00002420: 652d 6a25 4334 2541 420d 0a5b 7a68 7579  e-j%C4%AB..[zhuy
-00002430: 696e 2d77 696b 695d 3a20 6874 7470 733a  in-wiki]: https:
-00002440: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002450: 7267 2f77 696b 692f 5461 6977 616e 6573  rg/wiki/Taiwanes
-00002460: 655f 5068 6f6e 6574 6963 5f53 796d 626f  e_Phonetic_Symbo
-00002470: 6c73 0d0a 5b74 6c70 612d 7769 6b69 5d3a  ls..[tlpa-wiki]:
-00002480: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
-00002490: 7065 6469 612e 6f72 672f 7769 6b69 2f54  pedia.org/wiki/T
-000024a0: 6169 7761 6e65 7365 5f4c 616e 6775 6167  aiwanese_Languag
-000024b0: 655f 5068 6f6e 6574 6963 5f41 6c70 6861  e_Phonetic_Alpha
-000024c0: 6265 740d 0a5b 7069 6e67 7969 6d2d 7769  bet..[pingyim-wi
-000024d0: 6b69 5d3a 2068 7474 7073 3a2f 2f65 6e2e  ki]: https://en.
-000024e0: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-000024f0: 6b69 2f42 6225 4333 2541 316e 6c25 4333  ki/Bb%C3%A1nl%C3
-00002500: 2541 316d 5f70 2543 3325 4143 6e67 7925  %A1m_p%C3%ACngy%
-00002510: 4334 2541 426d 0d0a 5b74 6f6e 6769 6f6e  C4%ABm..[tongion
-00002520: 672d 7769 6b69 5d3a 2068 7474 7073 3a2f  g-wiki]: https:/
-00002530: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00002540: 672f 7769 6b69 2f44 6125 4334 2541 422d  g/wiki/Da%C4%AB-
-00002550: 6768 2543 3325 4145 5f74 2543 3525 3844  gh%C3%AE_t%C5%8D
-00002560: 6e67 2d69 2543 3525 3844 6e67 5f70 2543  ng-i%C5%8Dng_p%C
-00002570: 3425 4142 6e67 2d69 6d0d 0a5b 7a68 616e  4%ABng-im..[zhan
-00002580: 677a 686f 752d 7769 6b69 5d3a 2068 7474  gzhou-wiki]: htt
-00002590: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-000025a0: 612e 6f72 672f 7769 6b69 2f5a 6861 6e67  a.org/wiki/Zhang
-000025b0: 7a68 6f75 5f64 6961 6c65 6374 730d 0a5b  zhou_dialects..[
-000025c0: 7175 616e 7a68 6f75 2d77 696b 695d 3a20  quanzhou-wiki]: 
-000025d0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000025e0: 6564 6961 2e6f 7267 2f77 696b 692f 5175  edia.org/wiki/Qu
-000025f0: 616e 7a68 6f75 5f64 6961 6c65 6374 730d  anzhou_dialects.
-00002600: 0a5b 6e6c 746b 2d74 6f6b 656e 697a 655d  .[nltk-tokenize]
-00002610: 3a20 6874 7470 733a 2f2f 6e6c 746b 2e6f  : https://nltk.o
-00002620: 7267 2f61 7069 2f6e 6c74 6b2e 746f 6b65  rg/api/nltk.toke
-00002630: 6e69 7a65 2e68 746d 6c0d 0a5b 7361 6e64  nize.html..[sand
-00002640: 6869 2d77 696b 695d 3a20 6874 7470 733a  hi-wiki]: https:
-00002650: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002660: 7267 2f77 696b 692f 5461 6977 616e 6573  rg/wiki/Taiwanes
-00002670: 655f 486f 6b6b 6965 6e23 546f 6e65 2532  e_Hokkien#Tone%2
-00002680: 3073 616e 6468 693a 7e3a 7465 7874 3d74  0sandhi:~:text=t
-00002690: 686e 6725 4532 2539 4625 4139 2532 3028  hng%E2%9F%A9%20(
-000026a0: 2532 3273 6f75 7025 3232 292e 2d2c 546f  %22soup%22).-,To
-000026b0: 6e65 2532 3073 616e 6468 692c 2d25 3542  ne%20sandhi,-%5B
-000026c0: 6564 6974 2535 44                        edit%5D
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 2065 7861  : 2.1..Name: exa
+00000020: 6d70 6c65 3939 3034 3230 0d0a 5665 7273  mple990420..Vers
+00000030: 696f 6e3a 2031 2e31 2e30 0d0a 5375 6d6d  ion: 1.1.0..Summ
+00000040: 6172 793a 2054 6169 7761 6e65 7365 2048  ary: Taiwanese H
+00000050: 6f6b 6b69 656e 2054 7261 6e73 6c69 7465  okkien Translite
+00000060: 7261 746f 7220 616e 6420 546f 6b65 6e69  rator and Tokeni
+00000070: 7365 720d 0a48 6f6d 652d 7061 6765 3a20  ser..Home-page: 
+00000080: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000090: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
+000000a0: 6275 6e0d 0a41 7574 686f 723a 2041 6e64  bun..Author: And
+000000b0: 7265 6920 4861 7262 6163 686f 760d 0a41  rei Harbachov..A
+000000c0: 7574 686f 722d 656d 6169 6c3a 2061 6e64  uthor-email: and
+000000d0: 7265 692e 6861 7262 6163 686f 7640 676d  rei.harbachov@gm
+000000e0: 6169 6c2e 636f 6d0d 0a4c 6963 656e 7365  ail.com..License
+000000f0: 3a20 4d49 540d 0a4b 6579 776f 7264 733a  : MIT..Keywords:
+00000100: 2070 7974 686f 6e2c 7461 6977 616e 2c74   python,taiwan,t
+00000110: 6169 7761 6e65 7365 2c74 6169 6769 2c68  aiwanese,taigi,h
+00000120: 6f6b 6b69 656e 2c72 6f6d 616e 697a 6174  okkien,romanizat
+00000130: 696f 6e2c 7472 616e 736c 6974 6572 6174  ion,transliterat
+00000140: 696f 6e2c 7472 616e 736c 6974 6572 6174  ion,transliterat
+00000150: 6f72 2c74 6f6b 656e 697a 6174 696f 6e2c  or,tokenization,
+00000160: 746f 6b65 6e69 7a65 720d 0a43 6c61 7373  tokenizer..Class
+00000170: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+00000180: 5465 7874 2050 726f 6365 7373 696e 6720  Text Processing 
+00000190: 3a3a 204c 696e 6775 6973 7469 630d 0a43  :: Linguistic..C
+000001a0: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
+000001b0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+000001c0: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
+000001d0: 5374 6162 6c65 0d0a 436c 6173 7369 6669  Stable..Classifi
+000001e0: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+000001f0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000200: 6572 730d 0a43 6c61 7373 6966 6965 723a  ers..Classifier:
+00000210: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000230: 3a3a 2033 0d0a 436c 6173 7369 6669 6572  :: 3..Classifier
+00000240: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000250: 656d 203a 3a20 556e 6978 0d0a 436c 6173  em :: Unix..Clas
+00000260: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+00000270: 6720 5379 7374 656d 203a 3a20 4d61 634f  g System :: MacO
+00000280: 5320 3a3a 204d 6163 4f53 2058 0d0a 436c  S :: MacOS X..Cl
+00000290: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+000002a0: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
+000002b0: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
+000002c0: 7773 0d0a 5265 7175 6972 6573 2d50 7974  ws..Requires-Pyt
+000002d0: 686f 6e3a 203e 3d33 2e38 0d0a 4465 7363  hon: >=3.8..Desc
+000002e0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+000002f0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000300: 6f77 6e0d 0a4c 6963 656e 7365 2d46 696c  own..License-Fil
+00000310: 653a 204c 4943 454e 5345 0d0a 0d0a 3c21  e: LICENSE....<!
+00000320: 2d2d 2050 524f 4a45 4354 204c 4f47 4f20  -- PROJECT LOGO 
+00000330: 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c 6469  -->..<br />..<di
+00000340: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00000350: 3e0d 0a20 200d 0a23 2054 6169 6275 6e0d  >..  ..# Taibun.
+00000360: 0a0d 0a0d 0a0d 0a3c 212d 2d20 5052 4f4a  .......<!-- PROJ
+00000370: 4543 5420 5348 4945 4c44 5320 2d2d 3e0d  ECT SHIELDS -->.
+00000380: 0a5b 215b 5465 7374 735d 5b74 6573 7473  .[![Tests][tests
+00000390: 2d62 6164 6765 5d5d 5b74 6573 7473 5d0d  -badge]][tests].
+000003a0: 0a5b 215b 436f 6e74 7269 6275 746f 7273  .[![Contributors
+000003b0: 5d5b 636f 6e74 7269 6275 746f 7273 2d62  ][contributors-b
+000003c0: 6164 6765 5d5d 5b63 6f6e 7472 6962 7574  adge]][contribut
+000003d0: 6f72 735d 0d0a 5b21 5b52 656c 6561 7365  ors]..[![Release
+000003e0: 5d5b 7265 6c65 6173 652d 6261 6467 655d  ][release-badge]
+000003f0: 5d5b 7265 6c65 6173 655d 0d0a 5b21 5b4c  ][release]..[![L
+00000400: 6963 656e 6365 5d5b 6c69 6365 6e63 652d  icence][licence-
+00000410: 6261 6467 655d 5d5b 6c69 6365 6e63 655d  badge]][licence]
+00000420: 0d0a 5b21 5b4c 696e 6b65 6449 6e5d 5b6c  ..[![LinkedIn][l
+00000430: 696e 6b65 6469 6e2d 6261 6467 655d 5d5b  inkedin-badge]][
+00000440: 6c69 6e6b 6564 696e 5d0d 0a0d 0a2a 2a54  linkedin]....**T
+00000450: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
+00000460: 2054 7261 6e73 6c69 7465 7261 746f 7220   Transliterator 
+00000470: 616e 6420 546f 6b65 6e69 7365 722a 2a0d  and Tokeniser**.
+00000480: 0a0d 0a49 7420 6861 7320 6d65 7468 6f64  ...It has method
+00000490: 7320 7468 6174 2061 6c6c 6f77 2074 6f20  s that allow to 
+000004a0: 6375 7374 6f6d 6973 6520 7472 616e 736c  customise transl
+000004b0: 6974 6572 6174 696f 6e20 616e 6420 7265  iteration and re
+000004c0: 7472 6965 7665 2061 6e79 206e 6563 6573  trieve any neces
+000004d0: 7361 7279 2069 6e66 6f72 6d61 7469 6f6e  sary information
+000004e0: 2061 626f 7574 2054 6169 7761 6e65 7365   about Taiwanese
+000004f0: 2048 6f6b 6b69 656e 2070 726f 6e75 6e63   Hokkien pronunc
+00000500: 6961 7469 6f6e 2e3c 6272 202f 3e0d 0a49  iation.<br />..I
+00000510: 6e63 6c75 6465 7320 776f 7264 2074 6f6b  ncludes word tok
+00000520: 656e 6973 6572 2066 6f72 2054 6169 7761  eniser for Taiwa
+00000530: 6e65 7365 2048 6f6b 6b69 656e 2e0d 0a0d  nese Hokkien....
+00000540: 0a5b 5265 706f 7274 2042 7567 5d5b 6275  .[Report Bug][bu
+00000550: 675d 20e2 80a2 0d0a 5b50 7950 495d 5b70  g] .....[PyPI][p
+00000560: 7970 695d 0d0a 0d0a 3c2f 6469 763e 0d0a  ypi]....</div>..
+00000570: 0d0a 0d0a 0d0a 2d2d 2d0d 0a0d 0a0d 0a0d  ......---.......
+00000580: 0a3c 212d 2d20 494e 5354 414c 4c20 2d2d  .<!-- INSTALL --
+00000590: 3e0d 0a23 2320 496e 7374 616c 6c0d 0a0d  >..## Install...
+000005a0: 0a54 6169 6275 6e20 6361 6e20 6265 2069  .Taibun can be i
+000005b0: 6e73 7461 6c6c 6564 2066 726f 6d20 5b70  nstalled from [p
+000005c0: 7970 695d 5b70 7970 695d 0d0a 0d0a 6060  ypi][pypi]....``
+000005d0: 6062 6173 680d 0a24 2070 6970 2069 6e73  `bash..$ pip ins
+000005e0: 7461 6c6c 2074 6169 6275 6e0d 0a60 6060  tall taibun..```
+000005f0: 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2055 5341  ........<!-- USA
+00000600: 4745 202d 2d3e 0d0a 2323 2055 7361 6765  GE -->..## Usage
+00000610: 0d0a 0d0a 2323 2320 436f 6e76 6572 7465  ....### Converte
+00000620: 720d 0a0d 0a60 436f 6e76 6572 7465 7260  r....`Converter`
+00000630: 2063 6c61 7373 2074 7261 6e73 6c69 7465   class translite
+00000640: 7261 7465 7320 7468 6520 4368 696e 6573  rates the Chines
+00000650: 6520 6368 6172 6163 7465 7273 2074 6f20  e characters to 
+00000660: 7468 6520 6368 6f73 656e 2074 7261 6e73  the chosen trans
+00000670: 6c69 7465 7261 7469 6f6e 2073 7973 7465  literation syste
+00000680: 6d20 7769 7468 2070 6172 616d 6574 6572  m with parameter
+00000690: 7320 7370 6563 6966 6965 6420 6279 2074  s specified by t
+000006a0: 6865 2064 6576 656c 6f70 6572 2e20 576f  he developer. Wo
+000006b0: 726b 7320 666f 7220 626f 7468 2054 7261  rks for both Tra
+000006c0: 6469 7469 6f6e 616c 2061 6e64 2053 696d  ditional and Sim
+000006d0: 706c 6966 6965 6420 6368 6172 6163 7465  plified characte
+000006e0: 7273 2e0d 0a0d 0a60 6060 7079 7468 6f6e  rs.....```python
+000006f0: 0d0a 2320 636f 6e73 7472 7563 746f 720d  ..# constructor.
+00000700: 0a63 203d 2043 6f6e 7665 7274 6572 2873  .c = Converter(s
+00000710: 7973 7465 6d2c 2064 6961 6c65 6374 2c20  ystem, dialect, 
+00000720: 666f 726d 6174 2c20 6465 6c69 6d69 7465  format, delimite
+00000730: 722c 2073 616e 6468 692c 2070 756e 6374  r, sandhi, punct
+00000740: 7561 7469 6f6e 2c20 636f 6e76 6572 745f  uation, convert_
+00000750: 6e6f 6e5f 636a 6b29 0d0a 0d0a 2320 7472  non_cjk)....# tr
+00000760: 616e 736c 6974 6572 6174 6520 4368 696e  ansliterate Chin
+00000770: 6573 6520 6368 6172 6163 7465 7273 0d0a  ese characters..
+00000780: 632e 6765 7428 696e 7075 7429 0d0a 6060  c.get(input)..``
+00000790: 600d 0a0d 0a23 2323 2320 5379 7374 656d  `....#### System
+000007a0: 0d0a 0d0a 6073 7973 7465 6d60 2053 7472  ....`system` Str
+000007b0: 696e 6720 2d20 7379 7374 656d 206f 6620  ing - system of 
+000007c0: 7472 616e 736c 6974 6572 6174 696f 6e2e  transliteration.
+000007d0: 0d0a 0d0a 2a20 6054 6169 6c6f 6020 2864  ....* `Tailo` (d
+000007e0: 6566 6175 6c74 2920 2d20 5b54 c3a2 692d  efault) - [T..i-
+000007f0: 75c3 a26e 204c c3b4 2d6d c3a1 2d6a c4ab  u..n L..-m..-j..
+00000800: 2050 6869 6e67 2d69 6d20 486f 6e67 2dc3   Phing-im Hong-.
+00000810: a06e 5d5b 7461 696c 6f2d 7769 6b69 5d0d  .n][tailo-wiki].
+00000820: 0a2a 2060 504f 4a60 202d 205b 5065 cc8d  .* `POJ` - [Pe..
+00000830: 682d c58d 652d 6ac4 ab5d 5b70 6f6a 2d77  h-..e-j..][poj-w
+00000840: 696b 695d 0d0a 2a20 605a 6875 7969 6e60  iki]..* `Zhuyin`
+00000850: 202d 205b 5461 6977 616e 6573 6520 5068   - [Taiwanese Ph
+00000860: 6f6e 6574 6963 2053 796d 626f 6c73 5d5b  onetic Symbols][
+00000870: 7a68 7579 696e 2d77 696b 695d 0d0a 2a20  zhuyin-wiki]..* 
+00000880: 6054 4c50 4160 202d 205b 5461 6977 616e  `TLPA` - [Taiwan
+00000890: 6573 6520 4c61 6e67 7561 6765 2050 686f  ese Language Pho
+000008a0: 6e65 7469 6320 416c 7068 6162 6574 5d5b  netic Alphabet][
+000008b0: 746c 7061 2d77 696b 695d 0d0a 2a20 6050  tlpa-wiki]..* `P
+000008c0: 696e 6779 696d 6020 2d20 5b42 62c3 a16e  ingyim` - [Bb..n
+000008d0: 6cc3 a16d 2055 c493 2050 c3ac 6e67 79c4  l..m U.. P..ngy.
+000008e0: ab6d 2048 c58d 6e67 27c3 a06e 5d5b 7069  .m H..ng'..n][pi
+000008f0: 6e67 7969 6d2d 7769 6b69 5d0d 0a2a 2060  ngyim-wiki]..* `
+00000900: 546f 6e67 696f 6e67 6020 2d20 5b44 61c4  Tongiong` - [Da.
+00000910: ab2d 6768 c3ae 2054 c58d 6e67 2d69 c58d  .-gh.. T..ng-i..
+00000920: 6e67 2050 c4ab 6e67 2d69 6d5d 5b74 6f6e  ng P..ng-im][ton
+00000930: 6769 6f6e 672d 7769 6b69 5d0d 0a2a 2060  giong-wiki]..* `
+00000940: 4950 4160 202d 205b 496e 7465 726e 6174  IPA` - [Internat
+00000950: 696f 6e61 6c20 5068 6f6e 6574 6963 2041  ional Phonetic A
+00000960: 6c70 6861 6265 745d 5b69 7061 2d77 696b  lphabet][ipa-wik
+00000970: 695d 0d0a 0d0a 7c20 7465 7874 207c 2054  i]....| text | T
+00000980: 6169 6c6f 2020 207c 2050 4f4a 2020 2020  ailo   | POJ    
+00000990: 207c 205a 6875 7969 6e20 2020 2020 207c   | Zhuyin      |
+000009a0: 2054 4c50 4120 2020 2020 207c 2050 696e   TLPA      | Pin
+000009b0: 6779 696d 207c 2054 6f6e 6769 6f6e 6720  gyim | Tongiong 
+000009c0: 7c20 4950 4120 2020 2020 2020 2020 7c0d  | IPA         |.
+000009d0: 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  .| ---- | ------
+000009e0: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
+000009f0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
+00000a00: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d20  ----- | ------- 
+00000a10: 7c20 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  | -------- | ---
+00000a20: 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20 e58f  -------- |..| ..
+00000a30: b0e7 81a3 207c 2054 c3a2 692d 75c3 a26e  .... | T..i-u..n
+00000a40: 207c 2054 c3a2 692d 6fc3 a26e 207c 20e3   | T..i-o..n | .
+00000a50: 8489 e384 9ecb 8a20 e384 a8e3 84a2 cb8a  ....... ........
+00000a60: 207c 2054 6169 3520 7561 6e35 207c 2044   | Tai5 uan5 | D
+00000a70: c3a1 6977 c3a1 6e20 207c 2054 c481 692d  ..iw..n  | T..i-
+00000a80: 75c7 8e6e 2020 7c20 5461 69c2 b2e2 81b5  u..n  | Tai.....
+00000a90: 2075 616e c2b2 e281 b520 7c0d 0a0d 0a23   uan..... |....#
+00000aa0: 2323 2320 4469 616c 6563 740d 0a0d 0a60  ### Dialect....`
+00000ab0: 6469 616c 6563 7460 2053 7472 696e 6720  dialect` String 
+00000ac0: 2d20 7072 6566 6572 7265 6420 7072 6f6e  - preferred pron
+00000ad0: 756e 6369 6174 696f 6e2e 0d0a 0d0a 2a20  unciation.....* 
+00000ae0: 6073 6f75 7468 6020 2864 6566 6175 6c74  `south` (default
+00000af0: 2920 2d20 5b5a 6861 6e67 7a68 6f75 5d5b  ) - [Zhangzhou][
+00000b00: 7a68 616e 677a 686f 752d 7769 6b69 5d2d  zhangzhou-wiki]-
+00000b10: 6c65 616e 696e 6720 7072 6f6e 756e 6369  leaning pronunci
+00000b20: 6174 696f 6e0d 0a2a 2060 6e6f 7274 6860  ation..* `north`
+00000b30: 202d 205b 5175 616e 7a68 6f75 5d5b 7175   - [Quanzhou][qu
+00000b40: 616e 7a68 6f75 2d77 696b 695d 2d6c 6561  anzhou-wiki]-lea
+00000b50: 6e69 6e67 2070 726f 6e75 6e63 6961 7469  ning pronunciati
+00000b60: 6f6e 0d0a 0d0a 7c20 7465 7874 2020 207c  on....| text   |
+00000b70: 2073 6f75 7468 2020 2020 2020 2020 207c   south         |
+00000b80: 206e 6f72 7468 2020 2020 2020 2020 207c   north         |
+00000b90: 0d0a 7c20 2d2d 2d2d 2d2d 207c 202d 2d2d  ..| ------ | ---
+00000ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
+00000bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20  ---------- |..| 
+00000bc0: e4ba 94e6 9c88 e7af 8020 7c20 47c5 8d6f  ......... | G..o
+00000bd0: 2d67 7565 cc8d 682d 7473 6568 207c 2047  -gue..h-tseh | G
+00000be0: c58d 6f2d 6765 cc8d 682d 7473 7565 6820  ..o-ge..h-tsueh 
+00000bf0: 7c0d 0a0d 0a23 2323 2320 466f 726d 6174  |....#### Format
+00000c00: 0d0a 0d0a 6066 6f72 6d61 7460 2053 7472  ....`format` Str
+00000c10: 696e 6720 2d20 666f 726d 6174 2069 6e20  ing - format in 
+00000c20: 7768 6963 6820 746f 6e65 7320 7769 6c6c  which tones will
+00000c30: 2062 6520 7265 7072 6573 656e 7465 6420   be represented 
+00000c40: 696e 2074 6865 2063 6f6e 7665 7274 6564  in the converted
+00000c50: 2073 656e 7465 6e63 652e 0d0a 0d0a 2a20   sentence.....* 
+00000c60: 606d 6172 6b60 2028 6465 6661 756c 7429  `mark` (default)
+00000c70: 202d 2075 7365 7320 6469 6163 7269 7469   - uses diacriti
+00000c80: 6373 2066 6f72 2065 6163 6820 7379 6c6c  cs for each syll
+00000c90: 6162 6c65 2e20 4e6f 7420 6176 6169 6c61  able. Not availa
+00000ca0: 626c 6520 666f 7220 544c 5041 2e0d 0a2a  ble for TLPA...*
+00000cb0: 2060 6e75 6d62 6572 6020 2d20 6164 6420   `number` - add 
+00000cc0: 6120 6e75 6d62 6572 2077 6869 6368 2072  a number which r
+00000cd0: 6570 7265 7365 6e74 7320 7468 6520 746f  epresents the to
+00000ce0: 6e65 2061 7420 7468 6520 656e 6420 6f66  ne at the end of
+00000cf0: 2074 6865 2073 796c 6c61 626c 650d 0a2a   the syllable..*
+00000d00: 2060 7374 7269 7060 202d 2072 656d 6f76   `strip` - remov
+00000d10: 6573 2061 6e79 2074 6f6e 6520 6d61 726b  es any tone mark
+00000d20: 696e 670d 0a0d 0a7c 2074 6578 7420 7c20  ing....| text | 
+00000d30: 6d61 726b 2020 2020 7c20 6e75 6d62 6572  mark    | number
+00000d40: 2020 2020 7c20 7374 7269 7020 2020 7c0d      | strip   |.
+00000d50: 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  .| ---- | ------
+00000d60: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d20 7c20  - | --------- | 
+00000d70: 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0  ------- |..| ...
+00000d80: e781 a320 7c20 54c3 a269 2d75 c3a2 6e20  ... | T..i-u..n 
+00000d90: 7c20 5461 6935 2d75 616e 3520 7c20 5461  | Tai5-uan5 | Ta
+00000da0: 692d 7561 6e20 7c0d 0a0d 0a23 2323 2320  i-uan |....#### 
+00000db0: 4465 6c69 6d69 7465 720d 0a0d 0a60 6465  Delimiter....`de
+00000dc0: 6c69 6d69 7465 7260 2053 7472 696e 6720  limiter` String 
+00000dd0: 2d20 7365 7473 2074 6865 2064 656c 696d  - sets the delim
+00000de0: 6974 6572 2063 6861 7261 6374 6572 2074  iter character t
+00000df0: 6861 7420 7769 6c6c 2062 6520 706c 6163  hat will be plac
+00000e00: 6564 2069 6e20 6265 7477 6565 6e20 7379  ed in between sy
+00000e10: 6c6c 6162 6c65 7320 6f66 2061 2077 6f72  llables of a wor
+00000e20: 642e 0d0a 0d0a 4465 6661 756c 7420 7661  d.....Default va
+00000e30: 6c75 6520 6465 7065 6e64 7320 6f6e 2074  lue depends on t
+00000e40: 6865 2063 686f 7365 6e20 6073 7973 7465  he chosen `syste
+00000e50: 6d60 3a0d 0a0d 0a2a 2060 272d 2760 202d  m`:....* `'-'` -
+00000e60: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
+00000e70: 4f4a 602c 2060 546f 6e67 696f 6e67 600d  OJ`, `Tongiong`.
+00000e80: 0a2a 2060 2727 6020 2d20 666f 7220 6050  .* `''` - for `P
+00000e90: 696e 6779 696d 600d 0a2a 2060 2720 2760  ingyim`..* `' '`
+00000ea0: 202d 2066 6f72 2060 5a68 7579 696e 602c   - for `Zhuyin`,
+00000eb0: 2060 544c 5041 602c 2060 4950 4160 0d0a   `TLPA`, `IPA`..
+00000ec0: 0d0a 7c20 7465 7874 207c 2027 2d27 2020  ..| text | '-'  
+00000ed0: 2020 207c 2027 2720 2020 2020 7c20 2720     | ''     | ' 
+00000ee0: 2720 2020 2020 7c0d 0a7c 202d 2d2d 2d20  '     |..| ---- 
+00000ef0: 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  | ------- | ----
+00000f00: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
+00000f10: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
+00000f20: 75c3 a26e 207c 2054 c3a2 6975 c3a2 6e20  u..n | T..iu..n 
+00000f30: 7c20 54c3 a269 2075 c3a2 6e20 7c0d 0a0d  | T..i u..n |...
+00000f40: 0a23 2323 2320 5361 6e64 6869 0d0a 0d0a  .#### Sandhi....
+00000f50: 6073 616e 6468 6960 2053 7472 696e 6720  `sandhi` String 
+00000f60: 2d20 6170 706c 6965 7320 7468 6520 5b73  - applies the [s
+00000f70: 616e 6468 6920 7275 6c65 7320 6f66 2054  andhi rules of T
+00000f80: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
+00000f90: 5d5b 7361 6e64 6869 2d77 696b 695d 2074  ][sandhi-wiki] t
+00000fa0: 6f20 7379 6c6c 6162 6c65 7320 6f66 2061  o syllables of a
+00000fb0: 2073 696e 676c 6520 776f 7264 2e0d 0a0d   single word....
+00000fc0: 0a53 696e 6365 2069 7427 7320 6469 6666  .Since it's diff
+00000fd0: 6963 756c 7420 746f 2065 6e63 6f64 6520  icult to encode 
+00000fe0: 616c 6c20 7361 6e64 6869 2072 756c 6573  all sandhi rules
+00000ff0: 2c20 5461 6962 756e 2070 726f 7669 6465  , Taibun provide
+00001000: 7320 6d75 6c74 6970 6c65 206d 6f64 6573  s multiple modes
+00001010: 2066 6f72 2073 616e 6468 6920 636f 6e76   for sandhi conv
+00001020: 6572 7369 6f6e 2074 6f20 616c 6c6f 7720  ersion to allow 
+00001030: 666f 7220 6375 7374 6f6d 6973 6564 2073  for customised s
+00001040: 616e 6468 6920 6861 6e64 6c69 6e67 2e0d  andhi handling..
+00001050: 0a0d 0a2a 2060 6e6f 6e65 6020 2d20 646f  ...* `none` - do
+00001060: 6573 6e27 7420 7065 7266 6f72 6d20 616e  esn't perform an
+00001070: 7920 746f 6e65 2073 616e 6468 690d 0a2a  y tone sandhi..*
+00001080: 2060 6175 746f 6020 2d20 636c 6f73 6573   `auto` - closes
+00001090: 7420 6170 7072 6f78 696d 6174 696f 6e20  t approximation 
+000010a0: 746f 2066 756c 6c20 636f 7272 6563 7420  to full correct 
+000010b0: 746f 6e65 2073 616e 6468 6920 6f66 2054  tone sandhi of T
+000010c0: 6169 7761 6e65 7365 2c20 7769 7468 2070  aiwanese, with p
+000010d0: 726f 7065 7220 7361 6e64 6869 206f 6620  roper sandhi of 
+000010e0: 7072 6f6e 6f75 6e73 2c20 7375 6666 6978  pronouns, suffix
+000010f0: 6573 2c20 616e 6420 776f 7264 7320 7769  es, and words wi
+00001100: 7468 20e4 bb94 0d0a 2a20 6065 7863 5f6c  th .....* `exc_l
+00001110: 6173 7460 202d 2063 6861 6e67 6573 2074  ast` - changes t
+00001120: 6f6e 6520 666f 7220 6576 6572 7920 7379  one for every sy
+00001130: 6c6c 6162 6c65 2065 7863 6570 7420 666f  llable except fo
+00001140: 7220 7468 6520 6c61 7374 206f 6e65 0d0a  r the last one..
+00001150: 2a20 6069 6e63 6c5f 6c61 7374 6020 2d20  * `incl_last` - 
+00001160: 6368 616e 6765 7320 746f 6e65 2066 6f72  changes tone for
+00001170: 2065 7665 7279 2073 796c 6c61 626c 6520   every syllable 
+00001180: 696e 636c 7564 696e 6720 7468 6520 6c61  including the la
+00001190: 7374 206f 6e65 0d0a 0d0a 4465 6661 756c  st one....Defaul
+000011a0: 7420 7661 6c75 6520 6465 7065 6e64 7320  t value depends 
+000011b0: 6f6e 2074 6865 2063 686f 7365 6e20 6073  on the chosen `s
+000011c0: 7973 7465 6d60 3a0d 0a0d 0a2a 2060 6175  ystem`:....* `au
+000011d0: 746f 6020 2d20 666f 7220 6054 6f6e 6769  to` - for `Tongi
+000011e0: 6f6e 6760 0d0a 2a20 606e 6f6e 6560 202d  ong`..* `none` -
+000011f0: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
+00001200: 4f4a 602c 2060 5a68 7579 696e 602c 2060  OJ`, `Zhuyin`, `
+00001210: 544c 5041 602c 2060 5069 6e67 7969 6d60  TLPA`, `Pingyim`
+00001220: 2c20 6049 5041 600d 0a0d 0a7c 2074 6578  , `IPA`....| tex
+00001230: 7420 2020 2020 2020 2020 7c20 6e6f 6e65  t         | none
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 207c 2061 7574 6f20 2020 2020 2020 2020   | auto         
+00001260: 2020 2020 2020 2020 7c20 6578 635f 6c61          | exc_la
+00001270: 7374 2020 2020 2020 2020 2020 2020 207c  st             |
+00001280: 2069 6e63 6c5f 6c61 7374 2020 2020 2020   incl_last      
+00001290: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
+000012a0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+000012b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+000012c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000012d0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+000012e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
+000012f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001300: 2d2d 2d20 7c0d 0a7c 20e9 8099 e698 afe5  --- |..| .......
+00001310: 8fb0 e781 a3e5 9ba1 e4bb 9420 7c20 5473  ........... | Ts
+00001320: 6520 73c4 ab20 54c3 a269 2d75 c3a2 6e20  e s.. T..i-u..n 
+00001330: 67c3 ad6e 2dc3 a120 7c20 5473 6520 73c3  g..n-.. | Tse s.
+00001340: ac20 54c4 8169 2d75 c481 6e20 6769 6e2d  . T..i-u..n gin-
+00001350: c3a1 207c 2054 73c4 9320 73c3 ac20 54c4  .. | Ts.. s.. T.
+00001360: 8169 2d75 c481 6e20 6769 6e2d c3a1 207c  .i-u..n gin-.. |
+00001370: 2054 73c4 9320 73c3 ac20 54c4 8169 2d75   Ts.. s.. T..i-u
+00001380: c481 6e20 6769 6e2d 6120 7c0d 0a0d 0a53  ..n gin-a |....S
+00001390: 616e 6468 6920 7275 6c65 7320 616c 736f  andhi rules also
+000013a0: 2063 6861 6e67 6520 6465 7065 6e64 696e   change dependin
+000013b0: 6720 6f6e 2074 6865 2064 6961 6c65 6374  g on the dialect
+000013c0: 2063 686f 7365 6e2e 0d0a 0d0a 7c20 7465   chosen.....| te
+000013d0: 7874 207c 206e 6f20 7361 6e64 6869 207c  xt | no sandhi |
+000013e0: 2073 6f75 7468 2020 207c 206e 6f72 7468   south   | north
+000013f0: 2020 207c 0d0a 7c20 2d2d 2d2d 207c 202d     |..| ---- | -
+00001400: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
+00001410: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
+00001420: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
+00001430: 75c3 a26e 2020 207c 2054 c481 692d 75c3  u..n   | T..i-u.
+00001440: a26e 207c 2054 c3a0 692d 75c3 a26e 207c  .n | T..i-u..n |
+00001450: 0d0a 0d0a 2323 2323 2050 756e 6374 7561  ....#### Punctua
+00001460: 7469 6f6e 0d0a 0d0a 6070 756e 6374 7561  tion....`punctua
+00001470: 7469 6f6e 6020 5374 7269 6e67 0d0a 0d0a  tion` String....
+00001480: 2a20 6066 6f72 6d61 7460 2028 6465 6661  * `format` (defa
+00001490: 756c 7429 202d 2063 6f6e 7665 7274 7320  ult) - converts 
+000014a0: 4368 696e 6573 652d 7374 796c 6520 7075  Chinese-style pu
+000014b0: 6e63 7475 6174 696f 6e20 746f 204c 6174  nctuation to Lat
+000014c0: 696e 2d73 7479 6c65 2070 756e 6374 7561  in-style punctua
+000014d0: 7469 6f6e 2061 6e64 2063 6170 6974 616c  tion and capital
+000014e0: 6973 6573 2077 6f72 6473 2061 7420 7468  ises words at th
+000014f0: 6520 6265 6769 6e6e 696e 6720 6f66 2065  e beginning of e
+00001500: 6163 6820 7365 6e74 656e 6365 2e0d 0a2a  ach sentence...*
+00001510: 2060 6e6f 6e65 6020 2d20 7072 6573 6572   `none` - preser
+00001520: 7665 7320 4368 696e 6573 652d 7374 796c  ves Chinese-styl
+00001530: 6520 7075 6e63 7475 6174 696f 6e20 616e  e punctuation an
+00001540: 6420 646f 6573 6e27 7420 6361 7069 7461  d doesn't capita
+00001550: 6c69 7365 2077 6f72 6473 2061 7420 7468  lise words at th
+00001560: 6520 6265 6769 6e6e 696e 6720 6f66 206e  e beginning of n
+00001570: 6577 2073 656e 7465 6e63 6573 2e0d 0a0d  ew sentences....
+00001580: 0a7c 2074 6578 7420 2020 2020 2020 2020  .| text         
+00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015d0: 2020 7c20 666f 726d 6174 2020 2020 2020    | format      
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2020 2020 2020 7c20 6e6f 6e65 2020 2020        | none    
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001690: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
+000016a0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
+000016b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016f0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00001700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001750: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d 0a7c  ----------- |..|
+000017c0: 20e9 8099 e698 afe8 87ba e58d 97ef bc8c   ...............
+000017d0: e7b0 a1e7 a8b1 e380 8ce5 8d97 e380 8def  ................
+000017e0: bc88 e799 bde8 a9b1 e5ad 97ef bc9a 54c3  ..............T.
+000017f0: a269 2d6c c3a2 6def bc9b e6b3 a8e9 9fb3  .i-l..m.........
+00001800: e7ac a6e8 999f efbc 9ae3 848a e384 9ecb  ................
+00001810: 8a20 e384 8be3 84a2 cb8a efbc 8ce5 9c8b  . ..............
+00001820: e8aa 9eef bc9a 54c3 a169 6ec3 a16e efbc  ......T..in..n..
+00001830: 89e3 8082 207c 2054 7365 2073 c4ab 2054  .... | Tse s.. T
+00001840: c3a2 692d 6cc3 a26d 2c20 6bc3 a16e 2d74  ..i-l..m, k..n-t
+00001850: 7368 696e 6720 226c c3a2 6d22 2028 5065  shing "l..m" (Pe
+00001860: cc8d 682d 75c4 932d 6ac4 ab3a 2054 c3a2  ..h-u..-j..: T..
+00001870: 692d 6cc3 a26d 3b20 7473 c3b9 2d69 6d20  i-l..m; ts..-im 
+00001880: 68c3 bb2d 68c5 8d3a 20e3 848a e384 9ecb  h..-h..: .......
+00001890: 8a20 e384 8be3 84a2 cb8a 2c20 6b6f 6b2d  . ........, kok-
+000018a0: 67c3 ad3a 2054 c3a1 696e c3a1 6e29 2e20  g..: T..in..n). 
+000018b0: 7c20 7473 6520 73c4 ab20 54c3 a269 2d6c  | tse s.. T..i-l
+000018c0: c3a2 6def bc8c 6bc3 a16e 2d74 7368 696e  ..m...k..n-tshin
+000018d0: 67e3 808c 6cc3 a26d e380 8def bc88 5065  g...l..m......Pe
+000018e0: cc8d 682d 75c4 932d 6ac4 abef bc9a 54c3  ..h-u..-j.....T.
+000018f0: a269 2d6c c3a2 6def bc9b 7473 c3b9 2d69  .i-l..m...ts..-i
+00001900: 6d20 68c3 bb2d 68c5 8def bc9a e384 8ae3  m h..-h.........
+00001910: 849e cb8a 20e3 848b e384 a2cb 8aef bc8c  .... ...........
+00001920: 6b6f 6b2d 67c3 adef bc9a 54c3 a169 6ec3  kok-g.....T..in.
+00001930: a16e efbc 89e3 8082 207c 0d0a 0d0a 2323  .n...... |....##
+00001940: 2323 2043 6f6e 7665 7274 206e 6f6e 2d43  ## Convert non-C
+00001950: 4a4b 0d0a 0d0a 6063 6f6e 7665 7274 5f6e  JK....`convert_n
+00001960: 6f6e 5f63 6a6b 6020 426f 6f6c 6561 6e20  on_cjk` Boolean 
+00001970: 2d20 6465 6669 6e65 7320 7768 6574 6865  - defines whethe
+00001980: 7220 6f72 206e 6f74 2074 6f20 636f 6e76  r or not to conv
+00001990: 6572 7420 6e6f 6e2d 4368 696e 6573 6520  ert non-Chinese 
+000019a0: 776f 7264 732e 2043 616e 2062 6520 7573  words. Can be us
+000019b0: 6564 2074 6f20 636f 6e76 6572 7420 5461  ed to convert Ta
+000019c0: 696c 6f20 746f 2061 6e6f 7468 6572 2072  ilo to another r
+000019d0: 6f6d 616e 6973 6174 696f 6e20 7379 7374  omanisation syst
+000019e0: 656d 2e0d 0a0d 0a2a 2060 5472 7565 6020  em.....* `True` 
+000019f0: 2d20 636f 6e76 6572 7420 6e6f 6e2d 4368  - convert non-Ch
+00001a00: 696e 6573 6520 6368 6172 6163 7465 7220  inese character 
+00001a10: 776f 7264 730d 0a2a 2060 4661 6c73 6560  words..* `False`
+00001a20: 2028 6465 6661 756c 7429 202d 2063 6f6e   (default) - con
+00001a30: 7665 7274 206f 6e6c 7920 4368 696e 6573  vert only Chines
+00001a40: 6520 6368 6172 6163 7465 7220 776f 7264  e character word
+00001a50: 730d 0a0d 0a7c 2074 6578 7420 2020 2020  s....| text     
+00001a60: 207c 2046 616c 7365 2020 2020 2020 2020   | False        
+00001a70: 2020 2020 2020 2020 2020 207c 2054 7275             | Tru
+00001a80: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00001a90: 2020 2020 207c 0d0a 7c20 2d2d 2d2d 2d2d       |..| ------
+00001aa0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ad0: 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e6 8891  ------- |..| ...
+00001ae0: e9a3 9f70 68c3 a16e 6720 7c20 e386 a3e3  ...ph..ng | ....
+00001af0: 84a8 e384 9acb 8b20 e384 90e3 84a7 e384  ....... ........
+00001b00: 9ae3 86b7 cb99 2070 68c3 a16e 6720 7c20  ...... ph..ng | 
+00001b10: e386 a3e3 84a8 e384 9acb 8b20 e384 90e3  ........... ....
+00001b20: 84a7 e384 9ae3 86b7 cb99 20e3 8486 e384  .......... .....
+00001b30: a4cb 8b20 7c0d 0a0d 0a23 2323 2054 6f6b  ... |....### Tok
+00001b40: 656e 6973 6572 0d0a 0d0a 6054 6f6b 656e  eniser....`Token
+00001b50: 6973 6572 6020 636c 6173 7320 7065 7266  iser` class perf
+00001b60: 6f72 6d73 205b 4e4c 544b 2077 6f72 6470  orms [NLTK wordp
+00001b70: 756e 6374 5f74 6f6b 656e 697a 655d 5b6e  unct_tokenize][n
+00001b80: 6c74 6b2d 746f 6b65 6e69 7a65 5d2d 6c69  ltk-tokenize]-li
+00001b90: 6b65 2074 6f6b 656e 6973 6174 696f 6e20  ke tokenisation 
+00001ba0: 6f66 2061 2054 6169 7761 6e65 7365 2048  of a Taiwanese H
+00001bb0: 6f6b 6b69 656e 2073 656e 7465 6e63 652e  okkien sentence.
+00001bc0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a23  ....```python..#
+00001bd0: 2063 6f6e 7374 7275 6374 6f72 0d0a 7420   constructor..t 
+00001be0: 3d20 546f 6b65 6e69 7365 7228 290d 0a0d  = Tokeniser()...
+00001bf0: 0a23 2074 6f6b 656e 6973 6520 5461 6977  .# tokenise Taiw
+00001c00: 616e 6573 6520 486f 6b6b 6965 6e20 7365  anese Hokkien se
+00001c10: 6e74 656e 6365 0d0a 742e 746f 6b65 6e69  ntence..t.tokeni
+00001c20: 7365 2869 6e70 7574 290d 0a60 6060 0d0a  se(input)..```..
+00001c30: 0d0a 2323 2320 4f74 6865 7220 4675 6e63  ..### Other Func
+00001c40: 7469 6f6e 730d 0a0d 0a60 6060 7079 7468  tions....```pyth
+00001c50: 6f6e 0d0a 2320 436f 6e76 6572 7420 746f  on..# Convert to
+00001c60: 2054 7261 6469 7469 6f6e 616c 0d0a 746f   Traditional..to
+00001c70: 5f74 7261 6469 7469 6f6e 616c 2869 6e70  _traditional(inp
+00001c80: 7574 290d 0a0d 0a23 2043 6f6e 7665 7274  ut)....# Convert
+00001c90: 2074 6f20 5369 6d70 6c69 6669 6564 0d0a   to Simplified..
+00001ca0: 746f 5f73 696d 706c 6966 6965 6428 696e  to_simplified(in
+00001cb0: 7075 7429 0d0a 0d0a 2320 4368 6563 6b20  put)....# Check 
+00001cc0: 6966 2074 6865 2073 7472 696e 6720 6973  if the string is
+00001cd0: 2066 756c 6c79 2063 6f6d 706f 7365 6420   fully composed 
+00001ce0: 6f66 2043 6869 6e65 7365 2063 6861 7261  of Chinese chara
+00001cf0: 6374 6572 730d 0a69 735f 636a 6b28 696e  cters..is_cjk(in
+00001d00: 7075 7429 0d0a 6060 600d 0a0d 0a0d 0a0d  put)..```.......
+00001d10: 0a3c 212d 2d20 4558 414d 504c 4520 2d2d  .<!-- EXAMPLE --
+00001d20: 3e0d 0a23 2320 4578 616d 706c 650d 0a0d  >..## Example...
+00001d30: 0a60 6060 7079 7468 6f6e 0d0a 2320 436f  .```python..# Co
+00001d40: 6e76 6572 7465 720d 0a66 726f 6d20 7461  nverter..from ta
+00001d50: 6962 756e 2069 6d70 6f72 7420 436f 6e76  ibun import Conv
+00001d60: 6572 7465 720d 0a0d 0a23 2320 5379 7374  erter....## Syst
+00001d70: 656d 0d0a 6320 3d20 436f 6e76 6572 7465  em..c = Converte
+00001d80: 7228 2920 2320 5461 696c 6f20 7379 7374  r() # Tailo syst
+00001d90: 656d 2064 6566 6175 6c74 0d0a 632e 6765  em default..c.ge
+00001da0: 7428 27e5 8588 e794 9fe8 ac9b efbc 8ce5  t('.............
+00001db0: adb8 e794 9fe6 81ac e681 ace8 81bd e380  ................
+00001dc0: 8227 290d 0a3e 3e20 5369 616e 2d73 696e  .')..>> Sian-sin
+00001dd0: 6e20 6bc3 b36e 672c 2068 61cc 8d6b 2d73  n k..ng, ha..k-s
+00001de0: 696e 6720 7469 c481 6d2d 7469 c481 6d20  ing ti..m-ti..m 
+00001df0: 7468 6961 6e6e 2e0d 0a0d 0a63 203d 2043  thiann.....c = C
+00001e00: 6f6e 7665 7274 6572 2873 7973 7465 6d3d  onverter(system=
+00001e10: 275a 6875 7969 6e27 290d 0a63 2e67 6574  'Zhuyin')..c.get
+00001e20: 2827 e585 88e7 949f e8ac 9bef bc8c e5ad  ('..............
+00001e30: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
+00001e40: 2729 0d0a 3e3e 20e3 8492 e384 a7e3 84a2  ')..>> .........
+00001e50: 20e3 8492 e386 aa20 e384 8de3 86b2 cb8b   ...... ........
+00001e60: 2c20 e384 8fe3 849a e386 b6cb 9920 e384  , ........... ..
+00001e70: 92e3 84a7 e384 a520 e384 89e3 84a7 e386  ....... ........
+00001e80: b0cb ab20 e384 89e3 84a7 e386 b0cb ab20  ... ........... 
+00001e90: e384 8ae3 84a7 e386 a92e 0d0a 0d0a 2323  ..............##
+00001ea0: 2044 6961 6c65 6374 0d0a 6320 3d20 436f   Dialect..c = Co
+00001eb0: 6e76 6572 7465 7228 2920 2320 736f 7574  nverter() # sout
+00001ec0: 6820 6469 616c 6563 7420 6465 6661 756c  h dialect defaul
+00001ed0: 740d 0a63 2e67 6574 2822 e688 91e6 acb2  t..c.get("......
+00001ee0: e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a  ............")..
+00001ef0: 3e3e 2047 75c3 a120 6265 6820 c4ab 6e67  >> Gu.. beh ..ng
+00001f00: 2074 c4ab 2074 7369 61cc 8d68 2068 c3ae   t.. tsia..h h..
+00001f10: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00001f20: 7228 6469 616c 6563 743d 276e 6f72 7468  r(dialect='north
+00001f30: 2729 0d0a 632e 6765 7428 22e6 8891 e6ac  ')..c.get(".....
+00001f40: b2e7 94a8 e7ae b8e9 a39f e9ad 9a22 290d  .............").
+00001f50: 0a3e 3e20 4775 c3a1 2062 7565 6820 c4ab  .>> Gu.. bueh ..
+00001f60: 6e67 2074 c5ab 2074 7369 61cc 8d68 2068  ng t.. tsia..h h
+00001f70: c3bb 0d0a 0d0a 2323 2046 6f72 6d61 740d  ......## Format.
+00001f80: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
+00001f90: 2023 2066 6f72 2054 6169 6c6f 2c20 6d61   # for Tailo, ma
+00001fa0: 726b 2062 7920 6465 6661 756c 740d 0a63  rk by default..c
+00001fb0: 2e67 6574 2822 e794 9fe6 97a5 e5bf abe6  .get("..........
+00001fc0: a882 2229 0d0a 3e3e 2053 656e 6e2d 6a69  ..")..>> Senn-ji
+00001fd0: cc8d 7420 6b68 75c3 a069 2d6c 6fcc 8d6b  ..t khu..i-lo..k
+00001fe0: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00001ff0: 7228 666f 726d 6174 3d27 6e75 6d62 6572  r(format='number
+00002000: 2729 0d0a 632e 6765 7428 22e7 949f e697  ')..c.get(".....
+00002010: a5e5 bfab e6a8 8222 290d 0a3e 3e20 5365  .......")..>> Se
+00002020: 6e6e 312d 6a69 7438 206b 6875 6169 332d  nn1-jit8 khuai3-
+00002030: 6c6f 6b38 0d0a 0d0a 6320 3d20 436f 6e76  lok8....c = Conv
+00002040: 6572 7465 7228 666f 726d 6174 3d27 7374  erter(format='st
+00002050: 7269 7027 290d 0a63 2e67 6574 2822 e794  rip')..c.get("..
+00002060: 9fe6 97a5 e5bf abe6 a882 2229 0d0a 3e3e  ..........")..>>
+00002070: 2053 656e 6e2d 6a69 7420 6b68 7561 692d   Senn-jit khuai-
+00002080: 6c6f 6b0d 0a0d 0a23 2320 4465 6c69 6d69  lok....## Delimi
+00002090: 7465 720d 0a63 203d 2043 6f6e 7665 7274  ter..c = Convert
+000020a0: 6572 2864 656c 696d 6974 6572 3d27 2729  er(delimiter='')
+000020b0: 0d0a 632e 6765 7428 22e5 8588 e794 9fe8  ..c.get(".......
+000020c0: ac9b efbc 8ce5 adb8 e794 9fe6 81ac e681  ................
+000020d0: ace8 81bd e380 8222 290d 0a3e 3e20 5369  .......")..>> Si
+000020e0: 616e 7369 6e6e 206b c3b3 6e67 2c20 6861  ansinn k..ng, ha
+000020f0: cc8d 6b73 696e 6720 7469 c481 6d74 69c4  ..ksing ti..mti.
+00002100: 816d 2074 6869 616e 6e2e 0d0a 0d0a 6320  .m thiann.....c 
+00002110: 3d20 436f 6e76 6572 7465 7228 7379 7374  = Converter(syst
+00002120: 656d 3d27 5069 6e67 7969 6d27 2c20 6465  em='Pingyim', de
+00002130: 6c69 6d69 7465 723d 272d 2729 0d0a 632e  limiter='-')..c.
+00002140: 6765 7428 22e5 8588 e794 9fe8 ac9b efbc  get("...........
+00002150: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
+00002160: e380 8222 290d 0a3e 3e20 5369 c481 6e2d  ...")..>> Si..n-
+00002170: 736e c4ab 2067 c792 6e67 2c20 68c3 a167  sn.. g..ng, h..g
+00002180: 2d73 c4ab 6e67 2064 69c3 a26d 2d64 69c3  -s..ng di..m-di.
+00002190: a26d 2074 696e c481 2e0d 0a0d 0a23 2320  .m tin.......## 
+000021a0: 5361 6e64 6869 0d0a 6320 3d20 436f 6e76  Sandhi..c = Conv
+000021b0: 6572 7465 7228 2920 2320 666f 7220 5461  erter() # for Ta
+000021c0: 696c 6f2c 2073 616e 6468 6920 6e6f 6e65  ilo, sandhi none
+000021d0: 2062 7920 6465 6661 756c 740d 0a63 2e67   by default..c.g
+000021e0: 6574 2822 e980 99e6 98af e58f b0e7 81a3  et("............
+000021f0: e59b a1e4 bb94 2229 0d0a 3e3e 2054 7365  ......")..>> Tse
+00002200: 2073 c4ab 2054 c3a2 692d 75c3 a26e 2067   s.. T..i-u..n g
+00002210: c3ad 6e2d c3a1 0d0a 0d0a 6320 3d20 436f  ..n-......c = Co
+00002220: 6e76 6572 7465 7228 7361 6e64 6869 3d27  nverter(sandhi='
+00002230: 6175 746f 2729 0d0a 632e 6765 7428 22e9  auto')..c.get(".
+00002240: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
+00002250: 9422 290d 0a3e 3e20 5473 6520 73c3 ac20  .")..>> Tse s.. 
+00002260: 54c4 8169 2d75 c481 6e20 6769 6e2d c3a1  T..i-u..n gin-..
+00002270: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00002280: 7228 7361 6e64 6869 3d27 6578 635f 6c61  r(sandhi='exc_la
+00002290: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
+000022a0: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+000022b0: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
+000022c0: c481 692d 75c4 816e 2067 696e 2dc3 a10d  ..i-u..n gin-...
+000022d0: 0a0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
+000022e0: 2873 616e 6468 693d 2769 6e63 6c5f 6c61  (sandhi='incl_la
+000022f0: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
+00002300: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+00002310: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
+00002320: c481 692d 75c4 816e 2067 696e 2d61 0d0a  ..i-u..n gin-a..
+00002330: 0d0a 2323 2050 756e 6374 7561 7469 6f6e  ..## Punctuation
+00002340: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+00002350: 2920 2320 666f 726d 6174 2070 756e 6374  ) # format punct
+00002360: 7561 7469 6f6e 2064 6566 6175 6c74 0d0a  uation default..
+00002370: 632e 6765 7428 22e5 a4aa e7a9 bae6 9c8b  c.get(".........
+00002380: e58f 8bef bc8c e681 81e5 a5bd efbc 81e6  ................
+00002390: 8181 e9a3 9fe9 a3bd e69c aaef bc9f 2229  ..............")
+000023a0: 0d0a 3e3e 2054 68c3 a069 2d6b 686f 6e67  ..>> Th..i-khong
+000023b0: 2070 c3ae 6e67 2d69 c3ba 2c20 6cc3 ad6e   p..ng-i.., l..n
+000023c0: 2d68 c3b3 2120 4cc3 ad6e 2074 7369 61cc  -h..! L..n tsia.
+000023d0: 8d68 2d70 c3a1 2062 75c4 933f 0d0a 0d0a  .h-p.. bu..?....
+000023e0: 6320 3d20 436f 6e76 6572 7465 7228 7075  c = Converter(pu
+000023f0: 6e63 7475 6174 696f 6e3d 276e 6f6e 6527  nctuation='none'
+00002400: 290d 0a63 2e67 6574 2822 e5a4 aae7 a9ba  )..c.get("......
+00002410: e69c 8be5 8f8b efbc 8ce6 8181 e5a5 bdef  ................
+00002420: bc81 e681 81e9 a39f e9a3 bde6 9caa efbc  ................
+00002430: 9f22 290d 0a3e 3e20 7468 c3a0 692d 6b68  .")..>> th..i-kh
+00002440: 6f6e 6720 70c3 ae6e 672d 69c3 baef bc8c  ong p..ng-i.....
+00002450: 6cc3 ad6e 2d68 c3b3 efbc 816c c3ad 6e20  l..n-h.....l..n 
+00002460: 7473 6961 cc8d 682d 70c3 a120 6275 c493  tsia..h-p.. bu..
+00002470: efbc 9f0d 0a0d 0a23 2320 436f 6e76 6572  .......## Conver
+00002480: 7420 6e6f 6e2d 434a 4b0d 0a63 203d 2043  t non-CJK..c = C
+00002490: 6f6e 7665 7274 2873 7973 7465 6d3d 275a  onvert(system='Z
+000024a0: 6875 7969 6e27 2920 2320 4661 6c73 6520  huyin') # False 
+000024b0: 636f 6e76 6572 745f 6e6f 6e5f 636a 6b20  convert_non_cjk 
+000024c0: 6465 6661 756c 740d 0a63 2e67 6574 2822  default..c.get("
+000024d0: e688 91e9 a39f 7068 c3a1 6e67 2229 0d0a  ......ph..ng")..
+000024e0: 3e3e 20e3 86a3 e384 a8e3 849a cb8b 20e3  >> ........... .
+000024f0: 8490 e384 a7e3 849a e386 b7cb 9920 7068  ............. ph
+00002500: c3a1 6e67 0d0a 0d0a 6320 3d20 436f 6e76  ..ng....c = Conv
+00002510: 6572 7428 7379 7374 656d 3d27 5a68 7579  ert(system='Zhuy
+00002520: 696e 272c 2063 6f6e 7665 7274 5f6e 6f6e  in', convert_non
+00002530: 5f63 6a6b 3d54 7275 6529 0d0a 632e 6765  _cjk=True)..c.ge
+00002540: 7428 22e6 8891 e9a3 9f70 68c3 a16e 6722  t("......ph..ng"
+00002550: 290d 0a3e 3e20 e386 a3e3 84a8 e384 9acb  )..>> ..........
+00002560: 8b20 e384 90e3 84a7 e384 9ae3 86b7 cb99  . ..............
+00002570: 20e3 8486 e384 a4cb 8b0d 0a0d 0a0d 0a23   ..............#
+00002580: 2054 6f6b 656e 6973 6572 0d0a 6672 6f6d   Tokeniser..from
+00002590: 2074 6169 6275 6e20 696d 706f 7274 2054   taibun import T
+000025a0: 6f6b 656e 6973 6572 0d0a 0d0a 7420 3d20  okeniser....t = 
+000025b0: 546f 6b65 6e69 7365 7228 290d 0a74 2e74  Tokeniser()..t.t
+000025c0: 6f6b 656e 6973 6528 22e5 a4aa e7a9 bae6  okenise(".......
+000025d0: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
+000025e0: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
+000025f0: 2229 0d0a 3e3e 205b 27e5 a4aa e7a9 ba27  ")..>> ['......'
+00002600: 2c20 27e6 9c8b e58f 8b27 2c20 27ef bc8c  , '......', '...
+00002610: 272c 2027 e681 81e5 a5bd 272c 2027 efbc  ', '......', '..
+00002620: 8127 2c20 27e6 8181 272c 2027 e9a3 9fe9  .', '...', '....
+00002630: a3bd 272c 2027 e69c aa27 2c20 27ef bc9f  ..', '...', '...
+00002640: 275d 0d0a 0d0a 0d0a 2320 4f74 6865 7220  ']......# Other 
+00002650: 4675 6e63 7469 6f6e 730d 0a66 726f 6d20  Functions..from 
+00002660: 7461 6962 756e 2069 6d70 6f72 7420 746f  taibun import to
+00002670: 5f74 7261 6469 7469 6f6e 616c 2c20 746f  _traditional, to
+00002680: 5f73 696d 706c 6966 6965 642c 2069 735f  _simplified, is_
+00002690: 636a 6b0d 0a0d 0a74 6f5f 7472 6164 6974  cjk....to_tradit
+000026a0: 696f 6e61 6c28 22e6 8891 e590 ace6 97a0  ional(".........
+000026b0: e58f b0e6 b9be e8af 9d22 290d 0a3e 3e20  .........")..>> 
+000026c0: e688 91e8 81bd e784 a1e5 8fb0 e781 a3e8  ................
+000026d0: a9b1 0d0a 0d0a 746f 5f73 696d 706c 6966  ......to_simplif
+000026e0: 6965 6428 22e6 8891 e881 bde7 84a1 e887  ied("...........
+000026f0: bae7 81a3 e8a9 b122 290d 0a3e 3e20 e688  .......")..>> ..
+00002700: 91e5 90ac e697 a0e5 8fb0 e6b9 bee8 af9d  ................
+00002710: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
+00002720: a39f e9ba ad27 290d 0a3e 3e20 5472 7565  .....')..>> True
+00002730: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
+00002740: a39f 7068 c3a1 6e67 2729 0d0a 3e3e 2046  ..ph..ng')..>> F
+00002750: 616c 7365 0d0a 6060 600d 0a0d 0a0d 0a0d  alse..```.......
+00002760: 0a3c 212d 2d20 4441 5441 202d 2d3e 0d0a  .<!-- DATA -->..
+00002770: 2323 2044 6174 610d 0a0d 0a2d 205b 5461  ## Data....- [Ta
+00002780: 6977 616e 6573 652d 4368 696e 6573 6520  iwanese-Chinese 
+00002790: 4f6e 6c69 6e65 2044 6963 7469 6f6e 6172  Online Dictionar
+000027a0: 795d 5b6f 6e6c 696e 652d 6469 6374 696f  y][online-dictio
+000027b0: 6e61 7279 5d20 2876 6961 205b 4368 686f  nary] (via [Chho
+000027c0: 6554 6169 6769 5d5b 6461 7461 2d76 6961  eTaigi][data-via
+000027d0: 5d29 0d0a 2d20 5b69 5461 6967 6920 4368  ])..- [iTaigi Ch
+000027e0: 696e 6573 652d 5461 6977 616e 6573 6520  inese-Taiwanese 
+000027f0: 436f 6d70 6172 6973 6f6e 2044 6963 7469  Comparison Dicti
+00002800: 6f6e 6172 795d 5b69 7461 6967 692d 6469  onary][itaigi-di
+00002810: 6374 696f 6e61 7279 5d20 2876 6961 205b  ctionary] (via [
+00002820: 4368 686f 6554 6169 6769 5d5b 6461 7461  ChhoeTaigi][data
+00002830: 2d76 6961 5d29 0d0a 0d0a 0d0a 0d0a 3c21  -via])........<!
+00002840: 2d2d 2041 434b 4e4f 574c 4544 4745 4d45  -- ACKNOWLEDGEME
+00002850: 4e54 5320 2d2d 3e0d 0a23 2320 4163 6b6e  NTS -->..## Ackn
+00002860: 6f77 6c65 6467 656d 656e 7473 0d0a 0d0a  owledgements....
+00002870: 2d20 5361 6d75 656c 204a 656e 2028 5b47  - Samuel Jen ([G
+00002880: 6974 6875 625d 5b73 616d 7565 6c2d 6769  ithub][samuel-gi
+00002890: 7468 7562 5d20 c2b7 205b 4c69 6e6b 6564  thub] .. [Linked
+000028a0: 496e 5d5b 7361 6d75 656c 2d6c 696e 6b65  In][samuel-linke
+000028b0: 6469 6e5d 2920 2d20 5461 6977 616e 6573  din]) - Taiwanes
+000028c0: 6520 616e 6420 4d61 6e64 6172 696e 2074  e and Mandarin t
+000028d0: 7261 6e73 6c61 7469 6f6e 0d0a 0d0a 0d0a  ranslation......
+000028e0: 0d0a 3c21 2d2d 204c 4943 454e 4345 202d  ..<!-- LICENCE -
+000028f0: 2d3e 0d0a 2323 204c 6963 656e 6365 0d0a  ->..## Licence..
+00002900: 0d0a 4265 6361 7573 6520 5461 6962 756e  ..Because Taibun
+00002910: 2069 7320 4d49 542d 6c69 6365 6e73 6564   is MIT-licensed
+00002920: 2c20 616e 7920 6465 7665 6c6f 7065 7220  , any developer 
+00002930: 6361 6e20 6573 7365 6e74 6961 6c6c 7920  can essentially 
+00002940: 646f 2077 6861 7465 7665 7220 7468 6579  do whatever they
+00002950: 2077 616e 7420 7769 7468 2069 7420 6173   want with it as
+00002960: 206c 6f6e 6720 6173 2074 6865 7920 696e   long as they in
+00002970: 636c 7564 6520 7468 6520 6f72 6967 696e  clude the origin
+00002980: 616c 2063 6f70 7972 6967 6874 2061 6e64  al copyright and
+00002990: 206c 6963 656e 6365 206e 6f74 6963 6520   licence notice 
+000029a0: 696e 2061 6e79 2063 6f70 6965 7320 6f66  in any copies of
+000029b0: 2074 6865 2073 6f75 7263 6520 636f 6465   the source code
+000029c0: 2e20 4e6f 7465 2c20 7468 6174 2074 6865  . Note, that the
+000029d0: 2064 6174 6120 7573 6564 2062 7920 7468   data used by th
+000029e0: 6520 7061 636b 6167 6520 6973 206c 6963  e package is lic
+000029f0: 656e 7365 6420 756e 6465 7220 6120 6469  ensed under a di
+00002a00: 6666 6572 656e 7420 636f 7079 7269 6768  fferent copyrigh
+00002a10: 742e 0d0a 0d0a 5468 6520 6461 7461 2069  t.....The data i
+00002a20: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00002a30: 205b 4343 2042 592d 5341 2034 2e30 5d5b   [CC BY-SA 4.0][
+00002a40: 6461 7461 2d63 635d 0d0a 0d0a 0d0a 0d0a  data-cc]........
+00002a50: 3c21 2d2d 204d 4152 4b44 4f57 4e20 4c49  <!-- MARKDOWN LI
+00002a60: 4e4b 5320 2d2d 3e0d 0a5b 7465 7374 735d  NKS -->..[tests]
+00002a70: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00002a80: 2e63 6f6d 2f61 6e64 7265 6968 6172 2f74  .com/andreihar/t
+00002a90: 6169 6275 6e2f 6163 7469 6f6e 730d 0a5b  aibun/actions..[
+00002aa0: 7465 7374 732d 6261 6467 655d 3a20 6874  tests-badge]: ht
+00002ab0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00002ac0: 732e 696f 2f67 6974 6875 622f 6163 7469  s.io/github/acti
+00002ad0: 6f6e 732f 776f 726b 666c 6f77 2f73 7461  ons/workflow/sta
+00002ae0: 7475 732f 616e 6472 6569 6861 722f 7461  tus/andreihar/ta
+00002af0: 6962 756e 2f63 692e 7961 6d6c 3f73 7479  ibun/ci.yaml?sty
+00002b00: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00002b10: 266c 6f67 6f3d 6769 7468 7562 0d0a 5b63  &logo=github..[c
+00002b20: 6f6e 7472 6962 7574 6f72 732d 6261 6467  ontributors-badg
+00002b30: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
+00002b40: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00002b50: 622f 636f 6e74 7269 6275 746f 7273 2f61  b/contributors/a
+00002b60: 6e64 7265 6968 6172 2f74 6169 6275 6e3f  ndreihar/taibun?
+00002b70: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
+00002b80: 6467 650d 0a5b 636f 6e74 7269 6275 746f  dge..[contributo
+00002b90: 7273 5d3a 2023 7573 6167 650d 0a5b 7265  rs]: #usage..[re
+00002ba0: 6c65 6173 652d 6261 6467 655d 3a20 6874  lease-badge]: ht
+00002bb0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00002bc0: 732e 696f 2f67 6974 6875 622f 762f 7265  s.io/github/v/re
+00002bd0: 6c65 6173 652f 616e 6472 6569 6861 722f  lease/andreihar/
+00002be0: 7461 6962 756e 3f63 6f6c 6f72 3d33 3836  taibun?color=386
+00002bf0: 3138 6326 7374 796c 653d 666f 722d 7468  18c&style=for-th
+00002c00: 652d 6261 6467 650d 0a5b 7265 6c65 6173  e-badge..[releas
+00002c10: 655d 3a20 6874 7470 733a 2f2f 6769 7468  e]: https://gith
+00002c20: 7562 2e63 6f6d 2f61 6e64 7265 6968 6172  ub.com/andreihar
+00002c30: 2f74 6169 6275 6e2f 7265 6c65 6173 6573  /taibun/releases
+00002c40: 0d0a 5b6c 6963 656e 6365 2d62 6164 6765  ..[licence-badge
+00002c50: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
+00002c60: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00002c70: 2f6c 6963 656e 7365 2f61 6e64 7265 6968  /license/andreih
+00002c80: 6172 2f74 6169 6275 6e3f 636f 6c6f 723d  ar/taibun?color=
+00002c90: 3030 3030 3030 2673 7479 6c65 3d66 6f72  000000&style=for
+00002ca0: 2d74 6865 2d62 6164 6765 0d0a 5b6c 6963  -the-badge..[lic
+00002cb0: 656e 6365 5d3a 204c 4943 454e 5345 0d0a  ence]: LICENSE..
+00002cc0: 5b6c 696e 6b65 6469 6e2d 6261 6467 655d  [linkedin-badge]
+00002cd0: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
+00002ce0: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+00002cf0: 696e 6b65 6449 6e2d 3030 3737 4235 3f73  inkedIn-0077B5?s
+00002d00: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+00002d10: 6765 266c 6f67 6f3d 6c69 6e6b 6564 696e  ge&logo=linkedin
+00002d20: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
+00002d30: 0d0a 5b6c 696e 6b65 6469 6e5d 3a20 6874  ..[linkedin]: ht
+00002d40: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
+00002d50: 696e 2e63 6f6d 2f69 6e2f 616e 6472 6569  in.com/in/andrei
+00002d60: 2d68 6172 6261 6368 6f76 2f0d 0a0d 0a5b  -harbachov/....[
+00002d70: 7079 7069 5d3a 2068 7474 7073 3a2f 2f70  pypi]: https://p
+00002d80: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00002d90: 7461 6962 756e 0d0a 5b62 7567 5d3a 2068  taibun..[bug]: h
+00002da0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002db0: 6d2f 616e 6472 6569 6861 722f 7461 6962  m/andreihar/taib
+00002dc0: 756e 2f69 7373 7565 730d 0a5b 6f6e 6c69  un/issues..[onli
+00002dd0: 6e65 2d64 6963 7469 6f6e 6172 795d 3a20  ne-dictionary]: 
+00002de0: 6874 7470 3a2f 2f69 7031 3934 3039 372e  http://ip194097.
+00002df0: 6e74 6375 2e65 6475 2e74 772f 756e 6769  ntcu.edu.tw/ungi
+00002e00: 616e 2f73 6f61 6e6e 7465 6e67 2f63 6869  an/soannteng/chi
+00002e10: 6c2f 5461 6968 6f61 2e61 7370 0d0a 5b69  l/Taihoa.asp..[i
+00002e20: 7461 6967 692d 6469 6374 696f 6e61 7279  taigi-dictionary
+00002e30: 5d3a 2068 7474 7073 3a2f 2f69 7461 6967  ]: https://itaig
+00002e40: 692e 7477 2f0d 0a5b 6461 7461 2d76 6961  i.tw/..[data-via
+00002e50: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00002e60: 622e 636f 6d2f 4368 686f 6554 6169 6769  b.com/ChhoeTaigi
+00002e70: 2f43 6868 6f65 5461 6967 6944 6174 6162  /ChhoeTaigiDatab
+00002e80: 6173 650d 0a5b 6461 7461 2d63 635d 3a20  ase..[data-cc]: 
+00002e90: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
+00002ea0: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
+00002eb0: 6e73 6573 2f62 792d 7361 2f34 2e30 2f64  nses/by-sa/4.0/d
+00002ec0: 6565 642e 656e 0d0a 5b73 616d 7565 6c2d  eed.en..[samuel-
+00002ed0: 6769 7468 7562 5d3a 2068 7474 7073 3a2f  github]: https:/
+00002ee0: 2f67 6974 6875 622e 636f 6d2f 5353 5361  /github.com/SSSa
+00002ef0: 6d0d 0a5b 7361 6d75 656c 2d6c 696e 6b65  m..[samuel-linke
+00002f00: 6469 6e5d 3a20 6874 7470 733a 2f2f 7777  din]: https://ww
+00002f10: 772e 6c69 6e6b 6564 696e 2e63 6f6d 2f69  w.linkedin.com/i
+00002f20: 6e2f 7361 6d75 656c 2d6a 656e 2f0d 0a0d  n/samuel-jen/...
+00002f30: 0a5b 7461 696c 6f2d 7769 6b69 5d3a 2068  .[tailo-wiki]: h
+00002f40: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00002f50: 6469 612e 6f72 672f 7769 6b69 2f54 2543  dia.org/wiki/T%C
+00002f60: 3325 4132 692d 7525 4333 2541 326e 5f4c  3%A2i-u%C3%A2n_L
+00002f70: 2543 3325 4234 2d6d 2543 3325 4131 2d6a  %C3%B4-m%C3%A1-j
+00002f80: 2543 3425 4142 5f50 6869 6e67 2d69 6d5f  %C4%AB_Phing-im_
+00002f90: 486f 6e67 2d25 4333 2541 306e 0d0a 5b70  Hong-%C3%A0n..[p
+00002fa0: 6f6a 2d77 696b 695d 3a20 6874 7470 733a  oj-wiki]: https:
+00002fb0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00002fc0: 7267 2f77 696b 692f 5065 2543 4325 3844  rg/wiki/Pe%CC%8D
+00002fd0: 682d 2543 3525 3844 652d 6a25 4334 2541  h-%C5%8De-j%C4%A
+00002fe0: 420d 0a5b 7a68 7579 696e 2d77 696b 695d  B..[zhuyin-wiki]
+00002ff0: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
+00003000: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00003010: 5461 6977 616e 6573 655f 5068 6f6e 6574  Taiwanese_Phonet
+00003020: 6963 5f53 796d 626f 6c73 0d0a 5b74 6c70  ic_Symbols..[tlp
+00003030: 612d 7769 6b69 5d3a 2068 7474 7073 3a2f  a-wiki]: https:/
+00003040: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00003050: 672f 7769 6b69 2f54 6169 7761 6e65 7365  g/wiki/Taiwanese
+00003060: 5f4c 616e 6775 6167 655f 5068 6f6e 6574  _Language_Phonet
+00003070: 6963 5f41 6c70 6861 6265 740d 0a5b 7069  ic_Alphabet..[pi
+00003080: 6e67 7969 6d2d 7769 6b69 5d3a 2068 7474  ngyim-wiki]: htt
+00003090: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+000030a0: 612e 6f72 672f 7769 6b69 2f42 6225 4333  a.org/wiki/Bb%C3
+000030b0: 2541 316e 6c25 4333 2541 316d 5f70 2543  %A1nl%C3%A1m_p%C
+000030c0: 3325 4143 6e67 7925 4334 2541 426d 0d0a  3%ACngy%C4%ABm..
+000030d0: 5b74 6f6e 6769 6f6e 672d 7769 6b69 5d3a  [tongiong-wiki]:
+000030e0: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+000030f0: 7065 6469 612e 6f72 672f 7769 6b69 2f44  pedia.org/wiki/D
+00003100: 6125 4334 2541 422d 6768 2543 3325 4145  a%C4%AB-gh%C3%AE
+00003110: 5f74 2543 3525 3844 6e67 2d69 2543 3525  _t%C5%8Dng-i%C5%
+00003120: 3844 6e67 5f70 2543 3425 4142 6e67 2d69  8Dng_p%C4%ABng-i
+00003130: 6d0d 0a5b 6970 612d 7769 6b69 5d3a 2068  m..[ipa-wiki]: h
+00003140: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00003150: 6469 612e 6f72 672f 7769 6b69 2f49 6e74  dia.org/wiki/Int
+00003160: 6572 6e61 7469 6f6e 616c 5f50 686f 6e65  ernational_Phone
+00003170: 7469 635f 416c 7068 6162 6574 0d0a 5b7a  tic_Alphabet..[z
+00003180: 6861 6e67 7a68 6f75 2d77 696b 695d 3a20  hangzhou-wiki]: 
+00003190: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+000031a0: 6564 6961 2e6f 7267 2f77 696b 692f 5a68  edia.org/wiki/Zh
+000031b0: 616e 677a 686f 755f 6469 616c 6563 7473  angzhou_dialects
+000031c0: 0d0a 5b71 7561 6e7a 686f 752d 7769 6b69  ..[quanzhou-wiki
+000031d0: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
+000031e0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+000031f0: 2f51 7561 6e7a 686f 755f 6469 616c 6563  /Quanzhou_dialec
+00003200: 7473 0d0a 5b6e 6c74 6b2d 746f 6b65 6e69  ts..[nltk-tokeni
+00003210: 7a65 5d3a 2068 7474 7073 3a2f 2f6e 6c74  ze]: https://nlt
+00003220: 6b2e 6f72 672f 6170 692f 6e6c 746b 2e74  k.org/api/nltk.t
+00003230: 6f6b 656e 697a 652e 6874 6d6c 0d0a 5b73  okenize.html..[s
+00003240: 616e 6468 692d 7769 6b69 5d3a 2068 7474  andhi-wiki]: htt
+00003250: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00003260: 612e 6f72 672f 7769 6b69 2f54 6169 7761  a.org/wiki/Taiwa
+00003270: 6e65 7365 5f48 6f6b 6b69 656e 2354 6f6e  nese_Hokkien#Ton
+00003280: 6525 3230 7361 6e64 6869 3a7e 3a74 6578  e%20sandhi:~:tex
+00003290: 743d 7468 6e67 2545 3225 3946 2541 3925  t=thng%E2%9F%A9%
+000032a0: 3230 2825 3232 736f 7570 2532 3229 2e2d  20(%22soup%22).-
+000032b0: 2c54 6f6e 6525 3230 7361 6e64 6869 2c2d  ,Tone%20sandhi,-
+000032c0: 2535 4265 6469 7425 3544 0d0a            %5Bedit%5D..
```

### Comparing `example990420-0.0.7/taibun/data/simplified.json` & `example990420-1.1.0/taibun/data/simplified.json`

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

