# Comparing `tmp/fontfinder-0.10.0.tar.gz` & `tmp/fontfinder-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fontfinder-0.10.0.tar", last modified: Thu Apr 18 13:10:02 2024, max compression
+gzip compressed data, was "fontfinder-0.11.0.tar", last modified: Sun Apr 28 14:02:11 2024, max compression
```

## Comparing `fontfinder-0.10.0.tar` & `fontfinder-0.11.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-18 13:10:02.443979 fontfinder-0.10.0/
--rw-r--r--   0 james      (501) staff       (20)     1070 2023-10-04 08:55:25.000000 fontfinder-0.10.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     4500 2024-04-18 13:10:02.443527 fontfinder-0.10.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     3447 2024-04-17 13:23:00.000000 fontfinder-0.10.0/README.md
--rw-r--r--   0 james      (501) staff       (20)     1140 2024-04-18 12:57:42.000000 fontfinder-0.10.0/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2024-04-18 13:10:02.444037 fontfinder-0.10.0/setup.cfg
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-18 13:10:02.432486 fontfinder-0.10.0/src/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-18 13:10:02.435211 fontfinder-0.10.0/src/fontfinder/
--rw-r--r--   0 james      (501) staff       (20)    27643 2024-04-18 11:43:58.000000 fontfinder-0.10.0/src/fontfinder/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1522 2024-04-16 12:22:58.000000 fontfinder-0.10.0/src/fontfinder/_generate_data.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-18 13:10:02.439863 fontfinder-0.10.0/src/fontfinder/_platforms/
--rw-r--r--   0 james      (501) staff       (20)     3464 2024-04-13 11:30:21.000000 fontfinder-0.10.0/src/fontfinder/_platforms/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     8109 2024-04-16 12:45:01.000000 fontfinder-0.10.0/src/fontfinder/_platforms/mac.py
--rw-r--r--   0 james      (501) staff       (20)    10212 2024-04-17 13:25:56.000000 fontfinder-0.10.0/src/fontfinder/_platforms/windows.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-18 13:10:02.441228 fontfinder-0.10.0/src/fontfinder/data/
--rw-r--r--   0 james      (501) staff       (20)  1011476 2024-04-06 08:01:13.000000 fontfinder-0.10.0/src/fontfinder/data/noto.json
--rw-r--r--   0 james      (501) staff       (20)   636190 2024-04-07 11:12:34.000000 fontfinder-0.10.0/src/fontfinder/data/small_unihan.json
--rw-r--r--   0 james      (501) staff       (20)     2408 2024-04-13 06:52:36.000000 fontfinder-0.10.0/src/fontfinder/filters.py
--rw-r--r--   0 james      (501) staff       (20)    17987 2024-04-13 11:37:30.000000 fontfinder-0.10.0/src/fontfinder/model.py
--rw-r--r--   0 james      (501) staff       (20)    11024 2023-10-05 11:12:34.000000 fontfinder-0.10.0/src/fontfinder/noto.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-18 13:10:02.442630 fontfinder-0.10.0/src/fontfinder.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     4500 2024-04-18 13:10:02.000000 fontfinder-0.10.0/src/fontfinder.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      554 2024-04-18 13:10:02.000000 fontfinder-0.10.0/src/fontfinder.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-04-18 13:10:02.000000 fontfinder-0.10.0/src/fontfinder.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      175 2024-04-18 13:10:02.000000 fontfinder-0.10.0/src/fontfinder.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       11 2024-04-18 13:10:02.000000 fontfinder-0.10.0/src/fontfinder.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-18 13:10:02.442028 fontfinder-0.10.0/test/
--rw-r--r--   0 james      (501) staff       (20)    42692 2024-04-13 15:02:13.000000 fontfinder-0.10.0/test/test_fontfinder.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.863469 fontfinder-0.11.0/
+-rw-r--r--   0 james      (501) staff       (20)     1070 2023-10-04 08:55:25.000000 fontfinder-0.11.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     4500 2024-04-28 14:02:11.858080 fontfinder-0.11.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     3447 2024-04-17 13:23:00.000000 fontfinder-0.11.0/README.md
+-rw-r--r--   0 james      (501) staff       (20)     1140 2024-04-28 14:00:56.000000 fontfinder-0.11.0/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-04-28 14:02:11.863548 fontfinder-0.11.0/setup.cfg
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.806129 fontfinder-0.11.0/src/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.810732 fontfinder-0.11.0/src/fontfinder/
+-rw-r--r--   0 james      (501) staff       (20)    27988 2024-04-28 13:54:54.000000 fontfinder-0.11.0/src/fontfinder/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1522 2024-04-16 12:22:58.000000 fontfinder-0.11.0/src/fontfinder/_generate_data.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.819050 fontfinder-0.11.0/src/fontfinder/_platforms/
+-rw-r--r--   0 james      (501) staff       (20)     3464 2024-04-13 11:30:21.000000 fontfinder-0.11.0/src/fontfinder/_platforms/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     8109 2024-04-16 12:45:01.000000 fontfinder-0.11.0/src/fontfinder/_platforms/mac.py
+-rw-r--r--   0 james      (501) staff       (20)    10212 2024-04-17 13:25:56.000000 fontfinder-0.11.0/src/fontfinder/_platforms/windows.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.844544 fontfinder-0.11.0/src/fontfinder/data/
+-rw-r--r--   0 james      (501) staff       (20)  1011476 2024-04-06 08:01:13.000000 fontfinder-0.11.0/src/fontfinder/data/noto.json
+-rw-r--r--   0 james      (501) staff       (20)   636190 2024-04-07 11:12:34.000000 fontfinder-0.11.0/src/fontfinder/data/small_unihan.json
+-rw-r--r--   0 james      (501) staff       (20)     2408 2024-04-13 06:52:36.000000 fontfinder-0.11.0/src/fontfinder/filters.py
+-rw-r--r--   0 james      (501) staff       (20)    17987 2024-04-13 11:37:30.000000 fontfinder-0.11.0/src/fontfinder/model.py
+-rw-r--r--   0 james      (501) staff       (20)    11024 2023-10-05 11:12:34.000000 fontfinder-0.11.0/src/fontfinder/noto.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.855678 fontfinder-0.11.0/src/fontfinder.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     4500 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      554 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      175 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       11 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.854253 fontfinder-0.11.0/test/
+-rw-r--r--   0 james      (501) staff       (20)    43525 2024-04-28 13:58:29.000000 fontfinder-0.11.0/test/test_fontfinder.py
```

### Comparing `fontfinder-0.10.0/LICENSE` & `fontfinder-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/PKG-INFO` & `fontfinder-0.11.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontfinder
-Version: 0.10.0
+Version: 0.11.0
 Summary: Package for finding and installing fonts for Unicode scripts.
 Project-URL: Documentation, https://multiscript.app/fontfinder
 Project-URL: Source, https://github.com/multiscript/fontfinder
 Project-URL: Issue Tracker, https://github.com/multiscript/fontfinder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fontfinder-0.10.0/README.md` & `fontfinder-0.11.0/README.md`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/pyproject.toml` & `fontfinder-0.11.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fontfinder"
-version = "0.10.0"
+version = "0.11.0"
 
 description = "Package for finding and installing fonts for Unicode scripts."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "requests>=2.31",
     "semver>=3.0.2",
```

### Comparing `fontfinder-0.10.0/src/fontfinder/__init__.py` & `fontfinder-0.11.0/src/fontfinder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,29 +314,37 @@
         Some font families match several Unicode scripts. In these cases, `main_script` and `script_variant`
         can optionally be specified, to ensure these fields have the correct value in the returned `FontInfo` list.
         Otherwise, `main_script` and `script_variant` will have the first values found within the given font families.
         '''
         family_names = family_name_or_names
         if isinstance(family_names, str):
             family_names = [family_names]
-        font_infos = self.known_fonts(lambda font_info: font_info.family_name in family_names)
-        if len(font_infos) == 0:
-            return font_infos
-        # font_infos can be duplicated under multiple script variants. If no script and variant is specified, we
-        # just pick the first.
-        if main_script is None:
-            main_script = font_infos[0].main_script
-        if script_variant is None:
-            script_variant = font_infos[0].script_variant
-        font_infos = [font_info for font_info in font_infos if font_info.main_script == main_script and \
-                                                               font_info.script_variant == script_variant]
-        count_func = len
-        font_infos = self._apply_pref_dict(main_script, script_variant, self.family_font_prefs, count_func,
-                                           font_infos)
-        return font_infos
+        
+        result_font_infos = []
+        for family_name in family_names:
+            font_infos = self.known_fonts(lambda font_info: font_info.family_name == family_name)
+            if len(font_infos) == 0:
+                continue
+            # font_infos can be duplicated under multiple script variants. If no script and variant is specified, we
+            # just pick the first.
+            if main_script is None:
+                family_main_script = font_infos[0].main_script
+            else:
+                family_main_script = main_script
+            if script_variant is None:
+                family_script_variant = font_infos[0].script_variant
+            else:
+                family_script_variant = script_variant
+            font_infos = [font_info for font_info in font_infos if font_info.main_script == family_main_script and \
+                                                                font_info.script_variant == family_script_variant]
+            count_func = len
+            font_infos = self._apply_pref_dict(main_script, script_variant, self.family_font_prefs, count_func,
+                                            font_infos)
+            result_font_infos.extend(font_infos)
+        return result_font_infos
 
     def find_family_fonts_to_download(self, family_name_or_names: str | Iterable[str],
                                       main_script:str = None, script_variant:str = None) -> list[FontInfo]:
         '''Returns a list of `FontInfo` objects for font files that need to be downloaded. This list is formed
         by finding fonts matching the given family names, where those families are not currently installed,
         the filters in `family_font_prefs` have been applied, and the fonts have download URLs provided.
```

### Comparing `fontfinder-0.10.0/src/fontfinder/_generate_data.py` & `fontfinder-0.11.0/src/fontfinder/_generate_data.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder/_platforms/__init__.py` & `fontfinder-0.11.0/src/fontfinder/_platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder/_platforms/mac.py` & `fontfinder-0.11.0/src/fontfinder/_platforms/mac.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder/_platforms/windows.py` & `fontfinder-0.11.0/src/fontfinder/_platforms/windows.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder/data/noto.json` & `fontfinder-0.11.0/src/fontfinder/data/noto.json`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder/data/small_unihan.json` & `fontfinder-0.11.0/src/fontfinder/data/small_unihan.json`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder/filters.py` & `fontfinder-0.11.0/src/fontfinder/filters.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder/model.py` & `fontfinder-0.11.0/src/fontfinder/model.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder/noto.py` & `fontfinder-0.11.0/src/fontfinder/noto.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/src/fontfinder.egg-info/PKG-INFO` & `fontfinder-0.11.0/src/fontfinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontfinder
-Version: 0.10.0
+Version: 0.11.0
 Summary: Package for finding and installing fonts for Unicode scripts.
 Project-URL: Documentation, https://multiscript.app/fontfinder
 Project-URL: Source, https://github.com/multiscript/fontfinder
 Project-URL: Issue Tracker, https://github.com/multiscript/fontfinder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fontfinder-0.10.0/src/fontfinder.egg-info/SOURCES.txt` & `fontfinder-0.11.0/src/fontfinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fontfinder-0.10.0/test/test_fontfinder.py` & `fontfinder-0.11.0/test/test_fontfinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,20 +133,37 @@
         ff = FontFinder()
         for sample_text in sample_texts:
             family_name = ff.find_family(sample_text['text'])
             assert sample_text['expected_family_name'] == family_name
 
     def test_find_family_fonts(self):
         ff = FontFinder()
-        main_script = "Latin"
-        script_variant = ""
-        print("Finding family")
-        family_name = ff.find_family(TextInfo(main_script, script_variant))
         print("Finding family members")
-        ff.find_family_fonts(family_name)
+        font_infos = ff.find_family_fonts("Noto Naskh Arabic")
+        fullnames = {font_info.fullname for font_info in font_infos}
+        assert fullnames == {'Noto Naskh Arabic Bold', 'Noto Naskh Arabic Medium',
+                            'Noto Naskh Arabic Regular', 'Noto Naskh Arabic SemiBold'}
+    
+    def test_find_multiple_family_fonts(self):
+        ff = FontFinder()
+        family_1 = "Noto Naskh Arabic"
+        family_2 = "Noto Sans Cherokee"
+
+        font_infos_1 = ff.find_family_fonts(family_1)
+        fullnames_1 = {font_info.fullname for font_info in font_infos_1}
+        assert len(fullnames_1) > 0
+
+        font_infos_2 = ff.find_family_fonts(family_2)
+        fullnames_2 = {font_info.fullname for font_info in font_infos_2}
+        assert len(fullnames_2) > 0
+        assert fullnames_1 != fullnames_2
+
+        font_infos_combo = ff.find_family_fonts([family_1, family_2])
+        fullnames_combo = {font_info.fullname for font_info in font_infos_combo}
+        assert fullnames_combo == fullnames_1 | fullnames_2
 
     def test_find_empty_family_fonts(self):
         ff = FontFinder()
         font_infos = ff.find_family_fonts([])
         assert font_infos == []
 
         font_infos = ff.find_family_fonts([], "Latin")
```

