# Comparing `tmp/whisper_cpp_cli-0.0.1.tar.gz` & `tmp/whisper_cpp_cli-0.0.1a0.tar.gz`

## Comparing `whisper_cpp_cli-0.0.1.tar` & `whisper_cpp_cli-0.0.1a0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/requirements-dev.in
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/.github/workflows/workflow.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/whisper_cpp/__init__.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/whisper_cpp/__main__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/LICENSE
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/README.md
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/hatch_build.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/requirements-dev.in
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/requirements-dev.txt
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/.gitignore
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/encodings.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/vcs.xml
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/whisper-cpp.iml
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/workspace.xml
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/whisper_cpp/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/whisper_cpp/__main__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/LICENSE
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/README.md
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/hatch_build.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 whisper_cpp_cli-0.0.1a0/PKG-INFO
```

### Comparing `whisper_cpp_cli-0.0.1/.github/workflows/workflow.yml` & `whisper_cpp_cli-0.0.1a0/.github/workflows/workflow.yml`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.17.0
         env:
-          CIBW_TEST_COMMAND: >
-            whisper-cpp -h &&
-            python -m whisper_cpp -h
+          CIBW_TEST_COMMAND: whisper-cpp -h
           CIBW_ARCHS_MACOS: "native"
           CIBW_BUILD: "cp312-*"
 
       - uses: actions/upload-artifact@v4
         with:
           name: cibw-wheels-${{ matrix.os }}-${{ strategy.job-index }}
           path: ./wheelhouse/*.whl
@@ -55,17 +53,15 @@
         uses: docker/setup-qemu-action@v3
         with:
           platforms: all
 
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.17.0
         env:
-          CIBW_TEST_COMMAND: >
-            whisper-cpp -h &&
-            python -m whisper_cpp -h
+          CIBW_TEST_COMMAND: whisper-cpp -h
           CIBW_ARCHS_LINUX: ${{ matrix.arch }}
           CIBW_BUILD: "cp312-${{ matrix.tag }}_*"
 
       - uses: actions/upload-artifact@v4
         with:
           name: cibw-wheels-linux-${{ matrix.arch }}-${{ matrix.tag }}-${{ strategy.job-index }}
           path: ./wheelhouse/*.whl
```

### Comparing `whisper_cpp_cli-0.0.1/whisper_cpp/__main__.py` & `whisper_cpp_cli-0.0.1a0/whisper_cpp/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import sysconfig
 
 
 def find_whisper_bin() -> str:
     """Return the whisper binary path."""
 
-    whisper_exe = "whisper-cpp" + sysconfig.get_config_var("EXE")
+    whisper_exe = "whisper" + sysconfig.get_config_var("EXE")
 
     path = os.path.join(sysconfig.get_path("scripts"), whisper_exe)
     if os.path.isfile(path):
         return path
 
     if sys.version_info >= (3, 10):
         user_scheme = sysconfig.get_preferred_scheme("user")
```

### Comparing `whisper_cpp_cli-0.0.1/.gitignore` & `whisper_cpp_cli-0.0.1a0/.gitignore`

 * *Files identical despite different names*

### Comparing `whisper_cpp_cli-0.0.1/LICENSE` & `whisper_cpp_cli-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_cli-0.0.1/README.md` & `whisper_cpp_cli-0.0.1a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# whisper.cpp-cli
+# whisper.cpp-py
 
 A Python wrapper around the [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp) CLI.
 
 Packages [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp) into pre-built, `pip`-installable
 wheels, for macOS and Linux.
 
 ## Installation
@@ -44,15 +44,14 @@
 
 [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp) is compiled without any CPU or GPU
 acceleration.
 
 In the future, I'd like to distribute builds with
 [Core ML support](https://github.com/ggerganov/whisper.cpp?tab=readme-ov-file#core-ml-support),
 [CUDA support](https://github.com/ggerganov/whisper.cpp?tab=readme-ov-file#nvidia-gpu-support), and
-more, given [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp)'s own support for these
-features.
+more, given `whisper.cpp`'s own support for these features.
 
 The latest release compiles against [`v1.5.5`](https://github.com/ggerganov/whisper.cpp/releases/tag/v1.5.5).
 
 ## License
 
 MIT
```

### Comparing `whisper_cpp_cli-0.0.1/hatch_build.py` & `whisper_cpp_cli-0.0.1a0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_cli-0.0.1/pyproject.toml` & `whisper_cpp_cli-0.0.1a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "whisper.cpp-cli"
-version = "0.0.1"
+version = "0.0.1a0"
 description = "A Python package for the whisper.cpp CLI."
 authors = [{ name = "Charlie Marsh", email = "charlie.r.marsh@gmail.com" }]
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 dependencies = []
```

### Comparing `whisper_cpp_cli-0.0.1/PKG-INFO` & `whisper_cpp_cli-0.0.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: whisper.cpp-cli
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: A Python package for the whisper.cpp CLI.
 Author-email: Charlie Marsh <charlie.r.marsh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Charles Marsh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# whisper.cpp-cli
+# whisper.cpp-py
 
 A Python wrapper around the [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp) CLI.
 
 Packages [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp) into pre-built, `pip`-installable
 wheels, for macOS and Linux.
 
 ## Installation
@@ -74,15 +74,14 @@
 
 [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp) is compiled without any CPU or GPU
 acceleration.
 
 In the future, I'd like to distribute builds with
 [Core ML support](https://github.com/ggerganov/whisper.cpp?tab=readme-ov-file#core-ml-support),
 [CUDA support](https://github.com/ggerganov/whisper.cpp?tab=readme-ov-file#nvidia-gpu-support), and
-more, given [`whisper.cpp`](https://github.com/ggerganov/whisper.cpp)'s own support for these
-features.
+more, given `whisper.cpp`'s own support for these features.
 
 The latest release compiles against [`v1.5.5`](https://github.com/ggerganov/whisper.cpp/releases/tag/v1.5.5).
 
 ## License
 
 MIT
```

