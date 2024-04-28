# Comparing `tmp/shaq-0.0.2.tar.gz` & `tmp/shaq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaq-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "shaq-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shaq-0.0.2.tar` & `shaq-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2024-04-04 02:18:27.776173 shaq-0.0.2/LICENSE
--rw-r--r--   0        0        0     1430 2024-04-04 02:18:27.776173 shaq-0.0.2/README.md
--rw-r--r--   0        0        0     1608 2024-04-04 02:18:27.776173 shaq-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-04 02:18:27.776173 shaq-0.0.2/shaq/__init__.py
--rw-r--r--   0        0        0       70 2024-04-04 02:18:27.776173 shaq-0.0.2/shaq/__main__.py
--rw-r--r--   0        0        0     6448 2024-04-04 02:18:27.776173 shaq-0.0.2/shaq/_cli.py
--rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 shaq-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-04-28 16:07:14.205057 shaq-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1430 2024-04-28 16:07:14.205057 shaq-0.0.3/README.md
+-rw-r--r--   0        0        0     1596 2024-04-28 16:07:14.205057 shaq-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-28 16:07:14.205057 shaq-0.0.3/shaq/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-28 16:07:14.205057 shaq-0.0.3/shaq/__main__.py
+-rw-r--r--   0        0        0     6443 2024-04-28 16:07:14.205057 shaq-0.0.3/shaq/_cli.py
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 shaq-0.0.3/PKG-INFO
```

### Comparing `shaq-0.0.2/LICENSE` & `shaq-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shaq-0.0.2/README.md` & `shaq-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `shaq-0.0.2/pyproject.toml` & `shaq-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: Multimedia :: Sound/Audio :: Analysis",
 ]
 dependencies = [
     "pyaudio ~= 0.2.13",
     "pydub ~= 0.25.1",
     "rich ~= 13.4",
-    "shazamio >= 0.4.0.1,< 0.5.2.0",
+    "shazamio ~= 0.6.0",
 ]
 requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://pypi.org/project/shaq/"
 Issues = "https://github.com/woodruffw/shaq/issues"
 Source = "https://github.com/woodruffw/shaq"
```

### Comparing `shaq-0.0.2/shaq/_cli.py` & `shaq-0.0.3/shaq/_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     input: bytearray | AudioSegment
     if args.listen:
         input = _listen(console, args)
     else:
         input = _from_file(console, args)
 
     shazam = Shazam(language="en-US", endpoint_country="US")
-    return await shazam.recognize_song(input)  # type: ignore
+    return await shazam.recognize(input)  # type: ignore
 
 
 def _parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     input_group = parser.add_mutually_exclusive_group(required=True)
     input_group.add_argument(
         "--listen", action="store_true", help="detect from the system's microphone"
```

### Comparing `shaq-0.0.2/PKG-INFO` & `shaq-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: shaq
-Version: 0.0.2
+Version: 0.0.3
 Summary: A bare-bones Shazam CLI client
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Requires-Dist: pyaudio ~= 0.2.13
 Requires-Dist: pydub ~= 0.25.1
 Requires-Dist: rich ~= 13.4
-Requires-Dist: shazamio >= 0.4.0.1,< 0.5.2.0
+Requires-Dist: shazamio ~= 0.6.0
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: shaq[test,lint] ; extra == "dev"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: ruff ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
```

