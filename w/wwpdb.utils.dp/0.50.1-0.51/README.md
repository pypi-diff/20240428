# Comparing `tmp/wwpdb.utils.dp-0.50.1.tar.gz` & `tmp/wwpdb_utils_dp-0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.dp-0.50.1.tar", last modified: Sun Mar 31 11:52:41 2024, max compression
+gzip compressed data, was "wwpdb_utils_dp-0.51.tar", last modified: Sun Apr 28 10:15:06 2024, max compression
```

## Comparing `wwpdb.utils.dp-0.50.1.tar` & `wwpdb_utils_dp-0.51.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 11:52:41.731567 wwpdb.utils.dp-0.50.1/
--rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)      983 2024-03-31 11:52:41.731567 wwpdb.utils.dp-0.50.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-03-31 11:52:41.735567 wwpdb.utils.dp-0.50.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2125 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 11:52:41.727567 wwpdb.utils.dp-0.50.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 11:52:41.731567 wwpdb.utils.dp-0.50.1/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 11:52:41.731567 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/
--rw-r--r--   0 vsts      (1001) docker     (127)     5395 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/CentreOfMass.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11569 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/DataFileAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2358 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/DensityWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/DepositorSyncUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1918 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/PdbxChemShiftReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2694 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/PdbxMergeCategory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/PdbxSFMapCoefficients.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/PdbxStripCategory.py
--rw-r--r--   0 vsts      (1001) docker     (127)   211544 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/RcsbDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17219 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/RunRemote.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4429 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/ValidationWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 11:52:41.731567 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/electron_density/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/electron_density/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3930 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/electron_density/common_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/electron_density/em_density_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10363 2024-03-31 11:51:50.000000 wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/electron_density/x_ray_density_map.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 11:52:41.731567 wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      983 2024-03-31 11:52:41.000000 wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      934 2024-03-31 11:52:41.000000 wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-31 11:52:41.000000 wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-31 11:52:30.000000 wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-03-31 11:52:41.000000 wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-03-31 11:52:41.000000 wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/
+-rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2215 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.758348 wwpdb_utils_dp-0.51/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.762348 wwpdb_utils_dp-0.51/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/wwpdb/utils/dp/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5395 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/CentreOfMass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11569 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/DataFileAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2358 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/DensityWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/DepositorSyncUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1918 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxChemShiftReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2694 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxMergeCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5366 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxModelComplexity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxSFMapCoefficients.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxStripCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   212032 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/RcsbDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17219 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/RunRemote.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4429 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/ValidationWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3930 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/common_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/em_density_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10363 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/x_ray_density_map.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-28 10:14:52.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.dp-0.50.1/LICENSE` & `wwpdb_utils_dp-0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/PKG-INFO` & `wwpdb_utils_dp-0.51/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.50.1
+Version: 0.51
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
-Requires-Dist: future
 Requires-Dist: mmcif~=0.18
 Requires-Dist: wwpdb.utils.config>=0.34
 Requires-Dist: wwpdb.io
 Requires-Dist: gemmi>=0.4
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
```

### Comparing `wwpdb.utils.dp-0.50.1/setup.py` & `wwpdb_utils_dp-0.51/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,20 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     entry_points={"console_scripts": []},
     #
-    install_requires=["future", "mmcif ~= 0.18", "wwpdb.utils.config >= 0.34", "wwpdb.io", "gemmi >= 0.4"],
+    install_requires=[
+        "mmcif ~= 0.18",
+        "wwpdb.utils.config >= 0.34",
+        "wwpdb.io",
+        "gemmi >= 0.4",
+    ],
     packages=find_packages(exclude=["wwpdb.mock-data", "wwpdb.utils.tests-dp", "tests.*"]),
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         "": ["*.md", "*.rst", "*.txt", "*.cfg"],
     },
     #
     # These basic tests require no database services -
@@ -54,11 +59,17 @@
     #
     # Not configured ...
     extras_require={
         "dev": ["check-manifest"],
         "test": ["coverage"],
     },
     # Added for
-    command_options={"build_sphinx": {"project": ("setup.py", thisPackage), "version": ("setup.py", version), "release": ("setup.py", version)}},
+    command_options={
+        "build_sphinx": {
+            "project": ("setup.py", thisPackage),
+            "version": ("setup.py", version),
+            "release": ("setup.py", version),
+        }
+    },
     # This setting for namespace package support -
     zip_safe=False,
 )
```

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/CentreOfMass.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/CentreOfMass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/DataFileAdapter.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/DataFileAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/DensityWrapper.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/DensityWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/DepositorSyncUtil.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/DepositorSyncUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/PdbxChemShiftReport.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxChemShiftReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/PdbxMergeCategory.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxMergeCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/PdbxSFMapCoefficients.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxSFMapCoefficients.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/PdbxStripCategory.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxStripCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/RcsbDpUtility.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/RcsbDpUtility.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,29 +356,30 @@
             "annot-get-close-contact",
             "annot-convert-close-contact-to-link",
             "annot-get-covalent-bond",
             "annot-remove-covalent-bond",
             "em-density-bcif",
             "xray-density-bcif",
             "centre-of-mass",
+            "annot-complexity",
         ]
 
         self.__sequenceOps = ["seq-blastp", "seq-blastn", "fetch-uniprot", "fetch-gb", "format-uniprot", "format-gb", "backup-seqdb"]
         self.__validateOps = ["validate-geometry"]
         self.__dbOps = ["db-loader", "sync-depositors"]
         self.__emOps = [
             "mapfix-big",
             "em2em-spider",
             "fsc_check",
             "img-convert",
             "annot-read-map-header",
             "annot-read-map-header-in-place",
             "annot-update-map-header-in-place",
             "deposit-update-map-header-in-place",
-            "em-map-model-upload-check"
+            "em-map-model-upload-check",
         ]
 
         #
 
         # Source, destination and logfile path details
         #
         self.__srcPath = None
@@ -1463,14 +1464,24 @@
             cmd_args = ["--model-file-in {}".format(iPath), "--model-file-out {}".format(oPath)]
 
             cmd += "; {}".format(self.__site_config_command)
 
             cmd += " ; python -m wwpdb.utils.dp.CentreOfMass {}".format(" ".join(cmd_args))
             cmd += " > " + tPath + " 2>&1 ; cat " + tPath + " >> " + lPath
 
+        elif op == "annot-complexity":
+            cmd_path = "python -m wwpdb.utils.dp.PdbxModelComplexity"
+
+            cmd += "; " + cmd_path + " --model " + iPath + " --output " + oPath
+
+            if "threshold" in self.__inputParamDict:
+                cmd += " --threshold " + self.__inputParamDict["threshold"]
+
+            cmd += " > " + tPath + " 2>&1 ; cat " + tPath + " >> " + lPath
+
         elif op == "annot-dcc-report":
             # The sf-valid package is currently set to self configure in a wrapper
             # shell script.  PACKAGE_DIR and TOOLS_DIR only need to be set here.
             #
             cmd += " ; WWPDB_SITE_ID=" + self.__siteId + " ; export WWPDB_SITE_ID "
             cmd += " ; DEPLOY_DIR=" + self.__deployPath + " ; export DEPLOY_DIR "
             cmd += " ; TOOLS_DIR=" + os.path.join(self.__localAppsPath, "bin") + " ; export TOOLS_DIR "
@@ -2846,16 +2857,21 @@
                 if os.access(outFile, os.F_OK):
                     self.__resultPathList.append(outFile)
                 else:
                     self.__resultPathList.append("missing")
                 #
             #
 
-        elif (op == "annot-cif-to-public-pdbx") or (op == "annot-cif-to-pdbx-em-header") or (op == "annot-misc-checking") or \
-             (op == "annot-get-pdb-file") or (op == "annot-add-version-info"):
+        elif (
+            (op == "annot-cif-to-public-pdbx")
+            or (op == "annot-cif-to-pdbx-em-header")
+            or (op == "annot-misc-checking")
+            or (op == "annot-get-pdb-file")
+            or (op == "annot-add-version-info")
+        ):
             for fileName in (oPath, tPath, lPath):
                 outFile = os.path.join(self.__wrkPath, fileName)
                 if os.access(outFile, os.F_OK):
                     self.__resultPathList.append(outFile)
                 else:
                     self.__resultPathList.append("missing")
                 #
@@ -3423,15 +3439,15 @@
             "mapfix-big",
             "fsc_check",
             "img-convert",
             "annot-read-map-header",
             "annot-read-map-header-in-place",
             "annot-update-map-header-in-place",
             "deposit-update-map-header-in-place",
-            "em-map-model-upload-check"
+            "em-map-model-upload-check",
         ):
             return -1
         #
 
         if self.__debug:
             logger.info("+RcsbDpUtility._emStep()  - Application string:\n%s\n", cmd)
```

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/RunRemote.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/RunRemote.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/ValidationWrapper.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/ValidationWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/electron_density/common_functions.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/common_functions.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/electron_density/em_density_map.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/em_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb/utils/dp/electron_density/x_ray_density_map.py` & `wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/x_ray_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/PKG-INFO` & `wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.50.1
+Version: 0.51
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
-Requires-Dist: future
 Requires-Dist: mmcif~=0.18
 Requires-Dist: wwpdb.utils.config>=0.34
 Requires-Dist: wwpdb.io
 Requires-Dist: gemmi>=0.4
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
```

### Comparing `wwpdb.utils.dp-0.50.1/wwpdb.utils.dp.egg-info/SOURCES.txt` & `wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 wwpdb/utils/__init__.py
 wwpdb/utils/dp/CentreOfMass.py
 wwpdb/utils/dp/DataFileAdapter.py
 wwpdb/utils/dp/DensityWrapper.py
 wwpdb/utils/dp/DepositorSyncUtil.py
 wwpdb/utils/dp/PdbxChemShiftReport.py
 wwpdb/utils/dp/PdbxMergeCategory.py
+wwpdb/utils/dp/PdbxModelComplexity.py
 wwpdb/utils/dp/PdbxSFMapCoefficients.py
 wwpdb/utils/dp/PdbxStripCategory.py
 wwpdb/utils/dp/RcsbDpUtility.py
 wwpdb/utils/dp/RunRemote.py
 wwpdb/utils/dp/ValidationWrapper.py
 wwpdb/utils/dp/__init__.py
 wwpdb/utils/dp/electron_density/__init__.py
```

