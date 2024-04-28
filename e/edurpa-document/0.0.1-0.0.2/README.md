# Comparing `tmp/edurpa_document-0.0.1-py3-none-any.whl.zip` & `tmp/edurpa_document-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6007 bytes, number of entries: 9
+Zip file size: 6010 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-28 06:21 EduRPA/__init__.py
 -rw-rw-rw-  2.0 fat     4817 b- defN 24-Apr-28 06:18 EduRPA/Document/DocumentAutomation.py
 -rw-rw-rw-  2.0 fat      428 b- defN 24-Apr-28 06:21 EduRPA/Document/__init__.py
 -rw-rw-rw-  2.0 fat     2624 b- defN 24-Apr-28 06:18 EduRPA/Document/transform.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-Apr-28 06:32 edurpa_document-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2017 b- defN 24-Apr-28 06:32 edurpa_document-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 06:32 edurpa_document-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-28 06:32 edurpa_document-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      760 b- defN 24-Apr-28 06:32 edurpa_document-0.0.1.dist-info/RECORD
-9 files, 11848 bytes uncompressed, 4683 bytes compressed:  60.5%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-Apr-28 06:51 edurpa_document-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2019 b- defN 24-Apr-28 06:51 edurpa_document-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 06:51 edurpa_document-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-28 06:51 edurpa_document-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      760 b- defN 24-Apr-28 06:51 edurpa_document-0.0.2.dist-info/RECORD
+9 files, 11850 bytes uncompressed, 4686 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: EduRPA/Document/__init__.py
 Comment: 
 
 Filename: EduRPA/Document/transform.py
 Comment: 
 
-Filename: edurpa_document-0.0.1.dist-info/LICENSE
+Filename: edurpa_document-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_document-0.0.1.dist-info/METADATA
+Filename: edurpa_document-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_document-0.0.1.dist-info/WHEEL
+Filename: edurpa_document-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_document-0.0.1.dist-info/top_level.txt
+Filename: edurpa_document-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_document-0.0.1.dist-info/RECORD
+Filename: edurpa_document-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `edurpa_document-0.0.1.dist-info/LICENSE` & `edurpa_document-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_document-0.0.1.dist-info/METADATA` & `edurpa_document-0.0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-document
-Version: 0.0.1
+Version: 0.0.2
 Summary: education librabry for RPA
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,22 +36,22 @@
 Requires-Dist: prefetch-generator (==1.0.1)
 Requires-Dist: pyparsing (==3.1.1)
 Requires-Dist: PySocks (==1.7.1)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: robotframework (==6.1.1)
 Requires-Dist: scikit-image (==0.22.0)
-Requires-Dist: scipy (==1.4.1)
-Requires-Dist: shapely (==1.8.0)
+Requires-Dist: scipy (==1.11.4)
+Requires-Dist: shapely (==2.0.2)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: soupsieve (==2.5)
 Requires-Dist: tifffile (==2023.9.26)
 Requires-Dist: tqdm (==4.66.1)
 Requires-Dist: vietocr (==0.3.12)
-Requires-Dist: zipp (==3.5.0)
+Requires-Dist: zipp (==3.17.0)
 
 # EduRPA
 EduRPA is an robotframework librabry that support feature in education field
 
 # Pytorch and Anaconda environment
 This librabry need install pytorch asa dependency and due to the size, it should
 be installed later
```

## Comparing `edurpa_document-0.0.1.dist-info/RECORD` & `edurpa_document-0.0.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 EduRPA/__init__.py,sha256=h_8fnSBqTgA6QcTez7ro5lyaDZLhOqwBaotn0s9wfrY,15
 EduRPA/Document/DocumentAutomation.py,sha256=pb1J06G6cPWAJAebYEY3j9mY02FSqQaVZOyWKUkFrtk,4817
 EduRPA/Document/__init__.py,sha256=3b1yzf2k9Pd0QwikmByQnRPYOkkOecVrDkg2n2kVLqs,428
 EduRPA/Document/transform.py,sha256=TRL-dYUvUJcGS9h_pph3fm_-02dQfzh0pGMoVN3T7wY,2624
-edurpa_document-0.0.1.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
-edurpa_document-0.0.1.dist-info/METADATA,sha256=H0_Hc2kONybC15rTYJAiWw4K0iUH3kT32F7IJ8oUCQE,2017
-edurpa_document-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-edurpa_document-0.0.1.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
-edurpa_document-0.0.1.dist-info/RECORD,,
+edurpa_document-0.0.2.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
+edurpa_document-0.0.2.dist-info/METADATA,sha256=8bpjMEiolDwkscdQQMx7t8D_lC8M7xEqZqgOJUHRchs,2019
+edurpa_document-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+edurpa_document-0.0.2.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
+edurpa_document-0.0.2.dist-info/RECORD,,
```

