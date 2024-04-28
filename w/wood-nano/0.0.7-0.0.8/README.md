# Comparing `tmp/wood_nano-0.0.7-cp39-cp39-win_amd64.whl.zip` & `tmp/wood_nano-0.0.8-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1856298 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      968 b- defN 24-Apr-21 20:05 wood_nano/__init__.py
--rw-rw-rw-  2.0 fat     3560 b- defN 24-Apr-21 20:05 wood_nano/conversions_python.py
--rw-rw-rw-  2.0 fat   543027 b- defN 24-Apr-21 20:05 wood_nano/libgmp-10.dll
--rw-rw-rw-  2.0 fat   436011 b- defN 24-Apr-21 20:05 wood_nano/libmpfr-4.dll
--rw-rw-rw-  2.0 fat  3231744 b- defN 24-Apr-21 20:05 wood_nano/wood_nano_ext.cp39-win_amd64.pyd
--rw-rw-r--  2.0 fat     6389 b- defN 24-Apr-21 20:05 wood_nano-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 fat      103 b- defN 24-Apr-21 20:05 wood_nano-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 fat        0 b- defN 24-Apr-21 20:05 wood_nano-0.0.7.dist-info/entry_points.txt
--rw-rw-r--  2.0 fat     1547 b- defN 24-Apr-21 20:05 wood_nano-0.0.7.dist-info/licenses/LICENSE
--rw-rw-r--  2.0 fat      839 b- defN 24-Apr-21 20:05 wood_nano-0.0.7.dist-info/RECORD
-10 files, 4224188 bytes uncompressed, 1854874 bytes compressed:  56.1%
+Zip file size: 1855394 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      968 b- defN 24-Apr-28 21:41 wood_nano/__init__.py
+-rw-rw-rw-  2.0 fat     3560 b- defN 24-Apr-28 21:41 wood_nano/conversions_python.py
+-rw-rw-rw-  2.0 fat   543027 b- defN 24-Apr-28 21:41 wood_nano/libgmp-10.dll
+-rw-rw-rw-  2.0 fat   436011 b- defN 24-Apr-28 21:41 wood_nano/libmpfr-4.dll
+-rw-rw-rw-  2.0 fat  3230720 b- defN 24-Apr-28 21:41 wood_nano/wood_nano_ext.cp39-win_amd64.pyd
+-rw-rw-r--  2.0 fat     6400 b- defN 24-Apr-28 21:41 wood_nano-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 fat      103 b- defN 24-Apr-28 21:41 wood_nano-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 fat        0 b- defN 24-Apr-28 21:41 wood_nano-0.0.8.dist-info/entry_points.txt
+-rw-rw-r--  2.0 fat     1547 b- defN 24-Apr-28 21:41 wood_nano-0.0.8.dist-info/licenses/LICENSE
+-rw-rw-r--  2.0 fat      839 b- defN 24-Apr-28 21:41 wood_nano-0.0.8.dist-info/RECORD
+10 files, 4223175 bytes uncompressed, 1853970 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: wood_nano/libmpfr-4.dll
 Comment: 
 
 Filename: wood_nano/wood_nano_ext.cp39-win_amd64.pyd
 Comment: 
 
-Filename: wood_nano-0.0.7.dist-info/METADATA
+Filename: wood_nano-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: wood_nano-0.0.7.dist-info/WHEEL
+Filename: wood_nano-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: wood_nano-0.0.7.dist-info/entry_points.txt
+Filename: wood_nano-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: wood_nano-0.0.7.dist-info/licenses/LICENSE
+Filename: wood_nano-0.0.8.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: wood_nano-0.0.7.dist-info/RECORD
+Filename: wood_nano-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `wood_nano-0.0.7.dist-info/METADATA` & `wood_nano-0.0.8.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wood-nano
-Version: 0.0.7
+Version: 0.0.8
 Summary: Binding for wood project that  is compiled into a binding using nanobind and scikit-build
 Author-Email: Petras Vestartas <petrasvestartas@gmail.com>
 Classifier: License :: OSI Approved :: BSD License
 Project-URL: Homepage, https://github.com/petrasvestartas/wood_nano
 Requires-Python: >=3.8.16
 Description-Content-Type: text/markdown
 
@@ -161,20 +161,21 @@
         -   compas_wood - invoke docs and check the result
 
 compas_wood
 -----------
 
 
 ```bash
-git branch v2
-git checkout v2
+
 conda config --add channels conda-forge
-conda create -n compas_wood python==3.8.16 pypy=7.3.11
-conda activate compas_wood
-pip install build setuptools wheel cookiecutter jinja2_time compas_invocations
+conda create -n compas_wood_3_9_10 python==3.9_10 compas
+conda activate compas_wood_3_9_10
+conda install build setuptools wheel twine 
+upload to pip https://github.com/petrasvestartas/compas_snippets
+
 sudo apt install twine or conda install twine
 cookiecutter gh:compas-dev/compas_package_template
 export PATH="~/anaconda3/envs/compas_wood/bin:$PATH"
 sudo apt install invoke
 pip install -r requirements.txt
 ```
```

## Comparing `wood_nano-0.0.7.dist-info/licenses/LICENSE` & `wood_nano-0.0.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

