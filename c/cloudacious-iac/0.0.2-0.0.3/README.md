# Comparing `tmp/cloudacious_iac-0.0.2.tar.gz` & `tmp/cloudacious_iac-0.0.3.tar.gz`

## Comparing `cloudacious_iac-0.0.2.tar` & `cloudacious_iac-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/.pypirc
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/config.cfg
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/setup.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/src/cloudacious-iac/ContainerImages.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/src/cloudacious-iac/Naming.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/src/cloudacious-iac/README.md
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/src/cloudacious-iac/StackInfo.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/.gitignore
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/.pypirc
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/config.cfg
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/setup.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/src/cloudacious-iac/ContainerImages.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/src/cloudacious-iac/Naming.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/src/cloudacious-iac/README.md
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/src/cloudacious-iac/StackInfo.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/.gitignore
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cloudacious_iac-0.0.3/PKG-INFO
```

### Comparing `cloudacious_iac-0.0.2/.gitlab-ci.yml` & `cloudacious_iac-0.0.3/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     - cp .pypirc ~/
     - python -m pip install --upgrade build
     - python -m pip install --upgrade twine
   # environment:
   #   name: production
   #   url: https://prod.cloudacious.io
   rules:
-    # - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
+    - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
     - if: $CI_COMMIT_TAG
       when: manual
   variables:
     TWINE_PASSWORD: $PYPI_TOKEN
     TWINE_USERNAME: "__token__"
   script:
     - python -m build
```

### Comparing `cloudacious_iac-0.0.2/setup.py` & `cloudacious_iac-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 setup(
     name="cloudacious-iac",
     version=os.getenv("CI_COMMIT_TAG"), 
     description="Cloudacious's object-oriented IaC tooling w/Pulumi. Call our classes all day long!",
     long_description=long_description,
     long_description_content_type="README.md",
+    readme = "README.md"
     url="https://gitlab.com/money-marathon/cloudacious/cloudacious-iac.git",
     author="A. SurfingDoggo",
     author_email="git@surfingdoggo.com",  
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
```

### Comparing `cloudacious_iac-0.0.2/src/cloudacious-iac/ContainerImages.py` & `cloudacious_iac-0.0.3/src/cloudacious-iac/ContainerImages.py`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.2/src/cloudacious-iac/Naming.py` & `cloudacious_iac-0.0.3/src/cloudacious-iac/Naming.py`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.2/src/cloudacious-iac/README.md` & `cloudacious_iac-0.0.3/src/cloudacious-iac/README.md`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.2/src/cloudacious-iac/StackInfo.py` & `cloudacious_iac-0.0.3/src/cloudacious-iac/StackInfo.py`

 * *Files identical despite different names*

### Comparing `cloudacious_iac-0.0.2/.gitignore` & `cloudacious_iac-0.0.3/.gitignore`

 * *Files identical despite different names*

