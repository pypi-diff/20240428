# Comparing `tmp/cloudacious_iac-0.0.1.tar.gz` & `tmp/cloudacious_iac-0.0.2.tar.gz`

## Comparing `cloudacious_iac-0.0.1.tar` & `cloudacious_iac-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/.pypirc
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/config.cfg
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/setup.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/src/cloudacious-iac/ContainerImages.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/src/cloudacious-iac/Naming.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/src/cloudacious-iac/README.md
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/src/cloudacious-iac/StackInfo.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/.gitignore
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/.pypirc
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/config.cfg
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/setup.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/src/cloudacious-iac/ContainerImages.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/src/cloudacious-iac/Naming.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/src/cloudacious-iac/README.md
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/src/cloudacious-iac/StackInfo.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/.gitignore
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/PKG-INFO
```

### Comparing `cloudacious_iac-0.0.1/README.md` & `cloudacious_iac-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.1/setup.py` & `cloudacious_iac-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import os
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="cloudacious-iac",
-    version="0.0.1",
+    version=os.getenv("CI_COMMIT_TAG"), 
     description="Cloudacious's object-oriented IaC tooling w/Pulumi. Call our classes all day long!",
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type="README.md",
     url="https://gitlab.com/money-marathon/cloudacious/cloudacious-iac.git",
     author="A. SurfingDoggo",
-    author_email="git@surfingdoggo.com",  # Optional
+    author_email="git@surfingdoggo.com",  
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

### Comparing `cloudacious_iac-0.0.1/src/cloudacious-iac/ContainerImages.py` & `cloudacious_iac-0.0.2/src/cloudacious-iac/ContainerImages.py`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.1/src/cloudacious-iac/Naming.py` & `cloudacious_iac-0.0.2/src/cloudacious-iac/Naming.py`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.1/src/cloudacious-iac/README.md` & `cloudacious_iac-0.0.2/src/cloudacious-iac/README.md`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.1/src/cloudacious-iac/StackInfo.py` & `cloudacious_iac-0.0.2/src/cloudacious-iac/StackInfo.py`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.1/.gitignore` & `cloudacious_iac-0.0.2/.gitignore`

 * *Files identical despite different names*

