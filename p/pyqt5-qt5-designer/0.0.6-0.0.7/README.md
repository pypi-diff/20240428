# Comparing `tmp/pyqt5_qt5_designer-0.0.6.tar.gz` & `tmp/pyqt5_qt5_designer-0.0.7.tar.gz`

## Comparing `pyqt5_qt5_designer-0.0.6.tar` & `pyqt5_qt5_designer-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0  1895920 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/bin/Qt5DesignerComponents.dll
--rw-r--r--   0        0        0   562672 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/bin/designer.exe
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/bin/qt.conf
--rw-r--r--   0        0        0   139157 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/translations/designer_ar.qm
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/translations/designer_en.qm
--rw-r--r--   0        0        0   154036 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/translations/designer_fr.qm
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/pyqt5_qt5_designer/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/pyqt5_qt5_designer/__init__.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/src/pyqt5_qt5_designer/designer_runner.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/README.md
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0  1895920 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/bin/Qt5DesignerComponents.dll
+-rw-r--r--   0        0        0   562672 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/bin/designer.exe
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/bin/qt.conf
+-rw-r--r--   0        0        0   139157 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/translations/designer_ar.qm
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/translations/designer_en.qm
+-rw-r--r--   0        0        0   154036 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/translations/designer_fr.qm
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/pyqt5_qt5_designer/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/pyqt5_qt5_designer/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/src/pyqt5_qt5_designer/designer_runner.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/README.md
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pyqt5_qt5_designer-0.0.7/PKG-INFO
```

### Comparing `pyqt5_qt5_designer-0.0.6/.github/workflows/python-publish.yml` & `pyqt5_qt5_designer-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/bin/Qt5DesignerComponents.dll` & `pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/bin/Qt5DesignerComponents.dll`

 * *Files identical despite different names*

### Comparing `pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/bin/designer.exe` & `pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/bin/designer.exe`

 * *Files identical despite different names*

### Comparing `pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/translations/designer_ar.qm` & `pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/translations/designer_ar.qm`

 * *Files identical despite different names*

### Comparing `pyqt5_qt5_designer-0.0.6/src/PyQt5/Qt5/translations/designer_fr.qm` & `pyqt5_qt5_designer-0.0.7/src/PyQt5/Qt5/translations/designer_fr.qm`

 * *Files identical despite different names*

### Comparing `pyqt5_qt5_designer-0.0.6/LICENSE.txt` & `pyqt5_qt5_designer-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyqt5_qt5_designer-0.0.6/README.md` & `pyqt5_qt5_designer-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyqt5_qt5_designer-0.0.6/pyproject.toml` & `pyqt5_qt5_designer-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyqt5_qt5_designer-0.0.6/PKG-INFO` & `pyqt5_qt5_designer-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyqt5_qt5_designer
-Version: 0.0.6
+Version: 0.0.7
 Project-URL: Documentation, https://github.com/selmen2004/pyqt5_qt5_designer#readme
 Project-URL: Issues, https://github.com/selmen2004/pyqt5_qt5_designer/issues
 Project-URL: Source, https://github.com/selmen2004/pyqt5_qt5_designer
 Author-email: Selmen Arous <selmen.arous@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

