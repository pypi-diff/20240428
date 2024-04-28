# Comparing `tmp/regex-2023.8.8.tar.gz` & `tmp/regex-2024.4.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-2023.8.8.tar", last modified: Tue Aug  8 20:38:00 2023, max compression
+gzip compressed data, was "regex-2024.4.16.tar", last modified: Tue Apr 16 18:37:13 2024, max compression
```

## Comparing `regex-2023.8.8.tar` & `regex-2024.4.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.256177 regex-2023.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-08-08 20:37:59.000000 regex-2023.8.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-08 20:37:59.000000 regex-2023.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-08-08 20:38:00.256177 regex-2023.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39805 2023-08-08 20:37:59.000000 regex-2023.8.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.248177 regex-2023.8.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   143294 2023-08-08 20:37:59.000000 regex-2023.8.8/docs/Features.html
--rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-08-08 20:37:59.000000 regex-2023.8.8/docs/UnicodeProperties.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 20:37:59.000000 regex-2023.8.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.248177 regex-2023.8.8/regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-08-08 20:38:00.000000 regex-2023.8.8/regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 20:38:00.000000 regex-2023.8.8/regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:38:00.000000 regex-2023.8.8/regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 20:38:00.000000 regex-2023.8.8/regex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.252177 regex-2023.8.8/regex_3/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   826026 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex.c
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex.h
--rw-r--r--   0 runner    (1001) docker     (123)   141166 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex_core.py
--rw-r--r--   0 runner    (1001) docker     (123)  1837887 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex_unicode.c
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex_unicode.h
--rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)   220168 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:38:00.256177 regex-2023.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-08 20:37:59.000000 regex-2023.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.252177 regex-2023.8.8/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    55247 2023-08-08 20:37:59.000000 regex-2023.8.8/tools/build_regex_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:37:13.015751 regex-2024.4.16/
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-16 18:37:11.000000 regex-2024.4.16/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 18:37:11.000000 regex-2024.4.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40896 2024-04-16 18:37:13.015751 regex-2024.4.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39805 2024-04-16 18:37:11.000000 regex-2024.4.16/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:37:13.007750 regex-2024.4.16/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   143294 2024-04-16 18:37:11.000000 regex-2024.4.16/docs/Features.html
+-rw-r--r--   0 runner    (1001) docker     (127)    29426 2024-04-16 18:37:11.000000 regex-2024.4.16/docs/UnicodeProperties.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 18:37:11.000000 regex-2024.4.16/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:37:13.007750 regex-2024.4.16/regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40896 2024-04-16 18:37:12.000000 regex-2024.4.16/regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-16 18:37:12.000000 regex-2024.4.16/regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:37:12.000000 regex-2024.4.16/regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 18:37:12.000000 regex-2024.4.16/regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:37:13.011751 regex-2024.4.16/regex_3/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 18:37:11.000000 regex-2024.4.16/regex_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   826026 2024-04-16 18:37:11.000000 regex-2024.4.16/regex_3/_regex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-16 18:37:11.000000 regex-2024.4.16/regex_3/_regex.h
+-rw-r--r--   0 runner    (1001) docker     (127)   140971 2024-04-16 18:37:11.000000 regex-2024.4.16/regex_3/_regex_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1878313 2024-04-16 18:37:11.000000 regex-2024.4.16/regex_3/_regex_unicode.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-16 18:37:11.000000 regex-2024.4.16/regex_3/_regex_unicode.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32683 2024-04-16 18:37:11.000000 regex-2024.4.16/regex_3/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   219821 2024-04-16 18:37:11.000000 regex-2024.4.16/regex_3/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:37:13.015751 regex-2024.4.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-16 18:37:11.000000 regex-2024.4.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:37:13.015751 regex-2024.4.16/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    56426 2024-04-16 18:37:11.000000 regex-2024.4.16/tools/build_regex_unicode.py
```

### Comparing `regex-2023.8.8/LICENSE.txt` & `regex-2024.4.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `regex-2023.8.8/PKG-INFO` & `regex-2024.4.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2023.8.8
+Version: 2024.4.16
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Introduction
 ------------
 
 This regex implementation is backwards-compatible with the standard 're' module, but offers additional functionality.
@@ -49,15 +48,15 @@
 --------------
 
 The regex module releases the GIL during matching on instances of the built-in (immutable) string classes, enabling other Python threads to run concurrently. It is also possible to force the regex module to release the GIL during matching by calling the matching methods with the keyword argument ``concurrent=True``. The behaviour is undefined if the string changes during matching, so use it *only* when it is guaranteed that that won't happen.
 
 Unicode
 -------
 
-This module supports Unicode 15.0.0. Full Unicode case-folding is supported.
+This module supports Unicode 15.1.0. Full Unicode case-folding is supported.
 
 Flags
 -----
 
 There are 2 kinds of flag: scoped and global. Scoped flags can apply to only part of a pattern and can be turned on or off; global flags apply to the entire pattern and can only be turned on.
 
 The scoped flags are: ``ASCII (?a)``, ``FULLCASE (?f)``, ``IGNORECASE (?i)``, ``LOCALE (?L)``, ``MULTILINE (?m)``, ``DOTALL (?s)``, ``UNICODE (?u)``, ``VERBOSE (?x)``, ``WORD (?w)``.
```

### Comparing `regex-2023.8.8/README.rst` & `regex-2024.4.16/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 --------------
 
 The regex module releases the GIL during matching on instances of the built-in (immutable) string classes, enabling other Python threads to run concurrently. It is also possible to force the regex module to release the GIL during matching by calling the matching methods with the keyword argument ``concurrent=True``. The behaviour is undefined if the string changes during matching, so use it *only* when it is guaranteed that that won't happen.
 
 Unicode
 -------
 
-This module supports Unicode 15.0.0. Full Unicode case-folding is supported.
+This module supports Unicode 15.1.0. Full Unicode case-folding is supported.
 
 Flags
 -----
 
 There are 2 kinds of flag: scoped and global. Scoped flags can apply to only part of a pattern and can be turned on or off; global flags apply to the entire pattern and can only be turned on.
 
 The scoped flags are: ``ASCII (?a)``, ``FULLCASE (?f)``, ``IGNORECASE (?i)``, ``LOCALE (?L)``, ``MULTILINE (?m)``, ``DOTALL (?s)``, ``UNICODE (?u)``, ``VERBOSE (?x)``, ``WORD (?w)``.
```

### Comparing `regex-2023.8.8/docs/Features.html` & `regex-2024.4.16/docs/Features.html`

 * *Files 0% similar despite different names*

#### Comparing `regex-2023.8.8/docs/Features.html` & `regex-2024.4.16/docs/Features.html`

```diff
@@ -383,15 +383,15 @@
           . The behaviour is undefined if the string changes during matching, so use it
           <em>only</em>
           when it is guaranteed that that won't happen.
         </p>
       </div>
       <div class="section" id="unicode">
         <h1>Unicode</h1>
-        <p>This module supports Unicode 15.0.0. Full Unicode case-folding is supported.</p>
+        <p>This module supports Unicode 15.1.0. Full Unicode case-folding is supported.</p>
       </div>
       <div class="section" id="flags">
         <h1>Flags</h1>
         <p>There are 2 kinds of flag: scoped and global. Scoped flags can apply to only part of a pattern and can be turned on or off; global flags apply to the entire pattern and can only be turned on.</p>
         <p>
           The scoped flags are:
           <tt class="docutils literal">
```

### Comparing `regex-2023.8.8/docs/UnicodeProperties.rst` & `regex-2024.4.16/docs/UnicodeProperties.rst`

 * *Files identical despite different names*

### Comparing `regex-2023.8.8/regex.egg-info/PKG-INFO` & `regex-2024.4.16/regex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2023.8.8
+Version: 2024.4.16
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Introduction
 ------------
 
 This regex implementation is backwards-compatible with the standard 're' module, but offers additional functionality.
@@ -49,15 +48,15 @@
 --------------
 
 The regex module releases the GIL during matching on instances of the built-in (immutable) string classes, enabling other Python threads to run concurrently. It is also possible to force the regex module to release the GIL during matching by calling the matching methods with the keyword argument ``concurrent=True``. The behaviour is undefined if the string changes during matching, so use it *only* when it is guaranteed that that won't happen.
 
 Unicode
 -------
 
-This module supports Unicode 15.0.0. Full Unicode case-folding is supported.
+This module supports Unicode 15.1.0. Full Unicode case-folding is supported.
 
 Flags
 -----
 
 There are 2 kinds of flag: scoped and global. Scoped flags can apply to only part of a pattern and can be turned on or off; global flags apply to the entire pattern and can only be turned on.
 
 The scoped flags are: ``ASCII (?a)``, ``FULLCASE (?f)``, ``IGNORECASE (?i)``, ``LOCALE (?L)``, ``MULTILINE (?m)``, ``DOTALL (?s)``, ``UNICODE (?u)``, ``VERBOSE (?x)``, ``WORD (?w)``.
```

### Comparing `regex-2023.8.8/regex_3/_regex.c` & `regex-2024.4.16/regex_3/_regex.c`

 * *Files identical despite different names*

### Comparing `regex-2023.8.8/regex_3/_regex.h` & `regex-2024.4.16/regex_3/_regex.h`

 * *Files identical despite different names*

### Comparing `regex-2023.8.8/regex_3/_regex_core.py` & `regex-2024.4.16/regex_3/_regex_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1146,30 +1146,15 @@
         parse_positional_flags(source, info, flags_on, flags_off)
         return None
 
     raise error("unknown extension", source.string, source.pos)
 
 def parse_positional_flags(source, info, flags_on, flags_off):
     "Parses positional flags."
-    version = (info.flags & _ALL_VERSIONS) or DEFAULT_VERSION
-    if version == VERSION0:
-        # Positional flags are global and can only be turned on.
-        if flags_off:
-            raise error("bad inline flags: cannot turn flags off",
-              source.string, source.pos)
-
-        new_global_flags = flags_on & ~info.global_flags
-        if new_global_flags:
-            info.global_flags |= new_global_flags
-
-            # A global has been turned on, so reparse the pattern.
-            raise _UnscopedFlagSet(info.global_flags)
-    else:
-        info.flags = (info.flags | flags_on) & ~flags_off
-
+    info.flags = (info.flags | flags_on) & ~flags_off
     source.ignore_space = bool(info.flags & VERBOSE)
 
 def parse_name(source, allow_numeric=False, allow_group_0=False):
     "Parses a name."
     name = source.get_while(set(")>"), include=False)
 
     if not name:
@@ -1229,14 +1214,22 @@
         return parse_string_set(source, info)
     elif ch == "N":
         # A named codepoint.
         return parse_named_char(source, info, in_set)
     elif ch in "pP":
         # A Unicode property, positive or negative.
         return parse_property(source, info, ch == "p", in_set)
+    elif ch == "R" and not in_set:
+        # A line ending.
+        charset = [0x0A, 0x0B, 0x0C, 0x0D]
+        if info.guess_encoding == UNICODE:
+            charset.extend([0x85, 0x2028, 0x2029])
+
+        return Atomic(Branch([String([0x0D, 0x0A]), SetUnion(info, [Character(c)
+          for c in charset])]))
     elif ch == "X" and not in_set:
         # A grapheme cluster.
         return Grapheme()
     elif ch in ALPHA:
         # An alphabetic escape sequence.
         # Positional escapes aren't allowed inside a character set.
         if not in_set:
@@ -2114,14 +2107,17 @@
         fs = set()
         for b in self.branches:
             fs |= b.get_firstset(reverse)
 
         return fs or set([None])
 
     def _compile(self, reverse, fuzzy):
+        if not self.branches:
+            return []
+
         code = [(OP.BRANCH, )]
         for b in self.branches:
             code.extend(b.compile(reverse, fuzzy))
             code.append((OP.NEXT, ))
 
         code[-1] = (OP.END, )
```

### Comparing `regex-2023.8.8/regex_3/_regex_unicode.c` & `regex-2024.4.16/regex_3/_regex_unicode.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* For Unicode version 15.0.0 */
+/* For Unicode version 15.1.0 */
 
 #include "_regex_unicode.h"
 
 #define RE_BLANK_MASK ((1 << RE_PROP_ZL) | (1 << RE_PROP_ZP))
 #define RE_GRAPH_MASK ((1 << RE_PROP_CC) | (1 << RE_PROP_CS) | (1 << RE_PROP_CN))
 #define RE_WORD_MASK (RE_PROP_M_MASK | (1 << RE_PROP_ND) | (1 << RE_PROP_PC))
 
@@ -46,16 +46,18 @@
     "100",
     "1000",
     "10000",
     "100000",
     "1000000",
     "10000000",
     "100000000",
+    "1000000000",
     "10000000000",
     "1000000000000",
+    "10000000000000000",
     "103",
     "107",
     "11",
     "11/12",
     "11/2",
     "118",
     "12",
@@ -198,14 +200,18 @@
     "AFRICANNOON",
     "AFRICANQAF",
     "AGHB",
     "AHEX",
     "AHOM",
     "AI",
     "AIN",
+    "AK",
+    "AKSARA",
+    "AKSARAPREBASE",
+    "AKSARASTART",
     "AL",
     "ALAPH",
     "ALCHEMICAL",
     "ALCHEMICALSYMBOLS",
     "ALEF",
     "ALETTER",
     "ALNUM",
@@ -218,14 +224,15 @@
     "AN",
     "ANATOLIANHIEROGLYPHS",
     "ANCIENTGREEKMUSIC",
     "ANCIENTGREEKMUSICALNOTATION",
     "ANCIENTGREEKNUMBERS",
     "ANCIENTSYMBOLS",
     "ANY",
+    "AP",
     "AR",
     "ARAB",
     "ARABIC",
     "ARABICEXTA",
     "ARABICEXTB",
     "ARABICEXTC",
     "ARABICEXTENDEDA",
@@ -241,14 +248,15 @@
     "ARABICPRESENTATIONFORMSB",
     "ARABICSUP",
     "ARABICSUPPLEMENT",
     "ARMENIAN",
     "ARMI",
     "ARMN",
     "ARROWS",
+    "AS",
     "ASCII",
     "ASCIIHEXDIGIT",
     "ASSIGNED",
     "AT",
     "ATA",
     "ATAR",
     "ATB",
@@ -414,28 +422,30 @@
     "CJKEXTB",
     "CJKEXTC",
     "CJKEXTD",
     "CJKEXTE",
     "CJKEXTF",
     "CJKEXTG",
     "CJKEXTH",
+    "CJKEXTI",
     "CJKRADICALSSUP",
     "CJKRADICALSSUPPLEMENT",
     "CJKSTROKES",
     "CJKSYMBOLS",
     "CJKSYMBOLSANDPUNCTUATION",
     "CJKUNIFIEDIDEOGRAPHS",
     "CJKUNIFIEDIDEOGRAPHSEXTENSIONA",
     "CJKUNIFIEDIDEOGRAPHSEXTENSIONB",
     "CJKUNIFIEDIDEOGRAPHSEXTENSIONC",
     "CJKUNIFIEDIDEOGRAPHSEXTENSIOND",
     "CJKUNIFIEDIDEOGRAPHSEXTENSIONE",
     "CJKUNIFIEDIDEOGRAPHSEXTENSIONF",
     "CJKUNIFIEDIDEOGRAPHSEXTENSIONG",
     "CJKUNIFIEDIDEOGRAPHSEXTENSIONH",
+    "CJKUNIFIEDIDEOGRAPHSEXTENSIONI",
     "CL",
     "CLOSE",
     "CLOSEPARENTHESIS",
     "CLOSEPUNCTUATION",
     "CM",
     "CN",
     "CNTRL",
@@ -728,28 +738,34 @@
     "HRKT",
     "HST",
     "HUNG",
     "HY",
     "HYPHEN",
     "ID",
     "IDC",
+    "IDCOMPATMATHCONTINUE",
+    "IDCOMPATMATHSTART",
     "IDCONTINUE",
     "IDEO",
     "IDEOGRAPHIC",
     "IDEOGRAPHICDESCRIPTIONCHARACTERS",
     "IDEOGRAPHICSYMBOLS",
     "IDEOGRAPHICSYMBOLSANDPUNCTUATION",
     "IDS",
     "IDSB",
     "IDSBINARYOPERATOR",
     "IDST",
     "IDSTART",
     "IDSTRINARYOPERATOR",
+    "IDSU",
+    "IDSUNARYOPERATOR",
     "IMPERIALARAMAIC",
     "IN",
+    "INCB",
+    "INDICCONJUNCTBREAK",
     "INDICNUMBERFORMS",
     "INDICPOSITIONALCATEGORY",
     "INDICSIYAQNUMBERS",
     "INDICSYLLABICCATEGORY",
     "INFIXNUMERIC",
     "INHERITED",
     "INIT",
@@ -875,14 +891,15 @@
     "LINEARA",
     "LINEARB",
     "LINEARBIDEOGRAMS",
     "LINEARBSYLLABARY",
     "LINEBREAK",
     "LINEFEED",
     "LINESEPARATOR",
+    "LINKER",
     "LISU",
     "LISUSUP",
     "LISUSUPPLEMENT",
     "LL",
     "LM",
     "LO",
     "LOE",
@@ -1435,15 +1452,18 @@
     "VEDICEXT",
     "VEDICEXTENSIONS",
     "VERT",
     "VERTICAL",
     "VERTICALFORMS",
     "VERTICALTAIL",
     "VERTSPACE",
+    "VF",
+    "VI",
     "VIRAMA",
+    "VIRAMAFINAL",
     "VISARGA",
     "VISUALORDERLEFT",
     "VITH",
     "VITHKUQI",
     "VOWEL",
     "VOWELDEPENDENT",
     "VOWELINDEPENDENT",
@@ -1507,1828 +1527,1852 @@
     "ZWSPACE",
     "ZYYY",
     "ZZZZ",
 };
 
 /* Properties. */
 RE_Property re_properties[] = {
-    { 189,  0,  0}, /* ALPHABETIC */
-    { 188,  0,  0}, /* ALPHA */
-    { 192,  1,  0}, /* ALPHANUMERIC */
-    { 187,  1,  0}, /* ALNUM */
-    { 200,  2,  0}, /* ANY */
-    { 225,  3,  0}, /* ASCIIHEXDIGIT */
-    { 177,  3,  0}, /* AHEX */
-    { 266,  4,  1}, /* BIDICLASS */
-    { 255,  4,  1}, /* BC */
-    { 267,  5,  0}, /* BIDICONTROL */
-    { 265,  5,  0}, /* BIDIC */
-    { 269,  6,  0}, /* BIDIMIRRORED */
-    { 268,  6,  0}, /* BIDIM */
-    { 273,  7,  0}, /* BLANK */
-    { 275,  8,  2}, /* BLOCK */
-    { 274,  8,  2}, /* BLK */
-    { 312,  9,  3}, /* CANONICALCOMBININGCLASS */
-    { 324,  9,  3}, /* CCC */
-    { 318, 10,  0}, /* CASED */
-    { 320, 11,  0}, /* CASEIGNORABLE */
-    { 377, 11,  0}, /* CI */
-    { 365, 12,  0}, /* CHANGESWHENCASEFOLDED */
-    { 466, 12,  0}, /* CWCF */
-    { 366, 13,  0}, /* CHANGESWHENCASEMAPPED */
-    { 467, 13,  0}, /* CWCM */
-    { 367, 14,  0}, /* CHANGESWHENLOWERCASED */
-    { 468, 14,  0}, /* CWL */
-    { 368, 15,  0}, /* CHANGESWHENTITLECASED */
-    { 469, 15,  0}, /* CWT */
-    { 369, 16,  0}, /* CHANGESWHENUPPERCASED */
-    { 470, 16,  0}, /* CWU */
-    { 491, 17,  0}, /* DASH */
-    { 497, 18,  4}, /* DECOMPOSITIONTYPE */
-    { 528, 18,  4}, /* DT */
-    { 498, 19,  0}, /* DEFAULTIGNORABLECODEPOINT */
-    { 508, 19,  0}, /* DI */
-    { 500, 20,  0}, /* DEPRECATED */
-    { 499, 20,  0}, /* DEP */
-    { 510, 21,  0}, /* DIACRITIC */
-    { 509, 21,  0}, /* DIA */
-    { 535, 22,  5}, /* EASTASIANWIDTH */
-    { 533, 22,  5}, /* EA */
-    { 551, 23,  0}, /* EMOJI */
-    { 552, 24,  0}, /* EMOJICOMPONENT */
-    { 540, 24,  0}, /* ECOMP */
-    { 553, 25,  0}, /* EMOJIMODIFIER */
-    { 549, 25,  0}, /* EMOD */
-    { 554, 26,  0}, /* EMOJIMODIFIERBASE */
-    { 537, 26,  0}, /* EBASE */
-    { 555, 27,  0}, /* EMOJIPRESENTATION */
-    { 568, 27,  0}, /* EPRES */
-    { 588, 28,  0}, /* EXTENDEDPICTOGRAPHIC */
-    { 591, 28,  0}, /* EXTPICT */
-    { 589, 29,  0}, /* EXTENDER */
-    { 586, 29,  0}, /* EXT */
-    { 615, 30,  6}, /* GENERALCATEGORY */
-    { 612, 30,  6}, /* GC */
-    { 639, 31,  0}, /* GRAPH */
-    { 640, 32,  0}, /* GRAPHEMEBASE */
-    { 644, 32,  0}, /* GRBASE */
-    { 641, 33,  7}, /* GRAPHEMECLUSTERBREAK */
-    { 613, 33,  7}, /* GCB */
-    { 642, 34,  0}, /* GRAPHEMEEXTEND */
-    { 650, 34,  0}, /* GREXT */
-    { 643, 35,  0}, /* GRAPHEMELINK */
-    { 651, 35,  0}, /* GRLINK */
-    { 674, 36,  8}, /* HANGULSYLLABLETYPE */
-    { 705, 36,  8}, /* HST */
-    { 693, 37,  0}, /* HEXDIGIT */
-    { 692, 37,  0}, /* HEX */
-    { 703, 38,  0}, /* HORIZSPACE */
-    { 657, 38,  0}, /* H */
-    { 708, 39,  0}, /* HYPHEN */
-    { 711, 40,  0}, /* IDCONTINUE */
-    { 710, 40,  0}, /* IDC */
-    { 713, 41,  0}, /* IDEOGRAPHIC */
-    { 712, 41,  0}, /* IDEO */
-    { 719, 42,  0}, /* IDSBINARYOPERATOR */
-    { 718, 42,  0}, /* IDSB */
-    { 721, 43,  0}, /* IDSTART */
-    { 717, 43,  0}, /* IDS */
-    { 722, 44,  0}, /* IDSTRINARYOPERATOR */
-    { 720, 44,  0}, /* IDST */
-    { 726, 45,  9}, /* INDICPOSITIONALCATEGORY */
-    { 734, 45,  9}, /* INPC */
-    { 728, 46, 10}, /* INDICSYLLABICCATEGORY */
-    { 735, 46, 10}, /* INSC */
-    { 757, 47,  0}, /* JOINCONTROL */
-    { 755, 47,  0}, /* JOINC */
-    { 759, 48, 11}, /* JOININGGROUP */
-    { 753, 48, 11}, /* JG */
-    { 760, 49, 12}, /* JOININGTYPE */
-    { 761, 49, 12}, /* JT */
-    { 855, 50, 13}, /* LINEBREAK */
-    { 830, 50, 13}, /* LB */
-    { 865, 51,  0}, /* LOGICALORDEREXCEPTION */
-    { 864, 51,  0}, /* LOE */
-    { 867, 52,  0}, /* LOWERCASE */
-    { 866, 52,  0}, /* LOWER */
-    { 939, 53,  0}, /* MATH */
-    {1029, 54, 14}, /* NFCQUICKCHECK */
-    {1028, 54, 14}, /* NFCQC */
-    {1031, 55, 15}, /* NFDQUICKCHECK */
-    {1030, 55, 15}, /* NFDQC */
-    {1033, 56, 14}, /* NFKCQUICKCHECK */
-    {1032, 56, 14}, /* NFKCQC */
-    {1035, 57, 15}, /* NFKDQUICKCHECK */
-    {1034, 57, 15}, /* NFKDQC */
-    {1044, 58,  0}, /* NONCHARACTERCODEPOINT */
-    {1021, 58,  0}, /* NCHAR */
-    {1064, 59, 16}, /* NUMERICTYPE */
-    {1057, 59, 16}, /* NT */
-    {1065, 60, 17}, /* NUMERICVALUE */
-    {1068, 60, 17}, /* NV */
-    {1106, 61,  0}, /* OTHERALPHABETIC */
-    {1071, 61,  0}, /* OALPHA */
-    {1107, 62,  0}, /* OTHERDEFAULTIGNORABLECODEPOINT */
-    {1073, 62,  0}, /* ODI */
-    {1108, 63,  0}, /* OTHERGRAPHEMEEXTEND */
-    {1076, 63,  0}, /* OGREXT */
-    {1109, 64,  0}, /* OTHERIDCONTINUE */
-    {1077, 64,  0}, /* OIDC */
-    {1110, 65,  0}, /* OTHERIDSTART */
-    {1078, 65,  0}, /* OIDS */
-    {1112, 66,  0}, /* OTHERLOWERCASE */
-    {1091, 66,  0}, /* OLOWER */
-    {1113, 67,  0}, /* OTHERMATH */
-    {1092, 67,  0}, /* OMATH */
-    {1118, 68,  0}, /* OTHERUPPERCASE */
-    {1121, 68,  0}, /* OUPPER */
-    {1132, 69,  0}, /* PATTERNSYNTAX */
-    {1131, 69,  0}, /* PATSYN */
-    {1133, 70,  0}, /* PATTERNWHITESPACE */
-    {1134, 70,  0}, /* PATWS */
-    {1163, 71,  0}, /* POSIXALNUM */
-    {1164, 72,  0}, /* POSIXDIGIT */
-    {1165, 73,  0}, /* POSIXPUNCT */
-    {1166, 74,  0}, /* POSIXXDIGIT */
-    {1172, 75,  0}, /* PREPENDEDCONCATENATIONMARK */
-    {1138, 75,  0}, /* PCM */
-    {1173, 76,  0}, /* PRINT */
-    {1190, 77,  0}, /* QUOTATIONMARK */
-    {1187, 77,  0}, /* QMARK */
-    {1192, 78,  0}, /* RADICAL */
-    {1193, 79,  0}, /* REGIONALINDICATOR */
-    {1198, 79,  0}, /* RI */
-    {1228, 80, 18}, /* SCRIPT */
-    {1226, 80, 18}, /* SC */
-    {1229, 81, 18}, /* SCRIPTEXTENSIONS */
-    {1230, 81, 18}, /* SCX */
-    {1236, 82, 19}, /* SENTENCEBREAK */
-    {1225, 82, 19}, /* SB */
-    {1237, 83,  0}, /* SENTENCETERMINAL */
-    {1283, 83,  0}, /* STERM */
-    {1265, 84,  0}, /* SOFTDOTTED */
-    {1231, 84,  0}, /* SD */
-    {1358, 85,  0}, /* TERMINALPUNCTUATION */
-    {1357, 85,  0}, /* TERM */
-    {1399, 86,  0}, /* UNIFIEDIDEOGRAPH */
-    {1394, 86,  0}, /* UIDEO */
-    {1403, 87,  0}, /* UPPERCASE */
-    {1402, 87,  0}, /* UPPER */
-    {1408, 88,  0}, /* VARIATIONSELECTOR */
-    {1428, 88,  0}, /* VS */
-    {1417, 89,  0}, /* VERTSPACE */
-    {1405, 89,  0}, /* V */
-    {1437, 90,  0}, /* WHITESPACE */
-    {1445, 90,  0}, /* WSPACE */
-    {1274, 90,  0}, /* SPACE */
-    {1440, 91,  0}, /* WORD */
-    {1441, 92, 20}, /* WORDBREAK */
-    {1435, 92, 20}, /* WB */
-    {1446, 93,  0}, /* XDIGIT */
-    {1448, 94,  0}, /* XIDCONTINUE */
-    {1447, 94,  0}, /* XIDC */
-    {1450, 95,  0}, /* XIDSTART */
-    {1449, 95,  0}, /* XIDS */
+    { 195,  0,  0}, /* ALPHABETIC */
+    { 194,  0,  0}, /* ALPHA */
+    { 198,  1,  0}, /* ALPHANUMERIC */
+    { 193,  1,  0}, /* ALNUM */
+    { 206,  2,  0}, /* ANY */
+    { 233,  3,  0}, /* ASCIIHEXDIGIT */
+    { 179,  3,  0}, /* AHEX */
+    { 274,  4,  1}, /* BIDICLASS */
+    { 263,  4,  1}, /* BC */
+    { 275,  5,  0}, /* BIDICONTROL */
+    { 273,  5,  0}, /* BIDIC */
+    { 277,  6,  0}, /* BIDIMIRRORED */
+    { 276,  6,  0}, /* BIDIM */
+    { 281,  7,  0}, /* BLANK */
+    { 283,  8,  2}, /* BLOCK */
+    { 282,  8,  2}, /* BLK */
+    { 320,  9,  3}, /* CANONICALCOMBININGCLASS */
+    { 332,  9,  3}, /* CCC */
+    { 326, 10,  0}, /* CASED */
+    { 328, 11,  0}, /* CASEIGNORABLE */
+    { 385, 11,  0}, /* CI */
+    { 373, 12,  0}, /* CHANGESWHENCASEFOLDED */
+    { 476, 12,  0}, /* CWCF */
+    { 374, 13,  0}, /* CHANGESWHENCASEMAPPED */
+    { 477, 13,  0}, /* CWCM */
+    { 375, 14,  0}, /* CHANGESWHENLOWERCASED */
+    { 478, 14,  0}, /* CWL */
+    { 376, 15,  0}, /* CHANGESWHENTITLECASED */
+    { 479, 15,  0}, /* CWT */
+    { 377, 16,  0}, /* CHANGESWHENUPPERCASED */
+    { 480, 16,  0}, /* CWU */
+    { 501, 17,  0}, /* DASH */
+    { 507, 18,  4}, /* DECOMPOSITIONTYPE */
+    { 538, 18,  4}, /* DT */
+    { 508, 19,  0}, /* DEFAULTIGNORABLECODEPOINT */
+    { 518, 19,  0}, /* DI */
+    { 510, 20,  0}, /* DEPRECATED */
+    { 509, 20,  0}, /* DEP */
+    { 520, 21,  0}, /* DIACRITIC */
+    { 519, 21,  0}, /* DIA */
+    { 545, 22,  5}, /* EASTASIANWIDTH */
+    { 543, 22,  5}, /* EA */
+    { 561, 23,  0}, /* EMOJI */
+    { 562, 24,  0}, /* EMOJICOMPONENT */
+    { 550, 24,  0}, /* ECOMP */
+    { 563, 25,  0}, /* EMOJIMODIFIER */
+    { 559, 25,  0}, /* EMOD */
+    { 564, 26,  0}, /* EMOJIMODIFIERBASE */
+    { 547, 26,  0}, /* EBASE */
+    { 565, 27,  0}, /* EMOJIPRESENTATION */
+    { 578, 27,  0}, /* EPRES */
+    { 598, 28,  0}, /* EXTENDEDPICTOGRAPHIC */
+    { 601, 28,  0}, /* EXTPICT */
+    { 599, 29,  0}, /* EXTENDER */
+    { 596, 29,  0}, /* EXT */
+    { 625, 30,  6}, /* GENERALCATEGORY */
+    { 622, 30,  6}, /* GC */
+    { 649, 31,  0}, /* GRAPH */
+    { 650, 32,  0}, /* GRAPHEMEBASE */
+    { 654, 32,  0}, /* GRBASE */
+    { 651, 33,  7}, /* GRAPHEMECLUSTERBREAK */
+    { 623, 33,  7}, /* GCB */
+    { 652, 34,  0}, /* GRAPHEMEEXTEND */
+    { 660, 34,  0}, /* GREXT */
+    { 653, 35,  0}, /* GRAPHEMELINK */
+    { 661, 35,  0}, /* GRLINK */
+    { 684, 36,  8}, /* HANGULSYLLABLETYPE */
+    { 715, 36,  8}, /* HST */
+    { 703, 37,  0}, /* HEXDIGIT */
+    { 702, 37,  0}, /* HEX */
+    { 713, 38,  0}, /* HORIZSPACE */
+    { 667, 38,  0}, /* H */
+    { 718, 39,  0}, /* HYPHEN */
+    { 721, 40,  0}, /* IDCOMPATMATHCONTINUE */
+    { 722, 41,  0}, /* IDCOMPATMATHSTART */
+    { 723, 42,  0}, /* IDCONTINUE */
+    { 720, 42,  0}, /* IDC */
+    { 725, 43,  0}, /* IDEOGRAPHIC */
+    { 724, 43,  0}, /* IDEO */
+    { 731, 44,  0}, /* IDSBINARYOPERATOR */
+    { 730, 44,  0}, /* IDSB */
+    { 733, 45,  0}, /* IDSTART */
+    { 729, 45,  0}, /* IDS */
+    { 734, 46,  0}, /* IDSTRINARYOPERATOR */
+    { 732, 46,  0}, /* IDST */
+    { 736, 47,  0}, /* IDSUNARYOPERATOR */
+    { 735, 47,  0}, /* IDSU */
+    { 740, 48,  9}, /* INDICCONJUNCTBREAK */
+    { 739, 48,  9}, /* INCB */
+    { 742, 49, 10}, /* INDICPOSITIONALCATEGORY */
+    { 750, 49, 10}, /* INPC */
+    { 744, 50, 11}, /* INDICSYLLABICCATEGORY */
+    { 751, 50, 11}, /* INSC */
+    { 773, 51,  0}, /* JOINCONTROL */
+    { 771, 51,  0}, /* JOINC */
+    { 775, 52, 12}, /* JOININGGROUP */
+    { 769, 52, 12}, /* JG */
+    { 776, 53, 13}, /* JOININGTYPE */
+    { 777, 53, 13}, /* JT */
+    { 871, 54, 14}, /* LINEBREAK */
+    { 846, 54, 14}, /* LB */
+    { 882, 55,  0}, /* LOGICALORDEREXCEPTION */
+    { 881, 55,  0}, /* LOE */
+    { 884, 56,  0}, /* LOWERCASE */
+    { 883, 56,  0}, /* LOWER */
+    { 956, 57,  0}, /* MATH */
+    {1046, 58, 15}, /* NFCQUICKCHECK */
+    {1045, 58, 15}, /* NFCQC */
+    {1048, 59, 16}, /* NFDQUICKCHECK */
+    {1047, 59, 16}, /* NFDQC */
+    {1050, 60, 15}, /* NFKCQUICKCHECK */
+    {1049, 60, 15}, /* NFKCQC */
+    {1052, 61, 16}, /* NFKDQUICKCHECK */
+    {1051, 61, 16}, /* NFKDQC */
+    {1061, 62,  0}, /* NONCHARACTERCODEPOINT */
+    {1038, 62,  0}, /* NCHAR */
+    {1081, 63, 17}, /* NUMERICTYPE */
+    {1074, 63, 17}, /* NT */
+    {1082, 64, 18}, /* NUMERICVALUE */
+    {1085, 64, 18}, /* NV */
+    {1123, 65,  0}, /* OTHERALPHABETIC */
+    {1088, 65,  0}, /* OALPHA */
+    {1124, 66,  0}, /* OTHERDEFAULTIGNORABLECODEPOINT */
+    {1090, 66,  0}, /* ODI */
+    {1125, 67,  0}, /* OTHERGRAPHEMEEXTEND */
+    {1093, 67,  0}, /* OGREXT */
+    {1126, 68,  0}, /* OTHERIDCONTINUE */
+    {1094, 68,  0}, /* OIDC */
+    {1127, 69,  0}, /* OTHERIDSTART */
+    {1095, 69,  0}, /* OIDS */
+    {1129, 70,  0}, /* OTHERLOWERCASE */
+    {1108, 70,  0}, /* OLOWER */
+    {1130, 71,  0}, /* OTHERMATH */
+    {1109, 71,  0}, /* OMATH */
+    {1135, 72,  0}, /* OTHERUPPERCASE */
+    {1138, 72,  0}, /* OUPPER */
+    {1149, 73,  0}, /* PATTERNSYNTAX */
+    {1148, 73,  0}, /* PATSYN */
+    {1150, 74,  0}, /* PATTERNWHITESPACE */
+    {1151, 74,  0}, /* PATWS */
+    {1180, 75,  0}, /* POSIXALNUM */
+    {1181, 76,  0}, /* POSIXDIGIT */
+    {1182, 77,  0}, /* POSIXPUNCT */
+    {1183, 78,  0}, /* POSIXXDIGIT */
+    {1189, 79,  0}, /* PREPENDEDCONCATENATIONMARK */
+    {1155, 79,  0}, /* PCM */
+    {1190, 80,  0}, /* PRINT */
+    {1207, 81,  0}, /* QUOTATIONMARK */
+    {1204, 81,  0}, /* QMARK */
+    {1209, 82,  0}, /* RADICAL */
+    {1210, 83,  0}, /* REGIONALINDICATOR */
+    {1215, 83,  0}, /* RI */
+    {1245, 84, 19}, /* SCRIPT */
+    {1243, 84, 19}, /* SC */
+    {1246, 85, 19}, /* SCRIPTEXTENSIONS */
+    {1247, 85, 19}, /* SCX */
+    {1253, 86, 20}, /* SENTENCEBREAK */
+    {1242, 86, 20}, /* SB */
+    {1254, 87,  0}, /* SENTENCETERMINAL */
+    {1300, 87,  0}, /* STERM */
+    {1282, 88,  0}, /* SOFTDOTTED */
+    {1248, 88,  0}, /* SD */
+    {1375, 89,  0}, /* TERMINALPUNCTUATION */
+    {1374, 89,  0}, /* TERM */
+    {1416, 90,  0}, /* UNIFIEDIDEOGRAPH */
+    {1411, 90,  0}, /* UIDEO */
+    {1420, 91,  0}, /* UPPERCASE */
+    {1419, 91,  0}, /* UPPER */
+    {1425, 92,  0}, /* VARIATIONSELECTOR */
+    {1448, 92,  0}, /* VS */
+    {1434, 93,  0}, /* VERTSPACE */
+    {1422, 93,  0}, /* V */
+    {1457, 94,  0}, /* WHITESPACE */
+    {1465, 94,  0}, /* WSPACE */
+    {1291, 94,  0}, /* SPACE */
+    {1460, 95,  0}, /* WORD */
+    {1461, 96, 21}, /* WORDBREAK */
+    {1455, 96, 21}, /* WB */
+    {1466, 97,  0}, /* XDIGIT */
+    {1468, 98,  0}, /* XIDCONTINUE */
+    {1467, 98,  0}, /* XIDC */
+    {1470, 99,  0}, /* XIDSTART */
+    {1469, 99,  0}, /* XIDS */
 };
 
 /* Property values. */
 RE_PropertyValue re_property_values[] = {
-    {1040,  0,   0}, /* NO */
-    {1007,  0,   0}, /* N */
-    { 592,  0,   0}, /* F */
-    { 593,  0,   0}, /* FALSE */
-    {1458,  0,   1}, /* YES */
-    {1454,  0,   1}, /* Y */
-    {1326,  0,   1}, /* T */
-    {1387,  0,   1}, /* TRUE */
-    {1201,  1,   0}, /* RIGHTTOLEFT */
-    {1191,  1,   0}, /* R */
-    { 285,  1,   1}, /* BOUNDARYNEUTRAL */
-    { 277,  1,   1}, /* BN */
-    {1234,  1,   2}, /* SEGMENTSEPARATOR */
-    {1215,  1,   2}, /* S */
-    {1130,  1,   3}, /* PARAGRAPHSEPARATOR */
-    { 240,  1,   3}, /* B */
-    {1437,  1,   4}, /* WHITESPACE */
-    {1443,  1,   4}, /* WS */
-    {1114,  1,   5}, /* OTHERNEUTRAL */
-    {1093,  1,   5}, /* ON */
-    { 583,  1,   6}, /* EUROPEANTERMINATOR */
-    { 570,  1,   6}, /* ET */
-    { 582,  1,   7}, /* EUROPEANSEPARATOR */
-    { 569,  1,   7}, /* ES */
-    { 429,  1,   8}, /* COMMONSEPARATOR */
-    { 460,  1,   8}, /* CS */
-    { 581,  1,   9}, /* EUROPEANNUMBER */
-    { 557,  1,   9}, /* EN */
-    { 837,  1,  10}, /* LEFTTORIGHT */
-    { 802,  1,  10}, /* L */
-    {1048,  1,  11}, /* NONSPACINGMARK */
-    {1056,  1,  11}, /* NSM */
-    { 213,  1,  12}, /* ARABICNUMBER */
-    { 194,  1,  12}, /* AN */
-    { 210,  1,  13}, /* ARABICLETTER */
-    { 181,  1,  13}, /* AL */
-    { 838,  1,  14}, /* LEFTTORIGHTEMBEDDING */
-    { 870,  1,  14}, /* LRE */
-    {1202,  1,  15}, /* RIGHTTOLEFTEMBEDDING */
-    {1206,  1,  15}, /* RLE */
-    {1161,  1,  16}, /* POPDIRECTIONALFORMAT */
-    {1140,  1,  16}, /* PDF */
-    { 840,  1,  17}, /* LEFTTORIGHTOVERRIDE */
-    { 872,  1,  17}, /* LRO */
-    {1204,  1,  18}, /* RIGHTTOLEFTOVERRIDE */
-    {1208,  1,  18}, /* RLO */
-    { 839,  1,  19}, /* LEFTTORIGHTISOLATE */
-    { 871,  1,  19}, /* LRI */
-    {1203,  1,  20}, /* RIGHTTOLEFTISOLATE */
-    {1207,  1,  20}, /* RLI */
-    { 601,  1,  21}, /* FIRSTSTRONGISOLATE */
-    { 607,  1,  21}, /* FSI */
-    {1162,  1,  22}, /* POPDIRECTIONALISOLATE */
-    {1141,  1,  22}, /* PDI */
-    {1041,  2,   0}, /* NOBLOCK */
-    {1019,  2,   0}, /* NB */
-    { 249,  2,   1}, /* BASICLATIN */
-    { 224,  2,   1}, /* ASCII */
-    { 812,  2,   2}, /* LATIN1SUPPLEMENT */
-    { 811,  2,   2}, /* LATIN1SUP */
-    { 810,  2,   2}, /* LATIN1 */
-    { 819,  2,   3}, /* LATINEXTENDEDA */
-    { 813,  2,   3}, /* LATINEXTA */
-    { 821,  2,   4}, /* LATINEXTENDEDB */
-    { 815,  2,   4}, /* LATINEXTB */
-    { 743,  2,   5}, /* IPAEXTENSIONS */
-    { 742,  2,   5}, /* IPAEXT */
-    {1277,  2,   6}, /* SPACINGMODIFIERLETTERS */
-    { 986,  2,   6}, /* MODIFIERLETTERS */
-    { 420,  2,   7}, /* COMBININGDIACRITICALMARKS */
-    { 511,  2,   7}, /* DIACRITICALS */
-    { 646,  2,   8}, /* GREEKANDCOPTIC */
-    { 645,  2,   8}, /* GREEK */
-    { 474,  2,   9}, /* CYRILLIC */
-    { 484,  2,  10}, /* CYRILLICSUPPLEMENT */
-    { 483,  2,  10}, /* CYRILLICSUP */
-    { 485,  2,  10}, /* CYRILLICSUPPLEMENTARY */
-    { 220,  2,  11}, /* ARMENIAN */
-    { 687,  2,  12}, /* HEBREW */
-    { 203,  2,  13}, /* ARABIC */
-    {1322,  2,  14}, /* SYRIAC */
-    { 219,  2,  15}, /* ARABICSUPPLEMENT */
-    { 218,  2,  15}, /* ARABICSUP */
-    {1363,  2,  16}, /* THAANA */
-    {1037,  2,  17}, /* NKO */
-    {1220,  2,  18}, /* SAMARITAN */
-    { 904,  2,  19}, /* MANDAIC */
-    {1324,  2,  20}, /* SYRIACSUPPLEMENT */
-    {1323,  2,  20}, /* SYRIACSUP */
-    { 208,  2,  21}, /* ARABICEXTENDEDB */
-    { 205,  2,  21}, /* ARABICEXTB */
-    { 207,  2,  22}, /* ARABICEXTENDEDA */
-    { 204,  2,  22}, /* ARABICEXTA */
-    { 503,  2,  23}, /* DEVANAGARI */
-    { 261,  2,  24}, /* BENGALI */
-    { 655,  2,  25}, /* GURMUKHI */
-    { 652,  2,  26}, /* GUJARATI */
-    {1097,  2,  27}, /* ORIYA */
-    {1341,  2,  28}, /* TAMIL */
-    {1356,  2,  29}, /* TELUGU */
-    { 779,  2,  30}, /* KANNADA */
-    { 891,  2,  31}, /* MALAYALAM */
-    {1254,  2,  32}, /* SINHALA */
-    {1364,  2,  33}, /* THAI */
-    { 807,  2,  34}, /* LAO */
-    {1366,  2,  35}, /* TIBETAN */
-    {1001,  2,  36}, /* MYANMAR */
-    { 621,  2,  37}, /* GEORGIAN */
-    { 670,  2,  38}, /* HANGULJAMO */
-    { 748,  2,  38}, /* JAMO */
-    { 572,  2,  39}, /* ETHIOPIC */
-    { 580,  2,  40}, /* ETHIOPICSUPPLEMENT */
-    { 579,  2,  40}, /* ETHIOPICSUP */
-    { 371,  2,  41}, /* CHEROKEE */
-    {1396,  2,  42}, /* UNIFIEDCANADIANABORIGINALSYLLABICS */
-    {1389,  2,  42}, /* UCAS */
-    { 310,  2,  42}, /* CANADIANSYLLABICS */
-    {1075,  2,  43}, /* OGHAM */
-    {1213,  2,  44}, /* RUNIC */
-    {1327,  2,  45}, /* TAGALOG */
-    { 682,  2,  46}, /* HANUNOO */
-    { 301,  2,  47}, /* BUHID */
-    {1329,  2,  48}, /* TAGBANWA */
-    { 791,  2,  49}, /* KHMER */
-    { 991,  2,  50}, /* MONGOLIAN */
-    {1397,  2,  51}, /* UNIFIEDCANADIANABORIGINALSYLLABICSEXTENDED */
-    {1390,  2,  51}, /* UCASEXT */
-    { 848,  2,  52}, /* LIMBU */
-    {1332,  2,  53}, /* TAILE */
-    {1026,  2,  54}, /* NEWTAILUE */
-    { 792,  2,  55}, /* KHMERSYMBOLS */
-    { 299,  2,  56}, /* BUGINESE */
-    {1333,  2,  57}, /* TAITHAM */
-    { 421,  2,  58}, /* COMBININGDIACRITICALMARKSEXTENDED */
-    { 512,  2,  58}, /* DIACRITICALSEXT */
-    { 244,  2,  59}, /* BALINESE */
-    {1287,  2,  60}, /* SUNDANESE */
-    { 252,  2,  61}, /* BATAK */
-    { 842,  2,  62}, /* LEPCHA */
-    {1079,  2,  63}, /* OLCHIKI */
-    { 481,  2,  64}, /* CYRILLICEXTENDEDC */
-    { 477,  2,  64}, /* CYRILLICEXTC */
-    { 623,  2,  65}, /* GEORGIANEXTENDED */
-    { 622,  2,  65}, /* GEORGIANEXT */
-    {1289,  2,  66}, /* SUNDANESESUPPLEMENT */
-    {1288,  2,  66}, /* SUNDANESESUP */
-    {1412,  2,  67}, /* VEDICEXTENSIONS */
-    {1411,  2,  67}, /* VEDICEXT */
-    {1154,  2,  68}, /* PHONETICEXTENSIONS */
-    {1153,  2,  68}, /* PHONETICEXT */
-    {1155,  2,  69}, /* PHONETICEXTENSIONSSUPPLEMENT */
-    {1156,  2,  69}, /* PHONETICEXTSUP */
-    { 423,  2,  70}, /* COMBININGDIACRITICALMARKSSUPPLEMENT */
-    { 514,  2,  70}, /* DIACRITICALSSUP */
-    { 820,  2,  71}, /* LATINEXTENDEDADDITIONAL */
-    { 814,  2,  71}, /* LATINEXTADDITIONAL */
-    { 648,  2,  72}, /* GREEKEXTENDED */
-    { 647,  2,  72}, /* GREEKEXT */
-    { 616,  2,  73}, /* GENERALPUNCTUATION */
-    {1181,  2,  73}, /* PUNCTUATION */
-    {1296,  2,  74}, /* SUPERSCRIPTSANDSUBSCRIPTS */
-    {1295,  2,  74}, /* SUPERANDSUB */
-    { 465,  2,  75}, /* CURRENCYSYMBOLS */
-    { 422,  2,  76}, /* COMBININGDIACRITICALMARKSFORSYMBOLS */
-    { 513,  2,  76}, /* DIACRITICALSFORSYMBOLS */
-    { 426,  2,  76}, /* COMBININGMARKSFORSYMBOLS */
-    { 844,  2,  77}, /* LETTERLIKESYMBOLS */
-    {1061,  2,  78}, /* NUMBERFORMS */
-    { 223,  2,  79}, /* ARROWS */
-    { 942,  2,  80}, /* MATHEMATICALOPERATORS */
-    { 943,  2,  80}, /* MATHOPERATORS */
-    { 975,  2,  81}, /* MISCELLANEOUSTECHNICAL */
-    { 980,  2,  81}, /* MISCTECHNICAL */
-    { 450,  2,  82}, /* CONTROLPICTURES */
-    {1096,  2,  83}, /* OPTICALCHARACTERRECOGNITION */
-    {1072,  2,  83}, /* OCR */
-    { 560,  2,  84}, /* ENCLOSEDALPHANUMERICS */
-    { 559,  2,  84}, /* ENCLOSEDALPHANUM */
-    { 286,  2,  85}, /* BOXDRAWING */
-    { 276,  2,  86}, /* BLOCKELEMENTS */
-    { 617,  2,  87}, /* GEOMETRICSHAPES */
-    { 972,  2,  88}, /* MISCELLANEOUSSYMBOLS */
-    { 979,  2,  88}, /* MISCSYMBOLS */
-    { 517,  2,  89}, /* DINGBATS */
-    { 970,  2,  90}, /* MISCELLANEOUSMATHEMATICALSYMBOLSA */
-    { 976,  2,  90}, /* MISCMATHSYMBOLSA */
-    {1298,  2,  91}, /* SUPPLEMENTALARROWSA */
-    {1291,  2,  91}, /* SUPARROWSA */
-    { 293,  2,  92}, /* BRAILLEPATTERNS */
-    { 292,  2,  92}, /* BRAILLE */
-    {1299,  2,  93}, /* SUPPLEMENTALARROWSB */
-    {1292,  2,  93}, /* SUPARROWSB */
-    { 971,  2,  94}, /* MISCELLANEOUSMATHEMATICALSYMBOLSB */
-    { 977,  2,  94}, /* MISCMATHSYMBOLSB */
-    {1301,  2,  95}, /* SUPPLEMENTALMATHEMATICALOPERATORS */
-    {1297,  2,  95}, /* SUPMATHOPERATORS */
-    { 973,  2,  96}, /* MISCELLANEOUSSYMBOLSANDARROWS */
-    { 969,  2,  96}, /* MISCARROWS */
-    { 628,  2,  97}, /* GLAGOLITIC */
-    { 822,  2,  98}, /* LATINEXTENDEDC */
-    { 816,  2,  98}, /* LATINEXTC */
-    { 452,  2,  99}, /* COPTIC */
-    { 625,  2, 100}, /* GEORGIANSUPPLEMENT */
-    { 624,  2, 100}, /* GEORGIANSUP */
-    {1368,  2, 101}, /* TIFINAGH */
-    { 576,  2, 102}, /* ETHIOPICEXTENDED */
-    { 573,  2, 102}, /* ETHIOPICEXT */
-    { 479,  2, 103}, /* CYRILLICEXTENDEDA */
-    { 475,  2, 103}, /* CYRILLICEXTA */
-    {1302,  2, 104}, /* SUPPLEMENTALPUNCTUATION */
-    {1308,  2, 104}, /* SUPPUNCTUATION */
-    { 398,  2, 105}, /* CJKRADICALSSUPPLEMENT */
-    { 397,  2, 105}, /* CJKRADICALSSUP */
-    { 778,  2, 106}, /* KANGXIRADICALS */
-    { 777,  2, 106}, /* KANGXI */
-    { 714,  2, 107}, /* IDEOGRAPHICDESCRIPTIONCHARACTERS */
-    { 710,  2, 107}, /* IDC */
-    { 401,  2, 108}, /* CJKSYMBOLSANDPUNCTUATION */
-    { 400,  2, 108}, /* CJKSYMBOLS */
-    { 698,  2, 109}, /* HIRAGANA */
-    { 781,  2, 110}, /* KATAKANA */
-    { 279,  2, 111}, /* BOPOMOFO */
-    { 669,  2, 112}, /* HANGULCOMPATIBILITYJAMO */
-    { 431,  2, 112}, /* COMPATJAMO */
-    { 776,  2, 113}, /* KANBUN */
-    { 281,  2, 114}, /* BOPOMOFOEXTENDED */
-    { 280,  2, 114}, /* BOPOMOFOEXT */
-    { 399,  2, 115}, /* CJKSTROKES */
-    { 784,  2, 116}, /* KATAKANAPHONETICEXTENSIONS */
-    { 782,  2, 116}, /* KATAKANAEXT */
-    { 564,  2, 117}, /* ENCLOSEDCJKLETTERSANDMONTHS */
-    { 563,  2, 117}, /* ENCLOSEDCJK */
-    { 383,  2, 118}, /* CJKCOMPATIBILITY */
-    { 381,  2, 118}, /* CJKCOMPAT */
-    { 403,  2, 119}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONA */
-    { 389,  2, 119}, /* CJKEXTA */
-    {1464,  2, 120}, /* YIJINGHEXAGRAMSYMBOLS */
-    {1463,  2, 120}, /* YIJING */
-    { 402,  2, 121}, /* CJKUNIFIEDIDEOGRAPHS */
-    { 380,  2, 121}, /* CJK */
-    {1466,  2, 122}, /* YISYLLABLES */
-    {1465,  2, 123}, /* YIRADICALS */
-    { 858,  2, 124}, /* LISU */
-    {1406,  2, 125}, /* VAI */
-    { 480,  2, 126}, /* CYRILLICEXTENDEDB */
-    { 476,  2, 126}, /* CYRILLICEXTB */
-    { 246,  2, 127}, /* BAMUM */
-    { 988,  2, 128}, /* MODIFIERTONELETTERS */
-    { 823,  2, 129}, /* LATINEXTENDEDD */
-    { 817,  2, 129}, /* LATINEXTD */
-    {1316,  2, 130}, /* SYLOTINAGRI */
-    { 428,  2, 131}, /* COMMONINDICNUMBERFORMS */
-    { 725,  2, 131}, /* INDICNUMBERFORMS */
-    {1146,  2, 132}, /* PHAGSPA */
-    {1224,  2, 133}, /* SAURASHTRA */
-    { 506,  2, 134}, /* DEVANAGARIEXTENDED */
-    { 504,  2, 134}, /* DEVANAGARIEXT */
-    { 786,  2, 135}, /* KAYAHLI */
-    {1196,  2, 136}, /* REJANG */
-    { 671,  2, 137}, /* HANGULJAMOEXTENDEDA */
-    { 749,  2, 137}, /* JAMOEXTA */
-    { 752,  2, 138}, /* JAVANESE */
-    {1005,  2, 139}, /* MYANMAREXTENDEDB */
-    {1003,  2, 139}, /* MYANMAREXTB */
-    { 364,  2, 140}, /* CHAM */
-    {1004,  2, 141}, /* MYANMAREXTENDEDA */
-    {1002,  2, 141}, /* MYANMAREXTA */
-    {1334,  2, 142}, /* TAIVIET */
-    { 957,  2, 143}, /* MEETEIMAYEKEXTENSIONS */
-    { 956,  2, 143}, /* MEETEIMAYEKEXT */
-    { 577,  2, 144}, /* ETHIOPICEXTENDEDA */
-    { 574,  2, 144}, /* ETHIOPICEXTA */
-    { 824,  2, 145}, /* LATINEXTENDEDE */
-    { 818,  2, 145}, /* LATINEXTE */
-    { 373,  2, 146}, /* CHEROKEESUPPLEMENT */
-    { 372,  2, 146}, /* CHEROKEESUP */
-    { 955,  2, 147}, /* MEETEIMAYEK */
-    { 673,  2, 148}, /* HANGULSYLLABLES */
-    { 668,  2, 148}, /* HANGUL */
-    { 672,  2, 149}, /* HANGULJAMOEXTENDEDB */
-    { 750,  2, 149}, /* JAMOEXTB */
-    { 696,  2, 150}, /* HIGHSURROGATES */
-    { 694,  2, 151}, /* HIGHPRIVATEUSESURROGATES */
-    { 695,  2, 151}, /* HIGHPUSURROGATES */
-    { 869,  2, 152}, /* LOWSURROGATES */
-    {1175,  2, 153}, /* PRIVATEUSEAREA */
-    {1179,  2, 153}, /* PUA */
-    {1174,  2, 153}, /* PRIVATEUSE */
-    { 385,  2, 154}, /* CJKCOMPATIBILITYIDEOGRAPHS */
-    { 387,  2, 154}, /* CJKCOMPATIDEOGRAPHS */
-    { 191,  2, 155}, /* ALPHABETICPRESENTATIONFORMS */
-    { 190,  2, 155}, /* ALPHABETICPF */
-    { 216,  2, 156}, /* ARABICPRESENTATIONFORMSA */
-    { 214,  2, 156}, /* ARABICPFA */
-    {1409,  2, 157}, /* VARIATIONSELECTORS */
-    {1428,  2, 157}, /* VS */
-    {1415,  2, 158}, /* VERTICALFORMS */
-    { 424,  2, 159}, /* COMBININGHALFMARKS */
-    { 662,  2, 159}, /* HALFMARKS */
-    { 384,  2, 160}, /* CJKCOMPATIBILITYFORMS */
-    { 382,  2, 160}, /* CJKCOMPATFORMS */
-    {1260,  2, 161}, /* SMALLFORMVARIANTS */
-    {1259,  2, 161}, /* SMALLFORMS */
-    { 217,  2, 162}, /* ARABICPRESENTATIONFORMSB */
-    { 215,  2, 162}, /* ARABICPFB */
-    { 664,  2, 163}, /* HALFWIDTHANDFULLWIDTHFORMS */
-    { 661,  2, 163}, /* HALFANDFULLFORMS */
-    {1278,  2, 164}, /* SPECIALS */
-    { 854,  2, 165}, /* LINEARBSYLLABARY */
-    { 853,  2, 166}, /* LINEARBIDEOGRAMS */
-    { 172,  2, 167}, /* AEGEANNUMBERS */
-    { 198,  2, 168}, /* ANCIENTGREEKNUMBERS */
-    { 199,  2, 169}, /* ANCIENTSYMBOLS */
-    {1148,  2, 170}, /* PHAISTOSDISC */
-    {1147,  2, 170}, /* PHAISTOS */
-    { 880,  2, 171}, /* LYCIAN */
-    { 316,  2, 172}, /* CARIAN */
-    { 453,  2, 173}, /* COPTICEPACTNUMBERS */
-    {1082,  2, 174}, /* OLDITALIC */
-    { 636,  2, 175}, /* GOTHIC */
-    {1084,  2, 176}, /* OLDPERMIC */
-    {1393,  2, 177}, /* UGARITIC */
-    {1085,  2, 178}, /* OLDPERSIAN */
-    { 501,  2, 179}, /* DESERET */
-    {1243,  2, 180}, /* SHAVIAN */
-    {1104,  2, 181}, /* OSMANYA */
-    {1101,  2, 182}, /* OSAGE */
-    { 545,  2, 183}, /* ELBASAN */
-    { 321,  2, 184}, /* CAUCASIANALBANIAN */
-    {1422,  2, 185}, /* VITHKUQI */
-    { 851,  2, 186}, /* LINEARA */
-    { 825,  2, 187}, /* LATINEXTENDEDF */
-    { 827,  2, 187}, /* LATINEXTF */
-    { 472,  2, 188}, /* CYPRIOTSYLLABARY */
-    { 723,  2, 189}, /* IMPERIALARAMAIC */
-    {1129,  2, 190}, /* PALMYRENE */
-    {1010,  2, 191}, /* NABATAEAN */
-    { 684,  2, 192}, /* HATRAN */
-    {1152,  2, 193}, /* PHOENICIAN */
-    { 882,  2, 194}, /* LYDIAN */
-    { 963,  2, 195}, /* MEROITICHIEROGLYPHS */
-    { 962,  2, 196}, /* MEROITICCURSIVE */
-    { 789,  2, 197}, /* KHAROSHTHI */
-    {1087,  2, 198}, /* OLDSOUTHARABIAN */
-    {1083,  2, 199}, /* OLDNORTHARABIAN */
-    { 907,  2, 200}, /* MANICHAEAN */
-    { 238,  2, 201}, /* AVESTAN */
-    { 737,  2, 202}, /* INSCRIPTIONALPARTHIAN */
-    { 736,  2, 203}, /* INSCRIPTIONALPAHLAVI */
-    {1178,  2, 204}, /* PSALTERPAHLAVI */
-    {1088,  2, 205}, /* OLDTURKIC */
-    {1081,  2, 206}, /* OLDHUNGARIAN */
-    { 676,  2, 207}, /* HANIFIROHINGYA */
-    {1212,  2, 208}, /* RUMINUMERALSYMBOLS */
-    {1211,  2, 208}, /* RUMI */
-    {1460,  2, 209}, /* YEZIDI */
-    { 209,  2, 210}, /* ARABICEXTENDEDC */
-    { 206,  2, 210}, /* ARABICEXTC */
-    {1086,  2, 211}, /* OLDSOGDIAN */
-    {1267,  2, 212}, /* SOGDIAN */
-    {1089,  2, 213}, /* OLDUYGHUR */
-    { 375,  2, 214}, /* CHORASMIAN */
-    { 547,  2, 215}, /* ELYMAIC */
-    { 289,  2, 216}, /* BRAHMI */
-    { 765,  2, 217}, /* KAITHI */
-    {1270,  2, 218}, /* SORASOMPENG */
-    { 363,  2, 219}, /* CHAKMA */
-    { 885,  2, 220}, /* MAHAJANI */
-    {1242,  2, 221}, /* SHARADA */
-    {1255,  2, 222}, /* SINHALAARCHAICNUMBERS */
-    { 795,  2, 223}, /* KHOJKI */
-    { 998,  2, 224}, /* MULTANI */
-    { 796,  2, 225}, /* KHUDAWADI */
-    { 638,  2, 226}, /* GRANTHA */
-    {1024,  2, 227}, /* NEWA */
-    {1370,  2, 228}, /* TIRHUTA */
-    {1249,  2, 229}, /* SIDDHAM */
-    { 984,  2, 230}, /* MODI */
-    { 993,  2, 231}, /* MONGOLIANSUPPLEMENT */
-    { 992,  2, 231}, /* MONGOLIANSUP */
-    {1338,  2, 232}, /* TAKRI */
-    { 178,  2, 233}, /* AHOM */
-    { 520,  2, 234}, /* DOGRA */
-    {1433,  2, 235}, /* WARANGCITI */
-    { 518,  2, 236}, /* DIVESAKURU */
-    {1015,  2, 237}, /* NANDINAGARI */
-    {1472,  2, 238}, /* ZANABAZARSQUARE */
-    {1272,  2, 239}, /* SOYOMBO */
-    {1398,  2, 240}, /* UNIFIEDCANADIANABORIGINALSYLLABICSEXTENDEDA */
-    {1391,  2, 240}, /* UCASEXTA */
-    {1136,  2, 241}, /* PAUCINHAU */
-    { 507,  2, 242}, /* DEVANAGARIEXTENDEDA */
-    { 505,  2, 242}, /* DEVANAGARIEXTA */
-    { 263,  2, 243}, /* BHAIKSUKI */
-    { 936,  2, 244}, /* MARCHEN */
-    { 938,  2, 245}, /* MASARAMGONDI */
-    { 654,  2, 246}, /* GUNJALAGONDI */
-    { 890,  2, 247}, /* MAKASAR */
-    { 785,  2, 248}, /* KAWI */
-    { 860,  2, 249}, /* LISUSUPPLEMENT */
-    { 859,  2, 249}, /* LISUSUP */
-    {1343,  2, 250}, /* TAMILSUPPLEMENT */
-    {1342,  2, 250}, /* TAMILSUP */
-    { 461,  2, 251}, /* CUNEIFORM */
-    { 463,  2, 252}, /* CUNEIFORMNUMBERSANDPUNCTUATION */
-    { 462,  2, 252}, /* CUNEIFORMNUMBERS */
-    { 534,  2, 253}, /* EARLYDYNASTICCUNEIFORM */
-    { 473,  2, 254}, /* CYPROMINOAN */
-    { 543,  2, 255}, /* EGYPTIANHIEROGLYPHS */
-    { 542,  2, 256}, /* EGYPTIANHIEROGLYPHFORMATCONTROLS */
-    { 195,  2, 257}, /* ANATOLIANHIEROGLYPHS */
-    { 248,  2, 258}, /* BAMUMSUPPLEMENT */
-    { 247,  2, 258}, /* BAMUMSUP */
-    { 994,  2, 259}, /* MRO */
-    {1346,  2, 260}, /* TANGSA */
-    { 251,  2, 261}, /* BASSAVAH */
-    {1127,  2, 262}, /* PAHAWHHMONG */
-    { 951,  2, 263}, /* MEDEFAIDRIN */
-    { 964,  2, 264}, /* MIAO */
-    { 716,  2, 265}, /* IDEOGRAPHICSYMBOLSANDPUNCTUATION */
-    { 715,  2, 265}, /* IDEOGRAPHICSYMBOLS */
-    {1347,  2, 266}, /* TANGUT */
-    {1348,  2, 267}, /* TANGUTCOMPONENTS */
-    { 790,  2, 268}, /* KHITANSMALLSCRIPT */
-    {1350,  2, 269}, /* TANGUTSUPPLEMENT */
-    {1349,  2, 269}, /* TANGUTSUP */
-    { 772,  2, 270}, /* KANAEXTENDEDB */
-    { 770,  2, 270}, /* KANAEXTB */
-    { 774,  2, 271}, /* KANASUPPLEMENT */
-    { 773,  2, 271}, /* KANASUP */
-    { 771,  2, 272}, /* KANAEXTENDEDA */
-    { 769,  2, 272}, /* KANAEXTA */
-    {1262,  2, 273}, /* SMALLKANAEXTENSION */
-    {1261,  2, 273}, /* SMALLKANAEXT */
-    {1067,  2, 274}, /* NUSHU */
-    { 531,  2, 275}, /* DUPLOYAN */
-    {1246,  2, 276}, /* SHORTHANDFORMATCONTROLS */
-    {1478,  2, 277}, /* ZNAMENNYMUSICALNOTATION */
-    {1477,  2, 277}, /* ZNAMENNYMUSIC */
-    { 304,  2, 278}, /* BYZANTINEMUSICALSYMBOLS */
-    { 303,  2, 278}, /* BYZANTINEMUSIC */
-    {1000,  2, 279}, /* MUSICALSYMBOLS */
-    { 999,  2, 279}, /* MUSIC */
-    { 197,  2, 280}, /* ANCIENTGREEKMUSICALNOTATION */
-    { 196,  2, 280}, /* ANCIENTGREEKMUSIC */
-    { 766,  2, 281}, /* KAKTOVIKNUMERALS */
-    { 945,  2, 282}, /* MAYANNUMERALS */
-    {1336,  2, 283}, /* TAIXUANJINGSYMBOLS */
-    {1335,  2, 283}, /* TAIXUANJING */
-    { 455,  2, 284}, /* COUNTINGRODNUMERALS */
-    { 454,  2, 284}, /* COUNTINGROD */
-    { 941,  2, 285}, /* MATHEMATICALALPHANUMERICSYMBOLS */
-    { 940,  2, 285}, /* MATHALPHANUM */
-    {1311,  2, 286}, /* SUTTONSIGNWRITING */
-    { 826,  2, 287}, /* LATINEXTENDEDG */
-    { 828,  2, 287}, /* LATINEXTG */
-    { 630,  2, 288}, /* GLAGOLITICSUPPLEMENT */
-    { 629,  2, 288}, /* GLAGOLITICSUP */
-    { 482,  2, 289}, /* CYRILLICEXTENDEDD */
-    { 478,  2, 289}, /* CYRILLICEXTD */
-    {1070,  2, 290}, /* NYIAKENGPUACHUEHMONG */
-    {1382,  2, 291}, /* TOTO */
-    {1431,  2, 292}, /* WANCHO */
-    {1012,  2, 293}, /* NAGMUNDARI */
-    { 578,  2, 294}, /* ETHIOPICEXTENDEDB */
-    { 575,  2, 294}, /* ETHIOPICEXTB */
-    { 959,  2, 295}, /* MENDEKIKAKUI */
-    { 170,  2, 296}, /* ADLAM */
-    { 727,  2, 297}, /* INDICSIYAQNUMBERS */
-    {1119,  2, 298}, /* OTTOMANSIYAQNUMBERS */
-    { 212,  2, 299}, /* ARABICMATHEMATICALALPHABETICSYMBOLS */
-    { 211,  2, 299}, /* ARABICMATH */
-    { 888,  2, 300}, /* MAHJONGTILES */
-    { 887,  2, 300}, /* MAHJONG */
-    { 522,  2, 301}, /* DOMINOTILES */
-    { 521,  2, 301}, /* DOMINO */
-    {1158,  2, 302}, /* PLAYINGCARDS */
-    { 561,  2, 303}, /* ENCLOSEDALPHANUMERICSUPPLEMENT */
-    { 562,  2, 303}, /* ENCLOSEDALPHANUMSUP */
-    { 566,  2, 304}, /* ENCLOSEDIDEOGRAPHICSUPPLEMENT */
-    { 565,  2, 304}, /* ENCLOSEDIDEOGRAPHICSUP */
-    { 974,  2, 305}, /* MISCELLANEOUSSYMBOLSANDPICTOGRAPHS */
-    { 978,  2, 305}, /* MISCPICTOGRAPHS */
-    { 556,  2, 306}, /* EMOTICONS */
-    {1099,  2, 307}, /* ORNAMENTALDINGBATS */
-    {1386,  2, 308}, /* TRANSPORTANDMAPSYMBOLS */
-    {1385,  2, 308}, /* TRANSPORTANDMAP */
-    { 184,  2, 309}, /* ALCHEMICALSYMBOLS */
-    { 183,  2, 309}, /* ALCHEMICAL */
-    { 619,  2, 310}, /* GEOMETRICSHAPESEXTENDED */
-    { 618,  2, 310}, /* GEOMETRICSHAPESEXT */
-    {1300,  2, 311}, /* SUPPLEMENTALARROWSC */
-    {1293,  2, 311}, /* SUPARROWSC */
-    {1303,  2, 312}, /* SUPPLEMENTALSYMBOLSANDPICTOGRAPHS */
-    {1309,  2, 312}, /* SUPSYMBOLSANDPICTOGRAPHS */
-    { 374,  2, 313}, /* CHESSSYMBOLS */
-    {1319,  2, 314}, /* SYMBOLSANDPICTOGRAPHSEXTENDEDA */
-    {1318,  2, 314}, /* SYMBOLSANDPICTOGRAPHSEXTA */
-    {1320,  2, 315}, /* SYMBOLSFORLEGACYCOMPUTING */
-    { 404,  2, 316}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONB */
-    { 390,  2, 316}, /* CJKEXTB */
-    { 405,  2, 317}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONC */
-    { 391,  2, 317}, /* CJKEXTC */
-    { 406,  2, 318}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIOND */
-    { 392,  2, 318}, /* CJKEXTD */
-    { 407,  2, 319}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONE */
-    { 393,  2, 319}, /* CJKEXTE */
-    { 408,  2, 320}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONF */
-    { 394,  2, 320}, /* CJKEXTF */
-    { 386,  2, 321}, /* CJKCOMPATIBILITYIDEOGRAPHSSUPPLEMENT */
-    { 388,  2, 321}, /* CJKCOMPATIDEOGRAPHSSUP */
-    { 409,  2, 322}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONG */
-    { 395,  2, 322}, /* CJKEXTG */
-    { 410,  2, 323}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONH */
-    { 396,  2, 323}, /* CJKEXTH */
-    {1330,  2, 324}, /* TAGS */
-    {1410,  2, 325}, /* VARIATIONSELECTORSSUPPLEMENT */
-    {1429,  2, 325}, /* VSSUP */
-    {1304,  2, 326}, /* SUPPLEMENTARYPRIVATEUSEAREAA */
-    {1306,  2, 326}, /* SUPPUAA */
-    {1305,  2, 327}, /* SUPPLEMENTARYPRIVATEUSEAREAB */
-    {1307,  2, 327}, /* SUPPUAB */
-    {1052,  3,   0}, /* NOTREORDERED */
+    {1057,  0,   0}, /* NO */
+    {1024,  0,   0}, /* N */
+    { 602,  0,   0}, /* F */
+    { 603,  0,   0}, /* FALSE */
+    {1478,  0,   1}, /* YES */
+    {1474,  0,   1}, /* Y */
+    {1343,  0,   1}, /* T */
+    {1404,  0,   1}, /* TRUE */
+    {1218,  1,   0}, /* RIGHTTOLEFT */
+    {1208,  1,   0}, /* R */
+    { 293,  1,   1}, /* BOUNDARYNEUTRAL */
+    { 285,  1,   1}, /* BN */
+    {1251,  1,   2}, /* SEGMENTSEPARATOR */
+    {1232,  1,   2}, /* S */
+    {1147,  1,   3}, /* PARAGRAPHSEPARATOR */
+    { 248,  1,   3}, /* B */
+    {1457,  1,   4}, /* WHITESPACE */
+    {1463,  1,   4}, /* WS */
+    {1131,  1,   5}, /* OTHERNEUTRAL */
+    {1110,  1,   5}, /* ON */
+    { 593,  1,   6}, /* EUROPEANTERMINATOR */
+    { 580,  1,   6}, /* ET */
+    { 592,  1,   7}, /* EUROPEANSEPARATOR */
+    { 579,  1,   7}, /* ES */
+    { 439,  1,   8}, /* COMMONSEPARATOR */
+    { 470,  1,   8}, /* CS */
+    { 591,  1,   9}, /* EUROPEANNUMBER */
+    { 567,  1,   9}, /* EN */
+    { 853,  1,  10}, /* LEFTTORIGHT */
+    { 818,  1,  10}, /* L */
+    {1065,  1,  11}, /* NONSPACINGMARK */
+    {1073,  1,  11}, /* NSM */
+    { 220,  1,  12}, /* ARABICNUMBER */
+    { 200,  1,  12}, /* AN */
+    { 217,  1,  13}, /* ARABICLETTER */
+    { 187,  1,  13}, /* AL */
+    { 854,  1,  14}, /* LEFTTORIGHTEMBEDDING */
+    { 887,  1,  14}, /* LRE */
+    {1219,  1,  15}, /* RIGHTTOLEFTEMBEDDING */
+    {1223,  1,  15}, /* RLE */
+    {1178,  1,  16}, /* POPDIRECTIONALFORMAT */
+    {1157,  1,  16}, /* PDF */
+    { 856,  1,  17}, /* LEFTTORIGHTOVERRIDE */
+    { 889,  1,  17}, /* LRO */
+    {1221,  1,  18}, /* RIGHTTOLEFTOVERRIDE */
+    {1225,  1,  18}, /* RLO */
+    { 855,  1,  19}, /* LEFTTORIGHTISOLATE */
+    { 888,  1,  19}, /* LRI */
+    {1220,  1,  20}, /* RIGHTTOLEFTISOLATE */
+    {1224,  1,  20}, /* RLI */
+    { 611,  1,  21}, /* FIRSTSTRONGISOLATE */
+    { 617,  1,  21}, /* FSI */
+    {1179,  1,  22}, /* POPDIRECTIONALISOLATE */
+    {1158,  1,  22}, /* PDI */
+    {1058,  2,   0}, /* NOBLOCK */
+    {1036,  2,   0}, /* NB */
+    { 257,  2,   1}, /* BASICLATIN */
+    { 232,  2,   1}, /* ASCII */
+    { 828,  2,   2}, /* LATIN1SUPPLEMENT */
+    { 827,  2,   2}, /* LATIN1SUP */
+    { 826,  2,   2}, /* LATIN1 */
+    { 835,  2,   3}, /* LATINEXTENDEDA */
+    { 829,  2,   3}, /* LATINEXTA */
+    { 837,  2,   4}, /* LATINEXTENDEDB */
+    { 831,  2,   4}, /* LATINEXTB */
+    { 759,  2,   5}, /* IPAEXTENSIONS */
+    { 758,  2,   5}, /* IPAEXT */
+    {1294,  2,   6}, /* SPACINGMODIFIERLETTERS */
+    {1003,  2,   6}, /* MODIFIERLETTERS */
+    { 430,  2,   7}, /* COMBININGDIACRITICALMARKS */
+    { 521,  2,   7}, /* DIACRITICALS */
+    { 656,  2,   8}, /* GREEKANDCOPTIC */
+    { 655,  2,   8}, /* GREEK */
+    { 484,  2,   9}, /* CYRILLIC */
+    { 494,  2,  10}, /* CYRILLICSUPPLEMENT */
+    { 493,  2,  10}, /* CYRILLICSUP */
+    { 495,  2,  10}, /* CYRILLICSUPPLEMENTARY */
+    { 227,  2,  11}, /* ARMENIAN */
+    { 697,  2,  12}, /* HEBREW */
+    { 210,  2,  13}, /* ARABIC */
+    {1339,  2,  14}, /* SYRIAC */
+    { 226,  2,  15}, /* ARABICSUPPLEMENT */
+    { 225,  2,  15}, /* ARABICSUP */
+    {1380,  2,  16}, /* THAANA */
+    {1054,  2,  17}, /* NKO */
+    {1237,  2,  18}, /* SAMARITAN */
+    { 921,  2,  19}, /* MANDAIC */
+    {1341,  2,  20}, /* SYRIACSUPPLEMENT */
+    {1340,  2,  20}, /* SYRIACSUP */
+    { 215,  2,  21}, /* ARABICEXTENDEDB */
+    { 212,  2,  21}, /* ARABICEXTB */
+    { 214,  2,  22}, /* ARABICEXTENDEDA */
+    { 211,  2,  22}, /* ARABICEXTA */
+    { 513,  2,  23}, /* DEVANAGARI */
+    { 269,  2,  24}, /* BENGALI */
+    { 665,  2,  25}, /* GURMUKHI */
+    { 662,  2,  26}, /* GUJARATI */
+    {1114,  2,  27}, /* ORIYA */
+    {1358,  2,  28}, /* TAMIL */
+    {1373,  2,  29}, /* TELUGU */
+    { 795,  2,  30}, /* KANNADA */
+    { 908,  2,  31}, /* MALAYALAM */
+    {1271,  2,  32}, /* SINHALA */
+    {1381,  2,  33}, /* THAI */
+    { 823,  2,  34}, /* LAO */
+    {1383,  2,  35}, /* TIBETAN */
+    {1018,  2,  36}, /* MYANMAR */
+    { 631,  2,  37}, /* GEORGIAN */
+    { 680,  2,  38}, /* HANGULJAMO */
+    { 764,  2,  38}, /* JAMO */
+    { 582,  2,  39}, /* ETHIOPIC */
+    { 590,  2,  40}, /* ETHIOPICSUPPLEMENT */
+    { 589,  2,  40}, /* ETHIOPICSUP */
+    { 379,  2,  41}, /* CHEROKEE */
+    {1413,  2,  42}, /* UNIFIEDCANADIANABORIGINALSYLLABICS */
+    {1406,  2,  42}, /* UCAS */
+    { 318,  2,  42}, /* CANADIANSYLLABICS */
+    {1092,  2,  43}, /* OGHAM */
+    {1230,  2,  44}, /* RUNIC */
+    {1344,  2,  45}, /* TAGALOG */
+    { 692,  2,  46}, /* HANUNOO */
+    { 309,  2,  47}, /* BUHID */
+    {1346,  2,  48}, /* TAGBANWA */
+    { 807,  2,  49}, /* KHMER */
+    {1008,  2,  50}, /* MONGOLIAN */
+    {1414,  2,  51}, /* UNIFIEDCANADIANABORIGINALSYLLABICSEXTENDED */
+    {1407,  2,  51}, /* UCASEXT */
+    { 864,  2,  52}, /* LIMBU */
+    {1349,  2,  53}, /* TAILE */
+    {1043,  2,  54}, /* NEWTAILUE */
+    { 808,  2,  55}, /* KHMERSYMBOLS */
+    { 307,  2,  56}, /* BUGINESE */
+    {1350,  2,  57}, /* TAITHAM */
+    { 431,  2,  58}, /* COMBININGDIACRITICALMARKSEXTENDED */
+    { 522,  2,  58}, /* DIACRITICALSEXT */
+    { 252,  2,  59}, /* BALINESE */
+    {1304,  2,  60}, /* SUNDANESE */
+    { 260,  2,  61}, /* BATAK */
+    { 858,  2,  62}, /* LEPCHA */
+    {1096,  2,  63}, /* OLCHIKI */
+    { 491,  2,  64}, /* CYRILLICEXTENDEDC */
+    { 487,  2,  64}, /* CYRILLICEXTC */
+    { 633,  2,  65}, /* GEORGIANEXTENDED */
+    { 632,  2,  65}, /* GEORGIANEXT */
+    {1306,  2,  66}, /* SUNDANESESUPPLEMENT */
+    {1305,  2,  66}, /* SUNDANESESUP */
+    {1429,  2,  67}, /* VEDICEXTENSIONS */
+    {1428,  2,  67}, /* VEDICEXT */
+    {1171,  2,  68}, /* PHONETICEXTENSIONS */
+    {1170,  2,  68}, /* PHONETICEXT */
+    {1172,  2,  69}, /* PHONETICEXTENSIONSSUPPLEMENT */
+    {1173,  2,  69}, /* PHONETICEXTSUP */
+    { 433,  2,  70}, /* COMBININGDIACRITICALMARKSSUPPLEMENT */
+    { 524,  2,  70}, /* DIACRITICALSSUP */
+    { 836,  2,  71}, /* LATINEXTENDEDADDITIONAL */
+    { 830,  2,  71}, /* LATINEXTADDITIONAL */
+    { 658,  2,  72}, /* GREEKEXTENDED */
+    { 657,  2,  72}, /* GREEKEXT */
+    { 626,  2,  73}, /* GENERALPUNCTUATION */
+    {1198,  2,  73}, /* PUNCTUATION */
+    {1313,  2,  74}, /* SUPERSCRIPTSANDSUBSCRIPTS */
+    {1312,  2,  74}, /* SUPERANDSUB */
+    { 475,  2,  75}, /* CURRENCYSYMBOLS */
+    { 432,  2,  76}, /* COMBININGDIACRITICALMARKSFORSYMBOLS */
+    { 523,  2,  76}, /* DIACRITICALSFORSYMBOLS */
+    { 436,  2,  76}, /* COMBININGMARKSFORSYMBOLS */
+    { 860,  2,  77}, /* LETTERLIKESYMBOLS */
+    {1078,  2,  78}, /* NUMBERFORMS */
+    { 230,  2,  79}, /* ARROWS */
+    { 959,  2,  80}, /* MATHEMATICALOPERATORS */
+    { 960,  2,  80}, /* MATHOPERATORS */
+    { 992,  2,  81}, /* MISCELLANEOUSTECHNICAL */
+    { 997,  2,  81}, /* MISCTECHNICAL */
+    { 460,  2,  82}, /* CONTROLPICTURES */
+    {1113,  2,  83}, /* OPTICALCHARACTERRECOGNITION */
+    {1089,  2,  83}, /* OCR */
+    { 570,  2,  84}, /* ENCLOSEDALPHANUMERICS */
+    { 569,  2,  84}, /* ENCLOSEDALPHANUM */
+    { 294,  2,  85}, /* BOXDRAWING */
+    { 284,  2,  86}, /* BLOCKELEMENTS */
+    { 627,  2,  87}, /* GEOMETRICSHAPES */
+    { 989,  2,  88}, /* MISCELLANEOUSSYMBOLS */
+    { 996,  2,  88}, /* MISCSYMBOLS */
+    { 527,  2,  89}, /* DINGBATS */
+    { 987,  2,  90}, /* MISCELLANEOUSMATHEMATICALSYMBOLSA */
+    { 993,  2,  90}, /* MISCMATHSYMBOLSA */
+    {1315,  2,  91}, /* SUPPLEMENTALARROWSA */
+    {1308,  2,  91}, /* SUPARROWSA */
+    { 301,  2,  92}, /* BRAILLEPATTERNS */
+    { 300,  2,  92}, /* BRAILLE */
+    {1316,  2,  93}, /* SUPPLEMENTALARROWSB */
+    {1309,  2,  93}, /* SUPARROWSB */
+    { 988,  2,  94}, /* MISCELLANEOUSMATHEMATICALSYMBOLSB */
+    { 994,  2,  94}, /* MISCMATHSYMBOLSB */
+    {1318,  2,  95}, /* SUPPLEMENTALMATHEMATICALOPERATORS */
+    {1314,  2,  95}, /* SUPMATHOPERATORS */
+    { 990,  2,  96}, /* MISCELLANEOUSSYMBOLSANDARROWS */
+    { 986,  2,  96}, /* MISCARROWS */
+    { 638,  2,  97}, /* GLAGOLITIC */
+    { 838,  2,  98}, /* LATINEXTENDEDC */
+    { 832,  2,  98}, /* LATINEXTC */
+    { 462,  2,  99}, /* COPTIC */
+    { 635,  2, 100}, /* GEORGIANSUPPLEMENT */
+    { 634,  2, 100}, /* GEORGIANSUP */
+    {1385,  2, 101}, /* TIFINAGH */
+    { 586,  2, 102}, /* ETHIOPICEXTENDED */
+    { 583,  2, 102}, /* ETHIOPICEXT */
+    { 489,  2, 103}, /* CYRILLICEXTENDEDA */
+    { 485,  2, 103}, /* CYRILLICEXTA */
+    {1319,  2, 104}, /* SUPPLEMENTALPUNCTUATION */
+    {1325,  2, 104}, /* SUPPUNCTUATION */
+    { 407,  2, 105}, /* CJKRADICALSSUPPLEMENT */
+    { 406,  2, 105}, /* CJKRADICALSSUP */
+    { 794,  2, 106}, /* KANGXIRADICALS */
+    { 793,  2, 106}, /* KANGXI */
+    { 726,  2, 107}, /* IDEOGRAPHICDESCRIPTIONCHARACTERS */
+    { 720,  2, 107}, /* IDC */
+    { 410,  2, 108}, /* CJKSYMBOLSANDPUNCTUATION */
+    { 409,  2, 108}, /* CJKSYMBOLS */
+    { 708,  2, 109}, /* HIRAGANA */
+    { 797,  2, 110}, /* KATAKANA */
+    { 287,  2, 111}, /* BOPOMOFO */
+    { 679,  2, 112}, /* HANGULCOMPATIBILITYJAMO */
+    { 441,  2, 112}, /* COMPATJAMO */
+    { 792,  2, 113}, /* KANBUN */
+    { 289,  2, 114}, /* BOPOMOFOEXTENDED */
+    { 288,  2, 114}, /* BOPOMOFOEXT */
+    { 408,  2, 115}, /* CJKSTROKES */
+    { 800,  2, 116}, /* KATAKANAPHONETICEXTENSIONS */
+    { 798,  2, 116}, /* KATAKANAEXT */
+    { 574,  2, 117}, /* ENCLOSEDCJKLETTERSANDMONTHS */
+    { 573,  2, 117}, /* ENCLOSEDCJK */
+    { 391,  2, 118}, /* CJKCOMPATIBILITY */
+    { 389,  2, 118}, /* CJKCOMPAT */
+    { 412,  2, 119}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONA */
+    { 397,  2, 119}, /* CJKEXTA */
+    {1484,  2, 120}, /* YIJINGHEXAGRAMSYMBOLS */
+    {1483,  2, 120}, /* YIJING */
+    { 411,  2, 121}, /* CJKUNIFIEDIDEOGRAPHS */
+    { 388,  2, 121}, /* CJK */
+    {1486,  2, 122}, /* YISYLLABLES */
+    {1485,  2, 123}, /* YIRADICALS */
+    { 875,  2, 124}, /* LISU */
+    {1423,  2, 125}, /* VAI */
+    { 490,  2, 126}, /* CYRILLICEXTENDEDB */
+    { 486,  2, 126}, /* CYRILLICEXTB */
+    { 254,  2, 127}, /* BAMUM */
+    {1005,  2, 128}, /* MODIFIERTONELETTERS */
+    { 839,  2, 129}, /* LATINEXTENDEDD */
+    { 833,  2, 129}, /* LATINEXTD */
+    {1333,  2, 130}, /* SYLOTINAGRI */
+    { 438,  2, 131}, /* COMMONINDICNUMBERFORMS */
+    { 741,  2, 131}, /* INDICNUMBERFORMS */
+    {1163,  2, 132}, /* PHAGSPA */
+    {1241,  2, 133}, /* SAURASHTRA */
+    { 516,  2, 134}, /* DEVANAGARIEXTENDED */
+    { 514,  2, 134}, /* DEVANAGARIEXT */
+    { 802,  2, 135}, /* KAYAHLI */
+    {1213,  2, 136}, /* REJANG */
+    { 681,  2, 137}, /* HANGULJAMOEXTENDEDA */
+    { 765,  2, 137}, /* JAMOEXTA */
+    { 768,  2, 138}, /* JAVANESE */
+    {1022,  2, 139}, /* MYANMAREXTENDEDB */
+    {1020,  2, 139}, /* MYANMAREXTB */
+    { 372,  2, 140}, /* CHAM */
+    {1021,  2, 141}, /* MYANMAREXTENDEDA */
+    {1019,  2, 141}, /* MYANMAREXTA */
+    {1351,  2, 142}, /* TAIVIET */
+    { 974,  2, 143}, /* MEETEIMAYEKEXTENSIONS */
+    { 973,  2, 143}, /* MEETEIMAYEKEXT */
+    { 587,  2, 144}, /* ETHIOPICEXTENDEDA */
+    { 584,  2, 144}, /* ETHIOPICEXTA */
+    { 840,  2, 145}, /* LATINEXTENDEDE */
+    { 834,  2, 145}, /* LATINEXTE */
+    { 381,  2, 146}, /* CHEROKEESUPPLEMENT */
+    { 380,  2, 146}, /* CHEROKEESUP */
+    { 972,  2, 147}, /* MEETEIMAYEK */
+    { 683,  2, 148}, /* HANGULSYLLABLES */
+    { 678,  2, 148}, /* HANGUL */
+    { 682,  2, 149}, /* HANGULJAMOEXTENDEDB */
+    { 766,  2, 149}, /* JAMOEXTB */
+    { 706,  2, 150}, /* HIGHSURROGATES */
+    { 704,  2, 151}, /* HIGHPRIVATEUSESURROGATES */
+    { 705,  2, 151}, /* HIGHPUSURROGATES */
+    { 886,  2, 152}, /* LOWSURROGATES */
+    {1192,  2, 153}, /* PRIVATEUSEAREA */
+    {1196,  2, 153}, /* PUA */
+    {1191,  2, 153}, /* PRIVATEUSE */
+    { 393,  2, 154}, /* CJKCOMPATIBILITYIDEOGRAPHS */
+    { 395,  2, 154}, /* CJKCOMPATIDEOGRAPHS */
+    { 197,  2, 155}, /* ALPHABETICPRESENTATIONFORMS */
+    { 196,  2, 155}, /* ALPHABETICPF */
+    { 223,  2, 156}, /* ARABICPRESENTATIONFORMSA */
+    { 221,  2, 156}, /* ARABICPFA */
+    {1426,  2, 157}, /* VARIATIONSELECTORS */
+    {1448,  2, 157}, /* VS */
+    {1432,  2, 158}, /* VERTICALFORMS */
+    { 434,  2, 159}, /* COMBININGHALFMARKS */
+    { 672,  2, 159}, /* HALFMARKS */
+    { 392,  2, 160}, /* CJKCOMPATIBILITYFORMS */
+    { 390,  2, 160}, /* CJKCOMPATFORMS */
+    {1277,  2, 161}, /* SMALLFORMVARIANTS */
+    {1276,  2, 161}, /* SMALLFORMS */
+    { 224,  2, 162}, /* ARABICPRESENTATIONFORMSB */
+    { 222,  2, 162}, /* ARABICPFB */
+    { 674,  2, 163}, /* HALFWIDTHANDFULLWIDTHFORMS */
+    { 671,  2, 163}, /* HALFANDFULLFORMS */
+    {1295,  2, 164}, /* SPECIALS */
+    { 870,  2, 165}, /* LINEARBSYLLABARY */
+    { 869,  2, 166}, /* LINEARBIDEOGRAMS */
+    { 174,  2, 167}, /* AEGEANNUMBERS */
+    { 204,  2, 168}, /* ANCIENTGREEKNUMBERS */
+    { 205,  2, 169}, /* ANCIENTSYMBOLS */
+    {1165,  2, 170}, /* PHAISTOSDISC */
+    {1164,  2, 170}, /* PHAISTOS */
+    { 897,  2, 171}, /* LYCIAN */
+    { 324,  2, 172}, /* CARIAN */
+    { 463,  2, 173}, /* COPTICEPACTNUMBERS */
+    {1099,  2, 174}, /* OLDITALIC */
+    { 646,  2, 175}, /* GOTHIC */
+    {1101,  2, 176}, /* OLDPERMIC */
+    {1410,  2, 177}, /* UGARITIC */
+    {1102,  2, 178}, /* OLDPERSIAN */
+    { 511,  2, 179}, /* DESERET */
+    {1260,  2, 180}, /* SHAVIAN */
+    {1121,  2, 181}, /* OSMANYA */
+    {1118,  2, 182}, /* OSAGE */
+    { 555,  2, 183}, /* ELBASAN */
+    { 329,  2, 184}, /* CAUCASIANALBANIAN */
+    {1442,  2, 185}, /* VITHKUQI */
+    { 867,  2, 186}, /* LINEARA */
+    { 841,  2, 187}, /* LATINEXTENDEDF */
+    { 843,  2, 187}, /* LATINEXTF */
+    { 482,  2, 188}, /* CYPRIOTSYLLABARY */
+    { 737,  2, 189}, /* IMPERIALARAMAIC */
+    {1146,  2, 190}, /* PALMYRENE */
+    {1027,  2, 191}, /* NABATAEAN */
+    { 694,  2, 192}, /* HATRAN */
+    {1169,  2, 193}, /* PHOENICIAN */
+    { 899,  2, 194}, /* LYDIAN */
+    { 980,  2, 195}, /* MEROITICHIEROGLYPHS */
+    { 979,  2, 196}, /* MEROITICCURSIVE */
+    { 805,  2, 197}, /* KHAROSHTHI */
+    {1104,  2, 198}, /* OLDSOUTHARABIAN */
+    {1100,  2, 199}, /* OLDNORTHARABIAN */
+    { 924,  2, 200}, /* MANICHAEAN */
+    { 246,  2, 201}, /* AVESTAN */
+    { 753,  2, 202}, /* INSCRIPTIONALPARTHIAN */
+    { 752,  2, 203}, /* INSCRIPTIONALPAHLAVI */
+    {1195,  2, 204}, /* PSALTERPAHLAVI */
+    {1105,  2, 205}, /* OLDTURKIC */
+    {1098,  2, 206}, /* OLDHUNGARIAN */
+    { 686,  2, 207}, /* HANIFIROHINGYA */
+    {1229,  2, 208}, /* RUMINUMERALSYMBOLS */
+    {1228,  2, 208}, /* RUMI */
+    {1480,  2, 209}, /* YEZIDI */
+    { 216,  2, 210}, /* ARABICEXTENDEDC */
+    { 213,  2, 210}, /* ARABICEXTC */
+    {1103,  2, 211}, /* OLDSOGDIAN */
+    {1284,  2, 212}, /* SOGDIAN */
+    {1106,  2, 213}, /* OLDUYGHUR */
+    { 383,  2, 214}, /* CHORASMIAN */
+    { 557,  2, 215}, /* ELYMAIC */
+    { 297,  2, 216}, /* BRAHMI */
+    { 781,  2, 217}, /* KAITHI */
+    {1287,  2, 218}, /* SORASOMPENG */
+    { 371,  2, 219}, /* CHAKMA */
+    { 902,  2, 220}, /* MAHAJANI */
+    {1259,  2, 221}, /* SHARADA */
+    {1272,  2, 222}, /* SINHALAARCHAICNUMBERS */
+    { 811,  2, 223}, /* KHOJKI */
+    {1015,  2, 224}, /* MULTANI */
+    { 812,  2, 225}, /* KHUDAWADI */
+    { 648,  2, 226}, /* GRANTHA */
+    {1041,  2, 227}, /* NEWA */
+    {1387,  2, 228}, /* TIRHUTA */
+    {1266,  2, 229}, /* SIDDHAM */
+    {1001,  2, 230}, /* MODI */
+    {1010,  2, 231}, /* MONGOLIANSUPPLEMENT */
+    {1009,  2, 231}, /* MONGOLIANSUP */
+    {1355,  2, 232}, /* TAKRI */
+    { 180,  2, 233}, /* AHOM */
+    { 530,  2, 234}, /* DOGRA */
+    {1453,  2, 235}, /* WARANGCITI */
+    { 528,  2, 236}, /* DIVESAKURU */
+    {1032,  2, 237}, /* NANDINAGARI */
+    {1492,  2, 238}, /* ZANABAZARSQUARE */
+    {1289,  2, 239}, /* SOYOMBO */
+    {1415,  2, 240}, /* UNIFIEDCANADIANABORIGINALSYLLABICSEXTENDEDA */
+    {1408,  2, 240}, /* UCASEXTA */
+    {1153,  2, 241}, /* PAUCINHAU */
+    { 517,  2, 242}, /* DEVANAGARIEXTENDEDA */
+    { 515,  2, 242}, /* DEVANAGARIEXTA */
+    { 271,  2, 243}, /* BHAIKSUKI */
+    { 953,  2, 244}, /* MARCHEN */
+    { 955,  2, 245}, /* MASARAMGONDI */
+    { 664,  2, 246}, /* GUNJALAGONDI */
+    { 907,  2, 247}, /* MAKASAR */
+    { 801,  2, 248}, /* KAWI */
+    { 877,  2, 249}, /* LISUSUPPLEMENT */
+    { 876,  2, 249}, /* LISUSUP */
+    {1360,  2, 250}, /* TAMILSUPPLEMENT */
+    {1359,  2, 250}, /* TAMILSUP */
+    { 471,  2, 251}, /* CUNEIFORM */
+    { 473,  2, 252}, /* CUNEIFORMNUMBERSANDPUNCTUATION */
+    { 472,  2, 252}, /* CUNEIFORMNUMBERS */
+    { 544,  2, 253}, /* EARLYDYNASTICCUNEIFORM */
+    { 483,  2, 254}, /* CYPROMINOAN */
+    { 553,  2, 255}, /* EGYPTIANHIEROGLYPHS */
+    { 552,  2, 256}, /* EGYPTIANHIEROGLYPHFORMATCONTROLS */
+    { 201,  2, 257}, /* ANATOLIANHIEROGLYPHS */
+    { 256,  2, 258}, /* BAMUMSUPPLEMENT */
+    { 255,  2, 258}, /* BAMUMSUP */
+    {1011,  2, 259}, /* MRO */
+    {1363,  2, 260}, /* TANGSA */
+    { 259,  2, 261}, /* BASSAVAH */
+    {1144,  2, 262}, /* PAHAWHHMONG */
+    { 968,  2, 263}, /* MEDEFAIDRIN */
+    { 981,  2, 264}, /* MIAO */
+    { 728,  2, 265}, /* IDEOGRAPHICSYMBOLSANDPUNCTUATION */
+    { 727,  2, 265}, /* IDEOGRAPHICSYMBOLS */
+    {1364,  2, 266}, /* TANGUT */
+    {1365,  2, 267}, /* TANGUTCOMPONENTS */
+    { 806,  2, 268}, /* KHITANSMALLSCRIPT */
+    {1367,  2, 269}, /* TANGUTSUPPLEMENT */
+    {1366,  2, 269}, /* TANGUTSUP */
+    { 788,  2, 270}, /* KANAEXTENDEDB */
+    { 786,  2, 270}, /* KANAEXTB */
+    { 790,  2, 271}, /* KANASUPPLEMENT */
+    { 789,  2, 271}, /* KANASUP */
+    { 787,  2, 272}, /* KANAEXTENDEDA */
+    { 785,  2, 272}, /* KANAEXTA */
+    {1279,  2, 273}, /* SMALLKANAEXTENSION */
+    {1278,  2, 273}, /* SMALLKANAEXT */
+    {1084,  2, 274}, /* NUSHU */
+    { 541,  2, 275}, /* DUPLOYAN */
+    {1263,  2, 276}, /* SHORTHANDFORMATCONTROLS */
+    {1498,  2, 277}, /* ZNAMENNYMUSICALNOTATION */
+    {1497,  2, 277}, /* ZNAMENNYMUSIC */
+    { 312,  2, 278}, /* BYZANTINEMUSICALSYMBOLS */
+    { 311,  2, 278}, /* BYZANTINEMUSIC */
+    {1017,  2, 279}, /* MUSICALSYMBOLS */
+    {1016,  2, 279}, /* MUSIC */
+    { 203,  2, 280}, /* ANCIENTGREEKMUSICALNOTATION */
+    { 202,  2, 280}, /* ANCIENTGREEKMUSIC */
+    { 782,  2, 281}, /* KAKTOVIKNUMERALS */
+    { 962,  2, 282}, /* MAYANNUMERALS */
+    {1353,  2, 283}, /* TAIXUANJINGSYMBOLS */
+    {1352,  2, 283}, /* TAIXUANJING */
+    { 465,  2, 284}, /* COUNTINGRODNUMERALS */
+    { 464,  2, 284}, /* COUNTINGROD */
+    { 958,  2, 285}, /* MATHEMATICALALPHANUMERICSYMBOLS */
+    { 957,  2, 285}, /* MATHALPHANUM */
+    {1328,  2, 286}, /* SUTTONSIGNWRITING */
+    { 842,  2, 287}, /* LATINEXTENDEDG */
+    { 844,  2, 287}, /* LATINEXTG */
+    { 640,  2, 288}, /* GLAGOLITICSUPPLEMENT */
+    { 639,  2, 288}, /* GLAGOLITICSUP */
+    { 492,  2, 289}, /* CYRILLICEXTENDEDD */
+    { 488,  2, 289}, /* CYRILLICEXTD */
+    {1087,  2, 290}, /* NYIAKENGPUACHUEHMONG */
+    {1399,  2, 291}, /* TOTO */
+    {1451,  2, 292}, /* WANCHO */
+    {1029,  2, 293}, /* NAGMUNDARI */
+    { 588,  2, 294}, /* ETHIOPICEXTENDEDB */
+    { 585,  2, 294}, /* ETHIOPICEXTB */
+    { 976,  2, 295}, /* MENDEKIKAKUI */
+    { 172,  2, 296}, /* ADLAM */
+    { 743,  2, 297}, /* INDICSIYAQNUMBERS */
+    {1136,  2, 298}, /* OTTOMANSIYAQNUMBERS */
+    { 219,  2, 299}, /* ARABICMATHEMATICALALPHABETICSYMBOLS */
+    { 218,  2, 299}, /* ARABICMATH */
+    { 905,  2, 300}, /* MAHJONGTILES */
+    { 904,  2, 300}, /* MAHJONG */
+    { 532,  2, 301}, /* DOMINOTILES */
+    { 531,  2, 301}, /* DOMINO */
+    {1175,  2, 302}, /* PLAYINGCARDS */
+    { 571,  2, 303}, /* ENCLOSEDALPHANUMERICSUPPLEMENT */
+    { 572,  2, 303}, /* ENCLOSEDALPHANUMSUP */
+    { 576,  2, 304}, /* ENCLOSEDIDEOGRAPHICSUPPLEMENT */
+    { 575,  2, 304}, /* ENCLOSEDIDEOGRAPHICSUP */
+    { 991,  2, 305}, /* MISCELLANEOUSSYMBOLSANDPICTOGRAPHS */
+    { 995,  2, 305}, /* MISCPICTOGRAPHS */
+    { 566,  2, 306}, /* EMOTICONS */
+    {1116,  2, 307}, /* ORNAMENTALDINGBATS */
+    {1403,  2, 308}, /* TRANSPORTANDMAPSYMBOLS */
+    {1402,  2, 308}, /* TRANSPORTANDMAP */
+    { 190,  2, 309}, /* ALCHEMICALSYMBOLS */
+    { 189,  2, 309}, /* ALCHEMICAL */
+    { 629,  2, 310}, /* GEOMETRICSHAPESEXTENDED */
+    { 628,  2, 310}, /* GEOMETRICSHAPESEXT */
+    {1317,  2, 311}, /* SUPPLEMENTALARROWSC */
+    {1310,  2, 311}, /* SUPARROWSC */
+    {1320,  2, 312}, /* SUPPLEMENTALSYMBOLSANDPICTOGRAPHS */
+    {1326,  2, 312}, /* SUPSYMBOLSANDPICTOGRAPHS */
+    { 382,  2, 313}, /* CHESSSYMBOLS */
+    {1336,  2, 314}, /* SYMBOLSANDPICTOGRAPHSEXTENDEDA */
+    {1335,  2, 314}, /* SYMBOLSANDPICTOGRAPHSEXTA */
+    {1337,  2, 315}, /* SYMBOLSFORLEGACYCOMPUTING */
+    { 413,  2, 316}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONB */
+    { 398,  2, 316}, /* CJKEXTB */
+    { 414,  2, 317}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONC */
+    { 399,  2, 317}, /* CJKEXTC */
+    { 415,  2, 318}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIOND */
+    { 400,  2, 318}, /* CJKEXTD */
+    { 416,  2, 319}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONE */
+    { 401,  2, 319}, /* CJKEXTE */
+    { 417,  2, 320}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONF */
+    { 402,  2, 320}, /* CJKEXTF */
+    { 420,  2, 321}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONI */
+    { 405,  2, 321}, /* CJKEXTI */
+    { 394,  2, 322}, /* CJKCOMPATIBILITYIDEOGRAPHSSUPPLEMENT */
+    { 396,  2, 322}, /* CJKCOMPATIDEOGRAPHSSUP */
+    { 418,  2, 323}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONG */
+    { 403,  2, 323}, /* CJKEXTG */
+    { 419,  2, 324}, /* CJKUNIFIEDIDEOGRAPHSEXTENSIONH */
+    { 404,  2, 324}, /* CJKEXTH */
+    {1347,  2, 325}, /* TAGS */
+    {1427,  2, 326}, /* VARIATIONSELECTORSSUPPLEMENT */
+    {1449,  2, 326}, /* VSSUP */
+    {1321,  2, 327}, /* SUPPLEMENTARYPRIVATEUSEAREAA */
+    {1323,  2, 327}, /* SUPPUAA */
+    {1322,  2, 328}, /* SUPPLEMENTARYPRIVATEUSEAREAB */
+    {1324,  2, 328}, /* SUPPUAB */
+    {1069,  3,   0}, /* NOTREORDERED */
     {   1,  3,   0}, /* 0 */
-    {1053,  3,   0}, /* NR */
-    { 167,  3,   1}, /* ABOVE */
-    {  75,  3,   1}, /* 230 */
-    { 166,  3,   1}, /* A */
-    { 169,  3,   2}, /* ABOVERIGHT */
-    {  76,  3,   2}, /* 232 */
-    { 201,  3,   2}, /* AR */
-    { 257,  3,   3}, /* BELOW */
-    {  69,  3,   3}, /* 220 */
-    { 240,  3,   3}, /* B */
-    { 234,  3,   4}, /* ATTACHEDABOVERIGHT */
-    {  65,  3,   4}, /* 216 */
-    { 229,  3,   4}, /* ATAR */
-    { 235,  3,   5}, /* ATTACHEDBELOW */
-    {  62,  3,   5}, /* 202 */
-    { 230,  3,   5}, /* ATB */
-    {1123,  3,   6}, /* OVERLAY */
+    {1070,  3,   0}, /* NR */
+    { 169,  3,   1}, /* ABOVE */
+    {  77,  3,   1}, /* 230 */
+    { 168,  3,   1}, /* A */
+    { 171,  3,   2}, /* ABOVERIGHT */
+    {  78,  3,   2}, /* 232 */
+    { 208,  3,   2}, /* AR */
+    { 265,  3,   3}, /* BELOW */
+    {  71,  3,   3}, /* 220 */
+    { 248,  3,   3}, /* B */
+    { 242,  3,   4}, /* ATTACHEDABOVERIGHT */
+    {  67,  3,   4}, /* 216 */
+    { 237,  3,   4}, /* ATAR */
+    { 243,  3,   5}, /* ATTACHEDBELOW */
+    {  64,  3,   5}, /* 202 */
+    { 238,  3,   5}, /* ATB */
+    {1140,  3,   6}, /* OVERLAY */
     {   2,  3,   6}, /* 1 */
-    {1122,  3,   6}, /* OV */
-    { 741,  3,   7}, /* IOTASUBSCRIPT */
-    {  80,  3,   7}, /* 240 */
-    { 744,  3,   7}, /* IS */
-    { 524,  3,   8}, /* DOUBLEBELOW */
-    {  77,  3,   8}, /* 233 */
-    { 493,  3,   8}, /* DB */
-    { 523,  3,   9}, /* DOUBLEABOVE */
-    {  78,  3,   9}, /* 234 */
-    { 488,  3,   9}, /* DA */
-    { 259,  3,  10}, /* BELOWRIGHT */
-    {  70,  3,  10}, /* 222 */
-    { 287,  3,  10}, /* BR */
-    { 168,  3,  11}, /* ABOVELEFT */
-    {  73,  3,  11}, /* 228 */
-    { 181,  3,  11}, /* AL */
-    { 325,  3,  12}, /* CCC10 */
+    {1139,  3,   6}, /* OV */
+    { 757,  3,   7}, /* IOTASUBSCRIPT */
+    {  82,  3,   7}, /* 240 */
+    { 760,  3,   7}, /* IS */
+    { 534,  3,   8}, /* DOUBLEBELOW */
+    {  79,  3,   8}, /* 233 */
+    { 503,  3,   8}, /* DB */
+    { 533,  3,   9}, /* DOUBLEABOVE */
+    {  80,  3,   9}, /* 234 */
+    { 498,  3,   9}, /* DA */
+    { 267,  3,  10}, /* BELOWRIGHT */
+    {  72,  3,  10}, /* 222 */
+    { 295,  3,  10}, /* BR */
+    { 170,  3,  11}, /* ABOVELEFT */
+    {  75,  3,  11}, /* 228 */
+    { 187,  3,  11}, /* AL */
+    { 333,  3,  12}, /* CCC10 */
     {  21,  3,  12}, /* 10 */
-    { 328,  3,  13}, /* CCC11 */
-    {  33,  3,  13}, /* 11 */
-    { 330,  3,  14}, /* CCC12 */
-    {  37,  3,  14}, /* 12 */
-    { 333,  3,  15}, /* CCC13 */
-    {  40,  3,  15}, /* 13 */
-    { 337,  3,  16}, /* CCC14 */
-    {  45,  3,  16}, /* 14 */
-    { 338,  3,  17}, /* CCC15 */
-    {  46,  3,  17}, /* 15 */
-    { 339,  3,  18}, /* CCC16 */
-    {  48,  3,  18}, /* 16 */
-    { 340,  3,  19}, /* CCC17 */
-    {  49,  3,  19}, /* 17 */
-    { 341,  3,  20}, /* CCC18 */
-    {  51,  3,  20}, /* 18 */
-    { 342,  3,  21}, /* CCC19 */
-    {  52,  3,  21}, /* 19 */
-    { 343,  3,  22}, /* CCC20 */
-    {  56,  3,  22}, /* 20 */
-    { 344,  3,  23}, /* CCC21 */
-    {  63,  3,  23}, /* 21 */
-    { 345,  3,  24}, /* CCC22 */
-    {  68,  3,  24}, /* 22 */
-    { 346,  3,  25}, /* CCC23 */
-    {  74,  3,  25}, /* 23 */
-    { 347,  3,  26}, /* CCC24 */
-    {  79,  3,  26}, /* 24 */
-    { 348,  3,  27}, /* CCC25 */
-    {  81,  3,  27}, /* 25 */
-    { 353,  3,  28}, /* CCC30 */
-    {  95,  3,  28}, /* 30 */
-    { 354,  3,  29}, /* CCC31 */
-    { 100,  3,  29}, /* 31 */
-    { 355,  3,  30}, /* CCC32 */
-    { 101,  3,  30}, /* 32 */
-    { 350,  3,  31}, /* CCC27 */
-    {  83,  3,  31}, /* 27 */
-    { 351,  3,  32}, /* CCC28 */
-    {  84,  3,  32}, /* 28 */
-    { 352,  3,  33}, /* CCC29 */
-    {  85,  3,  33}, /* 29 */
-    { 356,  3,  34}, /* CCC33 */
-    { 102,  3,  34}, /* 33 */
-    { 357,  3,  35}, /* CCC34 */
-    { 103,  3,  35}, /* 34 */
-    { 358,  3,  36}, /* CCC35 */
-    { 104,  3,  36}, /* 35 */
-    { 359,  3,  37}, /* CCC36 */
-    { 105,  3,  37}, /* 36 */
-    {1059,  3,  38}, /* NUKTA */
-    { 142,  3,  38}, /* 7 */
-    {1036,  3,  38}, /* NK */
-    {1418,  3,  39}, /* VIRAMA */
-    { 158,  3,  39}, /* 9 */
-    {1427,  3,  39}, /* VR */
-    { 360,  3,  40}, /* CCC84 */
-    { 157,  3,  40}, /* 84 */
-    { 361,  3,  41}, /* CCC91 */
-    { 165,  3,  41}, /* 91 */
-    { 326,  3,  42}, /* CCC103 */
-    {  31,  3,  42}, /* 103 */
-    { 327,  3,  43}, /* CCC107 */
-    {  32,  3,  43}, /* 107 */
-    { 329,  3,  44}, /* CCC118 */
-    {  36,  3,  44}, /* 118 */
-    { 331,  3,  45}, /* CCC122 */
-    {  38,  3,  45}, /* 122 */
-    { 332,  3,  46}, /* CCC129 */
-    {  39,  3,  46}, /* 129 */
-    { 334,  3,  47}, /* CCC130 */
-    {  42,  3,  47}, /* 130 */
-    { 335,  3,  48}, /* CCC132 */
-    {  43,  3,  48}, /* 132 */
-    { 233,  3,  49}, /* ATTACHEDABOVE */
-    {  64,  3,  49}, /* 214 */
-    { 228,  3,  49}, /* ATA */
-    { 258,  3,  50}, /* BELOWLEFT */
-    {  67,  3,  50}, /* 218 */
-    { 272,  3,  50}, /* BL */
-    { 834,  3,  51}, /* LEFT */
-    {  71,  3,  51}, /* 224 */
-    { 802,  3,  51}, /* L */
-    { 775,  3,  52}, /* KANAVOICING */
-    { 151,  3,  52}, /* 8 */
-    { 801,  3,  52}, /* KV */
-    { 349,  3,  53}, /* CCC26 */
-    {  82,  3,  53}, /* 26 */
-    { 681,  3,  54}, /* HANREADING */
-    { 136,  3,  54}, /* 6 */
-    { 680,  3,  54}, /* HANR */
-    {1199,  3,  55}, /* RIGHT */
-    {  72,  3,  55}, /* 226 */
-    {1191,  3,  55}, /* R */
-    { 336,  3,  56}, /* CCC133 */
-    {  44,  3,  56}, /* 133 */
-    { 236,  3,  57}, /* ATTACHEDBELOWLEFT */
-    {  57,  3,  57}, /* 200 */
-    { 231,  3,  57}, /* ATBL */
-    {1045,  4,   0}, /* NONE */
-    {1042,  4,   1}, /* NOBREAK */
-    {1019,  4,   1}, /* NB */
-    { 430,  4,   2}, /* COMPAT */
-    { 419,  4,   2}, /* COM */
-    {1294,  4,   3}, /* SUPER */
-    {1290,  4,   3}, /* SUP */
-    { 606,  4,   4}, /* FRACTION */
-    { 605,  4,   4}, /* FRA */
-    { 311,  4,   5}, /* CANONICAL */
-    { 308,  4,   5}, /* CAN */
-    {1285,  4,   6}, /* SUB */
-    { 603,  4,   7}, /* FONT */
-    { 378,  4,   8}, /* CIRCLE */
-    { 558,  4,   8}, /* ENC */
-    {1438,  4,   9}, /* WIDE */
-    {1414,  4,  10}, /* VERTICAL */
-    {1413,  4,  10}, /* VERT */
-    {1281,  4,  11}, /* SQUARE */
-    {1280,  4,  11}, /* SQR */
-    { 746,  4,  12}, /* ISOLATED */
-    { 745,  4,  12}, /* ISO */
-    { 598,  4,  13}, /* FINAL */
-    { 597,  4,  13}, /* FIN */
-    { 732,  4,  14}, /* INITIAL */
-    { 731,  4,  14}, /* INIT */
-    { 953,  4,  15}, /* MEDIAL */
-    { 950,  4,  15}, /* MED */
-    {1258,  4,  16}, /* SMALL */
-    {1263,  4,  16}, /* SML */
-    {1018,  4,  17}, /* NARROW */
-    {1016,  4,  17}, /* NAR */
-    {1438,  5,   0}, /* WIDE */
-    {1430,  5,   0}, /* W */
-    {1023,  5,   1}, /* NEUTRAL */
-    {1007,  5,   1}, /* N */
-    {1018,  5,   2}, /* NARROW */
-    {1009,  5,   2}, /* NA */
-    { 193,  5,   3}, /* AMBIGUOUS */
-    { 166,  5,   3}, /* A */
-    { 663,  5,   4}, /* HALFWIDTH */
-    { 657,  5,   4}, /* H */
-    { 608,  5,   5}, /* FULLWIDTH */
-    { 592,  5,   5}, /* F */
-    {1395,  6,   0}, /* UNASSIGNED */
-    { 416,  6,   0}, /* CN */
-    { 449,  6,   1}, /* CONTROL */
-    { 323,  6,   1}, /* CC */
-    { 417,  6,   1}, /* CNTRL */
-    {1275,  6,   2}, /* SPACESEPARATOR */
-    {1480,  6,   2}, /* ZS */
-    {1116,  6,   3}, /* OTHERPUNCTUATION */
-    {1160,  6,   3}, /* PO */
-    { 464,  6,   4}, /* CURRENCYSYMBOL */
-    {1226,  6,   4}, /* SC */
-    {1095,  6,   5}, /* OPENPUNCTUATION */
-    {1177,  6,   5}, /* PS */
-    { 414,  6,   6}, /* CLOSEPUNCTUATION */
-    {1142,  6,   6}, /* PE */
-    { 944,  6,   7}, /* MATHSYMBOL */
-    {1257,  6,   7}, /* SM */
-    { 492,  6,   8}, /* DASHPUNCTUATION */
-    {1139,  6,   8}, /* PD */
-    { 496,  6,   9}, /* DECIMALNUMBER */
-    {1022,  6,   9}, /* ND */
-    { 516,  6,   9}, /* DIGIT */
-    {1404,  6,  10}, /* UPPERCASELETTER */
-    { 874,  6,  10}, /* LU */
-    { 987,  6,  11}, /* MODIFIERSYMBOL */
-    {1256,  6,  11}, /* SK */
-    { 434,  6,  12}, /* CONNECTORPUNCTUATION */
-    {1137,  6,  12}, /* PC */
-    { 868,  6,  13}, /* LOWERCASELETTER */
-    { 861,  6,  13}, /* LL */
-    {1117,  6,  14}, /* OTHERSYMBOL */
-    {1264,  6,  14}, /* SO */
-    {1111,  6,  15}, /* OTHERLETTER */
-    { 863,  6,  15}, /* LO */
-    { 733,  6,  16}, /* INITIALPUNCTUATION */
-    {1157,  6,  16}, /* PI */
-    { 604,  6,  17}, /* FORMAT */
-    { 362,  6,  17}, /* CF */
-    {1115,  6,  18}, /* OTHERNUMBER */
-    {1040,  6,  18}, /* NO */
-    { 599,  6,  19}, /* FINALPUNCTUATION */
-    {1144,  6,  19}, /* PF */
-    {1371,  6,  20}, /* TITLECASELETTER */
-    { 873,  6,  20}, /* LT */
-    { 985,  6,  21}, /* MODIFIERLETTER */
-    { 862,  6,  21}, /* LM */
-    {1048,  6,  22}, /* NONSPACINGMARK */
-    { 983,  6,  22}, /* MN */
-    { 567,  6,  23}, /* ENCLOSINGMARK */
-    { 949,  6,  23}, /* ME */
-    {1276,  6,  24}, /* SPACINGMARK */
-    { 948,  6,  24}, /* MC */
-    { 845,  6,  25}, /* LETTERNUMBER */
-    {1039,  6,  25}, /* NL */
-    { 857,  6,  26}, /* LINESEPARATOR */
-    {1476,  6,  26}, /* ZL */
-    {1130,  6,  27}, /* PARAGRAPHSEPARATOR */
-    {1479,  6,  27}, /* ZP */
-    {1310,  6,  28}, /* SURROGATE */
-    { 460,  6,  28}, /* CS */
-    {1174,  6,  29}, /* PRIVATEUSE */
-    { 418,  6,  29}, /* CO */
-    {1105,  6,  30}, /* OTHER */
-    { 305,  6,  30}, /* C */
-    { 306,  6,  30}, /* C& */
-    { 843,  6,  31}, /* LETTER */
-    { 802,  6,  31}, /* L */
-    { 803,  6,  31}, /* L& */
-    { 937,  6,  32}, /* MARK */
-    { 883,  6,  32}, /* M */
-    { 425,  6,  32}, /* COMBININGMARK */
-    { 884,  6,  32}, /* M& */
-    {1060,  6,  33}, /* NUMBER */
-    {1007,  6,  33}, /* N */
-    {1008,  6,  33}, /* N& */
-    {1181,  6,  34}, /* PUNCTUATION */
-    {1125,  6,  34}, /* P */
-    {1180,  6,  34}, /* PUNCT */
-    {1126,  6,  34}, /* P& */
-    {1317,  6,  35}, /* SYMBOL */
-    {1215,  6,  35}, /* S */
-    {1216,  6,  35}, /* S& */
-    {1239,  6,  36}, /* SEPARATOR */
-    {1469,  6,  36}, /* Z */
-    {1470,  6,  36}, /* Z& */
-    { 226,  6,  37}, /* ASSIGNED */
-    { 319,  6,  38}, /* CASEDLETTER */
-    { 831,  6,  38}, /* LC */
-    {1105,  7,   0}, /* OTHER */
-    {1453,  7,   0}, /* XX */
-    { 449,  7,   1}, /* CONTROL */
-    { 416,  7,   1}, /* CN */
-    { 846,  7,   2}, /* LF */
-    { 459,  7,   3}, /* CR */
-    { 587,  7,   4}, /* EXTEND */
-    { 584,  7,   4}, /* EX */
-    {1171,  7,   5}, /* PREPEND */
-    {1168,  7,   5}, /* PP */
-    {1276,  7,   6}, /* SPACINGMARK */
-    {1257,  7,   6}, /* SM */
-    { 802,  7,   7}, /* L */
-    {1405,  7,   8}, /* V */
-    {1326,  7,   9}, /* T */
-    {1482,  7,  10}, /* ZWJ */
-    { 875,  7,  11}, /* LV */
-    { 877,  7,  12}, /* LVT */
-    {1193,  7,  13}, /* REGIONALINDICATOR */
-    {1198,  7,  13}, /* RI */
-    { 537,  7,  14}, /* EBASE */
-    { 536,  7,  14}, /* EB */
-    { 538,  7,  15}, /* EBASEGAZ */
-    { 539,  7,  15}, /* EBG */
-    { 550,  7,  16}, /* EMODIFIER */
-    { 548,  7,  16}, /* EM */
-    { 632,  7,  17}, /* GLUEAFTERZWJ */
-    { 611,  7,  17}, /* GAZ */
-    {1051,  8,   0}, /* NOTAPPLICABLE */
-    {1009,  8,   0}, /* NA */
-    { 833,  8,   1}, /* LEADINGJAMO */
-    { 802,  8,   1}, /* L */
-    {1426,  8,   2}, /* VOWELJAMO */
-    {1405,  8,   2}, /* V */
-    {1383,  8,   3}, /* TRAILINGJAMO */
-    {1326,  8,   3}, /* T */
-    { 876,  8,   4}, /* LVSYLLABLE */
-    { 875,  8,   4}, /* LV */
-    { 878,  8,   5}, /* LVTSYLLABLE */
-    { 877,  8,   5}, /* LVT */
-    {1009,  9,   0}, /* NA */
-    {1375,  9,   1}, /* TOP */
-    {1199,  9,   2}, /* RIGHT */
-    { 282,  9,   3}, /* BOTTOM */
-    { 834,  9,   4}, /* LEFT */
-    { 835,  9,   5}, /* LEFTANDRIGHT */
-    {1381,  9,   6}, /* TOPANDRIGHT */
-    {1379,  9,   7}, /* TOPANDLEFT */
-    {1380,  9,   8}, /* TOPANDLEFTANDRIGHT */
-    {1376,  9,   9}, /* TOPANDBOTTOM */
-    {1420,  9,  10}, /* VISUALORDERLEFT */
-    {1377,  9,  11}, /* TOPANDBOTTOMANDLEFT */
-    { 284,  9,  12}, /* BOTTOMANDRIGHT */
-    {1378,  9,  13}, /* TOPANDBOTTOMANDRIGHT */
-    {1124,  9,  14}, /* OVERSTRUCK */
-    { 283,  9,  15}, /* BOTTOMANDLEFT */
-    {1105, 10,   0}, /* OTHER */
-    { 442, 10,   1}, /* CONSONANTPLACEHOLDER */
-    {1060, 10,   2}, /* NUMBER */
-    {1314, 10,   3}, /* SYLLABLEMODIFIER */
-    { 270, 10,   4}, /* BINDU */
-    {1419, 10,   5}, /* VISARGA */
-    {1425, 10,   6}, /* VOWELINDEPENDENT */
-    { 435, 10,   7}, /* CONSONANT */
-    {1424, 10,   8}, /* VOWELDEPENDENT */
-    {1059, 10,   9}, /* NUKTA */
-    { 237, 10,  10}, /* AVAGRAHA */
-    {1418, 10,  11}, /* VIRAMA */
-    { 314, 10,  12}, /* CANTILLATIONMARK */
-    { 436, 10,  13}, /* CONSONANTDEAD */
-    { 614, 10,  14}, /* GEMINATIONMARK */
-    { 441, 10,  15}, /* CONSONANTMEDIAL */
-    { 989, 10,  16}, /* MODIFYINGLETTER */
-    { 447, 10,  17}, /* CONSONANTWITHSTACKER */
-    {1182, 10,  18}, /* PUREKILLER */
-    { 443, 10,  19}, /* CONSONANTPRECEDINGREPHA */
-    {1374, 10,  20}, /* TONEMARK */
-    { 440, 10,  21}, /* CONSONANTKILLER */
-    { 438, 10,  22}, /* CONSONANTHEADLETTER */
-    { 445, 10,  23}, /* CONSONANTSUBJOINED */
-    { 740, 10,  24}, /* INVISIBLESTACKER */
-    {1194, 10,  25}, /* REGISTERSHIFTER */
-    { 446, 10,  26}, /* CONSONANTSUCCEEDINGREPHA */
-    { 437, 10,  27}, /* CONSONANTFINAL */
-    {1423, 10,  28}, /* VOWEL */
-    {1373, 10,  29}, /* TONELETTER */
-    { 439, 10,  30}, /* CONSONANTINITIALPOSTFIXED */
-    {1046, 10,  31}, /* NONJOINER */
-    { 758, 10,  32}, /* JOINER */
-    { 290, 10,  33}, /* BRAHMIJOININGNUMBER */
-    {1062, 10,  34}, /* NUMBERJOINER */
-    { 444, 10,  35}, /* CONSONANTPREFIXED */
-    {1043, 11,   0}, /* NOJOININGGROUP */
-    {1455, 11,   1}, /* YEH */
-    { 185, 11,   2}, /* ALEF */
-    {1434, 11,   3}, /* WAW */
-    { 256, 11,   4}, /* BEH */
-    {1353, 11,   5}, /* TEHMARBUTA */
-    { 660, 11,   6}, /* HAH */
-    { 489, 11,   7}, /* DAL */
-    {1195, 11,   8}, /* REH */
-    {1233, 11,   9}, /* SEEN */
-    {1218, 11,  10}, /* SAD */
-    {1331, 11,  11}, /* TAH */
-    { 180, 11,  12}, /* AIN */
-    { 609, 11,  13}, /* GAF */
-    { 594, 11,  14}, /* FARSIYEH */
-    { 596, 11,  15}, /* FEH */
-    {1185, 11,  16}, /* QAF */
-    { 764, 11,  17}, /* KAF */
-    { 804, 11,  18}, /* LAM */
-    { 954, 11,  19}, /* MEEM */
-    {1050, 11,  20}, /* NOON */
-    { 689, 11,  21}, /* HEH */
-    {1312, 11,  22}, /* SWASHKAF */
-    {1069, 11,  23}, /* NYA */
-    { 799, 11,  24}, /* KNOTTEDHEH */
-    { 690, 11,  25}, /* HEHGOAL */
-    { 665, 11,  26}, /* HAMZAONHEHGOAL */
-    {1354, 11,  26}, /* TEHMARBUTAGOAL */
-    {1457, 11,  27}, /* YEHWITHTAIL */
-    {1456, 11,  28}, /* YEHBARREE */
-    { 182, 11,  29}, /* ALAPH */
-    { 262, 11,  30}, /* BETH */
-    { 610, 11,  31}, /* GAMAL */
-    { 490, 11,  32}, /* DALATHRISH */
-    { 685, 11,  33}, /* HE */
-    {1325, 11,  34}, /* SYRIACWAW */
-    {1471, 11,  35}, /* ZAIN */
-    { 691, 11,  36}, /* HETH */
-    {1359, 11,  37}, /* TETH */
-    {1467, 11,  38}, /* YUDH */
-    {1468, 11,  39}, /* YUDHHE */
-    { 780, 11,  40}, /* KAPH */
-    { 805, 11,  41}, /* LAMADH */
-    { 968, 11,  42}, /* MIM */
-    {1066, 11,  43}, /* NUN */
-    {1235, 11,  44}, /* SEMKATH */
-    { 600, 11,  45}, /* FINALSEMKATH */
-    { 532, 11,  46}, /* E */
-    {1142, 11,  47}, /* PE */
-    {1197, 11,  48}, /* REVERSEDPE */
-    {1219, 11,  49}, /* SADHE */
-    {1186, 11,  50}, /* QAPH */
-    {1245, 11,  51}, /* SHIN */
-    {1352, 11,  52}, /* TAW */
-    {1474, 11,  53}, /* ZHAIN */
-    { 787, 11,  54}, /* KHAPH */
-    { 595, 11,  55}, /* FE */
-    { 302, 11,  56}, /* BURUSHASKIYEHBARREE */
-    { 896, 11,  57}, /* MALAYALAMNGA */
-    { 893, 11,  58}, /* MALAYALAMJA */
-    { 899, 11,  59}, /* MALAYALAMNYA */
-    { 902, 11,  60}, /* MALAYALAMTTA */
-    { 897, 11,  61}, /* MALAYALAMNNA */
-    { 898, 11,  62}, /* MALAYALAMNNNA */
-    { 892, 11,  63}, /* MALAYALAMBHA */
-    { 900, 11,  64}, /* MALAYALAMRA */
-    { 894, 11,  65}, /* MALAYALAMLLA */
-    { 895, 11,  66}, /* MALAYALAMLLLA */
-    { 901, 11,  67}, /* MALAYALAMSSA */
-    {1365, 11,  68}, /* THINYEH */
-    {1416, 11,  69}, /* VERTICALTAIL */
-    {1210, 11,  70}, /* ROHINGYAYEH */
-    {1284, 11,  71}, /* STRAIGHTWAW */
-    { 173, 11,  72}, /* AFRICANFEH */
-    { 175, 11,  73}, /* AFRICANQAF */
-    { 174, 11,  74}, /* AFRICANNOON */
-    { 908, 11,  75}, /* MANICHAEANALEPH */
-    { 910, 11,  76}, /* MANICHAEANBETH */
-    { 914, 11,  77}, /* MANICHAEANGIMEL */
-    { 911, 11,  78}, /* MANICHAEANDALETH */
-    { 932, 11,  79}, /* MANICHAEANWAW */
-    { 934, 11,  80}, /* MANICHAEANZAYIN */
-    { 915, 11,  81}, /* MANICHAEANHETH */
-    { 929, 11,  82}, /* MANICHAEANTETH */
-    { 933, 11,  83}, /* MANICHAEANYODH */
-    { 917, 11,  84}, /* MANICHAEANKAPH */
-    { 918, 11,  85}, /* MANICHAEANLAMEDH */
-    { 912, 11,  86}, /* MANICHAEANDHAMEDH */
-    { 930, 11,  87}, /* MANICHAEANTHAMEDH */
-    { 919, 11,  88}, /* MANICHAEANMEM */
-    { 920, 11,  89}, /* MANICHAEANNUN */
-    { 926, 11,  90}, /* MANICHAEANSAMEKH */
-    { 909, 11,  91}, /* MANICHAEANAYIN */
-    { 922, 11,  92}, /* MANICHAEANPE */
-    { 925, 11,  93}, /* MANICHAEANSADHE */
-    { 923, 11,  94}, /* MANICHAEANQOPH */
-    { 924, 11,  95}, /* MANICHAEANRESH */
-    { 927, 11,  96}, /* MANICHAEANTAW */
-    { 921, 11,  97}, /* MANICHAEANONE */
-    { 913, 11,  98}, /* MANICHAEANFIVE */
-    { 928, 11,  99}, /* MANICHAEANTEN */
-    { 931, 11, 100}, /* MANICHAEANTWENTY */
-    { 916, 11, 101}, /* MANICHAEANHUNDRED */
-    { 678, 11, 102}, /* HANIFIROHINGYAPA */
-    { 677, 11, 103}, /* HANIFIROHINGYAKINNAYA */
-    {1047, 12,   0}, /* NONJOINING */
-    {1388, 12,   0}, /* U */
-    {1384, 12,   1}, /* TRANSPARENT */
-    {1326, 12,   1}, /* T */
-    { 529, 12,   2}, /* DUALJOINING */
-    { 487, 12,   2}, /* D */
-    {1200, 12,   3}, /* RIGHTJOINING */
-    {1191, 12,   3}, /* R */
-    { 756, 12,   4}, /* JOINCAUSING */
-    { 305, 12,   4}, /* C */
-    { 836, 12,   5}, /* LEFTJOINING */
-    { 802, 12,   5}, /* L */
-    {1400, 13,   0}, /* UNKNOWN */
-    {1453, 13,   0}, /* XX */
-    { 425, 13,   1}, /* COMBININGMARK */
-    { 415, 13,   1}, /* CM */
-    { 294, 13,   2}, /* BREAKAFTER */
-    { 242, 13,   2}, /* BA */
-    { 856, 13,   3}, /* LINEFEED */
-    { 846, 13,   3}, /* LF */
-    { 905, 13,   4}, /* MANDATORYBREAK */
-    { 271, 13,   4}, /* BK */
-    { 317, 13,   5}, /* CARRIAGERETURN */
-    { 459, 13,   5}, /* CR */
-    {1274, 13,   6}, /* SPACE */
-    {1273, 13,   6}, /* SP */
-    { 585, 13,   7}, /* EXCLAMATION */
-    { 584, 13,   7}, /* EX */
-    {1189, 13,   8}, /* QUOTATION */
-    {1188, 13,   8}, /* QU */
-    { 189, 13,   9}, /* ALPHABETIC */
-    { 181, 13,   9}, /* AL */
-    {1170, 13,  10}, /* PREFIXNUMERIC */
-    {1169, 13,  10}, /* PR */
-    {1167, 13,  11}, /* POSTFIXNUMERIC */
-    {1160, 13,  11}, /* PO */
-    {1095, 13,  12}, /* OPENPUNCTUATION */
-    {1094, 13,  12}, /* OP */
-    { 413, 13,  13}, /* CLOSEPARENTHESIS */
-    { 456, 13,  13}, /* CP */
-    { 729, 13,  14}, /* INFIXNUMERIC */
-    { 744, 13,  14}, /* IS */
-    { 708, 13,  15}, /* HYPHEN */
-    { 707, 13,  15}, /* HY */
-    { 297, 13,  16}, /* BREAKSYMBOLS */
-    {1313, 13,  16}, /* SY */
-    {1063, 13,  17}, /* NUMERIC */
-    {1058, 13,  17}, /* NU */
-    { 414, 13,  18}, /* CLOSEPUNCTUATION */
-    { 411, 13,  18}, /* CL */
-    {1027, 13,  19}, /* NEXTLINE */
-    {1039, 13,  19}, /* NL */
-    { 631, 13,  20}, /* GLUE */
-    { 626, 13,  20}, /* GL */
-    { 193, 13,  21}, /* AMBIGUOUS */
-    { 179, 13,  21}, /* AI */
-    { 295, 13,  22}, /* BREAKBEFORE */
-    { 254, 13,  22}, /* BB */
-    { 688, 13,  23}, /* HEBREWLETTER */
-    { 699, 13,  23}, /* HL */
-    { 432, 13,  24}, /* COMPLEXCONTEXT */
-    {1217, 13,  24}, /* SA */
-    { 754, 13,  25}, /* JL */
-    { 762, 13,  26}, /* JV */
-    { 761, 13,  27}, /* JT */
-    {1049, 13,  28}, /* NONSTARTER */
-    {1054, 13,  28}, /* NS */
-    {1483, 13,  29}, /* ZWSPACE */
-    {1481, 13,  29}, /* ZW */
-    {1482, 13,  30}, /* ZWJ */
-    { 296, 13,  31}, /* BREAKBOTH */
-    { 241, 13,  31}, /* B2 */
-    { 738, 13,  32}, /* INSEPARABLE */
-    { 724, 13,  32}, /* IN */
-    { 739, 13,  32}, /* INSEPERABLE */
-    {1442, 13,  33}, /* WORDJOINER */
-    {1439, 13,  33}, /* WJ */
-    { 713, 13,  34}, /* IDEOGRAPHIC */
-    { 709, 13,  34}, /* ID */
-    { 537, 13,  35}, /* EBASE */
-    { 536, 13,  35}, /* EB */
-    { 433, 13,  36}, /* CONDITIONALJAPANESESTARTER */
-    { 379, 13,  36}, /* CJ */
-    { 658, 13,  37}, /* H2 */
-    { 659, 13,  38}, /* H3 */
-    {1310, 13,  39}, /* SURROGATE */
-    {1240, 13,  39}, /* SG */
-    { 448, 13,  40}, /* CONTINGENTBREAK */
-    { 322, 13,  40}, /* CB */
-    {1193, 13,  41}, /* REGIONALINDICATOR */
-    {1198, 13,  41}, /* RI */
-    { 550, 13,  42}, /* EMODIFIER */
-    { 548, 13,  42}, /* EM */
-    {1040, 14,   0}, /* NO */
-    {1007, 14,   0}, /* N */
-    {1458, 14,   1}, /* YES */
-    {1454, 14,   1}, /* Y */
-    { 946, 14,   2}, /* MAYBE */
-    { 883, 14,   2}, /* M */
-    {1040, 15,   0}, /* NO */
-    {1007, 15,   0}, /* N */
-    {1458, 15,   1}, /* YES */
-    {1454, 15,   1}, /* Y */
-    {1045, 16,   0}, /* NONE */
-    { 495, 16,   1}, /* DECIMAL */
-    { 494, 16,   1}, /* DE */
-    { 516, 16,   2}, /* DIGIT */
-    { 508, 16,   2}, /* DI */
-    {1063, 16,   3}, /* NUMERIC */
-    {1058, 16,   3}, /* NU */
-    {1013, 17,   0}, /* NAN */
-    {   1, 17,   1}, /* 0 */
-    {   2, 17,   2}, /* 1 */
-    {  53, 17,   3}, /* 2 */
-    {  86, 17,   4}, /* 3 */
-    { 109, 17,   5}, /* 4 */
-    { 126, 17,   6}, /* 5 */
-    { 136, 17,   7}, /* 6 */
-    { 142, 17,   8}, /* 7 */
-    { 151, 17,   9}, /* 8 */
-    { 158, 17,  10}, /* 9 */
-    {  12, 17,  11}, /* 1/4 */
-    {   7, 17,  12}, /* 1/2 */
-    {  90, 17,  13}, /* 3/4 */
-    {   5, 17,  14}, /* 1/16 */
-    {  18, 17,  15}, /* 1/8 */
-    {  87, 17,  16}, /* 3/16 */
-    {  48, 17,  17}, /* 16 */
-    {  21, 17,  18}, /* 10 */
-    {  22, 17,  19}, /* 100 */
-    {  23, 17,  20}, /* 1000 */
-    {   6, 17,  21}, /* 1/160 */
-    {  13, 17,  22}, /* 1/40 */
-    {  94, 17,  23}, /* 3/80 */
-    {   8, 17,  24}, /* 1/20 */
-    {   3, 17,  25}, /* 1/10 */
-    {  89, 17,  26}, /* 3/20 */
-    {  14, 17,  27}, /* 1/5 */
-    {  88, 17,  28}, /* 3/2 */
-    { 128, 17,  29}, /* 5/2 */
-    { 144, 17,  30}, /* 7/2 */
-    { 159, 17,  31}, /* 9/2 */
-    {  35, 17,  32}, /* 11/2 */
-    {  41, 17,  33}, /* 13/2 */
-    {  47, 17,  34}, /* 15/2 */
-    {  50, 17,  35}, /* 17/2 */
-    {   0, 17,  36}, /* -1/2 */
-    {  56, 17,  37}, /* 20 */
-    {  95, 17,  38}, /* 30 */
-    { 111, 17,  39}, /* 40 */
-    { 131, 17,  40}, /* 50 */
-    { 137, 17,  41}, /* 60 */
-    { 146, 17,  42}, /* 70 */
-    { 152, 17,  43}, /* 80 */
-    { 160, 17,  44}, /* 90 */
-    {  24, 17,  45}, /* 10000 */
-    {  49, 17,  46}, /* 17 */
-    {  51, 17,  47}, /* 18 */
-    {  52, 17,  48}, /* 19 */
-    {  17, 17,  49}, /* 1/7 */
-    {  20, 17,  50}, /* 1/9 */
-    {   9, 17,  51}, /* 1/3 */
-    {  54, 17,  52}, /* 2/3 */
-    {  55, 17,  53}, /* 2/5 */
-    {  91, 17,  54}, /* 3/5 */
-    { 110, 17,  55}, /* 4/5 */
-    {  15, 17,  56}, /* 1/6 */
-    { 129, 17,  57}, /* 5/6 */
-    {  93, 17,  58}, /* 3/8 */
-    { 130, 17,  59}, /* 5/8 */
-    { 145, 17,  60}, /* 7/8 */
-    {  33, 17,  61}, /* 11 */
-    {  37, 17,  62}, /* 12 */
-    { 132, 17,  63}, /* 500 */
-    { 133, 17,  64}, /* 5000 */
-    { 134, 17,  65}, /* 50000 */
-    {  25, 17,  66}, /* 100000 */
-    {  40, 17,  67}, /* 13 */
-    {  45, 17,  68}, /* 14 */
-    {  46, 17,  69}, /* 15 */
-    {  63, 17,  70}, /* 21 */
-    {  68, 17,  71}, /* 22 */
-    {  74, 17,  72}, /* 23 */
-    {  79, 17,  73}, /* 24 */
-    {  81, 17,  74}, /* 25 */
-    {  82, 17,  75}, /* 26 */
-    {  83, 17,  76}, /* 27 */
-    {  84, 17,  77}, /* 28 */
-    {  85, 17,  78}, /* 29 */
-    { 100, 17,  79}, /* 31 */
-    { 101, 17,  80}, /* 32 */
-    { 102, 17,  81}, /* 33 */
-    { 103, 17,  82}, /* 34 */
-    { 104, 17,  83}, /* 35 */
-    { 105, 17,  84}, /* 36 */
-    { 106, 17,  85}, /* 37 */
-    { 107, 17,  86}, /* 38 */
-    { 108, 17,  87}, /* 39 */
-    { 116, 17,  88}, /* 41 */
-    { 117, 17,  89}, /* 42 */
-    { 118, 17,  90}, /* 43 */
-    { 120, 17,  91}, /* 44 */
-    { 121, 17,  92}, /* 45 */
-    { 122, 17,  93}, /* 46 */
-    { 123, 17,  94}, /* 47 */
-    { 124, 17,  95}, /* 48 */
-    { 125, 17,  96}, /* 49 */
-    {  28, 17,  97}, /* 100000000 */
-    {  30, 17,  98}, /* 1000000000000 */
-    {  57, 17,  99}, /* 200 */
-    {  96, 17, 100}, /* 300 */
-    { 112, 17, 101}, /* 400 */
-    { 138, 17, 102}, /* 600 */
-    { 147, 17, 103}, /* 700 */
-    { 153, 17, 104}, /* 800 */
-    { 161, 17, 105}, /* 900 */
-    {  58, 17, 106}, /* 2000 */
-    {  97, 17, 107}, /* 3000 */
-    { 113, 17, 108}, /* 4000 */
-    { 139, 17, 109}, /* 6000 */
-    { 148, 17, 110}, /* 7000 */
-    { 154, 17, 111}, /* 8000 */
-    { 162, 17, 112}, /* 9000 */
-    {  59, 17, 113}, /* 20000 */
-    {  98, 17, 114}, /* 30000 */
-    { 114, 17, 115}, /* 40000 */
-    { 140, 17, 116}, /* 60000 */
-    { 149, 17, 117}, /* 70000 */
-    { 155, 17, 118}, /* 80000 */
-    { 163, 17, 119}, /* 90000 */
-    {  34, 17, 120}, /* 11/12 */
-    {  60, 17, 121}, /* 200000 */
-    {  99, 17, 122}, /* 300000 */
-    { 115, 17, 123}, /* 400000 */
-    { 135, 17, 124}, /* 500000 */
-    { 141, 17, 125}, /* 600000 */
-    { 150, 17, 126}, /* 700000 */
-    { 156, 17, 127}, /* 800000 */
-    { 164, 17, 128}, /* 900000 */
-    {   4, 17, 129}, /* 1/12 */
-    { 127, 17, 130}, /* 5/12 */
-    { 143, 17, 131}, /* 7/12 */
-    {  11, 17, 132}, /* 1/320 */
-    {  19, 17, 133}, /* 1/80 */
-    {  16, 17, 134}, /* 1/64 */
-    {  10, 17, 135}, /* 1/32 */
-    {  92, 17, 136}, /* 3/64 */
-    {  66, 17, 137}, /* 216000 */
-    { 119, 17, 138}, /* 432000 */
-    {  26, 17, 139}, /* 1000000 */
-    {  29, 17, 140}, /* 10000000000 */
-    {  27, 17, 141}, /* 10000000 */
-    {  61, 17, 142}, /* 20000000 */
-    {1400, 18,   0}, /* UNKNOWN */
-    {1485, 18,   0}, /* ZZZZ */
-    { 427, 18,   1}, /* COMMON */
-    {1484, 18,   1}, /* ZYYY */
-    { 809, 18,   2}, /* LATIN */
-    { 829, 18,   2}, /* LATN */
-    { 279, 18,   3}, /* BOPOMOFO */
-    { 278, 18,   3}, /* BOPO */
-    { 730, 18,   4}, /* INHERITED */
-    {1475, 18,   4}, /* ZINH */
-    {1184, 18,   4}, /* QAAI */
-    { 645, 18,   5}, /* GREEK */
-    { 649, 18,   5}, /* GREK */
-    { 452, 18,   6}, /* COPTIC */
-    { 451, 18,   6}, /* COPT */
-    {1183, 18,   6}, /* QAAC */
-    { 474, 18,   7}, /* CYRILLIC */
-    { 486, 18,   7}, /* CYRL */
-    { 220, 18,   8}, /* ARMENIAN */
-    { 222, 18,   8}, /* ARMN */
-    { 687, 18,   9}, /* HEBREW */
-    { 686, 18,   9}, /* HEBR */
-    { 203, 18,  10}, /* ARABIC */
-    { 202, 18,  10}, /* ARAB */
-    {1322, 18,  11}, /* SYRIAC */
-    {1321, 18,  11}, /* SYRC */
-    {1363, 18,  12}, /* THAANA */
-    {1362, 18,  12}, /* THAA */
-    {1037, 18,  13}, /* NKO */
-    {1038, 18,  13}, /* NKOO */
-    {1220, 18,  14}, /* SAMARITAN */
-    {1221, 18,  14}, /* SAMR */
-    { 904, 18,  15}, /* MANDAIC */
-    { 903, 18,  15}, /* MAND */
-    { 503, 18,  16}, /* DEVANAGARI */
-    { 502, 18,  16}, /* DEVA */
-    { 261, 18,  17}, /* BENGALI */
-    { 260, 18,  17}, /* BENG */
-    { 655, 18,  18}, /* GURMUKHI */
-    { 656, 18,  18}, /* GURU */
-    { 652, 18,  19}, /* GUJARATI */
-    { 653, 18,  19}, /* GUJR */
-    {1097, 18,  20}, /* ORIYA */
-    {1100, 18,  20}, /* ORYA */
-    {1341, 18,  21}, /* TAMIL */
-    {1344, 18,  21}, /* TAML */
-    {1356, 18,  22}, /* TELUGU */
-    {1355, 18,  22}, /* TELU */
-    { 779, 18,  23}, /* KANNADA */
-    { 798, 18,  23}, /* KNDA */
-    { 891, 18,  24}, /* MALAYALAM */
-    { 982, 18,  24}, /* MLYM */
-    {1254, 18,  25}, /* SINHALA */
-    {1253, 18,  25}, /* SINH */
-    {1364, 18,  26}, /* THAI */
-    { 807, 18,  27}, /* LAO */
-    { 808, 18,  27}, /* LAOO */
-    {1366, 18,  28}, /* TIBETAN */
-    {1367, 18,  28}, /* TIBT */
-    {1001, 18,  29}, /* MYANMAR */
-    {1006, 18,  29}, /* MYMR */
-    { 621, 18,  30}, /* GEORGIAN */
-    { 620, 18,  30}, /* GEOR */
-    { 668, 18,  31}, /* HANGUL */
-    { 667, 18,  31}, /* HANG */
-    { 572, 18,  32}, /* ETHIOPIC */
-    { 571, 18,  32}, /* ETHI */
-    { 371, 18,  33}, /* CHEROKEE */
-    { 370, 18,  33}, /* CHER */
-    { 309, 18,  34}, /* CANADIANABORIGINAL */
-    { 313, 18,  34}, /* CANS */
-    {1075, 18,  35}, /* OGHAM */
-    {1074, 18,  35}, /* OGAM */
-    {1213, 18,  36}, /* RUNIC */
-    {1214, 18,  36}, /* RUNR */
-    {1327, 18,  37}, /* TAGALOG */
-    {1361, 18,  37}, /* TGLG */
-    { 682, 18,  38}, /* HANUNOO */
-    { 679, 18,  38}, /* HANO */
-    { 301, 18,  39}, /* BUHID */
-    { 300, 18,  39}, /* BUHD */
-    {1329, 18,  40}, /* TAGBANWA */
-    {1328, 18,  40}, /* TAGB */
-    { 791, 18,  41}, /* KHMER */
-    { 793, 18,  41}, /* KHMR */
-    { 991, 18,  42}, /* MONGOLIAN */
-    { 990, 18,  42}, /* MONG */
-    { 848, 18,  43}, /* LIMBU */
-    { 847, 18,  43}, /* LIMB */
-    {1332, 18,  44}, /* TAILE */
-    {1339, 18,  44}, /* TALE */
-    {1026, 18,  45}, /* NEWTAILUE */
-    {1340, 18,  45}, /* TALU */
-    { 299, 18,  46}, /* BUGINESE */
-    { 298, 18,  46}, /* BUGI */
-    {1333, 18,  47}, /* TAITHAM */
-    { 806, 18,  47}, /* LANA */
-    { 244, 18,  48}, /* BALINESE */
-    { 243, 18,  48}, /* BALI */
-    {1287, 18,  49}, /* SUNDANESE */
-    {1286, 18,  49}, /* SUND */
-    { 252, 18,  50}, /* BATAK */
-    { 253, 18,  50}, /* BATK */
-    { 842, 18,  51}, /* LEPCHA */
-    { 841, 18,  51}, /* LEPC */
-    {1079, 18,  52}, /* OLCHIKI */
-    {1080, 18,  52}, /* OLCK */
-    { 292, 18,  53}, /* BRAILLE */
-    { 291, 18,  53}, /* BRAI */
-    { 628, 18,  54}, /* GLAGOLITIC */
-    { 627, 18,  54}, /* GLAG */
-    {1368, 18,  55}, /* TIFINAGH */
-    {1360, 18,  55}, /* TFNG */
-    { 666, 18,  56}, /* HAN */
-    { 675, 18,  56}, /* HANI */
-    { 698, 18,  57}, /* HIRAGANA */
-    { 697, 18,  57}, /* HIRA */
-    { 781, 18,  58}, /* KATAKANA */
-    { 768, 18,  58}, /* KANA */
-    {1461, 18,  59}, /* YI */
-    {1462, 18,  59}, /* YIII */
-    { 858, 18,  60}, /* LISU */
-    {1406, 18,  61}, /* VAI */
-    {1407, 18,  61}, /* VAII */
-    { 246, 18,  62}, /* BAMUM */
-    { 245, 18,  62}, /* BAMU */
-    {1316, 18,  63}, /* SYLOTINAGRI */
-    {1315, 18,  63}, /* SYLO */
-    {1146, 18,  64}, /* PHAGSPA */
-    {1145, 18,  64}, /* PHAG */
-    {1224, 18,  65}, /* SAURASHTRA */
-    {1223, 18,  65}, /* SAUR */
-    { 786, 18,  66}, /* KAYAHLI */
-    { 767, 18,  66}, /* KALI */
-    {1196, 18,  67}, /* REJANG */
-    {1205, 18,  67}, /* RJNG */
-    { 752, 18,  68}, /* JAVANESE */
-    { 751, 18,  68}, /* JAVA */
-    { 364, 18,  69}, /* CHAM */
-    {1334, 18,  70}, /* TAIVIET */
-    {1351, 18,  70}, /* TAVT */
-    { 955, 18,  71}, /* MEETEIMAYEK */
-    { 996, 18,  71}, /* MTEI */
-    { 852, 18,  72}, /* LINEARB */
-    { 850, 18,  72}, /* LINB */
-    { 880, 18,  73}, /* LYCIAN */
-    { 879, 18,  73}, /* LYCI */
-    { 316, 18,  74}, /* CARIAN */
-    { 315, 18,  74}, /* CARI */
-    {1082, 18,  75}, /* OLDITALIC */
-    { 747, 18,  75}, /* ITAL */
-    { 636, 18,  76}, /* GOTHIC */
-    { 635, 18,  76}, /* GOTH */
-    {1084, 18,  77}, /* OLDPERMIC */
-    {1143, 18,  77}, /* PERM */
-    {1393, 18,  78}, /* UGARITIC */
-    {1392, 18,  78}, /* UGAR */
-    {1085, 18,  79}, /* OLDPERSIAN */
-    {1451, 18,  79}, /* XPEO */
-    { 501, 18,  80}, /* DESERET */
-    { 527, 18,  80}, /* DSRT */
-    {1243, 18,  81}, /* SHAVIAN */
-    {1244, 18,  81}, /* SHAW */
-    {1104, 18,  82}, /* OSMANYA */
-    {1103, 18,  82}, /* OSMA */
-    {1101, 18,  83}, /* OSAGE */
-    {1102, 18,  83}, /* OSGE */
-    { 545, 18,  84}, /* ELBASAN */
-    { 544, 18,  84}, /* ELBA */
-    { 321, 18,  85}, /* CAUCASIANALBANIAN */
-    { 176, 18,  85}, /* AGHB */
-    {1422, 18,  86}, /* VITHKUQI */
-    {1421, 18,  86}, /* VITH */
-    { 851, 18,  87}, /* LINEARA */
-    { 849, 18,  87}, /* LINA */
-    { 471, 18,  88}, /* CYPRIOT */
-    { 458, 18,  88}, /* CPRT */
-    { 723, 18,  89}, /* IMPERIALARAMAIC */
-    { 221, 18,  89}, /* ARMI */
-    {1129, 18,  90}, /* PALMYRENE */
-    {1128, 18,  90}, /* PALM */
-    {1010, 18,  91}, /* NABATAEAN */
-    {1020, 18,  91}, /* NBAT */
-    { 684, 18,  92}, /* HATRAN */
-    { 683, 18,  92}, /* HATR */
-    {1152, 18,  93}, /* PHOENICIAN */
-    {1151, 18,  93}, /* PHNX */
-    { 882, 18,  94}, /* LYDIAN */
-    { 881, 18,  94}, /* LYDI */
-    { 963, 18,  95}, /* MEROITICHIEROGLYPHS */
-    { 961, 18,  95}, /* MERO */
-    { 962, 18,  96}, /* MEROITICCURSIVE */
-    { 960, 18,  96}, /* MERC */
-    { 789, 18,  97}, /* KHAROSHTHI */
-    { 788, 18,  97}, /* KHAR */
-    {1087, 18,  98}, /* OLDSOUTHARABIAN */
-    {1222, 18,  98}, /* SARB */
-    {1083, 18,  99}, /* OLDNORTHARABIAN */
-    {1017, 18,  99}, /* NARB */
-    { 907, 18, 100}, /* MANICHAEAN */
-    { 906, 18, 100}, /* MANI */
-    { 238, 18, 101}, /* AVESTAN */
-    { 239, 18, 101}, /* AVST */
-    { 737, 18, 102}, /* INSCRIPTIONALPARTHIAN */
-    {1176, 18, 102}, /* PRTI */
-    { 736, 18, 103}, /* INSCRIPTIONALPAHLAVI */
-    {1149, 18, 103}, /* PHLI */
-    {1178, 18, 104}, /* PSALTERPAHLAVI */
-    {1150, 18, 104}, /* PHLP */
-    {1088, 18, 105}, /* OLDTURKIC */
-    {1098, 18, 105}, /* ORKH */
-    {1081, 18, 106}, /* OLDHUNGARIAN */
-    { 706, 18, 106}, /* HUNG */
-    { 676, 18, 107}, /* HANIFIROHINGYA */
-    {1209, 18, 107}, /* ROHG */
-    {1460, 18, 108}, /* YEZIDI */
-    {1459, 18, 108}, /* YEZI */
-    {1086, 18, 109}, /* OLDSOGDIAN */
-    {1268, 18, 109}, /* SOGO */
-    {1267, 18, 110}, /* SOGDIAN */
-    {1266, 18, 110}, /* SOGD */
-    {1089, 18, 111}, /* OLDUYGHUR */
-    {1120, 18, 111}, /* OUGR */
-    { 375, 18, 112}, /* CHORASMIAN */
-    { 376, 18, 112}, /* CHRS */
-    { 547, 18, 113}, /* ELYMAIC */
-    { 546, 18, 113}, /* ELYM */
-    { 289, 18, 114}, /* BRAHMI */
-    { 288, 18, 114}, /* BRAH */
-    { 765, 18, 115}, /* KAITHI */
-    { 800, 18, 115}, /* KTHI */
-    {1270, 18, 116}, /* SORASOMPENG */
-    {1269, 18, 116}, /* SORA */
-    { 363, 18, 117}, /* CHAKMA */
-    { 307, 18, 117}, /* CAKM */
-    { 885, 18, 118}, /* MAHAJANI */
-    { 886, 18, 118}, /* MAHJ */
-    {1242, 18, 119}, /* SHARADA */
-    {1247, 18, 119}, /* SHRD */
-    { 795, 18, 120}, /* KHOJKI */
-    { 794, 18, 120}, /* KHOJ */
-    { 998, 18, 121}, /* MULTANI */
-    { 997, 18, 121}, /* MULT */
-    { 796, 18, 122}, /* KHUDAWADI */
-    {1251, 18, 122}, /* SIND */
-    { 638, 18, 123}, /* GRANTHA */
-    { 637, 18, 123}, /* GRAN */
-    {1024, 18, 124}, /* NEWA */
-    {1370, 18, 125}, /* TIRHUTA */
-    {1369, 18, 125}, /* TIRH */
-    {1249, 18, 126}, /* SIDDHAM */
-    {1248, 18, 126}, /* SIDD */
-    { 984, 18, 127}, /* MODI */
-    {1338, 18, 128}, /* TAKRI */
-    {1337, 18, 128}, /* TAKR */
-    { 178, 18, 129}, /* AHOM */
-    { 520, 18, 130}, /* DOGRA */
-    { 519, 18, 130}, /* DOGR */
-    {1433, 18, 131}, /* WARANGCITI */
-    {1432, 18, 131}, /* WARA */
-    { 518, 18, 132}, /* DIVESAKURU */
-    { 515, 18, 132}, /* DIAK */
-    {1015, 18, 133}, /* NANDINAGARI */
-    {1014, 18, 133}, /* NAND */
-    {1472, 18, 134}, /* ZANABAZARSQUARE */
-    {1473, 18, 134}, /* ZANB */
-    {1272, 18, 135}, /* SOYOMBO */
-    {1271, 18, 135}, /* SOYO */
-    {1136, 18, 136}, /* PAUCINHAU */
-    {1135, 18, 136}, /* PAUC */
-    { 263, 18, 137}, /* BHAIKSUKI */
-    { 264, 18, 137}, /* BHKS */
-    { 936, 18, 138}, /* MARCHEN */
-    { 935, 18, 138}, /* MARC */
-    { 938, 18, 139}, /* MASARAMGONDI */
-    { 634, 18, 139}, /* GONM */
-    { 654, 18, 140}, /* GUNJALAGONDI */
-    { 633, 18, 140}, /* GONG */
-    { 890, 18, 141}, /* MAKASAR */
-    { 889, 18, 141}, /* MAKA */
-    { 785, 18, 142}, /* KAWI */
-    { 461, 18, 143}, /* CUNEIFORM */
-    {1452, 18, 143}, /* XSUX */
-    { 473, 18, 144}, /* CYPROMINOAN */
-    { 457, 18, 144}, /* CPMN */
-    { 543, 18, 145}, /* EGYPTIANHIEROGLYPHS */
-    { 541, 18, 145}, /* EGYP */
-    { 195, 18, 146}, /* ANATOLIANHIEROGLYPHS */
-    { 700, 18, 146}, /* HLUW */
-    { 994, 18, 147}, /* MRO */
-    { 995, 18, 147}, /* MROO */
-    {1346, 18, 148}, /* TANGSA */
-    {1372, 18, 148}, /* TNSA */
-    { 251, 18, 149}, /* BASSAVAH */
-    { 250, 18, 149}, /* BASS */
-    {1127, 18, 150}, /* PAHAWHHMONG */
-    { 701, 18, 150}, /* HMNG */
-    { 951, 18, 151}, /* MEDEFAIDRIN */
-    { 952, 18, 151}, /* MEDF */
-    { 964, 18, 152}, /* MIAO */
-    {1159, 18, 152}, /* PLRD */
-    {1347, 18, 153}, /* TANGUT */
-    {1345, 18, 153}, /* TANG */
-    {1067, 18, 154}, /* NUSHU */
-    {1055, 18, 154}, /* NSHU */
-    { 790, 18, 155}, /* KHITANSMALLSCRIPT */
-    { 797, 18, 155}, /* KITS */
-    { 531, 18, 156}, /* DUPLOYAN */
-    { 530, 18, 156}, /* DUPL */
-    {1250, 18, 157}, /* SIGNWRITING */
-    {1241, 18, 157}, /* SGNW */
-    {1070, 18, 158}, /* NYIAKENGPUACHUEHMONG */
-    { 702, 18, 158}, /* HMNP */
-    {1382, 18, 159}, /* TOTO */
-    {1431, 18, 160}, /* WANCHO */
-    {1436, 18, 160}, /* WCHO */
-    {1012, 18, 161}, /* NAGMUNDARI */
-    {1011, 18, 161}, /* NAGM */
-    { 959, 18, 162}, /* MENDEKIKAKUI */
-    { 958, 18, 162}, /* MEND */
-    { 170, 18, 163}, /* ADLAM */
-    { 171, 18, 163}, /* ADLM */
-    { 783, 18, 164}, /* KATAKANAORHIRAGANA */
-    { 704, 18, 164}, /* HRKT */
-    {1105, 19,   0}, /* OTHER */
-    {1453, 19,   0}, /* XX */
-    {1273, 19,   1}, /* SP */
-    { 846, 19,   2}, /* LF */
-    { 459, 19,   3}, /* CR */
-    {1283, 19,   4}, /* STERM */
-    {1282, 19,   4}, /* ST */
-    { 412, 19,   5}, /* CLOSE */
-    { 411, 19,   5}, /* CL */
-    {1227, 19,   6}, /* SCONTINUE */
-    {1226, 19,   6}, /* SC */
-    { 232, 19,   7}, /* ATERM */
-    { 227, 19,   7}, /* AT */
-    {1063, 19,   8}, /* NUMERIC */
-    {1058, 19,   8}, /* NU */
-    {1402, 19,   9}, /* UPPER */
-    {1401, 19,   9}, /* UP */
-    { 866, 19,  10}, /* LOWER */
-    { 863, 19,  10}, /* LO */
-    {1238, 19,  11}, /* SEP */
-    {1232, 19,  11}, /* SE */
-    { 604, 19,  12}, /* FORMAT */
-    { 602, 19,  12}, /* FO */
-    {1090, 19,  13}, /* OLETTER */
-    { 832, 19,  13}, /* LE */
-    { 587, 19,  14}, /* EXTEND */
-    { 584, 19,  14}, /* EX */
-    {1105, 20,   0}, /* OTHER */
-    {1453, 20,   0}, /* XX */
-    { 846, 20,   1}, /* LF */
-    {1025, 20,   2}, /* NEWLINE */
-    {1039, 20,   2}, /* NL */
-    { 459, 20,   3}, /* CR */
-    {1444, 20,   4}, /* WSEGSPACE */
-    { 525, 20,   5}, /* DOUBLEQUOTE */
-    { 526, 20,   5}, /* DQ */
-    {1252, 20,   6}, /* SINGLEQUOTE */
-    {1279, 20,   6}, /* SQ */
-    { 966, 20,   7}, /* MIDNUM */
-    { 983, 20,   7}, /* MN */
-    { 967, 20,   8}, /* MIDNUMLET */
-    { 947, 20,   8}, /* MB */
-    {1063, 20,   9}, /* NUMERIC */
-    {1058, 20,   9}, /* NU */
-    { 965, 20,  10}, /* MIDLETTER */
-    { 981, 20,  10}, /* ML */
-    { 186, 20,  11}, /* ALETTER */
-    { 832, 20,  11}, /* LE */
-    { 590, 20,  12}, /* EXTENDNUMLET */
-    { 584, 20,  12}, /* EX */
-    { 604, 20,  13}, /* FORMAT */
-    { 602, 20,  13}, /* FO */
-    { 587, 20,  14}, /* EXTEND */
-    { 688, 20,  15}, /* HEBREWLETTER */
-    { 699, 20,  15}, /* HL */
-    {1482, 20,  16}, /* ZWJ */
-    { 781, 20,  17}, /* KATAKANA */
-    { 763, 20,  17}, /* KA */
-    {1193, 20,  18}, /* REGIONALINDICATOR */
-    {1198, 20,  18}, /* RI */
-    { 537, 20,  19}, /* EBASE */
-    { 536, 20,  19}, /* EB */
-    { 538, 20,  20}, /* EBASEGAZ */
-    { 539, 20,  20}, /* EBG */
-    { 550, 20,  21}, /* EMODIFIER */
-    { 548, 20,  21}, /* EM */
-    { 632, 20,  22}, /* GLUEAFTERZWJ */
-    { 611, 20,  22}, /* GAZ */
+    { 336,  3,  13}, /* CCC11 */
+    {  35,  3,  13}, /* 11 */
+    { 338,  3,  14}, /* CCC12 */
+    {  39,  3,  14}, /* 12 */
+    { 341,  3,  15}, /* CCC13 */
+    {  42,  3,  15}, /* 13 */
+    { 345,  3,  16}, /* CCC14 */
+    {  47,  3,  16}, /* 14 */
+    { 346,  3,  17}, /* CCC15 */
+    {  48,  3,  17}, /* 15 */
+    { 347,  3,  18}, /* CCC16 */
+    {  50,  3,  18}, /* 16 */
+    { 348,  3,  19}, /* CCC17 */
+    {  51,  3,  19}, /* 17 */
+    { 349,  3,  20}, /* CCC18 */
+    {  53,  3,  20}, /* 18 */
+    { 350,  3,  21}, /* CCC19 */
+    {  54,  3,  21}, /* 19 */
+    { 351,  3,  22}, /* CCC20 */
+    {  58,  3,  22}, /* 20 */
+    { 352,  3,  23}, /* CCC21 */
+    {  65,  3,  23}, /* 21 */
+    { 353,  3,  24}, /* CCC22 */
+    {  70,  3,  24}, /* 22 */
+    { 354,  3,  25}, /* CCC23 */
+    {  76,  3,  25}, /* 23 */
+    { 355,  3,  26}, /* CCC24 */
+    {  81,  3,  26}, /* 24 */
+    { 356,  3,  27}, /* CCC25 */
+    {  83,  3,  27}, /* 25 */
+    { 361,  3,  28}, /* CCC30 */
+    {  97,  3,  28}, /* 30 */
+    { 362,  3,  29}, /* CCC31 */
+    { 102,  3,  29}, /* 31 */
+    { 363,  3,  30}, /* CCC32 */
+    { 103,  3,  30}, /* 32 */
+    { 358,  3,  31}, /* CCC27 */
+    {  85,  3,  31}, /* 27 */
+    { 359,  3,  32}, /* CCC28 */
+    {  86,  3,  32}, /* 28 */
+    { 360,  3,  33}, /* CCC29 */
+    {  87,  3,  33}, /* 29 */
+    { 364,  3,  34}, /* CCC33 */
+    { 104,  3,  34}, /* 33 */
+    { 365,  3,  35}, /* CCC34 */
+    { 105,  3,  35}, /* 34 */
+    { 366,  3,  36}, /* CCC35 */
+    { 106,  3,  36}, /* 35 */
+    { 367,  3,  37}, /* CCC36 */
+    { 107,  3,  37}, /* 36 */
+    {1076,  3,  38}, /* NUKTA */
+    { 144,  3,  38}, /* 7 */
+    {1053,  3,  38}, /* NK */
+    {1437,  3,  39}, /* VIRAMA */
+    { 160,  3,  39}, /* 9 */
+    {1447,  3,  39}, /* VR */
+    { 368,  3,  40}, /* CCC84 */
+    { 159,  3,  40}, /* 84 */
+    { 369,  3,  41}, /* CCC91 */
+    { 167,  3,  41}, /* 91 */
+    { 334,  3,  42}, /* CCC103 */
+    {  33,  3,  42}, /* 103 */
+    { 335,  3,  43}, /* CCC107 */
+    {  34,  3,  43}, /* 107 */
+    { 337,  3,  44}, /* CCC118 */
+    {  38,  3,  44}, /* 118 */
+    { 339,  3,  45}, /* CCC122 */
+    {  40,  3,  45}, /* 122 */
+    { 340,  3,  46}, /* CCC129 */
+    {  41,  3,  46}, /* 129 */
+    { 342,  3,  47}, /* CCC130 */
+    {  44,  3,  47}, /* 130 */
+    { 343,  3,  48}, /* CCC132 */
+    {  45,  3,  48}, /* 132 */
+    { 241,  3,  49}, /* ATTACHEDABOVE */
+    {  66,  3,  49}, /* 214 */
+    { 236,  3,  49}, /* ATA */
+    { 266,  3,  50}, /* BELOWLEFT */
+    {  69,  3,  50}, /* 218 */
+    { 280,  3,  50}, /* BL */
+    { 850,  3,  51}, /* LEFT */
+    {  73,  3,  51}, /* 224 */
+    { 818,  3,  51}, /* L */
+    { 791,  3,  52}, /* KANAVOICING */
+    { 153,  3,  52}, /* 8 */
+    { 817,  3,  52}, /* KV */
+    { 357,  3,  53}, /* CCC26 */
+    {  84,  3,  53}, /* 26 */
+    { 691,  3,  54}, /* HANREADING */
+    { 138,  3,  54}, /* 6 */
+    { 690,  3,  54}, /* HANR */
+    {1216,  3,  55}, /* RIGHT */
+    {  74,  3,  55}, /* 226 */
+    {1208,  3,  55}, /* R */
+    { 344,  3,  56}, /* CCC133 */
+    {  46,  3,  56}, /* 133 */
+    { 244,  3,  57}, /* ATTACHEDBELOWLEFT */
+    {  59,  3,  57}, /* 200 */
+    { 239,  3,  57}, /* ATBL */
+    {1062,  4,   0}, /* NONE */
+    {1059,  4,   1}, /* NOBREAK */
+    {1036,  4,   1}, /* NB */
+    { 440,  4,   2}, /* COMPAT */
+    { 429,  4,   2}, /* COM */
+    {1311,  4,   3}, /* SUPER */
+    {1307,  4,   3}, /* SUP */
+    { 616,  4,   4}, /* FRACTION */
+    { 615,  4,   4}, /* FRA */
+    { 319,  4,   5}, /* CANONICAL */
+    { 316,  4,   5}, /* CAN */
+    {1302,  4,   6}, /* SUB */
+    { 613,  4,   7}, /* FONT */
+    { 386,  4,   8}, /* CIRCLE */
+    { 568,  4,   8}, /* ENC */
+    {1458,  4,   9}, /* WIDE */
+    {1431,  4,  10}, /* VERTICAL */
+    {1430,  4,  10}, /* VERT */
+    {1298,  4,  11}, /* SQUARE */
+    {1297,  4,  11}, /* SQR */
+    { 762,  4,  12}, /* ISOLATED */
+    { 761,  4,  12}, /* ISO */
+    { 608,  4,  13}, /* FINAL */
+    { 607,  4,  13}, /* FIN */
+    { 748,  4,  14}, /* INITIAL */
+    { 747,  4,  14}, /* INIT */
+    { 970,  4,  15}, /* MEDIAL */
+    { 967,  4,  15}, /* MED */
+    {1275,  4,  16}, /* SMALL */
+    {1280,  4,  16}, /* SML */
+    {1035,  4,  17}, /* NARROW */
+    {1033,  4,  17}, /* NAR */
+    {1458,  5,   0}, /* WIDE */
+    {1450,  5,   0}, /* W */
+    {1040,  5,   1}, /* NEUTRAL */
+    {1024,  5,   1}, /* N */
+    {1035,  5,   2}, /* NARROW */
+    {1026,  5,   2}, /* NA */
+    { 199,  5,   3}, /* AMBIGUOUS */
+    { 168,  5,   3}, /* A */
+    { 673,  5,   4}, /* HALFWIDTH */
+    { 667,  5,   4}, /* H */
+    { 618,  5,   5}, /* FULLWIDTH */
+    { 602,  5,   5}, /* F */
+    {1412,  6,   0}, /* UNASSIGNED */
+    { 426,  6,   0}, /* CN */
+    { 459,  6,   1}, /* CONTROL */
+    { 331,  6,   1}, /* CC */
+    { 427,  6,   1}, /* CNTRL */
+    {1292,  6,   2}, /* SPACESEPARATOR */
+    {1500,  6,   2}, /* ZS */
+    {1133,  6,   3}, /* OTHERPUNCTUATION */
+    {1177,  6,   3}, /* PO */
+    { 474,  6,   4}, /* CURRENCYSYMBOL */
+    {1243,  6,   4}, /* SC */
+    {1112,  6,   5}, /* OPENPUNCTUATION */
+    {1194,  6,   5}, /* PS */
+    { 424,  6,   6}, /* CLOSEPUNCTUATION */
+    {1159,  6,   6}, /* PE */
+    { 961,  6,   7}, /* MATHSYMBOL */
+    {1274,  6,   7}, /* SM */
+    { 502,  6,   8}, /* DASHPUNCTUATION */
+    {1156,  6,   8}, /* PD */
+    { 506,  6,   9}, /* DECIMALNUMBER */
+    {1039,  6,   9}, /* ND */
+    { 526,  6,   9}, /* DIGIT */
+    {1421,  6,  10}, /* UPPERCASELETTER */
+    { 891,  6,  10}, /* LU */
+    {1004,  6,  11}, /* MODIFIERSYMBOL */
+    {1273,  6,  11}, /* SK */
+    { 444,  6,  12}, /* CONNECTORPUNCTUATION */
+    {1154,  6,  12}, /* PC */
+    { 885,  6,  13}, /* LOWERCASELETTER */
+    { 878,  6,  13}, /* LL */
+    {1134,  6,  14}, /* OTHERSYMBOL */
+    {1281,  6,  14}, /* SO */
+    {1128,  6,  15}, /* OTHERLETTER */
+    { 880,  6,  15}, /* LO */
+    { 749,  6,  16}, /* INITIALPUNCTUATION */
+    {1174,  6,  16}, /* PI */
+    { 614,  6,  17}, /* FORMAT */
+    { 370,  6,  17}, /* CF */
+    {1132,  6,  18}, /* OTHERNUMBER */
+    {1057,  6,  18}, /* NO */
+    { 609,  6,  19}, /* FINALPUNCTUATION */
+    {1161,  6,  19}, /* PF */
+    {1388,  6,  20}, /* TITLECASELETTER */
+    { 890,  6,  20}, /* LT */
+    {1002,  6,  21}, /* MODIFIERLETTER */
+    { 879,  6,  21}, /* LM */
+    {1065,  6,  22}, /* NONSPACINGMARK */
+    {1000,  6,  22}, /* MN */
+    { 577,  6,  23}, /* ENCLOSINGMARK */
+    { 966,  6,  23}, /* ME */
+    {1293,  6,  24}, /* SPACINGMARK */
+    { 965,  6,  24}, /* MC */
+    { 861,  6,  25}, /* LETTERNUMBER */
+    {1056,  6,  25}, /* NL */
+    { 873,  6,  26}, /* LINESEPARATOR */
+    {1496,  6,  26}, /* ZL */
+    {1147,  6,  27}, /* PARAGRAPHSEPARATOR */
+    {1499,  6,  27}, /* ZP */
+    {1327,  6,  28}, /* SURROGATE */
+    { 470,  6,  28}, /* CS */
+    {1191,  6,  29}, /* PRIVATEUSE */
+    { 428,  6,  29}, /* CO */
+    {1122,  6,  30}, /* OTHER */
+    { 313,  6,  30}, /* C */
+    { 314,  6,  30}, /* C& */
+    { 859,  6,  31}, /* LETTER */
+    { 818,  6,  31}, /* L */
+    { 819,  6,  31}, /* L& */
+    { 954,  6,  32}, /* MARK */
+    { 900,  6,  32}, /* M */
+    { 435,  6,  32}, /* COMBININGMARK */
+    { 901,  6,  32}, /* M& */
+    {1077,  6,  33}, /* NUMBER */
+    {1024,  6,  33}, /* N */
+    {1025,  6,  33}, /* N& */
+    {1198,  6,  34}, /* PUNCTUATION */
+    {1142,  6,  34}, /* P */
+    {1197,  6,  34}, /* PUNCT */
+    {1143,  6,  34}, /* P& */
+    {1334,  6,  35}, /* SYMBOL */
+    {1232,  6,  35}, /* S */
+    {1233,  6,  35}, /* S& */
+    {1256,  6,  36}, /* SEPARATOR */
+    {1489,  6,  36}, /* Z */
+    {1490,  6,  36}, /* Z& */
+    { 234,  6,  37}, /* ASSIGNED */
+    { 327,  6,  38}, /* CASEDLETTER */
+    { 847,  6,  38}, /* LC */
+    {1122,  7,   0}, /* OTHER */
+    {1473,  7,   0}, /* XX */
+    { 459,  7,   1}, /* CONTROL */
+    { 426,  7,   1}, /* CN */
+    { 862,  7,   2}, /* LF */
+    { 469,  7,   3}, /* CR */
+    { 597,  7,   4}, /* EXTEND */
+    { 594,  7,   4}, /* EX */
+    {1188,  7,   5}, /* PREPEND */
+    {1185,  7,   5}, /* PP */
+    {1293,  7,   6}, /* SPACINGMARK */
+    {1274,  7,   6}, /* SM */
+    { 818,  7,   7}, /* L */
+    {1422,  7,   8}, /* V */
+    {1343,  7,   9}, /* T */
+    {1502,  7,  10}, /* ZWJ */
+    { 892,  7,  11}, /* LV */
+    { 894,  7,  12}, /* LVT */
+    {1210,  7,  13}, /* REGIONALINDICATOR */
+    {1215,  7,  13}, /* RI */
+    { 547,  7,  14}, /* EBASE */
+    { 546,  7,  14}, /* EB */
+    { 548,  7,  15}, /* EBASEGAZ */
+    { 549,  7,  15}, /* EBG */
+    { 560,  7,  16}, /* EMODIFIER */
+    { 558,  7,  16}, /* EM */
+    { 642,  7,  17}, /* GLUEAFTERZWJ */
+    { 621,  7,  17}, /* GAZ */
+    {1068,  8,   0}, /* NOTAPPLICABLE */
+    {1026,  8,   0}, /* NA */
+    { 849,  8,   1}, /* LEADINGJAMO */
+    { 818,  8,   1}, /* L */
+    {1446,  8,   2}, /* VOWELJAMO */
+    {1422,  8,   2}, /* V */
+    {1400,  8,   3}, /* TRAILINGJAMO */
+    {1343,  8,   3}, /* T */
+    { 893,  8,   4}, /* LVSYLLABLE */
+    { 892,  8,   4}, /* LV */
+    { 895,  8,   5}, /* LVTSYLLABLE */
+    { 894,  8,   5}, /* LVT */
+    {1062,  9,   0}, /* NONE */
+    { 597,  9,   1}, /* EXTEND */
+    { 445,  9,   2}, /* CONSONANT */
+    { 874,  9,   3}, /* LINKER */
+    {1026, 10,   0}, /* NA */
+    {1392, 10,   1}, /* TOP */
+    {1216, 10,   2}, /* RIGHT */
+    { 290, 10,   3}, /* BOTTOM */
+    { 850, 10,   4}, /* LEFT */
+    { 851, 10,   5}, /* LEFTANDRIGHT */
+    {1398, 10,   6}, /* TOPANDRIGHT */
+    {1396, 10,   7}, /* TOPANDLEFT */
+    {1397, 10,   8}, /* TOPANDLEFTANDRIGHT */
+    {1393, 10,   9}, /* TOPANDBOTTOM */
+    {1440, 10,  10}, /* VISUALORDERLEFT */
+    {1394, 10,  11}, /* TOPANDBOTTOMANDLEFT */
+    { 292, 10,  12}, /* BOTTOMANDRIGHT */
+    {1395, 10,  13}, /* TOPANDBOTTOMANDRIGHT */
+    {1141, 10,  14}, /* OVERSTRUCK */
+    { 291, 10,  15}, /* BOTTOMANDLEFT */
+    {1122, 11,   0}, /* OTHER */
+    { 452, 11,   1}, /* CONSONANTPLACEHOLDER */
+    {1077, 11,   2}, /* NUMBER */
+    {1331, 11,   3}, /* SYLLABLEMODIFIER */
+    { 278, 11,   4}, /* BINDU */
+    {1439, 11,   5}, /* VISARGA */
+    {1445, 11,   6}, /* VOWELINDEPENDENT */
+    { 445, 11,   7}, /* CONSONANT */
+    {1444, 11,   8}, /* VOWELDEPENDENT */
+    {1076, 11,   9}, /* NUKTA */
+    { 245, 11,  10}, /* AVAGRAHA */
+    {1437, 11,  11}, /* VIRAMA */
+    { 322, 11,  12}, /* CANTILLATIONMARK */
+    { 446, 11,  13}, /* CONSONANTDEAD */
+    { 624, 11,  14}, /* GEMINATIONMARK */
+    { 451, 11,  15}, /* CONSONANTMEDIAL */
+    {1006, 11,  16}, /* MODIFYINGLETTER */
+    { 457, 11,  17}, /* CONSONANTWITHSTACKER */
+    {1199, 11,  18}, /* PUREKILLER */
+    { 453, 11,  19}, /* CONSONANTPRECEDINGREPHA */
+    {1391, 11,  20}, /* TONEMARK */
+    { 450, 11,  21}, /* CONSONANTKILLER */
+    { 448, 11,  22}, /* CONSONANTHEADLETTER */
+    { 455, 11,  23}, /* CONSONANTSUBJOINED */
+    { 756, 11,  24}, /* INVISIBLESTACKER */
+    {1211, 11,  25}, /* REGISTERSHIFTER */
+    { 456, 11,  26}, /* CONSONANTSUCCEEDINGREPHA */
+    { 447, 11,  27}, /* CONSONANTFINAL */
+    {1443, 11,  28}, /* VOWEL */
+    {1390, 11,  29}, /* TONELETTER */
+    { 449, 11,  30}, /* CONSONANTINITIALPOSTFIXED */
+    {1063, 11,  31}, /* NONJOINER */
+    { 774, 11,  32}, /* JOINER */
+    { 298, 11,  33}, /* BRAHMIJOININGNUMBER */
+    {1079, 11,  34}, /* NUMBERJOINER */
+    { 454, 11,  35}, /* CONSONANTPREFIXED */
+    {1060, 12,   0}, /* NOJOININGGROUP */
+    {1475, 12,   1}, /* YEH */
+    { 191, 12,   2}, /* ALEF */
+    {1454, 12,   3}, /* WAW */
+    { 264, 12,   4}, /* BEH */
+    {1370, 12,   5}, /* TEHMARBUTA */
+    { 670, 12,   6}, /* HAH */
+    { 499, 12,   7}, /* DAL */
+    {1212, 12,   8}, /* REH */
+    {1250, 12,   9}, /* SEEN */
+    {1235, 12,  10}, /* SAD */
+    {1348, 12,  11}, /* TAH */
+    { 182, 12,  12}, /* AIN */
+    { 619, 12,  13}, /* GAF */
+    { 604, 12,  14}, /* FARSIYEH */
+    { 606, 12,  15}, /* FEH */
+    {1202, 12,  16}, /* QAF */
+    { 780, 12,  17}, /* KAF */
+    { 820, 12,  18}, /* LAM */
+    { 971, 12,  19}, /* MEEM */
+    {1067, 12,  20}, /* NOON */
+    { 699, 12,  21}, /* HEH */
+    {1329, 12,  22}, /* SWASHKAF */
+    {1086, 12,  23}, /* NYA */
+    { 815, 12,  24}, /* KNOTTEDHEH */
+    { 700, 12,  25}, /* HEHGOAL */
+    { 675, 12,  26}, /* HAMZAONHEHGOAL */
+    {1371, 12,  26}, /* TEHMARBUTAGOAL */
+    {1477, 12,  27}, /* YEHWITHTAIL */
+    {1476, 12,  28}, /* YEHBARREE */
+    { 188, 12,  29}, /* ALAPH */
+    { 270, 12,  30}, /* BETH */
+    { 620, 12,  31}, /* GAMAL */
+    { 500, 12,  32}, /* DALATHRISH */
+    { 695, 12,  33}, /* HE */
+    {1342, 12,  34}, /* SYRIACWAW */
+    {1491, 12,  35}, /* ZAIN */
+    { 701, 12,  36}, /* HETH */
+    {1376, 12,  37}, /* TETH */
+    {1487, 12,  38}, /* YUDH */
+    {1488, 12,  39}, /* YUDHHE */
+    { 796, 12,  40}, /* KAPH */
+    { 821, 12,  41}, /* LAMADH */
+    { 985, 12,  42}, /* MIM */
+    {1083, 12,  43}, /* NUN */
+    {1252, 12,  44}, /* SEMKATH */
+    { 610, 12,  45}, /* FINALSEMKATH */
+    { 542, 12,  46}, /* E */
+    {1159, 12,  47}, /* PE */
+    {1214, 12,  48}, /* REVERSEDPE */
+    {1236, 12,  49}, /* SADHE */
+    {1203, 12,  50}, /* QAPH */
+    {1262, 12,  51}, /* SHIN */
+    {1369, 12,  52}, /* TAW */
+    {1494, 12,  53}, /* ZHAIN */
+    { 803, 12,  54}, /* KHAPH */
+    { 605, 12,  55}, /* FE */
+    { 310, 12,  56}, /* BURUSHASKIYEHBARREE */
+    { 913, 12,  57}, /* MALAYALAMNGA */
+    { 910, 12,  58}, /* MALAYALAMJA */
+    { 916, 12,  59}, /* MALAYALAMNYA */
+    { 919, 12,  60}, /* MALAYALAMTTA */
+    { 914, 12,  61}, /* MALAYALAMNNA */
+    { 915, 12,  62}, /* MALAYALAMNNNA */
+    { 909, 12,  63}, /* MALAYALAMBHA */
+    { 917, 12,  64}, /* MALAYALAMRA */
+    { 911, 12,  65}, /* MALAYALAMLLA */
+    { 912, 12,  66}, /* MALAYALAMLLLA */
+    { 918, 12,  67}, /* MALAYALAMSSA */
+    {1382, 12,  68}, /* THINYEH */
+    {1433, 12,  69}, /* VERTICALTAIL */
+    {1227, 12,  70}, /* ROHINGYAYEH */
+    {1301, 12,  71}, /* STRAIGHTWAW */
+    { 175, 12,  72}, /* AFRICANFEH */
+    { 177, 12,  73}, /* AFRICANQAF */
+    { 176, 12,  74}, /* AFRICANNOON */
+    { 925, 12,  75}, /* MANICHAEANALEPH */
+    { 927, 12,  76}, /* MANICHAEANBETH */
+    { 931, 12,  77}, /* MANICHAEANGIMEL */
+    { 928, 12,  78}, /* MANICHAEANDALETH */
+    { 949, 12,  79}, /* MANICHAEANWAW */
+    { 951, 12,  80}, /* MANICHAEANZAYIN */
+    { 932, 12,  81}, /* MANICHAEANHETH */
+    { 946, 12,  82}, /* MANICHAEANTETH */
+    { 950, 12,  83}, /* MANICHAEANYODH */
+    { 934, 12,  84}, /* MANICHAEANKAPH */
+    { 935, 12,  85}, /* MANICHAEANLAMEDH */
+    { 929, 12,  86}, /* MANICHAEANDHAMEDH */
+    { 947, 12,  87}, /* MANICHAEANTHAMEDH */
+    { 936, 12,  88}, /* MANICHAEANMEM */
+    { 937, 12,  89}, /* MANICHAEANNUN */
+    { 943, 12,  90}, /* MANICHAEANSAMEKH */
+    { 926, 12,  91}, /* MANICHAEANAYIN */
+    { 939, 12,  92}, /* MANICHAEANPE */
+    { 942, 12,  93}, /* MANICHAEANSADHE */
+    { 940, 12,  94}, /* MANICHAEANQOPH */
+    { 941, 12,  95}, /* MANICHAEANRESH */
+    { 944, 12,  96}, /* MANICHAEANTAW */
+    { 938, 12,  97}, /* MANICHAEANONE */
+    { 930, 12,  98}, /* MANICHAEANFIVE */
+    { 945, 12,  99}, /* MANICHAEANTEN */
+    { 948, 12, 100}, /* MANICHAEANTWENTY */
+    { 933, 12, 101}, /* MANICHAEANHUNDRED */
+    { 688, 12, 102}, /* HANIFIROHINGYAPA */
+    { 687, 12, 103}, /* HANIFIROHINGYAKINNAYA */
+    {1064, 13,   0}, /* NONJOINING */
+    {1405, 13,   0}, /* U */
+    {1401, 13,   1}, /* TRANSPARENT */
+    {1343, 13,   1}, /* T */
+    { 539, 13,   2}, /* DUALJOINING */
+    { 497, 13,   2}, /* D */
+    {1217, 13,   3}, /* RIGHTJOINING */
+    {1208, 13,   3}, /* R */
+    { 772, 13,   4}, /* JOINCAUSING */
+    { 313, 13,   4}, /* C */
+    { 852, 13,   5}, /* LEFTJOINING */
+    { 818, 13,   5}, /* L */
+    {1417, 14,   0}, /* UNKNOWN */
+    {1473, 14,   0}, /* XX */
+    { 435, 14,   1}, /* COMBININGMARK */
+    { 425, 14,   1}, /* CM */
+    { 302, 14,   2}, /* BREAKAFTER */
+    { 250, 14,   2}, /* BA */
+    { 872, 14,   3}, /* LINEFEED */
+    { 862, 14,   3}, /* LF */
+    { 922, 14,   4}, /* MANDATORYBREAK */
+    { 279, 14,   4}, /* BK */
+    { 325, 14,   5}, /* CARRIAGERETURN */
+    { 469, 14,   5}, /* CR */
+    {1291, 14,   6}, /* SPACE */
+    {1290, 14,   6}, /* SP */
+    { 595, 14,   7}, /* EXCLAMATION */
+    { 594, 14,   7}, /* EX */
+    {1206, 14,   8}, /* QUOTATION */
+    {1205, 14,   8}, /* QU */
+    { 195, 14,   9}, /* ALPHABETIC */
+    { 187, 14,   9}, /* AL */
+    {1187, 14,  10}, /* PREFIXNUMERIC */
+    {1186, 14,  10}, /* PR */
+    {1184, 14,  11}, /* POSTFIXNUMERIC */
+    {1177, 14,  11}, /* PO */
+    {1112, 14,  12}, /* OPENPUNCTUATION */
+    {1111, 14,  12}, /* OP */
+    { 423, 14,  13}, /* CLOSEPARENTHESIS */
+    { 466, 14,  13}, /* CP */
+    { 745, 14,  14}, /* INFIXNUMERIC */
+    { 760, 14,  14}, /* IS */
+    { 718, 14,  15}, /* HYPHEN */
+    { 717, 14,  15}, /* HY */
+    { 305, 14,  16}, /* BREAKSYMBOLS */
+    {1330, 14,  16}, /* SY */
+    {1080, 14,  17}, /* NUMERIC */
+    {1075, 14,  17}, /* NU */
+    { 424, 14,  18}, /* CLOSEPUNCTUATION */
+    { 421, 14,  18}, /* CL */
+    {1044, 14,  19}, /* NEXTLINE */
+    {1056, 14,  19}, /* NL */
+    { 641, 14,  20}, /* GLUE */
+    { 636, 14,  20}, /* GL */
+    { 199, 14,  21}, /* AMBIGUOUS */
+    { 181, 14,  21}, /* AI */
+    { 303, 14,  22}, /* BREAKBEFORE */
+    { 262, 14,  22}, /* BB */
+    { 698, 14,  23}, /* HEBREWLETTER */
+    { 709, 14,  23}, /* HL */
+    { 442, 14,  24}, /* COMPLEXCONTEXT */
+    {1234, 14,  24}, /* SA */
+    { 770, 14,  25}, /* JL */
+    { 778, 14,  26}, /* JV */
+    { 777, 14,  27}, /* JT */
+    {1066, 14,  28}, /* NONSTARTER */
+    {1071, 14,  28}, /* NS */
+    { 184, 14,  29}, /* AKSARA */
+    { 183, 14,  29}, /* AK */
+    {1437, 14,  30}, /* VIRAMA */
+    {1436, 14,  30}, /* VI */
+    { 725, 14,  31}, /* IDEOGRAPHIC */
+    { 719, 14,  31}, /* ID */
+    { 186, 14,  32}, /* AKSARASTART */
+    { 231, 14,  32}, /* AS */
+    {1438, 14,  33}, /* VIRAMAFINAL */
+    {1435, 14,  33}, /* VF */
+    {1503, 14,  34}, /* ZWSPACE */
+    {1501, 14,  34}, /* ZW */
+    {1502, 14,  35}, /* ZWJ */
+    { 304, 14,  36}, /* BREAKBOTH */
+    { 249, 14,  36}, /* B2 */
+    { 754, 14,  37}, /* INSEPARABLE */
+    { 738, 14,  37}, /* IN */
+    { 755, 14,  37}, /* INSEPERABLE */
+    {1462, 14,  38}, /* WORDJOINER */
+    {1459, 14,  38}, /* WJ */
+    { 547, 14,  39}, /* EBASE */
+    { 546, 14,  39}, /* EB */
+    { 443, 14,  40}, /* CONDITIONALJAPANESESTARTER */
+    { 387, 14,  40}, /* CJ */
+    { 668, 14,  41}, /* H2 */
+    { 669, 14,  42}, /* H3 */
+    {1327, 14,  43}, /* SURROGATE */
+    {1257, 14,  43}, /* SG */
+    { 458, 14,  44}, /* CONTINGENTBREAK */
+    { 330, 14,  44}, /* CB */
+    { 185, 14,  45}, /* AKSARAPREBASE */
+    { 207, 14,  45}, /* AP */
+    {1210, 14,  46}, /* REGIONALINDICATOR */
+    {1215, 14,  46}, /* RI */
+    { 560, 14,  47}, /* EMODIFIER */
+    { 558, 14,  47}, /* EM */
+    {1057, 15,   0}, /* NO */
+    {1024, 15,   0}, /* N */
+    {1478, 15,   1}, /* YES */
+    {1474, 15,   1}, /* Y */
+    { 963, 15,   2}, /* MAYBE */
+    { 900, 15,   2}, /* M */
+    {1057, 16,   0}, /* NO */
+    {1024, 16,   0}, /* N */
+    {1478, 16,   1}, /* YES */
+    {1474, 16,   1}, /* Y */
+    {1062, 17,   0}, /* NONE */
+    { 505, 17,   1}, /* DECIMAL */
+    { 504, 17,   1}, /* DE */
+    { 526, 17,   2}, /* DIGIT */
+    { 518, 17,   2}, /* DI */
+    {1080, 17,   3}, /* NUMERIC */
+    {1075, 17,   3}, /* NU */
+    {1030, 18,   0}, /* NAN */
+    {   1, 18,   1}, /* 0 */
+    {   2, 18,   2}, /* 1 */
+    {  55, 18,   3}, /* 2 */
+    {  88, 18,   4}, /* 3 */
+    { 111, 18,   5}, /* 4 */
+    { 128, 18,   6}, /* 5 */
+    { 138, 18,   7}, /* 6 */
+    { 144, 18,   8}, /* 7 */
+    { 153, 18,   9}, /* 8 */
+    { 160, 18,  10}, /* 9 */
+    {  12, 18,  11}, /* 1/4 */
+    {   7, 18,  12}, /* 1/2 */
+    {  92, 18,  13}, /* 3/4 */
+    {   5, 18,  14}, /* 1/16 */
+    {  18, 18,  15}, /* 1/8 */
+    {  89, 18,  16}, /* 3/16 */
+    {  50, 18,  17}, /* 16 */
+    {  21, 18,  18}, /* 10 */
+    {  22, 18,  19}, /* 100 */
+    {  23, 18,  20}, /* 1000 */
+    {   6, 18,  21}, /* 1/160 */
+    {  13, 18,  22}, /* 1/40 */
+    {  96, 18,  23}, /* 3/80 */
+    {   8, 18,  24}, /* 1/20 */
+    {   3, 18,  25}, /* 1/10 */
+    {  91, 18,  26}, /* 3/20 */
+    {  14, 18,  27}, /* 1/5 */
+    {  90, 18,  28}, /* 3/2 */
+    { 130, 18,  29}, /* 5/2 */
+    { 146, 18,  30}, /* 7/2 */
+    { 161, 18,  31}, /* 9/2 */
+    {  37, 18,  32}, /* 11/2 */
+    {  43, 18,  33}, /* 13/2 */
+    {  49, 18,  34}, /* 15/2 */
+    {  52, 18,  35}, /* 17/2 */
+    {   0, 18,  36}, /* -1/2 */
+    {  58, 18,  37}, /* 20 */
+    {  97, 18,  38}, /* 30 */
+    { 113, 18,  39}, /* 40 */
+    { 133, 18,  40}, /* 50 */
+    { 139, 18,  41}, /* 60 */
+    { 148, 18,  42}, /* 70 */
+    { 154, 18,  43}, /* 80 */
+    { 162, 18,  44}, /* 90 */
+    {  24, 18,  45}, /* 10000 */
+    {  51, 18,  46}, /* 17 */
+    {  53, 18,  47}, /* 18 */
+    {  54, 18,  48}, /* 19 */
+    {  17, 18,  49}, /* 1/7 */
+    {  20, 18,  50}, /* 1/9 */
+    {   9, 18,  51}, /* 1/3 */
+    {  56, 18,  52}, /* 2/3 */
+    {  57, 18,  53}, /* 2/5 */
+    {  93, 18,  54}, /* 3/5 */
+    { 112, 18,  55}, /* 4/5 */
+    {  15, 18,  56}, /* 1/6 */
+    { 131, 18,  57}, /* 5/6 */
+    {  95, 18,  58}, /* 3/8 */
+    { 132, 18,  59}, /* 5/8 */
+    { 147, 18,  60}, /* 7/8 */
+    {  35, 18,  61}, /* 11 */
+    {  39, 18,  62}, /* 12 */
+    { 134, 18,  63}, /* 500 */
+    { 135, 18,  64}, /* 5000 */
+    { 136, 18,  65}, /* 50000 */
+    {  25, 18,  66}, /* 100000 */
+    {  42, 18,  67}, /* 13 */
+    {  47, 18,  68}, /* 14 */
+    {  48, 18,  69}, /* 15 */
+    {  65, 18,  70}, /* 21 */
+    {  70, 18,  71}, /* 22 */
+    {  76, 18,  72}, /* 23 */
+    {  81, 18,  73}, /* 24 */
+    {  83, 18,  74}, /* 25 */
+    {  84, 18,  75}, /* 26 */
+    {  85, 18,  76}, /* 27 */
+    {  86, 18,  77}, /* 28 */
+    {  87, 18,  78}, /* 29 */
+    { 102, 18,  79}, /* 31 */
+    { 103, 18,  80}, /* 32 */
+    { 104, 18,  81}, /* 33 */
+    { 105, 18,  82}, /* 34 */
+    { 106, 18,  83}, /* 35 */
+    { 107, 18,  84}, /* 36 */
+    { 108, 18,  85}, /* 37 */
+    { 109, 18,  86}, /* 38 */
+    { 110, 18,  87}, /* 39 */
+    { 118, 18,  88}, /* 41 */
+    { 119, 18,  89}, /* 42 */
+    { 120, 18,  90}, /* 43 */
+    { 122, 18,  91}, /* 44 */
+    { 123, 18,  92}, /* 45 */
+    { 124, 18,  93}, /* 46 */
+    { 125, 18,  94}, /* 47 */
+    { 126, 18,  95}, /* 48 */
+    { 127, 18,  96}, /* 49 */
+    {  32, 18,  97}, /* 10000000000000000 */
+    {  28, 18,  98}, /* 100000000 */
+    {  26, 18,  99}, /* 1000000 */
+    {  59, 18, 100}, /* 200 */
+    {  29, 18, 101}, /* 1000000000 */
+    {  98, 18, 102}, /* 300 */
+    { 114, 18, 103}, /* 400 */
+    { 140, 18, 104}, /* 600 */
+    { 149, 18, 105}, /* 700 */
+    { 155, 18, 106}, /* 800 */
+    { 163, 18, 107}, /* 900 */
+    {  60, 18, 108}, /* 2000 */
+    {  99, 18, 109}, /* 3000 */
+    { 115, 18, 110}, /* 4000 */
+    { 141, 18, 111}, /* 6000 */
+    { 150, 18, 112}, /* 7000 */
+    { 156, 18, 113}, /* 8000 */
+    { 164, 18, 114}, /* 9000 */
+    {  61, 18, 115}, /* 20000 */
+    { 100, 18, 116}, /* 30000 */
+    { 116, 18, 117}, /* 40000 */
+    { 142, 18, 118}, /* 60000 */
+    { 151, 18, 119}, /* 70000 */
+    { 157, 18, 120}, /* 80000 */
+    { 165, 18, 121}, /* 90000 */
+    {  36, 18, 122}, /* 11/12 */
+    {  62, 18, 123}, /* 200000 */
+    { 101, 18, 124}, /* 300000 */
+    { 117, 18, 125}, /* 400000 */
+    { 137, 18, 126}, /* 500000 */
+    { 143, 18, 127}, /* 600000 */
+    { 152, 18, 128}, /* 700000 */
+    { 158, 18, 129}, /* 800000 */
+    { 166, 18, 130}, /* 900000 */
+    {   4, 18, 131}, /* 1/12 */
+    { 129, 18, 132}, /* 5/12 */
+    { 145, 18, 133}, /* 7/12 */
+    {  11, 18, 134}, /* 1/320 */
+    {  19, 18, 135}, /* 1/80 */
+    {  16, 18, 136}, /* 1/64 */
+    {  10, 18, 137}, /* 1/32 */
+    {  94, 18, 138}, /* 3/64 */
+    {  68, 18, 139}, /* 216000 */
+    { 121, 18, 140}, /* 432000 */
+    {  30, 18, 141}, /* 10000000000 */
+    {  31, 18, 142}, /* 1000000000000 */
+    {  27, 18, 143}, /* 10000000 */
+    {  63, 18, 144}, /* 20000000 */
+    {1417, 19,   0}, /* UNKNOWN */
+    {1505, 19,   0}, /* ZZZZ */
+    { 437, 19,   1}, /* COMMON */
+    {1504, 19,   1}, /* ZYYY */
+    { 825, 19,   2}, /* LATIN */
+    { 845, 19,   2}, /* LATN */
+    { 287, 19,   3}, /* BOPOMOFO */
+    { 286, 19,   3}, /* BOPO */
+    { 746, 19,   4}, /* INHERITED */
+    {1495, 19,   4}, /* ZINH */
+    {1201, 19,   4}, /* QAAI */
+    { 655, 19,   5}, /* GREEK */
+    { 659, 19,   5}, /* GREK */
+    { 462, 19,   6}, /* COPTIC */
+    { 461, 19,   6}, /* COPT */
+    {1200, 19,   6}, /* QAAC */
+    { 484, 19,   7}, /* CYRILLIC */
+    { 496, 19,   7}, /* CYRL */
+    { 227, 19,   8}, /* ARMENIAN */
+    { 229, 19,   8}, /* ARMN */
+    { 697, 19,   9}, /* HEBREW */
+    { 696, 19,   9}, /* HEBR */
+    { 210, 19,  10}, /* ARABIC */
+    { 209, 19,  10}, /* ARAB */
+    {1339, 19,  11}, /* SYRIAC */
+    {1338, 19,  11}, /* SYRC */
+    {1380, 19,  12}, /* THAANA */
+    {1379, 19,  12}, /* THAA */
+    {1054, 19,  13}, /* NKO */
+    {1055, 19,  13}, /* NKOO */
+    {1237, 19,  14}, /* SAMARITAN */
+    {1238, 19,  14}, /* SAMR */
+    { 921, 19,  15}, /* MANDAIC */
+    { 920, 19,  15}, /* MAND */
+    { 513, 19,  16}, /* DEVANAGARI */
+    { 512, 19,  16}, /* DEVA */
+    { 269, 19,  17}, /* BENGALI */
+    { 268, 19,  17}, /* BENG */
+    { 665, 19,  18}, /* GURMUKHI */
+    { 666, 19,  18}, /* GURU */
+    { 662, 19,  19}, /* GUJARATI */
+    { 663, 19,  19}, /* GUJR */
+    {1114, 19,  20}, /* ORIYA */
+    {1117, 19,  20}, /* ORYA */
+    {1358, 19,  21}, /* TAMIL */
+    {1361, 19,  21}, /* TAML */
+    {1373, 19,  22}, /* TELUGU */
+    {1372, 19,  22}, /* TELU */
+    { 795, 19,  23}, /* KANNADA */
+    { 814, 19,  23}, /* KNDA */
+    { 908, 19,  24}, /* MALAYALAM */
+    { 999, 19,  24}, /* MLYM */
+    {1271, 19,  25}, /* SINHALA */
+    {1270, 19,  25}, /* SINH */
+    {1381, 19,  26}, /* THAI */
+    { 823, 19,  27}, /* LAO */
+    { 824, 19,  27}, /* LAOO */
+    {1383, 19,  28}, /* TIBETAN */
+    {1384, 19,  28}, /* TIBT */
+    {1018, 19,  29}, /* MYANMAR */
+    {1023, 19,  29}, /* MYMR */
+    { 631, 19,  30}, /* GEORGIAN */
+    { 630, 19,  30}, /* GEOR */
+    { 678, 19,  31}, /* HANGUL */
+    { 677, 19,  31}, /* HANG */
+    { 582, 19,  32}, /* ETHIOPIC */
+    { 581, 19,  32}, /* ETHI */
+    { 379, 19,  33}, /* CHEROKEE */
+    { 378, 19,  33}, /* CHER */
+    { 317, 19,  34}, /* CANADIANABORIGINAL */
+    { 321, 19,  34}, /* CANS */
+    {1092, 19,  35}, /* OGHAM */
+    {1091, 19,  35}, /* OGAM */
+    {1230, 19,  36}, /* RUNIC */
+    {1231, 19,  36}, /* RUNR */
+    {1344, 19,  37}, /* TAGALOG */
+    {1378, 19,  37}, /* TGLG */
+    { 692, 19,  38}, /* HANUNOO */
+    { 689, 19,  38}, /* HANO */
+    { 309, 19,  39}, /* BUHID */
+    { 308, 19,  39}, /* BUHD */
+    {1346, 19,  40}, /* TAGBANWA */
+    {1345, 19,  40}, /* TAGB */
+    { 807, 19,  41}, /* KHMER */
+    { 809, 19,  41}, /* KHMR */
+    {1008, 19,  42}, /* MONGOLIAN */
+    {1007, 19,  42}, /* MONG */
+    { 864, 19,  43}, /* LIMBU */
+    { 863, 19,  43}, /* LIMB */
+    {1349, 19,  44}, /* TAILE */
+    {1356, 19,  44}, /* TALE */
+    {1043, 19,  45}, /* NEWTAILUE */
+    {1357, 19,  45}, /* TALU */
+    { 307, 19,  46}, /* BUGINESE */
+    { 306, 19,  46}, /* BUGI */
+    {1350, 19,  47}, /* TAITHAM */
+    { 822, 19,  47}, /* LANA */
+    { 252, 19,  48}, /* BALINESE */
+    { 251, 19,  48}, /* BALI */
+    {1304, 19,  49}, /* SUNDANESE */
+    {1303, 19,  49}, /* SUND */
+    { 260, 19,  50}, /* BATAK */
+    { 261, 19,  50}, /* BATK */
+    { 858, 19,  51}, /* LEPCHA */
+    { 857, 19,  51}, /* LEPC */
+    {1096, 19,  52}, /* OLCHIKI */
+    {1097, 19,  52}, /* OLCK */
+    { 300, 19,  53}, /* BRAILLE */
+    { 299, 19,  53}, /* BRAI */
+    { 638, 19,  54}, /* GLAGOLITIC */
+    { 637, 19,  54}, /* GLAG */
+    {1385, 19,  55}, /* TIFINAGH */
+    {1377, 19,  55}, /* TFNG */
+    { 676, 19,  56}, /* HAN */
+    { 685, 19,  56}, /* HANI */
+    { 708, 19,  57}, /* HIRAGANA */
+    { 707, 19,  57}, /* HIRA */
+    { 797, 19,  58}, /* KATAKANA */
+    { 784, 19,  58}, /* KANA */
+    {1481, 19,  59}, /* YI */
+    {1482, 19,  59}, /* YIII */
+    { 875, 19,  60}, /* LISU */
+    {1423, 19,  61}, /* VAI */
+    {1424, 19,  61}, /* VAII */
+    { 254, 19,  62}, /* BAMUM */
+    { 253, 19,  62}, /* BAMU */
+    {1333, 19,  63}, /* SYLOTINAGRI */
+    {1332, 19,  63}, /* SYLO */
+    {1163, 19,  64}, /* PHAGSPA */
+    {1162, 19,  64}, /* PHAG */
+    {1241, 19,  65}, /* SAURASHTRA */
+    {1240, 19,  65}, /* SAUR */
+    { 802, 19,  66}, /* KAYAHLI */
+    { 783, 19,  66}, /* KALI */
+    {1213, 19,  67}, /* REJANG */
+    {1222, 19,  67}, /* RJNG */
+    { 768, 19,  68}, /* JAVANESE */
+    { 767, 19,  68}, /* JAVA */
+    { 372, 19,  69}, /* CHAM */
+    {1351, 19,  70}, /* TAIVIET */
+    {1368, 19,  70}, /* TAVT */
+    { 972, 19,  71}, /* MEETEIMAYEK */
+    {1013, 19,  71}, /* MTEI */
+    { 868, 19,  72}, /* LINEARB */
+    { 866, 19,  72}, /* LINB */
+    { 897, 19,  73}, /* LYCIAN */
+    { 896, 19,  73}, /* LYCI */
+    { 324, 19,  74}, /* CARIAN */
+    { 323, 19,  74}, /* CARI */
+    {1099, 19,  75}, /* OLDITALIC */
+    { 763, 19,  75}, /* ITAL */
+    { 646, 19,  76}, /* GOTHIC */
+    { 645, 19,  76}, /* GOTH */
+    {1101, 19,  77}, /* OLDPERMIC */
+    {1160, 19,  77}, /* PERM */
+    {1410, 19,  78}, /* UGARITIC */
+    {1409, 19,  78}, /* UGAR */
+    {1102, 19,  79}, /* OLDPERSIAN */
+    {1471, 19,  79}, /* XPEO */
+    { 511, 19,  80}, /* DESERET */
+    { 537, 19,  80}, /* DSRT */
+    {1260, 19,  81}, /* SHAVIAN */
+    {1261, 19,  81}, /* SHAW */
+    {1121, 19,  82}, /* OSMANYA */
+    {1120, 19,  82}, /* OSMA */
+    {1118, 19,  83}, /* OSAGE */
+    {1119, 19,  83}, /* OSGE */
+    { 555, 19,  84}, /* ELBASAN */
+    { 554, 19,  84}, /* ELBA */
+    { 329, 19,  85}, /* CAUCASIANALBANIAN */
+    { 178, 19,  85}, /* AGHB */
+    {1442, 19,  86}, /* VITHKUQI */
+    {1441, 19,  86}, /* VITH */
+    { 867, 19,  87}, /* LINEARA */
+    { 865, 19,  87}, /* LINA */
+    { 481, 19,  88}, /* CYPRIOT */
+    { 468, 19,  88}, /* CPRT */
+    { 737, 19,  89}, /* IMPERIALARAMAIC */
+    { 228, 19,  89}, /* ARMI */
+    {1146, 19,  90}, /* PALMYRENE */
+    {1145, 19,  90}, /* PALM */
+    {1027, 19,  91}, /* NABATAEAN */
+    {1037, 19,  91}, /* NBAT */
+    { 694, 19,  92}, /* HATRAN */
+    { 693, 19,  92}, /* HATR */
+    {1169, 19,  93}, /* PHOENICIAN */
+    {1168, 19,  93}, /* PHNX */
+    { 899, 19,  94}, /* LYDIAN */
+    { 898, 19,  94}, /* LYDI */
+    { 980, 19,  95}, /* MEROITICHIEROGLYPHS */
+    { 978, 19,  95}, /* MERO */
+    { 979, 19,  96}, /* MEROITICCURSIVE */
+    { 977, 19,  96}, /* MERC */
+    { 805, 19,  97}, /* KHAROSHTHI */
+    { 804, 19,  97}, /* KHAR */
+    {1104, 19,  98}, /* OLDSOUTHARABIAN */
+    {1239, 19,  98}, /* SARB */
+    {1100, 19,  99}, /* OLDNORTHARABIAN */
+    {1034, 19,  99}, /* NARB */
+    { 924, 19, 100}, /* MANICHAEAN */
+    { 923, 19, 100}, /* MANI */
+    { 246, 19, 101}, /* AVESTAN */
+    { 247, 19, 101}, /* AVST */
+    { 753, 19, 102}, /* INSCRIPTIONALPARTHIAN */
+    {1193, 19, 102}, /* PRTI */
+    { 752, 19, 103}, /* INSCRIPTIONALPAHLAVI */
+    {1166, 19, 103}, /* PHLI */
+    {1195, 19, 104}, /* PSALTERPAHLAVI */
+    {1167, 19, 104}, /* PHLP */
+    {1105, 19, 105}, /* OLDTURKIC */
+    {1115, 19, 105}, /* ORKH */
+    {1098, 19, 106}, /* OLDHUNGARIAN */
+    { 716, 19, 106}, /* HUNG */
+    { 686, 19, 107}, /* HANIFIROHINGYA */
+    {1226, 19, 107}, /* ROHG */
+    {1480, 19, 108}, /* YEZIDI */
+    {1479, 19, 108}, /* YEZI */
+    {1103, 19, 109}, /* OLDSOGDIAN */
+    {1285, 19, 109}, /* SOGO */
+    {1284, 19, 110}, /* SOGDIAN */
+    {1283, 19, 110}, /* SOGD */
+    {1106, 19, 111}, /* OLDUYGHUR */
+    {1137, 19, 111}, /* OUGR */
+    { 383, 19, 112}, /* CHORASMIAN */
+    { 384, 19, 112}, /* CHRS */
+    { 557, 19, 113}, /* ELYMAIC */
+    { 556, 19, 113}, /* ELYM */
+    { 297, 19, 114}, /* BRAHMI */
+    { 296, 19, 114}, /* BRAH */
+    { 781, 19, 115}, /* KAITHI */
+    { 816, 19, 115}, /* KTHI */
+    {1287, 19, 116}, /* SORASOMPENG */
+    {1286, 19, 116}, /* SORA */
+    { 371, 19, 117}, /* CHAKMA */
+    { 315, 19, 117}, /* CAKM */
+    { 902, 19, 118}, /* MAHAJANI */
+    { 903, 19, 118}, /* MAHJ */
+    {1259, 19, 119}, /* SHARADA */
+    {1264, 19, 119}, /* SHRD */
+    { 811, 19, 120}, /* KHOJKI */
+    { 810, 19, 120}, /* KHOJ */
+    {1015, 19, 121}, /* MULTANI */
+    {1014, 19, 121}, /* MULT */
+    { 812, 19, 122}, /* KHUDAWADI */
+    {1268, 19, 122}, /* SIND */
+    { 648, 19, 123}, /* GRANTHA */
+    { 647, 19, 123}, /* GRAN */
+    {1041, 19, 124}, /* NEWA */
+    {1387, 19, 125}, /* TIRHUTA */
+    {1386, 19, 125}, /* TIRH */
+    {1266, 19, 126}, /* SIDDHAM */
+    {1265, 19, 126}, /* SIDD */
+    {1001, 19, 127}, /* MODI */
+    {1355, 19, 128}, /* TAKRI */
+    {1354, 19, 128}, /* TAKR */
+    { 180, 19, 129}, /* AHOM */
+    { 530, 19, 130}, /* DOGRA */
+    { 529, 19, 130}, /* DOGR */
+    {1453, 19, 131}, /* WARANGCITI */
+    {1452, 19, 131}, /* WARA */
+    { 528, 19, 132}, /* DIVESAKURU */
+    { 525, 19, 132}, /* DIAK */
+    {1032, 19, 133}, /* NANDINAGARI */
+    {1031, 19, 133}, /* NAND */
+    {1492, 19, 134}, /* ZANABAZARSQUARE */
+    {1493, 19, 134}, /* ZANB */
+    {1289, 19, 135}, /* SOYOMBO */
+    {1288, 19, 135}, /* SOYO */
+    {1153, 19, 136}, /* PAUCINHAU */
+    {1152, 19, 136}, /* PAUC */
+    { 271, 19, 137}, /* BHAIKSUKI */
+    { 272, 19, 137}, /* BHKS */
+    { 953, 19, 138}, /* MARCHEN */
+    { 952, 19, 138}, /* MARC */
+    { 955, 19, 139}, /* MASARAMGONDI */
+    { 644, 19, 139}, /* GONM */
+    { 664, 19, 140}, /* GUNJALAGONDI */
+    { 643, 19, 140}, /* GONG */
+    { 907, 19, 141}, /* MAKASAR */
+    { 906, 19, 141}, /* MAKA */
+    { 801, 19, 142}, /* KAWI */
+    { 471, 19, 143}, /* CUNEIFORM */
+    {1472, 19, 143}, /* XSUX */
+    { 483, 19, 144}, /* CYPROMINOAN */
+    { 467, 19, 144}, /* CPMN */
+    { 553, 19, 145}, /* EGYPTIANHIEROGLYPHS */
+    { 551, 19, 145}, /* EGYP */
+    { 201, 19, 146}, /* ANATOLIANHIEROGLYPHS */
+    { 710, 19, 146}, /* HLUW */
+    {1011, 19, 147}, /* MRO */
+    {1012, 19, 147}, /* MROO */
+    {1363, 19, 148}, /* TANGSA */
+    {1389, 19, 148}, /* TNSA */
+    { 259, 19, 149}, /* BASSAVAH */
+    { 258, 19, 149}, /* BASS */
+    {1144, 19, 150}, /* PAHAWHHMONG */
+    { 711, 19, 150}, /* HMNG */
+    { 968, 19, 151}, /* MEDEFAIDRIN */
+    { 969, 19, 151}, /* MEDF */
+    { 981, 19, 152}, /* MIAO */
+    {1176, 19, 152}, /* PLRD */
+    {1364, 19, 153}, /* TANGUT */
+    {1362, 19, 153}, /* TANG */
+    {1084, 19, 154}, /* NUSHU */
+    {1072, 19, 154}, /* NSHU */
+    { 806, 19, 155}, /* KHITANSMALLSCRIPT */
+    { 813, 19, 155}, /* KITS */
+    { 541, 19, 156}, /* DUPLOYAN */
+    { 540, 19, 156}, /* DUPL */
+    {1267, 19, 157}, /* SIGNWRITING */
+    {1258, 19, 157}, /* SGNW */
+    {1087, 19, 158}, /* NYIAKENGPUACHUEHMONG */
+    { 712, 19, 158}, /* HMNP */
+    {1399, 19, 159}, /* TOTO */
+    {1451, 19, 160}, /* WANCHO */
+    {1456, 19, 160}, /* WCHO */
+    {1029, 19, 161}, /* NAGMUNDARI */
+    {1028, 19, 161}, /* NAGM */
+    { 976, 19, 162}, /* MENDEKIKAKUI */
+    { 975, 19, 162}, /* MEND */
+    { 172, 19, 163}, /* ADLAM */
+    { 173, 19, 163}, /* ADLM */
+    { 799, 19, 164}, /* KATAKANAORHIRAGANA */
+    { 714, 19, 164}, /* HRKT */
+    {1122, 20,   0}, /* OTHER */
+    {1473, 20,   0}, /* XX */
+    {1290, 20,   1}, /* SP */
+    { 862, 20,   2}, /* LF */
+    { 469, 20,   3}, /* CR */
+    {1300, 20,   4}, /* STERM */
+    {1299, 20,   4}, /* ST */
+    { 422, 20,   5}, /* CLOSE */
+    { 421, 20,   5}, /* CL */
+    {1244, 20,   6}, /* SCONTINUE */
+    {1243, 20,   6}, /* SC */
+    { 240, 20,   7}, /* ATERM */
+    { 235, 20,   7}, /* AT */
+    {1080, 20,   8}, /* NUMERIC */
+    {1075, 20,   8}, /* NU */
+    {1419, 20,   9}, /* UPPER */
+    {1418, 20,   9}, /* UP */
+    { 883, 20,  10}, /* LOWER */
+    { 880, 20,  10}, /* LO */
+    {1255, 20,  11}, /* SEP */
+    {1249, 20,  11}, /* SE */
+    { 614, 20,  12}, /* FORMAT */
+    { 612, 20,  12}, /* FO */
+    {1107, 20,  13}, /* OLETTER */
+    { 848, 20,  13}, /* LE */
+    { 597, 20,  14}, /* EXTEND */
+    { 594, 20,  14}, /* EX */
+    {1122, 21,   0}, /* OTHER */
+    {1473, 21,   0}, /* XX */
+    { 862, 21,   1}, /* LF */
+    {1042, 21,   2}, /* NEWLINE */
+    {1056, 21,   2}, /* NL */
+    { 469, 21,   3}, /* CR */
+    {1464, 21,   4}, /* WSEGSPACE */
+    { 535, 21,   5}, /* DOUBLEQUOTE */
+    { 536, 21,   5}, /* DQ */
+    {1269, 21,   6}, /* SINGLEQUOTE */
+    {1296, 21,   6}, /* SQ */
+    { 983, 21,   7}, /* MIDNUM */
+    {1000, 21,   7}, /* MN */
+    { 984, 21,   8}, /* MIDNUMLET */
+    { 964, 21,   8}, /* MB */
+    {1080, 21,   9}, /* NUMERIC */
+    {1075, 21,   9}, /* NU */
+    { 982, 21,  10}, /* MIDLETTER */
+    { 998, 21,  10}, /* ML */
+    { 192, 21,  11}, /* ALETTER */
+    { 848, 21,  11}, /* LE */
+    { 600, 21,  12}, /* EXTENDNUMLET */
+    { 594, 21,  12}, /* EX */
+    { 614, 21,  13}, /* FORMAT */
+    { 612, 21,  13}, /* FO */
+    { 597, 21,  14}, /* EXTEND */
+    { 698, 21,  15}, /* HEBREWLETTER */
+    { 709, 21,  15}, /* HL */
+    {1502, 21,  16}, /* ZWJ */
+    { 797, 21,  17}, /* KATAKANA */
+    { 779, 21,  17}, /* KA */
+    {1210, 21,  18}, /* REGIONALINDICATOR */
+    {1215, 21,  18}, /* RI */
+    { 547, 21,  19}, /* EBASE */
+    { 546, 21,  19}, /* EB */
+    { 548, 21,  20}, /* EBASEGAZ */
+    { 549, 21,  20}, /* EBG */
+    { 560, 21,  21}, /* EMODIFIER */
+    { 558, 21,  21}, /* EM */
+    { 642, 21,  22}, /* GLUEAFTERZWJ */
+    { 621, 21,  22}, /* GAZ */
 };
 
 /* Codepoints which expand on full case-folding. */
 RE_UINT16 re_expand_on_folding[] = {
       223,   304,   329,   496,   912,   944,  1415,  7830,
      7831,  7832,  7833,  7834,  7838,  8016,  8018,  8020,
      8022,  8064,  8065,  8066,  8067,  8068,  8069,  8070,
@@ -3353,16 +3397,16 @@
     20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 10, 30, 13, 31, 10, 10,
     10, 32, 10, 10, 10, 10, 10, 10, 10, 10, 33, 34, 13, 13, 13, 13,
     13, 35, 13, 36, 10, 10, 10, 10, 10, 10, 10, 37, 38, 10, 10, 39,
     10, 10, 10, 10, 10, 40, 10, 41, 42, 43, 44, 45, 46, 10, 10, 10,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 47, 13, 13, 13, 48, 49, 13,
-    13, 13, 13, 50, 13, 13, 13, 13, 13, 13, 51, 10, 10, 10, 52, 10,
-    13, 13, 13, 13, 53, 13, 13, 13, 54, 10, 10, 10, 10, 10, 10, 10,
+    13, 13, 13, 50, 13, 13, 13, 13, 13, 13, 51, 52, 10, 10, 53, 10,
+    13, 13, 13, 13, 54, 13, 13, 13, 55, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
@@ -3516,15 +3560,17 @@
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4, 166,   4,   4,   4,   4,   4,   4,
     117,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4, 268,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
-      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  78,
+      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4, 269,
+      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
+      4,   4, 117,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
     117,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  32,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  92,   0,   0
 };
@@ -3593,15 +3639,15 @@
       7,   0,   4,   0,   0,   0,  39,   0, 255,   7, 255,  31, 255,   1, 255,  67,
     255, 255, 223, 255, 255, 255, 255, 223, 100, 222, 255, 235, 239, 255, 255, 255,
     191, 231, 223, 223, 255, 255, 255, 123,  95, 252, 253, 255,  63, 255, 255, 255,
     253, 255, 255, 247, 255, 127, 255, 255, 247,  15,   0,   0, 224,   7,   0,   0,
     127, 255, 255, 249, 219,   7, 255, 255, 255,  31, 128,  63,   0,  64,   0,   0,
     255,  15,   0,   0, 127, 111, 255, 127, 143,   8,   0,   0, 150, 254, 247,  10,
     132, 234, 150, 170, 150, 247, 247,  94, 255, 251, 255,  15, 238, 251, 255,  15,
-      3,   0, 255, 255
+      3,   0, 255, 255,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_alphabetic(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -3628,16 +3674,16 @@
     20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 10, 30, 13, 31, 10, 10,
     10, 32, 10, 10, 10, 10, 10, 10, 10, 10, 33, 34, 13, 13, 13, 13,
     13, 35, 13, 36, 10, 10, 10, 10, 10, 10, 10, 37, 38, 10, 10, 39,
     10, 10, 10, 10, 10, 40, 10, 41, 42, 43, 44, 45, 46, 10, 47, 10,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 48, 13, 13, 13, 49, 50, 13,
-    13, 13, 13, 51, 13, 13, 13, 13, 13, 13, 52, 10, 10, 10, 53, 10,
-    13, 13, 13, 13, 54, 13, 13, 13, 55, 10, 10, 10, 10, 10, 10, 10,
+    13, 13, 13, 51, 13, 13, 13, 13, 13, 13, 52, 53, 10, 10, 54, 10,
+    13, 13, 13, 13, 55, 13, 13, 13, 56, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
@@ -3793,15 +3839,17 @@
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5, 168,   5,   5,   5,   5,   5,   5,
      87,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5, 276,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
-      5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,  79,
+      5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5, 277,
+      5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
+      5,   5,  87,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
      87,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,  32,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,  95,   0,   0
 };
@@ -3872,15 +3920,15 @@
       7,   0,   4,   0,   0,   0,  39,   0, 255,   7, 255,  31, 255,   1, 255,  67,
     255, 255, 223, 255, 255, 255, 255, 223, 100, 222, 255, 235, 239, 255, 255, 255,
     191, 231, 223, 223, 255, 255, 255, 123,  95, 252, 253, 255,  63, 255, 255, 255,
     253, 255, 255, 247, 255, 127, 255, 255, 247, 207, 255, 255, 224,   7,   0,   0,
     127, 255, 255, 249, 219,   7, 255, 255, 255,  31, 128,  63, 255,  67,   0,   0,
     255,  15, 255,   3, 127, 111, 255, 127, 143,   8, 255,   3, 150, 254, 247,  10,
     132, 234, 150, 170, 150, 247, 247,  94, 255, 251, 255,  15, 238, 251, 255,  15,
-      3,   0, 255, 255
+      3,   0, 255, 255,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_alphanumeric(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -3924,16 +3972,16 @@
     21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 18, 31, 13, 32, 18, 18,
     18, 33, 18, 18, 18, 18, 18, 18, 18, 18, 34, 35, 13, 13, 13, 13,
     13, 36, 13, 37, 18, 18, 18, 18, 18, 18, 18, 38, 39, 18, 18, 40,
     18, 18, 18, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 54, 13, 13, 13, 55, 56, 13,
-    13, 13, 13, 57, 13, 13, 13, 13, 13, 13, 58, 18, 18, 18, 59, 53,
-    13, 13, 13, 13, 60, 13, 13, 13, 61, 18, 18, 18, 18, 18, 18, 18,
+    13, 13, 13, 57, 13, 13, 13, 13, 13, 13, 58, 59, 18, 18, 60, 53,
+    13, 13, 13, 13, 61, 13, 13, 13, 62, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 53,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 53,
@@ -3969,26 +4017,26 @@
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 53,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 53,
-    62, 63, 63, 63, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
+    63, 64, 64, 64, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 53,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
-    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 64,
+    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 65,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
-    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 64
+    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 65
 };
 
 static RE_UINT16 re_bidi_class_table_2[] = {
       0,   1,   2,   3,   4,   5,   6,   6,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   8,   9,  10,  11,  11,  11,  12,  13,  14,   7,  15,
       7,   7,   7,   7,  16,   7,   7,   7,   7,  17,  18,   7,  19,  20,  21,  22,
      23,  24,  25,  26,  24,  24,  27,  28,  29,  30,  31,  24,  24,  32,  22,  33,
@@ -4103,14 +4151,16 @@
     149,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7, 455,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 456,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
+      7,   7, 149,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,
+      7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
     149,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,  22,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 267,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 366,  22,  22,
     457, 457, 457, 457, 457, 457, 457, 457,  11,  11,  11,  11,  11,  11,  11, 458,
     457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457,
@@ -4486,28 +4536,28 @@
      5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,
      5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  0,  5,  5,  5,  5,  5,
      5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,
      5,  5,  5,  5,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,
      5,  5,  5,  5,  5,  5,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  0,  0,  0,  0,
+     5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,
      4,  5,  5,  5,  5, 10, 10, 10,  5,  5,  5,  5,  5,  5,  5,  5,
      5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,
      5, 10, 10, 10, 10, 10, 10, 10, 10, 10, 11, 11, 11, 11, 10, 10,
      5, 10, 10, 10, 10, 10,  5,  5, 10, 10, 10, 10, 10,  5,  5,  5,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10,  0,  0, 11, 11,  5,  5, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,  5, 10, 10, 10, 10,
      0,  0,  0,  0,  0, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,  0,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
-     5,  5,  5,  5,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     5,  5,  5,  5,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  5,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,  5,  5,  0,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
      5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,  5,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,  5,  5,  5, 10,
@@ -5030,15 +5080,15 @@
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  1,
     10, 10,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,  1,  1
 };
@@ -5237,16 +5287,16 @@
     26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 36, 36,
     36, 40, 36, 36, 36, 36, 36, 36, 36, 36, 41, 42, 43, 43, 43, 43,
     43, 43, 44, 45, 36, 36, 36, 36, 36, 36, 36, 46, 47, 36, 36, 48,
     36, 36, 36, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 36,
     61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61,
     61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61, 61,
     61, 61, 61, 61, 61, 61, 61, 61, 61, 62, 63, 63, 63, 64, 65, 66,
-    66, 66, 66, 67, 68, 68, 68, 68, 68, 68, 69, 36, 36, 36, 70, 36,
-    71, 71, 71, 71, 72, 73, 73, 73, 74, 36, 36, 36, 36, 36, 36, 36,
+    66, 66, 66, 67, 68, 68, 68, 68, 68, 68, 69, 70, 36, 36, 71, 36,
+    72, 72, 72, 72, 73, 74, 74, 74, 75, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
@@ -5282,26 +5332,26 @@
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
-    75, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
+    76, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
     36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
-    76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76,
-    76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76,
-    76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76,
-    76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76, 76,
     77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77,
     77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77,
     77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77,
-    77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77
+    77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77, 77,
+    78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78,
+    78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78,
+    78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78,
+    78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78, 78
 };
 
 static RE_UINT16 re_block_table_2[] = {
       0,   0,   0,   0,   1,   1,   1,   1,   2,   2,   2,   2,   3,   3,   3,   3,
       3,   3,   4,   5,   5,   6,   7,   7,   8,   8,   8,   9,  10,  10,  10,  10,
      11,  11,  11,  11,  11,  11,  11,  11,  12,  13,  14,  14,  15,  16,  16,  16,
      17,  17,  17,  17,  17,  17,  17,  17,  18,  18,  19,  20,  21,  21,  22,  22,
@@ -5438,29 +5488,31 @@
     385, 385, 385, 385, 385, 385, 385, 385, 385, 385, 385, 385, 385, 385, 385, 385,
     385, 385, 385, 385, 385, 386, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387,
     387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387,
     387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387,
     387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387,
     387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 387, 388,
     389, 389, 389, 389, 389, 389, 389, 389, 389, 389, 389, 389, 389, 389, 389, 389,
-    389, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194,
-    390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390,
-    390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390,
+    389, 389, 389, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194,
     390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 390,
-    390, 390, 390, 390, 390, 390, 390, 390, 390, 390, 391, 392, 392, 392, 392, 392,
-    392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392,
-    392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392,
-    392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392,
-    392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 392, 393, 194, 194,
-    394, 394, 394, 394, 194, 194, 194, 194, 395, 395, 395, 395, 395, 395, 395, 396,
+    390, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194,
+    391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391,
+    391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391,
+    391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 391,
+    391, 391, 391, 391, 391, 391, 391, 391, 391, 391, 392, 393, 393, 393, 393, 393,
+    393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393,
+    393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393,
+    393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393,
+    393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 393, 394, 194, 194,
+    395, 395, 395, 395, 194, 194, 194, 194, 396, 396, 396, 396, 396, 396, 396, 397,
     194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194, 194,
-    397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397,
-    397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397, 397,
     398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398,
-    398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398
+    398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398, 398,
+    399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399,
+    399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399, 399
 };
 
 static RE_UINT16 re_block_table_3[] = {
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
@@ -6233,35 +6285,37 @@
     319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319,
     319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319,
     319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319, 319,
     320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320,
     320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320,
     320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320,
     320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320, 320,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321,
     321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321,
     321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321, 321,
     322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322,
     322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322,
-    322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322, 322,
-    323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323,
     323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323,
     323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323,
     323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323, 323,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
     324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324,
     324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324,
+    324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324,
+    324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324, 324,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
     325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325,
     325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325,
-    325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325, 325,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
     326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326,
     326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326,
+    326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326, 326,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327,
     327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327,
-    327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327, 327
+    328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328,
+    328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328, 328
 };
 
 RE_UINT32 re_get_block(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 v;
@@ -10493,16 +10547,16 @@
     23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 13, 35, 33, 33,
     33, 36, 33, 33, 33, 33, 33, 33, 33, 33, 37, 38, 13, 13, 13, 13,
     13, 39, 13, 40, 33, 33, 33, 33, 33, 33, 33, 41, 42, 33, 33, 43,
     33, 33, 33, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 33,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 56, 13, 13, 13, 57, 58, 13,
-    13, 13, 13, 59, 13, 13, 13, 13, 13, 13, 60, 33, 33, 33, 61, 33,
-    13, 13, 13, 13, 62, 13, 13, 13, 63, 33, 33, 33, 33, 33, 33, 33,
+    13, 13, 13, 59, 13, 13, 13, 13, 13, 13, 60, 61, 33, 33, 62, 33,
+    13, 13, 13, 13, 63, 13, 13, 13, 64, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
@@ -10538,26 +10592,26 @@
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
-    64, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
+    65, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33, 33,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
-    20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 65,
+    20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 66,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
-    20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 65
+    20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 66
 };
 
 static RE_UINT16 re_general_category_table_2[] = {
       0,   1,   2,   3,   0,   4,   5,   6,   7,   8,   9,  10,  11,  12,  13,  14,
       7,  15,  16,  17,  18,  19,  20,  21,  22,  22,  22,  23,  24,  25,  26,  27,
      28,  29,  17,   7,  30,   7,  31,   7,   7,  32,  33,  17,  34,  35,  36,  37,
      38,  39,  40,  41,  39,  39,  42,  43,  44,  45,  46,  39,  39,  47,  48,  49,
@@ -10599,100 +10653,102 @@
     294, 294, 294, 294, 294, 294, 294, 294, 294, 294, 294, 294, 294, 294, 294, 294,
     295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295,
     295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295,
     295, 295, 295, 295, 295, 295, 295, 295,  39,  39,  39,  39,  39,  39,  39,  39,
      39,  39,  39, 296,  39,  39, 297, 100, 298, 299, 300,  39,  39, 301, 302,  39,
      39,  39,  39,  39,  39,  39,  39,  39,  39, 303, 304,  39, 305,  39, 306, 307,
     308, 309, 310, 311,  39,  39,  39, 312, 313,   2, 314, 315, 316, 143, 317, 318,
-    319, 320, 321, 100,  39,  39,  39, 322, 323, 324, 194, 325, 326, 327, 328, 329,
-    100, 100, 100, 100, 276,  39, 330, 331,  39, 332, 333, 334, 335,  39, 336, 100,
-     28, 337, 338,  39, 339, 340, 341, 342,  39, 343,  39, 344, 345, 346, 100, 100,
-     39,  39,  39,  39,  39,  39,  39,  39,  39, 231, 142, 347, 348, 349, 100, 100,
-    350, 351, 352, 353, 143, 354, 100, 355, 356, 357, 100, 100,  39, 358, 359, 209,
-    360, 361, 362, 363, 364, 100, 365, 366,  39, 367, 368, 369, 370, 371, 100, 100,
-     39,  39, 372, 100,  28, 373,  17, 374,  39, 375, 100, 100, 100, 100, 100, 100,
-    100, 100, 100, 376,  39, 377, 100, 378, 364, 379, 380, 381, 382, 381, 383, 231,
-    384, 385, 386, 387, 160, 388, 389, 390, 391, 392, 393, 394, 160, 395, 396, 397,
-    398, 399, 400, 100, 401, 402, 403, 404, 405, 406, 407, 408, 100, 100, 100, 100,
-     39, 409, 410, 411,  39, 412, 413, 100, 100, 100, 100, 100,  39, 414, 415, 100,
-     39, 416, 417, 418,  39, 419, 420, 100, 122, 421, 422, 100, 100, 100, 100, 100,
-     39, 423, 100, 100, 100,  28,  17, 424, 425, 426, 427, 100, 100, 428, 429, 430,
-    431, 432, 433,  39, 434, 435,  39, 139, 436, 100, 100, 100, 100, 100, 100, 100,
-    437, 438, 439, 440, 441, 442, 100, 100, 443, 444, 445, 446, 447, 420, 100, 100,
-    100, 100, 100, 100, 100, 100, 100, 448, 449, 450, 451, 100, 100, 452, 453, 454,
+    319, 320, 321, 100,  39,  39,  39, 322, 323, 324, 194, 325, 326, 327, 239, 328,
+    100, 100, 100, 100, 276,  39, 329, 330,  39, 331, 332, 333, 334,  39, 335, 100,
+     28, 336, 337,  39, 338, 339, 340, 341,  39, 342,  39, 343, 344, 345, 100, 100,
+     39,  39,  39,  39,  39,  39,  39,  39,  39, 231, 142, 346, 347, 348, 100, 100,
+    349, 350, 351, 352, 143, 353, 100, 354, 355, 356, 100, 100,  39, 357, 358, 209,
+    359, 360, 361, 362, 363, 100, 364, 365,  39, 366, 367, 368, 369, 370, 100, 100,
+     39,  39, 371, 100,  28, 372,  17, 373,  39, 374, 100, 100, 100, 100, 100, 100,
+    100, 100, 100, 375,  39, 376, 100, 377, 363, 378, 379, 380, 381, 380, 382, 231,
+    383, 384, 385, 386, 160, 387, 388, 389, 390, 391, 392, 393, 160, 394, 395, 396,
+    397, 398, 399, 100, 400, 401, 402, 403, 404, 405, 406, 407, 100, 100, 100, 100,
+     39, 408, 409, 410,  39, 411, 412, 100, 100, 100, 100, 100,  39, 413, 414, 100,
+     39, 415, 416, 417,  39, 418, 419, 100, 122, 420, 421, 100, 100, 100, 100, 100,
+     39, 422, 100, 100, 100,  28,  17, 423, 424, 425, 426, 100, 100, 427, 428, 429,
+    430, 431, 432,  39, 433, 434,  39, 139, 435, 100, 100, 100, 100, 100, 100, 100,
+    436, 437, 438, 439, 440, 441, 100, 100, 442, 443, 444, 445, 446, 419, 100, 100,
+    100, 100, 100, 100, 100, 100, 100, 447, 448, 449, 450, 100, 100, 451, 452, 453,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39, 297, 100, 100, 100,
-    194, 194, 194, 455,  39,  39,  39,  39,  39,  39, 456, 100, 100, 100, 100, 100,
+    194, 194, 194, 454,  39,  39,  39,  39,  39,  39, 455, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
-    100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 381,  39,  39, 457,
-     39, 458, 459, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
+    100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 380,  39,  39, 456,
+     39, 457, 458, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
-     39,  39, 422, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
+     39,  39, 421, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
-     39, 139, 143, 460,  39, 143, 461, 462,  39, 463, 464, 465, 466, 100, 100, 100,
+     39, 139, 143, 459,  39, 143, 460, 461,  39, 462, 463, 464, 465, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
-    100, 100,  28,  17, 467, 100, 100, 100,  39,  39, 468, 469, 470, 100, 100, 471,
+    100, 100,  28,  17, 466, 100, 100, 100,  39,  39, 467, 468, 469, 100, 100, 470,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
-     39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39, 472,
-     39,  39,  39,  39,  39,  39, 142, 100, 372, 100, 100, 100, 100, 100, 100, 100,
+     39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39, 471,
+     39,  39,  39,  39,  39,  39, 142, 100, 371, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
-    100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 473,
-     39,  39,  39,  39,  39,  39,  39,  39,  39, 474, 475, 476,  39,  39,  39,  39,
+    100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 472,
+     39,  39,  39,  39,  39,  39,  39,  39,  39, 473, 474, 475,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39, 293, 100, 100, 100, 100, 100, 100, 100, 100,
-     39,  39,  39, 477, 478, 479, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
+     39,  39,  39, 476, 477, 478, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
-    100, 100, 100, 100, 100, 100, 100, 100,  22, 480, 481, 149, 149, 149, 482, 100,
-    149, 149, 149, 149, 149, 149, 149, 238, 149, 483, 149, 484, 485, 486, 149, 208,
-    149, 149, 487, 100, 100, 100, 488, 488, 149, 149, 489, 490, 100, 100, 100, 100,
-    491, 492, 493, 494, 495, 496, 497, 498, 499, 500, 501, 502, 503, 491, 492, 504,
-    494, 505, 506, 507, 498, 508, 509, 510, 511, 512, 513, 514, 515, 516, 517, 518,
+    100, 100, 100, 100, 100, 100, 100, 100,  22, 479, 480, 149, 149, 149, 481, 100,
+    149, 149, 149, 149, 149, 149, 149, 238, 149, 482, 149, 483, 484, 485, 149, 208,
+    149, 149, 486, 100, 100, 100, 487, 487, 149, 149, 488, 489, 100, 100, 100, 100,
+    490, 491, 492, 493, 494, 495, 496, 497, 498, 499, 500, 501, 502, 490, 491, 503,
+    493, 504, 505, 506, 497, 507, 508, 509, 510, 511, 512, 513, 514, 515, 516, 517,
     149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149,
-     22, 519,  22, 520, 521, 522, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
+     22, 518,  22, 519, 520, 521, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
-    100, 100, 100, 100, 100, 100, 100, 100, 523, 524, 100, 100, 100, 100, 100, 100,
-    525, 526, 171, 527, 528, 100, 100, 100,  39, 529, 530, 100, 100, 100, 100, 100,
-    100, 100, 100, 100, 381, 531,  39, 532, 100, 100, 100, 100, 100, 100, 100, 100,
-    100, 100, 100, 100, 100, 100, 381, 533, 100, 100, 100, 100, 100, 100, 100, 100,
-    100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 534,
-     39,  39,  39,  39,  39,  39, 535, 100,  28, 536, 537, 100, 100, 100, 100, 100,
+    100, 100, 100, 100, 100, 100, 100, 100, 522, 523, 100, 100, 100, 100, 100, 100,
+    524, 525, 171, 526, 527, 100, 100, 100,  39, 528, 529, 100, 100, 100, 100, 100,
+    100, 100, 100, 100, 380, 530,  39, 531, 100, 100, 100, 100, 100, 100, 100, 100,
+    100, 100, 100, 100, 100, 100, 380, 532, 100, 100, 100, 100, 100, 100, 100, 100,
+    100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 533,
+     39,  39,  39,  39,  39,  39, 534, 100,  28, 535, 536, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
-    100, 100, 100, 538, 209, 539, 100, 100, 540, 541, 100, 100, 100, 100, 100, 100,
-    542, 543, 544, 545, 546, 547, 100, 548, 100, 100, 100, 100, 100, 100, 100, 100,
-    149, 549, 149, 149, 237, 550, 551, 238, 552, 149, 149, 149, 149, 553, 100, 554,
-    555, 556, 557, 558, 100, 100, 100, 100, 149, 149, 149, 149, 149, 149, 149, 559,
+    100, 100, 100, 537, 209, 538, 100, 100, 539, 540, 100, 100, 100, 100, 100, 100,
+    541, 542, 543, 544, 545, 546, 100, 547, 100, 100, 100, 100, 100, 100, 100, 100,
+    149, 548, 149, 149, 237, 549, 550, 238, 551, 149, 149, 149, 149, 552, 100, 553,
+    554, 555, 556, 557, 100, 100, 100, 100, 149, 149, 149, 149, 149, 149, 149, 558,
     149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149, 149,
-    149, 149, 149, 149, 149, 149, 560, 561, 149, 149, 149, 562, 149, 149, 563, 564,
-    549, 149, 565, 149, 566, 567, 100, 100, 149, 149, 149, 149, 149, 149, 149, 149,
-    149, 149, 237, 568, 569, 570, 571, 572, 149, 149, 149, 149, 573, 149, 208, 574,
+    149, 149, 149, 149, 149, 149, 559, 560, 149, 149, 149, 561, 149, 149, 562, 563,
+    548, 149, 564, 149, 565, 566, 100, 100, 149, 149, 149, 149, 149, 149, 149, 149,
+    149, 149, 237, 567, 568, 569, 570, 571, 149, 149, 149, 149, 572, 149, 208, 573,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39, 100,  39,  39,  39,  39,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39,  39,  39, 297,  39,  39,  39,  39,  39,  39,
-    339,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
+    338,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
+     39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
+     39,  39,  39,  39,  39, 574,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
-     39,  39,  39,  39,  39, 575,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
+     39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39, 575,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
-     39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39, 576,
+     39,  39, 338, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
-    339, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
+    338, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  53,  39,  39,  39,  39,  39,
      39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,
-     39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39, 466, 100, 100,
-    577, 578, 578, 578, 100, 100, 100, 100,  22,  22,  22,  22,  22,  22,  22, 579,
+     39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39,  39, 465, 100, 100,
+    576, 577, 577, 577, 100, 100, 100, 100,  22,  22,  22,  22,  22,  22,  22, 578,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295,
-    295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 580
+    295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 295, 579
 };
 
 static RE_UINT8 re_general_category_table_3[] = {
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      2,  3,  3,  3,  4,  3,  3,  3,  5,  6,  3,  7,  3,  8,  3,  3,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  3,  3,  7,  7,  7,  3,
@@ -11167,30 +11223,30 @@
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,  0,  0,  0,
+    14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
      2,  3,  3,  3, 14, 21, 15, 25,  5,  6,  5,  6,  5,  6,  5,  6,
      5,  6, 14, 14,  5,  6,  5,  6,  5,  6,  5,  6,  8,  5,  6,  6,
     14, 25, 25, 25, 25, 25, 25, 25, 25, 25, 22, 22, 22, 22, 24, 24,
      8, 21, 21, 21, 21, 21, 14, 14, 25, 25, 25, 21, 15,  3, 14, 14,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     15, 15, 15, 15, 15, 15, 15,  0,  0, 22, 22, 11, 11, 21, 21, 15,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,  3, 21, 21, 21, 15,
      0,  0,  0,  0,  0, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
      0, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,  0,
     14, 14, 18, 18, 18, 18, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
-    14, 14, 14, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    14, 14, 14, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 14,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 18, 18, 18, 18, 18, 18, 18, 18,
     14, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
@@ -11344,16 +11400,14 @@
     18, 18, 18, 18,  0,  0,  0, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25,
     25, 25, 25, 25, 25, 18, 18, 18, 18, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 18, 18, 14, 14, 14,  0,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,  0,  0,
     14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 22,  0,  0,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     15,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     22, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,  0,  0,  0,  0,
     18, 18, 18, 18,  0,  0,  0,  0,  0,  0,  0,  0,  0, 15, 15, 15,
@@ -11841,15 +11895,15 @@
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14,  0, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,
     15, 15,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     15,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
      0, 17,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
@@ -11882,16 +11936,16 @@
     20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 17, 30, 13, 31, 17, 17,
     17, 32, 17, 17, 17, 17, 17, 17, 17, 17, 33, 34, 13, 13, 13, 13,
     13, 35, 13, 36, 17, 17, 17, 17, 17, 17, 17, 37, 38, 17, 17, 39,
     17, 17, 17, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 17,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 52, 13, 13, 13, 53, 54, 13,
-    13, 13, 13, 55, 13, 13, 13, 13, 13, 13, 56, 17, 17, 17, 57, 17,
-    13, 13, 13, 13, 58, 13, 13, 13, 59, 17, 17, 17, 17, 17, 17, 17,
+    13, 13, 13, 55, 13, 13, 13, 13, 13, 13, 56, 57, 17, 17, 58, 17,
+    13, 13, 13, 13, 59, 13, 13, 13, 60, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
@@ -11927,26 +11981,26 @@
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
-    60, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
+    61, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
-    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 61,
+    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 62,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
-    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 61
+    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 62
 };
 
 static RE_UINT16 re_graph_table_2[] = {
       0,   1,   2,   3,   0,   1,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   4,   5,   6,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   7,   8,   2,   9,   2,  10,  11,
       2,   2,   2,   2,   2,   2,   2,   2,  12,   2,  13,   2,   2,  14,   2,  15,
@@ -11975,43 +12029,43 @@
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,  89,   2, 117,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2, 118,   2,   2,   2,   2,   2, 119,   2,   2,   2,   2,   2,   2, 120, 121,
       2, 122,   2, 119,   2,   2, 123,   2,   2,   2, 124,  68,   2,   2, 125,   3,
       2,  74, 126,   2,   2,   2, 127,  74, 128, 129,   2,  83,   2,   2,   2, 130,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
-      2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2, 116, 131,  53,
+      2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2, 131, 132,  53,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
-      2,   2,   2,  87,   2,   2,  69,   0, 132, 133, 134,   2,   2,   2, 135,   2,
-      2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2, 136,   2, 137, 138,
+      2,   2,   2,  87,   2,   2,  69,   0, 133, 134, 135,   2,   2,   2, 136,   2,
+      2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2, 137,   2, 138, 113,
      69,   2, 139, 140,   2,   2,   2,  86,   1,   2,   2,   2,   2,   3, 141, 142,
-    143, 144, 145,   0,   2,   2,   2,  94, 146, 147,   2,   2, 102, 148, 138,  77,
+    143, 144, 145,   0,   2,   2,   2,  94, 146, 147,   2,   2, 102, 148, 113,  77,
       0,   0,   0,   0,  68,   2, 104,  53,   2, 149,  18,  94, 150,   2, 151,   0,
       2,   2,   2,   2,  77, 152, 153,  53,   2,  10,   2, 154, 155, 156,   0,   0,
       2,   2,   2,   2,   2,   2,   2,   2,   2,  74,  79, 157, 158, 159,   0,   0,
-    160, 161, 108,   2,   3, 162,   0, 163, 164, 165,   0,   0,   2, 166, 136,   2,
+    160, 161, 108,   2,   3, 162,   0, 163, 164, 165,   0,   0,   2, 166, 137,   2,
     167, 168, 169,   2,   2,   0,   2, 170,   2, 171, 172, 173, 174, 175,   0,   0,
       2,   2, 176,   0,   2, 177,   2, 178,   2, 179,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   3,   2, 180,   0, 181,   2,  10,  69, 138, 182, 138, 118,  74,
+      0,   0,   0,   3,   2, 180,   0, 181,   2,  10,  69, 113, 182, 113, 118,  74,
       2,   2, 183,  73,   2,   2, 184, 185,   2,  96,  10,  74,   2,   2,   2, 186,
     187,   2, 188,   0, 189, 152,   2, 190,  20, 191, 192, 193,   0,   0,   0,   0,
       2,   2, 194, 188,   2,   2, 179,   0,   0,   0,   0,   0,   2, 172,  77,   0,
       2,   2, 195, 196,   2,  69, 182,   0,  15,  83, 105,   0,   0,   0,   0,   0,
       2,  53,   0,   0,   0,   2,   2, 197, 198, 199, 200,   0,   0, 201,   4, 202,
       2,   2,  10,   2,   2, 203,   2,  72, 182,   0,   0,   0,   0,   0,   0,   0,
-    204, 205, 206,  89, 136, 207,   0,   0, 208, 209, 179, 210, 211, 182,   0,   0,
+    204, 205, 206,  89, 137, 207,   0,   0, 208, 209, 179, 210, 211, 182,   0,   0,
       0,   0,   0,   0,   0,   0,   0,  72, 212, 213,  69,   0,   0, 214,   2, 215,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,  69,   0,   0,   0,
       2,   2,   2, 216,   2,   2,   2,   2,   2,   2, 217,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 138,   2,   2, 177,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 113,   2,   2, 177,
       2,   2,  79,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2, 105,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,  72,   3, 218,   2,   3, 152, 219,   2,   2, 220, 221, 222,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -12033,16 +12087,16 @@
       2,   2,  96,   2,  60, 234, 235,   2, 236, 237, 238,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2, 239,   2,   2,   2,   2,   2,   2,   2,   2, 240,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2, 241, 242,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   3, 243,   0,   0,   0,   0,   0,   0,
     244, 245,   2, 246, 247,   0,   0,   0,   2, 248, 249,   0,   0,   0,   0,   0,
-      0,   0,   0,   0, 138,  88,   2, 165,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 138,  69,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0, 113,  88,   2, 165,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 113,  69,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 250,
       2,   2,   2,   2,   2,   2, 251,   0,   2,   2, 252,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0, 253,   2, 254,   0,   0,   1,  77,   0,   0,   0,   0,   0,   0,
     235, 255, 256, 257, 258, 259,   0, 260,   0,   0,   0,   0,   0,   0,   0,   0,
       2,  83,   2,   2,  75, 261, 262,  79,   2,   2,   2,   2,   2, 246,   0, 263,
     203,  53, 264, 233,   0,   0,   0,   0,   2,   2,   2,   2,   2,   2,   2,   2,
@@ -12055,15 +12109,17 @@
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,  69,   2,   2,   2,   2,   2,   2,
      77,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2, 272,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
-      2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2, 148,
+      2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2, 103,
+      2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
+      2,   2,  77,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
      77,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,  18,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2, 222,   0,   0,
     273,   2,   2,   2,   0,   0,   0,   0,   2,   2,   2,   2,   2,   2,   2, 222,
@@ -12097,21 +12153,21 @@
     255,   3, 255, 199, 255, 255, 255, 207, 255, 255, 255, 159, 255,  63, 255, 255,
     255, 127,   0,   0, 255,  31, 255, 255, 255, 255,  15, 240, 255, 255, 255, 248,
     255, 227, 255, 255, 255,   1, 255, 255, 255, 255, 255,   7,  63,  63, 255, 170,
     255, 255, 223, 255, 223, 255, 207, 239, 255, 255, 220, 127,   0, 248, 255, 255,
     255, 124, 255, 255, 223, 255, 243, 255, 255, 127, 255,  31,   1,   0, 255, 255,
     255, 255,   1,   0, 127,   0,   0,   0, 255,   7,   0,   0, 255, 255, 207, 255,
     255, 255, 191, 255, 255, 255,  15, 254, 255, 128,   1, 128, 127, 127, 127, 127,
-    255, 255, 255, 251,   0,   0, 255,  15, 224, 255, 255, 255, 255, 127, 255, 255,
-     15,   0, 255, 255, 127,   0, 255, 255, 255,  15,   0,   0, 255, 255, 255,   0,
+    255, 255, 255, 251,   0,   0, 255, 255, 224, 255, 255, 255, 255, 127, 255, 255,
+     15, 128, 255, 255, 127,   0, 255, 255, 255,  15,   0,   0, 255, 255, 255,   0,
     255,   7, 235,   3,   0,   0, 252, 255, 255,  31, 255,   3,  63, 192, 255,   3,
     255, 255,  15, 128, 255, 191, 255, 195, 255,  63, 255, 243,   7,   0,   0, 248,
-    126, 126, 126,   0, 127, 127, 255, 255, 255,  63, 255,   3, 127, 248, 255, 255,
-    127,   0, 248, 224, 255, 255, 127,  95, 219, 255, 255, 255,   7,   0, 248, 255,
-    255, 255, 252, 255, 255, 128,   0,   0,   0,   0, 255, 255, 255, 255, 247, 255,
+    126, 126, 126,   0, 127, 127, 255, 255, 255,  63, 255,   3,  15,   0, 255, 255,
+    127, 248, 255, 255, 127,   0, 248, 224, 255, 255, 127,  95, 219, 255, 255, 255,
+      7,   0, 248, 255, 255, 255, 252, 255, 255, 128,   0,   0, 255, 255, 247, 255,
     127,  15, 223, 255, 252, 252, 252,  28, 127, 127,   0,  62, 255, 239, 255, 255,
     127, 255, 255, 183, 255,  63, 255,  63, 135, 255, 255, 255, 255, 255, 143, 255,
       1,   0,   0,   0,  15, 224, 255, 255, 255, 255, 255, 191,  15, 255,  63,   0,
     255,   3, 255, 255, 255, 255,  15, 255,  15, 128, 255, 247, 255, 247, 183, 255,
     251, 255, 251,  27, 255,   0,   0,   0, 191, 255, 255, 255, 255, 255, 253,   7,
      63, 253, 255, 255, 255, 255, 191, 145, 128, 255,   0,   0, 255, 255,  55, 248,
     255, 255, 255, 143, 255, 255, 255, 131, 255, 255, 255, 240, 111, 240, 239, 254,
@@ -12172,16 +12228,16 @@
     20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 17, 30, 13, 31, 17, 17,
     17, 32, 17, 17, 17, 17, 17, 17, 17, 17, 33, 34, 13, 13, 13, 13,
     13, 35, 13, 36, 17, 17, 17, 17, 17, 17, 17, 37, 38, 17, 17, 39,
     17, 17, 17, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 17,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 52, 13, 13, 13, 53, 54, 13,
-    13, 13, 13, 55, 13, 13, 13, 13, 13, 13, 56, 17, 17, 17, 57, 17,
-    13, 13, 13, 13, 58, 13, 13, 13, 59, 17, 17, 17, 17, 17, 17, 17,
+    13, 13, 13, 55, 13, 13, 13, 13, 13, 13, 56, 57, 17, 17, 58, 17,
+    13, 13, 13, 13, 59, 13, 13, 13, 60, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
@@ -12265,43 +12321,43 @@
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1, 154,   1, 155,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1, 156,   1, 157, 131,   1,   1, 158,   1,   1,   1,   1,   1,   1, 159, 160,
     161, 162,   1, 163,   1,   1, 164, 165,   1, 166, 167,  93,  29, 168, 169, 170,
       1, 171, 172, 173,   1, 174, 175, 176, 177, 178,   1, 111,   1,   1,   1, 179,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 153, 180, 181,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 180, 181, 182,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   1,   1,   1,   1,   1,   1,   1,   1,
-      1,   1,   1, 182,   1,   1,  94,   0, 183, 184, 185,   1,   1,   1, 186,   1,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 187,   1, 188, 189,
-    190, 189, 191, 192,   1,   1,   1,  93,  69,   1,   1,   1, 131,   2, 193, 194,
-    195, 196, 197,   0,   1,   1,   1,  92, 198, 199,   1,   1, 137, 138, 189,  93,
+      1,   1,   1, 183,   1,   1,  94,   0, 184, 185, 186,   1,   1,   1, 187,   1,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 188,   1, 189, 148,
+    190, 148, 191, 192,   1,   1,   1,  93,  69,   1,   1,   1, 131,   2, 193, 194,
+    195, 196, 197,   0,   1,   1,   1,  92, 198, 199,   1,   1, 137, 138, 148,  93,
       0,   0,   0,   0,  93,   1, 200, 201,   1, 202,  26, 107, 203,   1, 204,   0,
-      1,   1,   1,   1, 131, 149, 205, 181,   1, 206,   1, 207, 208, 209,   0,   0,
+      1,   1,   1,   1, 131, 149, 205, 182,   1, 206,   1, 207, 208, 209,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1, 144, 107, 210, 211, 212,   0,   0,
-    213, 214, 141,   1,   2, 215,   0, 216, 217, 218,   0,   0,   1, 219, 187,   1,
+    213, 214, 141,   1,   2, 215,   0, 216, 217, 218,   0,   0,   1, 219, 188,   1,
     220, 107, 221,   1,   1,   0,   1, 222,   1, 223, 224, 225, 226, 227,   0,   0,
       1,   1, 228,   0,   1, 229,   1, 230,   1, 231,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   2,   1, 232,   0,   0,   1, 206, 233, 189, 234, 189, 156, 144,
+      0,   0,   0,   2,   1, 232,   0,   0,   1, 206, 233, 148, 234, 148, 156, 144,
     235, 163, 236, 237, 121, 238, 239, 240,  29, 241, 206, 242, 121, 243, 244, 245,
     246, 247, 138,   0, 248, 149,   2, 249,  45, 250, 251, 252,   0,   0,   0,   0,
       1, 163, 253, 254,   1, 255, 256,   0,   0,   0,   0,   0,   1, 257, 201,   0,
       1, 258, 259, 260,   1, 261,  28,   0,  92, 262, 139,   0,   0,   0,   0,   0,
       1, 263,   0,   0,   0,   1,   1, 264, 265, 266, 267,   0,   0, 268, 269, 270,
     271, 272, 273,   1, 274, 275,   1,  96,  28,   0,   0,   0,   0,   0,   0,   0,
     276, 277, 278, 154,  19, 279,   0,   0, 280, 200, 281, 282, 283,  28,   0,   0,
       0,   0,   0,   0,   0,   0,   0, 284, 285, 286, 287,   0,   0, 288,   1, 289,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,  94,   0,   0,   0,
       1,   1,   1, 290,   1,   1,   1,   1,   1,   1, 252,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 189,   1,   1, 229,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 148,   1,   1, 229,
       1,  19, 291,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1, 139,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,  96,   2, 292,   1,   2, 149, 293,   1, 294, 295, 296,  19,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -12309,51 +12365,53 @@
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 163,
       1,   1,   1,   1,   1,   1, 107,   0, 228,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 299,
       1,   1,   1,   1,   1,   1,   1,   1,   1, 300, 301, 302,   1,   1,   1,   1,
-      1,   1,   1,   1,   1,   1,   1, 181,   0,   0,   0,   0,   0,   0,   0,   0,
+      1,   1,   1,   1,   1,   1,   1, 182,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1, 303, 304,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 189,   1,   1,   1, 252,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 148,   1,   1,   1, 252,   0,
       1,   1,   1,   1,   1,   1,   1, 107,   1, 305,   1, 306, 307, 292,   1,  15,
       1,   1, 308,   0,   0,   0, 147, 147,   1,   1, 144,  96,   0,   0,   0,   0,
       1,   1, 132,   1, 309, 310, 311,   1, 312, 313, 314,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1, 315,   1,   1,   1,   1,   1,   1,   1,   1, 316,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       0, 317,   0, 318, 319,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   2, 320,   0,   0,   0,   0,   0,   0,
-      0, 189,   1, 116,   0,   0,   0,   0,   1, 321, 322,   0,   0,   0,   0,   0,
-      0,   0,   0,   0, 189, 116,   1, 323,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 189, 324,   0,   0,   0,   0,   0,   0,   0,   0,
+      0, 148,   1, 116,   0,   0,   0,   0,   1, 321, 322,   0,   0,   0,   0,   0,
+      0,   0,   0,   0, 148, 116,   1, 323,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 148, 324,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 325,
       1,   1,   1,   1,   1,   1, 326,   0,   1,   1, 327,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0, 328,   1, 329,   0,   0,  69, 131,   0,   0,   0,   0,   0,   0,
     311, 330, 331, 332, 333, 334,   0, 335,   0,   0,   0,   0,   0,   0,   0,   0,
       1, 111,   1,   1, 147, 336, 337, 107,   1,   1,   1,   1,   1, 116,   0, 338,
-    275, 181, 339, 340,   0,   0,   0,   0,   1,   1,   1,   1,   1,   1,   1,   1,
+    275, 182, 339, 340,   0,   0,   0,   0,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1, 219, 341,   1,   1,   1, 150,   1,   1,  94, 342,
     111,   1, 343,   1, 206, 344,   0,   0,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1, 147, 345, 126, 203, 346, 221,   1,   1,   1,   1, 191,   1,  15, 190,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   0,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,  94,   1,   1,   1,   1,   1,   1,
     131,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1, 239,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 138,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 347,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
+      1,   1, 131,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
     131,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,  26,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,  19,   0,   0
 };
@@ -12392,25 +12450,25 @@
     255,   7, 240, 127, 252, 255, 255, 255, 195, 196, 255, 255, 191,  92,  12, 240,
     255,  15,  48, 248, 255, 227, 255, 255, 255,   1, 255, 255, 255, 255, 255, 231,
     255,   0,   8,   0,   2, 222, 239,   4,  63,  63, 255, 170, 255, 255, 255,  63,
     255, 255, 223, 255, 223, 255, 207, 239, 255, 255, 220, 127, 255, 128, 255, 255,
       0,   0, 243, 255, 255, 127, 255,  31,   1,   0,   0,   0, 127,   0,   0,   0,
     255, 255, 207, 255, 255, 255, 191, 255, 255, 127,  12, 254, 255, 128,   1,   0,
     255, 255, 127,   0, 127, 127, 127, 127, 255, 255, 255, 251, 255, 255,  15,   0,
-      0,   0, 255,  15, 255,   3, 255, 255, 255, 255, 127, 248, 224, 255, 255, 255,
-    255, 127, 255, 255,  15,   0, 255, 255, 255,  31, 255, 255, 127,   0, 255, 255,
+      0,   0, 255, 255, 255,   3, 255, 255, 255, 255, 127, 248, 224, 255, 255, 255,
+    255, 127, 255, 255,  15, 128, 255, 255, 255,  31, 255, 255, 127,   0, 255, 255,
     255,  15,   0,   0, 255, 127,   8, 192, 255, 255, 252,   0, 255,   7, 235,   3,
       0,   0, 252, 255, 187, 247, 255, 255, 159,  15, 255,   3, 255, 255, 255,   0,
      15, 192, 255,   3,   0,   0, 252, 127,  63, 192, 255, 255, 127,   0,  12, 128,
     255, 255,  55, 204, 255, 191, 255, 195, 223, 255, 255, 127, 255, 129,  25,   0,
     247,  47, 255, 243, 255, 255, 255, 239, 255, 255,  98,  62,   5,   0,   0, 248,
     255, 207,  63,   0, 126, 126, 126,   0, 127, 127, 255, 255, 223,  30, 255,   3,
-    127, 248, 255, 255, 255, 255, 255,  15, 255,  63, 255, 255, 127,   0, 248, 160,
-    255, 255, 127,  95, 219, 255, 255, 255,   7,   0, 248, 255, 255, 255, 252, 255,
-    255, 128,   0,   0,   0,   0, 255, 255,   0,   0, 255,   3, 255, 255, 247, 255,
+     15,   0, 255, 255, 127, 248, 255, 255, 255, 255, 255,  15, 255,  63, 255, 255,
+    127,   0, 248, 160, 255, 255, 127,  95, 219, 255, 255, 255,   7,   0, 248, 255,
+    255, 255, 252, 255, 255, 128,   0,   0,   0,   0, 255,   3, 255, 255, 247, 255,
     127,  15, 223, 255, 252, 252, 252,  28, 127, 127,   0,  48, 255, 239, 255, 255,
     127, 255, 255, 183, 255,  63, 255,  63, 135, 255, 255, 255, 255, 255, 143, 255,
     255, 255,   1,   0, 254, 255, 255,  15,  15, 224, 255, 255, 255, 255, 255, 191,
      15, 255,  63,   0, 255, 255,  15, 255, 255,   0, 255, 255,  15, 128, 255, 247,
     255, 247, 183, 255, 251, 255, 251,  27, 255,   0,   0,   0, 191, 255, 255, 255,
     255, 255, 253,   7,  63, 253, 255, 255, 255, 255, 191, 145, 128, 255,   0,   0,
     255, 255,  55, 248, 255, 255, 255, 143, 255, 255, 255, 131, 255, 255, 255, 240,
@@ -12441,15 +12499,15 @@
     255, 207, 255, 255,   0,   0, 128,   7,   0, 224, 223, 255, 239,  15,   0,   0,
     224,   7,   0,   0, 255,  31, 128,  63, 255, 195,   0,   0, 255,  15, 255, 131,
     255,  15, 255,   3, 127, 111, 255, 127, 159, 255,   0,   0,  15,   8, 255, 195,
       0,   0, 254, 255, 255, 255,  31,   0, 150, 254, 247,  10, 132, 234, 150, 170,
     150, 247, 247,  94, 255, 251, 255,  15, 238, 251, 255,  15,   0,   0,   3,   0,
     255, 127, 254, 255, 254, 255, 254, 255, 192, 255, 255, 255, 255,   1,   3,   0,
      63,   0,   0,   0, 255,  31, 255,  31, 255,  15,   1,   0, 255,   0, 255,   3,
-    255,  63,   3,   0, 255,  63, 255,  31,  63, 192, 255,  15
+    255,  63,   3,   0, 255,  63, 255,  31,  63, 192, 255,  15,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_grapheme_base(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -13819,29 +13877,242 @@
     v = re_hyphen_table_1[field_2];
     v = re_hyphen_table_2[(v << 5) | field_1];
     v = re_hyphen_table_3[(v << 2) | field_0];
 
     return (v >> offset) & 0x1;
 }
 
+/* ID_Compat_Math_Continue. */
+static RE_UINT8 re_id_compat_math_continue_table_1[] = {
+    0, 1, 1, 1, 1, 1, 1, 1, 2, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 3, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1
+};
+
+static RE_UINT8 re_id_compat_math_continue_table_2[] = {
+     0,  0,  0,  0,  0,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  2,  3,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     4,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  5,  6,  7,  7,  8,  8,  9,  9, 10,  0
+};
+
+static RE_UINT8 re_id_compat_math_continue_table_3[] = {
+      0,   0,   0,   0,   0,   0,  12,   2,   0,   0, 241, 127, 255, 127,   0,   0,
+    132,   0,   0,  64,   2,   0,   0,   8,   0,   0,   0,   8,   0,   0,  32,   0,
+      0, 128,   0,   0,   0,   2,   0,   0,   8,   0,   0,   0
+};
+
+RE_UINT32 re_get_id_compat_math_continue(RE_UINT32 codepoint) {
+    RE_UINT32 field_2;
+    RE_UINT32 field_1;
+    RE_UINT32 field_0;
+    RE_UINT32 offset;
+    RE_UINT32 v;
+
+    field_2 = codepoint >> 10;
+    field_1 = (codepoint >> 5) & 0x1F;
+    field_0 = (codepoint >> 3) & 0x3;
+    offset = codepoint & 0x7;
+
+    v = re_id_compat_math_continue_table_1[field_2];
+    v = re_id_compat_math_continue_table_2[(v << 5) | field_1];
+    v = re_id_compat_math_continue_table_3[(v << 2) | field_0];
+
+    return (v >> offset) & 0x1;
+}
+
+/* ID_Compat_Math_Start. */
+static RE_UINT8 re_id_compat_math_start_table_1[] = {
+    0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 2, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+};
+
+static RE_UINT8 re_id_compat_math_start_table_2[] = {
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 2, 3, 4, 4, 5, 5, 6, 6, 7, 0
+};
+
+static RE_UINT8 re_id_compat_math_start_table_3[] = {
+      0,   0,   0,   0, 132,   0,   0,  64,   2,   0,   0,   8,   0,   0,   0,   8,
+      0,   0,  32,   0,   0, 128,   0,   0,   0,   2,   0,   0,   8,   0,   0,   0
+};
+
+RE_UINT32 re_get_id_compat_math_start(RE_UINT32 codepoint) {
+    RE_UINT32 field_2;
+    RE_UINT32 field_1;
+    RE_UINT32 field_0;
+    RE_UINT32 offset;
+    RE_UINT32 v;
+
+    field_2 = codepoint >> 10;
+    field_1 = (codepoint >> 5) & 0x1F;
+    field_0 = (codepoint >> 3) & 0x3;
+    offset = codepoint & 0x7;
+
+    v = re_id_compat_math_start_table_1[field_2];
+    v = re_id_compat_math_start_table_2[(v << 5) | field_1];
+    v = re_id_compat_math_start_table_3[(v << 2) | field_0];
+
+    return (v >> offset) & 0x1;
+}
+
 /* ID_Continue. */
 static RE_UINT8 re_id_continue_table_1[] = {
      0,  1,  2,  3,  4,  5,  6,  7,  8,  9,  9, 10, 11, 12, 12, 12,
     12, 12, 12, 13, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 14, 15, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 16,  9,  9,  9,  9,  9,  9,  9,  9, 17, 18,
     19, 20, 21, 22, 23, 24, 25, 26, 27, 28,  9, 29, 12, 30,  9,  9,
      9, 31,  9,  9,  9,  9,  9,  9,  9,  9, 32, 33, 12, 12, 12, 12,
     12, 34, 12, 35,  9,  9,  9,  9,  9,  9,  9, 36, 37,  9,  9, 38,
      9,  9,  9, 39, 40, 41, 42, 43, 44, 45, 46, 47,  9,  9, 48,  9,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 49, 12, 12, 12, 50, 51, 12,
-    12, 12, 12, 52, 12, 12, 12, 12, 12, 12, 53,  9,  9,  9, 54,  9,
-    12, 12, 12, 12, 55, 12, 12, 12, 56,  9,  9,  9,  9,  9,  9,  9,
+    12, 12, 12, 52, 12, 12, 12, 12, 12, 12, 53, 54,  9,  9, 55,  9,
+    12, 12, 12, 12, 56, 12, 12, 12, 57,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -13877,15 +14148,15 @@
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-    57,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+    58,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -13908,106 +14179,108 @@
       6,   6,  83,   6,  84,  85,  86,   6,  87,   6,  88,  89,  90,   6,   6,  91,
      66,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,  92,   3,   6,   6,  93,  94,  95,  96,  97,   6,   6,  98,  99,
     100,   6,   6, 101,   6,  30,   6, 102, 103, 104, 105, 106,   6, 107, 108,   0,
      29,   6, 103, 109, 110, 111, 112,   0,   6,   6, 113, 114,   6,   6,   6,  96,
       6, 115, 116,  80, 117,  88, 118,  67,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,  91,   6, 119,  80,   6, 120, 121, 122,
-      0, 123, 124, 125, 126,   0, 126, 127, 128, 129, 130,   6, 131,   0,   0,   0,
+    123, 124, 125, 126, 127,   0, 127, 128, 129, 130, 131,   6, 132,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      6,   6,   6,   6,   6,   6,   6, 132,   6,  81,   6, 133, 134, 135, 135,   6,
+      6,   6,   6,   6,   6,   6,   6, 133,   6,  81,   6, 134, 135, 136, 136,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    136, 137,  66,   6, 138,  66,   6,  82, 139,  14,   6,   6, 112,   6,   0,  24,
+    137, 138,  66,   6, 139,  66,   6,   6, 140,  14,   6,   6, 112,   6,   0,  24,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6, 140,   0,  24,  80,   6,   6,   6,   6,   6,   6,   6,   6,
-    141, 142,   6, 143,   6,   6,   6,  26, 144, 145,   6,   6, 146,   6, 147, 148,
-      6, 149,   6,  96,   6,   6, 150, 151,   6, 152,  96,  77,   6,   6, 153, 103,
-      6, 134, 154, 155,   6,   6, 156, 157, 158, 159,  82,  79,   6,   6,   6, 160,
+      6,   6,   6,   6, 141,   0,  24,  80,   6,   6,   6,   6,   6,   6,   6,   6,
+    142, 143,   6, 144,   6,   6,   6,  26, 145, 146,   6,   6, 147,   6, 148, 149,
+      6, 150,   6,  96,   6,   6, 151, 152,   6, 153,  96,  77,   6,   6, 154, 103,
+      6, 135, 155, 156,   6,   6, 157, 158, 159, 160,  82,  79,   6,   6,   6, 161,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 161, 162,  29,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 162, 163,  29,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6, 152,   6,   6, 163,   0, 164, 165, 166,   6,   6,  26, 167,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6,  80,  24,   6, 168,   6, 169, 170,
-     90, 171, 172, 173,   6,   6,   6,  77,   1,   2,   3, 105,   6, 103, 174,   0,
-    175, 176, 177,   0,   6,   6,   6,  67,   0,   0,   6,  95,   0,   0,   0, 178,
-      0,   0,   0,   0,  77,   6, 179, 180,   6, 181,  30,  67,  80,   6, 182,   0,
-      6,   6,   6,   6,  80,  79, 183,  29,   6, 184,   6, 185, 186, 187,   0,   0,
-      6,   6,   6,   6,   6,   6,   6,   6,   6, 134, 102, 169, 188, 189,   0,   0,
-    190, 191, 102, 134, 103,   0,   0, 192, 102, 163,   0,   0,   6, 193,   0,   0,
-    194, 195,   0,  77,  77,   0,  74, 196,   6, 102, 102, 197,  26,   0,   0,   0,
-      6,   6, 131,   0,   6, 197,   6, 197,   6, 198,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   6, 199,   0, 200,  77, 201, 179,  24, 202,  24, 203, 134,
-      6,   6, 196, 204,   6,  67, 205, 206,   6, 207, 208, 209,   6,   6, 210,   0,
-    211, 193, 212,   0, 213, 117,   6, 214,  33, 215, 216, 217,   0,   0,   0,   0,
-      6,   6, 218, 212,   6,   6, 219,   0,   0,   0,   0,   0,   6, 220, 221,   0,
-      6,   6, 222,   0,   6, 101,  99,   0,  88, 223, 196,   0,   0,   0,   0,   0,
-      6,  67,   0,   0,   0,   6,   6, 224, 225, 226, 227,   0,   0, 228, 229, 230,
-      6, 103, 201,   6, 231,  24,   6, 101,   0,   0,   0,   0,   0,   0,   0,   0,
-    232,   5, 233, 148, 168, 234,   0,   0, 235, 236, 198, 237, 238,  99,   0,   0,
-      0,   0,   0,   0,   0,   0,   0, 134, 239, 240, 241,   0,   0, 242,   0,   0,
+      6,   6,   6, 153,   6,   6, 164,   0, 165, 166, 167,   6,   6,  26, 168,   6,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,  80,  24,   6, 169,   6, 170, 171,
+     90, 172, 173, 174,   6,   6,   6,  77,   1,   2,   3, 140,   6, 103, 175,   0,
+    176, 177, 178,   0,   6,   6,   6,  67,   0,   0,   6,  95,   0,   0,   0, 179,
+      0,   0,   0,   0,  77,   6, 180, 181,   6, 182,  30,  67,  80,   6, 183,   0,
+      6,   6,   6,   6,  80,  79, 184,  29,   6, 185,   6, 186, 187, 188,   0,   0,
+      6,   6,   6,   6,   6,   6,   6,   6,   6, 135, 102, 170, 189, 190,   0,   0,
+    191, 192, 102, 135, 103,   0,   0, 193, 102, 164,   0,   0,   6, 194,   0,   0,
+    195, 196,   0,  77,  77,   0,  74, 197,   6, 102, 102, 198,  26,   0,   0,   0,
+      6,   6, 132,   0,   6, 198,   6, 198,   6, 199,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   6, 200,   0, 201,  77, 202, 180,  24, 203,  24, 204, 135,
+      6,   6, 197, 205,   6,  67, 206, 207,   6, 208, 209, 210,   6,   6, 211,   0,
+    212, 194, 213,   0, 214, 117,   6, 215,  33, 216, 217, 218,   0,   0,   0,   0,
+      6,   6, 219, 213,   6,   6, 220,   0,   0,   0,   0,   0,   6, 221, 222,   0,
+      6,   6, 223,   0,   6, 101,  99,   0,  88, 224, 197,   0,   0,   0,   0,   0,
+      6,  67,   0,   0,   0,   6,   6, 225, 226, 227, 228,   0,   0, 229, 230, 231,
+      6, 103, 202,   6, 232,  24,   6, 101,   0,   0,   0,   0,   0,   0,   0,   0,
+    233,   5, 234, 149, 169, 235,   0,   0, 236, 237, 199, 238, 239,  99,   0,   0,
+      0,   0,   0,   0,   0,   0,   0, 135, 240, 241, 242,   0,   0, 243,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 163,   0,   0,   0,
-      6,   6,   6, 112,   6,   6,   6,   6,   6,   6, 243,   0,   0,   0,   0,   0,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 164,   0,   0,   0,
+      6,   6,   6, 112,   6,   6,   6,   6,   6,   6, 244,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  24,   6,   6, 179,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  24,   6,   6, 180,
       6,  90, 102,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6, 196,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      6,   6, 197,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6, 101, 103,  79,   6, 103,  79, 106,   6, 134, 227, 244,  90,   0,   0,   0,
+      6, 101, 103,  79,   6, 103,  79, 106,   6, 135, 228, 245,  90,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   6,   6,   0,   0,   0,   0,   6,   6, 245,   6, 246,   0,   0, 247,
+      0,   0,   6,   6,   0,   0,   0,   0,   6,   6, 246,   6, 247,   0,   0, 248,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 115,
-      6,   6,   6,   6,   6,   6, 102,   0, 131,   0,   0,   0,   0,   0,   0,   0,
+      6,   6,   6,   6,   6,   6, 102,   0, 132,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 248,
-      6,   6,   6,   6,   6,   6,   6,   6,   6, 249, 250, 208,   6,   6,   6,   6,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 249,
+      6,   6,   6,   6,   6,   6,   6,   6,   6, 250, 251, 209,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,  29,   0,   0,   0,   0,   0,   0,   0,   0,
-      6,   6,   6, 251, 252,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      6,   6,   6, 252, 253,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   6, 152, 196,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 253, 254, 255,   0,   0,
-      0,   0, 256,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      6,   6, 207,   6, 257, 258, 259,   6, 260, 261, 262,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6, 263, 264,  82, 207, 207, 265, 265, 232, 232, 266,   6,
+      0,   0,   0,   0,   0,   0,   0,   0,   6, 153, 197,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 254, 255, 256,   0,   0,
+      0,   0, 257,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      6,   6, 208,   6, 258, 259, 260,   6, 261, 262, 263,   6,   6,   6,   6,   6,
+      6,   6,   6,   6,   6, 264, 265,  82, 208, 208, 266, 266, 233, 233, 267,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      6, 267,   6, 268, 269, 270,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      6, 268,   6, 269, 270, 271,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0, 103, 271,   0,   0,   0,   0,   0,   0,
-    272, 273,   6,  28, 274,   0,   0,   0,   6, 275, 276,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,  24, 112,   6, 163,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,  24, 163,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 277,
-      6,   6,   6,   6,   6,   6, 278,   0,   6,   6, 223,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0, 103, 272,   0,   0,   0,   0,   0,   0,
+    273, 274,   6,  28, 275,   0,   0,   0,   6, 276, 277,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,  24, 112,   6, 164,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  24, 164,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 278,
+      6,   6,   6,   6,   6,   6, 279,   0,   6,   6, 224,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    259, 279, 280, 281, 282, 283,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    260, 280, 281, 282, 283, 284,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   0,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6, 163,   6,   6,   6,   6,   6,   6,
+      6,   6,   6,   6,   6,   6,   6,   6,   6, 164,   6,   6,   6,   6,   6,   6,
      80,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6, 284,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
+      6,   6,   6,   6,   6, 285,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 180,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 286,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
+      6,   6,  80,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
      80,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,  30,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,  90,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,  90,
@@ -14041,56 +14314,56 @@
     255, 159, 255, 255, 255, 199, 255,   1, 255, 255,  63, 128, 255, 255,  31,   0,
     255, 255,  15,   0, 255, 223,  13,   0, 255, 255, 143,  48, 255,   3,   0,   0,
       0, 184, 255,   3, 255, 255, 255,   1, 255, 255,  63,   0, 255, 255, 255, 127,
     255,  15, 255,  15, 192, 255, 255, 255, 255,  63,  31,   0, 255,  15, 255, 255,
     255,   3, 255,   7, 255, 255, 255, 159, 255,   3, 255,   3, 128,   0, 255, 191,
     255, 127,   0,   0, 255,  31, 255,   3,   0, 248,  15,   0, 255, 255, 255,   0,
     255, 227, 255, 255, 255,   1, 255, 255,   0,   0, 247, 255,  63,  63, 255, 170,
-    255, 255, 223,  95, 220,  31, 207,  15, 255,  31, 220,  31,   0,   0,   0, 128,
-      1,   0,  16,   0,   0,   0,   2, 128,   0,   0, 255,  31, 226, 255,   1,   0,
-    132, 252,  47,  63,  80, 253, 255, 243, 224,  67,   0,   0, 255,   1,   0,   0,
-     31, 248,  15,   0, 255, 128,   0, 128, 255, 255, 127,   0, 127, 127, 127, 127,
-    224,   0,   0,   0, 254, 255,  62,  31, 255, 255, 127, 254, 224, 255, 255, 255,
-    255,  31,   0,   0, 255,  31, 255, 255, 255,  15,   0,   0, 255, 255, 240, 191,
-      0,   0, 128, 255, 252, 255, 255, 255, 255, 249, 255, 255, 255,   7, 235,   3,
-      0,   0, 252, 255, 255,  16,   0,   0,  63,   0, 255,   3, 255, 255, 255, 232,
-    255,  63, 255, 255,   1, 128, 255,   3, 255,  63, 255,   3, 255, 255, 127, 252,
-      7,   0,   0,  56, 255, 255, 124,   0, 126, 126, 126,   0, 127, 127, 255, 255,
-    255,  55, 255,   3,  15,   0, 255, 255, 127, 248, 255, 255, 255, 255, 255,   3,
-    127,   0, 248, 224, 255, 253, 127,  95, 219, 255, 255, 255,   0,   0, 248, 255,
-    255, 255, 252, 255, 255,   0,   0,   0,   0,   0, 255,  15, 255, 255,  24,   0,
-      0, 224,   0,   0,   0,   0, 223, 255, 252, 252, 252,  28, 255, 239, 255, 255,
-    127, 255, 255, 183, 255,  63, 255,  63,   0,   0,   0,  32, 255, 255,   1,   0,
-      1,   0,   0,   0,   0, 224, 255, 255,  15, 255,  62,   0, 255, 255,  15, 255,
-    255,   0, 255, 255,  15,   0, 255, 247, 255, 247, 183, 255, 251, 255, 251,  27,
-    191, 255, 255, 255, 255, 255, 253,   7,  63, 253, 255, 255, 255, 255, 191, 145,
-    255, 255,  55,   0, 255, 255, 255, 192, 111, 240, 239, 254, 255, 255,  63, 135,
-    127,   0,   0,   0, 255, 255,   7,   0, 255,   0, 255,   3, 255,  27,   3,   0,
-      0,   0,   0, 224, 128,   0, 255, 255,  63,   0,   0,   0,  31,   0,   0,   0,
-    192, 255,  63, 128,   4,   0, 255, 255, 255,   1, 255,   3, 255, 255, 223, 255,
-    240,   0, 255, 255, 255, 255,  79,   0,  31, 222, 255,  23, 255, 255, 251, 255,
-      3,   0,   0,   0, 127, 189, 255, 191, 255,   7, 255,   3, 255, 253, 237, 251,
-    159,  57, 129, 224, 207,  31,  31,   0, 255,   7, 255, 195, 191,   0, 255,   3,
-    255, 255,  63, 255,   1,   0,   0,  63,  17,   0, 255,   3, 255,  15, 255,   3,
-    255,   3,   0, 128, 127, 242, 111, 255, 255, 255, 191, 249,  15,   0, 255,   3,
-    255, 252, 255, 255, 255, 255, 255, 252,  27,   0,   0,   0, 255, 255, 255,  35,
-    255, 253, 255, 255,   1,   0, 255,   3, 255, 254, 127,   0, 127, 251, 255, 255,
-    255, 255, 127, 180, 191, 253, 255, 255, 255, 127, 251,   1, 255, 255, 253, 255,
-    255, 255, 255, 199,   7,   0, 255,   3,   0,   0,   1,   0,  15,   0,   0,   0,
-    248, 255, 255, 224, 255, 135, 255, 255, 255, 128, 255, 255,  27,   0,   3,   0,
-      0,   0, 239, 111,   7,   0,   4,   0,   0,   0,  39,   0, 255,   7, 255,  31,
-    255,   1, 255,  99, 224, 227,   7, 248, 231,  15,   0,   0,   0,  60,   0,   0,
-     28,   0,   0,   0, 255, 255, 255, 223, 100, 222, 255, 235, 239, 255, 255, 255,
-    191, 231, 223, 223, 255, 255, 255, 123,  95, 252, 253, 255,  63, 255, 255, 255,
-    253, 255, 255, 247, 255, 127, 255, 255, 247, 207, 255, 255, 255, 255, 127, 248,
-    255,  31,  32,   0,  16,   0,   0, 248, 254, 255,   0,   0, 224,   7,   0,   0,
-    127, 255, 255, 249, 219,   7, 255, 255,   0, 128,   0,   0, 255,  31, 255,  63,
-    255,  67,   0,   0, 127, 111, 255, 127,  31,   0, 127,   0, 150, 254, 247,  10,
-    132, 234, 150, 170, 150, 247, 247,  94, 255, 251, 255,  15, 238, 251, 255,  15,
-      3,   0, 255, 255
+    255, 255, 223,  95, 220,  31, 207,  15, 255,  31, 220,  31,   0,  48,   0,   0,
+      0,   0,   0, 128,   1,   0,  16,   0,   0,   0,   2, 128,   0,   0, 255,  31,
+    226, 255,   1,   0, 132, 252,  47,  63,  80, 253, 255, 243, 224,  67,   0,   0,
+    255,   1,   0,   0,  31, 248,  15,   0, 255, 128,   0, 128, 255, 255, 127,   0,
+    127, 127, 127, 127, 224,   0,   0,   0, 254, 255,  62,  31, 255, 255, 127, 254,
+    224, 255, 255, 255, 255,  31,   0,   0, 255,  31, 255, 255, 255,  15,   0,   0,
+    255, 255, 240, 191,   0,   0, 128, 255, 252, 255, 255, 255, 255, 249, 255, 255,
+    255,   7, 235,   3,   0,   0, 252, 255, 255,  16,   0,   0,  63,   0, 255,   3,
+    255, 255, 255, 232, 255,  63, 255, 255,   1, 128, 255,   3, 255,  63, 255,   3,
+    255, 255, 127, 252,   7,   0,   0,  56, 255, 255, 124,   0, 126, 126, 126,   0,
+    127, 127, 255, 255, 255,  55, 255,   3,  15,   0, 255, 255, 127, 248, 255, 255,
+    255, 255, 255,   3, 127,   0, 248, 224, 255, 253, 127,  95, 219, 255, 255, 255,
+      0,   0, 248, 255, 255, 255, 252, 255, 255,   0,   0,   0,   0,   0, 255,  15,
+    255, 255,  24,   0,   0, 224,   0,   0,   0,   0, 223, 255, 252, 252, 252,  28,
+    255, 239, 255, 255, 127, 255, 255, 183, 255,  63, 255,  63,   0,   0,   0,  32,
+    255, 255,   1,   0,   1,   0,   0,   0,   0, 224, 255, 255,  15, 255,  62,   0,
+    255, 255,  15, 255, 255,   0, 255, 255,  15,   0, 255, 247, 255, 247, 183, 255,
+    251, 255, 251,  27, 191, 255, 255, 255, 255, 255, 253,   7,  63, 253, 255, 255,
+    255, 255, 191, 145, 255, 255,  55,   0, 255, 255, 255, 192, 111, 240, 239, 254,
+    255, 255,  63, 135, 127,   0,   0,   0, 255, 255,   7,   0, 255,   0, 255,   3,
+    255,  27,   3,   0,   0,   0,   0, 224, 128,   0, 255, 255,  63,   0,   0,   0,
+     31,   0,   0,   0, 192, 255,  63, 128,   4,   0, 255, 255, 255,   1, 255,   3,
+    255, 255, 223, 255, 240,   0, 255, 255, 255, 255,  79,   0,  31, 222, 255,  23,
+    255, 255, 251, 255,   3,   0,   0,   0, 127, 189, 255, 191, 255,   7, 255,   3,
+    255, 253, 237, 251, 159,  57, 129, 224, 207,  31,  31,   0, 255,   7, 255, 195,
+    191,   0, 255,   3, 255, 255,  63, 255,   1,   0,   0,  63,  17,   0, 255,   3,
+    255,  15, 255,   3, 255,   3,   0, 128, 127, 242, 111, 255, 255, 255, 191, 249,
+     15,   0, 255,   3, 255, 252, 255, 255, 255, 255, 255, 252,  27,   0,   0,   0,
+    255, 255, 255,  35, 255, 253, 255, 255,   1,   0, 255,   3, 255, 254, 127,   0,
+    127, 251, 255, 255, 255, 255, 127, 180, 191, 253, 255, 255, 255, 127, 251,   1,
+    255, 255, 253, 255, 255, 255, 255, 199,   7,   0, 255,   3,   0,   0,   1,   0,
+     15,   0,   0,   0, 248, 255, 255, 224, 255, 135, 255, 255, 255, 128, 255, 255,
+     27,   0,   3,   0,   0,   0, 239, 111,   7,   0,   4,   0,   0,   0,  39,   0,
+    255,   7, 255,  31, 255,   1, 255,  99, 224, 227,   7, 248, 231,  15,   0,   0,
+      0,  60,   0,   0,  28,   0,   0,   0, 255, 255, 255, 223, 100, 222, 255, 235,
+    239, 255, 255, 255, 191, 231, 223, 223, 255, 255, 255, 123,  95, 252, 253, 255,
+     63, 255, 255, 255, 253, 255, 255, 247, 255, 127, 255, 255, 247, 207, 255, 255,
+    255, 255, 127, 248, 255,  31,  32,   0,  16,   0,   0, 248, 254, 255,   0,   0,
+    224,   7,   0,   0, 127, 255, 255, 249, 219,   7, 255, 255,   0, 128,   0,   0,
+    255,  31, 255,  63, 255,  67,   0,   0, 127, 111, 255, 127,  31,   0, 127,   0,
+    150, 254, 247,  10, 132, 234, 150, 170, 150, 247, 247,  94, 255, 251, 255,  15,
+    238, 251, 255,  15,   3,   0, 255, 255,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_id_continue(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -14117,16 +14390,16 @@
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  5,  2,  2,  2,  2,
      2,  6,  2,  7,  0,  0,  0,  0,  0,  0,  0,  0,  8,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  9,  2,  2,  2, 10, 11,  2,
-     2,  2,  2, 12,  2,  2,  2,  2,  2,  2, 13,  0,  0,  0, 14,  0,
-     2,  2,  2,  2, 15,  2,  2,  2, 16,  0,  0,  0,  0,  0,  0,  0,
+     2,  2,  2, 12,  2,  2,  2,  2,  2,  2, 13, 14,  0,  0, 15,  0,
+     2,  2,  2,  2, 16,  2,  2,  2, 17,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
@@ -14206,26 +14479,28 @@
     12,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
      3,  3,  3,  3,  3, 13,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3, 14,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
+     3,  3, 12,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
     12,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3, 15,  3,  3,  3,  3,  3,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,
      3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3,  3, 16,  0,  0
 };
 
 static RE_UINT8 re_ideographic_table_3[] = {
       0,   0,   0,   0, 192,   0,   0,   0, 254,   3,   0,   7, 255, 255, 255, 255,
     255,  63, 255, 255, 255, 255, 255,   3,  16,   0,   0,   0, 255, 255, 255,   0,
     255, 255,  63,   0, 255,   1,   0,   0,   0,   0, 255, 255, 255, 255, 255,  15,
-    255, 255, 255,  63,   3,   0, 255, 255,   1,   0,   0,   0, 255,   7, 255, 255,
+    255, 255, 255,  63,   3,   0, 255, 255,   1,   0, 255, 255, 255,   7, 255, 255,
     255, 255,   0,   0
 };
 
 RE_UINT32 re_get_ideographic(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
@@ -14244,15 +14519,17 @@
     return (v >> offset) & 0x1;
 }
 
 /* IDS_Binary_Operator. */
 RE_UINT32 re_get_ids_binary_operator(RE_UINT32 codepoint) {
     if (0x2FF0 <= codepoint && codepoint <= 0x2FF1)
         return 1;
-    if (0x2FF4 <= codepoint && codepoint <= 0x2FFB)
+    if (0x2FF4 <= codepoint && codepoint <= 0x2FFD)
+        return 1;
+    if (codepoint == 0x31EF)
         return 1;
 
     return 0;
 }
 
 /* ID_Start. */
 static RE_UINT8 re_id_start_table_1[] = {
@@ -14263,16 +14540,16 @@
     19, 20, 21, 22, 23, 24, 25, 26, 27, 28,  9, 29, 12, 30,  9,  9,
      9, 31,  9,  9,  9,  9,  9,  9,  9,  9, 32, 33, 12, 12, 12, 12,
     12, 34, 12, 35,  9,  9,  9,  9,  9,  9,  9, 36, 37,  9,  9, 38,
      9,  9,  9,  9,  9, 39,  9, 40, 41, 42, 43, 44,  9,  9,  9,  9,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 45, 12, 12, 12, 46, 47, 12,
-    12, 12, 12, 48, 12, 12, 12, 12, 12, 12, 49,  9,  9,  9, 50,  9,
-    12, 12, 12, 12, 51, 12, 12, 12, 52,  9,  9,  9,  9,  9,  9,  9,
+    12, 12, 12, 48, 12, 12, 12, 12, 12, 12, 49, 50,  9,  9, 51,  9,
+    12, 12, 12, 12, 52, 12, 12, 12, 53,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -14422,15 +14699,17 @@
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4, 161,   4,   4,   4,   4,   4,   4,
     113,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4, 254,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
-      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  74,
+      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4, 255,
+      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
+      4,   4, 113,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
     113,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  30,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  22,   0,   0
 };
@@ -14495,15 +14774,15 @@
     255,  63,   0,   0, 248, 255, 255, 224, 255,   7,   1,   0,  11,   0,   0,   0,
       0,   0, 239, 111,   7,   0,   4,   0,   0,   0,  39,   0, 240,   0, 255, 255,
     255,   7, 255,  31, 255,   1, 255,   3, 255, 255, 223, 255, 255, 255, 255, 223,
     100, 222, 255, 235, 239, 255, 255, 255, 191, 231, 223, 223, 255, 255, 255, 123,
      95, 252, 253, 255,  63, 255, 255, 255, 253, 255, 255, 247, 255, 127, 255, 255,
     224,   7,   0,   0, 255,  31, 128,  63,   0,  64,   0,   0, 127, 111, 255, 127,
      15,   8,   0,   0, 150, 254, 247,  10, 132, 234, 150, 170, 150, 247, 247,  94,
-    255, 251, 255,  15, 238, 251, 255,  15,   3,   0, 255, 255
+    255, 251, 255,  15, 238, 251, 255,  15,   3,   0, 255, 255,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_id_start(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -14525,14 +14804,401 @@
 RE_UINT32 re_get_ids_trinary_operator(RE_UINT32 codepoint) {
     if (0x2FF2 <= codepoint && codepoint <= 0x2FF3)
         return 1;
 
     return 0;
 }
 
+/* IDS_Unary_Operator. */
+RE_UINT32 re_get_ids_unary_operator(RE_UINT32 codepoint) {
+    if (0x2FFE <= codepoint && codepoint <= 0x2FFF)
+        return 1;
+
+    return 0;
+}
+
+/* Indic_Conjunct_Break. */
+static RE_UINT8 re_indic_conjunct_break_table_1[] = {
+     0,  1,  2,  3,  4,  5,  6,  7,  8,  9,  9, 10, 11,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9, 12, 13,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 14, 15,
+    16,  9, 17, 18, 19, 20, 21, 22,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 23,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 24,
+     9,  9,  9,  9, 25,  9,  9,  9, 26, 27, 28,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9
+};
+
+static RE_UINT8 re_indic_conjunct_break_table_2[] = {
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   1,   1,   2,   3,   0,   0,   0,   0,
+      0,   0,   0,   0,   4,   0,   0,   0,   0,   0,   0,   0,   5,   6,   7,   0,
+      8,   0,   9,  10,   0,   0,  11,  12,  13,  14,  15,   0,   0,   0,   0,  16,
+     17,  18,  19,   0,  20,   0,  21,  22,  23,  24,  25,  26,  23,  27,  28,  29,
+      0,  30,   0,   0,  23,  31,  32,  33,  23,  31,  28,  34,   0,   0,   0,   0,
+     23,  35,  36,   0,   0,  30,   0,   0,  23,  37,  32,   0,   0,   0,   0,   0,
+      0,  38,  39,   0,   0,  38,  39,   0,  40,  41,   0,  42,  43,   0,  44,   0,
+      0,  45,   0,   0,  46,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  47,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  48,   0,   0,   0,   0,   0,  49,   0,
+      0,   0,   0,   0,   0,  50,   0,   0,   0,  19,   0,   0,   0,   0,   0,   0,
+     51,   0,   0,  52,   0,  53,  54,   0,   0,  48,   0,  55,   0,  56,   0,  44,
+      0,  57,   0,   0,   0,   0,  58,  59,   0,   0,   0,   0,   0,   0,   1,   1,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+     46,   0,   0,   0,   0,   0,  60,  61,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,  62,   0,   0,   0,  63,   0,   0,   0,   1,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,  64,   0,   0,  65,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,  66,  67,   0,   0,  68,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,  69,   0,   0,   0,   0,   0,  70,   0,  71,   0,   0,   0,  72,   0,   0,
+      0,   0,   0,   0,   0,  73,  74,  75,   0,   0,   0,   0,   0,   0,   0,  46,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  76,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  77,
+      0,   0,   0,   0,   0,   0,   0,  78,   0,   0,   0,  79,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+     80,  81,   0,   0,   0,   0,   0,  82,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,  83,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,  84,   0,  47,   0,   0,  85,   0,  86,   0,   0,   0,
+      0,   0,   0,  87,   0,  88,   0,   0,  89,  90,   0,  72,   0,   0,  91,   0,
+      0,  75,   0,   0,   0,   0,   0,  92,   0,  93,   0,  94,   0,   0,   0,   0,
+      0,   0,  95,   0,   0,   0,  96,   0,   0,   0,   0,   0,   0,   0,  78,   0,
+      0,   0,   0,   0,   0,  57,   0,   0,   0,  56,   0,   0,   0,   0,   0,   0,
+      0,  88,   0,   0,   0,   0,   0,   0,   0,  76,  96,   0,   0,   0,   0,   0,
+      0,  48,  97,   0,  98,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  99,   0,  57,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 100,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0, 101,   0, 102,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,  76,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 103, 104, 105,   0,   0,
+      0,   0, 106,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    107, 108,   0,   0, 109,   0,   0,   0,   0, 102,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0, 110,   0, 111,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0, 111,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 102,   0,   0,   0, 112,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0
+};
+
+static RE_UINT8 re_indic_conjunct_break_table_3[] = {
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1,
+    0, 1, 1, 0, 1, 1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1,
+    1, 1, 1, 1, 1, 0, 0, 1, 1, 0, 1, 1, 1, 1, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 0, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 0, 1, 1, 1, 0, 1, 1, 1, 1, 1, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+    2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+    2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 0, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0,
+    0, 1, 1, 1, 1, 0, 0, 0, 2, 2, 2, 2, 2, 2, 2, 2,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 2, 2, 2, 2, 2, 2, 2, 2,
+    2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 2, 2, 2, 2, 2, 2,
+    2, 0, 2, 0, 0, 0, 2, 2, 2, 2, 0, 0, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 2, 0, 2,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    2, 2, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0,
+    2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 2, 2, 2, 2, 2, 2,
+    2, 0, 2, 2, 0, 2, 2, 2, 2, 2, 0, 0, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 2, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 2, 2, 2, 2, 2, 2,
+    2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 0, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0,
+    0, 0, 0, 0, 0, 1, 1, 0, 2, 2, 2, 0, 0, 0, 0, 0,
+    2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+    2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 1, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 1, 1, 0, 1, 0, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0,
+    1, 0, 1, 1, 1, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 1, 0, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0,
+    1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 1, 0, 0,
+    0, 0, 0, 0, 1, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0,
+    0, 1, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 0, 1, 1, 1, 0, 0, 1, 1, 0, 0, 0, 0, 0, 1, 1,
+    0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0,
+    1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0,
+    1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0,
+    1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0,
+    0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0,
+    0, 0, 1, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 1, 0, 1, 1, 1, 0, 0, 0, 0, 1, 1,
+    1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1,
+    1, 1, 1, 0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 1,
+    1, 1, 0, 1, 1, 0, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+};
+
+RE_UINT32 re_get_indic_conjunct_break(RE_UINT32 codepoint) {
+    RE_UINT32 field_2;
+    RE_UINT32 field_1;
+    RE_UINT32 field_0;
+    RE_UINT32 v;
+
+    field_2 = codepoint >> 10;
+    field_1 = (codepoint >> 5) & 0x1F;
+    field_0 = codepoint & 0x1F;
+
+    v = re_indic_conjunct_break_table_1[field_2];
+    v = re_indic_conjunct_break_table_2[(v << 5) | field_1];
+    v = re_indic_conjunct_break_table_3[(v << 5) | field_0];
+
+    return v;
+}
+
 /* Indic_Positional_Category. */
 static RE_UINT8 re_indic_positional_category_table_1[] = {
      0,  0,  1,  2,  3,  4,  5,  6,  7,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  8,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  9,  0, 10, 11, 12, 13,  0,  0,  0,  0,  0,  0,  0,  0,
@@ -16203,132 +16869,132 @@
      62,  63,  64,  65,  66,  67,  68,  69,  70,  71,  72,  73,  74,  75,  76,  77,
      78,  79,  80,  81,  82,  83,  84,  81,  85,  86,  87,  88,  89,  90,  91,  81,
      92,  92,  93,  92,  94,   7,  95,   7,  96,  96,  96,  97,  97,  98,  99,  99,
       7,   7, 100,   7, 101, 102, 103,   7, 104,   7, 105, 106, 107,   7,   7, 108,
     109,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7, 110,   7,   7, 111, 112, 113, 114, 115,  92,  92, 116, 117,
     118,   7,   7, 119, 120, 121,   7, 122, 123, 124, 125, 126,  92, 127, 128,   7,
-    129,  92, 130, 131, 132, 133, 134,  81, 135, 136, 137, 138, 139, 140,   7, 141,
-      7, 142, 143, 144, 145, 146, 147, 148,   7,   7,   7,   7,   7,   7, 149, 150,
-      7,   7,   7,   7,   7,   7,   7,   7, 108,   7, 151, 152,   7, 153, 154, 155,
-    156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168,   7, 169,   7,
-    170, 171, 172, 173, 174, 175,   7, 176, 177, 178,   7,   7,   7,   7,   7, 179,
-      7, 180, 181, 182, 182, 182, 182, 183, 182, 182, 184, 185, 186, 187, 188, 189,
-    190, 191, 192, 193, 194, 195, 196, 197, 198,   7, 199, 200, 201,   7, 202, 203,
-      7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 204,   7, 205, 206,
-      7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 207, 208, 209,   7,   7,   7,
-      7,   7,   7,   7,   7,   7,   7, 210,   7,  95,   7, 211, 212, 213, 213,   9,
-    214, 215, 216,  81, 217, 218, 218, 219, 218, 218, 218, 218, 218, 218, 220, 221,
-    222, 223, 224, 225, 226, 227, 225, 228, 229, 230, 218, 218, 231, 218, 218, 232,
-    233, 218, 234, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,   7,   7,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    235, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 236, 218, 237, 144,   7,   7,   7,   7,   7,   7,   7,   7,
-    238, 239,   7, 240, 241,   7,   7, 242,   7,   7,   7,   7,   7,   7, 243, 244,
-    245, 246,   7, 247, 248, 136, 249, 250,  30, 251, 252, 253,  39, 254, 255, 256,
-      7, 257, 258,  92,  92,  92, 259, 260, 261, 262,   7, 263,   7,   7,   7, 264,
-    265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266,
-    267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268,
-    269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270,
-    271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265,
-    266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267,
-    268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269,
-    270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271,
-    265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266,
-    267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268,
-    269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270,
-    271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265,
-    266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267,
-    268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269,
-    270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271,
-    270, 271, 265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 271,
-    265, 266, 267, 268, 269, 270, 271, 265, 266, 267, 268, 269, 270, 272, 273, 274,
-    275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275,
-    275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275, 275,
+    129,  92, 130, 131, 132, 133, 134,  81, 135, 136, 137, 138, 139, 140, 141, 142,
+      7, 143, 144, 145, 146, 147, 148, 149,   7,   7,   7,   7,   7,   7, 150, 151,
+      7,   7,   7,   7,   7,   7,   7,   7, 108,   7, 152, 153,   7, 154, 155, 156,
+    157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169,   7, 170,   7,
+    171, 172, 173, 174, 175, 176,   7, 177, 178, 179,   7,   7,   7,   7,   7, 180,
+      7, 181, 182, 183, 183, 183, 183, 184, 183, 183, 185, 186, 187, 188, 189, 190,
+    191, 192, 193, 194, 195, 196, 197, 198, 199,   7, 200, 201, 202,   7, 203, 204,
+      7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 205,   7, 206, 207,
+      7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 208, 209, 210,   7,   7,   7,
+      7,   7,   7,   7,   7,   7,   7, 211,   7,  95,   7, 212, 213, 214, 214,   9,
+    215, 216, 217,  81, 218, 219, 219, 220, 219, 219, 219, 219, 219, 219, 221, 222,
+    223, 224, 225, 226, 227, 228, 226, 229, 230, 231, 219, 219, 232, 219, 219, 233,
+    234, 219, 235, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,   7,   7,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    236, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 237, 219, 238, 145,   7,   7,   7,   7,   7,   7,   7,   7,
+    239, 240,   7, 241, 242,   7,   7, 243,   7,   7,   7,   7,   7,   7, 244, 245,
+    246, 247,   7, 248, 249, 250, 251, 252,  30, 253, 254, 255, 256, 257, 258, 259,
+    141, 260, 261,  92,  92,  92, 262, 263, 264, 265,   7, 266,   7,   7,   7, 267,
+    268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269,
+    270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271,
+    272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273,
+    274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268,
+    269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270,
+    271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272,
+    273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274,
+    268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269,
+    270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271,
+    272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273,
+    274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268,
+    269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270,
+    271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272,
+    273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274,
+    273, 274, 268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 274,
+    268, 269, 270, 271, 272, 273, 274, 268, 269, 270, 271, 272, 273, 275, 276, 277,
+    278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278,
+    278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278, 278,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,  81,  81,  81,  81,  81,  81, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 218, 276, 277, 278,   7,   7,   7, 279,   7,
-      7,   7,   7,   7,   7,   7,   7,   7,   7, 280,   7,   7, 281,   7, 282, 283,
-    284, 285, 286, 287,   7,   7,   7, 288, 289, 290, 291, 292, 293, 233, 294, 295,
-    296, 297, 298,  81,   7,   7,   7, 299, 300, 301,   7,   7, 302, 303, 304, 305,
-     81,  81,  81,  81, 306,   7, 307, 308,   7, 309,  35, 310, 311,   7, 312,  81,
-      7,   7,   7,   7, 152, 313, 314, 315,   7, 316,   7, 317, 318, 319,  81,  81,
-      7,   7,   7,   7,   7,   7,   7,   7,   7, 212, 122, 320, 321, 322,  81,  81,
-    323, 324, 325,   7, 123, 326,  81, 327, 328, 329,  81,  81,   7, 330, 281,   7,
-    331, 332, 333,   7,   7,  81,   7, 334,   7, 335, 336, 337, 338, 339,  81,  81,
-      7,   7, 340,  81,   7, 341,   7, 342,   7, 343,  81,  81,  81,  81,  81,  81,
-     81,  81,  81, 123,   7, 344,  81, 345,   7, 316, 346, 304, 347, 304, 348, 212,
-    139, 349, 350, 351, 139, 352, 353, 354, 139, 355, 356, 357, 139, 254, 358, 359,
-    360, 361, 362,  81, 363, 364, 365, 366, 367, 368, 369, 370,  81,  81,  81,  81,
-      7, 371, 372, 373,   7,  27, 374,  81,  81,  81,  81,  81,   7, 375, 376,  81,
-      7,  27, 377, 378,   7, 379, 380,  81, 381, 382, 383,  81,  81,  81,  81,  81,
-      7, 384,  81,  81,  81,   7,   7, 385, 386, 387, 388,  81,  81, 389, 390, 391,
-    392, 393, 394,   7, 395, 396,   7, 119, 397,  81,  81,  81,  81,  81,  81,  81,
-    398, 399, 400, 401, 402, 403,  81,  81, 404, 405, 406, 407, 408, 380,  81,  81,
-     81,  81,  81,  81,  81,  81,  81, 409, 410, 411, 412,  81,  81, 413, 414, 415,
+     81,  81,  81,  81,  81,  81,  81,  81, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 219, 279, 280, 281,   7,   7,   7, 282,   7,
+      7,   7,   7,   7,   7,   7,   7,   7,   7, 283,   7,   7, 284,   7, 285, 286,
+    287, 288, 289, 290,   7,   7,   7, 291, 292, 293, 294, 295, 296, 234, 297, 298,
+    299, 300, 301,  81,   7,   7,   7, 302, 303, 304,   7,   7, 305, 306, 307, 308,
+     81,  81,  81,  81, 309,   7, 310, 311,   7, 312,  35, 313, 314,   7, 315,  81,
+      7,   7,   7,   7, 153, 316, 317, 318,   7, 319,   7, 320, 321, 322,  81,  81,
+      7,   7,   7,   7,   7,   7,   7,   7,   7, 213, 122, 323, 324, 325,  81,  81,
+    326, 327, 328,   7, 123, 329,  81, 330, 331, 332,  81,  81,   7, 333, 284,   7,
+    334, 335, 336,   7,   7,  81,   7, 337,   7, 338, 339, 340, 341, 342,  81,  81,
+      7,   7, 343,  81,   7, 344,   7, 345,   7, 346,  81,  81,  81,  81,  81,  81,
+     81,  81,  81, 123,   7, 347,  81, 348,   7, 319, 349, 307, 350, 307, 351, 213,
+    352, 353, 354, 355, 139, 356, 357, 358, 139, 359, 360, 361, 139, 362, 363, 364,
+    365, 366, 367,  81, 368, 369, 370, 371, 372, 373, 374, 375,  81,  81,  81,  81,
+      7, 376, 377, 378,   7,  27, 379,  81,  81,  81,  81,  81,   7, 380, 381,  81,
+      7,  27, 382, 383,   7, 384, 385,  81, 386, 387, 388,  81,  81,  81,  81,  81,
+      7, 389,  81,  81,  81,   7,   7, 390, 391, 392, 393,  81,  81, 394, 395, 396,
+    397, 398, 399,   7, 400, 401,   7, 119, 402,  81,  81,  81,  81,  81,  81,  81,
+    403, 404, 405, 406, 407, 408,  81,  81, 409, 410, 411, 412, 413, 385,  81,  81,
+     81,  81,  81,  81,  81,  81,  81, 414, 415, 416, 417,  81,  81, 418, 419, 420,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 107,  81,  81,  81,
-      7,   7,   7, 416,   7,   7,   7,   7,   7,   7, 417,  81,  81,  81,  81,  81,
+      7,   7,   7, 421,   7,   7,   7,   7,   7,   7, 422,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81, 304,   7,   7, 341,
+     81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81, 307,   7,   7, 344,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
-      7,   7, 418,   7, 419,   7,   7,   7,   7,   7,   7, 420,   7,   7,   7,   7,
-      7, 421, 422,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
+      7,   7, 423,   7, 424,   7,   7,   7,   7,   7,   7, 425,   7,   7,   7,   7,
+      7, 426, 427,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-      7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 423,   7,
-      7,   7, 180,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
+      7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7, 428,   7,
+      7,   7, 181,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
-      7, 119, 123, 424,   7, 123, 313, 425,   7, 426, 427, 428, 429,  81,  81,  81,
+      7, 119, 123, 429,   7, 123, 316, 430,   7, 431, 432, 433, 434,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,   7,   7, 430,  81,  81,  81,   7,   7, 431,   9, 432,  81,  81, 433,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 434,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 218,   7,   7,   7,   7,   7,   7,   7,   7,
-      7,   7,   7,   7,   7,   7, 122,  81, 435,  81,  81,  81,  81,  81,  81,  81,
+     81,  81,   7,   7, 435,  81,  81,  81,   7,   7, 436,   9, 437,  81,  81, 438,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 439,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 219,   7,   7,   7,   7,   7,   7,   7,   7,
+      7,   7,   7,   7,   7,   7, 122,  81, 440,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81, 436,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 437, 438, 439, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 440,  81,  81,  81,  81,  81,  81,  81,  81,
-      7,   7,   7, 441, 442, 443,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
+     81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81, 441,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 442, 443, 444, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 445,  81,  81,  81,  81,  81,  81,  81,  81,
+      7,   7,   7, 446, 447, 448,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,  81,  81,  81,  81,  81,  81,   9, 444, 445,   7,   7,   7, 417,  81,
-      7,   7,   7,   7,   7,   7,   7, 122,   7, 446,   7, 447, 448, 449,   7, 181,
-      7,   7, 450,  81,  81,  81, 451, 451,   7,   7, 212, 119,  81,  81,  81,  81,
-      7,   7, 153,   7, 452, 453, 454,   7, 455, 456, 457,   7,   7,   7,   7,   7,
-      7,   7,   7,   7,   7, 458,   7,   7,   7,   7,   7,   7,   7,   7, 459, 460,
+     81,  81,  81,  81,  81,  81,  81,  81,   9, 449, 450,   7,   7,   7, 422,  81,
+      7,   7,   7,   7,   7,   7,   7, 122,   7, 451,   7, 452, 453, 454,   7, 182,
+      7,   7, 455,  81,  81,  81, 456, 456,   7,   7, 213, 119,  81,  81,  81,  81,
+      7,   7, 154,   7, 457, 458, 459,   7, 460, 461, 462,   7,   7,   7,   7,   7,
+      7,   7,   7,   7,   7, 463,   7,   7,   7,   7,   7,   7,   7,   7, 464, 465,
       7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,   7,
-      9, 461,   9, 462, 463, 464,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
+      9, 466,   9, 467, 468, 469,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,  81,  81,  81,  81,  81,  81, 123, 465,  81,  81,  81,  81,  81,  81,
-    466, 467,   7, 468, 469,  81,  81,  81,   7, 470, 471,  81,  81,  81,  81,  81,
-     81,  81,  81,  81, 304, 472,   7, 473,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,  81,  81,  81,  81, 304, 474,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81, 475,
-      7,   7,   7,   7,   7,   7, 476,  81,   7,   7, 477,  81,  81,  81,  81,  81,
+     81,  81,  81,  81,  81,  81,  81,  81, 123, 470,  81,  81,  81,  81,  81,  81,
+    471, 472,   7, 473, 474,  81,  81,  81,   7, 475, 476,  81,  81,  81,  81,  81,
+     81,  81,  81,  81, 307, 477,   7, 478,  81,  81,  81,  81,  81,  81,  81,  81,
+     81,  81,  81,  81,  81,  81, 307, 479,  81,  81,  81,  81,  81,  81,  81,  81,
+     81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81, 480,
+      7,   7,   7,   7,   7,   7, 481,  81,   7,   7, 482,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,  81, 478,   7, 479,  81,  81, 480, 152,  81,  81,  81,  81,  81,  81,
-    454, 481, 482, 483, 484, 485,  81, 486,  81,  81,  81,  81,  81,  81,  81,  81,
-    218, 218, 218, 218, 218, 218, 218, 218, 487, 488, 182, 489, 182, 490, 218, 491,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 492, 493, 494, 495,
-    218, 218, 496, 497, 498, 499, 218, 218, 500, 501, 502, 503, 504, 218, 505, 506,
-    218, 218, 507, 508, 218, 509, 510, 218,   7,   7,   7, 511,   7,   7, 512, 218,
-    513,   7, 514,   7, 515, 516, 218, 218, 517, 518, 218, 519, 218, 520, 521, 218,
-      7,   7, 511, 218, 218, 218, 522, 523,   7,   7,   7,   7, 524,   7, 181, 525,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218,
-    218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 218, 526,
-    527,   9,   9,   9,  81,  81,  81,  81,   9,   9,   9,   9,   9,   9,   9, 528,
+     81,  81,  81, 483,   7, 484,  81,  81, 485, 153,  81,  81,  81,  81,  81,  81,
+    459, 486, 487, 488, 489, 490,  81, 491,  81,  81,  81,  81,  81,  81,  81,  81,
+    219, 219, 219, 219, 219, 219, 219, 219, 492, 493, 183, 494, 183, 495, 219, 496,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 497, 498, 499, 500,
+    219, 219, 501, 502, 503, 504, 219, 219, 505, 506, 507, 508, 509, 219, 510, 511,
+    219, 219, 512, 513, 219, 514, 515, 219,   7,   7,   7, 516,   7,   7, 517, 219,
+    518,   7, 519,   7, 520, 521, 219, 219, 522, 523, 219, 524, 219, 525, 526, 219,
+      7,   7, 516, 219, 219, 219, 527, 528,   7,   7,   7,   7, 529,   7, 182, 530,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219,
+    219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 219, 531,
+    532,   9,   9,   9,  81,  81,  81,  81,   9,   9,   9,   9,   9,   9,   9, 533,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81
 };
 
 static RE_UINT8 re_line_break_table_3[] = {
      1,  1,  1,  1,  1,  1,  1,  1,  1,  2,  3,  4,  4,  5,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      6,  7,  8,  9, 10, 11,  9,  8, 12, 13,  9, 10, 14, 15, 14, 16,
@@ -16367,22 +17033,22 @@
      0,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  2,  1,
      9,  1,  1,  9,  1,  1,  7,  1,  0,  0,  0,  0,  0,  0,  0,  0,
     23, 23, 23, 23, 23, 23, 23, 23, 23, 23, 23, 23, 23, 23, 23, 23,
     23, 23, 23, 23, 23, 23, 23, 23, 23, 23, 23,  0,  0,  0,  0, 23,
     23, 23, 23,  9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     9,  9,  9,  9,  9,  9,  9,  9,  9, 11, 11, 11, 14, 14,  9,  9,
+    17, 17, 17, 17, 17, 17,  9,  9,  9, 11, 11, 11, 14, 14,  9,  9,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  7,  1,  7,  7,  7,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 11, 17, 17,  9,  9,  9,
      1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  7,  9,  1,  1,  1,  1,  1,  1,  1,  9,  9,  1,
+     9,  9,  9,  9,  7,  9,  1,  1,  1,  1,  1,  1,  1, 17,  9,  1,
      1,  1,  1,  1,  1,  9,  9,  1,  1,  9,  1,  1,  1,  1,  9,  9,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  9,
      9,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  0,  0,  9,  9,  9,
@@ -16398,18 +17064,18 @@
      1,  1,  1,  1,  9,  1,  1,  1,  9,  1,  1,  1,  1,  1,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  0,  0,  9,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,
-     9,  9,  0,  0,  0,  0,  0,  0,  1,  1,  1,  1,  1,  1,  1,  1,
+    17, 17,  0,  0,  0,  0,  0,  0,  1,  1,  1,  1,  1,  1,  1,  1,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
-     1,  1,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
+     1,  1, 17,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  9,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      9,  1,  1,  1,  1,  1,  1,  1,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -16595,28 +17261,30 @@
     24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24,  0,  0,  1,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
     24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24,  0,  0,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     1,  1,  1,  1,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
-     1,  1,  1,  1,  1,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,
-    17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  2,  2,  9,  2,  2,  2,
-     2,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,
-     1,  1,  1,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  2,  2,  0,
+     1,  1,  1,  1,  1, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
+     1,  1,  1,  1, 30, 29, 29, 29, 29, 29, 29, 29, 29,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  2,  2, 31,  2,  2,  2,
+     2, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  1,  1,  1,  1,  1,
+     1,  1,  1,  1, 31, 31, 31, 31, 31, 31, 31, 31, 31,  2,  2,  0,
      1,  1,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  9,  9,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
-     1,  1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  9,  9,  9,  9,
+    32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32,
+    32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32,
+    32, 32, 32, 32, 32, 32,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
+     1,  1, 33, 33,  0,  0,  0,  0,  0,  0,  0,  0,  9,  9,  9,  9,
      9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  0,  0,  0,  2,  2,  2,  2,  2,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  9,  9,  9,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  2,  2,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,
@@ -16637,21 +17305,21 @@
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  0,  0,  9,  9,  9,  9,  9,  9,  0,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      0,  0,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9, 22,  9,  0,
-     2,  2,  2,  2,  2,  2,  2, 20,  2,  2,  2, 29,  1, 30,  1,  1,
-     2, 20,  2,  2, 31, 21, 21,  9,  8,  8, 12,  8,  8,  8, 12,  8,
-    21, 21,  9,  9, 32, 32, 32,  2,  4,  4,  1,  1,  1,  1,  1, 20,
+     2,  2,  2,  2,  2,  2,  2, 20,  2,  2,  2, 34,  1, 35,  1,  1,
+     2, 20,  2,  2, 36, 21, 21,  9,  8,  8, 12,  8,  8,  8, 12,  8,
+    21, 21,  9,  9, 37, 37, 37,  2,  4,  4,  1,  1,  1,  1,  1, 20,
     11, 11, 11, 11, 11, 11, 11, 11,  9,  8,  8, 21, 28, 28,  9,  9,
      9,  9,  9,  9, 14, 12, 18, 28, 28, 28,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  2, 11,  2,  2,  2,  2,  9,  2,  2,  2,
-    33,  9,  9,  9,  9,  0,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
+    38,  9,  9,  9,  9,  0,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      9,  9,  0,  0, 21,  9,  9,  9,  9,  9,  9,  9,  9, 12, 18, 21,
      9, 21, 21, 21, 21,  9,  9,  9,  9,  9,  9,  9,  9, 12, 18,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,
     10, 10, 10, 10, 10, 10, 10, 11, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 11, 10, 10, 10, 10, 11, 10, 10, 11, 10,
     11, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
@@ -16677,22 +17345,22 @@
      9,  9, 21,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
     21, 21,  9,  9, 21, 21, 21, 21,  9,  9, 21, 21,  9,  9, 21, 21,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9, 21, 21,  9,  9, 21, 21,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9, 21,  9,  9,  9, 21,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9, 21,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 21,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 32,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 37,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9, 12, 18, 12, 18,  9,  9,  9,  9,
-     9,  9, 21,  9,  9,  9,  9,  9,  9,  9, 34, 34,  9,  9,  9,  9,
+     9,  9, 21,  9,  9,  9,  9,  9,  9,  9, 31, 31,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9, 12, 18,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-    34, 34, 34, 34,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+    31, 31, 31, 31,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
     21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
     21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
@@ -16705,35 +17373,35 @@
      9,  9, 21, 21, 21, 21,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
     21, 21,  9, 21, 21, 21, 21, 21, 21, 21,  9,  9,  9,  9,  9,  9,
      9,  9, 21, 21,  9,  9, 21, 21,  9,  9,  9,  9, 21, 21,  9,  9,
     21, 21,  9,  9,  9,  9, 21, 21, 21,  9,  9, 21,  9,  9, 21, 21,
     21, 21,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9, 21, 21, 21, 21,  9,  9,  9,  9,  9,  9,  9,  9,  9, 21,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-    34, 34, 34, 34,  9, 21, 21,  9,  9, 21,  9,  9,  9,  9, 21, 21,
-     9,  9,  9,  9, 34, 34, 21, 21, 34,  9, 34, 34, 34, 35, 34, 34,
+    31, 31, 31, 31,  9, 21, 21,  9,  9, 21,  9,  9,  9,  9, 21, 21,
+     9,  9,  9,  9, 31, 31, 21, 21, 31,  9, 31, 31, 31, 39, 31, 31,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9, 34, 34, 34,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9, 31, 31, 31,  9,  9,  9,  9,
     21,  9, 21,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-    21, 21,  9, 21, 21, 21,  9, 21, 34, 21, 21,  9, 21, 21,  9, 21,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 34,
+    21, 21,  9, 21, 21, 21,  9, 21, 31, 21, 21,  9, 21, 21,  9, 21,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 31,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 21, 21,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 21, 21, 21, 21, 34,  9, 34,
-    34, 34, 21, 34, 34, 21, 21, 21, 34, 34, 21, 21, 34, 21, 21, 34,
-    34, 34,  9, 21,  9,  9,  9,  9, 21, 21, 34, 21, 21, 21, 21, 21,
-    21, 34, 34, 34, 34, 34, 21, 34, 34, 35, 34, 21, 21, 34, 34, 34,
-    34, 34, 34, 34, 34,  9,  9,  9, 34, 34, 35, 35, 35, 35,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 21, 21, 21, 21, 31,  9, 31,
+    31, 31, 21, 31, 31, 21, 21, 21, 31, 31, 21, 21, 31, 21, 21, 31,
+    31, 31,  9, 21,  9,  9,  9,  9, 21, 21, 31, 21, 21, 21, 21, 21,
+    21, 31, 31, 31, 31, 31, 21, 31, 31, 39, 31, 21, 21, 31, 31, 31,
+    31, 31, 31, 31, 31,  9,  9,  9, 31, 31, 39, 39, 39, 39,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9, 21,  9,  9,  9,  8,  8,  8,  8,  8,
-     8,  9,  7,  7, 34,  9,  9,  9, 12, 18, 12, 18, 12, 18, 12, 18,
+     8,  9,  7,  7, 31,  9,  9,  9, 12, 18, 12, 18, 12, 18, 12, 18,
     12, 18, 12, 18, 12, 18, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
     21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
     21, 21, 21, 21,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9, 12, 18,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9, 12, 18, 12, 18, 12, 18, 12, 18, 12, 18,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -16756,58 +17424,58 @@
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  0,
      9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  0,
      8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  2,  2,
      2,  2,  2,  2,  2,  2,  9,  2, 12,  2,  9,  9,  8,  8,  9,  9,
      8,  8, 12, 18, 12, 18, 12, 18, 12, 18,  2,  2,  2,  2,  7,  9,
-     2,  2,  9,  2,  2,  9,  9,  9,  9,  9, 31, 31,  2,  2,  2,  9,
+     2,  2,  9,  2,  2,  9,  9,  9,  9,  9, 36, 36,  2,  2,  2,  9,
      2,  2, 12,  2,  2,  2,  2,  2,  2,  2,  2,  9,  2,  9,  2,  2,
      9,  9,  9,  7,  7, 12, 18, 12, 18, 12, 18, 12, 18,  2,  0,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  0, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  0,  0,  0,  0,
-     2, 18, 18, 34, 34, 28, 34, 34, 12, 18, 12, 18, 12, 18, 12, 18,
-    12, 18, 34, 34, 12, 18, 12, 18, 12, 18, 12, 18, 28, 12, 18, 18,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  1,  1,  1,  1,  1,  1,
-    34, 34, 34, 34, 34,  1, 34, 34, 34, 34, 34, 28, 28, 34, 34, 34,
-     0, 36, 34, 36, 34, 36, 34, 36, 34, 36, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 36, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 36, 34, 36, 34, 36, 34, 34, 34, 34, 34, 34, 36, 34,
-    34, 34, 34, 34, 34, 36, 36,  0,  0,  1,  1, 28, 28, 28, 28, 34,
-    28, 36, 34, 36, 34, 36, 34, 36, 34, 36, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 36, 34, 36, 34, 36, 34, 34, 34, 34, 34, 34, 36, 34,
-    34, 34, 34, 34, 34, 36, 36, 34, 34, 34, 34, 28, 36, 28, 28, 34,
-     0,  0,  0,  0,  0, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-     0, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36, 36,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 21, 21, 21, 21, 21, 21, 21, 21,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 28, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  0,  0,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+     2, 18, 18, 31, 31, 28, 31, 31, 12, 18, 12, 18, 12, 18, 12, 18,
+    12, 18, 31, 31, 12, 18, 12, 18, 12, 18, 12, 18, 28, 12, 18, 18,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  1,  1,  1,  1,  1,  1,
+    31, 31, 31, 31, 31,  1, 31, 31, 31, 31, 31, 28, 28, 31, 31, 31,
+     0, 40, 31, 40, 31, 40, 31, 40, 31, 40, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 40, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 40, 31, 40, 31, 40, 31, 31, 31, 31, 31, 31, 40, 31,
+    31, 31, 31, 31, 31, 40, 40,  0,  0,  1,  1, 28, 28, 28, 28, 31,
+    28, 40, 31, 40, 31, 40, 31, 40, 31, 40, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 40, 31, 40, 31, 40, 31, 31, 31, 31, 31, 31, 40, 31,
+    31, 31, 31, 31, 31, 40, 40, 31, 31, 31, 31, 28, 40, 28, 28, 31,
+     0,  0,  0,  0,  0, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+     0, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 31,
+    40, 40, 40, 40, 40, 40, 40, 40, 40, 40, 40, 40, 40, 40, 40, 40,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 21, 21, 21, 21, 21, 21, 21, 21,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 28, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  2,  7,  2,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  9,  9,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,
      1,  1,  1,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  9,  9,
@@ -16823,68 +17491,72 @@
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  1,  1,  1,  1,  1,  9,  9,  9,  9,  1,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9, 11,  9,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9, 22, 22,  7,  7,  0,  0,  0,  0,  0,  0,  0,  0,
      1,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  2,  2,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 22,  9,  9,  1,
      9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  2,  2,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  9,
     25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25,
     25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25,  0,  0,  0,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
-     1,  9,  9,  9,  9,  9,  9,  2,  2,  2,  9,  9,  9,  9,  0,  9,
-    17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  9,  9,
+     1,  1,  1,  1, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
+    30, 31, 31, 31, 31, 31, 31,  2,  2,  2, 31, 31, 31, 31,  0,  2,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0,  0,  0,  0, 31, 31,
     24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 24, 24, 24, 24, 24,  0,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,
+    32, 32, 32, 32, 32, 32, 32, 32, 32,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     9,  9,  9,  1,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  0,  0,
-    17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  9,  2,  2,  2,
+     2,  2,  2,  1,  2,  2,  2,  2,  2,  2,  2,  2,  1,  1,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0,  0, 31,  2,  2,  2,
     24, 24, 24,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 24, 24, 24, 24, 24,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,
      2,  2,  9,  9,  9,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  9,  9,  9,  9,  9,  9,  0,  0,  9,  9,  9,  9,  9,  9,  0,
      0,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  2,  1,  1,  0,  0,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
-    37, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 37, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 37, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 37, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    37, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 37, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 37, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 37, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38, 38,
-    38, 38, 38, 38,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    41, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 41, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 41, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 41, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    41, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 41, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 41, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 41, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42, 42,
+    42, 42, 42, 42,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26,
     26, 26, 26, 26, 26, 26, 26,  0,  0,  0,  0, 27, 27, 27, 27, 27,
     27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27,
     27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27,
     27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27,  0,  0,  0,  0,
-    39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39,
-    39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39,
+    43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43,
+    43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43, 43,
      9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0, 23,  1, 23,
     23, 23, 23, 23, 23, 23, 23, 23, 23,  9, 23, 23, 23, 23, 23, 23,
     23, 23, 23, 23, 23, 23, 23,  0, 23, 23, 23, 23, 23,  0, 23,  0,
     23, 23,  0, 23, 23,  0, 23, 23, 23, 23, 23, 23, 23, 23, 23, 23,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
@@ -16894,37 +17566,37 @@
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      0,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,  9,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 11,  9,  9,  9,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
-    14, 18, 18, 14, 14,  7,  7, 12, 18, 32,  0,  0,  0,  0,  0,  0,
+    14, 18, 18, 14, 14,  7,  7, 12, 18, 37,  0,  0,  0,  0,  0,  0,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
-    34, 34, 34, 34, 34, 12, 18, 12, 18, 12, 18, 12, 18, 12, 18, 12,
-    18, 12, 18, 12, 18, 34, 34, 12, 18, 34, 34, 34, 34, 34, 34, 34,
-    18, 34, 18,  0, 28, 28,  7,  7, 34, 12, 18, 12, 18, 12, 18, 34,
-    34, 34, 34, 34, 34, 34, 34,  0, 34, 10, 11, 34,  0,  0,  0,  0,
+    31, 31, 31, 31, 31, 12, 18, 12, 18, 12, 18, 12, 18, 12, 18, 12,
+    18, 12, 18, 12, 18, 31, 31, 12, 18, 31, 31, 31, 31, 31, 31, 31,
+    18, 31, 18,  0, 28, 28,  7,  7, 31, 12, 18, 12, 18, 12, 18, 31,
+    31, 31, 31, 31, 31, 31, 31,  0, 31, 10, 11, 31,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0, 33,
-     0,  7, 34, 34, 10, 11, 34, 34, 12, 18, 34, 34, 18, 34, 18, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 28, 28, 34, 34, 34,  7,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 12, 34, 18, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 12, 34, 18, 34, 12,
-    18, 18, 12, 18, 18, 28, 34, 36, 36, 36, 36, 36, 36, 36, 36, 36,
-    36, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 28, 28,
-     0,  0, 34, 34, 34, 34, 34, 34,  0,  0, 34, 34, 34, 34, 34, 34,
-     0,  0, 34, 34, 34, 34, 34, 34,  0,  0, 34, 34, 34,  0,  0,  0,
-    11, 10, 34, 34, 34, 10, 10,  0,  9,  9,  9,  9,  9,  9,  9,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  1,  1, 40, 21,  0,  0,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0, 38,
+     0,  7, 31, 31, 10, 11, 31, 31, 12, 18, 31, 31, 18, 31, 18, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 28, 28, 31, 31, 31,  7,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 12, 31, 18, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 12, 31, 18, 31, 12,
+    18, 18, 12, 18, 18, 28, 31, 40, 40, 40, 40, 40, 40, 40, 40, 40,
+    40, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 28, 28,
+     0,  0, 31, 31, 31, 31, 31, 31,  0,  0, 31, 31, 31, 31, 31, 31,
+     0,  0, 31, 31, 31, 31, 31, 31,  0,  0, 31, 31, 31,  0,  0,  0,
+    11, 10, 31, 31, 31, 10, 10,  0,  9,  9,  9,  9,  9,  9,  9,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  1,  1, 44, 21,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  0,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -16994,15 +17666,15 @@
      9,  1,  1,  1,  0,  1,  1,  0,  0,  0,  0,  0,  1,  1,  1,  1,
      9,  9,  9,  9,  0,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  0,  0,  1,  1,  1,  0,  0,  0,  0,  1,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,
      2,  2,  2,  2,  2,  2,  2,  2,  9,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  1,  1,  0,  0,  0,  0,  9,  9,  9,  9,  9,
-     2,  2,  2,  2,  2,  2, 32,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     2,  2,  2,  2,  2,  2, 37,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  0,  0,  0,  2,  2,  2,  2,  2,  2,  2,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  0,  0,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  0,  0,  0,  0,  0,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -17023,32 +17695,36 @@
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  1,  1,
      9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,
      9,  9,  1,  1,  1,  1,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     1,  1,  1, 45, 45, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29,  1,  1,  1,  1,  1,  1,  1,  1,
+     1,  1,  1,  1,  1,  1, 30,  2,  2, 31, 31, 31, 31, 31,  0,  0,
+     0,  0, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32,
+     1, 29, 29,  1,  1, 29,  0,  0,  0,  0,  0,  0,  0,  0,  0, 20,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,
-     1,  1,  1,  1,  1,  1,  1,  2,  2,  9,  9,  9,  9,  9,  0,  0,
-     0,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
-     1,  9,  9,  1,  1,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  9,  9,  9,  2,  2,
-     2,  2,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  9,  0,  0,
+     1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  9,  9, 17,  2,  2,
+     2,  2,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 17,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  0, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
      2,  2,  2,  2,  9,  1,  1,  9,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  1,  9, 22,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  9,  9,  9,  9,  2,  2,  9,  2,  1,  1,  1,  1,  9,  1,  1,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  9, 22,  9,  2,  2,  2,
      0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,
@@ -17059,21 +17735,21 @@
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  2,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  0,  0,  0,  0,  0,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
-     1,  1,  1,  1,  0,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  9,
-     9,  0,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,
-     9,  0,  9,  9,  0,  9,  9,  9,  9,  9,  0,  1,  1,  9,  1,  1,
-     1,  1,  1,  1,  1,  0,  0,  1,  1,  0,  0,  1,  1,  1,  0,  0,
-     9,  0,  0,  0,  0,  0,  0,  1,  0,  0,  0,  0,  0,  9,  9,  9,
-     9,  9,  1,  1,  0,  0,  1,  1,  1,  1,  1,  1,  1,  0,  0,  0,
+     1,  1,  1,  1,  0, 29, 29, 29, 29, 29, 29, 29, 29,  0,  0, 29,
+    29,  0,  0, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29,  0, 29, 29, 29, 29, 29, 29,
+    29,  0, 29, 29,  0, 29, 29, 29, 29, 29,  0,  1,  1,  2,  1,  1,
+     1,  1,  1,  1,  1,  0,  0,  1,  1,  0,  0,  1,  1, 30,  0,  0,
+    32,  0,  0,  0,  0,  0,  0,  1,  0,  0,  0,  0,  0,  2, 32, 32,
+    29, 29,  1,  1,  0,  0,  1,  1,  1,  1,  1,  1,  1,  0,  0,  0,
      1,  1,  1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  9,  9,  9,  9,  2,  2,  2,  2,  9,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  2,  2,  0,  9,  1,  9,
      9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
@@ -17097,20 +17773,20 @@
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 24, 24,  2,  2,  2, 24,
     24, 24, 24, 24, 24, 24, 24,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  9,  0,  0,  0,  0,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  9,
-     9,  9,  9,  9,  9,  9,  9,  0,  0,  9,  0,  0,  9,  9,  9,  9,
-     9,  9,  9,  9,  0,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     1,  1,  1,  1,  1,  1,  0,  1,  1,  0,  0,  1,  1,  1,  1,  9,
-     1,  9,  1,  1,  2,  2,  2,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
+    29, 29, 29, 29, 29, 29, 29,  0,  0, 29,  0,  0, 29, 29, 29, 29,
+    29, 29, 29, 29,  0, 29, 29,  0, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+     1,  1,  1,  1,  1,  1,  0,  1,  1,  0,  0,  1,  1,  1, 30, 45,
+     1, 45,  1,  1,  2,  2,  2,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  1,  1,  1,  1,  1,  1,  1,  0,  0,  1,  1,  1,  1,  1,  1,
      1,  9, 22,  9,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  9,  9,  9,  9,  9,
@@ -17143,22 +17819,22 @@
      9,  1,  1,  1,  1,  1,  1,  0,  0,  0,  1,  0,  1,  1,  0,  1,
      1,  1,  1,  1,  1,  1,  9,  1,  0,  0,  0,  0,  0,  0,  0,  0,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  0,  9,  9,  0,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  0,
      1,  1,  0,  1,  1,  1,  1,  1,  9,  0,  0,  0,  0,  0,  0,  0,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  1,  1,  1,  1,  9,  9,  0,  0,  0,  0,  0,  0,  0,
-     1,  1,  9,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  0,  0,  0,  1,  1,
-     1,  1,  1,  2,  2, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
+    32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32, 32,
+    32, 32,  2,  1,  1,  1,  1,  2,  2,  0,  0,  0,  0,  0,  0,  0,
+     1,  1, 45,  1, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29,  0, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+    29, 29, 29, 29,  1,  1,  1,  1,  1,  1,  1,  0,  0,  0,  1,  1,
+     1,  1, 30,  2,  2, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    32, 32, 32, 32, 32, 32, 32, 32, 32, 32,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 11, 11, 11,
     11,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  2,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,
@@ -17167,15 +17843,15 @@
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9, 12, 12, 12, 18, 18, 18,  9,  9,
      9,  9, 18,  9,  9,  9, 12, 18, 12, 18,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9, 12, 18, 18,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 12,
     20, 20, 20, 20, 20, 20, 20, 12, 18, 20, 20, 20, 12, 18, 12, 18,
      1,  9,  9,  9,  9,  9,  9,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 12, 18,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  2,  2,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -17193,28 +17869,28 @@
      9,  9,  9,  9,  9,  9,  9,  2,  2,  9,  9,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  1,
      9,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  1,
      1,  1,  1,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
     28, 28, 28, 28, 20,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34,  0,  0,  0,  0,  0,  0,  0,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34,  0,  0,  0,  0,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31,  0,  0,  0,  0,  0,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  0,
-    34, 34, 34,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0, 36,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    31, 31, 31,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0, 40,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    36, 36, 36,  0,  0, 36,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0, 36, 36, 36, 36,  0,  0,  0,  0,  0,  0,  0,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  0,  0,  0,  0,
+    40, 40, 40,  0,  0, 40,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0, 40, 40, 40, 40,  0,  0,  0,  0,  0,  0,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  9,  1,  1,  2,
      1,  1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  0,  0,
@@ -17299,94 +17975,94 @@
      9,  9,  9,  0,  9,  9,  9,  9,  0,  9,  9,  9,  9,  0,  9,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,
      0,  9,  9,  9,  0,  9,  9,  9,  9,  9,  0,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 34, 34, 34,
+    21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 31, 31, 31,
     21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
     21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,  9,  9,
     21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
-    21, 21, 21, 21, 21, 21, 21, 21, 21, 21,  9,  9,  9, 34, 34, 34,
+    21, 21, 21, 21, 21, 21, 21, 21, 21, 21,  9,  9,  9, 31, 31, 31,
     21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
-    21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 41, 41, 41, 41, 41, 41, 41, 41, 41, 41,
-    41, 41, 41, 41, 41, 41, 41, 41, 41, 41, 41, 41, 41, 41, 41, 41,
-    34, 34, 34, 34, 34, 35, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  9,  9, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34,  9,  9, 34, 34, 34, 34, 34,  9, 34, 34, 34,
-    34, 34, 35, 35, 35, 34, 34, 35, 34, 34, 35, 35, 35, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 42, 42, 42, 42, 42,
-    34, 34, 35, 35, 34, 34, 35, 35, 35, 35, 35, 35, 35, 35, 35, 35,
-    35, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 35, 35, 35, 35, 35, 35, 35, 35, 35, 35,
-    35, 35, 35, 35, 35, 35, 35, 35, 35, 34, 34, 34, 35, 34, 34, 34,
-    34, 35, 35, 35, 34, 35, 35, 35, 34, 34, 34, 34, 34, 34, 34, 35,
-    34, 35, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-     9, 34,  9, 34,  9, 34, 34, 34, 34, 34, 35, 34, 34, 34, 34,  9,
-    34,  9,  9, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 35, 35, 34, 34, 34, 34, 35, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    35, 34, 34, 34, 34, 35, 35, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34,  9,  9,  9,  9,  9,  9,  9,  9, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34,  9,  9,  9,  9,  9,  9, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 35, 35, 35, 34, 34, 34, 35, 35, 35, 35, 35,
+    21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 46, 46, 46, 46, 46, 46, 46, 46, 46, 46,
+    46, 46, 46, 46, 46, 46, 46, 46, 46, 46, 46, 46, 46, 46, 46, 46,
+    31, 31, 31, 31, 31, 39, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  9,  9, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31,  9,  9, 31, 31, 31, 31, 31,  9, 31, 31, 31,
+    31, 31, 39, 39, 39, 31, 31, 39, 31, 31, 39, 39, 39, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 47, 47, 47, 47, 47,
+    31, 31, 39, 39, 31, 31, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39,
+    39, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39,
+    39, 39, 39, 39, 39, 39, 39, 39, 39, 31, 31, 31, 39, 31, 31, 31,
+    31, 39, 39, 39, 31, 39, 39, 39, 31, 31, 31, 31, 31, 31, 31, 39,
+    31, 39, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+     9, 31,  9, 31,  9, 31, 31, 31, 31, 31, 39, 31, 31, 31, 31,  9,
+    31,  9,  9, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 39, 39, 31, 31, 31, 31, 39, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    39, 31, 31, 31, 31, 39, 39, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31,  9,  9,  9,  9,  9,  9,  9,  9, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31,  9,  9,  9,  9,  9,  9, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 39, 39, 39, 31, 31, 31, 39, 39, 39, 39, 39,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  8,  8,  8, 28, 28, 28,  9,  9,  9,  9,
-    34, 34, 34, 35, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 35, 35, 35, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    35, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 35, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9, 34, 34, 34, 34, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 34, 34, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9,  9, 34, 34, 34, 34, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 35, 34, 34, 35,
-    34, 34, 34, 34, 34, 34, 34, 34, 35, 35, 35, 35, 35, 35, 35, 35,
-    34, 34, 34, 34, 34, 34, 35, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    35, 35, 35, 35, 35, 35, 35, 35, 35, 35, 34, 34, 35, 35, 35, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 35, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 35, 35, 34, 35, 35, 34, 35, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 35, 35, 35,
-    34, 35, 35, 35, 35, 35, 35, 35, 35, 35, 35, 35, 35, 35, 34, 34,
-    34, 34, 34, 35, 35, 35, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    35, 35, 35, 35, 35, 35, 35, 35, 35, 34, 34, 34, 34, 34, 34, 34,
+    31, 31, 31, 39, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 39, 39, 39, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    39, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 39, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9, 31, 31, 31, 31, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 31, 31, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9,  9, 31, 31, 31, 31, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+     9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 39, 31, 31, 39,
+    31, 31, 31, 31, 31, 31, 31, 31, 39, 39, 39, 39, 39, 39, 39, 39,
+    31, 31, 31, 31, 31, 31, 39, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 31, 31, 39, 39, 39, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 39, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 39, 39, 31, 39, 39, 31, 39, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 39, 39, 39,
+    31, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 39, 31, 31,
+    31, 31, 31, 39, 39, 39, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    39, 39, 39, 39, 39, 39, 39, 39, 39, 31, 31, 31, 31, 31, 31, 31,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17,  0,  0,  0,  0,  0,  0,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,
-    34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34, 34,  0,  0,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,
+    31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31, 31,  0,  0,
      0,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0
 };
 
 RE_UINT32 re_get_line_break(RE_UINT32 codepoint) {
@@ -18825,25 +19501,25 @@
 
     return (v >> offset) & 0x1;
 }
 
 /* Numeric_Type. */
 static RE_UINT8 re_numeric_type_table_1[] = {
      0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12, 13, 14, 10,
-    10, 10, 10, 15, 16, 17, 18, 19, 20, 21, 10, 22, 23, 24, 10, 10,
-    25, 26, 10, 27, 10, 28, 10, 10, 10, 29, 30, 10, 10, 10, 10, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 31, 32,
-    33, 34, 35, 36, 37, 38, 39, 40, 10, 41, 10, 10, 10, 10, 10, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 42, 43, 10, 10, 10, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
-    10, 10, 10, 10, 44, 45, 10, 10, 46, 47, 48, 49, 50, 10, 51, 10,
-    52, 10, 53, 10, 10, 10, 10, 10, 54, 10, 55, 10, 10, 10, 56, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 57, 10, 10, 10, 10, 10, 10, 10,
+    10, 10, 10, 15, 16, 17, 18, 19, 20, 21, 10, 22, 23, 24, 25, 10,
+    26, 27, 10, 28, 29, 30, 10, 10, 10, 31, 32, 10, 10, 10, 10, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 33, 34,
+    35, 36, 37, 38, 39, 40, 41, 42, 10, 43, 10, 10, 10, 10, 10, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 44, 45, 10, 10, 10, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
+    10, 10, 10, 10, 46, 47, 10, 10, 48, 49, 50, 51, 52, 10, 53, 10,
+    54, 10, 55, 10, 10, 10, 10, 10, 56, 10, 57, 10, 10, 10, 58, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 59, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 58, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 60, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
@@ -18926,100 +19602,104 @@
      28,  29,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  30,   0,   0,   0,
       0,  31,  32,   0,  31,  33,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      34,   0,   0,   0,  35,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,  36,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  37,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-     38,   0,  27,   0,  39,  40,  41,  42,  37,   0,   0,  43,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,  44,   0,  45,  46,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  47,   0,   0,   0,  48,   0,
+     38,  39,  27,   0,  40,  41,  42,  43,  37,   0,   0,  44,   0,   0,   0,  45,
+     46,   0,   0,   0,   0,   0,   0,   0,  39,   0,  46,  47,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  48,   0,   0,   0,  49,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,  49,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  50,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  50,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,  51,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,  51,   0,   0,   0,  52,  53,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,  52,   0,   0,   0,  53,  54,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  54,   0,   0,  55,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  44,  55,   0,   0,  56,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  56,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  57,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  55,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  46,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,  45,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  58,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  57,   0,   0,   0,
+      0,   0,   0,  55,  59,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  37,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,  54,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,  45,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,  46,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,  55,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,  56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,  58,   0,   0,   0,  43,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,  60,   0,   0,   0,  44,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,  59,  60,  61,   0,   0,   0,  57,   0,   0,   0,   0,   0,   0,   0,   0,
+     61,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,  45,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,  62,  63,  64,   0,   0,   0,  58,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   3,   0,   0,   0,   0,   0,  62,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,  63,   0,   0,   0,   0,   1,   0,   3,   0,   0,   0,   0,   0,   1,   1,
+      0,   3,   0,   0,   0,   0,   0,  65,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,  66,   0,   0,   0,   0,   1,   0,   3,   0,   0,   0,   0,   0,   1,   1,
       0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  64,   0,  56,  65,  27,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  67,   0,  57,  68,  27,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,  66,  67,  20,  68,  69,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  70,   0,  71,  72,   0,   0,   0,  73,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  69,  70,  20,  71,  72,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,  73,   0,  74,  75,   0,   0,   0,  76,   0,
       0,   0,   0,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,  74,  75,   0,  76,   0,  77,  78,   0,   0,   0,   0,  79,  80,  20,
-      0,   0,  81,  82,  83,   0,   0,  84,   0,   0,  74,  74,   0,  85,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  86,   0,   1,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,  87,   0,   0,   0,   0,  83,  88,  89,   0,   0,   0,  90,   0,
-      0,   0,  91,  92,   0,   0,   0,   1,   0,  93,   0,   0,   0,   0,   1,  94,
+      0,   0,  77,  78,   0,  79,   0,  80,  81,   0,   0,   0,   0,  82,  83,  20,
+      0,   0,  84,  85,  86,   0,   0,  87,   0,   0,  77,  77,   0,  88,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,  89,   0,   1,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,  90,   0,   0,   0,   0,  86,  91,  92,   0,   0,   0,  93,   0,
+      0,   0,  94,  95,   0,   0,   0,   1,   0,  96,   0,   0,   0,   0,   1,  97,
       0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   1,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   1,   0,   0,   0,   3,   0,   0,  95,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  96,   0,   0,   1,   0,   0,   0,   0,   0,
+      0,   0,   1,   0,   0,   0,   3,   0,   0,  98,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,  99,   0,   0,   1,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,  97,  98,   0,   0,   0,   0,   0,   0,   1,   0,   0,   3,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,  99,   0,
-     20,  20,  20, 100,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0, 100, 101,   0,   0,   0,   0,   0,   0,   1,   0,   0,   3,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0, 102,   0,
+     20,  20,  20, 103,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   3,   0,   0,   3,   0,   0,   0, 101, 102,   0,   0,   0,   0,
+      0,   0,   0,   3,   0,   0,   3,   0,   0,   0, 104, 105,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0, 103,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0, 106,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,  67,  67,   0,   0,   0,  68,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  70,  70,   0,   0,   0,  71,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 104, 105,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 107, 108,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   3,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,  76,   0,   0,   0,   1,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  79,   0,   0,   0,   1,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,  33,  20, 106,   0,   0, 107, 108,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,  33,  20, 109,   0,   0, 110, 111,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0, 109,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0, 112,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,
-     59,   0,   0,  44,   0,   0,   0, 110,   0,  59,   0,   0,   0,   0,   0,   0,
+     62,   0,   0,  39,   0,   0,   0, 113,   0,  62,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,  36,   0,   0, 111,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0, 112, 113,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,  36,   0,   0, 114,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0, 115, 116,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  43,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  61,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  44,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  64,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,  49,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  50,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,  37,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,  43,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,  44,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0
 };
 
 static RE_UINT8 re_numeric_type_table_3[] = {
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
@@ -19094,25 +19774,27 @@
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     3, 0, 0, 3, 0, 0, 0, 3, 0, 3, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0, 0,
     0, 0, 0, 0, 3, 0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0,
-    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3,
     3, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3,
     0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     3, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
-    0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 3, 0, 3, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 3, 0, 3, 3, 3, 0, 0, 0, 0, 0, 0, 3, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
@@ -19132,16 +19814,20 @@
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0,
     0, 0, 0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 3, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 3, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 0, 0, 3, 0, 0, 0, 0, 0, 0, 0,
     0, 0, 0, 0, 0, 0, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
@@ -19266,25 +19952,25 @@
 
     return v;
 }
 
 /* Numeric_Value. */
 static RE_UINT8 re_numeric_value_table_1[] = {
      0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12, 13, 14, 10,
-    10, 10, 10, 15, 16, 17, 18, 19, 20, 21, 10, 22, 23, 24, 10, 10,
-    25, 26, 10, 27, 10, 28, 10, 10, 10, 29, 30, 10, 10, 10, 10, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 31, 32,
-    33, 34, 35, 36, 37, 38, 39, 40, 10, 41, 10, 10, 10, 10, 10, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 42, 43, 10, 10, 10, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
-    10, 10, 10, 10, 44, 45, 10, 10, 46, 47, 48, 49, 50, 10, 51, 10,
-    52, 10, 53, 10, 10, 10, 10, 10, 54, 10, 55, 10, 10, 10, 56, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 57, 10, 10, 10, 10, 10, 10, 10,
+    10, 10, 10, 15, 16, 17, 18, 19, 20, 21, 10, 22, 23, 24, 25, 10,
+    26, 27, 10, 28, 29, 30, 10, 10, 10, 31, 32, 10, 10, 10, 10, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 33, 34,
+    35, 36, 37, 38, 39, 40, 41, 42, 10, 43, 10, 10, 10, 10, 10, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 44, 45, 10, 10, 10, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
+    10, 10, 10, 10, 46, 47, 10, 10, 48, 49, 50, 51, 52, 10, 53, 10,
+    54, 10, 55, 10, 10, 10, 10, 10, 56, 10, 57, 10, 10, 10, 58, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 59, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
-    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 58, 10,
+    10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 60, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
@@ -19367,100 +20053,104 @@
      26,  27,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  28,   0,   0,   0,
       0,  29,  30,   0,  29,  31,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      32,   0,   0,   0,  33,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,  34,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  35,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-     36,   0,  37,   0,  38,  39,  40,  41,  42,   0,   0,  43,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,  44,   0,  45,  46,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  47,   0,   0,   0,  48,   0,
+     36,  37,  38,   0,  39,  40,  41,  42,  43,   0,   0,  44,   0,   0,   0,  45,
+     46,   0,   0,   0,   0,   0,   0,   0,  47,   0,  48,  49,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  50,   0,   0,   0,  51,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,  49,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  50,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  52,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,  53,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,  51,   0,   0,   0,  52,  53,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,  54,   0,   0,   0,  55,  56,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  54,   0,   0,  55,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  57,  58,   0,   0,  59,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  56,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  60,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  61,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  62,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,  57,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  63,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  58,   0,   0,   0,
+      0,   0,   0,  64,  65,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  66,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,  59,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,  60,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,  67,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,  61,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,  68,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,  62,   0,   0,   0,  63,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,  69,   0,   0,   0,  70,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,  64,  65,  66,   0,   0,   0,  67,   0,   0,   0,   0,   0,   0,   0,   0,
+     71,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,  72,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,  73,  74,  75,   0,   0,   0,  76,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   3,   0,   0,   0,   0,   0,  68,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,  69,   0,   0,   0,   0,   1,   0,   3,   0,   0,   0,   0,   0,   1,   1,
+      0,   3,   0,   0,   0,   0,   0,  77,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,  78,   0,   0,   0,   0,   1,   0,   3,   0,   0,   0,   0,   0,   1,   1,
       0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  70,   0,  71,  72,  73,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  79,   0,  80,  81,  82,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,  74,  75,  76,  77,  78,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  79,   0,  80,  81,   0,   0,   0,  82,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,  83,  84,  85,  86,  87,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,  88,   0,  89,  90,   0,   0,   0,  91,   0,
       0,   0,   0,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,  83,  84,   0,  85,   0,  86,  87,   0,   0,   0,   0,  88,  89,  90,
-      0,   0,  91,  92,  93,   0,   0,  94,   0,   0,  95,  95,   0,  96,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,  97,   0,   1,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,  98,   0,   0,   0,   0,  99, 100, 101,   0,   0,   0, 102,   0,
-      0,   0, 103, 104,   0,   0,   0,   1,   0, 105,   0,   0,   0,   0,   1, 106,
+      0,   0,  92,  93,   0,  94,   0,  95,  96,   0,   0,   0,   0,  97,  98,  99,
+      0,   0, 100, 101, 102,   0,   0, 103,   0,   0, 104, 104,   0, 105,   0,   0,
+      0,   0,   0,   0,   0,   0,   0, 106,   0,   1,   0,   0,   0,   0,   0,   0,
+      0,   0,   0, 107,   0,   0,   0,   0, 108, 109, 110,   0,   0,   0, 111,   0,
+      0,   0, 112, 113,   0,   0,   0,   1,   0, 114,   0,   0,   0,   0,   1, 115,
       0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   1,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   1,   0,   0,   0,   3,   0,   0, 107,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0, 108,   0,   0,   1,   0,   0,   0,   0,   0,
+      0,   0,   1,   0,   0,   0,   3,   0,   0, 116,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0, 117,   0,   0,   1,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0, 109, 110,   0,   0,   0,   0,   0,   0,   1,   0,   0,   3,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0, 111,   0,
-    112, 113, 114, 115,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0, 118, 119,   0,   0,   0,   0,   0,   0,   1,   0,   0,   3,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0, 120,   0,
+    121, 122, 123, 124,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   3,   0,   0,   3,   0,   0,   0, 116, 117,   0,   0,   0,   0,
+      0,   0,   0,   3,   0,   0,   3,   0,   0,   0, 125, 126,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0, 118,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0, 127,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 119, 119,   0,   0,   0, 120,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 128, 128,   0,   0,   0, 129,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 121, 122,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 130, 131,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   3,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 123,   0,   0,   0,   1,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 132,   0,   0,   0,   1,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0, 124, 125, 126,   0,   0, 127, 128,   0,   0,   0,   0,   0,   0,
+      0,   0,   0, 133, 134, 135,   0,   0, 136, 137,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0, 129,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0, 138,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,
-    130,   0,   0, 131,   0,   0,   0, 132,   0, 133,   0,   0,   0,   0,   0,   0,
+    139,   0,   0, 140,   0,   0,   0, 141,   0, 142,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0, 134,   0,   0, 135,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0, 136, 137,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0, 143,   0,   0, 144,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0, 145, 146,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  63,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 138,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  70,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 147,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0, 139,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0, 148,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0, 140,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0, 141,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0, 149,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0, 150,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0
 };
 
 static RE_UINT8 re_numeric_value_table_3[] = {
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -19531,31 +20221,37 @@
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   6,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   8,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       2,   0,   0,   8,   0,   0,   0,  45,   0,   4,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  10,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   3,   0,   0,   0,
       0,   0,   0,   0,   6,   0,   5,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  97,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  97,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  98,
      18,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  20,
       0,   0,   0,   0,   0,   0,   0,   0,   4,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   6,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      19,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,  97,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   3,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,  98,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,  98,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  99,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   3,   0,   9,   0,   7,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,  18,   0,  20,  37,  38,   0,   0,   0,   0,   0,   0,  39,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   4,   4,   4,   4,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -19566,33 +20262,45 @@
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   2,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  10,  37,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   2,   3,   4,   0,
       3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      8,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  18,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   9,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   8,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,   0,
       0,   0,   0,   0,   0,   0,   8,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,  10,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  19,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0, 100,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 101,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   5,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  45,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   3,   0,
       0,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  10,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,  10,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,  20,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   7,   0,   0,   0,   0,   0,  19,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   7,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -19606,47 +20314,47 @@
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   7,   0,   7,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  18,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   2,   3,   4,   5,   6,   7,   8,   9,  10,
-     18,  37,  38,  39,  40,  41,  42,  43,  44,  19,  99, 100, 101,  63, 102, 103,
-    104, 105,  20, 106, 107, 108,  64, 109, 110, 111, 112,  45, 113, 114, 115,  65,
-    116, 117, 118, 119,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+     18,  37,  38,  39,  40,  41,  42,  43,  44,  19, 100, 102, 103,  63, 104, 105,
+    106, 107,  20, 108, 109, 110,  64, 111, 112, 113, 114,  45, 115, 116, 117,  65,
+    118, 119, 120, 121,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      11,  12,   2,   6,  40,  63,  64,  65,   6,  18,  40,  19,  63,  20,  64,   6,
      18,  40,  19,  63,  20,  45,  65,  18,   2,   2,   2,   3,   3,   3,   3,   6,
-     18,  18,  18,  18,  18,  38,  40,  40,  40,  40,  19, 100,  63,  63,  63,  63,
+     18,  18,  18,  18,  18,  38,  40,  40,  40,  40,  19, 102,  63,  63,  63,  63,
      63,  20,  64,   6,  40,  12,  12,  52,  13,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,  11,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  37,  38,  39,  40,  41,
-     42,  43,  44,  19,  99, 100, 101,  63, 102, 103, 104, 105,   0,   0,   0,   0,
+     42,  43,  44,  19, 100, 102, 103,  63, 104, 105, 106, 107,   0,   0,   0,   0,
       2,   6,  18,  40,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,  44,   0,   0,   0,   0,   0,   0,   0,   0, 105,   0,   0,   0,   0,   0,
+      0,  44,   0,   0,   0,   0,   0,   0,   0,   0, 107,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   2,   3,  18,  37,  19,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   2,   3,   4,  18,  37,  19,  20,  45,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   2,   3,   4,   5,   6,  18,  37,
       0,   0,   0,   0,   0,   0,   0,   2,   3,   4,   5,   5,   6,  18,  37,  19,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   2,   6,  18,  37,  19,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   2,  18,  37,  19,   3,   4,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 120,  12,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 122,  12,   0,   0,
       2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  37,  38,  39,  40,  41,  42,
-      0,   0,  19,  99, 100, 101,  63, 102, 103, 104, 105,  20, 106, 107, 108,  64,
-    109, 110, 111, 112,  45, 113, 114, 115,  65, 116, 117, 118, 119,  66, 121, 122,
-    123, 124, 125, 126, 127, 128, 129,  56,  11,  51, 130,  12, 131,  52,  13,  57,
+      0,   0,  19, 100, 102, 103,  63, 104, 105, 106, 107,  20, 108, 109, 110,  64,
+    111, 112, 113, 114,  45, 115, 116, 117,  65, 118, 119, 120, 121,  66, 123, 124,
+    125, 126, 127, 128, 129, 130, 131,  56,  11,  51, 132,  12, 133,  52,  13,  57,
       2,   3,   4,   5,  18,  37,  19,  20,  12,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   2,  40,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   2,  18,  37,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   2,   6,  18,  37,  19,
@@ -19654,15 +20362,15 @@
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   2,   3,   4,   5,  18,  37,  19,  20,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   2,   3,   4,   5,  18,  37,  19,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   2,   6,  18,  40,  19,  20,
       2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  37,  38,  39,  40,  41,  42,
-     43,  44,  19,  99, 100, 101,  63, 102, 103, 104, 105,  12,  11,  51,  52,   0,
+     43,  44,  19, 100, 102, 103,  63, 104, 105, 106, 107,  12,  11,  51,  52,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   2,   3,   4,
       5,   6,  18,  37,  38,  19,  12,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   2,  18,  37,  19,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   2,   3,   4,   5,  18,  37,  19,   0,   0,   0,   0,
@@ -19679,27 +20387,27 @@
       1,   2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  37,   0,   0,   0,   0,
       1,   2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  37,  38,  39,  40,  41,
      42,  43,  44,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   2,   3,   4,   5,   6,   7,   8,   9,  10,   2,   3,   4,   5,   6,   7,
       8,   9,  10,  18,  37,  38,  39,  40,  41,  42,  43,  44,  19,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    132,  21, 133, 134,  22, 135,  23, 136,  24,  14,  14,  25,  15,  26,  16,  27,
-     11,  12,  12,  13, 132,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    134,  21, 135, 136,  22, 137,  23, 138,  24,  14,  14,  25,  15,  26,  16,  27,
+     11,  12,  12,  13, 134,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       3,   4,   5,   6,   7,   8,   9,  10,   4,   5,   6,   7,   8,   9,  10,   5,
       6,   7,   8,   9,  10,   2,   3,   4,   5,   6,   7,   8,   9,  10,   2,   3,
       4,   5,   6,   3,   4,   4,   5,   6,   7,   8,   9,  10,   2,   3,   4,   4,
-      5,   6, 137, 138,   2,   3,   4,   4,   5,   6,   4,   4,   5,   5,   5,   5,
+      5,   6, 139, 140,   2,   3,   4,   4,   5,   6,   4,   4,   5,   5,   5,   5,
       7,   8,   8,   8,   9,   9,  10,  10,  10,  10,   3,   4,   5,   6,   7,   2,
       3,   4,   5,   5,   6,   6,   3,   4,   2,   3,  51,  52,  57,  51,  52,  15,
      11,  56,  11,  11,  12,  51,  52,  39,  40,   5,   6,   7,   8,   9,  10,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      1,   2,   3,   4,   5,   6,   7,   8,   9,  10,   0,  18,  19,  45, 139,  97,
-    140,  98,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      1,   2,   3,   4,   5,   6,   7,   8,   9,  10,   0,  18,  19,  45,  99,  98,
+    141, 142,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  61,  62,  67,  68,  69,
      17,  46,  47,  48,   2,   3,   4,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  61,  62,  67,  68,  69,
      17,  46,  47,  48,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  37,  38,  39,  40,  41,  42,
      43,  44,   2,   3,   4,   5,   6,   2,   6,   0,   0,   0,   0,   0,   0,   0,
@@ -19707,22 +20415,22 @@
       3,   4,   5,   6,   7,   8,   9,  10,   1,   2,   3,   4,   5,   6,   7,   8,
       9,  10,   1,   2,   3,   4,   5,   6,   7,   8,   9,  10,   1,   2,   3,   4,
       5,   6,   7,   8,   9,  10,   1,   2,   3,   4,   5,   6,   7,   8,   9,  10,
       0,   0,   0,   0,   0,   0,   0,   2,   3,   4,   5,   6,   7,   8,   9,  10,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  37,  38,  39,  40,  41,
-     42,  43,  44,  19,  99, 100, 101,  63, 102, 103, 104, 105,  20, 106, 107, 108,
-     64, 109, 110, 111, 112,  45, 113, 114, 115,  65, 116, 117, 118, 119,  66, 121,
-     66, 141, 142,   2,   3,   4,   5,   6,   7,   8,   9,  10,   0,  11,  12,  13,
+     42,  43,  44,  19, 100, 102, 103,  63, 104, 105, 106, 107,  20, 108, 109, 110,
+     64, 111, 112, 113, 114,  45, 115, 116, 117,  65, 118, 119, 120, 121,  66, 123,
+     66, 143, 144,   2,   3,   4,   5,   6,   7,   8,   9,  10,   0,  11,  12,  13,
       0,   2,   3,  45,  66,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   2,   3,   4,   5,   6,   7,   8,   9,  10,  18,  37,  38,  39,  40,  41,
-     42,  43,  44,  19,  99, 100, 101,  63, 102, 103, 104, 105,  20, 106, 107, 108,
-     64, 109, 110, 111, 112,  45, 113, 114, 115,  65, 116, 117, 118, 119,   0,   3,
-      4,   5,   6,   7,   8,   9,  10,  18, 101, 102, 106,  45,  12,  56,   0,   0,
+     42,  43,  44,  19, 100, 102, 103,  63, 104, 105, 106, 107,  20, 108, 109, 110,
+     64, 111, 112, 113, 114,  45, 115, 116, 117,  65, 118, 119, 120, 121,   0,   3,
+      4,   5,   6,   7,   8,   9,  10,  18, 103, 104, 108,  45,  12,  56,   0,   0,
       1,   1,   2,   3,   4,   5,   6,   7,   8,   9,  10,   1,   1,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   8,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   5,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   5,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -20193,14 +20901,20 @@
         return 1;
     if (codepoint == 0x0387)
         return 1;
     if (0x1369 <= codepoint && codepoint <= 0x1371)
         return 1;
     if (codepoint == 0x19DA)
         return 1;
+    if (0x200C <= codepoint && codepoint <= 0x200D)
+        return 1;
+    if (codepoint == 0x30FB)
+        return 1;
+    if (codepoint == 0xFF65)
+        return 1;
 
     return 0;
 }
 
 /* Other_ID_Start. */
 RE_UINT32 re_get_other_id_start(RE_UINT32 codepoint) {
     if (0x1885 <= codepoint && codepoint <= 0x1886)
@@ -20625,16 +21339,16 @@
     20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 10, 30, 13, 31, 10, 10,
     10, 32, 10, 10, 10, 10, 10, 10, 10, 10, 33, 34, 13, 13, 13, 13,
     13, 35, 13, 36, 10, 10, 10, 10, 10, 10, 10, 37, 38, 10, 10, 39,
     10, 10, 10, 10, 10, 40, 10, 41, 42, 43, 44, 45, 46, 10, 10, 10,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 47, 13, 13, 13, 48, 49, 13,
-    13, 13, 13, 50, 13, 13, 13, 13, 13, 13, 51, 10, 10, 10, 52, 10,
-    13, 13, 13, 13, 53, 13, 13, 13, 54, 10, 10, 10, 10, 10, 10, 10,
+    13, 13, 13, 50, 13, 13, 13, 13, 13, 13, 51, 52, 10, 10, 53, 10,
+    13, 13, 13, 13, 54, 13, 13, 13, 55, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
@@ -20788,15 +21502,17 @@
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5, 167,   5,   5,   5,   5,   5,   5,
     118,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5, 269,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
-      5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,  79,
+      5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5, 270,
+      5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
+      5,   5, 118,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
     118,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,  33,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,  93,   0,   0
 };
@@ -20865,15 +21581,15 @@
       0,   0, 239, 111,   7,   0,   4,   0,   0,   0,  39,   0, 255,   7, 255,  31,
     255,   1, 255,  67, 255, 255, 223, 255, 255, 255, 255, 223, 100, 222, 255, 235,
     239, 255, 255, 255, 191, 231, 223, 223, 255, 255, 255, 123,  95, 252, 253, 255,
      63, 255, 255, 255, 253, 255, 255, 247, 255, 127, 255, 255, 247,  15,   0,   0,
     224,   7,   0,   0, 127, 255, 255, 249, 219,   7, 255, 255, 255,  31, 128,  63,
       0,  64,   0,   0, 255,  15,   0,   0, 127, 111, 255, 127, 143,   8,   0,   0,
     150, 254, 247,  10, 132, 234, 150, 170, 150, 247, 247,  94, 255, 251, 255,  15,
-    238, 251, 255,  15,   3,   0, 255, 255
+    238, 251, 255,  15,   3,   0, 255, 255,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_posix_alnum(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -20991,75 +21707,75 @@
      63,  64,  65,  66,  67,  54,  46,   0,  68,  69,  70,   0,  71,  54,  54,  54,
      54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,
      54,  72,  52,   0,  57,  73,   0,   0,  54,  54,  54,  54,  54,  54,  54,  54,
      54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  73,  74,  54,  54,  54,
      54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,
      54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  75,  76,  54,  54,  54,
       0,   0,   0,   0,   0,   0,   0,  77,   0,   0,   0,  28,   0,   0,   0,   0,
-     54,  78,  79,   0,  80,  54,  54,  81,  54,  54,  54,  54,  54,  54,  73,  82,
-     83,  84,   0,   0,  48,  46,   0,  43,   0,   0,   0,   0,  85,   0,  54,  86,
-     65,  87,  88,  54,  87,  89,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,
+     54,  78,  79,   0,  80,  54,  54,  81,  54,  54,  54,  54,  54,  54,  73,  63,
+     82,  83,   0,   0,  48,  46,   0,  43,   0,   0,   0,   0,  84,   0,  54,  85,
+     65,  86,  87,  54,  86,  88,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  54,  54,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,  63,  54,  72,  40,   0,   0,   0,   0,   0,   0,   0,   0,
-     90,   0,   0,  91,   0,   0,   0,  92,  93,  94,   0,   0,  95,   0,   0,   0,
-      0,  96,   0,  97,   0,   0,  98,  99,   0,  98,  35,   0,   0,   0, 100,   0,
-      0,   0,  57, 101,   0,   0,  40,  27,   0,   0,  43, 102,   0,   0,   0, 103,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0, 104,   0,   0,   0, 105, 106,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,  40, 107,   0,   0,   0,  32,  57,
-     45,  63, 108, 109,   0,   0,   0,   0,   1,   2,   2, 110,   0,   0,   0, 111,
-      0,   0,   0,   0,   0,   0,   0,   0, 106, 112,   0, 113, 114,  46,  63, 115,
+     89,   0,   0,  90,   0,   0,   0,  91,  92,  93,   0,   0,  94,   0,   0,   0,
+      0,  95,   0,  96,   0,   0,  97,  98,   0,  97,  35,   0,   0,   0,  99,   0,
+      0,   0,  57, 100,   0,   0,  40,  27,   0,   0,  43, 101,   0,   0,   0, 102,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0, 103,   0,   0,   0, 104, 105,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,  40, 106,   0,   0,   0,  32,  57,
+     45,  63, 107, 108,   0,   0,   0,   0,   1,   2,   2, 109,   0,   0,   0, 110,
+      0,   0,   0,   0,   0,   0,   0,   0, 105, 111,   0, 112, 113,  46,  63, 114,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  35,   0,  28,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  32,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   5, 116,   0,   0,   0,   0,  35,  35,   0,   0,   0,   0,   0,   0,
-      0,   0, 117,  35,   0,   0,  24, 118,   0, 113,   0,   0, 119,   0,   0,   0,
+      0,   0,   5, 115,   0,   0,   0,   0,  35,  35,   0,   0,   0,   0,   0,   0,
+      0,   0, 116,  35,   0,   0,  24, 117,   0, 112,   0,   0, 118,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0, 120,   0,   0,   0,   0, 121,   0, 122,   0,   0,   0,
-      0,   0, 123,   0,   0, 124,  94,   0,   0,   0,  86, 125,   0,   0, 126,   0,
-      0, 127,   0,   0,   0, 104,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0, 119,   0,   0,   0,   0, 120,   0, 121,   0,   0,   0,
+      0,   0, 122,   0,   0, 123,  93,   0,   0,   0, 124, 125,   0,   0, 126,   0,
+      0, 127,   0,   0,   0, 103,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0, 128,   0,   0,   0, 129,   0,   0,   0,   0,   0,   0,   0, 130,   0,
       0,   0, 131, 132,   0,  33,   0,   0,   0,  57,   0,   0,   0,   0,   0,   0,
       0,  43,   0,   0,   0,   0,   0,   0,   0,   0, 133,   0,   0,   0,   0,  11,
-      0,  35,  72,   0, 134, 106,   0,   0, 135,   0,   0,   0,   0,   0,   0,   0,
+      0,  35,  72,   0, 134, 105,   0,   0, 135,   0,   0,   0,   0,   0,   0,   0,
       0,   0, 136,  27,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0, 116,   0,   0, 137,   0,   0,   0, 138, 139,
+      0,   0,   0,   0,   0,   0,   0, 115,   0,   0, 137,   0,   0,   0, 138, 139,
       0,   0,   0, 140,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 141,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,  98,   0,   0,   0, 142,   0, 112, 143,   0,   0,   0,   0,   0,
+      0,   0,   0,  97,   0,   0,   0, 142,   0, 111, 143,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0, 144,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  11,
       0,   0,   0,   0, 145,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  63,  54,  54,  54,  86,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  63,  54,  54,  54, 124,   0,
      54,  54,  54,  54,  54,  54,  54,  73,  54, 146,  54, 147, 148, 149,  54,  52,
-     54,  54, 150,   0,   0,   0,   0,   0,  54,  54,  93,   0,   0,   0,   0,   0,
+     54,  54, 150,   0,   0,   0,   0,   0,  54,  54,  92,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 151,  43, 142, 142,  32,  32, 104, 104, 152,   0,
+      0,   0,   0,   0,   0,   0, 151,  43, 142, 142,  32,  32, 103, 103, 152,   0,
      54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,
       0, 144,   0, 153, 154,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  32,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,  35,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  40,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0, 155,   0,   0,   0, 156,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,  27,   0,   0,   0,   0,   0,   0,   0,   0,
-     54, 157,  54,  54,  81, 158, 159,  73, 160, 107,  42,  42,  87,  21,   0, 161,
-    162, 163, 164, 110,   0,   0,   0,   0,  54,  54,  54,  54,  54,  54,  54,  54,
+     54, 157,  54,  54,  81, 158, 159,  73, 160, 106,  42,  42,  86,  21,   0, 161,
+    162, 163, 164, 109,   0,   0,   0,   0,  54,  54,  54,  54,  54,  54,  54,  54,
      54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,  54,
      54,  54,  54,  54,  54,  54, 165, 166,  54,  54,  54, 167,  54,  54, 168, 169,
     157,  54, 170,  54,  64, 171,   0,   0,  54,  54,  54,  54,  54,  54,  54,  54,
-     54,  54,  81, 172, 173, 174, 175, 176,  54,  54,  54,  54, 108,  54,  52,   0
+     54,  54,  81, 172, 173, 174, 175, 176,  54,  54,  54,  54, 107,  54,  52,   0
 };
 
 static RE_UINT8 re_posix_punct_table_3[] = {
       0,   0,   0,   0, 254, 255,   0, 252,   1,   0,   0, 248,   1,   0,   0, 120,
     254, 219, 211, 137,   0,   0, 128,   0,  60,   0, 252, 255, 224, 175, 255, 255,
       0,   0,  32,  64, 176,   0,   0,   0,   0,   0,  64,   0,   4,   0,   0,   0,
       0,   0,   0, 252,   0, 230,   0,   0,   0,   0,   0,  64,  73,   0,   0,   0,
@@ -21075,26 +21791,26 @@
     255,   7,   0,   0,  49,   0,   0,   0, 255, 255, 255, 255, 127,  63,   0,   0,
     255,   7, 240, 127,   0,   0,   0, 240,   0,   0,   0, 248, 255,   0,   8,   0,
       0,   0,   0, 160,   3, 224,   0, 224,   0, 224,   0,  96,   0,   0, 255, 255,
     255,   0, 255, 255, 255, 255, 255, 127,   0,   0,   0, 124,   0, 124,   0,   0,
     123,   3, 208, 193, 175,  66,   0,  12,  31, 188,   0,   0,   0,  12, 255, 255,
     127,   0,   0,   0, 255, 255,  63,   0,   0,   0, 240, 255, 255, 255, 207, 255,
     255, 255, 191, 255, 224,   7,   0, 222, 255, 127, 255, 255, 255, 255, 255,  63,
-    255, 255, 255, 251, 255, 255,  15,   0,   0,   0, 255,  15,  30, 255, 255, 255,
-      1,   0, 193, 224,   0,   0, 195, 255,  15,   0,   0,   0,   0, 252, 255, 255,
-    255,   0,   1,   0, 255, 255,   1,   0,   0, 224,   0,   0,   0,   0,   8,  64,
-      0,   0, 252,   0, 255, 255, 127,   0,   3,   0,   0,   0,   0,   6,   0,   0,
-      0,  15, 192,   3,   0,   0, 240,   0,   0, 192,   0,   0,   0,   0,   0,  23,
-    254,  63,   0, 192,   0,   0, 128,   3,   0,  12,   0,   0,   0,   8,   0,   0,
-      0,   2,   0,   0,   0,   0, 252, 255,   7,   0,   0,   0, 255, 255,   0,   0,
-    255, 255, 247, 255, 127,  15,   0,   0,  63,   0,   0,   0, 127, 127,   0,  48,
-      0,   0, 128, 255,   0,   0,   0, 254, 255, 115, 255,  31, 255, 255, 255,  31,
-      0,   0, 128,   1,   0,   0, 255,   1,   0,   0, 127,   0,   0,   0,   0,  30,
-      0,  32,   0,   0,   0,   0, 224,   3, 192,   3,   0,   0, 128,  63,   0,   0,
-      0,   0,   0, 216,   0,   0,  48,   0, 224,  33,   0, 232,   0,   0,   0,  63,
+    255, 255, 255, 251, 255, 255,  15,   0,  30, 255, 255, 255,   1,   0, 193, 224,
+      0,   0, 195, 255,  15, 128,   0,   0,   0, 252, 255, 255, 255,   0,   1,   0,
+    255, 255,   1,   0,   0, 224,   0,   0,   0,   0,   8,  64,   0,   0, 252,   0,
+    255, 255, 127,   0,   3,   0,   0,   0,   0,   6,   0,   0,   0,  15, 192,   3,
+      0,   0, 240,   0,   0, 192,   0,   0,   0,   0,   0,  23, 254,  63,   0, 192,
+      0,   0, 128,   3,   0,  12,   0,   0,   0,   8,   0,   0,   0,   2,   0,   0,
+      0,   0, 252, 255,   7,   0,   0,   0, 255, 255,   0,   0, 255, 255, 247, 255,
+    127,  15,   0,   0,  63,   0,   0,   0, 127, 127,   0,  48,   0,   0, 128, 255,
+      0,   0,   0, 254, 255, 115, 255,  31, 255, 255, 255,  31,   0,   0, 128,   1,
+      0,   0, 255,   1,   0,   0, 127,   0,   0,   0,   0,  30,   0,  32,   0,   0,
+      0,   0, 224,   3, 192,   3,   0,   0, 128,  63,   0,   0,   0,   0,   0, 216,
+     15,   0,   0,   0,   0,   0,  48,   0, 224,  33,   0, 232,   0,   0,   0,  63,
       0, 248,   0,  44,  64,   0,   0,   0, 254, 255, 255,   0,  14,   0,   0,   0,
     255,  31,   0,   0, 112,   0,   0,   0,   0,   0,   0, 220, 255,   3,   0,   0,
      62,   0,   0,   0, 248, 255,   0,   0,   0,   0, 224, 255, 255, 255,   3, 128,
       0,   0,  31,   0,   0,   0,   6,   0,   0,   0,  32,   0,  48,   0,   0,   0,
       0,   0, 128,   7,   0,   0,   0, 144, 127, 254, 255, 255,  31,  28,   0,   0,
      24, 240, 255, 255, 255, 195, 255, 255,  35,   0,   0,   0,   2,   0,   0,   8,
       8,   0,   0,   0,   0, 224, 223, 255, 239,  15,   0,   0,   0,  16,   1,   0,
@@ -21166,16 +21882,16 @@
     20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 17, 30, 13, 31, 17, 17,
     17, 32, 17, 17, 17, 17, 17, 17, 17, 17, 33, 34, 13, 13, 13, 13,
     13, 35, 13, 36, 17, 17, 17, 17, 17, 17, 17, 37, 38, 17, 17, 39,
     17, 17, 17, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 17,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 52, 13, 13, 13, 53, 54, 13,
-    13, 13, 13, 55, 13, 13, 13, 13, 13, 13, 56, 17, 17, 17, 57, 17,
-    13, 13, 13, 13, 58, 13, 13, 13, 59, 17, 17, 17, 17, 17, 17, 17,
+    13, 13, 13, 55, 13, 13, 13, 13, 13, 13, 56, 57, 17, 17, 58, 17,
+    13, 13, 13, 13, 59, 13, 13, 13, 60, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
@@ -21211,26 +21927,26 @@
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
-    60, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
+    61, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
-    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 61,
+    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 62,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
-    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 61
+    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 62
 };
 
 static RE_UINT16 re_print_table_2[] = {
       0,   1,   1,   2,   0,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   3,   4,   5,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   6,   7,   1,   8,   1,   9,  10,
       1,   1,   1,   1,   1,   1,   1,   1,  11,   1,  12,   1,   1,  13,   1,  14,
@@ -21259,43 +21975,43 @@
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,  88,   1, 115,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1, 116,   1,   1,   1,   1,   1, 117,   1,   1,   1,   1,   1,   1, 118, 119,
       1, 120,   1, 117,   1,   1, 121,   1,   1,   1, 122,  68,   1,   1, 123,   2,
       1,  73, 124,   1,   1,   1, 125,  73, 126, 127,   1,  82,   1,   1,   1, 128,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 114, 129,  53,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 129, 130,  53,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
-      1,   1,   1,  86,   1,   1,  69,   0, 130, 131, 132,   1,   1,   1, 133,   1,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 134,   1, 135, 136,
+      1,   1,   1,  86,   1,   1,  69,   0, 131, 132, 133,   1,   1,   1, 134,   1,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 135,   1, 136, 111,
      69,   1, 137, 138,   1,   1,   1,  85,  51,   1,   1,   1,   1,   2, 139, 140,
-    141, 142, 143,   0,   1,   1,   1,  93, 144, 145,   1,   1, 100, 146, 136,  76,
+    141, 142, 143,   0,   1,   1,   1,  93, 144, 145,   1,   1, 100, 146, 111,  76,
       0,   0,   0,   0,  68,   1, 102,  53,   1, 147,  17,  93, 148,   1, 149,   0,
       1,   1,   1,   1,  76, 150, 151,  53,   1,   9,   1, 152, 153, 154,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,  73,  78, 155, 156, 157,   0,   0,
-    158, 159, 106,   1,   2, 160,   0, 161, 162, 163,   0,   0,   1, 164, 134,   1,
+    158, 159, 106,   1,   2, 160,   0, 161, 162, 163,   0,   0,   1, 164, 135,   1,
     165, 166, 167,   1,   1,   0,   1, 168,   1, 169, 170, 171, 172, 173,   0,   0,
       1,   1, 174,   0,   1, 175,   1, 176,   1, 177,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   2,   1, 178,   0, 179,   1,   9,  69, 136, 180, 136, 116,  73,
+      0,   0,   0,   2,   1, 178,   0, 179,   1,   9,  69, 111, 180, 111, 116,  73,
       1,   1, 181,  72,   1,   1, 182, 183,   1,  95,   9,  73,   1,   1,   1, 184,
     185,   1, 186,   0, 187, 150,   1, 188,  19, 189, 190, 191,   0,   0,   0,   0,
       1,   1, 192, 186,   1,   1, 177,   0,   0,   0,   0,   0,   1, 170,  76,   0,
       1,   1, 193, 194,   1,  69, 180,   0,  14,  82, 103,   0,   0,   0,   0,   0,
       1,  53,   0,   0,   0,   1,   1, 195, 196, 197, 198,   0,   0,  98,   3, 199,
       1,   1,   9,   1,   1, 200,   1,  71, 180,   0,   0,   0,   0,   0,   0,   0,
-    201, 202, 203,  88, 134, 204,   0,   0, 205, 206, 177, 207, 208, 180,   0,   0,
+    201, 202, 203,  88, 135, 204,   0,   0, 205, 206, 177, 207, 208, 180,   0,   0,
       0,   0,   0,   0,   0,   0,   0,  71, 209, 210,  69,   0,   0, 211,   1, 212,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,  69,   0,   0,   0,
       1,   1,   1, 213,   1,   1,   1,   1,   1,   1, 214,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 136,   1,   1, 175,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 111,   1,   1, 175,
       1,   1,  78,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1, 103,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,  71,   2, 215,   1,   2, 150, 216,   1,   1, 217, 218, 219,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -21317,16 +22033,16 @@
       1,   1,  95,   1,  60, 231, 232,   1, 233, 234, 235,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1, 236,   1,   1,   1,   1,   1,   1,   1,   1, 237,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1, 238, 239,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   2, 240,   0,   0,   0,   0,   0,   0,
     241, 242,   1, 243, 244,   0,   0,   0,   1, 245, 246,   0,   0,   0,   0,   0,
-      0,   0,   0,   0, 136,  87,   1, 163,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 136,  69,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0, 111,  87,   1, 163,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 111,  69,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 247,
       1,   1,   1,   1,   1,   1, 248,   0,   1,   1, 249,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0, 250,   1, 251,   0,   0,  51,  76,   0,   0,   0,   0,   0,   0,
     232, 252, 253, 254, 255, 256,   0, 257,   0,   0,   0,   0,   0,   0,   0,   0,
       1,  82,   1,   1,  74, 258, 259,  78,   1,   1,   1,   1,   1, 243,   0, 260,
     200,  53, 261, 230,   0,   0,   0,   0,   1,   1,   1,   1,   1,   1,   1,   1,
@@ -21339,15 +22055,17 @@
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,  69,   1,   1,   1,   1,   1,   1,
      76,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1, 269,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 146,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 101,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
+      1,   1,  76,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
      76,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,  17,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1, 219,   0,   0,
     270,   1,   1,   1,   0,   0,   0,   0,   1,   1,   1,   1,   1,   1,   1, 219,
@@ -21380,22 +22098,22 @@
     241, 255, 255, 255, 255,  63,  31,   0, 255,  15, 255, 255, 255,   3, 255, 199,
     255, 255, 255, 207, 255, 255, 255, 159, 255,  63, 255, 255, 255, 127,   0,   0,
     255,  31, 255, 255, 255, 255,  15, 240, 255, 255, 255, 248, 255, 227, 255, 255,
     255,   1, 255, 255, 255, 255, 255,   7,  63,  63, 255, 170, 255, 255, 223, 255,
     223, 255, 207, 239, 255, 255, 220, 127, 255, 252, 255, 255, 223, 255, 243, 255,
     255, 127, 255,  31,   1,   0, 255, 255, 255, 255,   1,   0, 127,   0,   0,   0,
     255,   7,   0,   0, 255, 255, 207, 255, 255, 255, 191, 255, 255, 255,  15, 254,
-    255, 128,   1, 128, 127, 127, 127, 127, 255, 255, 255, 251,   0,   0, 255,  15,
-    224, 255, 255, 255, 255, 127, 255, 255,  15,   0, 255, 255, 127,   0, 255, 255,
+    255, 128,   1, 128, 127, 127, 127, 127, 255, 255, 255, 251,   0,   0, 255, 255,
+    224, 255, 255, 255, 255, 127, 255, 255,  15, 128, 255, 255, 127,   0, 255, 255,
     255,  15,   0,   0, 255, 255, 255,   0, 255,   7, 235,   3,   0,   0, 252, 255,
     255,  31, 255,   3,  63, 192, 255,   3, 255, 255,  15, 128, 255, 191, 255, 195,
     255,  63, 255, 243,   7,   0,   0, 248, 126, 126, 126,   0, 127, 127, 255, 255,
-    255,  63, 255,   3, 127, 248, 255, 255, 127,   0, 248, 224, 255, 255, 127,  95,
-    219, 255, 255, 255,   7,   0, 248, 255, 255, 255, 252, 255, 255, 128,   0,   0,
-      0,   0, 255, 255, 255, 255, 247, 255, 127,  15, 223, 255, 252, 252, 252,  28,
+    255,  63, 255,   3,  15,   0, 255, 255, 127, 248, 255, 255, 127,   0, 248, 224,
+    255, 255, 127,  95, 219, 255, 255, 255,   7,   0, 248, 255, 255, 255, 252, 255,
+    255, 128,   0,   0, 255, 255, 247, 255, 127,  15, 223, 255, 252, 252, 252,  28,
     127, 127,   0,  62, 255, 239, 255, 255, 127, 255, 255, 183, 255,  63, 255,  63,
     135, 255, 255, 255, 255, 255, 143, 255,   1,   0,   0,   0,  15, 224, 255, 255,
     255, 255, 255, 191,  15, 255,  63,   0, 255,   3, 255, 255, 255, 255,  15, 255,
      15, 128, 255, 247, 255, 247, 183, 255, 251, 255, 251,  27, 255,   0,   0,   0,
     191, 255, 255, 255, 255, 255, 253,   7,  63, 253, 255, 255, 255, 255, 191, 145,
     128, 255,   0,   0, 255, 255,  55, 248, 255, 255, 255, 143, 255, 255, 255, 131,
     255, 255, 255, 240, 111, 240, 239, 254, 255, 255,  63, 135, 255,   1, 255,   1,
@@ -21587,16 +22305,16 @@
     23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 20, 33, 34, 35, 20, 20,
     20, 36, 20, 20, 20, 20, 20, 20, 20, 20, 37, 38, 39, 39, 39, 39,
     39, 40, 41, 42, 20, 20, 20, 20, 20, 20, 20, 43, 44, 20, 20, 45,
     20, 20, 20, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 20,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 58, 13, 13, 13, 59, 60, 13,
-    13, 13, 13, 61, 13, 13, 13, 13, 13, 13, 62, 20, 20, 20, 63, 20,
-    13, 13, 13, 13, 64, 13, 13, 13, 65, 20, 20, 20, 20, 20, 20, 20,
+    13, 13, 13, 61, 13, 13, 13, 13, 13, 13, 62, 63, 20, 20, 64, 20,
+    13, 13, 13, 13, 65, 13, 13, 13, 66, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
@@ -21632,15 +22350,15 @@
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
-    66, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
+    67, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
@@ -21693,101 +22411,103 @@
      96,  96,  96,  96,  96,  96,  96,  96,  96,  96,  96,  96,  96, 244, 245, 246,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82, 185, 185, 185, 185, 185, 185, 185, 185,
     185, 185, 185, 247, 185, 185, 248,  82, 249, 250, 251,  23,  23,  23, 252,  23,
      23,  23,  23,  23,  23,  23,  23,  23,  23, 253,  23,  23, 254,  23, 255, 256,
     257, 258, 259, 260,  23,  23,  23, 261, 262,   1,   1, 263, 264, 202, 265, 266,
-    267, 268, 269,  82, 270, 270, 270, 271, 272, 273,  11,  11, 274, 275, 276, 277,
-     82,  82,  82,  82, 278, 279, 280, 281, 282, 283, 284, 285, 286, 287, 288,  82,
-    289, 289, 290, 291, 292, 293, 294, 295, 296, 297, 298, 299, 300, 301,  82,  82,
-    302, 302, 302, 302, 302, 302, 302, 302, 302, 303, 304, 305, 306, 307,  82,  82,
-    308, 309, 310, 311, 312, 313,  82, 314, 315, 316,  82,  82, 317, 318, 319, 320,
-    321, 322, 323, 324, 325,  82, 326, 327, 328, 329, 330, 331, 332, 333,  82,  82,
-    334, 334, 335,  82, 336, 337, 336, 338, 339, 340,  82,  82,  82,  82,  82,  82,
-     82,  82,  82, 341, 342, 343,  82, 344, 345, 346, 347, 348, 349, 350, 351, 352,
-    353, 353, 354, 355, 356, 356, 357, 358, 359, 360, 361, 362, 363, 363, 363, 364,
-    365, 366, 367,  82, 368, 369, 370, 371, 372, 373, 374, 375,  82,  82,  82,  82,
-    376, 376, 377, 378, 379, 379, 380,  82,  82,  82,  82,  82, 381, 382, 383,  82,
-    384, 384, 385, 386, 387, 388, 389,  82, 390, 391, 392,  82,  82,  82,  82,  82,
-    393, 394,  82,  82,  82, 395, 395, 396, 397, 398, 399,  82,  82, 400, 401, 402,
-    403, 403, 404, 405, 405, 406, 407, 408, 409,  82,  82,  82,  82,  82,  82,  82,
-    410, 411, 412, 413, 414, 415,  82,  82, 416, 417, 418, 419, 420, 421,  82,  82,
-     82,  82,  82,  82,  82,  82,  82, 422, 423, 424, 425,  82,  82, 426, 427, 428,
-    429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 429,
-    429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 429, 430,  82,  82,  82,
-    429, 429, 429, 431, 429, 429, 429, 429, 429, 429, 432,  82,  82,  82,  82,  82,
+    267, 268, 269,  82, 270, 270, 270, 271, 272, 273,  11,  11, 274, 275, 188, 276,
+     82,  82,  82,  82, 277, 278, 279, 280, 281, 282, 283, 284, 285, 286, 287,  82,
+    288, 288, 289, 290, 291, 292, 293, 294, 295, 296, 297, 298, 299, 300,  82,  82,
+    301, 301, 301, 301, 301, 301, 301, 301, 301, 302, 303, 304, 305, 306,  82,  82,
+    307, 308, 309, 310, 311, 312,  82, 313, 314, 315,  82,  82, 316, 317, 318, 319,
+    320, 321, 322, 323, 324,  82, 325, 326, 327, 328, 329, 330, 331, 332,  82,  82,
+    333, 333, 334,  82, 335, 336, 335, 337, 338, 339,  82,  82,  82,  82,  82,  82,
+     82,  82,  82, 340, 341, 342,  82, 343, 344, 345, 346, 347, 348, 349, 350, 351,
+    352, 352, 353, 354, 355, 355, 356, 357, 358, 359, 360, 361, 362, 362, 362, 363,
+    364, 365, 366,  82, 367, 368, 369, 370, 371, 372, 373, 374,  82,  82,  82,  82,
+    375, 375, 376, 377, 378, 378, 379,  82,  82,  82,  82,  82, 380, 381, 382,  82,
+    383, 383, 384, 385, 386, 387, 388,  82, 389, 390, 391,  82,  82,  82,  82,  82,
+    392, 393,  82,  82,  82, 394, 394, 395, 396, 397, 398,  82,  82, 399, 400, 401,
+    402, 402, 403, 404, 404, 405, 406, 407, 408,  82,  82,  82,  82,  82,  82,  82,
+    409, 410, 411, 412, 413, 414,  82,  82, 415, 416, 417, 418, 419, 420,  82,  82,
+     82,  82,  82,  82,  82,  82,  82, 421, 422, 423, 424,  82,  82, 425, 426, 427,
+    428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 428,
+    428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 428, 429,  82,  82,  82,
+    428, 428, 428, 430, 428, 428, 428, 428, 428, 428, 431,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
-     82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82, 433, 434, 434, 435,
-    436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436,
-    436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436, 436,
-    436, 436, 437,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
+     82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82, 432, 433, 433, 434,
+    435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435,
+    435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435, 435,
+    435, 435, 436,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
-    438, 438, 438, 438, 438, 438, 438, 438, 438, 438, 438, 438, 438, 438, 438, 438,
-    438, 438, 439,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
+    437, 437, 437, 437, 437, 437, 437, 437, 437, 437, 437, 437, 437, 437, 437, 437,
+    437, 437, 438,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
     213, 213, 213, 213, 213, 213, 213, 213, 213, 213, 213, 213, 213, 213, 213, 213,
-    213, 440, 441, 442, 443, 444, 445, 446, 447, 447, 448, 449, 450,  82,  82,  82,
+    213, 439, 440, 441, 442, 443, 444, 445, 446, 446, 447, 448, 449,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
-     82,  82, 451, 451, 452,  82,  82,  82, 453, 453, 454, 453, 455,  82,  82, 456,
-    457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457,
-    457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457,
-    457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457,
-    457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 458,
-    457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457, 457,
-    457, 457, 457, 457, 457, 457, 457, 457, 459, 459, 459, 459, 459, 459, 459, 459,
-    459, 459, 459, 459, 459, 459, 460,  82, 461,  82,  82,  82,  82,  82,  82,  82,
+     82,  82, 450, 450, 451,  82,  82,  82, 452, 452, 453, 452, 454,  82,  82, 455,
+    456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456,
+    456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456,
+    456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456,
+    456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 457,
+    456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456, 456,
+    456, 456, 456, 456, 456, 456, 456, 456, 458, 458, 458, 458, 458, 458, 458, 458,
+    458, 458, 458, 458, 458, 458, 459,  82, 460,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
-     82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82, 462,
-    463, 192, 192, 192, 192, 192, 192, 192, 192, 464, 465, 466, 467, 467, 467, 467,
-    467, 467, 467, 467, 467, 467, 467, 468,  82,  82,  82,  82,  82,  82,  82,  82,
-    469, 469, 469, 470, 471, 472,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
+     82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82, 461,
+    462, 192, 192, 192, 192, 192, 192, 192, 192, 463, 464, 465, 466, 466, 466, 466,
+    466, 466, 466, 466, 466, 466, 466, 467,  82,  82,  82,  82,  82,  82,  82,  82,
+    468, 468, 468, 469, 470, 471,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
-     82,  82,  82,  82,  82,  82,  82,  82,   7, 473, 474,   0,   0,   0, 472,  82,
-      0,   0,   0,   0,   0,   0,   0, 475,   0, 476,   0, 477, 478, 479,   0, 171,
-     11,  11, 480,  82,  82,  82, 481, 481,   0,   0, 482, 483,  82,  82,  82,  82,
-      0,   0, 484,   0, 485, 486, 487,   0, 488, 489, 490,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0, 491,   0,   0,   0,   0,   0,   0,   0,   0, 492,   0,
-    493, 493, 493, 493, 493, 493, 493, 493, 493, 493, 493, 493, 493, 493, 493, 493,
-    493, 493, 493, 493, 494, 495,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
+     82,  82,  82,  82,  82,  82,  82,  82,   7, 472, 473,   0,   0,   0, 471,  82,
+      0,   0,   0,   0,   0,   0,   0, 474,   0, 475,   0, 476, 477, 478,   0, 171,
+     11,  11, 479,  82,  82,  82, 480, 480,   0,   0, 481, 482,  82,  82,  82,  82,
+      0,   0, 483,   0, 484, 485, 486,   0, 487, 488, 489,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0, 490,   0,   0,   0,   0,   0,   0,   0,   0, 491,   0,
+    492, 492, 492, 492, 492, 492, 492, 492, 492, 492, 492, 492, 492, 492, 492, 492,
+    492, 492, 492, 492, 493, 494,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
-     82,  82,  82,  82,  82,  82,  82,  82, 496, 497,  82,  82,  82,  82,  82,  82,
-    498, 499,  13, 500, 501,  82,  82,  82, 502, 503, 504,  82,  82,  82,  82,  82,
-     82,  82,  82,  82, 505, 506, 507, 508,  82,  82,  82,  82,  82,  82,  82,  82,
-     82,  82,  82,  82,  82,  82, 509, 510,  82,  82,  82,  82,  82,  82,  82,  82,
-     82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82, 511,
-    512, 512, 512, 512, 512, 512, 513,  82, 514, 514, 515,  82,  82,  82,  82,  82,
+     82,  82,  82,  82,  82,  82,  82,  82, 495, 496,  82,  82,  82,  82,  82,  82,
+    497, 498,  13, 499, 500,  82,  82,  82, 501, 502, 503,  82,  82,  82,  82,  82,
+     82,  82,  82,  82, 504, 505, 506, 507,  82,  82,  82,  82,  82,  82,  82,  82,
+     82,  82,  82,  82,  82,  82, 508, 509,  82,  82,  82,  82,  82,  82,  82,  82,
+     82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82, 510,
+    511, 511, 511, 511, 511, 511, 512,  82, 513, 513, 514,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
-     82,  82,  82, 516,   0, 517,  82,  82, 262, 183,  82,  82,  82,  82,  82,  82,
-    518, 519, 520, 521, 522, 523,  82, 524,  82,  82,  82,  82,  82,  82,  82,  82,
-      0, 525,   0,   0, 481, 526, 527, 475,   0,   0,   0,   0,   0, 528,  82, 529,
-    530, 531, 532, 533,  82,  82,  82,  82,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 534, 535,   0,   0,   0, 536,   0,   0, 537, 538,
-    525,   0, 539,   0, 540, 541,  82,  82,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0, 481, 542, 543, 544, 545, 546,   0,   0,   0,   0, 259,   0, 171, 547,
+     82,  82,  82, 515,   0, 516,  82,  82, 262, 183,  82,  82,  82,  82,  82,  82,
+    517, 518, 519, 520, 521, 522,  82, 523,  82,  82,  82,  82,  82,  82,  82,  82,
+      0, 524,   0,   0, 480, 525, 526, 474,   0,   0,   0,   0,   0, 527,  82, 528,
+    529, 530, 531, 532,  82,  82,  82,  82,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 533, 534,   0,   0,   0, 535,   0,   0, 536, 537,
+    524,   0, 538,   0, 539, 540,  82,  82,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0, 480, 541, 542, 543, 544, 545,   0,   0,   0,   0, 259,   0, 171, 546,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
     185, 185, 185, 185, 185, 185, 185,  82, 185, 185, 185, 185, 185, 185, 185, 185,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 248, 185, 185, 185, 185, 185, 185,
-    548, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
+    547, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
+    185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
+    185, 185, 185, 185, 185, 548, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
-    185, 185, 185, 185, 185, 549, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
+    185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 549,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
-    185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 550,
+    185, 185, 547,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
-    548,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
+    547,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
-    185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 551, 185, 185, 185, 185, 185,
+    185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 550, 185, 185, 185, 185, 185,
     185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185,
-    185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 552,  82,  82,
-    553,   0,   0,   0,  82,  82,  82,  82,   7,   7,   7,   7,   7,   7,   7, 554,
+    185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 185, 551,  82,  82,
+    552,   0,   0,   0,  82,  82,  82,  82,   7,   7,   7,   7,   7,   7,   7, 553,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82
 };
 
 static RE_UINT8 re_script_table_3[] = {
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
@@ -22161,15 +22881,15 @@
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,   0,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,  56,   1,  56,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,  56,  56,  56,  56,  56,  56,  56,  56,  56,   4,   4,   4,   4,  31,  31,
       1,   1,   1,   1,   1,   1,   1,   1,  56,  56,  56,  56,   1,   1,   1,   1,
       0,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,
      57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,
      57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,
@@ -22186,15 +22906,15 @@
       3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,
       3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,
       0,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,
       3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,
-      1,   1,   1,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      1,   1,   1,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,
      58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,   0,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
      58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,
@@ -22336,16 +23056,14 @@
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   0,   0,   0,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,
       5,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   4,   0,   0,
      73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,
      73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,   0,   0,   0,
      74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,
      74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,
      74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,
@@ -22885,15 +23603,15 @@
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,   0,   0,   0,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,   0,   0,
      56,  56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+     56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,   0,   0,   0,   0,   0,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
@@ -22926,16 +23644,16 @@
     23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 20, 33, 34, 35, 20, 20,
     20, 36, 20, 20, 20, 20, 20, 20, 20, 20, 37, 38, 39, 39, 39, 39,
     39, 40, 41, 42, 20, 20, 20, 20, 20, 20, 20, 43, 44, 20, 20, 45,
     20, 20, 20, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 20,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 58, 13, 13, 13, 59, 60, 13,
-    13, 13, 13, 61, 13, 13, 13, 13, 13, 13, 62, 20, 20, 20, 63, 20,
-    13, 13, 13, 13, 64, 13, 13, 13, 65, 20, 20, 20, 20, 20, 20, 20,
+    13, 13, 13, 61, 13, 13, 13, 13, 13, 13, 62, 63, 20, 20, 64, 20,
+    13, 13, 13, 13, 65, 13, 13, 13, 66, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
@@ -22971,15 +23689,15 @@
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
-    66, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
+    67, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
     20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20, 20,
@@ -23031,101 +23749,103 @@
      98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98, 257, 258, 259,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83, 190, 190, 190, 190, 190, 190, 190, 190,
     190, 190, 190, 260, 190, 190, 261,  83, 262, 263, 264,  24,  24,  24, 265,  24,
      24,  24,  24,  24,  24,  24,  24,  24,  24, 266,  24,  24, 267,  24, 268, 269,
     270, 271, 272, 273,  24,  24,  24, 274, 275,   1,   1, 276, 277, 208, 278, 279,
-    280, 281, 282,  83, 283, 283, 283, 284, 285, 286,  12,  12, 287, 288, 289, 290,
-     83,  83,  83,  83, 291, 292, 293, 294, 295, 296, 297, 298, 299, 300, 301,  83,
-    302, 302, 303, 304, 305, 306, 307, 308, 309, 310, 311, 312, 313, 314,  83,  83,
-    315, 315, 315, 315, 315, 315, 315, 315, 315, 316, 317, 318, 319, 320,  83,  83,
-    321, 322, 323, 324, 325, 326,  83, 327, 328, 329,  83,  83, 330, 331, 332, 333,
-    334, 335, 336, 337, 338,  83, 339, 340, 341, 342, 343, 344, 345, 346,  83,  83,
-    347, 347, 348,  83, 349, 350, 349, 351, 352, 353,  83,  83,  83,  83,  83,  83,
-     83,  83,  83, 354, 355, 356,  83, 357, 358, 359, 360, 361, 362, 363, 364, 365,
-    366, 366, 367, 368, 369, 369, 370, 371, 372, 373, 374, 375, 376, 376, 376, 377,
-    378, 379, 380,  83, 381, 382, 383, 384, 385, 386, 387, 388,  83,  83,  83,  83,
-    389, 389, 390, 391, 392, 392, 393,  83,  83,  83,  83,  83, 394, 395, 396,  83,
-    397, 397, 398, 399, 400, 401, 402,  83, 403, 404, 405,  83,  83,  83,  83,  83,
-    406, 407,  83,  83,  83, 408, 408, 409, 410, 411, 412,  83,  83, 413, 414, 415,
-    416, 416, 417, 418, 418, 419, 420, 421, 422,  83,  83,  83,  83,  83,  83,  83,
-    423, 424, 425, 426, 427, 428,  83,  83, 429, 430, 431, 432, 433, 434,  83,  83,
-     83,  83,  83,  83,  83,  83,  83, 435, 436, 437, 438,  83,  83, 439, 440, 441,
-    442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 442,
-    442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 442, 443,  83,  83,  83,
-    442, 442, 442, 444, 442, 442, 442, 442, 442, 442, 445,  83,  83,  83,  83,  83,
+    280, 281, 282,  83, 283, 283, 283, 284, 285, 286,  12,  12, 287, 288, 193, 289,
+     83,  83,  83,  83, 290, 291, 292, 293, 294, 295, 296, 297, 298, 299, 300,  83,
+    301, 301, 302, 303, 304, 305, 306, 307, 308, 309, 310, 311, 312, 313,  83,  83,
+    314, 314, 314, 314, 314, 314, 314, 314, 314, 315, 316, 317, 318, 319,  83,  83,
+    320, 321, 322, 323, 324, 325,  83, 326, 327, 328,  83,  83, 329, 330, 331, 332,
+    333, 334, 335, 336, 337,  83, 338, 339, 340, 341, 342, 343, 344, 345,  83,  83,
+    346, 346, 347,  83, 348, 349, 348, 350, 351, 352,  83,  83,  83,  83,  83,  83,
+     83,  83,  83, 353, 354, 355,  83, 356, 357, 358, 359, 360, 361, 362, 363, 364,
+    365, 365, 366, 367, 368, 368, 369, 370, 371, 372, 373, 374, 375, 375, 375, 376,
+    377, 378, 379,  83, 380, 381, 382, 383, 384, 385, 386, 387,  83,  83,  83,  83,
+    388, 388, 389, 390, 391, 391, 392,  83,  83,  83,  83,  83, 393, 394, 395,  83,
+    396, 396, 397, 398, 399, 400, 401,  83, 402, 403, 404,  83,  83,  83,  83,  83,
+    405, 406,  83,  83,  83, 407, 407, 408, 409, 410, 411,  83,  83, 412, 413, 414,
+    415, 415, 416, 417, 417, 418, 419, 420, 421,  83,  83,  83,  83,  83,  83,  83,
+    422, 423, 424, 425, 426, 427,  83,  83, 428, 429, 430, 431, 432, 433,  83,  83,
+     83,  83,  83,  83,  83,  83,  83, 434, 435, 436, 437,  83,  83, 438, 439, 440,
+    441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 441,
+    441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 441, 442,  83,  83,  83,
+    441, 441, 441, 443, 441, 441, 441, 441, 441, 441, 444,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
-     83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83, 446, 447, 447, 448,
-    449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449,
-    449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449, 449,
-    449, 449, 450,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
+     83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83, 445, 446, 446, 447,
+    448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448,
+    448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448, 448,
+    448, 448, 449,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
-    451, 451, 451, 451, 451, 451, 451, 451, 451, 451, 451, 451, 451, 451, 451, 451,
-    451, 451, 452,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
+    450, 450, 450, 450, 450, 450, 450, 450, 450, 450, 450, 450, 450, 450, 450, 450,
+    450, 450, 451,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
     224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224,
-    224, 453, 454, 455, 456, 457, 458, 459, 460, 460, 461, 462, 463,  83,  83,  83,
+    224, 452, 453, 454, 455, 456, 457, 458, 459, 459, 460, 461, 462,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
-     83,  83, 464, 464, 465,  83,  83,  83, 466, 466, 467, 466, 468,  83,  83, 469,
-    470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470,
-    470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470,
-    470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470,
-    470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 471,
-    470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470, 470,
-    470, 470, 470, 470, 470, 470, 470, 470, 472, 472, 472, 472, 472, 472, 472, 472,
-    472, 472, 472, 472, 472, 472, 473,  83, 474,  83,  83,  83,  83,  83,  83,  83,
+     83,  83, 463, 463, 464,  83,  83,  83, 465, 465, 466, 465, 467,  83,  83, 468,
+    469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469,
+    469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469,
+    469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469,
+    469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 470,
+    469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469, 469,
+    469, 469, 469, 469, 469, 469, 469, 469, 471, 471, 471, 471, 471, 471, 471, 471,
+    471, 471, 471, 471, 471, 471, 472,  83, 473,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
-     83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83, 475,
-    476, 197, 197, 197, 197, 197, 197, 197, 197, 477, 478, 479, 480, 480, 480, 480,
-    480, 480, 480, 480, 480, 480, 480, 481,  83,  83,  83,  83,  83,  83,  83,  83,
-    482, 482, 482, 483, 484, 485,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
+     83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83, 474,
+    475, 197, 197, 197, 197, 197, 197, 197, 197, 476, 477, 478, 479, 479, 479, 479,
+    479, 479, 479, 479, 479, 479, 479, 480,  83,  83,  83,  83,  83,  83,  83,  83,
+    481, 481, 481, 482, 483, 484,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
-     83,  83,  83,  83,  83,  83,  83,  83,   7, 486, 487,   0,   0,   0, 488,  83,
-      0,   0,   0,   0,   0,   0,   0, 489,   0, 490,   0, 491, 492, 493,   0, 176,
-     12,  12, 494,  83,  83,  83, 495, 495,   0,   0, 496, 497,  83,  83,  83,  83,
-      0,   0, 498,   0, 499, 500, 501,   0, 502, 503, 504,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0, 505,   0,   0,   0,   0,   0,   0,   0,   0, 506,   0,
-    507, 507, 507, 507, 507, 507, 507, 507, 507, 507, 507, 507, 507, 507, 507, 507,
-    507, 507, 507, 507, 508, 509,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
+     83,  83,  83,  83,  83,  83,  83,  83,   7, 485, 486,   0,   0,   0, 487,  83,
+      0,   0,   0,   0,   0,   0,   0, 488,   0, 489,   0, 490, 491, 492,   0, 176,
+     12,  12, 493,  83,  83,  83, 494, 494,   0,   0, 495, 496,  83,  83,  83,  83,
+      0,   0, 497,   0, 498, 499, 500,   0, 501, 502, 503,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0, 504,   0,   0,   0,   0,   0,   0,   0,   0, 505,   0,
+    506, 506, 506, 506, 506, 506, 506, 506, 506, 506, 506, 506, 506, 506, 506, 506,
+    506, 506, 506, 506, 507, 508,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
-     83,  83,  83,  83,  83,  83,  83,  83, 510, 511,  83,  83,  83,  83,  83,  83,
-    512, 513,  14, 514, 515,  83,  83,  83, 516, 517, 518,  83,  83,  83,  83,  83,
-     83,  83,  83,  83, 519, 520, 521, 522,  83,  83,  83,  83,  83,  83,  83,  83,
-     83,  83,  83,  83,  83,  83, 523, 524,  83,  83,  83,  83,  83,  83,  83,  83,
-     83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83, 525,
-    526, 526, 526, 526, 526, 526, 527,  83, 528, 528, 529,  83,  83,  83,  83,  83,
+     83,  83,  83,  83,  83,  83,  83,  83, 509, 510,  83,  83,  83,  83,  83,  83,
+    511, 512,  14, 513, 514,  83,  83,  83, 515, 516, 517,  83,  83,  83,  83,  83,
+     83,  83,  83,  83, 518, 519, 520, 521,  83,  83,  83,  83,  83,  83,  83,  83,
+     83,  83,  83,  83,  83,  83, 522, 523,  83,  83,  83,  83,  83,  83,  83,  83,
+     83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83, 524,
+    525, 525, 525, 525, 525, 525, 526,  83, 527, 527, 528,  83,  83,  83,  83,  83,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
-     83,  83,  83, 530,   0, 531,  83,  83, 275, 532,  83,  83,  83,  83,  83,  83,
-    533, 534, 535, 536, 537, 538,  83, 539,  83,  83,  83,  83,  83,  83,  83,  83,
-      0, 540,   0,   0, 495, 541, 542, 489,   0,   0,   0,   0,   0, 543,  83, 544,
-    545, 546, 547, 548,  83,  83,  83,  83,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 549, 550,   0,   0,   0, 551,   0,   0, 552, 553,
-    540,   0, 554,   0, 555, 556,  83,  83,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0, 495, 557, 558, 559, 560, 561,   0,   0,   0,   0, 562,   0, 176, 563,
+     83,  83,  83, 529,   0, 530,  83,  83, 275, 531,  83,  83,  83,  83,  83,  83,
+    532, 533, 534, 535, 536, 537,  83, 538,  83,  83,  83,  83,  83,  83,  83,  83,
+      0, 539,   0,   0, 494, 540, 541, 488,   0,   0,   0,   0,   0, 542,  83, 543,
+    544, 545, 546, 547,  83,  83,  83,  83,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 548, 549,   0,   0,   0, 550,   0,   0, 551, 552,
+    539,   0, 553,   0, 554, 555,  83,  83,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0, 494, 556, 557, 558, 559, 560,   0,   0,   0,   0, 561,   0, 176, 562,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
     190, 190, 190, 190, 190, 190, 190,  83, 190, 190, 190, 190, 190, 190, 190, 190,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 261, 190, 190, 190, 190, 190, 190,
-    564, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
+    563, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
-    190, 190, 190, 190, 190, 565, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
+    190, 190, 190, 190, 190, 564, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
-    190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 566,
+    190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 565,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
-    564,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
+    190, 190, 563,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
-    190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 567, 190, 190, 190, 190, 190,
+    563,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,
     190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
-    190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 568,  83,  83,
-    569,   0,   0,   0,  83,  83,  83,  83,   7,   7,   7,   7,   7,   7,   7, 570,
+    190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 566, 190, 190, 190, 190, 190,
+    190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190,
+    190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 190, 567,  83,  83,
+    568,   0,   0,   0,  83,  83,  83,  83,   7,   7,   7,   7,   7,   7,   7, 569,
      83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83,  83
 };
 static RE_UINT8 script_extensions_table_3[] = {
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   1,   1,   1,   1,   1,
@@ -23508,15 +24228,15 @@
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,   0,
+      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1, 206, 206, 207,   1,  56, 208,  56, 206, 206, 206, 206, 206, 206, 206, 206,
     206, 206,   1, 207, 206, 206, 206, 206, 206, 206, 206, 206, 207, 207, 207, 207,
       1,  56,  56,  56,  56,  56,  56,  56,  56,  56, 209, 209, 209, 209,  31,  31,
     207, 210, 210, 210, 210, 210,   1, 207,  56,  56,  56,  56, 211, 211, 208, 208,
       0,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,
      57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,
      57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,  57,
@@ -23535,15 +24255,15 @@
       0,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,   0,
     208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208,
       3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,
       3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,   3,
     208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208,
     208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208, 208,
-    208, 208, 208, 208,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    208, 208, 208, 208,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,
      58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,  58,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,   0,
     208, 208, 208, 208, 208, 208, 208, 208,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,   1,
@@ -23586,36 +24306,36 @@
       2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   0,   0,   0,   0,   0,
       2,   2,   0,   2,   0,   2,   2,   2,   2,   2,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,   2,
      63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,
      63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,
      63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,  63,   0,   0,   0,
-    213, 213, 213, 214, 214, 214, 215, 215, 215, 215,   0,   0,   0,   0,   0,   0,
+    213, 213, 213, 214, 214, 214, 215, 215, 216, 215,   0,   0,   0,   0,   0,   0,
      64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,
      64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,
      64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,  64,
      64,  64,  64,  64,  64,  64,  64,  64,   0,   0,   0,   0,   0,   0,   0,   0,
      65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,
      65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,
      65,  65,  65,  65,  65,  65,   0,   0,   0,   0,   0,   0,   0,   0,  65,  65,
      65,  65,  65,  65,  65,  65,  65,  65,  65,  65,   0,   0,   0,   0,   0,   0,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-     16, 194,  16, 216,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
+     16, 194,  16, 217,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,
      66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,
-     66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66, 217,  66,
+     66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66,  66, 218,  66,
      67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,
      67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,  67,
      67,  67,  67,  67,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  67,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,
      31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,  31,   0,   0,   0,
      68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,
      68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,
-     68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,   0, 218,
+     68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,  68,   0, 219,
      68,  68,  68,  68,  68,  68,  68,  68,  68,  68,   0,   0,   0,   0,  68,  68,
      29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,
      29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,   0,
      69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,
      69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,
      69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,  69,
      69,  69,  69,  69,  69,  69,  69,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -23654,21 +24374,21 @@
       9,   9,   9,   9,   9,   9,   9,   9,   9,   9,   9,   9,   9,   9,   9,   9,
       9,   9,   9,   9,   9,   9,   9,   0,   9,   9,   9,   9,   9,   0,   9,   0,
       9,   9,   0,   9,   9,   0,   9,   9,   9,   9,   9,   9,   9,   9,   9,   9,
      10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,
      10,  10,  10,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,
      10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,
-     10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10, 219, 219,
+     10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10, 220, 220,
      10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,
       0,   0,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10,
      10,  10,  10,  10,  10,  10,  10,  10,   0,   0,   0,   0,   0,   0,   0,  10,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-     10,  10, 220,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10, 220,  10,  10,
+     10,  10, 221,  10,  10,  10,  10,  10,  10,  10,  10,  10,  10, 221,  10,  10,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   7,   7,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1, 207, 207,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   0,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   0,   1,   1,   1,   1,   0,   0,   0,   0,
@@ -23691,34 +24411,32 @@
      72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,   0,  72,  72,   0,  72,
      72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,   0,   0,
      72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,   0,   0,
      72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,
      72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,
      72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,
      72,  72,  72,  72,  72,  72,  72,  72,  72,  72,  72,   0,   0,   0,   0,   0,
-    221, 221, 222,   0,   0,   0,   0, 223, 223, 223, 223, 223, 223, 223, 223, 223,
-    223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223,
-    223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223, 223,
-    223, 223, 223, 223,   0,   0,   0, 222, 222, 222, 222, 222, 222, 222, 222, 222,
+    222, 222, 223,   0,   0,   0,   0, 224, 224, 224, 224, 224, 224, 224, 224, 224,
+    224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224,
+    224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224,
+    224, 224, 224, 224,   0,   0,   0, 223, 223, 223, 223, 223, 223, 223, 223, 223,
       5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   5,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,
       5,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   4,   0,   0,
      73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,
      73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,   0,   0,   0,
      74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,
      74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,
      74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,  74,
      74,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224,
-    224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224, 224,   0,   0,   0,   0,
+    225, 225, 225, 225, 225, 225, 225, 225, 225, 225, 225, 225, 225, 225, 225, 225,
+    225, 225, 225, 225, 225, 225, 225, 225, 225, 225, 225, 225,   0,   0,   0,   0,
      75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,
      75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,  75,
      75,  75,  75,  75,   0,   0,   0,   0,   0,   0,   0,   0,   0,  75,  75,  75,
      76,  76,  76,  76,  76,  76,  76,  76,  76,  76,  76,  76,  76,  76,  76,  76,
      76,  76,  76,  76,  76,  76,  76,  76,  76,  76,  76,   0,   0,   0,   0,   0,
      77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,
      77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,
@@ -23802,15 +24520,15 @@
      98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,
      98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,  98,
      99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,
      99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,  99,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100,   0,   0,   0,   0, 100, 100, 100, 100, 100,
-    100, 100, 225, 100, 100, 100, 100,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    100, 100, 226, 100, 100, 100, 100,   0,   0,   0,   0,   0,   0,   0,   0,   0,
     101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101,
     101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101,
     101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101,
     101, 101, 101, 101, 101, 101,   0,   0,   0, 101, 101, 101, 101, 101, 101, 101,
     102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102,
     102, 102, 102, 102, 102, 102,   0,   0, 102, 102, 102, 102, 102, 102, 102, 102,
     103, 103, 103, 103, 103, 103, 103, 103, 103, 103, 103, 103, 103, 103, 103, 103,
@@ -24091,15 +24809,15 @@
     154, 154, 154, 154, 154, 154, 154, 154, 154, 154, 154, 154,   0,   0,   0,   0,
     156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156,
     156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156,
     156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156,   0,   0,   0,   0,   0,
     156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156, 156,   0,   0,   0,
     156, 156, 156, 156, 156, 156, 156, 156, 156,   0,   0,   0,   0,   0,   0,   0,
     156, 156, 156, 156, 156, 156, 156, 156, 156, 156,   0,   0, 156, 156, 156, 156,
-    226, 226, 226, 226,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    227, 227, 227, 227,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -24254,51 +24972,52 @@
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,   0,   0,   0,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,   0,   0,
      56,  56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+     56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,   0,   0,   0,   0,   0,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
      56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,  56,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0
 };
 static RE_UINT16 script_extensions_table_4[] = {
       0,   2,   4,   7,  10,  13,  20,  24,  32,  42,  45,  49,  52,  66,  79, 100,
     122, 127, 131, 134, 137, 140, 143, 147, 150, 155, 158, 163, 165, 168, 171, 174,
-    181, 184, 193, 197, 199, 201, 204, 206, 209, 213, 220, 226, 228, 231, 234, 238,
-    241, 256, 270, 282, 285, 289, 292, 295, 298, 302, 305, 309, 312, 315
+    181, 184, 195, 199, 201, 203, 206, 208, 211, 215, 222, 228, 230, 233, 236, 240,
+    243, 259, 274, 286, 299, 302, 306, 309, 312, 315, 319, 322, 326, 329, 332
 };
 static RE_UINT8 script_extensions_table_5[] = {
       5,   0,   2,   0,   7,  77,   0,   7,  54,   0,   7,   2,   0,  10,  13, 107,
      11,  12, 108,   0,  10,  11,  12,   0, 163,  10,  13, 107,  11,  12, 108,   0,
     163,  10,  15, 100, 111, 104, 107, 110,  11,   0,  10,  11,   0,  10,  12, 108,
       0,  10, 107,   0,  17,  16, 123,  19,  18,  23,   2,  24,  20, 119,  21,  22,
     125,   0,  17,  16, 123,  19,  18,  23,   2,  24,  20,  21,  22, 125,   0,  17,
      16, 130, 140, 139, 123,  19,  18,  23, 118,  24, 133,  20, 122,  25,  63, 128,
      21,  22, 125,   0,  17,  16, 130, 140, 139, 123,  19,  18,  23,  43, 118,  24,
     133,  20, 122,  25,  63, 128,  21,  22, 125,   0,  16, 130, 115, 118,   0,  17,
     117,  63,   0,  18, 121,   0,  19, 120,   0, 123,  21,   0,  23, 133,   0, 117,
      29,  44,   0,  30,   2,   0,  39,  38,  40,  37,   0,  42,  64,   0,  17,  16,
     123,  23,   0,  16,   0,  16, 123,   0,  17,  16,   0,  16, 119,   0,  16,  23,
-     24,  20,  21,  22,   0,  16, 133,   0,  17,  16, 123,  23, 133,  20,  22, 125,
-      0,  16, 123,  23,   0,  17,   0, 133,   0,   7,  11,   0,  11,   0,   2,  42,
-      0,  16, 123,   2,   0,   3,  31,  56,  57,  58,  59,   0,   3,  31,  56,  57,
-     58,   0,  56,   0,   3,  56,   0,  57,  58,   0,  56,  57,  58,   0,  56,   2,
-      0,  16, 130,  19,  18, 120,  23, 115, 118,  24, 127, 133, 122, 128, 125,   0,
-     16, 130,  19,  18, 120,  23, 115, 118, 127, 133, 122, 128, 125,   0,  16, 130,
-     19,  18, 120, 115, 118, 127, 122, 128, 125,   0,  16,  21,   0,  66,   2,  29,
-      0,  46,  68,   0,  10,  13,   0,  10,  12,   0, 144,  88,  72,   0,  88,  72,
-      0,  88,  87,  72,   0,  10,   6,   0, 100, 111,   0, 156,   0
+     24,  20,  21,  22,   0,  16, 133,   0,  17,  16, 123,  23,  24, 133,  20,  25,
+     22, 125,   0,  16, 123,  23,   0,  17,   0, 133,   0,   7,  11,   0,  11,   0,
+      2,  42,   0,  16, 123,   2,   0,   3,  31,  56,  57,  58,  59,   0,   3,  31,
+     56,  57,  58,   0,  56,   0,   3,  56,   0,  57,  58,   0,  56,  57,  58,   0,
+     56,   2,   0,  16, 130,  19,  18, 120,  23, 115, 118,  24, 127, 133, 119, 122,
+    128, 125,   0,  16, 130,  19,  18, 120,  23, 115, 118, 127, 133, 119, 122, 128,
+    125,   0,  16, 130,  19,  18, 120, 115, 118, 127, 122, 128, 125,   0,  16, 130,
+     19,  18, 120, 115, 118, 127, 119, 122, 128, 125,   0,  16,  21,   0,  66,   2,
+     29,   0,  46,  68,   0,  10,  13,   0,  10,  12,   0, 144,  88,  72,   0,  88,
+     72,   0,  88,  87,  72,   0,  10,   6,   0, 100, 111,   0, 156,   0
 };
 
 int re_get_script_extensions(RE_UINT32 codepoint, RE_UINT8* scripts) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 v;
@@ -24339,16 +25058,16 @@
     21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 18, 31, 13, 32, 18, 18,
     18, 33, 18, 18, 18, 18, 18, 18, 18, 18, 34, 35, 13, 13, 13, 13,
     13, 36, 13, 37, 18, 18, 18, 18, 18, 18, 18, 38, 39, 18, 18, 40,
     18, 18, 18, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 18,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 53, 13, 13, 13, 54, 55, 13,
-    13, 13, 13, 56, 13, 13, 13, 13, 13, 13, 57, 18, 18, 18, 58, 18,
-    13, 13, 13, 13, 59, 13, 13, 13, 60, 18, 18, 18, 18, 18, 18, 18,
+    13, 13, 13, 56, 13, 13, 13, 13, 13, 13, 57, 58, 18, 18, 59, 18,
+    13, 13, 13, 13, 60, 13, 13, 13, 61, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
@@ -24384,15 +25103,15 @@
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
-    61, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
+    62, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
     18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18, 18,
@@ -24516,14 +25235,16 @@
     285,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
      40,  40,  40,  40,  40, 460,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40, 461,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
+     40,  40, 285, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
+     40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
     285, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  54,  40,  40,  40,  40,  40,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,
      40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40,  40, 124, 100, 100,
     462,  23,  23,  23, 100, 100, 100, 100,  23,  23,  23,  23,  23,  23,  23, 463,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100
@@ -24604,24 +25325,24 @@
      0, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0, 14,
      0, 14, 14,  0, 14, 14,  0, 14,  0,  0,  0,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,  0,  0,  0,  0, 13,
     13, 13, 13, 13,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    12, 12, 12, 12, 12, 12,  0,  0,  0,  0,  0,  0,  6,  6,  0,  0,
+     8,  8,  8,  8,  8,  8,  0,  0,  0,  0,  0,  0,  6,  6,  0,  0,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0, 12,  4,  4,  4,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
      8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  0,  8,  8,  0, 13, 13,
     14, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
-    13, 13, 13, 13,  4, 13, 14, 14, 14, 14, 14, 14, 14, 12,  0, 14,
+    13, 13, 13, 13,  4, 13, 14, 14, 14, 14, 14, 14, 14,  8,  0, 14,
     14, 14, 14, 14, 14, 13, 13, 14, 14,  0, 14, 14, 14, 14, 13, 13,
      8,  8,  8,  8,  8,  8,  8,  8,  8,  8, 13, 13, 13,  0,  0, 13,
      4,  4,  4,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 12,
     13, 14, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,  0, 13, 13, 13,
@@ -24637,18 +25358,18 @@
     14, 14, 14, 14, 13, 14, 14, 14, 13, 14, 14, 14, 14, 14,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  4,  0,  4,  0,  0,  0,  4,  4,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 14, 14, 14,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13,  0, 13, 13, 13, 13, 13, 13,  0,
-    12, 12,  0,  0,  0,  0,  0,  0, 14, 14, 14, 14, 14, 14, 14, 14,
+     8,  8,  0,  0,  0,  0,  0,  0, 14, 14, 14, 14, 14, 14, 14, 14,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
-    14, 14, 12, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
+    14, 14,  8, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 14, 14, 14, 13, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     13, 14, 14, 14, 14, 14, 14, 14, 13, 13, 13, 13, 13, 13, 13, 13,
@@ -24795,15 +25516,15 @@
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 14, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,  0, 13, 13,
     13,  0, 14, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
-    14, 14, 14, 14,  0,  0,  0, 13,  0,  0,  0,  0, 13, 14,  0,  0,
+    14, 14, 14, 14,  4,  4,  0, 13,  0,  0,  0,  0, 13, 14,  0,  0,
      8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  6,  4,  0,  0,  0,  0,  6,  4,  0, 14, 14, 14, 12, 14,
      8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  0,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13,  0,  0,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 14, 14, 13, 13, 13, 13, 13, 13, 13, 13, 13,
@@ -25167,16 +25888,16 @@
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14,  4,  4,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  8,  8,  8,  8,  8,  8,  8,  8,  8,  8,
     14, 13, 13, 14, 14, 13,  0,  0,  0,  0,  0,  0,  0,  0,  0, 14,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
-    14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,  0, 12,  4,  4,
-     4,  4, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 12,  0,  0,
+    14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,  0,  8,  4,  4,
+     4,  4, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  8,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13,  0,  0,  0,  0,  0,  0,  0,
      8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  0,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14,  0,  8,  8,  8,  8,  8,  8,  8,  8,  8,  8,
      0,  4,  4,  4, 13, 14, 14, 13,  0,  0,  0,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
@@ -25449,15 +26170,15 @@
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  5,  5,  5,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      8,  8,  8,  8,  8,  8,  8,  8,  8,  8,  0,  0,  0,  0,  0,  0,
     13, 13,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
      0, 12,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0
 };
 
 RE_UINT32 re_get_sentence_break(RE_UINT32 codepoint) {
@@ -25557,68 +26278,68 @@
      0,  7,  0,  0,  0,  0,  0,  0,  0,  0,  0,  8,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  9,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 10,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0, 11,  0,  0,  0,  0,  0, 12,  0,  0,  0,  0,  0,  0,
-    13,  0,  0,  0,  0,  0,  0,  0,  0,  0,  8,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0, 14,  0,  0,  0,  0, 15, 16,  0,  0,  0,  0,
-     0, 17,  0, 18,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0, 11,  0,  0,  0,  0,  0, 12,  0,  0,  0,  0, 13,  0,
+    14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  8,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0, 15,  0,  0,  0,  0, 16, 17,  0,  0,  0,  0,
+     0, 18,  0, 19,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0, 19, 20,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0, 20, 21,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0, 21, 22,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    23,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0, 22, 23,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+    24,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0, 24,  0,  0,  0,  0,  0,  0,  0,  0,
-    25,  0,  0,  0,  0,  0,  0, 26,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0, 27,  0,  0, 25,  0,  0, 28,  0,  0,  0,  0, 29,  0,
-     0,  0,  3,  0,  0,  0,  0, 30,  0,  0,  0,  0,  0,  0,  0, 31,
+     0,  0,  0,  0,  0,  0,  0, 25,  0,  0,  0,  0,  0,  0,  0,  0,
+    26,  0,  0,  0,  0,  0,  0, 27,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0, 28,  0,  0, 26,  0,  0, 29,  0,  0,  0,  0, 30,  0,
+     0,  0,  3,  0,  0,  0,  0, 31,  0,  0,  0,  0,  0,  0,  0, 32,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0, 32,  0,  0,  0,  0,  0,  1,  0,  0, 33,  0,  0,  0,  0,
+     0,  0, 33,  0,  0,  0,  0,  0,  1,  0,  0, 34,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0, 27,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0, 28,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 34,  0, 35,  0,  0,  0,
-     0,  0, 36,  0,  0, 18, 37,  0,  0,  0, 38,  0,  0,  0, 39,  0,
-     0, 40,  0,  0,  0,  2,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0, 41,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 42,  0,
-     0,  0, 43,  0,  0,  0,  0,  0,  0, 44,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 45,  0,  0,  0,  0,  0,
-     0,  0, 46,  0, 17,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0, 43,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0, 47,  0,  0, 48,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 35,  0, 36,  0,  0,  0,
+     0,  0, 37,  0,  0, 19, 38,  0,  0,  0, 39,  0,  0,  0, 40,  0,
+     0, 41,  0,  0,  0,  2,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0, 42,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 43,  0,
+     0,  0, 44,  0,  0,  0,  0,  0,  0, 45,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 46,  0,  0,  0,  0,  0,
+     0,  0, 47,  0, 18,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0, 44,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0, 48,  0,  0, 49,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0, 25,  0,  0,  0, 49,  0, 47, 50,  0,  0,  0,  0,  0,
+     0,  0,  0, 26,  0,  0,  0, 50,  0, 48, 51,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0, 51,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0, 24,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0, 52,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0, 25,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0, 52,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0
+     0,  0,  0,  0, 53,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0
 };
 
 static RE_UINT8 re_sentence_terminal_table_3[] = {
       0,   0,   0,   0,   2,  64,   0, 128,   0,   2,   0,   0,   0,   0,   0, 224,
       0,   0,  16,   0,   7,   0,   0,   0,   0,   0,   0,   2,   0,   0, 128,  98,
      48,   0,   0,   0,   0,  12,   0,   0, 132,   1,   0,   0,   0,  64,   0,   0,
-      0,   0,  96,   0,   8,   2,   0,   0,   0,  15,   0,   0,   0,   0,   0, 204,
-      0,   0,   0,  96,   0,   0,   0,  24,   0,   0,   0, 192,   0,   0,   0,  48,
-    128,   3,   0,   0,   0,  64,   0,  16,   0,   0,  24,   0,   4,   0,   0,   0,
-      0,   0,   0, 128,   0, 192,   0,   0,   0,   0, 136,   0,   0,   0, 192,   0,
-      0, 128,   0,   0,   0,   3,   0,   0,   0,   0,   3,   0,   0,   8,   0,   0,
-      0,   0, 196,   0,   2,   0,   0,   0,   0,   0, 224,   3, 192,   3,   0,   0,
-    128,   1,   0,   0,   3,   0,   0,   0,  14,   0,   0,   0,  96,  32,   0, 192,
-      0,   0,   0,  27,   0,  24,   0,   0,  12, 254, 255,   0,   6,   0,   0,   0,
-      0,   0,   0, 112,  80,   0,   0,   0,  12,   0,   0,   0,   0,   0, 128,   1,
-     24,   0,   0,   0,   0,   0,  32,   0,  16,   0,   0,   0,   0,   0,   0,   1,
-      0,   1,   0,   0
+      0,   0,  96,   0,   0,   0,  48,   0,   8,   2,   0,   0,   0,  15,   0,   0,
+      0,   0,   0, 204,   0,   0,   0,  96,   0,   0,   0,  24,   0,   0,   0, 192,
+      0,   0,   0,  48, 128,   3,   0,   0,   0,  64,   0,  16,   0,   0,  24,   0,
+      4,   0,   0,   0,   0,   0,   0, 128,   0, 192,   0,   0,   0,   0, 136,   0,
+      0,   0, 192,   0,   0, 128,   0,   0,   0,   3,   0,   0,   0,   0,   3,   0,
+      0,   8,   0,   0,   0,   0, 196,   0,   2,   0,   0,   0,   0,   0, 224,   3,
+    192,   3,   0,   0, 128,   1,   0,   0,   3,   0,   0,   0,  14,   0,   0,   0,
+     96,  32,   0, 192,   0,   0,   0,  27,   0,  24,   0,   0,  12, 254, 255,   0,
+      6,   0,   0,   0,   0,   0,   0, 112,  80,   0,   0,   0,  12,   0,   0,   0,
+      0,   0, 128,   1,  24,   0,   0,   0,   0,   0,  32,   0,  16,   0,   0,   0,
+      0,   0,   0,   1,   0,   1,   0,   0
 };
 
 RE_UINT32 re_get_sentence_terminal(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -25935,16 +26656,16 @@
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,  1,
      1,  1,  1,  1,  1,  1,  1,  1,  1,  4,  1,  1,  1,  5,  6,  1,
-     1,  1,  1,  7,  1,  1,  1,  1,  1,  1,  8,  0,  0,  0,  0,  0,
-     1,  1,  1,  1,  9,  1,  1,  1, 10,  0,  0,  0,  0,  0,  0,  0,
+     1,  1,  1,  7,  1,  1,  1,  1,  1,  1,  8,  9,  0,  0,  0,  0,
+     1,  1,  1,  1, 10,  1,  1,  1, 11,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
@@ -26014,22 +26735,24 @@
     5, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 1, 1, 1, 1, 6, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 7,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+    1, 1, 5, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 8, 1, 1, 1, 1, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 9, 0, 0
 };
 
 static RE_UINT8 re_unified_ideograph_table_3[] = {
       0,   0,   0,   0, 255, 255, 255, 255,   0, 192,  26, 128, 154,   3,   0,   0,
-    255, 255, 255,   3, 255, 255, 255,  63,   3,   0, 255, 255,   1,   0,   0,   0,
+    255, 255, 255,   3, 255, 255, 255,  63,   3,   0, 255, 255,   1,   0, 255, 255,
     255,   7, 255, 255, 255, 255,   0,   0
 };
 
 RE_UINT32 re_get_unified_ideograph(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
@@ -26343,16 +27066,16 @@
     20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 10, 30, 13, 31, 10, 10,
     10, 32, 10, 10, 10, 10, 10, 10, 10, 10, 33, 34, 13, 13, 13, 13,
     13, 35, 13, 36, 10, 10, 10, 10, 10, 10, 10, 37, 38, 10, 10, 39,
     10, 10, 10, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 10, 50, 10,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
     13, 13, 13, 13, 13, 13, 13, 13, 13, 51, 13, 13, 13, 52, 53, 13,
-    13, 13, 13, 54, 13, 13, 13, 13, 13, 13, 55, 10, 10, 10, 56, 10,
-    13, 13, 13, 13, 57, 13, 13, 13, 58, 10, 10, 10, 10, 10, 10, 10,
+    13, 13, 13, 54, 13, 13, 13, 13, 13, 13, 55, 56, 10, 10, 57, 10,
+    13, 13, 13, 13, 58, 13, 13, 13, 59, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
@@ -26388,15 +27111,15 @@
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
-    59, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
+    60, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
     10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
@@ -26514,15 +27237,17 @@
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6, 163,   6,   6,   6,   6,   6,   6,
      79,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6, 281,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 179,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 282,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
+      6,   6,  79,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
      79,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,  29,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,  88,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,  88,
@@ -26596,15 +27321,15 @@
     231,  15,   0,   0,   0,  60,   0,   0,  28,   0,   0,   0, 255, 255, 255, 223,
     100, 222, 255, 235, 239, 255, 255, 255, 191, 231, 223, 223, 255, 255, 255, 123,
      95, 252, 253, 255,  63, 255, 255, 255, 253, 255, 255, 247, 255, 127, 255, 255,
     247, 207, 255, 255, 255, 255, 127, 248, 255,  31,  32,   0,  16,   0,   0, 248,
     254, 255,   0,   0, 224,   7,   0,   0, 127, 255, 255, 249, 219,   7, 255, 255,
     255,  31, 255,  63, 255,  67,   0,   0, 127, 111, 255, 127,  31,   0, 127,   0,
     150, 254, 247,  10, 132, 234, 150, 170, 150, 247, 247,  94, 255, 251, 255,  15,
-    238, 251, 255,  15,   3,   0, 255, 255
+    238, 251, 255,  15,   3,   0, 255, 255,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_word(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -26834,25 +27559,25 @@
      0, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0, 14,
      0, 14, 14,  0, 14, 14,  0, 14,  0,  0,  0,  0,  0,  0,  0,  0,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
     15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,  0,  0,  0,  0, 15,
     15, 15, 15, 11, 10,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-    13, 13, 13, 13, 13, 13,  0,  0,  0,  0,  0,  0,  7,  7,  0,  0,
+     9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,  7,  7,  0,  0,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0, 13,  0,  0,  0,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  9,  7,  0, 11, 11,
     14, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
-    11, 11, 11, 11,  0, 11, 14, 14, 14, 14, 14, 14, 14, 13,  0, 14,
+    11, 11, 11, 11,  0, 11, 14, 14, 14, 14, 14, 14, 14,  9,  0, 14,
     14, 14, 14, 14, 14, 11, 11, 14, 14,  0, 14, 14, 14, 14, 11, 11,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9, 11, 11, 11,  0,  0, 11,
-     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 13,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 11,
     11, 14, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,  0, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 11,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
@@ -26865,18 +27590,18 @@
     14, 14, 14, 14, 11, 14, 14, 14, 11, 14, 14, 14, 14, 14,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 14, 14, 14,  0,  0,  0,  0,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,  0,  0,  0,  0,  0,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11,  0, 11, 11, 11, 11, 11, 11,  0,
-    13, 13,  0,  0,  0,  0,  0,  0, 14, 14, 14, 14, 14, 14, 14, 14,
+     9,  9,  0,  0,  0,  0,  0,  0, 14, 14, 14, 14, 14, 14, 14, 14,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
-    14, 14, 13, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
+    14, 14,  9, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 14, 14, 14, 11, 14, 14,
     14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     11, 14, 14, 14, 14, 14, 14, 14, 11, 11, 11, 11, 11, 11, 11, 11,
@@ -27321,16 +28046,16 @@
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14, 14, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
     14, 11, 11, 14, 14, 11,  0,  0,  0,  0,  0,  0,  0,  0,  0, 14,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
-    14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,  0, 13,  0,  0,
-     0,  0, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 13,  0,  0,
+    14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,  0,  0,  9,  0,  0,
+     0,  0, 14,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  9,  0,  0,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
     11, 11, 11, 11, 11, 11, 11, 11, 11,  0,  0,  0,  0,  0,  0,  0,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  0,  0,  0,  0,  0,  0,
     11, 11, 11, 11, 11, 11, 11, 14, 14, 14, 14, 14, 14, 14, 14, 14,
     14, 14, 14, 14, 14,  0,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      0,  0,  0,  0, 11, 14, 14, 11,  0,  0,  0,  0,  0,  0,  0,  0,
     11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
@@ -27728,16 +28453,16 @@
     19, 20, 21, 22, 23, 24, 25, 26, 27, 28,  9, 29, 12, 30,  9,  9,
      9, 31,  9,  9,  9,  9,  9,  9,  9,  9, 32, 33, 12, 12, 12, 12,
     12, 34, 12, 35,  9,  9,  9,  9,  9,  9,  9, 36, 37,  9,  9, 38,
      9,  9,  9, 39, 40, 41, 42, 43, 44, 45, 46, 47,  9,  9, 48,  9,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 49, 12, 12, 12, 50, 51, 12,
-    12, 12, 12, 52, 12, 12, 12, 12, 12, 12, 53,  9,  9,  9, 54,  9,
-    12, 12, 12, 12, 55, 12, 12, 12, 56,  9,  9,  9,  9,  9,  9,  9,
+    12, 12, 12, 52, 12, 12, 12, 12, 12, 12, 53, 54,  9,  9, 55,  9,
+    12, 12, 12, 12, 56, 12, 12, 12, 57,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -27773,15 +28498,15 @@
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
-    57,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
+    58,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -27804,106 +28529,108 @@
       6,   6,  83,   6,  84,  85,  86,   6,  87,   6,  88,  89,  90,   6,   6,  91,
      66,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,  92,   3,   6,   6,  93,  94,  95,  96,  97,   6,   6,  98,  99,
     100,   6,   6, 101,   6,  30,   6, 102, 103, 104, 105, 106,   6, 107, 108,   0,
      29,   6, 103, 109, 110, 111, 112,   0,   6,   6, 113, 114,   6,   6,   6,  96,
       6, 115, 116,  80, 117,  88, 118,  67,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,  91,   6, 119,  80,   6, 120, 121, 122,
-      0, 123, 124, 125, 126,   0, 126, 127, 128, 129, 130,   6, 131,   0,   0,   0,
+    123, 124, 125, 126, 127,   0, 127, 128, 129, 130, 131,   6, 132,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      6,   6,   6,   6,   6,   6,   6, 132,   6,  81,   6, 133, 134, 135, 135,   6,
+      6,   6,   6,   6,   6,   6,   6, 133,   6,  81,   6, 134, 135, 136, 136,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    136, 137,  66,   6, 138,  66,   6,  82, 139,  14,   6,   6, 112,   6,   0,  24,
+    137, 138,  66,   6, 139,  66,   6,   6, 140,  14,   6,   6, 112,   6,   0,  24,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6, 140,   0,  24,  80,   6,   6,   6,   6,   6,   6,   6,   6,
-    141, 142,   6, 143,   6,   6,   6,  26, 144, 145,   6,   6, 146,   6, 147, 148,
-      6, 149,   6,  96,   6,   6, 150, 151,   6, 152,  96,  77,   6,   6, 153, 103,
-      6, 134, 154, 155,   6,   6, 156, 157, 158, 159,  82,  79,   6,   6,   6, 160,
+      6,   6,   6,   6, 141,   0,  24,  80,   6,   6,   6,   6,   6,   6,   6,   6,
+    142, 143,   6, 144,   6,   6,   6,  26, 145, 146,   6,   6, 147,   6, 148, 149,
+      6, 150,   6,  96,   6,   6, 151, 152,   6, 153,  96,  77,   6,   6, 154, 103,
+      6, 135, 155, 156,   6,   6, 157, 158, 159, 160,  82,  79,   6,   6,   6, 161,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 161, 162,  29,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 162, 163,  29,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6, 152,   6,   6, 163,   0, 164, 165, 166,   6,   6,  26, 167,   6,
-      6,   6,  80, 168,   6,   6,   6,   6,   6,  80,  24,   6, 169,   6, 170,   1,
-     90, 171, 172, 173,   6,   6,   6,  77,   1,   2,   3, 105,   6, 103, 174,   0,
-    175, 176, 177,   0,   6,   6,   6,  67,   0,   0,   6,  95,   0,   0,   0, 178,
-      0,   0,   0,   0,  77,   6, 179, 180,   6, 181,  30,  67,  80,   6, 182,   0,
-      6,   6,   6,   6,  80,  79, 183,  29,   6, 184,   6, 185, 186, 187,   0,   0,
-      6,   6,   6,   6,   6,   6,   6,   6,   6, 134, 102, 170, 188, 189,   0,   0,
-    190, 191, 102, 134, 103,   0,   0, 192, 102, 163,   0,   0,   6, 193,   0,   0,
-    194, 195,   0,  77,  77,   0,  74, 196,   6, 102, 102, 197,  26,   0,   0,   0,
-      6,   6, 131,   0,   6, 197,   6, 197,   6, 198,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   6, 199,   0, 200,  77, 201, 179,  24, 202,  24, 203, 134,
-      6,   6, 196, 204,   6,  67, 205, 206,   6, 207, 208, 209,   6,   6, 210,   0,
-    211, 193, 212,   0, 213, 117,   6, 214,  33, 215, 216, 217,   0,   0,   0,   0,
-      6,   6, 218, 212,   6,   6, 219,   0,   0,   0,   0,   0,   6, 220, 221,   0,
-      6,   6, 222,   0,   6, 101,  99,   0,  88, 223, 196,   0,   0,   0,   0,   0,
-      6,  67,   0,   0,   0,   6,   6, 224, 225, 226, 227,   0,   0, 228, 229, 230,
-      6, 103, 201,   6, 231,  24,   6, 101,   0,   0,   0,   0,   0,   0,   0,   0,
-    232,   5, 233, 148, 169, 234,   0,   0, 235, 236, 198, 237, 238,  99,   0,   0,
-      0,   0,   0,   0,   0,   0,   0, 134, 239, 240, 241,   0,   0, 242,   0,   0,
+      6,   6,   6, 153,   6,   6, 164,   0, 165, 166, 167,   6,   6,  26, 168,   6,
+      6,   6,  80, 169,   6,   6,   6,   6,   6,  80,  24,   6, 170,   6, 171,   1,
+     90, 172, 173, 174,   6,   6,   6,  77,   1,   2,   3, 140,   6, 103, 175,   0,
+    176, 177, 178,   0,   6,   6,   6,  67,   0,   0,   6,  95,   0,   0,   0, 179,
+      0,   0,   0,   0,  77,   6, 180, 181,   6, 182,  30,  67,  80,   6, 183,   0,
+      6,   6,   6,   6,  80,  79, 184,  29,   6, 185,   6, 186, 187, 188,   0,   0,
+      6,   6,   6,   6,   6,   6,   6,   6,   6, 135, 102, 171, 189, 190,   0,   0,
+    191, 192, 102, 135, 103,   0,   0, 193, 102, 164,   0,   0,   6, 194,   0,   0,
+    195, 196,   0,  77,  77,   0,  74, 197,   6, 102, 102, 198,  26,   0,   0,   0,
+      6,   6, 132,   0,   6, 198,   6, 198,   6, 199,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   6, 200,   0, 201,  77, 202, 180,  24, 203,  24, 204, 135,
+      6,   6, 197, 205,   6,  67, 206, 207,   6, 208, 209, 210,   6,   6, 211,   0,
+    212, 194, 213,   0, 214, 117,   6, 215,  33, 216, 217, 218,   0,   0,   0,   0,
+      6,   6, 219, 213,   6,   6, 220,   0,   0,   0,   0,   0,   6, 221, 222,   0,
+      6,   6, 223,   0,   6, 101,  99,   0,  88, 224, 197,   0,   0,   0,   0,   0,
+      6,  67,   0,   0,   0,   6,   6, 225, 226, 227, 228,   0,   0, 229, 230, 231,
+      6, 103, 202,   6, 232,  24,   6, 101,   0,   0,   0,   0,   0,   0,   0,   0,
+    233,   5, 234, 149, 170, 235,   0,   0, 236, 237, 199, 238, 239,  99,   0,   0,
+      0,   0,   0,   0,   0,   0,   0, 135, 240, 241, 242,   0,   0, 243,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 163,   0,   0,   0,
-      6,   6,   6, 112,   6,   6,   6,   6,   6,   6, 243,   0,   0,   0,   0,   0,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 164,   0,   0,   0,
+      6,   6,   6, 112,   6,   6,   6,   6,   6,   6, 244,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  24,   6,   6, 179,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  24,   6,   6, 180,
       6,  90, 102,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6, 196,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      6,   6, 197,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6, 101, 103,  79,   6, 103,  79, 106,   6, 134, 227, 244,  90,   0,   0,   0,
+      6, 101, 103,  79,   6, 103,  79, 106,   6, 135, 228, 245,  90,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   6,   6,   0,   0,   0,   0,   6,   6, 245,   6, 246,   0,   0, 247,
+      0,   0,   6,   6,   0,   0,   0,   0,   6,   6, 246,   6, 247,   0,   0, 248,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 115,
-      6,   6,   6,   6,   6,   6, 102,   0, 131,   0,   0,   0,   0,   0,   0,   0,
+      6,   6,   6,   6,   6,   6, 102,   0, 132,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 248,
-      6,   6,   6,   6,   6,   6,   6,   6,   6, 249, 250, 208,   6,   6,   6,   6,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 249,
+      6,   6,   6,   6,   6,   6,   6,   6,   6, 250, 251, 209,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,  29,   0,   0,   0,   0,   0,   0,   0,   0,
-      6,   6,   6, 251, 252,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      6,   6,   6, 252, 253,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   6, 152, 196,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 253, 254, 255,   0,   0,
-      0,   0, 256,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      6,   6, 207,   6, 257, 258, 259,   6, 260, 261, 262,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6, 263, 264,  82, 207, 207, 265, 265, 232, 232, 266,   6,
+      0,   0,   0,   0,   0,   0,   0,   0,   6, 153, 197,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 254, 255, 256,   0,   0,
+      0,   0, 257,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      6,   6, 208,   6, 258, 259, 260,   6, 261, 262, 263,   6,   6,   6,   6,   6,
+      6,   6,   6,   6,   6, 264, 265,  82, 208, 208, 266, 266, 233, 233, 267,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      6, 267,   6, 268, 269, 270,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      6, 268,   6, 269, 270, 271,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0, 103, 271,   0,   0,   0,   0,   0,   0,
-    272, 273,   6,  28, 274,   0,   0,   0,   6, 275, 276,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,  24, 112,   6, 163,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,  24, 163,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 277,
-      6,   6,   6,   6,   6,   6, 278,   0,   6,   6, 223,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0, 103, 272,   0,   0,   0,   0,   0,   0,
+    273, 274,   6,  28, 275,   0,   0,   0,   6, 276, 277,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,  24, 112,   6, 164,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  24, 164,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 278,
+      6,   6,   6,   6,   6,   6, 279,   0,   6,   6, 224,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    259, 279, 280, 281, 282, 283,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    260, 280, 281, 282, 283, 284,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   1,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   0,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6, 163,   6,   6,   6,   6,   6,   6,
+      6,   6,   6,   6,   6,   6,   6,   6,   6, 164,   6,   6,   6,   6,   6,   6,
      80,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6, 284,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
+      6,   6,   6,   6,   6, 285,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
+      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 286,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
-      6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6, 180,
+      6,   6,  80,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
      80,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,  30,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,
       6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,   6,  90,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,  90,
@@ -27937,56 +28664,56 @@
     255, 159, 255, 255, 255, 199, 255,   1, 255, 255,  63, 128, 255, 255,  31,   0,
     255, 255,  15,   0, 255, 223,  13,   0, 255, 255, 143,  48, 255,   3,   0,   0,
       0, 184, 255,   3, 255, 255, 255,   1, 255, 255,  63,   0, 255, 255, 255, 127,
     255,  15, 255,  15, 192, 255, 255, 255, 255,  63,  31,   0, 255,  15, 255, 255,
     255,   3, 255,   7, 255, 255, 255, 159, 255,   3, 255,   3, 128,   0, 255, 191,
     255, 127,   0,   0, 255,  31, 255,   3,   0, 248,  15,   0, 255, 255, 255,   0,
     255, 227, 255, 255, 255,   1, 255, 255,   0,   0, 247, 255,  63,  63, 255, 170,
-    255, 255, 223,  95, 220,  31, 207,  15, 255,  31, 220,  31,   0,   0,   0, 128,
-      1,   0,  16,   0,   0,   0,   2, 128,   0,   0, 255,  31, 226, 255,   1,   0,
-    132, 252,  47,  63,  80, 253, 255, 243, 224,  67,   0,   0, 255,   1,   0,   0,
-     31, 248,  15,   0, 255, 128,   0, 128, 255, 255, 127,   0, 127, 127, 127, 127,
-    224,   0,   0,   0, 254, 255,  62,  31, 255, 255, 127, 230, 224, 255, 255, 255,
-    255,  31,   0,   0, 255,  31, 255, 255, 255,  15,   0,   0, 255, 255, 240, 191,
-      0,   0, 128, 255, 252, 255, 255, 255, 255, 249, 255, 255, 255,   7, 235,   3,
-      0,   0, 252, 255, 255,  16,   0,   0,  63,   0, 255,   3, 255, 255, 255, 232,
-    255,  63, 255, 255,   1, 128, 255,   3, 255,  63, 255,   3, 255, 255, 127, 252,
-      7,   0,   0,  56, 255, 255, 124,   0, 126, 126, 126,   0, 127, 127, 255, 255,
-    255,  55, 255,   3,  15,   0, 255, 255, 127, 248, 255, 255, 255, 255, 255,   3,
-    127,   0, 248, 224, 255, 253, 127,  95, 219, 255, 255, 255,   0,   0, 248, 255,
-    240, 255, 255, 255, 255, 255, 252, 255, 255,   0,   0,   0, 255, 255,  24,   0,
-      0, 224,   0,   0,   0,   0, 138, 170, 252, 252, 252,  28, 255, 239, 255, 255,
-    127, 255, 255, 183, 255,  63, 255,  63,   0,   0,   0,  32, 255, 255,   1,   0,
-      1,   0,   0,   0,   0, 224, 255, 255,  15, 255,  62,   0, 255, 255,  15, 255,
-    255,   0, 255, 255,  15,   0, 255, 247, 255, 247, 183, 255, 251, 255, 251,  27,
-    191, 255, 255, 255, 255, 255, 253,   7,  63, 253, 255, 255, 255, 255, 191, 145,
-    255, 255,  55,   0, 255, 255, 255, 192, 111, 240, 239, 254, 255, 255,  63, 135,
-    127,   0,   0,   0, 255, 255,   7,   0, 255,   0, 255,   3, 255,  27,   3,   0,
-      0,   0,   0, 224, 128,   0, 255, 255,  63,   0,   0,   0,  31,   0,   0,   0,
-    192, 255,  63, 128,   4,   0, 255, 255, 255,   1, 255,   3, 255, 255, 223, 255,
-    240,   0, 255, 255, 255, 255,  79,   0,  31, 222, 255,  23, 255, 255, 251, 255,
-      3,   0,   0,   0, 127, 189, 255, 191, 255,   7, 255,   3, 255, 253, 237, 251,
-    159,  57, 129, 224, 207,  31,  31,   0, 255,   7, 255, 195, 191,   0, 255,   3,
-    255, 255,  63, 255,   1,   0,   0,  63,  17,   0, 255,   3, 255,  15, 255,   3,
-    255,   3,   0, 128, 127, 242, 111, 255, 255, 255, 191, 249,  15,   0, 255,   3,
-    255, 252, 255, 255, 255, 255, 255, 252,  27,   0,   0,   0, 255, 255, 255,  35,
-    255, 253, 255, 255,   1,   0, 255,   3, 255, 254, 127,   0, 127, 251, 255, 255,
-    255, 255, 127, 180, 191, 253, 255, 255, 255, 127, 251,   1, 255, 255, 253, 255,
-    255, 255, 255, 199,   7,   0, 255,   3,   0,   0,   1,   0,  15,   0,   0,   0,
-    248, 255, 255, 224, 255, 135, 255, 255, 255, 128, 255, 255,  27,   0,   3,   0,
-      0,   0, 239, 111,   7,   0,   4,   0,   0,   0,  39,   0, 255,   7, 255,  31,
-    255,   1, 255,  99, 224, 227,   7, 248, 231,  15,   0,   0,   0,  60,   0,   0,
-     28,   0,   0,   0, 255, 255, 255, 223, 100, 222, 255, 235, 239, 255, 255, 255,
-    191, 231, 223, 223, 255, 255, 255, 123,  95, 252, 253, 255,  63, 255, 255, 255,
-    253, 255, 255, 247, 255, 127, 255, 255, 247, 207, 255, 255, 255, 255, 127, 248,
-    255,  31,  32,   0,  16,   0,   0, 248, 254, 255,   0,   0, 224,   7,   0,   0,
-    127, 255, 255, 249, 219,   7, 255, 255,   0, 128,   0,   0, 255,  31, 255,  63,
-    255,  67,   0,   0, 127, 111, 255, 127,  31,   0, 127,   0, 150, 254, 247,  10,
-    132, 234, 150, 170, 150, 247, 247,  94, 255, 251, 255,  15, 238, 251, 255,  15,
-      3,   0, 255, 255
+    255, 255, 223,  95, 220,  31, 207,  15, 255,  31, 220,  31,   0,  48,   0,   0,
+      0,   0,   0, 128,   1,   0,  16,   0,   0,   0,   2, 128,   0,   0, 255,  31,
+    226, 255,   1,   0, 132, 252,  47,  63,  80, 253, 255, 243, 224,  67,   0,   0,
+    255,   1,   0,   0,  31, 248,  15,   0, 255, 128,   0, 128, 255, 255, 127,   0,
+    127, 127, 127, 127, 224,   0,   0,   0, 254, 255,  62,  31, 255, 255, 127, 230,
+    224, 255, 255, 255, 255,  31,   0,   0, 255,  31, 255, 255, 255,  15,   0,   0,
+    255, 255, 240, 191,   0,   0, 128, 255, 252, 255, 255, 255, 255, 249, 255, 255,
+    255,   7, 235,   3,   0,   0, 252, 255, 255,  16,   0,   0,  63,   0, 255,   3,
+    255, 255, 255, 232, 255,  63, 255, 255,   1, 128, 255,   3, 255,  63, 255,   3,
+    255, 255, 127, 252,   7,   0,   0,  56, 255, 255, 124,   0, 126, 126, 126,   0,
+    127, 127, 255, 255, 255,  55, 255,   3,  15,   0, 255, 255, 127, 248, 255, 255,
+    255, 255, 255,   3, 127,   0, 248, 224, 255, 253, 127,  95, 219, 255, 255, 255,
+      0,   0, 248, 255, 240, 255, 255, 255, 255, 255, 252, 255, 255,   0,   0,   0,
+    255, 255,  24,   0,   0, 224,   0,   0,   0,   0, 138, 170, 252, 252, 252,  28,
+    255, 239, 255, 255, 127, 255, 255, 183, 255,  63, 255,  63,   0,   0,   0,  32,
+    255, 255,   1,   0,   1,   0,   0,   0,   0, 224, 255, 255,  15, 255,  62,   0,
+    255, 255,  15, 255, 255,   0, 255, 255,  15,   0, 255, 247, 255, 247, 183, 255,
+    251, 255, 251,  27, 191, 255, 255, 255, 255, 255, 253,   7,  63, 253, 255, 255,
+    255, 255, 191, 145, 255, 255,  55,   0, 255, 255, 255, 192, 111, 240, 239, 254,
+    255, 255,  63, 135, 127,   0,   0,   0, 255, 255,   7,   0, 255,   0, 255,   3,
+    255,  27,   3,   0,   0,   0,   0, 224, 128,   0, 255, 255,  63,   0,   0,   0,
+     31,   0,   0,   0, 192, 255,  63, 128,   4,   0, 255, 255, 255,   1, 255,   3,
+    255, 255, 223, 255, 240,   0, 255, 255, 255, 255,  79,   0,  31, 222, 255,  23,
+    255, 255, 251, 255,   3,   0,   0,   0, 127, 189, 255, 191, 255,   7, 255,   3,
+    255, 253, 237, 251, 159,  57, 129, 224, 207,  31,  31,   0, 255,   7, 255, 195,
+    191,   0, 255,   3, 255, 255,  63, 255,   1,   0,   0,  63,  17,   0, 255,   3,
+    255,  15, 255,   3, 255,   3,   0, 128, 127, 242, 111, 255, 255, 255, 191, 249,
+     15,   0, 255,   3, 255, 252, 255, 255, 255, 255, 255, 252,  27,   0,   0,   0,
+    255, 255, 255,  35, 255, 253, 255, 255,   1,   0, 255,   3, 255, 254, 127,   0,
+    127, 251, 255, 255, 255, 255, 127, 180, 191, 253, 255, 255, 255, 127, 251,   1,
+    255, 255, 253, 255, 255, 255, 255, 199,   7,   0, 255,   3,   0,   0,   1,   0,
+     15,   0,   0,   0, 248, 255, 255, 224, 255, 135, 255, 255, 255, 128, 255, 255,
+     27,   0,   3,   0,   0,   0, 239, 111,   7,   0,   4,   0,   0,   0,  39,   0,
+    255,   7, 255,  31, 255,   1, 255,  99, 224, 227,   7, 248, 231,  15,   0,   0,
+      0,  60,   0,   0,  28,   0,   0,   0, 255, 255, 255, 223, 100, 222, 255, 235,
+    239, 255, 255, 255, 191, 231, 223, 223, 255, 255, 255, 123,  95, 252, 253, 255,
+     63, 255, 255, 255, 253, 255, 255, 247, 255, 127, 255, 255, 247, 207, 255, 255,
+    255, 255, 127, 248, 255,  31,  32,   0,  16,   0,   0, 248, 254, 255,   0,   0,
+    224,   7,   0,   0, 127, 255, 255, 249, 219,   7, 255, 255,   0, 128,   0,   0,
+    255,  31, 255,  63, 255,  67,   0,   0, 127, 111, 255, 127,  31,   0, 127,   0,
+    150, 254, 247,  10, 132, 234, 150, 170, 150, 247, 247,  94, 255, 251, 255,  15,
+    238, 251, 255,  15,   3,   0, 255, 255,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_xid_continue(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -28013,16 +28740,16 @@
     19, 20, 21, 22, 23, 24, 25, 26, 27, 28,  9, 29, 12, 30,  9,  9,
      9, 31,  9,  9,  9,  9,  9,  9,  9,  9, 32, 33, 12, 12, 12, 12,
     12, 34, 12, 35,  9,  9,  9,  9,  9,  9,  9, 36, 37,  9,  9, 38,
      9,  9,  9,  9,  9, 39,  9, 40, 41, 42, 43, 44,  9,  9,  9,  9,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
     12, 12, 12, 12, 12, 12, 12, 12, 12, 45, 12, 12, 12, 46, 47, 12,
-    12, 12, 12, 48, 12, 12, 12, 12, 12, 12, 49,  9,  9,  9, 50,  9,
-    12, 12, 12, 12, 51, 12, 12, 12, 52,  9,  9,  9,  9,  9,  9,  9,
+    12, 12, 12, 48, 12, 12, 12, 12, 12, 12, 49, 50,  9,  9, 51,  9,
+    12, 12, 12, 12, 52, 12, 12, 12, 53,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
      9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,  9,
@@ -28172,15 +28899,17 @@
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4, 161,   4,   4,   4,   4,   4,   4,
     113,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4, 254,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
-      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  74,
+      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4, 255,
+      4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
+      4,   4, 113,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
     113,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  30,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,
       4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,   4,  22,   0,   0
 };
@@ -28245,15 +28974,15 @@
     255,  63,   0,   0, 248, 255, 255, 224, 255,   7,   1,   0,  11,   0,   0,   0,
       0,   0, 239, 111,   7,   0,   4,   0,   0,   0,  39,   0, 240,   0, 255, 255,
     255,   7, 255,  31, 255,   1, 255,   3, 255, 255, 223, 255, 255, 255, 255, 223,
     100, 222, 255, 235, 239, 255, 255, 255, 191, 231, 223, 223, 255, 255, 255, 123,
      95, 252, 253, 255,  63, 255, 255, 255, 253, 255, 255, 247, 255, 127, 255, 255,
     224,   7,   0,   0, 255,  31, 128,  63,   0,  64,   0,   0, 127, 111, 255, 127,
      15,   8,   0,   0, 150, 254, 247,  10, 132, 234, 150, 170, 150, 247, 247,  94,
-    255, 251, 255,  15, 238, 251, 255,  15,   3,   0, 255, 255
+    255, 251, 255,  15, 238, 251, 255,  15,   3,   0, 255, 255,   1,   0, 255, 255
 };
 
 RE_UINT32 re_get_xid_start(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 offset;
@@ -28272,19 +29001,19 @@
 }
 
 /* All cases. */
 static RE_UINT8 re_all_cases_table_1[] = {
      0,  1,  2,  2,  3,  2,  2,  4,  5,  6,  2,  7,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  8,  9,  2,  2,  2,  2,  2,
-     2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 10,
-     2, 11,  2, 12,  2,  2, 13,  2,  2,  2,  2,  2,  2,  2,  2,  2,
-     2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 14,  2,  2,  2,  2,
+     2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 10, 11,
+     2, 12,  2, 13,  2,  2, 14,  2,  2,  2,  2,  2,  2,  2,  2,  2,
+     2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 15,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
-     2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 15,  2,  2,  2,  2,  2,
+     2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 16,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
@@ -28361,76 +29090,78 @@
     59, 60, 61, 62,  6,  6,  6, 63, 34, 64,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0, 65, 66, 67,  0,  0,  0,  0, 68,  6, 69, 70, 71, 72, 73,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 74, 75, 76, 77,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0, 78, 78,  0,  0,  0,  0,  0,
-    79, 80, 81,  0,  0, 82, 83, 84,  0,  0,  0, 85, 86, 87,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0, 78,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0, 88, 89, 88, 89,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0, 79, 79,  0,  0,  0,  0,  0,
+    80, 81, 82,  0,  0, 83, 84, 85,  0,  0,  0, 86, 87, 88,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0, 90, 90,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0, 89, 90, 89, 90,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0, 91, 91,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0, 91, 91,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0, 92, 93, 94,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0, 92, 92,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0, 93, 94, 95,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0
 };
 
 static RE_UINT8 re_all_cases_table_3[] = {
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   1,   1,   1,   1,   1,   1,   1,   1, 147,   1,   3,   1,   1,   1,   1,
+      0,   1,   1,   1,   1,   1,   1,   1,   1, 149,   1,   3,   1,   1,   1,   1,
       1,   1,   1,   4,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,   0,   0,
       0,   1,   1,   1,   1,   1,   1,   1,   1,   2,   1,   3,   1,   1,   1,   1,
       1,   1,   1,   4,   1,   1,   1,   1,   1,   1,   1,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0, 158,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0, 160,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   1,   1,   1,   1,   5,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   0,   1,   1,   1,   1,   1,   1,   1,  83,
       1,   1,   1,   1,   1,   5,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   0,   1,   1,   1,   1,   1,   1,   1,  29,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-    146,  15,  16,  16,  16,  16,  16,  16,   0,  23,  23,  25,  25,  23,  23,  27,
+    148,  15,  16,  16,  16,  16,  16,  16,   0,  23,  23,  25,  25,  23,  23,  27,
      27,  23,  23,  25,  25,  23,  23,  28,  28,   0,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-     16,  16,  16,  16,  16,  16,  16,  16,  29,  23,  23,  25,  25,  23,  23, 149,
+     16,  16,  16,  16,  16,  16,  16,  16,  29,  23,  23,  25,  25,  23,  23, 151,
      53,  30,  16,  16,  16,  16,  30,  28,  28,  31,  32,  25,  25,   0,  33,  34,
      35,  23,  23,  36,  37,  47,  38,  38,  16,  16,  51,   0,  36,  39,  49,  40,
      16,  16,  16,  16,  16,  16,  41,  28,  28,  42,   0,   0,  16,  16,  41,  43,
      43,  44,  45,  25,  25,  23,  23,  46,  16,  16,   0,   0,  16,  16,   0,  48,
-      0,   0,   0,   0, 168, 168,  24, 162, 162,  17, 169, 169,  26,  23,  23,  43,
+      0,   0,   0,   0, 170, 170,  24, 164, 164,  17, 171, 171,  26,  23,  23,  43,
      43,  23,  23,  25,  25,  23,  23,  28,  28,  23,  23,  25,  25,  33,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-      0, 163, 163,  18,  16,  16,  47,  48,  16,  16,  16,  16,  16,  16,  16,  16,
+      0, 165, 165,  18,  16,  16,  47,  48,  16,  16,  16,  16,  16,  16,  16,  16,
      49,   0,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-     16,  16,  16,  16,   0,   0,   0,   0,   0,   0,  50,  25,  25,  51,  52, 108,
-    106,  23,  23,  53,  54,  55,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-    106, 104, 107,  30,  30,   0,  31,  32,   0,  34,   0,  35, 112,   0,   0,   0,
-     36, 113,   0,  37,   0, 110, 111,   0,  38,  38, 115, 101, 114,   0,   0,  36,
-      0, 105,  39,   0,   0,  40,   0,   0,   0,   0,   0,   0,   0, 103,   0,   0,
-     41,   0, 120,  42,   0,   0,   0, 117,  41,  54,  44,  45,  55,   0,   0,   0,
-      0,   0,  46,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 118, 116,   0,
-      0,   0,   0,   0,   0, 155,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+     16,  16,  16,  16,   0,   0,   0,   0,   0,   0,  50,  25,  25,  51,  52, 110,
+    108,  23,  23,  53,  54,  55,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
+    108, 106, 109,  30,  30,   0,  31,  32,   0,  34,   0,  35, 114,   0,   0,   0,
+     36, 115,   0,  37,   0, 112, 113,   0,  38,  38, 117, 103, 116,   0,   0,  36,
+      0, 107,  39,   0,   0,  40,   0,   0,   0,   0,   0,   0,   0, 105,   0,   0,
+     41,   0, 122,  42,   0,   0,   0, 119,  41,  54,  44,  45,  55,   0,   0,   0,
+      0,   0,  46,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 120, 118,   0,
+      0,   0,   0,   0,   0, 157,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      16,  16,  16,  16,   0,   0,  16,  16,   0,   0,   0,  75,  76,  76,   0,  56,
       0,   0,   0,   0,   0,   0,  57,   0,  58,  59,  58,   0,  60,   0,  61,  62,
-      0,   1,   6,   1,   1,   7,   1,   1,   8, 155,  10,   1, 158,   1,   1,   1,
-     63,  64,   0, 164,  65,  65,  66,  65,  65,  67,  65,  65,  57,  58,  59,  58,
-      0,   1,   6,   1,   1,   7,   1,   1,   8,   9,  10,   1,  11,   1,   1,   1,
-     63,  64, 164,  19,  65,  65,  66,  65,  65,  67,  65,  65,  60,  61,  62,  71,
-    151, 153,   0,   0,   0, 172, 170,  71,  16,  16,  16,  16,  16,  16,  16,  16,
+     87,   1,   6,   1,   1,   7,   1,   1,   8, 157,  10,   1, 160,   1,   1,   1,
+     63,  64,   0, 166,  65,  65,  66,  65,  65,  67,  65,  65,  57,  58,  59,  58,
+     89,   1,   6,   1,   1,   7,   1,   1,   8,   9,  10,   1,  11,   1,   1,   1,
+     63,  64, 166,  19,  65,  65,  66,  65,  65,  67,  65,  65,  60,  61,  62,  71,
+    153, 155,   0,   0,   0, 174, 172,  71,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-    157, 171,  74,  56, 154, 152,   0,  28,  28,  74,  16,  16,   0,  75,  76,  76,
+    159, 173,  74,  56, 156, 154,   0,  28,  28,  74,  16,  16,   0,  75,  76,  76,
      77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,
       1,   1,  12,   1,  13,   1,   1,   1,   1,   1,   1,   1,   1,   1,  14,   1,
      65,  68,  69,  65,  65,  65,  65,  65,  65,  65,  70,  65,  65,  65,  65,  65,
       1,   1,  12,   1,  13,   1,   1,   1,   1,   1,   1,   1,   1,   1,  14,   1,
      65,  68,  69,  65,  65,  65,  65,  65,  65,  65,  70,  65,  65,  65,  65,  65,
      77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,
      16,  16,  20,  20,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
@@ -28449,129 +29180,131 @@
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,
      79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,  79,
      80,  80,  80,  80,  80,  80,   0,  80,   0,   0,   0,   0,   0,  80,   0,   0,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,   0,   0,  82,  82,  82,
-    122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122,
-    123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123,
     124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124,
     125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125,
-    124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124,
+    126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126,
+    127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127,
+    126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126,
      81,  81,  81,  81,  81,  81,   0,   0,  81,  81,  81,  81,  81,  81,   0,   0,
-    159, 160, 161, 174, 175, 176, 177, 165, 167,   0,   0,   0,   0,   0,   0,   0,
+    161, 162, 163, 176, 177, 178, 179, 167, 169,   0,   0,   0,   0,   0,   0,   0,
      82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,  82,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0, 109,   0,   0,   0, 102,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 121,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0, 111,   0,   0,   0, 104,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0, 123,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      21,  21,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-     16,  16,  16,  16,  16,  16,   0,   0,   0,   0,   0, 166,   0,   0,  83,   0,
+     16,  16,  16,  16,  16,  16,   0,   0,   0,   0,   0, 168,   0,   0,  83,   0,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,   0,   0,  81,  81,  81,  81,  81,  81,   0,   0,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
      81,  81,  81,  81,  81,  81,   0,   0,  81,  81,  81,  81,  81,  81,   0,   0,
       0,  81,   0,  81,   0,  81,   0,  81,   0,  81,   0,  81,   0,  81,   0,  81,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     84,  84,  85,  85,  86,  86,  87,  87,  90,  90,  88,  88,  75,  75,   0,   0,
+     84,  84,  85,  85,  86,  86,  88,  88,  92,  92,  90,  90,  75,  75,   0,   0,
      81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,  81,
-     81,  81,   0,  28,   0,   0,   0,   0,  81,  81,  84,  84,  28,   0, 156,   0,
+     81,  81,   0,  28,   0,   0,   0,   0,  81,  81,  84,  84,  28,   0, 158,   0,
       0,   0,   0,  28,   0,   0,   0,   0,  85,  85,  86,  86,  28,   0,   0,   0,
-     81,  81,   0,   0,   0,   0,   0,   0,  81,  81,  87,  87,   0,   0,   0,   0,
-     81,  81,   0,   0,   0,  89,   0,   0,  81,  81,  88,  88,  89,   0,   0,   0,
-      0,   0,   0,  28,   0,   0,   0,   0,  90,  90,  75,  75,  28,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 173,   0,   0,   0, 148, 150,   0,   0,   0,   0,
-      0,   0,  91,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  91,   0,
+     81,  81,   0,  87,   0,   0,   0,   0,  81,  81,  88,  88,   0,   0,   0,   0,
+     81,  81,   0,  89,   0,  91,   0,   0,  81,  81,  90,  90,  91,   0,   0,   0,
+      0,   0,   0,  28,   0,   0,   0,   0,  92,  92,  75,  75,  28,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 175,   0,   0,   0, 150, 152,   0,   0,   0,   0,
+      0,   0,  93,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,  93,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-     92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,
-     92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,  92,
+     94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,
+     94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,  94,
       0,   0,   0,  25,  25,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,  93,  93,  94,  94,  95,  95,  94,  94,  93,  93,
-     96,  96,  97,  97,  96,  96,  98,  98,  57,  57,  99,  99,  57,  57,  98,  98,
-     93,  93,  94,  94,  95,  95,  94,  94,  93,  93,  96,  96,  97,  97,  96,  96,
-     98,  98,  57,  57,  99,  99,  57,  57,  98,  98,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,  95,  95,  96,  96,  97,  97,  96,  96,  95,  95,
+     98,  98,  99,  99,  98,  98, 100, 100,  57,  57, 101, 101,  57,  57, 100, 100,
+     95,  95,  96,  96,  97,  97,  96,  96,  95,  95,  98,  98,  99,  99,  98,  98,
+    100, 100,  57,  57, 101, 101,  57,  57, 100, 100,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,
      77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,
-    100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
+    102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102,
      73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,  73,
      77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,  77,
-    100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
-     16,  16, 101, 102, 103,  50,  52,  28,  28,  23,  23,  25,  25, 104, 105, 106,
-    107,   0,  16,  16,   0,  23,  23,   0,   0,   0,   0,   0,   0,   0, 108, 106,
+    102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102, 102,
+     16,  16, 103, 104, 105,  50,  52,  28,  28,  23,  23,  25,  25, 106, 107, 108,
+    109,   0,  16,  16,   0,  23,  23,   0,   0,   0,   0,   0,   0,   0, 110, 108,
      16,  16,  16,  16,   0,   0,   0,   0,   0,   0,   0,  25,  25,  23,  23,   0,
       0,   0,  16,  16,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      80,  80,  80,  80,  80,  80,   0,  80,   0,   0,   0,   0,   0,  80,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-     16,  16,  16,  16,  16,  16,  16,  16,  16,  16, 167,  22,  16,  16,  16,  16,
+     16,  16,  16,  16,  16,  16,  16,  16,  16,  16, 169,  22,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,   0,   0,   0,   0,
       0,   0,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
       0,   0,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
      16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,  23,  23,  25,  25, 109,  16,  16,
-     16,  16,  16,  16,  16,  16,  16,  16,   0,   0,   0,  25,  25, 110,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,  23,  23,  25,  25, 111,  16,  16,
+     16,  16,  16,  16,  16,  16,  16,  16,   0,   0,   0,  25,  25, 112,   0,   0,
      16,  16,  16,  16,  77,   0,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-     16,  16,  16,  16,  16,  16,  16,  16,  16,  16, 111, 112, 113, 114, 115,   0,
-    116, 117, 118, 119,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
-     16,  16,  16,  16,  77, 120, 121,  28,  28,  23,  23,   0,   0,   0,   0,   0,
+     16,  16,  16,  16,  16,  16,  16,  16,  16,  16, 113, 114, 115, 116, 117,   0,
+    118, 119, 120, 121,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,  16,
+     16,  16,  16,  16,  77, 122, 123,  28,  28,  23,  23,   0,   0,   0,   0,   0,
      16,  16,   0,   0,   0,   0,  16,  16,  16,  16,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,  23,  23,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      0,   0,   0, 119,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0, 121,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122, 122,
-    123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123, 123,
     124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124,
     125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125,
-    124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124, 124,
+    126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126,
+    127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127,
+    126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126, 126,
+      0,   0,   0,   0,   0,  23,  23,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,
      65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,   0,   0,   0,   0,   0,
-    126, 126, 126, 126, 126, 126, 126, 126, 127, 127, 127, 127, 127, 127, 127, 127,
-    126, 126, 126, 126, 126, 126, 126, 126, 128, 128, 128, 128, 128, 128, 128, 128,
-    129, 129, 129, 129, 129, 129, 129, 129, 126, 126, 126, 126, 126, 126, 126, 126,
-    127, 127, 127, 127, 127, 127, 127, 127, 126, 126, 126, 126, 126, 126, 126, 126,
     128, 128, 128, 128, 128, 128, 128, 128, 129, 129, 129, 129, 129, 129, 129, 129,
+    128, 128, 128, 128, 128, 128, 128, 128, 130, 130, 130, 130, 130, 130, 130, 130,
+    131, 131, 131, 131, 131, 131, 131, 131, 128, 128, 128, 128, 128, 128, 128, 128,
+    129, 129, 129, 129, 129, 129, 129, 129, 128, 128, 128, 128, 128, 128, 128, 128,
+    130, 130, 130, 130, 130, 130, 130, 130, 131, 131, 131, 131, 131, 131, 131, 131,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    129, 129, 129, 129, 129, 129, 129, 129, 128, 128, 128, 128, 128, 128, 128, 128,
-    126, 126, 126, 126, 126, 126, 126, 126, 127, 127, 127, 127, 127, 127, 127, 127,
-    126, 126, 126, 126,   0,   0,   0,   0, 129, 129, 129, 129, 129, 129, 129, 129,
-    128, 128, 128, 128, 128, 128, 128, 128, 126, 126, 126, 126, 126, 126, 126, 126,
-    127, 127, 127, 127, 127, 127, 127, 127, 126, 126, 126, 126,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    130, 131, 132, 131, 133, 131, 132, 131, 130, 134, 135,   0, 136, 134, 135, 134,
-     59, 137, 138, 137, 139, 137, 138, 137,  59, 140, 141,   0, 142, 140, 141, 140,
-     59, 137, 138,   0, 139, 137,   0, 130, 131, 132, 131, 133, 131, 132, 131, 130,
-    134, 135,   0, 136, 134, 135, 134,  59, 137, 138, 137, 139, 137, 138, 137,  59,
-    140, 141,   0, 142, 140, 141, 140,  59, 137, 138,   0, 139, 137,   0,   0,   0,
+    131, 131, 131, 131, 131, 131, 131, 131, 130, 130, 130, 130, 130, 130, 130, 130,
+    128, 128, 128, 128, 128, 128, 128, 128, 129, 129, 129, 129, 129, 129, 129, 129,
+    128, 128, 128, 128,   0,   0,   0,   0, 131, 131, 131, 131, 131, 131, 131, 131,
+    130, 130, 130, 130, 130, 130, 130, 130, 128, 128, 128, 128, 128, 128, 128, 128,
+    129, 129, 129, 129, 129, 129, 129, 129, 128, 128, 128, 128,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    132, 133, 134, 133, 135, 133, 134, 133, 132, 136, 137,   0, 138, 136, 137, 136,
+     59, 139, 140, 139, 141, 139, 140, 139,  59, 142, 143,   0, 144, 142, 143, 142,
+     59, 139, 140,   0, 141, 139,   0, 132, 133, 134, 133, 135, 133, 134, 133, 132,
+    136, 137,   0, 138, 136, 137, 136,  59, 139, 140, 139, 141, 139, 140, 139,  59,
+    142, 143,   0, 144, 142, 143, 142,  59, 139, 140,   0, 141, 139,   0,   0,   0,
      60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,
      60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,
      60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,  60,
      60,  60,  60,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,
      65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,  65,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
       1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
-    143, 143,  98,  98, 143, 143,  99,  99, 143, 143,  98,  98, 143, 143, 144, 144,
-    143, 143,  98,  98, 143, 143,  99,  99, 143, 143,  98,  98, 143, 143, 145, 145,
-     72,  72, 143, 143,  98,  98, 143, 143,  99,  99, 143, 143,  98,  98, 143, 143,
-    144, 144, 143, 143,  98,  98, 143, 143,  99,  99, 143, 143,  98,  98, 143, 143,
-    145, 145,  72,  72,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+    145, 145, 100, 100, 145, 145, 101, 101, 145, 145, 100, 100, 145, 145, 146, 146,
+    145, 145, 100, 100, 145, 145, 101, 101, 145, 145, 100, 100, 145, 145, 147, 147,
+     72,  72, 145, 145, 100, 100, 145, 145, 101, 101, 145, 145, 100, 100, 145, 145,
+    146, 146, 145, 145, 100, 100, 145, 145, 101, 101, 145, 145, 100, 100, 145, 145,
+    147, 147,  72,  72,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0
 };
 
 static RE_AllCases re_all_cases_table_4[] = {
     {    0, {    0,     0}},
     {   32, {    0,     0}},
     {   32, {  304,     0}},
@@ -28655,15 +29388,17 @@
     {15840, {    0,     0}},
     {    8, {    0,     0}},
     { 3136, {    0,     0}},
     { 7745, {    0,     0}},
     {  202, {    0,     0}},
     {  186, {    0,     0}},
     {  190, {    0,     0}},
+    { 7235, {    0,     0}},
     {  172, {    0,     0}},
+    { 7251, {    0,     0}},
     {  144, {    0,     0}},
     {    9, {    0,     0}},
     {  128, {    0,     0}},
     {  124, {    0,     0}},
     {   16, {    0,     0}},
     {  102, {    0,     0}},
     {  106, {    0,     0}},
@@ -28787,19 +29522,19 @@
 }
 
 /* Simple case folding. */
 static RE_UINT8 re_simple_folding_table_1[] = {
      0,  1,  2,  2,  3,  2,  2,  4,  5,  6,  2,  7,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  8,  9,  2,  2,  2,  2,  2,
-     2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 10,
-     2, 11,  2, 12,  2,  2, 13,  2,  2,  2,  2,  2,  2,  2,  2,  2,
-     2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 14,  2,  2,  2,  2,
+     2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 10, 11,
+     2, 12,  2, 13,  2,  2, 14,  2,  2,  2,  2,  2,  2,  2,  2,  2,
+     2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 15,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
-     2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 15,  2,  2,  2,  2,  2,
+     2,  2,  2,  2,  2,  2,  2,  2,  2,  2, 16,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
      2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,  2,
@@ -28876,24 +29611,26 @@
     44, 45,  0, 46,  4,  4,  4, 47,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  4, 48, 49,  0,  0,  0,  0, 50,  4, 51, 52, 53, 54, 55,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, 56, 57, 58,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0,  0, 59,  0,  0,  0,  0,  0,  0,
-    60, 61,  0,  0,  0, 62, 63,  0,  0,  0,  0, 64, 65,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0, 59,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0,  0, 60,  0,  0,  0,  0,  0,  0,
+    61, 62,  0,  0,  0, 63, 64,  0,  0,  0,  0, 65, 66,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0, 66, 67,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0, 67, 68,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0, 68,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0, 69,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0, 69,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
-     0,  0,  0,  0,  0,  0,  0,  0, 70, 71,  0,  0,  0,  0,  0,  0,
+     0,  0, 70,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,
+     0,  0,  0,  0,  0,  0,  0,  0, 71, 72,  0,  0,  0,  0,  0,  0,
      0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0
 };
 
 static RE_UINT8 re_simple_folding_table_3[] = {
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,  18,  18,  18,  18,  18,  18,  18,  18,  79,  18,  18,  18,  18,  18,  18,
@@ -28915,15 +29652,15 @@
       1,   0,   1,   0,   1,   0,  83,  10,   0,  84,   0,   0,   1,   0,  83,  17,
       0,  86,  85,   5,   0,   3,   0,  82,   1,   0,   0,   0,   1,   0,   0,   0,
       0,   0,   0,   0,   2,   3,   0,   9,   1,   0,   4,   5,   0,   3,   0,  17,
       0,   3,   0,   5,   0,   3,   0,  10,   0,   3,   0,   5,   0,   0,   1,   0,
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
       0,   2,   1,   0,   1,   0,  47,  38,   1,   0,   1,   0,   1,   0,   1,   0,
      88,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
-      1,   0,   1,   0,   0,   0,   0,   0,   0,   0, 123,   5,   0,  87, 122,   0,
+      1,   0,   1,   0,   0,   0,   0,   0,   0,   0, 125,   5,   0,  87, 124,   0,
       0,   3,   0,  89,  66,  64,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,  76,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   0,   1,   0,   0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,  59,
       0,   0,   0,   0,   0,   0,  25,   0,  20,  22,  20,   0,  35,   0,  37,  36,
@@ -28942,80 +29679,82 @@
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
      10,   3,   0,   5,   0,   3,   0,  10,   0,   3,   0,   5,   0,   3,   0,   0,
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
       0,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,
      29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,
      67,  67,  67,  67,  67,  67,  67,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125,
-    125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125, 125,
-    126, 126, 126, 126, 126, 126,   0, 126,   0,   0,   0,   0,   0, 126,   0,   0,
+    127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127,
+    127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127, 127,
+    128, 128, 128, 128, 128, 128,   0, 128,   0,   0,   0,   0,   0, 128,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   0,   0,
-    102, 103, 104, 105, 106, 107, 108, 109, 143,   0,   0,   0,   0,   0,   0,   0,
+    102, 103, 104, 105, 106, 107, 108, 109, 145,   0,   0,   0,   0,   0,   0,   0,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,
     100, 100, 100, 100, 100, 100, 100, 100, 100, 100, 100,   0,   0, 100, 100, 100,
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
-      1,   0,   1,   0,   1,   0,   0,   0,   0,   0,   0,  75,   0,   0, 111,   0,
+      1,   0,   1,   0,   1,   0,   0,   0,   0,   0,   0,  75,   0,   0, 113,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   6,   0,   6,   0,   6,   0,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,   6,   6,   6,   6,   6,   6,
       0,   0,   0,   0,   0,   0,   0,   0,   6,   6,  65,  65,  10,   0, 110,   0,
       0,   0,   0,   0,   0,   0,   0,   0,  62,  62,  63,  63,  10,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   6,   6,  61,  61,   0,   0,   0,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   6,   6,  60,  60,   7,   0,   0,   0,
+      0,   0,   0, 111,   0,   0,   0,   0,   6,   6,  61,  61,   0,   0,   0,   0,
+      0,   0,   0, 112,   0,   0,   0,   0,   6,   6,  60,  60,   7,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,  56,  56,  58,  58,  10,   0,   0,   0,
-      0,   0,   0,   0,   0,   0, 114,   0,   0,   0, 112, 113,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0, 116,   0,   0,   0, 114, 115,   0,   0,   0,   0,
       0,   0,  54,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      11,  11,  11,  11,  11,  11,  11,  11,  11,  11,  11,  11,  11,  11,  11,  11,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   5,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,  48,  48,  51,  51,  52,  52,  51,  51,  48,  48,
      15,  15,  16,  16,  15,  15,  21,  21,  25,  25,  27,  27,  25,  25,  21,  21,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
      29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,  29,
      41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,  41,
      53,  53,  53,  53,  53,  53,  53,  53,  53,  53,  53,  53,  53,  53,  53,  53,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-      1,   0, 115, 124, 116,   0,   0,  10,   0,   3,   0,   5,   0, 119, 117, 120,
-    118,   0,   1,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0, 121, 120,
+      1,   0, 117, 126, 118,   0,   0,  10,   0,   3,   0,   5,   0, 121, 119, 122,
+    120,   0,   1,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0, 123, 122,
       1,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   5,   0,   3,   0,   0,
       0,   0,   1,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   0,   0,   0,   0,
       0,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
       0,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
       1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
-      0,   0,   0,   0,   0,   0,   0,   0,   0,   3,   0,   5,   0, 141,   1,   0,
-      1,   0,   1,   0,   1,   0,   1,   0,   0,   0,   0,   5,   0, 135,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   3,   0,   5,   0, 143,   1,   0,
+      1,   0,   1,   0,   1,   0,   1,   0,   0,   0,   0,   5,   0, 137,   0,   0,
       1,   0,   1,   0,   0,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
-      1,   0,   1,   0,   1,   0,   1,   0,   1,   0, 133, 136, 134, 131, 132,   0,
-    127, 129, 128, 101,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
-      1,   0,   1,   0,  41, 130, 142,  10,   0,   3,   0,   0,   0,   0,   0,   0,
+      1,   0,   1,   0,   1,   0,   1,   0,   1,   0, 135, 138, 136, 133, 134,   0,
+    129, 131, 130, 101,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,   1,   0,
+      1,   0,   1,   0,  41, 132, 144,  10,   0,   3,   0,   0,   0,   0,   0,   0,
       1,   0,   0,   0,   0,   0,   1,   0,   1,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
-    140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140,
-    137, 137, 137, 137, 137, 137, 137, 137, 137, 137, 137, 137, 137, 137, 137, 137,
-    138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138,
+    142, 142, 142, 142, 142, 142, 142, 142, 142, 142, 142, 142, 142, 142, 142, 142,
     139, 139, 139, 139, 139, 139, 139, 139, 139, 139, 139, 139, 139, 139, 139, 139,
-    138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138, 138,
+    140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140,
+    141, 141, 141, 141, 141, 141, 141, 141, 141, 141, 141, 141, 141, 141, 141, 141,
+    140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140, 140,
+      0,   0,   0,   0,   0,   3,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
+      0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,  45,  45,  45,  45,  45,  45,  45,  45,  45,  45,  45,  45,  45,  45,  45,
      45,  45,  45,  45,  45,  45,  45,  45,  45,  45,  45,   0,   0,   0,   0,   0,
      23,  23,  23,  23,  23,  23,  23,  23,  30,  30,  30,  30,  30,  30,  30,  30,
      23,  23,  23,  23,  23,  23,  23,  23,  43,  43,  43,  43,  43,  43,  43,  43,
      49,  49,  49,  49,  49,  49,  49,  49,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
       0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -29050,19 +29789,20 @@
       102,   104,   105,   106,   110,   112,   124,   127,
       128,   130,   134,   140,   144,   172,   186,   190,
       201,   202,   205,   208,   217,   219,   223,   231,
       233,   235,   239,   250,   252,   268,   345,   376,
       391,   777,   805,   806,   810,   825,   827,   935,
       958,   963,   971,   978,   982,   989,   991,  1002,
      1007,  1011,  1015,  1023,  3136,  3296,  6322,  6325,
-     6332,  6338,  6342,  6343,  6348,  6372,  7175,  7745,
-     8513,  8654,  8943, 11785, 11801, 11807, 11810, 11836,
-    11839, 11841, 11864, 11871, 12574, 15776, 15840, 42286,
-    42287, 42294, 42311, 42433, 42436, 42444, 42445, 42472,
-    42487, 47152, 47184, 47216, 47312, 47620, 47688, 47811
+     6332,  6338,  6342,  6343,  6348,  6372,  7175,  7235,
+     7251,  7745,  8513,  8654,  8943, 11785, 11801, 11807,
+    11810, 11836, 11839, 11841, 11864, 11871, 12574, 15776,
+    15840, 42286, 42287, 42294, 42311, 42433, 42436, 42444,
+    42445, 42472, 42487, 47152, 47184, 47216, 47312, 47620,
+    47688, 47811
 };
 
 RE_UINT32 re_get_simple_case_folding(RE_UINT32 codepoint) {
     RE_UINT32 field_2;
     RE_UINT32 field_1;
     RE_UINT32 field_0;
     RE_UINT32 v;
@@ -29616,19 +30356,23 @@
     re_get_grapheme_cluster_break,
     re_get_grapheme_extend,
     re_get_grapheme_link,
     re_get_hangul_syllable_type,
     re_get_hex_digit,
     re_get_horiz_space,
     re_get_hyphen,
+    re_get_id_compat_math_continue,
+    re_get_id_compat_math_start,
     re_get_id_continue,
     re_get_ideographic,
     re_get_ids_binary_operator,
     re_get_id_start,
     re_get_ids_trinary_operator,
+    re_get_ids_unary_operator,
+    re_get_indic_conjunct_break,
     re_get_indic_positional_category,
     re_get_indic_syllabic_category,
     re_get_join_control,
     re_get_joining_group,
     re_get_joining_type,
     re_get_line_break,
     re_get_logical_order_exception,
```

### Comparing `regex-2023.8.8/regex_3/_regex_unicode.h` & `regex-2024.4.16/regex_3/_regex_unicode.h`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     RE_UINT16 id;
 } RE_PropertyValue;
 
 typedef RE_UINT32 (*RE_GetPropertyFunc)(RE_UINT32 codepoint);
 
 #define RE_PROP_GC 0x1E
 #define RE_PROP_CASED 0xA
-#define RE_PROP_UPPERCASE 0x57
-#define RE_PROP_LOWERCASE 0x34
-#define RE_PROP_SCX 0x51
+#define RE_PROP_UPPERCASE 0x5B
+#define RE_PROP_LOWERCASE 0x38
+#define RE_PROP_SCX 0x55
 
 #define RE_PROP_C 30
 #define RE_PROP_L 31
 #define RE_PROP_M 32
 #define RE_PROP_N 33
 #define RE_PROP_P 34
 #define RE_PROP_S 35
@@ -91,24 +91,24 @@
 #define RE_PROP_ALPHA 0x000001
 #define RE_PROP_ANY 0x020001
 #define RE_PROP_ASCII 0x080001
 #define RE_PROP_BLANK 0x070001
 #define RE_PROP_CNTRL 0x1E0001
 #define RE_PROP_DIGIT 0x1E0009
 #define RE_PROP_GRAPH 0x1F0001
-#define RE_PROP_LOWER 0x340001
-#define RE_PROP_PRINT 0x4C0001
-#define RE_PROP_SPACE 0x5A0001
-#define RE_PROP_UPPER 0x570001
-#define RE_PROP_WORD 0x5B0001
-#define RE_PROP_XDIGIT 0x5D0001
-#define RE_PROP_POSIX_ALNUM 0x470001
-#define RE_PROP_POSIX_DIGIT 0x480001
-#define RE_PROP_POSIX_PUNCT 0x490001
-#define RE_PROP_POSIX_XDIGIT 0x4A0001
+#define RE_PROP_LOWER 0x380001
+#define RE_PROP_PRINT 0x500001
+#define RE_PROP_SPACE 0x5E0001
+#define RE_PROP_UPPER 0x5B0001
+#define RE_PROP_WORD 0x5F0001
+#define RE_PROP_XDIGIT 0x610001
+#define RE_PROP_POSIX_ALNUM 0x4B0001
+#define RE_PROP_POSIX_DIGIT 0x4C0001
+#define RE_PROP_POSIX_PUNCT 0x4D0001
+#define RE_PROP_POSIX_XDIGIT 0x4E0001
 
 #define RE_WBREAK_OTHER 0
 #define RE_WBREAK_LF 1
 #define RE_WBREAK_NEWLINE 2
 #define RE_WBREAK_CR 3
 #define RE_WBREAK_WSEGSPACE 4
 #define RE_WBREAK_DOUBLEQUOTE 5
@@ -174,34 +174,39 @@
 #define RE_LBREAK_BREAKBEFORE 22
 #define RE_LBREAK_HEBREWLETTER 23
 #define RE_LBREAK_COMPLEXCONTEXT 24
 #define RE_LBREAK_JL 25
 #define RE_LBREAK_JV 26
 #define RE_LBREAK_JT 27
 #define RE_LBREAK_NONSTARTER 28
-#define RE_LBREAK_ZWSPACE 29
-#define RE_LBREAK_ZWJ 30
-#define RE_LBREAK_BREAKBOTH 31
-#define RE_LBREAK_INSEPARABLE 32
-#define RE_LBREAK_WORDJOINER 33
-#define RE_LBREAK_IDEOGRAPHIC 34
-#define RE_LBREAK_EBASE 35
-#define RE_LBREAK_CONDITIONALJAPANESESTARTER 36
-#define RE_LBREAK_H2 37
-#define RE_LBREAK_H3 38
-#define RE_LBREAK_SURROGATE 39
-#define RE_LBREAK_CONTINGENTBREAK 40
-#define RE_LBREAK_REGIONALINDICATOR 41
-#define RE_LBREAK_EMODIFIER 42
-
-extern char* re_strings[1486];
-extern RE_Property re_properties[177];
-extern RE_PropertyValue re_property_values[1633];
+#define RE_LBREAK_AKSARA 29
+#define RE_LBREAK_VIRAMA 30
+#define RE_LBREAK_IDEOGRAPHIC 31
+#define RE_LBREAK_AKSARASTART 32
+#define RE_LBREAK_VIRAMAFINAL 33
+#define RE_LBREAK_ZWSPACE 34
+#define RE_LBREAK_ZWJ 35
+#define RE_LBREAK_BREAKBOTH 36
+#define RE_LBREAK_INSEPARABLE 37
+#define RE_LBREAK_WORDJOINER 38
+#define RE_LBREAK_EBASE 39
+#define RE_LBREAK_CONDITIONALJAPANESESTARTER 40
+#define RE_LBREAK_H2 41
+#define RE_LBREAK_H3 42
+#define RE_LBREAK_SURROGATE 43
+#define RE_LBREAK_CONTINGENTBREAK 44
+#define RE_LBREAK_AKSARAPREBASE 45
+#define RE_LBREAK_REGIONALINDICATOR 46
+#define RE_LBREAK_EMODIFIER 47
+
+extern char* re_strings[1506];
+extern RE_Property re_properties[183];
+extern RE_PropertyValue re_property_values[1651];
 extern RE_UINT16 re_expand_on_folding[104];
-extern RE_GetPropertyFunc re_get_property[96];
+extern RE_GetPropertyFunc re_get_property[100];
 
 RE_UINT32 re_get_alphabetic(RE_UINT32 codepoint);
 RE_UINT32 re_get_alphanumeric(RE_UINT32 codepoint);
 RE_UINT32 re_get_any(RE_UINT32 codepoint);
 RE_UINT32 re_get_ascii_hex_digit(RE_UINT32 codepoint);
 RE_UINT32 re_get_bidi_class(RE_UINT32 codepoint);
 RE_UINT32 re_get_bidi_control(RE_UINT32 codepoint);
@@ -235,19 +240,23 @@
 RE_UINT32 re_get_grapheme_cluster_break(RE_UINT32 codepoint);
 RE_UINT32 re_get_grapheme_extend(RE_UINT32 codepoint);
 RE_UINT32 re_get_grapheme_link(RE_UINT32 codepoint);
 RE_UINT32 re_get_hangul_syllable_type(RE_UINT32 codepoint);
 RE_UINT32 re_get_hex_digit(RE_UINT32 codepoint);
 RE_UINT32 re_get_horiz_space(RE_UINT32 codepoint);
 RE_UINT32 re_get_hyphen(RE_UINT32 codepoint);
+RE_UINT32 re_get_id_compat_math_continue(RE_UINT32 codepoint);
+RE_UINT32 re_get_id_compat_math_start(RE_UINT32 codepoint);
 RE_UINT32 re_get_id_continue(RE_UINT32 codepoint);
 RE_UINT32 re_get_ideographic(RE_UINT32 codepoint);
 RE_UINT32 re_get_ids_binary_operator(RE_UINT32 codepoint);
 RE_UINT32 re_get_id_start(RE_UINT32 codepoint);
 RE_UINT32 re_get_ids_trinary_operator(RE_UINT32 codepoint);
+RE_UINT32 re_get_ids_unary_operator(RE_UINT32 codepoint);
+RE_UINT32 re_get_indic_conjunct_break(RE_UINT32 codepoint);
 RE_UINT32 re_get_indic_positional_category(RE_UINT32 codepoint);
 RE_UINT32 re_get_indic_syllabic_category(RE_UINT32 codepoint);
 RE_UINT32 re_get_join_control(RE_UINT32 codepoint);
 RE_UINT32 re_get_joining_group(RE_UINT32 codepoint);
 RE_UINT32 re_get_joining_type(RE_UINT32 codepoint);
 RE_UINT32 re_get_line_break(RE_UINT32 codepoint);
 RE_UINT32 re_get_logical_order_exception(RE_UINT32 codepoint);
```

### Comparing `regex-2023.8.8/regex_3/regex.py` & `regex-2024.4.16/regex_3/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
   "sub", "subf", "subfn", "subn", "template", "Scanner", "A", "ASCII", "B",
   "BESTMATCH", "D", "DEBUG", "E", "ENHANCEMATCH", "S", "DOTALL", "F",
   "FULLCASE", "I", "IGNORECASE", "L", "LOCALE", "M", "MULTILINE", "P", "POSIX",
   "R", "REVERSE", "T", "TEMPLATE", "U", "UNICODE", "V0", "VERSION0", "V1",
   "VERSION1", "X", "VERBOSE", "W", "WORD", "error", "Regex", "__version__",
   "__doc__", "RegexFlag"]
 
-__version__ = "2.5.132"
+__version__ = "2.5.141"
 
 # --------------------------------------------------------------------
 # Public interface.
 
 def match(pattern, string, flags=0, pos=None, endpos=None, partial=False,
   concurrent=None, timeout=None, ignore_unused=False, **kwargs):
     """Try to apply the pattern at the start of the string, returning a match
@@ -388,26 +388,22 @@
     if special_only:
         for c in p:
             if c == " " and literal_spaces:
                 s.append(c)
             elif c in _METACHARS or c.isspace():
                 s.append("\\")
                 s.append(c)
-            elif c == "\x00":
-                s.append("\\000")
             else:
                 s.append(c)
     else:
         for c in p:
             if c == " " and literal_spaces:
                 s.append(c)
             elif c in _ALNUM:
                 s.append(c)
-            elif c == "\x00":
-                s.append("\\000")
             else:
                 s.append("\\")
                 s.append(c)
 
     r = "".join(s)
     # Convert it back to bytes if necessary.
     if isinstance(pattern, bytes):
```

### Comparing `regex-2023.8.8/regex_3/test_regex.py` & `regex-2024.4.16/regex_3/test_regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,18 +907,17 @@
 
         p = regex.compile('(?iu)' + upper_char)
         self.assertEqual(bool(p.match(lower_char)), True)
 
         p = regex.compile('(?iu)' + lower_char)
         self.assertEqual(bool(p.match(upper_char)), True)
 
+        # Changed to positional flags in regex 2023.12.23.
         self.assertEqual(bool(regex.match(r"(?i)a", "A")), True)
-        self.assertEqual(bool(regex.match(r"a(?i)", "A")), True)
-        self.assertEqual(bool(regex.match(r"(?iV1)a", "A")), True)
-        self.assertEqual(regex.match(r"a(?iV1)", "A"), None)
+        self.assertEqual(regex.match(r"a(?i)", "A"), None)
 
     def test_dollar_matches_twice(self):
         # $ matches the end of string, and just before the terminating \n.
         pattern = regex.compile('$')
         self.assertEqual(pattern.sub('#', 'a\nb\n'), 'a\nb#\n#')
         self.assertEqual(pattern.sub('#', 'a\nb\nc'), 'a\nb\nc#')
         self.assertEqual(pattern.sub('#', '\n'), '#\n#')
@@ -1392,26 +1391,23 @@
         self.assertEqual([m for m in regex.splititer("(?rV1)", "xaxbxc")], ['',
           'c', 'x', 'b', 'x', 'a', 'x', ''])
 
     def test_scoped_and_inline_flags(self):
         # Issues 433028, 433024, 433027.
         self.assertEqual(regex.search(r"(?i)Ab", "ab").span(), (0, 2))
         self.assertEqual(regex.search(r"(?i:A)b", "ab").span(), (0, 2))
-        self.assertEqual(regex.search(r"A(?i)b", "ab").span(), (0, 2))
-        self.assertEqual(regex.search(r"A(?iV1)b", "ab"), None)
-
-        self.assertRaisesRegex(regex.error, self.CANT_TURN_OFF, lambda:
-          regex.search(r"(?V0-i)Ab", "ab", flags=regex.I))
+        # Changed to positional flags in regex 2023.12.23.
+        self.assertEqual(regex.search(r"A(?i)b", "ab"), None)
 
         self.assertEqual(regex.search(r"(?V0)Ab", "ab"), None)
         self.assertEqual(regex.search(r"(?V1)Ab", "ab"), None)
-        self.assertEqual(regex.search(r"(?V1-i)Ab", "ab", flags=regex.I), None)
+        self.assertEqual(regex.search(r"(?-i)Ab", "ab", flags=regex.I), None)
         self.assertEqual(regex.search(r"(?-i:A)b", "ab", flags=regex.I), None)
-        self.assertEqual(regex.search(r"A(?V1-i)b", "ab",
-          flags=regex.I).span(), (0, 2))
+        self.assertEqual(regex.search(r"A(?-i)b", "ab", flags=regex.I).span(),
+          (0, 2))
 
     def test_repeated_repeats(self):
         # Issue 2537.
         self.assertEqual(regex.search(r"(?:a+)+", "aaa").span(), (0, 3))
         self.assertEqual(regex.search(r"(?:(?:ab)+c)+", "abcabc").span(), (0,
           6))
 
@@ -1816,20 +1812,18 @@
 
             # Test that . only matches \n in DOTALL mode.
             ('a.b', 'acb', '0', ascii('acb')),
             ('a.b', 'a\nb', '', ascii(None)),
             ('a.*b', 'acc\nccb', '', ascii(None)),
             ('a.{4,5}b', 'acc\nccb', '', ascii(None)),
             ('a.b', 'a\rb', '0', ascii('a\rb')),
-            # The new behaviour is that the inline flag affects only what follows.
-            ('a.b(?s)', 'a\nb', '0', ascii('a\nb')),
-            ('a.b(?sV1)', 'a\nb', '', ascii(None)),
+            # Changed to positional flags in regex 2023.12.23.
+            ('a.b(?s)', 'a\nb', '', ascii(None)),
             ('(?s)a.b', 'a\nb', '0', ascii('a\nb')),
-            ('a.*(?s)b', 'acc\nccb', '0', ascii('acc\nccb')),
-            ('a.*(?sV1)b', 'acc\nccb', '', ascii(None)),
+            ('a.*(?s)b', 'acc\nccb', '', ascii(None)),
             ('(?s)a.*b', 'acc\nccb', '0', ascii('acc\nccb')),
             ('(?s)a.{4,5}b', 'acc\nccb', '0', ascii('acc\nccb')),
 
             (')', '', '', regex.error, self.TRAILING_CHARS),           # Unmatched right bracket.
             ('', '', '0', "''"),    # Empty pattern.
             ('abc', 'abc', '0', ascii('abc')),
             ('abc', 'xbc', '', ascii(None)),
@@ -2341,20 +2335,17 @@
             ('w(?# comment 1)xy(?# comment 2)z', 'wxyz', '0', ascii('wxyz')),
 
             # Check odd placement of embedded pattern modifiers.
 
             # Not an error under PCRE/PRE:
             # When the new behaviour is turned on positional inline flags affect
             # only what follows.
-            ('w(?i)', 'W', '0', ascii('W')),
-            ('w(?iV1)', 'W', '0', ascii(None)),
+            ('w(?i)', 'W', '0', ascii(None)),
             ('w(?i)', 'w', '0', ascii('w')),
-            ('w(?iV1)', 'w', '0', ascii('w')),
             ('(?i)w', 'W', '0', ascii('W')),
-            ('(?iV1)w', 'W', '0', ascii('W')),
 
             # Comments using the x embedded pattern modifier.
             ("""(?x)w# comment 1
 x y
 # comment 2
 z""", 'wxyz', '0', ascii('wxyz')),
 
@@ -2399,22 +2390,18 @@
             (r'.*d', 'abc\nabd', '0', ascii('abd')),
             # Bug 112468: various expected syntax errors.
             (r'(', '', '', regex.error, self.MISSING_RPAREN),
             (r'[\41]', '!', '0', ascii('!')),
             # Bug 114033: nothing to repeat.
             (r'(x?)?', 'x', '0', ascii('x')),
             # Bug 115040: rescan if flags are modified inside pattern.
-            # If the new behaviour is turned on then positional inline flags
-            # affect only what follows.
-            (r' (?x)foo ', 'foo', '0', ascii('foo')),
-            (r' (?V1x)foo ', 'foo', '0', ascii(None)),
+            # Changed to positional flags in regex 2023.12.23.
+            (r' (?x)foo ', 'foo', '0', ascii(None)),
             (r'(?x) foo ', 'foo', '0', ascii('foo')),
-            (r'(?V1x) foo ', 'foo', '0', ascii('foo')),
             (r'(?x)foo ', 'foo', '0', ascii('foo')),
-            (r'(?V1x)foo ', 'foo', '0', ascii('foo')),
             # Bug 115618: negative lookahead.
             (r'(?<!abc)(d.f)', 'abcdefdof', '0', ascii('dof')),
             # Bug 116251: character class bug.
             (r'[\w-]+', 'laser_beam', '0', ascii('laser_beam')),
             # Bug 123769+127259: non-greedy backtracking bug.
             (r'.*?\S *:', 'xx:', '0', ascii('xx:')),
             (r'a[ ]*?\ (\d+).*', 'a   10', '0', ascii('a   10')),
@@ -3150,18 +3137,16 @@
           None))
 
         # Hg issue 38: regex.search("(?>.*/)b", "a/b") returns None
         self.assertEqual(regex.search("(?>.*/)b", "a/b").group(0), "a/b")
 
         # Hg issue 39: regex.search("((?i)blah)\\s+\\1", "blah BLAH") doesn't
         # return None
-        self.assertEqual(regex.search(r"(?V0)((?i)blah)\s+\1",
-          "blah BLAH").group(0, 1), ("blah BLAH", "blah"))
-        self.assertEqual(regex.search(r"(?V1)((?i)blah)\s+\1", "blah BLAH"),
-          None)
+        # Changed to positional flags in regex 2023.12.23.
+        self.assertEqual(regex.search(r"((?i)blah)\s+\1", "blah BLAH"), None)
 
         # Hg issue 40: regex.search("(\()?[^()]+(?(1)\)|)", "(abcd").group(0)
         # returns "bcd" instead of "abcd"
         self.assertEqual(regex.search(r"(\()?[^()]+(?(1)\)|)",
           "(abcd").group(0), "abcd")
 
         # Hg issue 42: regex.search("(a*)*", "a", flags=regex.V1).span(1)
@@ -4332,18 +4317,21 @@
         self.assertEqual(regex.match(r'(?(?<=A)|(?(?![^B])C|D))', 'A'), None)
         self.assertEqual(regex.search(r'(?(?<=A)|(?(?![^B])C|D))', 'A').span(), (1, 1))
 
         # Git issue 494: Backtracking failure matching regex ^a?(a?)b?c\1$ against string abca
         self.assertEqual(regex.search(r"^a?(a?)b?c\1$", "abca").span(), (0, 4))
 
         # Git issue 498: Conditional negative lookahead inside positive lookahead fails to match
-        self.assertEqual(regex.match(r"(?(?=a).|..)", "ab").span(), (0, 1))
-        self.assertEqual(regex.match(r"(?(?=b).|..)", "ab").span(), (0, 2))
-        self.assertEqual(regex.match(r"(?(?!a).|..)", "ab").span(), (0, 2))
-        self.assertEqual(regex.match(r"(?(?!b).|..)", "ab").span(), (0, 1))
+        self.assertEqual(regex.match(r'(?(?=a).|..)', 'ab').span(), (0, 1))
+        self.assertEqual(regex.match(r'(?(?=b).|..)', 'ab').span(), (0, 2))
+        self.assertEqual(regex.match(r'(?(?!a).|..)', 'ab').span(), (0, 2))
+        self.assertEqual(regex.match(r'(?(?!b).|..)', 'ab').span(), (0, 1))
+
+        # Git issue 525: segfault when fuzzy matching empty list
+        self.assertEqual(regex.match(r"(\L<foo>){e<=5}", "blah", foo=[]).span(), (0, 0))
 
     def test_fuzzy_ext(self):
         self.assertEqual(bool(regex.fullmatch(r'(?r)(?:a){e<=1:[a-z]}', 'e')),
           True)
         self.assertEqual(bool(regex.fullmatch(r'(?:a){e<=1:[a-z]}', 'e')),
           True)
         self.assertEqual(bool(regex.fullmatch(r'(?:a){e<=1:[a-z]}', '-')),
@@ -4456,12 +4444,18 @@
             self.assertEqual(regex.findall(r'\b|:+', 'a::bc'), ['', '', '::',
               '', ''])
             self.assertEqual([m.span() for m in regex.finditer(r'\b|:+',
               'a::bc')], [(0, 0), (1, 1), (1, 3), (3, 3), (5, 5)])
             self.assertEqual([m.span() for m in regex.finditer(r'(?m)^\s*?$',
               'foo\n\n\nbar')], [(4, 4), (4, 5), (5, 5)])
 
+    def test_line_ending(self):
+      self.assertEqual(regex.findall(r'\R', '\r\n\n\x0B\f\r\x85\u2028\u2029'),
+        ['\r\n', '\n', '\x0B', '\f', '\r', '\x85', '\u2028', '\u2029'])
+      self.assertEqual(regex.findall(br'\R', b'\r\n\n\x0B\f\r\x85'), [b'\r\n',
+        b'\n', b'\x0B', b'\f', b'\r'])
+
 def test_main():
     unittest.main(verbosity=2)
 
 if __name__ == "__main__":
     test_main()
```

### Comparing `regex-2023.8.8/setup.py` & `regex-2024.4.16/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 #!/usr/bin/env python
 from setuptools import setup, Extension
 from os.path import join
 
-with open('README.rst') as file:
+with open('README.rst', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='regex',
-    version='2023.8.8',
+    version='2024.4.16',
     description='Alternative regular expression module, to replace re.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Matthew Barnett',
     author_email='regex@mrabarnett.plus.com',
     url='https://github.com/mrabarnett/mrab-regex',
     license='Apache Software License',
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Text Processing',
         'Topic :: Text Processing :: General',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
 
     package_dir={'regex': 'regex_3'},
     py_modules=['regex.__init__', 'regex.regex', 'regex._regex_core',
      'regex.test_regex'],
     ext_modules=[Extension('regex._regex', [join('regex_3', '_regex.c'),
       join('regex_3', '_regex_unicode.c')])],
 )
```

### Comparing `regex-2023.8.8/tools/build_regex_unicode.py` & `regex-2024.4.16/tools/build_regex_unicode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-#! python3.9
+#! python3.11
 # -*- coding: utf-8 -*-
 #
-# This Python script parses the Unicode data files and generates the C files
-# for the regex module.
+# This Python script parses the Unicode data files in the UCD.zip file and
+# generates the C files for the regex module.
 #
 # Written by MRAB.
 #
-from contextlib import suppress
+from contextlib import contextmanager, suppress
+from io import TextIOWrapper
 from itertools import chain
 from os import listdir, mkdir
 from os.path import basename, dirname, exists, join, normpath
+from time import time
 from urllib.parse import urljoin
 from urllib.request import urlretrieve
-from time import time
+from zipfile import ZipFile
+import re
 
 import codecs
 import sys
 sys.stdout = codecs.getwriter('utf-8')(sys.stdout.detach())
 
-class Timed:
-    def __init__(self, message=None):
-        self._message = message
-
-    def __enter__(self):
-        self._start = time()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        finish = time()
-        elapsed = finish - self._start
+@contextmanager
+def UCDSubfile(zip_path, subfile_name):
+    with ZipFile(ucd_zip_path) as ucd_zip_file:
+        with ucd_zip_file.open(subfile_name) as bin_file:
+            with TextIOWrapper(bin_file, encoding='utf-8') as file:
+                yield file
 
-        if self._message is None:
-            print(f'Took {elapsed:0.2f} secs')
-        else:
-            print(f'{self._message} took {elapsed:0.2f} secs')
+def have_ucd_version(ucd_zip_path, desired_version):
+    with UCDSubfile(ucd_zip_path, 'ReadMe.txt') as file:
+        for line in file:
+            m = re.search(r'(?i)Version (\d+\.\d+\.\d+)', line)
 
-        return False
+            if m and m[1] == desired_version:
+                return True
+
+    return False
 
 def unique(iterable, key=None):
 
     if key is None:
         def key(item):
             return item
 
@@ -188,20 +190,18 @@
 
             if not exists(path):
                 url = urljoin(unicode_data_base, rel_path)
                 print('Downloading {} from {}'.format(rel_path, url),
                   flush=True)
                 urlretrieve(url, path)
 
-def parse_property_aliases(data_folder):
+def parse_property_aliases(ucd_zip_path):
     properties = {}
 
-    path = join(data_folder, 'PropertyAliases.txt')
-
-    with open(path, encoding='utf-8') as file:
+    with UCDSubfile(ucd_zip_path, 'PropertyAliases.txt') as file:
         for line in file:
             line = line.strip()
 
             if not line or line.startswith('#'):
                 continue
 
             fields = [field.strip() for field in line.split(';')]
@@ -210,18 +210,16 @@
             property = {'names': list(unique([prop_name] + fields, key=munge))}
 
             for name in property['names']:
                 properties[munge(name)] = property
 
     return properties
 
-def parse_value_aliases(data_folder, properties):
-    path = join(data_folder, 'PropertyValueAliases.txt')
-
-    with open(path, encoding='utf-8') as file:
+def parse_value_aliases(ucd_zip_path, properties):
+    with UCDSubfile(ucd_zip_path, 'PropertyValueAliases.txt') as file:
         for line in file:
             line = line.strip()
 
             if not line or line.startswith('#'):
                 continue
 
             line = line.partition('#')[0]
@@ -232,34 +230,55 @@
             property = properties[munge(prop_name)]
             value = {'names': list(unique([val_name] + fields, key=munge))}
             values = property.setdefault('values', {})
 
             for name in value['names']:
                 values[munge(name)] = value
 
-def parse_binary(properties, path):
-    with open(path, encoding='utf-8') as file:
+    binary_values = {'N', 'YES', 'TRUE', 'FALSE', 'T', 'Y', 'NO', 'F'}
+
+    for property in properties.values():
+        property['is_binary'] = set(property.get('values', [])) == binary_values
+
+def parse_binary(properties, subpath):
+    print('Parsing %s' % subpath, flush=True)
+
+    with UCDSubfile(ucd_zip_path, subpath) as file:
         for line in file:
             line = line.strip()
 
+            if line.startswith('# @missing:'):
+                default = line.split(';')[-1].strip()
+
             if not line or line.startswith('#'):
                 continue
 
             line = line.partition('#')[0]
             fields = [field.strip() for field in line.split(';')]
             codepoints = [int(part, 16) for part in fields[0].split('..')]
             prop_name = fields[1]
             property = properties[munge(prop_name)]
-            property.setdefault('default', munge('No'))
-            value = property['values'][munge('Yes')]
-            value.setdefault('codepoints', Ranges()).add(codepoints[0],
-              codepoints[-1])
 
-def parse_emoji(properties, path):
-    with open(path, encoding='utf-8') as file:
+            if property['is_binary']:
+                property.setdefault('default', munge('No'))
+                value = property['values'][munge('Yes')]
+                value.setdefault('codepoints', Ranges()).add(codepoints[0],
+                  codepoints[-1])
+            else:
+                # Not a binary property!
+                property.setdefault('default', munge(default))
+                val_name = fields[2]
+                value = property['values'][munge(val_name)]
+                value.setdefault('codepoints', Ranges()).add(codepoints[0],
+                  codepoints[-1])
+
+def parse_emoji(properties, subpath):
+    print('Parsing %s' % subpath, flush=True)
+
+    with UCDSubfile(ucd_zip_path, subpath) as file:
         for line in file:
             line = line.strip()
 
             if not line:
                 continue
 
             if line.startswith('# @missing:'):
@@ -291,16 +310,18 @@
                 except KeyError:
                     value = {'names': ['Yes']}
                     property['values'][munge('Yes')] = value
 
                 value.setdefault('codepoints', Ranges()).add(codepoints[0],
                   codepoints[-1])
 
-def parse_multivalue(properties, path):
-    with open(path, encoding='utf-8') as file:
+def parse_multivalue(properties, subpath):
+    print('Parsing %s' % subpath, flush=True)
+
+    with UCDSubfile(ucd_zip_path, subpath) as file:
         for line in file:
             line = line.strip()
 
             if not line:
                 continue
 
             if line.startswith('# Property:'):
@@ -320,18 +341,20 @@
                 fields = [field.strip() for field in line.split(';')]
                 codepoints = [int(part, 16) for part in fields[0].split('..')]
                 val_name = fields[1]
                 value = property['values'][munge(val_name)]
                 value.setdefault('codepoints', Ranges()).add(codepoints[0],
                   codepoints[-1])
 
-def parse_normalisation(properties, path):
+def parse_normalisation(properties, subpath):
+    print('Parsing %s' % subpath, flush=True)
+
     property = None
 
-    with open(path, encoding='utf-8') as file:
+    with UCDSubfile(ucd_zip_path, subpath) as file:
         for line in file:
             line = line.strip()
 
             if not line:
                 continue
 
             if line.startswith('# Derived Property:'):
@@ -350,16 +373,18 @@
                       fields[0].split('..')]
                     val_name = fields[2]
 
                     value = property['values'][munge(val_name)]
                     value.setdefault('codepoints', Ranges()).add(codepoints[0],
                       codepoints[-1])
 
-def parse_numeric_values(properties, path):
-    with open(path, encoding='utf-8') as file:
+def parse_numeric_values(properties, subpath):
+    print('Parsing %s' % subpath, flush=True)
+
+    with UCDSubfile(ucd_zip_path, subpath) as file:
         for line in file:
             line = line.strip()
 
             if not line:
                 continue
 
             if line.startswith('# Derived Property:'):
@@ -382,16 +407,18 @@
                 except KeyError:
                     value = {'names': [val_name]}
                     property['values'][munge(val_name)] = value
 
                 value.setdefault('codepoints', Ranges()).add(codepoints[0],
                   codepoints[-1])
 
-def parse_script_extensions(properties, path):
-    with open(path, encoding='utf-8') as file:
+def parse_script_extensions(properties, subpath):
+    print('Parsing %s' % subpath, flush=True)
+
+    with UCDSubfile(ucd_zip_path, subpath) as file:
         for line in file:
             line = line.strip()
 
             if not line:
                 continue
 
             if line.startswith('# Property:'):
@@ -409,20 +436,22 @@
                     value = property['values'][key]
                 except KeyError:
                     value = {'codepoints': Ranges()}
                     property['values'][key] = value
 
                 value['codepoints'].add(codepoints[0], codepoints[-1])
 
-def parse_case_folding(properties, path):
+def parse_case_folding(properties, subpath):
+    print('Parsing %s' % subpath, flush=True)
+
     simple_folding = {}
     full_folding = {}
     turkic_set = set()
 
-    with open(path, encoding='utf-8') as file:
+    with UCDSubfile(ucd_zip_path, subpath) as file:
         for line in file:
             line = line.strip()
 
             if not line or line.startswith('#'):
                 continue
 
             line = line.partition('#')[0]
@@ -447,40 +476,49 @@
     # Is the Turkic set what we expected?
     if turkic_set != {(0x49, (0x131, )), (0x130, (0x69, ))}:
         raise ValueError('Turkic set has changed')
 
     properties['simple_folding'] = simple_folding
     properties['full_folding'] = full_folding
 
-def parse_unicode_files(data_files, data_folder):
-    properties = parse_property_aliases(data_folder)
-    parse_value_aliases(data_folder, properties)
-
-    def ignore(*args):
-        pass
-
-    parsers = {
-        'aliases': ignore,
-        'binary': parse_binary,
-        'emoji': parse_emoji,
-        'multivalue': parse_multivalue,
-        'normalisation': parse_normalisation,
-        'numeric_values': parse_numeric_values,
-        'script_extensions': parse_script_extensions,
-        'case_folding': parse_case_folding,
-    }
+def parse_unicode_data_files(ucd_zip_path):
+    properties = parse_property_aliases(ucd_zip_path)
+    parse_value_aliases(ucd_zip_path, properties)
+
+    parse_binary(properties, 'PropList.txt')
+    parse_binary(properties, 'extracted/DerivedBinaryProperties.txt')
+    parse_binary(properties, 'DerivedCoreProperties.txt')
+
+    parse_emoji(properties, 'emoji/emoji-data.txt')
+
+    parse_normalisation(properties, 'DerivedNormalizationProps.txt')
+
+    parse_multivalue(properties, 'auxiliary/GraphemeBreakProperty.txt')
+    parse_multivalue(properties, 'auxiliary/SentenceBreakProperty.txt')
+    parse_multivalue(properties, 'auxiliary/WordBreakProperty.txt')
+    parse_multivalue(properties, 'Blocks.txt')
+    parse_multivalue(properties, 'extracted/DerivedBidiClass.txt')
+    parse_multivalue(properties, 'extracted/DerivedCombiningClass.txt')
+    parse_multivalue(properties, 'extracted/DerivedDecompositionType.txt')
+    parse_multivalue(properties, 'extracted/DerivedEastAsianWidth.txt')
+    parse_multivalue(properties, 'extracted/DerivedGeneralCategory.txt')
+    parse_multivalue(properties, 'extracted/DerivedJoiningGroup.txt')
+    parse_multivalue(properties, 'extracted/DerivedJoiningType.txt')
+    parse_multivalue(properties, 'LineBreak.txt')
+    parse_multivalue(properties, 'extracted/DerivedNumericType.txt')
+    parse_multivalue(properties, 'HangulSyllableType.txt')
+    parse_multivalue(properties, 'IndicPositionalCategory.txt')
+    parse_multivalue(properties, 'IndicSyllabicCategory.txt')
+    parse_multivalue(properties, 'Scripts.txt')
 
-    for section, rel_paths in data_files.items():
-        parse = parsers[section]
+    parse_numeric_values(properties, 'extracted/DerivedNumericValues.txt')
 
-        for rel_path in rel_paths:
-            data_file = basename(rel_path)
+    parse_script_extensions(properties, 'ScriptExtensions.txt')
 
-            print('Parsing {}'.format(data_file), flush=True)
-            parse(properties, join(data_folder, data_file))
+    parse_case_folding(properties, 'CaseFolding.txt')
 
     unicode_data = {'properties': {}}
 
     for prop_name, property in properties.items():
         if has_codepoints(property):
             unicode_data['properties'][prop_name] = property
         elif prop_name in {'simple_folding', 'full_folding'}:
@@ -637,23 +675,23 @@
 
 def has_codepoints(property):
     if 'values' not in property:
         return False
 
     return any('codepoints' in value for value in property['values'].values())
 
-def write_summary(unicode_data, tools_folder):
+def write_summary(unicode_data, unicode_version, tools_folder):
     print('Writing summary')
 
     properties = unicode_data['properties']
 
-    path = join(tools_folder, 'Unicode.txt')
+    path = join(tools_folder, 'Unicode %s.txt' % unicode_version)
 
     with open(path, 'w', encoding='ascii') as file:
-        file.write('Version {}\n'.format(UNICODE_VERSION))
+        file.write('Version {}\n'.format(unicode_version))
 
         for property in sorted(unique(properties.values(), key=id),
           key=preferred):
             if not has_codepoints(property):
                 print(property['names'][0])
                 continue
 
@@ -1304,15 +1342,15 @@
 
     folded[2] = data[2];
 
     return 3;
 }
 ''')
 
-def generate_code(unicode_data, tools_folder):
+def generate_code(unicode_data, unicode_version, output_folder):
     print('Generating code')
 
     # Codepoints that expand on full casefolding.
     expanded = []
 
     for key, ranges in unicode_data['full_folding'].items():
         if len(key) > 1:
@@ -1418,16 +1456,16 @@
 
             valueset_id = valueset_dict.setdefault(tuple(valueset),
               len(valueset_dict))
             property['valueset_id'] = valueset_id
 
     strings = collect_strings(properties)
 
-    c_path = join(tools_folder, 'unicode.c')
-    h_path = join(tools_folder, 'unicode.h')
+    c_path = join(output_folder, '_regex_unicode.c')
+    h_path = join(output_folder, '_regex_unicode.h')
 
     with open(c_path, 'w', newline='\n', encoding='ascii') as c_file:
         c_file.write('''\
 /* For Unicode version {} */
 
 #include "_regex_unicode.h"
 
@@ -1446,15 +1484,15 @@
 
 typedef struct {{
     RE_UINT16 data[RE_MAX_FOLDED];
 }} RE_FullCaseFolding;
 
 /* Strings. */
 char* re_strings[] = {{
-'''.format(UNICODE_VERSION))
+'''.format(unicode_version))
 
         lines = []
 
         for string in strings:
             lines.append('    "{}",\n'.format(string))
 
         strings_dict = {string: i for i, string in enumerate(strings)}
@@ -1711,83 +1749,36 @@
             else:
                 h_file.write('RE_UINT32 re_get_{}(RE_UINT32 codepoint);\n'.format(prop_name.lower()))
 
         h_file.write('int re_get_all_cases(RE_UINT32 codepoint, RE_UINT32* cases);\n')
         h_file.write('RE_UINT32 re_get_simple_case_folding(RE_UINT32 codepoint);\n')
         h_file.write('int re_get_full_case_folding(RE_UINT32 codepoint, RE_UINT32* folded);\n')
 
-# Whether to update the Unicode data files from the Unicode website.
-UNICODE_VERSION = '15.0.0'
+# The Unicode version.
+UNICODE_VERSION = '15.1.0'
 
-# The URL from which the Unicode data files can be obtained.
-unicode_data_base = 'http://www.unicode.org/Public/UNIDATA/'
+this_folder = dirname(__file__)
 
-NUM_CODEPOINTS = 0x110000
+# The URL from which the Unicode data can be obtained.
+ucd_zip_url = 'https://www.unicode.org/Public/zipped/%s/UCD.zip' % UNICODE_VERSION
 
-# The Unicode data files. The file names are relative to the website URL.
-unicode_data_files = '''
-[aliases]
-PropertyAliases.txt
-PropertyValueAliases.txt
-[binary]
-PropList.txt
-extracted/DerivedBinaryProperties.txt
-DerivedCoreProperties.txt
-[emoji]
-emoji/emoji-data.txt
-[normalisation]
-DerivedNormalizationProps.txt
-[multivalue]
-auxiliary/GraphemeBreakProperty.txt
-auxiliary/SentenceBreakProperty.txt
-auxiliary/WordBreakProperty.txt
-Blocks.txt
-extracted/DerivedBidiClass.txt
-extracted/DerivedCombiningClass.txt
-extracted/DerivedDecompositionType.txt
-extracted/DerivedEastAsianWidth.txt
-extracted/DerivedGeneralCategory.txt
-extracted/DerivedJoiningGroup.txt
-extracted/DerivedJoiningType.txt
-LineBreak.txt
-extracted/DerivedNumericType.txt
-HangulSyllableType.txt
-IndicPositionalCategory.txt
-IndicSyllabicCategory.txt
-Scripts.txt
-[numeric_values]
-extracted/DerivedNumericValues.txt
-[case_folding]
-CaseFolding.txt
-[script_extensions]
-ScriptExtensions.txt
-'''
-
-data_files = {}
-section = ''
-
-for line in unicode_data_files.splitlines():
-    if line[ : 1] + line[-1 : ] == '[]':
-        section = line[1 : -1]
-    elif line:
-        data_files.setdefault(section, []).append(line)
+ucd_zip_path = join(this_folder, 'UCD.zip')
 
-# The generated C files will be written into this folder.
-tools_folder = dirname(__file__)
+if not have_ucd_version(ucd_zip_path, UNICODE_VERSION):
+    # Download the zipped Unicode data.
+    print('Downloading UCD.zip for Unicode %s' % UNICODE_VERSION, flush=True)
+    urlretrieve(ucd_zip_url, ucd_zip_path)
 
-# The local folder in which the Unicode data files are stored.
-data_folder = join(tools_folder, 'unicode_data')
-
-with suppress(FileExistsError):
-    mkdir(data_folder)
+NUM_CODEPOINTS = 0x110000
 
-download_unicode_files(unicode_data_base, data_files, data_folder)
+# The generated C files will be written into this folder.
+tools_folder = dirname(__file__)
 
-unicode_data = parse_unicode_files(data_files, data_folder)
+unicode_data = parse_unicode_data_files(ucd_zip_path)
 make_additional_properties(unicode_data)
-write_summary(unicode_data, tools_folder)
+write_summary(unicode_data, UNICODE_VERSION, this_folder)
 
 binary_dict = make_binary_dict()
 
-generate_code(unicode_data, tools_folder)
+generate_code(unicode_data, UNICODE_VERSION, this_folder)
 
-print('\nFinished!')
+print('\nSuccessfully generated _regex_unicode.h and _regex_unicode.c in %s' % tools_folder)
```

