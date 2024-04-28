# Comparing `tmp/geopandas-0.9.0.tar.gz` & `tmp/geopandas-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopandas-0.9.0.tar", last modified: Sun Feb 28 21:10:40 2021, max compression
+gzip compressed data, was "geopandas-1.0.0a1.tar", last modified: Sat Apr 13 20:59:23 2024, max compression
```

## Comparing `geopandas-0.9.0.tar` & `geopandas-1.0.0a1.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1504 2021-02-28 21:10:37.000000 geopandas-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       72 2021-02-28 21:10:37.000000 geopandas-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      890 2021-02-28 21:10:40.387239 geopandas-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6296 2021-02-28 21:10:37.000000 geopandas-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.391239 geopandas-0.9.0/geopandas/
--rw-r--r--   0 runner    (1001) docker     (116)      969 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6385 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     4083 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    27301 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (116)      471 2021-02-28 21:10:40.391239 geopandas-0.9.0/geopandas/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)    43316 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/array.py
--rw-r--r--   0 runner    (1001) docker     (116)   111554 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/base.py
--rw-r--r--   0 runner    (1001) docker     (116)      694 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)     1161 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/
--rw-r--r--   0 runner    (1001) docker     (116)    32111 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.README.html
--rw-r--r--   0 runner    (1001) docker     (116)        5 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.cpg
--rw-r--r--   0 runner    (1001) docker     (116)    16427 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.dbf
--rw-r--r--   0 runner    (1001) docker     (116)      143 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.prj
--rw-r--r--   0 runner    (1001) docker     (116)     5756 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.shp
--rw-r--r--   0 runner    (1001) docker     (116)     1716 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_cities/naturalearth_cities.shx
--rw-r--r--   0 runner    (1001) docker     (116)      736 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.cpg
--rw-r--r--   0 runner    (1001) docker     (116)    48869 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.dbf
--rw-r--r--   0 runner    (1001) docker     (116)      143 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.prj
--rw-r--r--   0 runner    (1001) docker     (116)   180924 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shp
--rw-r--r--   0 runner    (1001) docker     (116)     1516 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/naturalearth_lowres/naturalearth_lowres.shx
--rw-r--r--   0 runner    (1001) docker     (116)   661032 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/datasets/nybb_16a.zip
--rw-r--r--   0 runner    (1001) docker     (116)    64184 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/geodataframe.py
--rw-r--r--   0 runner    (1001) docker     (116)    40294 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/geoseries.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas/io/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14773 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/io/arrow.py
--rw-r--r--   0 runner    (1001) docker     (116)    13697 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/io/file.py
--rw-r--r--   0 runner    (1001) docker     (116)    14124 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/io/sql.py
--rw-r--r--   0 runner    (1001) docker     (116)    36526 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/plotting.py
--rw-r--r--   0 runner    (1001) docker     (116)    21858 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/sindex.py
--rw-r--r--   0 runner    (1001) docker     (116)     9486 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/geopandas/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/geopandas/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)      506 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/data/null_geom.geojson
--rw-r--r--   0 runner    (1001) docker     (116)     1153 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    26836 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)      781 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    21680 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (116)      312 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)     9283 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_dissolve.py
--rw-r--r--   0 runner    (1001) docker     (116)    15258 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_extension_array.py
--rw-r--r--   0 runner    (1001) docker     (116)     5410 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_geocode.py
--rw-r--r--   0 runner    (1001) docker     (116)    35283 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_geodataframe.py
--rw-r--r--   0 runner    (1001) docker     (116)    37334 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_geom_methods.py
--rw-r--r--   0 runner    (1001) docker     (116)    16325 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_geoseries.py
--rw-r--r--   0 runner    (1001) docker     (116)     2105 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (116)    20148 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_overlay.py
--rw-r--r--   0 runner    (1001) docker     (116)    17336 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_pandas_methods.py
--rw-r--r--   0 runner    (1001) docker     (116)    64812 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1171 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)    27341 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_sindex.py
--rw-r--r--   0 runner    (1001) docker     (116)     3774 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (116)     2504 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     4235 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/geopandas/tools/
--rw-r--r--   0 runner    (1001) docker     (116)      329 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3307 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (116)     8098 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/clip.py
--rw-r--r--   0 runner    (1001) docker     (116)     1489 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/crs.py
--rw-r--r--   0 runner    (1001) docker     (116)     5897 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/geocoding.py
--rw-r--r--   0 runner    (1001) docker     (116)    13373 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/overlay.py
--rw-r--r--   0 runner    (1001) docker     (116)    11220 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/sjoin.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.387239 geopandas-0.9.0/geopandas/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14652 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (116)    18421 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/tests/test_sjoin.py
--rw-r--r--   0 runner    (1001) docker     (116)     2954 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     1454 2021-02-28 21:10:37.000000 geopandas-0.9.0/geopandas/tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-28 21:10:40.383239 geopandas-0.9.0/geopandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      890 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2584 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       53 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-28 21:10:40.000000 geopandas-0.9.0/geopandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      562 2021-02-28 21:10:40.387239 geopandas-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1993 2021-02-28 21:10:37.000000 geopandas-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)    65747 2021-02-28 21:10:37.000000 geopandas-0.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.768060 geopandas-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-13 20:59:23.768060 geopandas-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.756060 geopandas-1.0.0a1/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-13 20:59:23.768060 geopandas-1.0.0a1/geopandas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58152 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)   184675 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.756060 geopandas-1.0.0a1/geopandas/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36190 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96232 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/geodataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/geoseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.756060 geopandas-1.0.0a1/geopandas/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/_pyarrow_hotfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23840 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30174 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14263 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.760060 geopandas-1.0.0a1/geopandas/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/tests/generate_legacy_storage_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30069 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/tests/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45665 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/tests/test_file_geom_types_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/tests/test_infer_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27726 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/io/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33153 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/sindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.764060 geopandas-1.0.0a1/geopandas/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.764060 geopandas-1.0.0a1/geopandas/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/data/null_geom.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29327 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26001 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_dissolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36072 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_extension_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_geocode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57994 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_geodataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69789 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_geom_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26707 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_geoseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_op_output_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29668 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28134 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_pandas_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72914 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35054 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_sindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.764060 geopandas-1.0.0a1/geopandas/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/hilbert_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22519 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/sjoin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.768060 geopandas-1.0.0a1/geopandas/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17240 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/tests/test_hilbert_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45623 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/tests/test_sjoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/geopandas/tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:59:23.768060 geopandas-1.0.0a1/geopandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-13 20:59:23.000000 geopandas-1.0.0a1/geopandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-13 20:59:23.000000 geopandas-1.0.0a1/geopandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 20:59:23.000000 geopandas-1.0.0a1/geopandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 20:59:23.000000 geopandas-1.0.0a1/geopandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 20:59:23.000000 geopandas-1.0.0a1/geopandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-13 20:59:23.768060 geopandas-1.0.0a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86854 2024-04-13 20:59:13.000000 geopandas-1.0.0a1/versioneer.py
```

### Comparing `geopandas-0.9.0/LICENSE.txt` & `geopandas-1.0.0a1/LICENSE.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2013-2016, GeoPandas developers.
+Copyright (c) 2013-2022, GeoPandas developers.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
  * Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
  * Redistributions in binary form must reproduce the above copyright notice,
    this list of conditions and the following disclaimer in the documentation
    and/or other materials provided with the distribution.
- * Neither the name of Enthought, Inc. nor the names of its contributors may
+ * Neither the name of GeoPandas nor the names of its contributors may
    be used to endorse or promote products derived from this software without
    specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
```

### Comparing `geopandas-0.9.0/README.md` & `geopandas-1.0.0a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,394 +1,450 @@
-00000000: 4765 6f50 616e 6461 7320 5b21 5b41 6374  GeoPandas [![Act
-00000010: 696f 6e73 2053 7461 7475 735d 2868 7474  ions Status](htt
-00000020: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000030: 6765 6f70 616e 6461 732f 6765 6f70 616e  geopandas/geopan
-00000040: 6461 732f 776f 726b 666c 6f77 732f 5465  das/workflows/Te
-00000050: 7374 732f 6261 6467 652e 7376 6729 5d28  sts/badge.svg)](
-00000060: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000070: 6f6d 2f67 656f 7061 6e64 6173 2f67 656f  om/geopandas/geo
-00000080: 7061 6e64 6173 2f61 6374 696f 6e73 3f71  pandas/actions?q
-00000090: 7565 7279 3d77 6f72 6b66 6c6f 7725 3341  uery=workflow%3A
-000000a0: 5465 7374 7329 205b 215b 436f 7665 7261  Tests) [![Covera
-000000b0: 6765 2053 7461 7475 735d 2868 7474 7073  ge Status](https
-000000c0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-000000d0: 2f67 656f 7061 6e64 6173 2f67 656f 7061  /geopandas/geopa
-000000e0: 6e64 6173 2f62 7261 6e63 682f 6d61 7374  ndas/branch/mast
-000000f0: 6572 2f67 7261 7068 2f62 6164 6765 2e73  er/graph/badge.s
-00000100: 7667 295d 2868 7474 7073 3a2f 2f63 6f64  vg)](https://cod
-00000110: 6563 6f76 2e69 6f2f 6768 2f67 656f 7061  ecov.io/gh/geopa
-00000120: 6e64 6173 2f67 656f 7061 6e64 6173 2920  ndas/geopandas) 
-00000130: 5b21 5b4a 6f69 6e20 7468 6520 6368 6174  [![Join the chat
-00000140: 2061 7420 6874 7470 733a 2f2f 6769 7474   at https://gitt
-00000150: 6572 2e69 6d2f 6765 6f70 616e 6461 732f  er.im/geopandas/
-00000160: 6765 6f70 616e 6461 735d 2868 7474 7073  geopandas](https
-00000170: 3a2f 2f62 6164 6765 732e 6769 7474 6572  ://badges.gitter
-00000180: 2e69 6d2f 4a6f 696e 2532 3043 6861 742e  .im/Join%20Chat.
-00000190: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
-000001a0: 7474 6572 2e69 6d2f 6765 6f70 616e 6461  tter.im/geopanda
-000001b0: 732f 6765 6f70 616e 6461 733f 7574 6d5f  s/geopandas?utm_
-000001c0: 736f 7572 6365 3d62 6164 6765 2675 746d  source=badge&utm
-000001d0: 5f6d 6564 6975 6d3d 6261 6467 6526 7574  _medium=badge&ut
-000001e0: 6d5f 6361 6d70 6169 676e 3d70 722d 6261  m_campaign=pr-ba
-000001f0: 6467 6526 7574 6d5f 636f 6e74 656e 743d  dge&utm_content=
-00000200: 6261 6467 6529 205b 215b 4269 6e64 6572  badge) [![Binder
-00000210: 5d28 6874 7470 733a 2f2f 6d79 6269 6e64  ](https://mybind
-00000220: 6572 2e6f 7267 2f62 6164 6765 2e73 7667  er.org/badge.svg
-00000230: 295d 2868 7474 7073 3a2f 2f6d 7962 696e  )](https://mybin
-00000240: 6465 722e 6f72 672f 7632 2f67 682f 6765  der.org/v2/gh/ge
-00000250: 6f70 616e 6461 732f 6765 6f70 616e 6461  opandas/geopanda
-00000260: 732f 6d61 7374 6572 2920 5b21 5b44 4f49  s/master) [![DOI
-00000270: 5d28 6874 7470 733a 2f2f 7a65 6e6f 646f  ](https://zenodo
-00000280: 2e6f 7267 2f62 6164 6765 2f31 3130 3032  .org/badge/11002
-00000290: 3831 352e 7376 6729 5d28 6874 7470 733a  815.svg)](https:
-000002a0: 2f2f 7a65 6e6f 646f 2e6f 7267 2f62 6164  //zenodo.org/bad
-000002b0: 6765 2f6c 6174 6573 7464 6f69 2f31 3130  ge/latestdoi/110
-000002c0: 3032 3831 3529 0a3d 3d3d 3d3d 3d3d 3d3d  02815).=========
-000002d0: 0a0a 5079 7468 6f6e 2074 6f6f 6c73 2066  ..Python tools f
-000002e0: 6f72 2067 656f 6772 6170 6869 6320 6461  or geographic da
-000002f0: 7461 0a0a 496e 7472 6f64 7563 7469 6f6e  ta..Introduction
-00000300: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a47  .------------..G
-00000310: 656f 5061 6e64 6173 2069 7320 6120 7072  eoPandas is a pr
-00000320: 6f6a 6563 7420 746f 2061 6464 2073 7570  oject to add sup
-00000330: 706f 7274 2066 6f72 2067 656f 6772 6170  port for geograp
-00000340: 6869 6320 6461 7461 2074 6f0a 5b70 616e  hic data to.[pan
-00000350: 6461 735d 2868 7474 703a 2f2f 7061 6e64  das](http://pand
-00000360: 6173 2e70 7964 6174 612e 6f72 6729 206f  as.pydata.org) o
-00000370: 626a 6563 7473 2e20 2049 7420 6375 7272  bjects.  It curr
-00000380: 656e 746c 7920 696d 706c 656d 656e 7473  ently implements
-00000390: 0a60 4765 6f53 6572 6965 7360 2061 6e64  .`GeoSeries` and
-000003a0: 2060 4765 6f44 6174 6146 7261 6d65 6020   `GeoDataFrame` 
-000003b0: 7479 7065 7320 7768 6963 6820 6172 6520  types which are 
-000003c0: 7375 6263 6c61 7373 6573 206f 660a 6070  subclasses of.`p
-000003d0: 616e 6461 732e 5365 7269 6573 6020 616e  andas.Series` an
-000003e0: 6420 6070 616e 6461 732e 4461 7461 4672  d `pandas.DataFr
-000003f0: 616d 6560 2072 6573 7065 6374 6976 656c  ame` respectivel
-00000400: 792e 2020 4765 6f50 616e 6461 730a 6f62  y.  GeoPandas.ob
-00000410: 6a65 6374 7320 6361 6e20 6163 7420 6f6e  jects can act on
-00000420: 205b 7368 6170 656c 795d 2868 7474 703a   [shapely](http:
-00000430: 2f2f 7368 6170 656c 792e 7265 6164 7468  //shapely.readth
-00000440: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000450: 7374 2f29 0a67 656f 6d65 7472 7920 6f62  st/).geometry ob
-00000460: 6a65 6374 7320 616e 6420 7065 7266 6f72  jects and perfor
-00000470: 6d20 6765 6f6d 6574 7269 6320 6f70 6572  m geometric oper
-00000480: 6174 696f 6e73 2e0a 0a47 656f 5061 6e64  ations...GeoPand
-00000490: 6173 2067 656f 6d65 7472 7920 6f70 6572  as geometry oper
-000004a0: 6174 696f 6e73 2061 7265 2063 6172 7465  ations are carte
-000004b0: 7369 616e 2e20 2054 6865 2063 6f6f 7264  sian.  The coord
-000004c0: 696e 6174 6520 7265 6665 7265 6e63 650a  inate reference.
-000004d0: 7379 7374 656d 2028 6372 7329 2063 616e  system (crs) can
-000004e0: 2062 6520 7374 6f72 6564 2061 7320 616e   be stored as an
-000004f0: 2061 7474 7269 6275 7465 206f 6e20 616e   attribute on an
-00000500: 206f 626a 6563 742c 2061 6e64 2069 730a   object, and is.
-00000510: 6175 746f 6d61 7469 6361 6c6c 7920 7365  automatically se
-00000520: 7420 7768 656e 206c 6f61 6469 6e67 2066  t when loading f
-00000530: 726f 6d20 6120 6669 6c65 2e20 204f 626a  rom a file.  Obj
-00000540: 6563 7473 206d 6179 2062 650a 7472 616e  ects may be.tran
-00000550: 7366 6f72 6d65 6420 746f 206e 6577 2063  sformed to new c
-00000560: 6f6f 7264 696e 6174 6520 7379 7374 656d  oordinate system
-00000570: 7320 7769 7468 2074 6865 2060 746f 5f63  s with the `to_c
-00000580: 7273 2829 6020 6d65 7468 6f64 2e0a 5468  rs()` method..Th
-00000590: 6572 6520 6973 2063 7572 7265 6e74 6c79  ere is currently
-000005a0: 206e 6f20 656e 666f 7263 656d 656e 7420   no enforcement 
-000005b0: 6f66 206c 696b 6520 636f 6f72 6469 6e61  of like coordina
-000005c0: 7465 7320 666f 7220 6f70 6572 6174 696f  tes for operatio
-000005d0: 6e73 2c0a 6275 7420 7468 6174 206d 6179  ns,.but that may
-000005e0: 2063 6861 6e67 6520 696e 2074 6865 2066   change in the f
-000005f0: 7574 7572 652e 0a0a 446f 6375 6d65 6e74  uture...Document
-00000600: 6174 696f 6e20 6973 2061 7661 696c 6162  ation is availab
-00000610: 6c65 2061 7420 5b67 656f 7061 6e64 6173  le at [geopandas
-00000620: 2e6f 7267 5d28 6874 7470 3a2f 2f67 656f  .org](http://geo
-00000630: 7061 6e64 6173 2e6f 7267 290a 2863 7572  pandas.org).(cur
-00000640: 7265 6e74 2072 656c 6561 7365 2920 616e  rent release) an
-00000650: 640a 5b52 6561 6420 7468 6520 446f 6373  d.[Read the Docs
-00000660: 5d28 6874 7470 3a2f 2f67 656f 7061 6e64  ](http://geopand
-00000670: 6173 2e72 6561 6474 6865 646f 6373 2e69  as.readthedocs.i
-00000680: 6f2f 656e 2f6c 6174 6573 742f 290a 2872  o/en/latest/).(r
-00000690: 656c 6561 7365 2061 6e64 2064 6576 656c  elease and devel
-000006a0: 6f70 6d65 6e74 2076 6572 7369 6f6e 7329  opment versions)
-000006b0: 2e0a 0a49 6e73 7461 6c6c 0a2d 2d2d 2d2d  ...Install.-----
-000006c0: 2d2d 2d0a 0a53 6565 2074 6865 205b 696e  ---..See the [in
-000006d0: 7374 616c 6c61 7469 6f6e 2064 6f63 735d  stallation docs]
-000006e0: 2868 7474 7073 3a2f 2f67 656f 7061 6e64  (https://geopand
-000006f0: 6173 2e72 6561 6474 6865 646f 6373 2e69  as.readthedocs.i
-00000700: 6f2f 656e 2f6c 6174 6573 742f 696e 7374  o/en/latest/inst
-00000710: 616c 6c2e 6874 6d6c 290a 666f 7220 616c  all.html).for al
-00000720: 6c20 6465 7461 696c 732e 2047 656f 5061  l details. GeoPa
-00000730: 6e64 6173 2064 6570 656e 6473 206f 6e20  ndas depends on 
-00000740: 7468 6520 666f 6c6c 6f77 696e 6720 7061  the following pa
-00000750: 636b 6167 6573 3a0a 0a2d 2060 6070 616e  ckages:..- ``pan
-00000760: 6461 7360 600a 2d20 6060 7368 6170 656c  das``.- ``shapel
-00000770: 7960 600a 2d20 6060 6669 6f6e 6160 600a  y``.- ``fiona``.
-00000780: 2d20 6060 7079 7072 6f6a 6060 0a0a 4675  - ``pyproj``..Fu
-00000790: 7274 6865 722c 2060 606d 6174 706c 6f74  rther, ``matplot
-000007a0: 6c69 6260 6020 6973 2061 6e20 6f70 7469  lib`` is an opti
-000007b0: 6f6e 616c 2064 6570 656e 6465 6e63 792c  onal dependency,
-000007c0: 2072 6571 7569 7265 640a 666f 7220 706c   required.for pl
-000007d0: 6f74 7469 6e67 2c20 616e 6420 5b60 6072  otting, and [``r
-000007e0: 7472 6565 6060 5d28 6874 7470 733a 2f2f  tree``](https://
-000007f0: 6769 7468 7562 2e63 6f6d 2f54 6f62 6c65  github.com/Toble
-00000800: 7269 7479 2f72 7472 6565 2920 6973 2061  rity/rtree) is a
-00000810: 6e20 6f70 7469 6f6e 616c 0a64 6570 656e  n optional.depen
-00000820: 6465 6e63 792c 2072 6571 7569 7265 6420  dency, required 
-00000830: 666f 7220 7370 6174 6961 6c20 6a6f 696e  for spatial join
-00000840: 732e 2060 6072 7472 6565 6060 2072 6571  s. ``rtree`` req
-00000850: 7569 7265 7320 7468 6520 4320 6c69 6272  uires the C libr
-00000860: 6172 7920 5b60 606c 6962 7370 6174 6961  ary [``libspatia
-00000870: 6c69 6e64 6578 6060 5d28 6874 7470 733a  lindex``](https:
-00000880: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6962  //github.com/lib
-00000890: 7370 6174 6961 6c69 6e64 6578 2f6c 6962  spatialindex/lib
-000008a0: 7370 6174 6961 6c69 6e64 6578 292e 0a0a  spatialindex)...
-000008b0: 5468 6f73 6520 7061 636b 6167 6573 2064  Those packages d
-000008c0: 6570 656e 6420 6f6e 2073 6576 6572 616c  epend on several
-000008d0: 206c 6f77 2d6c 6576 656c 206c 6962 7261   low-level libra
-000008e0: 7269 6573 2066 6f72 2067 656f 7370 6174  ries for geospat
-000008f0: 6961 6c20 616e 616c 7973 6973 2c20 7768  ial analysis, wh
-00000900: 6963 6820 6361 6e20 6265 2061 2063 6861  ich can be a cha
-00000910: 6c6c 656e 6765 2074 6f20 696e 7374 616c  llenge to instal
-00000920: 6c2e 2054 6865 7265 666f 7265 2c20 7765  l. Therefore, we
-00000930: 2072 6563 6f6d 6d65 6e64 2074 6f20 696e   recommend to in
-00000940: 7374 616c 6c20 4765 6f50 616e 6461 7320  stall GeoPandas 
-00000950: 7573 696e 6720 7468 6520 5b63 6f6e 6461  using the [conda
-00000960: 2070 6163 6b61 6765 206d 616e 6167 6572   package manager
-00000970: 5d28 6874 7470 733a 2f2f 636f 6e64 612e  ](https://conda.
-00000980: 696f 2f65 6e2f 6c61 7465 7374 2f29 2e20  io/en/latest/). 
-00000990: 5365 6520 7468 6520 5b69 6e73 7461 6c6c  See the [install
-000009a0: 6174 696f 6e20 646f 6373 5d28 6874 7470  ation docs](http
-000009b0: 733a 2f2f 6765 6f70 616e 6461 732e 7265  s://geopandas.re
-000009c0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-000009d0: 6c61 7465 7374 2f69 6e73 7461 6c6c 2e68  latest/install.h
-000009e0: 746d 6c29 2066 6f72 206d 6f72 6520 6465  tml) for more de
-000009f0: 7461 696c 732e 0a0a 0a47 6574 2069 6e20  tails....Get in 
-00000a00: 746f 7563 680a 2d2d 2d2d 2d2d 2d2d 2d2d  touch.----------
-00000a10: 2d2d 0a0a 2d20 4173 6b20 7573 6167 6520  --..- Ask usage 
-00000a20: 7175 6573 7469 6f6e 7320 2822 486f 7720  questions ("How 
-00000a30: 646f 2049 3f22 2920 6f6e 205b 5374 6163  do I?") on [Stac
-00000a40: 6b4f 7665 7266 6c6f 775d 2868 7474 7073  kOverflow](https
-00000a50: 3a2f 2f73 7461 636b 6f76 6572 666c 6f77  ://stackoverflow
-00000a60: 2e63 6f6d 2f71 7565 7374 696f 6e73 2f74  .com/questions/t
-00000a70: 6167 6765 642f 6765 6f70 616e 6461 7329  agged/geopandas)
-00000a80: 206f 7220 5b47 4953 2053 7461 636b 4578   or [GIS StackEx
-00000a90: 6368 616e 6765 5d28 6874 7470 733a 2f2f  change](https://
-00000aa0: 6769 732e 7374 6163 6b65 7863 6861 6e67  gis.stackexchang
-00000ab0: 652e 636f 6d2f 7175 6573 7469 6f6e 732f  e.com/questions/
-00000ac0: 7461 6767 6564 2f67 656f 7061 6e64 6173  tagged/geopandas
-00000ad0: 292e 0a2d 2052 6570 6f72 7420 6275 6773  )..- Report bugs
-00000ae0: 2c20 7375 6767 6573 7420 6665 6174 7572  , suggest featur
-00000af0: 6573 206f 7220 7669 6577 2074 6865 2073  es or view the s
-00000b00: 6f75 7263 6520 636f 6465 205b 6f6e 2047  ource code [on G
-00000b10: 6974 4875 625d 2868 7474 7073 3a2f 2f67  itHub](https://g
-00000b20: 6974 6875 622e 636f 6d2f 6765 6f70 616e  ithub.com/geopan
-00000b30: 6461 732f 6765 6f70 616e 6461 7329 2e0a  das/geopandas)..
-00000b40: 2d20 466f 7220 6120 7175 6963 6b20 7175  - For a quick qu
-00000b50: 6573 7469 6f6e 2061 626f 7574 2061 2062  estion about a b
-00000b60: 7567 2072 6570 6f72 7420 6f72 2066 6561  ug report or fea
-00000b70: 7475 7265 2072 6571 7565 7374 2c20 6f72  ture request, or
-00000b80: 2050 756c 6c20 5265 7175 6573 742c 2068   Pull Request, h
-00000b90: 6561 6420 6f76 6572 2074 6f20 7468 6520  ead over to the 
-00000ba0: 5b67 6974 7465 7220 6368 616e 6e65 6c5d  [gitter channel]
-00000bb0: 2868 7474 7073 3a2f 2f67 6974 7465 722e  (https://gitter.
-00000bc0: 696d 2f67 656f 7061 6e64 6173 2f67 656f  im/geopandas/geo
-00000bd0: 7061 6e64 6173 292e 0a2d 2046 6f72 206c  pandas)..- For l
-00000be0: 6573 7320 7765 6c6c 2064 6566 696e 6564  ess well defined
-00000bf0: 2071 7565 7374 696f 6e73 206f 7220 6964   questions or id
-00000c00: 6561 732c 206f 7220 746f 2061 6e6e 6f75  eas, or to annou
-00000c10: 6e63 6520 6f74 6865 7220 7072 6f6a 6563  nce other projec
-00000c20: 7473 206f 6620 696e 7465 7265 7374 2074  ts of interest t
-00000c30: 6f20 4765 6f50 616e 6461 7320 7573 6572  o GeoPandas user
-00000c40: 732c 202e 2e2e 2075 7365 2074 6865 205b  s, ... use the [
-00000c50: 6d61 696c 696e 6720 6c69 7374 5d28 6874  mailing list](ht
-00000c60: 7470 733a 2f2f 6772 6f75 7073 2e67 6f6f  tps://groups.goo
-00000c70: 676c 652e 636f 6d2f 666f 7275 6d2f 2321  gle.com/forum/#!
-00000c80: 666f 7275 6d2f 6765 6f70 616e 6461 7329  forum/geopandas)
-00000c90: 2e0a 0a0a 4578 616d 706c 6573 0a2d 2d2d  ....Examples.---
-00000ca0: 2d2d 2d2d 2d0a 0a20 2020 203e 3e3e 2069  -----..    >>> i
-00000cb0: 6d70 6f72 7420 6765 6f70 616e 6461 730a  mport geopandas.
-00000cc0: 2020 2020 3e3e 3e20 6672 6f6d 2073 6861      >>> from sha
-00000cd0: 7065 6c79 2e67 656f 6d65 7472 7920 696d  pely.geometry im
-00000ce0: 706f 7274 2050 6f6c 7967 6f6e 0a20 2020  port Polygon.   
-00000cf0: 203e 3e3e 2070 3120 3d20 506f 6c79 676f   >>> p1 = Polygo
-00000d00: 6e28 5b28 302c 2030 292c 2028 312c 2030  n([(0, 0), (1, 0
-00000d10: 292c 2028 312c 2031 295d 290a 2020 2020  ), (1, 1)]).    
-00000d20: 3e3e 3e20 7032 203d 2050 6f6c 7967 6f6e  >>> p2 = Polygon
-00000d30: 285b 2830 2c20 3029 2c20 2831 2c20 3029  ([(0, 0), (1, 0)
-00000d40: 2c20 2831 2c20 3129 2c20 2830 2c20 3129  , (1, 1), (0, 1)
-00000d50: 5d29 0a20 2020 203e 3e3e 2070 3320 3d20  ]).    >>> p3 = 
-00000d60: 506f 6c79 676f 6e28 5b28 322c 2030 292c  Polygon([(2, 0),
-00000d70: 2028 332c 2030 292c 2028 332c 2031 292c   (3, 0), (3, 1),
-00000d80: 2028 322c 2031 295d 290a 2020 2020 3e3e   (2, 1)]).    >>
-00000d90: 3e20 6720 3d20 6765 6f70 616e 6461 732e  > g = geopandas.
-00000da0: 4765 6f53 6572 6965 7328 5b70 312c 2070  GeoSeries([p1, p
-00000db0: 322c 2070 335d 290a 2020 2020 3e3e 3e20  2, p3]).    >>> 
-00000dc0: 670a 2020 2020 3020 2020 2020 2020 2020  g.    0         
-00000dd0: 504f 4c59 474f 4e20 2828 3020 302c 2031  POLYGON ((0 0, 1
-00000de0: 2030 2c20 3120 312c 2030 2030 2929 0a20   0, 1 1, 0 0)). 
-00000df0: 2020 2031 2020 2020 504f 4c59 474f 4e20     1    POLYGON 
-00000e00: 2828 3020 302c 2031 2030 2c20 3120 312c  ((0 0, 1 0, 1 1,
-00000e10: 2030 2031 2c20 3020 3029 290a 2020 2020   0 1, 0 0)).    
-00000e20: 3220 2020 2050 4f4c 5947 4f4e 2028 2832  2    POLYGON ((2
-00000e30: 2030 2c20 3320 302c 2033 2031 2c20 3220   0, 3 0, 3 1, 2 
-00000e40: 312c 2032 2030 2929 0a20 2020 2064 7479  1, 2 0)).    dty
-00000e50: 7065 3a20 6765 6f6d 6574 7279 0a0a 215b  pe: geometry..![
-00000e60: 4578 616d 706c 6520 315d 2864 6f63 2f73  Example 1](doc/s
-00000e70: 6f75 7263 652f 6761 6c6c 6572 792f 7465  ource/gallery/te
-00000e80: 7374 2e70 6e67 290a 0a53 6f6d 6520 6765  st.png)..Some ge
-00000e90: 6f67 7261 7068 6963 206f 7065 7261 7469  ographic operati
-00000ea0: 6f6e 7320 7265 7475 726e 206e 6f72 6d61  ons return norma
-00000eb0: 6c20 7061 6e64 6173 206f 626a 6563 742e  l pandas object.
-00000ec0: 2020 5468 6520 6061 7265 6160 2070 726f    The `area` pro
-00000ed0: 7065 7274 7920 6f66 2061 2060 4765 6f53  perty of a `GeoS
-00000ee0: 6572 6965 7360 2077 696c 6c20 7265 7475  eries` will retu
-00000ef0: 726e 2061 2060 7061 6e64 6173 2e53 6572  rn a `pandas.Ser
-00000f00: 6965 7360 2063 6f6e 7461 696e 696e 6720  ies` containing 
-00000f10: 7468 6520 6172 6561 206f 6620 6561 6368  the area of each
-00000f20: 2069 7465 6d20 696e 2074 6865 2060 4765   item in the `Ge
-00000f30: 6f53 6572 6965 7360 3a0a 0a20 2020 203e  oSeries`:..    >
-00000f40: 3e3e 2070 7269 6e74 2867 2e61 7265 6129  >> print(g.area)
-00000f50: 0a20 2020 2030 2020 2020 302e 350a 2020  .    0    0.5.  
-00000f60: 2020 3120 2020 2031 2e30 0a20 2020 2032    1    1.0.    2
-00000f70: 2020 2020 312e 300a 2020 2020 6474 7970      1.0.    dtyp
-00000f80: 653a 2066 6c6f 6174 3634 0a0a 4f74 6865  e: float64..Othe
-00000f90: 7220 6f70 6572 6174 696f 6e73 2072 6574  r operations ret
-00000fa0: 7572 6e20 4765 6f50 616e 6461 7320 6f62  urn GeoPandas ob
-00000fb0: 6a65 6374 733a 0a0a 2020 2020 3e3e 3e20  jects:..    >>> 
-00000fc0: 672e 6275 6666 6572 2830 2e35 290a 2020  g.buffer(0.5).  
-00000fd0: 2020 3020 2020 2050 4f4c 5947 4f4e 2028    0    POLYGON (
-00000fe0: 282d 302e 3335 3335 3533 3339 3035 3933  (-0.353553390593
-00000ff0: 3237 3337 2030 2e33 3533 3535 3333 3930  2737 0.353553390
-00001000: 3539 3332 372e 2e2e 0a20 2020 2031 2020  59327....    1  
-00001010: 2020 504f 4c59 474f 4e20 2828 2d30 2e35    POLYGON ((-0.5
-00001020: 2030 2c20 2d30 2e35 2031 2c20 2d30 2e34   0, -0.5 1, -0.4
-00001030: 3937 3539 3233 3633 3333 3630 3938 3520  975923633360985 
-00001040: 2e2e 2e0a 2020 2020 3220 2020 2050 4f4c  ....    2    POL
-00001050: 5947 4f4e 2028 2831 2e35 2030 2c20 312e  YGON ((1.5 0, 1.
-00001060: 3520 312c 2031 2e35 3032 3430 3736 3336  5 1, 1.502407636
-00001070: 3636 3339 3031 2031 2e30 342e 2e2e 0a20  663901 1.04.... 
-00001080: 2020 2064 7479 7065 3a20 6765 6f6d 6574     dtype: geomet
-00001090: 7279 0a0a 215b 4578 616d 706c 6520 325d  ry..![Example 2]
-000010a0: 2864 6f63 2f73 6f75 7263 652f 6761 6c6c  (doc/source/gall
-000010b0: 6572 792f 7465 7374 5f62 7566 6665 722e  ery/test_buffer.
-000010c0: 706e 6729 0a0a 4765 6f50 616e 6461 7320  png)..GeoPandas 
-000010d0: 6f62 6a65 6374 7320 616c 736f 206b 6e6f  objects also kno
-000010e0: 7720 686f 7720 746f 2070 6c6f 7420 7468  w how to plot th
-000010f0: 656d 7365 6c76 6573 2e20 4765 6f50 616e  emselves. GeoPan
-00001100: 6461 7320 7573 6573 0a5b 6d61 7470 6c6f  das uses.[matplo
-00001110: 746c 6962 5d28 6874 7470 3a2f 2f6d 6174  tlib](http://mat
-00001120: 706c 6f74 6c69 622e 6f72 6729 2066 6f72  plotlib.org) for
-00001130: 2070 6c6f 7474 696e 672e 2054 6f20 6765   plotting. To ge
-00001140: 6e65 7261 7465 2061 2070 6c6f 7420 6f66  nerate a plot of
-00001150: 206f 7572 0a47 656f 5365 7269 6573 2c20   our.GeoSeries, 
-00001160: 7573 653a 0a0a 2020 2020 3e3e 3e20 672e  use:..    >>> g.
-00001170: 706c 6f74 2829 0a0a 4765 6f50 616e 6461  plot()..GeoPanda
-00001180: 7320 616c 736f 2069 6d70 6c65 6d65 6e74  s also implement
-00001190: 7320 616c 7465 726e 6174 6520 636f 6e73  s alternate cons
-000011a0: 7472 7563 746f 7273 2074 6861 7420 6361  tructors that ca
-000011b0: 6e20 7265 6164 2061 6e79 2064 6174 6120  n read any data 
-000011c0: 666f 726d 6174 2072 6563 6f67 6e69 7a65  format recognize
-000011d0: 6420 6279 205b 6669 6f6e 615d 2868 7474  d by [fiona](htt
-000011e0: 703a 2f2f 6669 6f6e 612e 7265 6164 7468  p://fiona.readth
-000011f0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00001200: 7374 2f29 2e20 546f 2072 6561 6420 6120  st/). To read a 
-00001210: 7a69 7020 6669 6c65 2063 6f6e 7461 696e  zip file contain
-00001220: 696e 6720 616e 2045 5352 4920 7368 6170  ing an ESRI shap
-00001230: 6566 696c 6520 7769 7468 2074 6865 205b  efile with the [
-00001240: 626f 726f 7567 6873 2062 6f75 6e64 6172  boroughs boundar
-00001250: 6965 7320 6f66 204e 6577 2059 6f72 6b20  ies of New York 
-00001260: 4369 7479 5d28 6874 7470 733a 2f2f 6461  City](https://da
-00001270: 7461 2e63 6974 796f 666e 6577 796f 726b  ta.cityofnewyork
-00001280: 2e75 732f 4369 7479 2d47 6f76 6572 6e6d  .us/City-Governm
-00001290: 656e 742f 426f 726f 7567 682d 426f 756e  ent/Borough-Boun
-000012a0: 6461 7269 6573 2f74 716d 6a2d 6a38 7a6d  daries/tqmj-j8zm
-000012b0: 2920 2847 656f 5061 6e64 6173 2069 6e63  ) (GeoPandas inc
-000012c0: 6c75 6465 7320 7468 6973 2061 7320 616e  ludes this as an
-000012d0: 2065 7861 6d70 6c65 2064 6174 6173 6574   example dataset
-000012e0: 293a 0a0a 2020 2020 3e3e 3e20 6e79 6262  ):..    >>> nybb
-000012f0: 5f70 6174 6820 3d20 6765 6f70 616e 6461  _path = geopanda
-00001300: 732e 6461 7461 7365 7473 2e67 6574 5f70  s.datasets.get_p
-00001310: 6174 6828 276e 7962 6227 290a 2020 2020  ath('nybb').    
-00001320: 3e3e 3e20 626f 726f 7320 3d20 6765 6f70  >>> boros = geop
-00001330: 616e 6461 732e 7265 6164 5f66 696c 6528  andas.read_file(
-00001340: 6e79 6262 5f70 6174 6829 0a20 2020 203e  nybb_path).    >
-00001350: 3e3e 2062 6f72 6f73 2e73 6574 5f69 6e64  >> boros.set_ind
-00001360: 6578 2827 426f 726f 436f 6465 272c 2069  ex('BoroCode', i
-00001370: 6e70 6c61 6365 3d54 7275 6529 0a20 2020  nplace=True).   
-00001380: 203e 3e3e 2062 6f72 6f73 2e73 6f72 745f   >>> boros.sort_
-00001390: 696e 6465 7828 696e 706c 6163 653d 5472  index(inplace=Tr
-000013a0: 7565 290a 2020 2020 3e3e 3e20 626f 726f  ue).    >>> boro
-000013b0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000013c0: 2020 2020 2042 6f72 6f4e 616d 6520 2020       BoroName   
-000013d0: 2020 5368 6170 655f 4c65 6e67 2020 2020    Shape_Leng    
-000013e0: 5368 6170 655f 4172 6561 2020 5c0a 2020  Shape_Area  \.  
-000013f0: 2020 426f 726f 436f 6465 0a20 2020 2031    BoroCode.    1
-00001400: 2020 2020 2020 2020 2020 2020 204d 616e               Man
-00001410: 6861 7474 616e 2020 3335 3932 3939 2e30  hattan  359299.0
-00001420: 3936 3437 3120 2036 2e33 3634 3731 3565  96471  6.364715e
-00001430: 2b30 380a 2020 2020 3220 2020 2020 2020  +08.    2       
-00001440: 2020 2020 2020 2020 2020 4272 6f6e 7820            Bronx 
-00001450: 2034 3634 3339 322e 3939 3138 3234 2020   464392.991824  
-00001460: 312e 3138 3639 3235 652b 3039 0a20 2020  1.186925e+09.   
-00001470: 2033 2020 2020 2020 2020 2020 2020 2020   3              
-00001480: 4272 6f6f 6b6c 796e 2020 3734 3130 3830  Brooklyn  741080
-00001490: 2e35 3233 3136 3620 2031 2e39 3337 3437  .523166  1.93747
-000014a0: 3965 2b30 390a 2020 2020 3420 2020 2020  9e+09.    4     
-000014b0: 2020 2020 2020 2020 2020 2051 7565 656e             Queen
-000014c0: 7320 2038 3936 3334 342e 3034 3737 3633  s  896344.047763
-000014d0: 2020 332e 3034 3532 3133 652b 3039 0a20    3.045213e+09. 
-000014e0: 2020 2035 2020 2020 2020 2020 2053 7461     5         Sta
-000014f0: 7465 6e20 4973 6c61 6e64 2020 3333 3034  ten Island  3304
-00001500: 3730 2e30 3130 3333 3220 2031 2e36 3233  70.010332  1.623
-00001510: 3832 3065 2b30 390a 0a20 2020 2020 2020  820e+09..       
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 6765 6f6d 6574 7279 0a20 2020 2042 6f72  geometry.    Bor
-00001560: 6f43 6f64 650a 2020 2020 3120 2020 2020  oCode.    1     
-00001570: 2020 2020 4d55 4c54 4950 4f4c 5947 4f4e      MULTIPOLYGON
-00001580: 2028 2828 3938 3132 3139 2e30 3535 3738   (((981219.05578
-00001590: 3631 3332 3820 3138 3836 3535 2e33 3135  61328 188655.315
-000015a0: 3739 2e2e 2e0a 2020 2020 3220 2020 2020  79....    2     
-000015b0: 2020 2020 4d55 4c54 4950 4f4c 5947 4f4e      MULTIPOLYGON
-000015c0: 2028 2828 3130 3132 3832 312e 3830 3537   (((1012821.8057
-000015d0: 3836 3133 3320 3232 3932 3238 2e32 3634  86133 229228.264
-000015e0: 3538 2e2e 2e0a 2020 2020 3320 2020 2020  58....    3     
-000015f0: 2020 2020 4d55 4c54 4950 4f4c 5947 4f4e      MULTIPOLYGON
-00001600: 2028 2828 3130 3231 3137 362e 3437 3930   (((1021176.4790
-00001610: 3033 3930 3620 3135 3133 3734 2e37 3936  03906 151374.796
-00001620: 3939 2e2e 2e0a 2020 2020 3420 2020 2020  99....    4     
-00001630: 2020 2020 4d55 4c54 4950 4f4c 5947 4f4e      MULTIPOLYGON
-00001640: 2028 2828 3130 3239 3630 362e 3037 3635   (((1029606.0765
-00001650: 3939 3132 3120 3135 3630 3733 2e38 3134  99121 156073.814
-00001660: 3230 2e2e 2e0a 2020 2020 3520 2020 2020  20....    5     
-00001670: 2020 2020 4d55 4c54 4950 4f4c 5947 4f4e      MULTIPOLYGON
-00001680: 2028 2828 3937 3032 3137 2e30 3232 3339   (((970217.02239
-00001690: 3939 3032 3320 3134 3536 3433 2e33 3332  99023 145643.332
-000016a0: 3231 2e2e 2e0a 0a21 5b4e 6577 2059 6f72  21.....![New Yor
-000016b0: 6b20 4369 7479 2062 6f72 6f75 6768 735d  k City boroughs]
-000016c0: 2864 6f63 2f73 6f75 7263 652f 6761 6c6c  (doc/source/gall
-000016d0: 6572 792f 6e79 632e 706e 6729 0a0a 2020  ery/nyc.png)..  
-000016e0: 2020 3e3e 3e20 626f 726f 735b 2767 656f    >>> boros['geo
-000016f0: 6d65 7472 7927 5d2e 636f 6e76 6578 5f68  metry'].convex_h
-00001700: 756c 6c0a 2020 2020 426f 726f 436f 6465  ull.    BoroCode
-00001710: 0a20 2020 2031 2020 2020 504f 4c59 474f  .    1    POLYGO
-00001720: 4e20 2828 3937 3738 3535 2e34 3435 3139  N ((977855.44519
-00001730: 3034 3239 3720 3138 3830 3832 2e33 3232  04297 188082.322
-00001740: 3338 3736 3935 332c 2e2e 2e0a 2020 2020  3876953,....    
-00001750: 3220 2020 2050 4f4c 5947 4f4e 2028 2831  2    POLYGON ((1
-00001760: 3031 3739 3439 2e39 3737 3630 3030 3938  017949.977600098
-00001770: 2032 3235 3432 362e 3838 3435 3832 3531   225426.88458251
-00001780: 3935 2c2e 2e2e 0a20 2020 2033 2020 2020  95,....    3    
-00001790: 504f 4c59 474f 4e20 2828 3938 3838 3732  POLYGON ((988872
-000017a0: 2e38 3231 3232 3830 3237 3320 3134 3637  .8212280273 1467
-000017b0: 3732 2e30 3331 3739 3933 3136 342c 2e2e  72.0317993164,..
-000017c0: 2e0a 2020 2020 3420 2020 2050 4f4c 5947  ..    4    POLYG
-000017d0: 4f4e 2028 2831 3030 3037 3231 2e35 3331  ON ((1000721.531
-000017e0: 3739 3933 3136 2031 3336 3638 312e 3737  799316 136681.77
-000017f0: 3631 3834 3038 322c 202e 2e2e 0a20 2020  6184082, ....   
-00001800: 2035 2020 2020 504f 4c59 474f 4e20 2828   5    POLYGON ((
-00001810: 3931 3535 3137 2e36 3837 3734 3538 3131  915517.687745811
-00001820: 3420 3132 3031 3231 2e38 3831 3235 3433  4 120121.8812543
-00001830: 3337 322c 2e2e 2e0a 2020 2020 6474 7970  372,....    dtyp
-00001840: 653a 2067 656f 6d65 7472 790a 0a21 5b43  e: geometry..![C
-00001850: 6f6e 7665 7820 6875 6c6c 7320 6f66 204e  onvex hulls of N
-00001860: 6577 2059 6f72 6b20 4369 7479 2062 6f72  ew York City bor
-00001870: 6f75 6768 735d 2864 6f63 2f73 6f75 7263  oughs](doc/sourc
-00001880: 652f 6761 6c6c 6572 792f 6e79 635f 6875  e/gallery/nyc_hu
-00001890: 6c6c 2e70 6e67 290a                      ll.png).
+00000000: 5b21 5b70 7970 695d 2868 7474 7073 3a2f  [![pypi](https:/
+00000010: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000020: 7079 7069 2f76 2f67 656f 7061 6e64 6173  pypi/v/geopandas
+00000030: 2e73 7667 295d 2868 7474 7073 3a2f 2f70  .svg)](https://p
+00000040: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+00000050: 7970 692f 6765 6f70 616e 6461 732f 290a  ypi/geopandas/).
+00000060: 5b21 5b41 6374 696f 6e73 2053 7461 7475  [![Actions Statu
+00000070: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000080: 622e 636f 6d2f 6765 6f70 616e 6461 732f  b.com/geopandas/
+00000090: 6765 6f70 616e 6461 732f 776f 726b 666c  geopandas/workfl
+000000a0: 6f77 732f 5465 7374 732f 6261 6467 652e  ows/Tests/badge.
+000000b0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+000000c0: 7468 7562 2e63 6f6d 2f67 656f 7061 6e64  thub.com/geopand
+000000d0: 6173 2f67 656f 7061 6e64 6173 2f61 6374  as/geopandas/act
+000000e0: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
+000000f0: 6c6f 7725 3341 5465 7374 7329 0a5b 215b  low%3ATests).[![
+00000100: 436f 7665 7261 6765 2053 7461 7475 735d  Coverage Status]
+00000110: 2868 7474 7073 3a2f 2f63 6f64 6563 6f76  (https://codecov
+00000120: 2e69 6f2f 6768 2f67 656f 7061 6e64 6173  .io/gh/geopandas
+00000130: 2f67 656f 7061 6e64 6173 2f62 7261 6e63  /geopandas/branc
+00000140: 682f 6d61 696e 2f67 7261 7068 2f62 6164  h/main/graph/bad
+00000150: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
+00000160: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f67  /codecov.io/gh/g
+00000170: 656f 7061 6e64 6173 2f67 656f 7061 6e64  eopandas/geopand
+00000180: 6173 290a 5b21 5b4a 6f69 6e20 7468 6520  as).[![Join the 
+00000190: 6368 6174 2061 7420 6874 7470 733a 2f2f  chat at https://
+000001a0: 6769 7474 6572 2e69 6d2f 6765 6f70 616e  gitter.im/geopan
+000001b0: 6461 732f 6765 6f70 616e 6461 735d 2868  das/geopandas](h
+000001c0: 7474 7073 3a2f 2f62 6164 6765 732e 6769  ttps://badges.gi
+000001d0: 7474 6572 2e69 6d2f 4a6f 696e 2532 3043  tter.im/Join%20C
+000001e0: 6861 742e 7376 6729 5d28 6874 7470 733a  hat.svg)](https:
+000001f0: 2f2f 6769 7474 6572 2e69 6d2f 6765 6f70  //gitter.im/geop
+00000200: 616e 6461 732f 6765 6f70 616e 6461 733f  andas/geopandas?
+00000210: 7574 6d5f 736f 7572 6365 3d62 6164 6765  utm_source=badge
+00000220: 2675 746d 5f6d 6564 6975 6d3d 6261 6467  &utm_medium=badg
+00000230: 6526 7574 6d5f 6361 6d70 6169 676e 3d70  e&utm_campaign=p
+00000240: 722d 6261 6467 6526 7574 6d5f 636f 6e74  r-badge&utm_cont
+00000250: 656e 743d 6261 6467 6529 0a5b 215b 4269  ent=badge).[![Bi
+00000260: 6e64 6572 5d28 6874 7470 733a 2f2f 6d79  nder](https://my
+00000270: 6269 6e64 6572 2e6f 7267 2f62 6164 6765  binder.org/badge
+00000280: 2e73 7667 295d 2868 7474 7073 3a2f 2f6d  .svg)](https://m
+00000290: 7962 696e 6465 722e 6f72 672f 7632 2f67  ybinder.org/v2/g
+000002a0: 682f 6765 6f70 616e 6461 732f 6765 6f70  h/geopandas/geop
+000002b0: 616e 6461 732f 6d61 696e 290a 5b21 5b44  andas/main).[![D
+000002c0: 4f49 5d28 6874 7470 733a 2f2f 7a65 6e6f  OI](https://zeno
+000002d0: 646f 2e6f 7267 2f62 6164 6765 2f31 3130  do.org/badge/110
+000002e0: 3032 3831 352e 7376 6729 5d28 6874 7470  02815.svg)](http
+000002f0: 733a 2f2f 7a65 6e6f 646f 2e6f 7267 2f62  s://zenodo.org/b
+00000300: 6164 6765 2f6c 6174 6573 7464 6f69 2f31  adge/latestdoi/1
+00000310: 3130 3032 3831 3529 0a5b 215b 506f 7765  1002815).[![Powe
+00000320: 7265 6420 6279 204e 756d 464f 4355 535d  red by NumFOCUS]
+00000330: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000340: 656c 6473 2e69 6f2f 6261 6467 652f 706f  elds.io/badge/po
+00000350: 7765 7265 6425 3230 6279 2d4e 756d 464f  wered%20by-NumFO
+00000360: 4355 532d 6f72 616e 6765 2e73 7667 3f73  CUS-orange.svg?s
+00000370: 7479 6c65 3d66 6c61 7426 636f 6c6f 7241  tyle=flat&colorA
+00000380: 3d45 3135 3233 4426 636f 6c6f 7242 3d30  =E1523D&colorB=0
+00000390: 3037 4438 4129 5d28 6874 7470 733a 2f2f  07D8A)](https://
+000003a0: 6e75 6d66 6f63 7573 2e6f 7267 290a 0a47  numfocus.org)..G
+000003b0: 656f 5061 6e64 6173 0a2d 2d2d 2d2d 2d2d  eoPandas.-------
+000003c0: 2d2d 0a0a 5079 7468 6f6e 2074 6f6f 6c73  --..Python tools
+000003d0: 2066 6f72 2067 656f 6772 6170 6869 6320   for geographic 
+000003e0: 6461 7461 0a0a 496e 7472 6f64 7563 7469  data..Introducti
+000003f0: 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  on.------------.
+00000400: 0a47 656f 5061 6e64 6173 2069 7320 6120  .GeoPandas is a 
+00000410: 7072 6f6a 6563 7420 746f 2061 6464 2073  project to add s
+00000420: 7570 706f 7274 2066 6f72 2067 656f 6772  upport for geogr
+00000430: 6170 6869 6320 6461 7461 2074 6f0a 5b70  aphic data to.[p
+00000440: 616e 6461 735d 2868 7474 703a 2f2f 7061  andas](http://pa
+00000450: 6e64 6173 2e70 7964 6174 612e 6f72 6729  ndas.pydata.org)
+00000460: 206f 626a 6563 7473 2e20 2049 7420 6375   objects.  It cu
+00000470: 7272 656e 746c 7920 696d 706c 656d 656e  rrently implemen
+00000480: 7473 0a60 4765 6f53 6572 6965 7360 2061  ts.`GeoSeries` a
+00000490: 6e64 2060 4765 6f44 6174 6146 7261 6d65  nd `GeoDataFrame
+000004a0: 6020 7479 7065 7320 7768 6963 6820 6172  ` types which ar
+000004b0: 6520 7375 6263 6c61 7373 6573 206f 660a  e subclasses of.
+000004c0: 6070 616e 6461 732e 5365 7269 6573 6020  `pandas.Series` 
+000004d0: 616e 6420 6070 616e 6461 732e 4461 7461  and `pandas.Data
+000004e0: 4672 616d 6560 2072 6573 7065 6374 6976  Frame` respectiv
+000004f0: 656c 792e 2020 4765 6f50 616e 6461 730a  ely.  GeoPandas.
+00000500: 6f62 6a65 6374 7320 6361 6e20 6163 7420  objects can act 
+00000510: 6f6e 205b 7368 6170 656c 795d 2868 7474  on [shapely](htt
+00000520: 703a 2f2f 7368 6170 656c 792e 7265 6164  p://shapely.read
+00000530: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000540: 7465 7374 2f29 0a67 656f 6d65 7472 7920  test/).geometry 
+00000550: 6f62 6a65 6374 7320 616e 6420 7065 7266  objects and perf
+00000560: 6f72 6d20 6765 6f6d 6574 7269 6320 6f70  orm geometric op
+00000570: 6572 6174 696f 6e73 2e0a 0a47 656f 5061  erations...GeoPa
+00000580: 6e64 6173 2067 656f 6d65 7472 7920 6f70  ndas geometry op
+00000590: 6572 6174 696f 6e73 2061 7265 2063 6172  erations are car
+000005a0: 7465 7369 616e 2e20 2054 6865 2063 6f6f  tesian.  The coo
+000005b0: 7264 696e 6174 6520 7265 6665 7265 6e63  rdinate referenc
+000005c0: 650a 7379 7374 656d 2028 6372 7329 2063  e.system (crs) c
+000005d0: 616e 2062 6520 7374 6f72 6564 2061 7320  an be stored as 
+000005e0: 616e 2061 7474 7269 6275 7465 206f 6e20  an attribute on 
+000005f0: 616e 206f 626a 6563 742c 2061 6e64 2069  an object, and i
+00000600: 730a 6175 746f 6d61 7469 6361 6c6c 7920  s.automatically 
+00000610: 7365 7420 7768 656e 206c 6f61 6469 6e67  set when loading
+00000620: 2066 726f 6d20 6120 6669 6c65 2e20 204f   from a file.  O
+00000630: 626a 6563 7473 206d 6179 2062 650a 7472  bjects may be.tr
+00000640: 616e 7366 6f72 6d65 6420 746f 206e 6577  ansformed to new
+00000650: 2063 6f6f 7264 696e 6174 6520 7379 7374   coordinate syst
+00000660: 656d 7320 7769 7468 2074 6865 2060 746f  ems with the `to
+00000670: 5f63 7273 2829 6020 6d65 7468 6f64 2e0a  _crs()` method..
+00000680: 5468 6572 6520 6973 2063 7572 7265 6e74  There is current
+00000690: 6c79 206e 6f20 656e 666f 7263 656d 656e  ly no enforcemen
+000006a0: 7420 6f66 206c 696b 6520 636f 6f72 6469  t of like coordi
+000006b0: 6e61 7465 7320 666f 7220 6f70 6572 6174  nates for operat
+000006c0: 696f 6e73 2c0a 6275 7420 7468 6174 206d  ions,.but that m
+000006d0: 6179 2063 6861 6e67 6520 696e 2074 6865  ay change in the
+000006e0: 2066 7574 7572 652e 0a0a 446f 6375 6d65   future...Docume
+000006f0: 6e74 6174 696f 6e20 6973 2061 7661 696c  ntation is avail
+00000700: 6162 6c65 2061 7420 5b67 656f 7061 6e64  able at [geopand
+00000710: 6173 2e6f 7267 5d28 6874 7470 3a2f 2f67  as.org](http://g
+00000720: 656f 7061 6e64 6173 2e6f 7267 290a 2863  eopandas.org).(c
+00000730: 7572 7265 6e74 2072 656c 6561 7365 2920  urrent release) 
+00000740: 616e 640a 5b52 6561 6420 7468 6520 446f  and.[Read the Do
+00000750: 6373 5d28 6874 7470 3a2f 2f67 656f 7061  cs](http://geopa
+00000760: 6e64 6173 2e72 6561 6474 6865 646f 6373  ndas.readthedocs
+00000770: 2e69 6f2f 656e 2f6c 6174 6573 742f 290a  .io/en/latest/).
+00000780: 2872 656c 6561 7365 2061 6e64 2064 6576  (release and dev
+00000790: 656c 6f70 6d65 6e74 2076 6572 7369 6f6e  elopment version
+000007a0: 7329 2e0a 0a5b 2f2f 5d3a 2023 2028 6e75  s)...[//]: # (nu
+000007b0: 6d66 6f63 7573 2d66 6973 6361 6c2d 7370  mfocus-fiscal-sp
+000007c0: 6f6e 736f 722d 6174 7472 6962 7574 696f  onsor-attributio
+000007d0: 6e29 0a0a 5468 6520 4765 6f50 616e 6461  n)..The GeoPanda
+000007e0: 7320 7072 6f6a 6563 7420 7573 6573 2061  s project uses a
+000007f0: 6e20 5b6f 7065 6e20 676f 7665 726e 616e  n [open governan
+00000800: 6365 206d 6f64 656c 5d28 6874 7470 733a  ce model](https:
+00000810: 2f2f 6769 7468 7562 2e63 6f6d 2f67 656f  //github.com/geo
+00000820: 7061 6e64 6173 2f67 6f76 6572 6e61 6e63  pandas/governanc
+00000830: 652f 626c 6f62 2f6d 6169 6e2f 476f 7665  e/blob/main/Gove
+00000840: 726e 616e 6365 2e6d 6429 0a61 6e64 2069  rnance.md).and i
+00000850: 7320 6669 7363 616c 6c79 2073 706f 6e73  s fiscally spons
+00000860: 6f72 6564 2062 7920 5b4e 756d 464f 4355  ored by [NumFOCU
+00000870: 535d 2868 7474 7073 3a2f 2f6e 756d 666f  S](https://numfo
+00000880: 6375 732e 6f72 672f 292e 2043 6f6e 7369  cus.org/). Consi
+00000890: 6465 7220 6d61 6b69 6e67 0a61 205b 7461  der making.a [ta
+000008a0: 782d 6465 6475 6374 6962 6c65 2064 6f6e  x-deductible don
+000008b0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6e  ation](https://n
+000008c0: 756d 666f 6375 732e 6f72 672f 646f 6e61  umfocus.org/dona
+000008d0: 7465 2d66 6f72 2d67 656f 7061 6e64 6173  te-for-geopandas
+000008e0: 2920 746f 2068 656c 7020 7468 6520 7072  ) to help the pr
+000008f0: 6f6a 6563 740a 7061 7920 666f 7220 6465  oject.pay for de
+00000900: 7665 6c6f 7065 7220 7469 6d65 2c20 7072  veloper time, pr
+00000910: 6f66 6573 7369 6f6e 616c 2073 6572 7669  ofessional servi
+00000920: 6365 732c 2074 7261 7665 6c2c 2077 6f72  ces, travel, wor
+00000930: 6b73 686f 7073 2c20 616e 6420 6120 7661  kshops, and a va
+00000940: 7269 6574 7920 6f66 206f 7468 6572 206e  riety of other n
+00000950: 6565 6473 2e0a 0a3c 6469 7620 616c 6967  eeds...<div alig
+00000960: 6e3d 2263 656e 7465 7222 3e0a 2020 3c61  n="center">.  <a
+00000970: 2068 7265 663d 2268 7474 7073 3a2f 2f6e   href="https://n
+00000980: 756d 666f 6375 732e 6f72 672f 7072 6f6a  umfocus.org/proj
+00000990: 6563 742f 6765 6f70 616e 6461 7322 3e0a  ect/geopandas">.
+000009a0: 2020 2020 3c69 6d67 2068 6569 6768 743d      <img height=
+000009b0: 2236 3070 7822 0a20 2020 2020 2020 2020  "60px".         
+000009c0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+000009d0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000009e0: 6e74 2e63 6f6d 2f6e 756d 666f 6375 732f  nt.com/numfocus/
+000009f0: 7465 6d70 6c61 7465 732f 6d61 7374 6572  templates/master
+00000a00: 2f69 6d61 6765 732f 6e75 6d66 6f63 7573  /images/numfocus
+00000a10: 2d6c 6f67 6f2e 706e 6722 0a20 2020 2020  -logo.png".     
+00000a20: 2020 2020 616c 6967 6e3d 2263 656e 7465      align="cente
+00000a30: 7222 3e0a 2020 3c2f 613e 0a3c 2f64 6976  r">.  </a>.</div
+00000a40: 3e0a 3c62 723e 0a0a 496e 7374 616c 6c0a  >.<br>..Install.
+00000a50: 2d2d 2d2d 2d2d 2d2d 0a0a 5365 6520 7468  --------..See th
+00000a60: 6520 5b69 6e73 7461 6c6c 6174 696f 6e20  e [installation 
+00000a70: 646f 6373 5d28 6874 7470 733a 2f2f 6765  docs](https://ge
+00000a80: 6f70 616e 6461 732e 7265 6164 7468 6564  opandas.readthed
+00000a90: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000aa0: 2f69 6e73 7461 6c6c 2e68 746d 6c29 0a66  /install.html).f
+00000ab0: 6f72 2061 6c6c 2064 6574 6169 6c73 2e20  or all details. 
+00000ac0: 4765 6f50 616e 6461 7320 6465 7065 6e64  GeoPandas depend
+00000ad0: 7320 6f6e 2074 6865 2066 6f6c 6c6f 7769  s on the followi
+00000ae0: 6e67 2070 6163 6b61 6765 733a 0a0a 2d20  ng packages:..- 
+00000af0: 6060 7061 6e64 6173 6060 0a2d 2060 6073  ``pandas``.- ``s
+00000b00: 6861 7065 6c79 6060 0a2d 2060 6070 796f  hapely``.- ``pyo
+00000b10: 6772 696f 6060 0a2d 2060 6070 7970 726f  grio``.- ``pypro
+00000b20: 6a60 600a 2d20 6060 7061 636b 6167 696e  j``.- ``packagin
+00000b30: 6760 600a 0a46 7572 7468 6572 2c20 6060  g``..Further, ``
+00000b40: 6d61 7470 6c6f 746c 6962 6060 2069 7320  matplotlib`` is 
+00000b50: 616e 206f 7074 696f 6e61 6c20 6465 7065  an optional depe
+00000b60: 6e64 656e 6379 2c20 7265 7175 6972 6564  ndency, required
+00000b70: 2066 6f72 2070 6c6f 7474 696e 672e 0a54   for plotting..T
+00000b80: 686f 7365 2070 6163 6b61 6765 7320 6465  hose packages de
+00000b90: 7065 6e64 206f 6e20 7365 7665 7261 6c20  pend on several 
+00000ba0: 6c6f 772d 6c65 7665 6c20 6c69 6272 6172  low-level librar
+00000bb0: 6965 7320 666f 7220 6765 6f73 7061 7469  ies for geospati
+00000bc0: 616c 2061 6e61 6c79 7369 732c 2077 6869  al analysis, whi
+00000bd0: 6368 2063 616e 2062 6520 6120 6368 616c  ch can be a chal
+00000be0: 6c65 6e67 6520 746f 2069 6e73 7461 6c6c  lenge to install
+00000bf0: 2e20 5468 6572 6566 6f72 652c 2077 6520  . Therefore, we 
+00000c00: 7265 636f 6d6d 656e 6420 746f 2069 6e73  recommend to ins
+00000c10: 7461 6c6c 2047 656f 5061 6e64 6173 2075  tall GeoPandas u
+00000c20: 7369 6e67 2074 6865 205b 636f 6e64 6120  sing the [conda 
+00000c30: 7061 636b 6167 6520 6d61 6e61 6765 725d  package manager]
+00000c40: 2868 7474 7073 3a2f 2f63 6f6e 6461 2e69  (https://conda.i
+00000c50: 6f2f 656e 2f6c 6174 6573 742f 292e 2053  o/en/latest/). S
+00000c60: 6565 2074 6865 205b 696e 7374 616c 6c61  ee the [installa
+00000c70: 7469 6f6e 2064 6f63 735d 2868 7474 7073  tion docs](https
+00000c80: 3a2f 2f67 656f 7061 6e64 6173 2e72 6561  ://geopandas.rea
+00000c90: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000ca0: 6174 6573 742f 696e 7374 616c 6c2e 6874  atest/install.ht
+00000cb0: 6d6c 2920 666f 7220 6d6f 7265 2064 6574  ml) for more det
+00000cc0: 6169 6c73 2e0a 0a47 6574 2069 6e20 746f  ails...Get in to
+00000cd0: 7563 680a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  uch.------------
+00000ce0: 0a0a 2d20 4173 6b20 7573 6167 6520 7175  ..- Ask usage qu
+00000cf0: 6573 7469 6f6e 7320 2822 486f 7720 646f  estions ("How do
+00000d00: 2049 3f22 2920 6f6e 205b 5374 6163 6b4f   I?") on [StackO
+00000d10: 7665 7266 6c6f 775d 2868 7474 7073 3a2f  verflow](https:/
+00000d20: 2f73 7461 636b 6f76 6572 666c 6f77 2e63  /stackoverflow.c
+00000d30: 6f6d 2f71 7565 7374 696f 6e73 2f74 6167  om/questions/tag
+00000d40: 6765 642f 6765 6f70 616e 6461 7329 206f  ged/geopandas) o
+00000d50: 7220 5b47 4953 2053 7461 636b 4578 6368  r [GIS StackExch
+00000d60: 616e 6765 5d28 6874 7470 733a 2f2f 6769  ange](https://gi
+00000d70: 732e 7374 6163 6b65 7863 6861 6e67 652e  s.stackexchange.
+00000d80: 636f 6d2f 7175 6573 7469 6f6e 732f 7461  com/questions/ta
+00000d90: 6767 6564 2f67 656f 7061 6e64 6173 292e  gged/geopandas).
+00000da0: 0a2d 2047 6574 2069 6e76 6f6c 7665 6420  .- Get involved 
+00000db0: 696e 205b 6469 7363 7573 7369 6f6e 7320  in [discussions 
+00000dc0: 6f6e 2047 6974 4875 625d 2868 7474 7073  on GitHub](https
+00000dd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6765  ://github.com/ge
+00000de0: 6f70 616e 6461 732f 6765 6f70 616e 6461  opandas/geopanda
+00000df0: 732f 6469 7363 7573 7369 6f6e 7329 0a2d  s/discussions).-
+00000e00: 2052 6570 6f72 7420 6275 6773 2c20 7375   Report bugs, su
+00000e10: 6767 6573 7420 6665 6174 7572 6573 206f  ggest features o
+00000e20: 7220 7669 6577 2074 6865 2073 6f75 7263  r view the sourc
+00000e30: 6520 636f 6465 205b 6f6e 2047 6974 4875  e code [on GitHu
+00000e40: 625d 2868 7474 7073 3a2f 2f67 6974 6875  b](https://githu
+00000e50: 622e 636f 6d2f 6765 6f70 616e 6461 732f  b.com/geopandas/
+00000e60: 6765 6f70 616e 6461 7329 2e0a 2d20 466f  geopandas)..- Fo
+00000e70: 7220 6120 7175 6963 6b20 7175 6573 7469  r a quick questi
+00000e80: 6f6e 2061 626f 7574 2061 2062 7567 2072  on about a bug r
+00000e90: 6570 6f72 7420 6f72 2066 6561 7475 7265  eport or feature
+00000ea0: 2072 6571 7565 7374 2c20 6f72 2050 756c   request, or Pul
+00000eb0: 6c20 5265 7175 6573 742c 2068 6561 6420  l Request, head 
+00000ec0: 6f76 6572 2074 6f20 7468 6520 5b67 6974  over to the [git
+00000ed0: 7465 7220 6368 616e 6e65 6c5d 2868 7474  ter channel](htt
+00000ee0: 7073 3a2f 2f67 6974 7465 722e 696d 2f67  ps://gitter.im/g
+00000ef0: 656f 7061 6e64 6173 2f67 656f 7061 6e64  eopandas/geopand
+00000f00: 6173 292e 0a2d 2046 6f72 206c 6573 7320  as)..- For less 
+00000f10: 7765 6c6c 2064 6566 696e 6564 2071 7565  well defined que
+00000f20: 7374 696f 6e73 206f 7220 6964 6561 732c  stions or ideas,
+00000f30: 206f 7220 746f 2061 6e6e 6f75 6e63 6520   or to announce 
+00000f40: 6f74 6865 7220 7072 6f6a 6563 7473 206f  other projects o
+00000f50: 6620 696e 7465 7265 7374 2074 6f20 4765  f interest to Ge
+00000f60: 6f50 616e 6461 7320 7573 6572 732c 202e  oPandas users, .
+00000f70: 2e2e 2075 7365 2074 6865 205b 6d61 696c  .. use the [mail
+00000f80: 696e 6720 6c69 7374 5d28 6874 7470 733a  ing list](https:
+00000f90: 2f2f 6772 6f75 7073 2e67 6f6f 676c 652e  //groups.google.
+00000fa0: 636f 6d2f 666f 7275 6d2f 2321 666f 7275  com/forum/#!foru
+00000fb0: 6d2f 6765 6f70 616e 6461 7329 2e0a 0a45  m/geopandas)...E
+00000fc0: 7861 6d70 6c65 730a 2d2d 2d2d 2d2d 2d2d  xamples.--------
+00000fd0: 0a0a 2020 2020 3e3e 3e20 696d 706f 7274  ..    >>> import
+00000fe0: 2067 656f 7061 6e64 6173 0a20 2020 203e   geopandas.    >
+00000ff0: 3e3e 2066 726f 6d20 7368 6170 656c 792e  >> from shapely.
+00001000: 6765 6f6d 6574 7279 2069 6d70 6f72 7420  geometry import 
+00001010: 506f 6c79 676f 6e0a 2020 2020 3e3e 3e20  Polygon.    >>> 
+00001020: 7031 203d 2050 6f6c 7967 6f6e 285b 2830  p1 = Polygon([(0
+00001030: 2c20 3029 2c20 2831 2c20 3029 2c20 2831  , 0), (1, 0), (1
+00001040: 2c20 3129 5d29 0a20 2020 203e 3e3e 2070  , 1)]).    >>> p
+00001050: 3220 3d20 506f 6c79 676f 6e28 5b28 302c  2 = Polygon([(0,
+00001060: 2030 292c 2028 312c 2030 292c 2028 312c   0), (1, 0), (1,
+00001070: 2031 292c 2028 302c 2031 295d 290a 2020   1), (0, 1)]).  
+00001080: 2020 3e3e 3e20 7033 203d 2050 6f6c 7967    >>> p3 = Polyg
+00001090: 6f6e 285b 2832 2c20 3029 2c20 2833 2c20  on([(2, 0), (3, 
+000010a0: 3029 2c20 2833 2c20 3129 2c20 2832 2c20  0), (3, 1), (2, 
+000010b0: 3129 5d29 0a20 2020 203e 3e3e 2067 203d  1)]).    >>> g =
+000010c0: 2067 656f 7061 6e64 6173 2e47 656f 5365   geopandas.GeoSe
+000010d0: 7269 6573 285b 7031 2c20 7032 2c20 7033  ries([p1, p2, p3
+000010e0: 5d29 0a20 2020 203e 3e3e 2067 0a20 2020  ]).    >>> g.   
+000010f0: 2030 2020 2020 2020 2020 2050 4f4c 5947   0         POLYG
+00001100: 4f4e 2028 2830 2030 2c20 3120 302c 2031  ON ((0 0, 1 0, 1
+00001110: 2031 2c20 3020 3029 290a 2020 2020 3120   1, 0 0)).    1 
+00001120: 2020 2050 4f4c 5947 4f4e 2028 2830 2030     POLYGON ((0 0
+00001130: 2c20 3120 302c 2031 2031 2c20 3020 312c  , 1 0, 1 1, 0 1,
+00001140: 2030 2030 2929 0a20 2020 2032 2020 2020   0 0)).    2    
+00001150: 504f 4c59 474f 4e20 2828 3220 302c 2033  POLYGON ((2 0, 3
+00001160: 2030 2c20 3320 312c 2032 2031 2c20 3220   0, 3 1, 2 1, 2 
+00001170: 3029 290a 2020 2020 6474 7970 653a 2067  0)).    dtype: g
+00001180: 656f 6d65 7472 790a 0a21 5b45 7861 6d70  eometry..![Examp
+00001190: 6c65 2031 5d28 646f 632f 736f 7572 6365  le 1](doc/source
+000011a0: 2f67 616c 6c65 7279 2f74 6573 742e 706e  /gallery/test.pn
+000011b0: 6729 0a0a 536f 6d65 2067 656f 6772 6170  g)..Some geograp
+000011c0: 6869 6320 6f70 6572 6174 696f 6e73 2072  hic operations r
+000011d0: 6574 7572 6e20 6e6f 726d 616c 2070 616e  eturn normal pan
+000011e0: 6461 7320 6f62 6a65 6374 732e 2020 5468  das objects.  Th
+000011f0: 6520 6061 7265 6160 2070 726f 7065 7274  e `area` propert
+00001200: 7920 6f66 2061 2060 4765 6f53 6572 6965  y of a `GeoSerie
+00001210: 7360 2077 696c 6c20 7265 7475 726e 2061  s` will return a
+00001220: 2060 7061 6e64 6173 2e53 6572 6965 7360   `pandas.Series`
+00001230: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00001240: 6172 6561 206f 6620 6561 6368 2069 7465  area of each ite
+00001250: 6d20 696e 2074 6865 2060 4765 6f53 6572  m in the `GeoSer
+00001260: 6965 7360 3a0a 0a20 2020 203e 3e3e 2070  ies`:..    >>> p
+00001270: 7269 6e74 2867 2e61 7265 6129 0a20 2020  rint(g.area).   
+00001280: 2030 2020 2020 302e 350a 2020 2020 3120   0    0.5.    1 
+00001290: 2020 2031 2e30 0a20 2020 2032 2020 2020     1.0.    2    
+000012a0: 312e 300a 2020 2020 6474 7970 653a 2066  1.0.    dtype: f
+000012b0: 6c6f 6174 3634 0a0a 4f74 6865 7220 6f70  loat64..Other op
+000012c0: 6572 6174 696f 6e73 2072 6574 7572 6e20  erations return 
+000012d0: 4765 6f50 616e 6461 7320 6f62 6a65 6374  GeoPandas object
+000012e0: 733a 0a0a 2020 2020 3e3e 3e20 672e 6275  s:..    >>> g.bu
+000012f0: 6666 6572 2830 2e35 290a 2020 2020 3020  ffer(0.5).    0 
+00001300: 2020 2050 4f4c 5947 4f4e 2028 282d 302e     POLYGON ((-0.
+00001310: 3335 3335 3533 3339 3035 3933 3237 3337  3535533905932737
+00001320: 2030 2e33 3533 3535 3333 3930 3539 3332   0.3535533905932
+00001330: 372e 2e2e 0a20 2020 2031 2020 2020 504f  7....    1    PO
+00001340: 4c59 474f 4e20 2828 2d30 2e35 2030 2c20  LYGON ((-0.5 0, 
+00001350: 2d30 2e35 2031 2c20 2d30 2e34 3937 3539  -0.5 1, -0.49759
+00001360: 3233 3633 3333 3630 3938 3520 2e2e 2e0a  23633360985 ....
+00001370: 2020 2020 3220 2020 2050 4f4c 5947 4f4e      2    POLYGON
+00001380: 2028 2831 2e35 2030 2c20 312e 3520 312c   ((1.5 0, 1.5 1,
+00001390: 2031 2e35 3032 3430 3736 3336 3636 3339   1.5024076366639
+000013a0: 3031 2031 2e30 342e 2e2e 0a20 2020 2064  01 1.04....    d
+000013b0: 7479 7065 3a20 6765 6f6d 6574 7279 0a0a  type: geometry..
+000013c0: 215b 4578 616d 706c 6520 325d 2864 6f63  ![Example 2](doc
+000013d0: 2f73 6f75 7263 652f 6761 6c6c 6572 792f  /source/gallery/
+000013e0: 7465 7374 5f62 7566 6665 722e 706e 6729  test_buffer.png)
+000013f0: 0a0a 4765 6f50 616e 6461 7320 6f62 6a65  ..GeoPandas obje
+00001400: 6374 7320 616c 736f 206b 6e6f 7720 686f  cts also know ho
+00001410: 7720 746f 2070 6c6f 7420 7468 656d 7365  w to plot themse
+00001420: 6c76 6573 2e20 4765 6f50 616e 6461 7320  lves. GeoPandas 
+00001430: 7573 6573 0a5b 6d61 7470 6c6f 746c 6962  uses.[matplotlib
+00001440: 5d28 6874 7470 3a2f 2f6d 6174 706c 6f74  ](http://matplot
+00001450: 6c69 622e 6f72 6729 2066 6f72 2070 6c6f  lib.org) for plo
+00001460: 7474 696e 672e 2054 6f20 6765 6e65 7261  tting. To genera
+00001470: 7465 2061 2070 6c6f 7420 6f66 2061 0a60  te a plot of a.`
+00001480: 4765 6f53 6572 6965 7360 2c20 7573 653a  GeoSeries`, use:
+00001490: 0a0a 2020 2020 3e3e 3e20 672e 706c 6f74  ..    >>> g.plot
+000014a0: 2829 0a0a 4765 6f50 616e 6461 7320 616c  ()..GeoPandas al
+000014b0: 736f 2069 6d70 6c65 6d65 6e74 7320 616c  so implements al
+000014c0: 7465 726e 6174 6520 636f 6e73 7472 7563  ternate construc
+000014d0: 746f 7273 2074 6861 7420 6361 6e20 7265  tors that can re
+000014e0: 6164 2061 6e79 2064 6174 6120 666f 726d  ad any data form
+000014f0: 6174 2072 6563 6f67 6e69 7a65 6420 6279  at recognized by
+00001500: 205b 7079 6f67 7269 6f5d 2868 7474 703a   [pyogrio](http:
+00001510: 2f2f 7079 6f67 7269 6f2e 7265 6164 7468  //pyogrio.readth
+00001520: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00001530: 7374 2f29 2e20 546f 2072 6561 6420 6120  st/). To read a 
+00001540: 7a69 7020 6669 6c65 2063 6f6e 7461 696e  zip file contain
+00001550: 696e 6720 616e 2045 5352 4920 7368 6170  ing an ESRI shap
+00001560: 6566 696c 6520 7769 7468 2074 6865 205b  efile with the [
+00001570: 626f 726f 7567 6873 2062 6f75 6e64 6172  boroughs boundar
+00001580: 6965 7320 6f66 204e 6577 2059 6f72 6b20  ies of New York 
+00001590: 4369 7479 5d28 6874 7470 733a 2f2f 6461  City](https://da
+000015a0: 7461 2e63 6974 796f 666e 6577 796f 726b  ta.cityofnewyork
+000015b0: 2e75 732f 4369 7479 2d47 6f76 6572 6e6d  .us/City-Governm
+000015c0: 656e 742f 426f 726f 7567 682d 426f 756e  ent/Borough-Boun
+000015d0: 6461 7269 6573 2f74 716d 6a2d 6a38 7a6d  daries/tqmj-j8zm
+000015e0: 2920 2874 6865 2065 7861 6d70 6c65 2063  ) (the example c
+000015f0: 616e 2062 6520 6665 7463 6865 6420 7573  an be fetched us
+00001600: 696e 6720 7468 6520 5b60 6765 6f64 6174  ing the [`geodat
+00001610: 6173 6574 7360 5d28 6874 7470 733a 2f2f  asets`](https://
+00001620: 6765 6f64 6174 6173 6574 732e 7265 6164  geodatasets.read
+00001630: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00001640: 7465 7374 2f29 2070 6163 6b61 6765 293a  test/) package):
+00001650: 0a0a 2020 2020 3e3e 3e20 696d 706f 7274  ..    >>> import
+00001660: 2067 656f 6461 7461 7365 7473 0a20 2020   geodatasets.   
+00001670: 203e 3e3e 206e 7962 625f 7061 7468 203d   >>> nybb_path =
+00001680: 2067 656f 6461 7461 7365 7473 2e67 6574   geodatasets.get
+00001690: 5f70 6174 6828 276e 7962 6227 290a 2020  _path('nybb').  
+000016a0: 2020 3e3e 3e20 626f 726f 7320 3d20 6765    >>> boros = ge
+000016b0: 6f70 616e 6461 732e 7265 6164 5f66 696c  opandas.read_fil
+000016c0: 6528 6e79 6262 5f70 6174 6829 0a20 2020  e(nybb_path).   
+000016d0: 203e 3e3e 2062 6f72 6f73 2e73 6574 5f69   >>> boros.set_i
+000016e0: 6e64 6578 2827 426f 726f 436f 6465 272c  ndex('BoroCode',
+000016f0: 2069 6e70 6c61 6365 3d54 7275 6529 0a20   inplace=True). 
+00001700: 2020 203e 3e3e 2062 6f72 6f73 2e73 6f72     >>> boros.sor
+00001710: 745f 696e 6465 7828 696e 706c 6163 653d  t_index(inplace=
+00001720: 5472 7565 290a 2020 2020 3e3e 3e20 626f  True).    >>> bo
+00001730: 726f 730a 2020 2020 2020 2020 2020 2020  ros.            
+00001740: 2020 2020 2020 2042 6f72 6f4e 616d 6520         BoroName 
+00001750: 2020 2020 5368 6170 655f 4c65 6e67 2020      Shape_Leng  
+00001760: 2020 5368 6170 655f 4172 6561 2020 5c0a    Shape_Area  \.
+00001770: 2020 2020 426f 726f 436f 6465 0a20 2020      BoroCode.   
+00001780: 2031 2020 2020 2020 2020 2020 2020 204d   1             M
+00001790: 616e 6861 7474 616e 2020 3335 3932 3939  anhattan  359299
+000017a0: 2e30 3936 3437 3120 2036 2e33 3634 3731  .096471  6.36471
+000017b0: 3565 2b30 380a 2020 2020 3220 2020 2020  5e+08.    2     
+000017c0: 2020 2020 2020 2020 2020 2020 4272 6f6e              Bron
+000017d0: 7820 2034 3634 3339 322e 3939 3138 3234  x  464392.991824
+000017e0: 2020 312e 3138 3639 3235 652b 3039 0a20    1.186925e+09. 
+000017f0: 2020 2033 2020 2020 2020 2020 2020 2020     3            
+00001800: 2020 4272 6f6f 6b6c 796e 2020 3734 3130    Brooklyn  7410
+00001810: 3830 2e35 3233 3136 3620 2031 2e39 3337  80.523166  1.937
+00001820: 3437 3965 2b30 390a 2020 2020 3420 2020  479e+09.    4   
+00001830: 2020 2020 2020 2020 2020 2020 2051 7565               Que
+00001840: 656e 7320 2038 3936 3334 342e 3034 3737  ens  896344.0477
+00001850: 3633 2020 332e 3034 3532 3133 652b 3039  63  3.045213e+09
+00001860: 0a20 2020 2035 2020 2020 2020 2020 2053  .    5         S
+00001870: 7461 7465 6e20 4973 6c61 6e64 2020 3333  taten Island  33
+00001880: 3034 3730 2e30 3130 3333 3220 2031 2e36  0470.010332  1.6
+00001890: 3233 3832 3065 2b30 390a 0a20 2020 2020  23820e+09..     
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 2020 6765 6f6d 6574 7279 0a20 2020 2042    geometry.    B
+000018e0: 6f72 6f43 6f64 650a 2020 2020 3120 2020  oroCode.    1   
+000018f0: 2020 2020 2020 4d55 4c54 4950 4f4c 5947        MULTIPOLYG
+00001900: 4f4e 2028 2828 3938 3132 3139 2e30 3535  ON (((981219.055
+00001910: 3738 3631 3332 3820 3138 3836 3535 2e33  7861328 188655.3
+00001920: 3135 3739 2e2e 2e0a 2020 2020 3220 2020  1579....    2   
+00001930: 2020 2020 2020 4d55 4c54 4950 4f4c 5947        MULTIPOLYG
+00001940: 4f4e 2028 2828 3130 3132 3832 312e 3830  ON (((1012821.80
+00001950: 3537 3836 3133 3320 3232 3932 3238 2e32  5786133 229228.2
+00001960: 3634 3538 2e2e 2e0a 2020 2020 3320 2020  6458....    3   
+00001970: 2020 2020 2020 4d55 4c54 4950 4f4c 5947        MULTIPOLYG
+00001980: 4f4e 2028 2828 3130 3231 3137 362e 3437  ON (((1021176.47
+00001990: 3930 3033 3930 3620 3135 3133 3734 2e37  9003906 151374.7
+000019a0: 3936 3939 2e2e 2e0a 2020 2020 3420 2020  9699....    4   
+000019b0: 2020 2020 2020 4d55 4c54 4950 4f4c 5947        MULTIPOLYG
+000019c0: 4f4e 2028 2828 3130 3239 3630 362e 3037  ON (((1029606.07
+000019d0: 3635 3939 3132 3120 3135 3630 3733 2e38  6599121 156073.8
+000019e0: 3134 3230 2e2e 2e0a 2020 2020 3520 2020  1420....    5   
+000019f0: 2020 2020 2020 4d55 4c54 4950 4f4c 5947        MULTIPOLYG
+00001a00: 4f4e 2028 2828 3937 3032 3137 2e30 3232  ON (((970217.022
+00001a10: 3339 3939 3032 3320 3134 3536 3433 2e33  3999023 145643.3
+00001a20: 3332 3231 2e2e 2e0a 0a21 5b4e 6577 2059  3221.....![New Y
+00001a30: 6f72 6b20 4369 7479 2062 6f72 6f75 6768  ork City borough
+00001a40: 735d 2864 6f63 2f73 6f75 7263 652f 6761  s](doc/source/ga
+00001a50: 6c6c 6572 792f 6e79 632e 706e 6729 0a0a  llery/nyc.png)..
+00001a60: 2020 2020 3e3e 3e20 626f 726f 735b 2767      >>> boros['g
+00001a70: 656f 6d65 7472 7927 5d2e 636f 6e76 6578  eometry'].convex
+00001a80: 5f68 756c 6c0a 2020 2020 426f 726f 436f  _hull.    BoroCo
+00001a90: 6465 0a20 2020 2031 2020 2020 504f 4c59  de.    1    POLY
+00001aa0: 474f 4e20 2828 3937 3738 3535 2e34 3435  GON ((977855.445
+00001ab0: 3139 3034 3239 3720 3138 3830 3832 2e33  1904297 188082.3
+00001ac0: 3232 3338 3736 3935 332c 2e2e 2e0a 2020  223876953,....  
+00001ad0: 2020 3220 2020 2050 4f4c 5947 4f4e 2028    2    POLYGON (
+00001ae0: 2831 3031 3739 3439 2e39 3737 3630 3030  (1017949.9776000
+00001af0: 3938 2032 3235 3432 362e 3838 3435 3832  98 225426.884582
+00001b00: 3531 3935 2c2e 2e2e 0a20 2020 2033 2020  5195,....    3  
+00001b10: 2020 504f 4c59 474f 4e20 2828 3938 3838    POLYGON ((9888
+00001b20: 3732 2e38 3231 3232 3830 3237 3320 3134  72.8212280273 14
+00001b30: 3637 3732 2e30 3331 3739 3933 3136 342c  6772.0317993164,
+00001b40: 2e2e 2e0a 2020 2020 3420 2020 2050 4f4c  ....    4    POL
+00001b50: 5947 4f4e 2028 2831 3030 3037 3231 2e35  YGON ((1000721.5
+00001b60: 3331 3739 3933 3136 2031 3336 3638 312e  31799316 136681.
+00001b70: 3737 3631 3834 3038 322c 202e 2e2e 0a20  776184082, .... 
+00001b80: 2020 2035 2020 2020 504f 4c59 474f 4e20     5    POLYGON 
+00001b90: 2828 3931 3535 3137 2e36 3837 3734 3538  ((915517.6877458
+00001ba0: 3131 3420 3132 3031 3231 2e38 3831 3235  114 120121.88125
+00001bb0: 3433 3337 322c 2e2e 2e0a 2020 2020 6474  43372,....    dt
+00001bc0: 7970 653a 2067 656f 6d65 7472 790a 0a21  ype: geometry..!
+00001bd0: 5b43 6f6e 7665 7820 6875 6c6c 7320 6f66  [Convex hulls of
+00001be0: 204e 6577 2059 6f72 6b20 4369 7479 2062   New York City b
+00001bf0: 6f72 6f75 6768 735d 2864 6f63 2f73 6f75  oroughs](doc/sou
+00001c00: 7263 652f 6761 6c6c 6572 792f 6e79 635f  rce/gallery/nyc_
+00001c10: 6875 6c6c 2e70 6e67 290a                 hull.png).
```

### Comparing `geopandas-0.9.0/geopandas/_config.py` & `geopandas-1.0.0a1/geopandas/_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 Lightweight options machinery.
 
 Based on https://github.com/topper-123/optioneer, but simplified (don't deal
 with nested options, deprecated options, ..), just the attribute-style dict
 like holding the options and giving a nice repr.
 """
+
 from collections import namedtuple
 import textwrap
 
 
 Option = namedtuple("Option", "key default_value doc validator callback")
 
 
 class Options(object):
     """Provide attribute-style access to configuration dict."""
 
     def __init__(self, options):
-        super(Options, self).__setattr__("_options", options)
+        super().__setattr__("_options", options)
         # populate with default values
         config = {}
         for key, option in options.items():
             config[key] = option.default_value
 
-        super(Options, self).__setattr__("_config", config)
+        super().__setattr__("_config", config)
 
     def __setattr__(self, key, value):
         # you can't set new keys
         if key in self._config:
             option = self._options[key]
             if option.validator:
                 option.validator(value)
@@ -46,47 +47,30 @@
     def __dir__(self):
         return list(self._config.keys())
 
     def __repr__(self):
         cls = self.__class__.__name__
         description = ""
         for key, option in self._options.items():
-            descr = u"{key}: {cur!r} [default: {default!r}]\n".format(
+            descr = "{key}: {cur!r} [default: {default!r}]\n".format(
                 key=key, cur=self._config[key], default=option.default_value
             )
             description += descr
 
             if option.doc:
                 doc_text = "\n".join(textwrap.wrap(option.doc, width=70))
             else:
-                doc_text = u"No description available."
-            doc_text = indent(doc_text, prefix="    ")
+                doc_text = "No description available."
+            doc_text = textwrap.indent(doc_text, prefix="    ")
             description += doc_text + "\n"
         space = "\n  "
         description = description.replace("\n", space)
         return "{}({}{})".format(cls, space, description)
 
 
-def indent(text, prefix, predicate=None):
-    """
-    This is the python 3 textwrap.indent function, which is not available in
-    python 2.
-    """
-    if predicate is None:
-
-        def predicate(line):
-            return line.strip()
-
-    def prefixed_lines():
-        for line in text.splitlines(True):
-            yield (prefix + line if predicate(line) else line)
-
-    return "".join(prefixed_lines())
-
-
 def _validate_display_precision(value):
     if value is not None:
         if not isinstance(value, int) or not (0 <= value <= 16):
             raise ValueError("Invalid value, needs to be an integer [0-16]")
 
 
 display_precision = Option(
@@ -104,34 +88,44 @@
 
 
 def _validate_bool(value):
     if not isinstance(value, bool):
         raise TypeError("Expected bool value, got {0}".format(type(value)))
 
 
-def _default_use_pygeos():
-    import geopandas._compat as compat
-
-    return compat.USE_PYGEOS
-
-
-def _callback_use_pygeos(key, value):
-    assert key == "use_pygeos"
-    import geopandas._compat as compat
+def _validate_io_engine(value):
+    if value is not None:
+        if value not in ("pyogrio", "fiona"):
+            raise ValueError(f"Expected 'pyogrio' or 'fiona', got '{value}'")
 
-    compat.set_use_pygeos(value)
 
+io_engine = Option(
+    key="io_engine",
+    default_value=None,
+    doc=(
+        "The default engine for ``read_file`` and ``to_file``. "
+        "Options are 'pyogrio' and 'fiona'."
+    ),
+    validator=_validate_io_engine,
+    callback=None,
+)
 
+# TODO: deprecate this
 use_pygeos = Option(
     key="use_pygeos",
-    default_value=_default_use_pygeos(),
+    default_value=False,
     doc=(
         "Whether to use PyGEOS to speed up spatial operations. The default is True "
         "if PyGEOS is installed, and follows the USE_PYGEOS environment variable "
         "if set."
     ),
     validator=_validate_bool,
-    callback=_callback_use_pygeos,
+    callback=None,
 )
 
-
-options = Options({"display_precision": display_precision, "use_pygeos": use_pygeos})
+options = Options(
+    {
+        "display_precision": display_precision,
+        "use_pygeos": use_pygeos,
+        "io_engine": io_engine,
+    }
+)
```

### Comparing `geopandas-0.9.0/geopandas/array.py` & `geopandas-1.0.0a1/geopandas/array.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,53 @@
-from collections.abc import Iterable
+import inspect
 import numbers
 import operator
 import warnings
-import inspect
+from functools import lru_cache
 
 import numpy as np
 import pandas as pd
+import shapely
+import shapely.affinity
+import shapely.geometry
+import shapely.ops
+import shapely.wkt
 from pandas.api.extensions import (
     ExtensionArray,
     ExtensionDtype,
     register_extension_dtype,
 )
 
-import shapely
-import shapely.affinity
-import shapely.geometry
 from shapely.geometry.base import BaseGeometry
-import shapely.ops
-import shapely.wkt
-from pyproj import CRS, Transformer
 
-try:
-    import pygeos
-except ImportError:
-    geos = None
-
-from . import _compat as compat
-from . import _vectorized as vectorized
-from .sindex import _get_sindex_class
+from .sindex import SpatialIndex
+from ._compat import HAS_PYPROJ, requires_pyproj
+
+if HAS_PYPROJ:
+    from pyproj import Transformer
+
+    TransformerFromCRS = lru_cache(Transformer.from_crs)
+
+_names = {
+    "MISSING": None,
+    "NAG": None,
+    "POINT": "Point",
+    "LINESTRING": "LineString",
+    "LINEARRING": "LinearRing",
+    "POLYGON": "Polygon",
+    "MULTIPOINT": "MultiPoint",
+    "MULTILINESTRING": "MultiLineString",
+    "MULTIPOLYGON": "MultiPolygon",
+    "GEOMETRYCOLLECTION": "GeometryCollection",
+}
+
+
+type_mapping = {p.value: _names[p.name] for p in shapely.GeometryType}
+geometry_type_ids = list(type_mapping.keys())
+geometry_type_values = np.array(list(type_mapping.values()), dtype=object)
 
 
 class GeometryDtype(ExtensionDtype):
     type = BaseGeometry
     name = "geometry"
     na_value = np.nan
 
@@ -52,31 +68,14 @@
     def construct_array_type(cls):
         return GeometryArray
 
 
 register_extension_dtype(GeometryDtype)
 
 
-def _isna(value):
-    """
-    Check if scalar value is NA-like (None, np.nan or pd.NA).
-
-    Custom version that only works for scalars (returning True or False),
-    as `pd.isna` also works for array-like input returning a boolean array.
-    """
-    if value is None:
-        return True
-    elif isinstance(value, float) and np.isnan(value):
-        return True
-    elif compat.PANDAS_GE_10 and value is pd.NA:
-        return True
-    else:
-        return False
-
-
 def _check_crs(left, right, allow_none=False):
     """
     Check if the projection of both arrays is the same.
 
     If allow_none is True, empty CRS is treated as the same.
     """
     if allow_none:
@@ -113,44 +112,38 @@
         "Left CRS: {0}\n"
         "Right CRS: {1}\n".format(left_srs, right_srs),
         UserWarning,
         stacklevel=stacklevel,
     )
 
 
-# -----------------------------------------------------------------------------
-# Constructors / converters to other formats
-# -----------------------------------------------------------------------------
-
-
-def _geom_to_shapely(geom):
+def isna(value):
     """
-    Convert internal representation (PyGEOS or Shapely) to external Shapely object.
+    Check if scalar value is NA-like (None, np.nan or pd.NA).
+
+    Custom version that only works for scalars (returning True or False),
+    as `pd.isna` also works for array-like input returning a boolean array.
     """
-    if not compat.USE_PYGEOS:
-        return geom
+    if value is None:
+        return True
+    elif isinstance(value, float) and np.isnan(value):
+        return True
+    elif value is pd.NA:
+        return True
     else:
-        return vectorized._pygeos_to_shapely(geom)
+        return False
 
 
-def _shapely_to_geom(geom):
-    """
-    Convert external Shapely object to internal representation (PyGEOS or Shapely).
-    """
-    if not compat.USE_PYGEOS:
-        return geom
-    else:
-        return vectorized._shapely_to_pygeos(geom)
+# -----------------------------------------------------------------------------
+# Constructors / converters to other formats
+# -----------------------------------------------------------------------------
 
 
 def _is_scalar_geometry(geom):
-    if compat.USE_PYGEOS:
-        return isinstance(geom, (pygeos.Geometry, BaseGeometry))
-    else:
-        return isinstance(geom, BaseGeometry)
+    return isinstance(geom, BaseGeometry)
 
 
 def from_shapely(data, crs=None):
     """
     Convert a list or array of shapely objects to a GeometryArray.
 
     Validates the elements.
@@ -161,76 +154,109 @@
         list or array of shapely objects
     crs : value, optional
         Coordinate Reference System of the geometry objects. Can be anything accepted by
         :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
         such as an authority string (eg "EPSG:4326") or a WKT string.
 
     """
-    return GeometryArray(vectorized.from_shapely(data), crs=crs)
+    if not isinstance(data, np.ndarray):
+        arr = np.empty(len(data), dtype=object)
+        arr[:] = data
+    else:
+        arr = data
+
+    if not shapely.is_valid_input(arr).all():
+        out = []
+
+        for geom in data:
+            if isinstance(geom, BaseGeometry):
+                out.append(geom)
+            elif hasattr(geom, "__geo_interface__"):
+                geom = shapely.geometry.shape(geom)
+                out.append(geom)
+            elif isna(geom):
+                out.append(None)
+            else:
+                raise TypeError(
+                    "Input must be valid geometry objects: {0}".format(geom)
+                )
+        arr = np.array(out, dtype=object)
+
+    return GeometryArray(arr, crs=crs)
 
 
 def to_shapely(geoms):
     """
     Convert GeometryArray to numpy object array of shapely objects.
     """
     if not isinstance(geoms, GeometryArray):
         raise ValueError("'geoms' must be a GeometryArray")
-    return vectorized.to_shapely(geoms.data)
+    return geoms._data
 
 
-def from_wkb(data, crs=None):
+def from_wkb(data, crs=None, on_invalid="raise"):
     """
     Convert a list or array of WKB objects to a GeometryArray.
 
     Parameters
     ----------
     data : array-like
         list or array of WKB objects
     crs : value, optional
         Coordinate Reference System of the geometry objects. Can be anything accepted by
         :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
         such as an authority string (eg "EPSG:4326") or a WKT string.
+    on_invalid: {"raise", "warn", "ignore"}, default "raise"
+        - raise: an exception will be raised if a WKB input geometry is invalid.
+        - warn: a warning will be raised and invalid WKB geometries will be returned as
+          None.
+        - ignore: invalid WKB geometries will be returned as None without a warning.
 
     """
-    return GeometryArray(vectorized.from_wkb(data), crs=crs)
+    return GeometryArray(shapely.from_wkb(data, on_invalid=on_invalid), crs=crs)
 
 
 def to_wkb(geoms, hex=False, **kwargs):
     """
     Convert GeometryArray to a numpy object array of WKB objects.
     """
     if not isinstance(geoms, GeometryArray):
         raise ValueError("'geoms' must be a GeometryArray")
-    return vectorized.to_wkb(geoms.data, hex=hex, **kwargs)
+    return shapely.to_wkb(geoms, hex=hex, **kwargs)
 
 
-def from_wkt(data, crs=None):
+def from_wkt(data, crs=None, on_invalid="raise"):
     """
     Convert a list or array of WKT objects to a GeometryArray.
 
     Parameters
     ----------
     data : array-like
         list or array of WKT objects
     crs : value, optional
         Coordinate Reference System of the geometry objects. Can be anything accepted by
         :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
         such as an authority string (eg "EPSG:4326") or a WKT string.
+    on_invalid : {"raise", "warn", "ignore"}, default "raise"
+        - raise: an exception will be raised if a WKT input geometry is invalid.
+        - warn: a warning will be raised and invalid WKT geometries will be
+          returned as ``None``.
+        - ignore: invalid WKT geometries will be returned as ``None`` without a warning.
 
     """
-    return GeometryArray(vectorized.from_wkt(data), crs=crs)
+    return GeometryArray(shapely.from_wkt(data, on_invalid=on_invalid), crs=crs)
 
 
 def to_wkt(geoms, **kwargs):
     """
     Convert GeometryArray to a numpy object array of WKT objects.
     """
     if not isinstance(geoms, GeometryArray):
         raise ValueError("'geoms' must be a GeometryArray")
-    return vectorized.to_wkt(geoms.data, **kwargs)
+    return shapely.to_wkt(geoms, **kwargs)
 
 
 def points_from_xy(x, y, z=None, crs=None):
     """
     Generate GeometryArray of shapely Point geometries from x, y(, z) coordinates.
 
     In case of geographic coordinates, it is assumed that longitude is captured by
@@ -268,49 +294,54 @@
     2        123        48
     >>> geometry = geopandas.points_from_xy(df.longitude, df.latitude, crs="EPSG:4326")
 
     Returns
     -------
     output : GeometryArray
     """
-    return GeometryArray(vectorized.points_from_xy(x, y, z), crs=crs)
+    x = np.asarray(x, dtype="float64")
+    y = np.asarray(y, dtype="float64")
+    if z is not None:
+        z = np.asarray(z, dtype="float64")
+
+    return GeometryArray(shapely.points(x, y, z), crs=crs)
 
 
 class GeometryArray(ExtensionArray):
     """
     Class wrapping a numpy array of Shapely objects and
     holding the array-based implementations.
     """
 
     _dtype = GeometryDtype()
 
     def __init__(self, data, crs=None):
         if isinstance(data, self.__class__):
             if not crs:
                 crs = data.crs
-            data = data.data
+            data = data._data
         elif not isinstance(data, np.ndarray):
             raise TypeError(
                 "'data' should be array of geometry objects. Use from_shapely, "
                 "from_wkb, from_wkt functions to construct a GeometryArray."
             )
         elif not data.ndim == 1:
             raise ValueError(
                 "'data' should be a 1-dimensional array of geometry objects."
             )
-        self.data = data
+        self._data = data
 
         self._crs = None
         self.crs = crs
         self._sindex = None
 
     @property
     def sindex(self):
         if self._sindex is None:
-            self._sindex = _get_sindex_class()(self.data)
+            self._sindex = SpatialIndex(self._data)
         return self._sindex
 
     @property
     def has_sindex(self):
         """Check the existence of the spatial index without generating it.
 
         Use the `.sindex` attribute on a GeoDataFrame or GeoSeries
@@ -346,15 +377,29 @@
         such as an authority string (eg "EPSG:4326") or a WKT string.
         """
         return self._crs
 
     @crs.setter
     def crs(self, value):
         """Sets the value of the crs"""
-        self._crs = None if not value else CRS.from_user_input(value)
+        if HAS_PYPROJ:
+            from pyproj import CRS
+
+            self._crs = None if not value else CRS.from_user_input(value)
+        else:
+            if value is not None:
+                warnings.warn(
+                    "Cannot set the CRS, falling back to None. The CRS support requires"
+                    " the 'pyproj' package, but it is not installed or does not import"
+                    " correctly. The functions depending on CRS will raise an error or"
+                    " may produce unexpected results.",
+                    UserWarning,
+                    stacklevel=2,
+                )
+            self._crs = None
 
     def check_geographic_crs(self, stacklevel):
         """Check CRS and warn if the planar operation is done in a geographic CRS"""
         if self.crs and self.crs.is_geographic:
             warnings.warn(
                 "Geometry is in a geographic CRS. Results from '{}' are likely "
                 "incorrect. Use 'GeoSeries.to_crs()' to re-project geometries to a "
@@ -370,54 +415,50 @@
         return self._dtype
 
     def __len__(self):
         return self.shape[0]
 
     def __getitem__(self, idx):
         if isinstance(idx, numbers.Integral):
-            return _geom_to_shapely(self.data[idx])
+            return self._data[idx]
         # array-like, slice
-        if compat.PANDAS_GE_10:
-            # for pandas >= 1.0, validate and convert IntegerArray/BooleanArray
-            # to numpy array, pass-through non-array-like indexers
-            idx = pd.api.indexers.check_array_indexer(self, idx)
-        if isinstance(idx, (Iterable, slice)):
-            return GeometryArray(self.data[idx], crs=self.crs)
-        else:
-            raise TypeError("Index type not supported", idx)
+        # validate and convert IntegerArray/BooleanArray
+        # to numpy array, pass-through non-array-like indexers
+        idx = pd.api.indexers.check_array_indexer(self, idx)
+        return GeometryArray(self._data[idx], crs=self.crs)
 
     def __setitem__(self, key, value):
-        if compat.PANDAS_GE_10:
-            # for pandas >= 1.0, validate and convert IntegerArray/BooleanArray
-            # keys to numpy array, pass-through non-array-like indexers
-            key = pd.api.indexers.check_array_indexer(self, key)
+        # validate and convert IntegerArray/BooleanArray
+        # keys to numpy array, pass-through non-array-like indexers
+        key = pd.api.indexers.check_array_indexer(self, key)
         if isinstance(value, pd.Series):
             value = value.values
+        if isinstance(value, pd.DataFrame):
+            value = value.values.flatten()
         if isinstance(value, (list, np.ndarray)):
             value = from_shapely(value)
         if isinstance(value, GeometryArray):
             if isinstance(key, numbers.Integral):
                 raise ValueError("cannot set a single element with an array")
-            self.data[key] = value.data
-        elif isinstance(value, BaseGeometry) or _isna(value):
-            if _isna(value):
+            self._data[key] = value._data
+        elif isinstance(value, BaseGeometry) or isna(value):
+            if isna(value):
                 # internally only use None as missing value indicator
                 # but accept others
                 value = None
             elif isinstance(value, BaseGeometry):
-                value = from_shapely([value]).data[0]
+                value = from_shapely([value])._data[0]
             else:
                 raise TypeError("should be valid geometry")
             if isinstance(key, (slice, list, np.ndarray)):
                 value_array = np.empty(1, dtype=object)
-                with compat.ignore_shapely2_warnings():
-                    value_array[:] = [value]
-                self.data[key] = value_array
+                value_array[:] = [value]
+                self._data[key] = value_array
             else:
-                self.data[key] = value
+                self._data[key] = value
         else:
             raise TypeError(
                 "Value should be either a BaseGeometry or None, got %s" % str(value)
             )
 
         # invalidate spatial index
         self._sindex = None
@@ -427,105 +468,217 @@
         #     if value.crs and (value.crs != self.crs):
         #         raise ValueError(
         #             "CRS mismatch between CRS of the passed geometries "
         #             "and CRS of existing geometries."
         #         )
 
     def __getstate__(self):
-        if compat.USE_PYGEOS:
-            return (pygeos.to_wkb(self.data), self._crs)
-        else:
-            return self.__dict__
+        return (shapely.to_wkb(self._data), self._crs)
 
     def __setstate__(self, state):
-        if compat.USE_PYGEOS:
-            geoms = pygeos.from_wkb(state[0])
+        if not isinstance(state, dict):
+            # pickle file saved with pygeos
+            geoms = shapely.from_wkb(state[0])
             self._crs = state[1]
             self._sindex = None  # pygeos.STRtree could not be pickled yet
-            self.data = geoms
+            self._data = geoms
             self.base = None
         else:
+            if "data" in state:
+                state["_data"] = state.pop("data")
             if "_crs" not in state:
                 state["_crs"] = None
             self.__dict__.update(state)
 
     # -------------------------------------------------------------------------
     # Geometry related methods
     # -------------------------------------------------------------------------
 
     @property
     def is_valid(self):
-        return vectorized.is_valid(self.data)
+        return shapely.is_valid(self._data)
 
     @property
     def is_empty(self):
-        return vectorized.is_empty(self.data)
+        return shapely.is_empty(self._data)
 
     @property
     def is_simple(self):
-        return vectorized.is_simple(self.data)
+        return shapely.is_simple(self._data)
 
     @property
     def is_ring(self):
-        return vectorized.is_ring(self.data)
+        return shapely.is_ring(self._data)
 
     @property
     def is_closed(self):
-        return vectorized.is_closed(self.data)
+        return shapely.is_closed(self._data)
+
+    @property
+    def is_ccw(self):
+        return shapely.is_ccw(self._data)
 
     @property
     def has_z(self):
-        return vectorized.has_z(self.data)
+        return shapely.has_z(self._data)
 
     @property
     def geom_type(self):
-        return vectorized.geom_type(self.data)
+        res = shapely.get_type_id(self._data)
+        return geometry_type_values[np.searchsorted(geometry_type_ids, res)]
 
     @property
     def area(self):
         self.check_geographic_crs(stacklevel=5)
-        return vectorized.area(self.data)
+        return shapely.area(self._data)
 
     @property
     def length(self):
         self.check_geographic_crs(stacklevel=5)
-        return vectorized.length(self.data)
+        return shapely.length(self._data)
+
+    def count_coordinates(self):
+        out = np.empty(len(self._data), dtype=np.int_)
+        out[:] = [shapely.count_coordinates(s) for s in self._data]
+        return out
+
+    def get_precision(self):
+        return shapely.get_precision(self._data)
 
     #
     # Unary operations that return new geometries
     #
 
     @property
     def boundary(self):
-        return GeometryArray(vectorized.boundary(self.data), crs=self.crs)
+        return GeometryArray(shapely.boundary(self._data), crs=self.crs)
 
     @property
     def centroid(self):
         self.check_geographic_crs(stacklevel=5)
-        return GeometryArray(vectorized.centroid(self.data), crs=self.crs)
+        return GeometryArray(shapely.centroid(self._data), crs=self.crs)
+
+    def concave_hull(self, ratio, allow_holes):
+        return shapely.concave_hull(self._data, ratio=ratio, allow_holes=allow_holes)
 
     @property
     def convex_hull(self):
-        return GeometryArray(vectorized.convex_hull(self.data), crs=self.crs)
+        return GeometryArray(shapely.convex_hull(self._data), crs=self.crs)
+
+    def delaunay_triangles(self, tolerance, only_edges):
+        return GeometryArray(
+            shapely.delaunay_triangles(self._data, tolerance, only_edges),
+            crs=self.crs,
+        )
 
     @property
     def envelope(self):
-        return GeometryArray(vectorized.envelope(self.data), crs=self.crs)
+        return GeometryArray(shapely.envelope(self._data), crs=self.crs)
+
+    def minimum_rotated_rectangle(self):
+        return GeometryArray(shapely.oriented_envelope(self._data), crs=self.crs)
 
     @property
     def exterior(self):
-        return GeometryArray(vectorized.exterior(self.data), crs=self.crs)
+        return GeometryArray(shapely.get_exterior_ring(self._data), crs=self.crs)
+
+    def extract_unique_points(self):
+        return GeometryArray(shapely.extract_unique_points(self._data), crs=self.crs)
+
+    def offset_curve(self, distance, quad_segs=8, join_style="round", mitre_limit=5.0):
+        return GeometryArray(
+            shapely.offset_curve(
+                self._data,
+                distance,
+                quad_segs=quad_segs,
+                join_style=join_style,
+                mitre_limit=mitre_limit,
+            ),
+            crs=self.crs,
+        )
 
     @property
     def interiors(self):
         # no GeometryArray as result
-        return vectorized.interiors(self.data)
+        has_non_poly = False
+        inner_rings = []
+        for geom in self._data:
+            interior_ring_seq = getattr(geom, "interiors", None)
+            # polygon case
+            if interior_ring_seq is not None:
+                inner_rings.append(list(interior_ring_seq))
+            # non-polygon case
+            else:
+                has_non_poly = True
+                inner_rings.append(None)
+        if has_non_poly:
+            warnings.warn(
+                "Only Polygon objects have interior rings. For other "
+                "geometry types, None is returned.",
+                stacklevel=2,
+            )
+        # need to allocate empty first in case of all empty lists in inner_rings
+        data = np.empty(len(inner_rings), dtype=object)
+        data[:] = inner_rings
+        return data
+
+    def remove_repeated_points(self, tolerance=0.0):
+        return GeometryArray(
+            shapely.remove_repeated_points(self._data, tolerance=tolerance),
+            crs=self.crs,
+        )
 
     def representative_point(self):
-        return GeometryArray(vectorized.representative_point(self.data), crs=self.crs)
+        return GeometryArray(shapely.point_on_surface(self._data), crs=self.crs)
+
+    def minimum_bounding_circle(self):
+        return GeometryArray(shapely.minimum_bounding_circle(self._data), crs=self.crs)
+
+    def minimum_bounding_radius(self):
+        return shapely.minimum_bounding_radius(self._data)
+
+    def minimum_clearance(self):
+        return shapely.minimum_clearance(self._data)
+
+    def normalize(self):
+        return GeometryArray(shapely.normalize(self._data), crs=self.crs)
+
+    def make_valid(self):
+        return GeometryArray(shapely.make_valid(self._data), crs=self.crs)
+
+    def reverse(self):
+        return GeometryArray(shapely.reverse(self._data), crs=self.crs)
+
+    def segmentize(self, max_segment_length):
+        return GeometryArray(
+            shapely.segmentize(self._data, max_segment_length),
+            crs=self.crs,
+        )
+
+    def force_2d(self):
+        return GeometryArray(shapely.force_2d(self._data), crs=self.crs)
+
+    def force_3d(self, z=0):
+        return GeometryArray(shapely.force_3d(self._data, z=z), crs=self.crs)
+
+    def transform(self, transformation, include_z=False):
+        return GeometryArray(
+            shapely.transform(self._data, transformation, include_z), crs=self.crs
+        )
+
+    def line_merge(self, directed=False):
+        return GeometryArray(
+            shapely.line_merge(self._data, directed=directed), crs=self.crs
+        )
+
+    def set_precision(self, grid_size, mode="valid_output"):
+        return GeometryArray(
+            shapely.set_precision(self._data, grid_size=grid_size, mode=mode),
+            crs=self.crs,
+        )
 
     #
     # Binary predicates
     #
 
     @staticmethod
     def _binary_method(op, left, right, **kwargs):
@@ -533,27 +686,30 @@
             if len(left) != len(right):
                 msg = "Lengths of inputs do not match. Left: {0}, Right: {1}".format(
                     len(left), len(right)
                 )
                 raise ValueError(msg)
             if not _check_crs(left, right):
                 _crs_mismatch_warn(left, right, stacklevel=7)
-            right = right.data
+            right = right._data
 
-        return getattr(vectorized, op)(left.data, right, **kwargs)
+        return getattr(shapely, op)(left._data, right, **kwargs)
 
     def covers(self, other):
         return self._binary_method("covers", self, other)
 
     def covered_by(self, other):
         return self._binary_method("covered_by", self, other)
 
     def contains(self, other):
         return self._binary_method("contains", self, other)
 
+    def contains_properly(self, other):
+        return self._binary_method("contains_properly", self, other)
+
     def crosses(self, other):
         return self._binary_method("crosses", self, other)
 
     def disjoint(self, other):
         return self._binary_method("disjoint", self, other)
 
     def geom_equals(self, other):
@@ -567,43 +723,39 @@
 
     def touches(self, other):
         return self._binary_method("touches", self, other)
 
     def within(self, other):
         return self._binary_method("within", self, other)
 
+    def dwithin(self, other, distance):
+        self.check_geographic_crs(stacklevel=6)
+        return self._binary_method("dwithin", self, other, distance=distance)
+
     def geom_equals_exact(self, other, tolerance):
         return self._binary_method("equals_exact", self, other, tolerance=tolerance)
 
     def geom_almost_equals(self, other, decimal):
-        return self.geom_equals_exact(other, 0.5 * 10 ** (-decimal))
-        # return _binary_predicate("almost_equals", self, other, decimal=decimal)
-
-    def equals_exact(self, other, tolerance):
-        warnings.warn(
-            "GeometryArray.equals_exact() is now GeometryArray.geom_equals_exact(). "
-            "GeometryArray.equals_exact() will be deprecated in the future.",
-            FutureWarning,
-            stacklevel=2,
-        )
-        return self._binary_method("equals_exact", self, other, tolerance=tolerance)
-
-    def almost_equals(self, other, decimal):
         warnings.warn(
-            "GeometryArray.almost_equals() is now GeometryArray.geom_almost_equals(). "
-            "GeometryArray.almost_equals() will be deprecated in the future.",
+            "The 'geom_almost_equals()' method is deprecated because the name is "
+            "confusing. The 'geom_equals_exact()' method should be used instead.",
             FutureWarning,
             stacklevel=2,
         )
         return self.geom_equals_exact(other, 0.5 * 10 ** (-decimal))
 
     #
     # Binary operations that return new geometries
     #
 
+    def clip_by_rect(self, xmin, ymin, xmax, ymax):
+        return GeometryArray(
+            shapely.clip_by_rect(self._data, xmin, ymin, xmax, ymax), crs=self.crs
+        )
+
     def difference(self, other):
         return GeometryArray(
             self._binary_method("difference", self, other), crs=self.crs
         )
 
     def intersection(self, other):
         return GeometryArray(
@@ -614,114 +766,157 @@
         return GeometryArray(
             self._binary_method("symmetric_difference", self, other), crs=self.crs
         )
 
     def union(self, other):
         return GeometryArray(self._binary_method("union", self, other), crs=self.crs)
 
+    def shortest_line(self, other):
+        return GeometryArray(
+            self._binary_method("shortest_line", self, other), crs=self.crs
+        )
+
+    def snap(self, other, tolerance):
+        return GeometryArray(
+            self._binary_method("snap", self, other, tolerance=tolerance), crs=self.crs
+        )
+
     #
     # Other operations
     #
 
     def distance(self, other):
         self.check_geographic_crs(stacklevel=6)
         return self._binary_method("distance", self, other)
 
+    def hausdorff_distance(self, other, **kwargs):
+        self.check_geographic_crs(stacklevel=6)
+        return self._binary_method("hausdorff_distance", self, other, **kwargs)
+
+    def frechet_distance(self, other, **kwargs):
+        self.check_geographic_crs(stacklevel=6)
+        return self._binary_method("frechet_distance", self, other, **kwargs)
+
     def buffer(self, distance, resolution=16, **kwargs):
         if not (isinstance(distance, (int, float)) and distance == 0):
             self.check_geographic_crs(stacklevel=5)
         return GeometryArray(
-            vectorized.buffer(self.data, distance, resolution=resolution, **kwargs),
+            shapely.buffer(self._data, distance, quad_segs=resolution, **kwargs),
             crs=self.crs,
         )
 
     def interpolate(self, distance, normalized=False):
         self.check_geographic_crs(stacklevel=5)
         return GeometryArray(
-            vectorized.interpolate(self.data, distance, normalized=normalized),
+            shapely.line_interpolate_point(self._data, distance, normalized=normalized),
             crs=self.crs,
         )
 
     def simplify(self, tolerance, preserve_topology=True):
         return GeometryArray(
-            vectorized.simplify(
-                self.data, tolerance, preserve_topology=preserve_topology
+            shapely.simplify(
+                self._data, tolerance, preserve_topology=preserve_topology
             ),
             crs=self.crs,
         )
 
     def project(self, other, normalized=False):
-        if isinstance(other, BaseGeometry):
-            other = _shapely_to_geom(other)
-        elif isinstance(other, GeometryArray):
-            other = other.data
-        return vectorized.project(self.data, other, normalized=normalized)
+        if isinstance(other, GeometryArray):
+            other = other._data
+        return shapely.line_locate_point(self._data, other, normalized=normalized)
 
     def relate(self, other):
         if isinstance(other, GeometryArray):
-            other = other.data
-        return vectorized.relate(self.data, other)
+            other = other._data
+        return shapely.relate(self._data, other)
 
     #
     # Reduction operations that return a Shapely geometry
     #
 
     def unary_union(self):
-        return vectorized.unary_union(self.data)
+        warnings.warn(
+            "The 'unary_union' attribute is deprecated, "
+            "use the 'union_all' method instead.",
+            FutureWarning,
+            stacklevel=2,
+        )
+        return self.union_all()
+
+    def union_all(self):
+        return shapely.union_all(self._data)
 
     #
     # Affinity operations
     #
 
+    @staticmethod
+    def _affinity_method(op, left, *args, **kwargs):
+        # not all shapely.affinity methods can handle empty geometries:
+        # affine_transform itself works (as well as translate), but rotate, scale
+        # and skew fail (they try to unpack the bounds).
+        # Here: consistently returning empty geom for input empty geom
+        out = []
+        for geom in left:
+            if geom is None or geom.is_empty:
+                res = geom
+            else:
+                res = getattr(shapely.affinity, op)(geom, *args, **kwargs)
+            out.append(res)
+        data = np.empty(len(left), dtype=object)
+        data[:] = out
+        return data
+
     def affine_transform(self, matrix):
         return GeometryArray(
-            vectorized._affinity_method("affine_transform", self.data, matrix),
+            self._affinity_method("affine_transform", self._data, matrix),
             crs=self.crs,
         )
 
     def translate(self, xoff=0.0, yoff=0.0, zoff=0.0):
         return GeometryArray(
-            vectorized._affinity_method("translate", self.data, xoff, yoff, zoff),
+            self._affinity_method("translate", self._data, xoff, yoff, zoff),
             crs=self.crs,
         )
 
     def rotate(self, angle, origin="center", use_radians=False):
         return GeometryArray(
-            vectorized._affinity_method(
-                "rotate", self.data, angle, origin=origin, use_radians=use_radians
+            self._affinity_method(
+                "rotate", self._data, angle, origin=origin, use_radians=use_radians
             ),
             crs=self.crs,
         )
 
     def scale(self, xfact=1.0, yfact=1.0, zfact=1.0, origin="center"):
         return GeometryArray(
-            vectorized._affinity_method(
-                "scale", self.data, xfact, yfact, zfact, origin=origin
+            self._affinity_method(
+                "scale", self._data, xfact, yfact, zfact, origin=origin
             ),
             crs=self.crs,
         )
 
     def skew(self, xs=0.0, ys=0.0, origin="center", use_radians=False):
         return GeometryArray(
-            vectorized._affinity_method(
-                "skew", self.data, xs, ys, origin=origin, use_radians=use_radians
+            self._affinity_method(
+                "skew", self._data, xs, ys, origin=origin, use_radians=use_radians
             ),
             crs=self.crs,
         )
 
+    @requires_pyproj
     def to_crs(self, crs=None, epsg=None):
         """Returns a ``GeometryArray`` with all geometries transformed to a new
         coordinate reference system.
 
         Transform all geometries in a GeometryArray to a different coordinate
         reference system.  The ``crs`` attribute on the current GeometryArray must
         be set.  Either ``crs`` or ``epsg`` may be specified for output.
 
         This method will transform all points in all objects.  It has no notion
-        or projecting entire geometries.  All segments joining points are
+        of projecting entire geometries.  All segments joining points are
         assumed to be lines in the current projection, not geodesics.  Objects
         crossing the dateline (or other projection boundary) will have
         undesirable behavior.
 
         Parameters
         ----------
         crs : pyproj.CRS, optional if `epsg` is specified
@@ -753,16 +948,17 @@
         - bounds: (-180.0, -90.0, 180.0, 90.0)
         Datum: World Geodetic System 1984
         - Ellipsoid: WGS 84
         - Prime Meridian: Greenwich
 
         >>> a = a.to_crs(3857)
         >>> to_wkt(a)
-        array(['POINT (111319 111325)', 'POINT (222639 222684)',
-               'POINT (333958 334111)'], dtype=object)
+        array(['POINT (111319.490793 111325.142866)',
+               'POINT (222638.981587 222684.208506)',
+               'POINT (333958.47238 334111.171402)'], dtype=object)
         >>> a.crs  # doctest: +SKIP
         <Projected CRS: EPSG:3857>
         Name: WGS 84 / Pseudo-Mercator
         Axis Info [cartesian]:
         - X[east]: Easting (metre)
         - Y[north]: Northing (metre)
         Area of Use:
@@ -772,14 +968,16 @@
         - name: Popular Visualisation Pseudo-Mercator
         - method: Popular Visualisation Pseudo Mercator
         Datum: World Geodetic System 1984
         - Ellipsoid: WGS 84
         - Prime Meridian: Greenwich
 
         """
+        from pyproj import CRS
+
         if self.crs is None:
             raise ValueError(
                 "Cannot transform naive geometries.  "
                 "Please set a crs on the object first."
             )
         if crs is not None:
             crs = CRS.from_user_input(crs)
@@ -788,19 +986,20 @@
         else:
             raise ValueError("Must pass either crs or epsg.")
 
         # skip if the input CRS and output CRS are the exact same
         if self.crs.is_exact_same(crs):
             return self
 
-        transformer = Transformer.from_crs(self.crs, crs, always_xy=True)
+        transformer = TransformerFromCRS(self.crs, crs, always_xy=True)
 
-        new_data = vectorized.transform(self.data, transformer.transform)
+        new_data = transform(self._data, transformer.transform)
         return GeometryArray(new_data, crs=crs)
 
+    @requires_pyproj
     def estimate_utm_crs(self, datum_name="WGS 84"):
         """Returns the estimated UTM CRS based on the bounds of the dataset.
 
         .. versionadded:: 0.9
 
         .. note:: Requires pyproj 3+
 
@@ -811,54 +1010,63 @@
 
         Returns
         -------
         pyproj.CRS
 
         Examples
         --------
-        >>> world = geopandas.read_file(
-        ...     geopandas.datasets.get_path("naturalearth_lowres")
+        >>> import geodatasets
+        >>> df = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.chicago_commpop")
         ... )
-        >>> germany = world.loc[world.name == "Germany"]
-        >>> germany.geometry.values.estimate_utm_crs()  # doctest: +SKIP
-        <Projected CRS: EPSG:32632>
-        Name: WGS 84 / UTM zone 32N
+        >>> df.geometry.values.estimate_utm_crs()  # doctest: +SKIP
+        <Derived Projected CRS: EPSG:32616>
+        Name: WGS 84 / UTM zone 16N
         Axis Info [cartesian]:
         - E[east]: Easting (metre)
         - N[north]: Northing (metre)
         Area of Use:
-        - name: World - N hemisphere - 6°E to 12°E - by country
-        - bounds: (6.0, 0.0, 12.0, 84.0)
+        - name: Between 90°W and 84°W, northern hemisphere between equator and 84°N,...
+        - bounds: (-90.0, 0.0, -84.0, 84.0)
         Coordinate Operation:
-        - name: UTM zone 32N
+        - name: UTM zone 16N
         - method: Transverse Mercator
-        Datum: World Geodetic System 1984
+        Datum: World Geodetic System 1984 ensemble
         - Ellipsoid: WGS 84
         - Prime Meridian: Greenwich
         """
-        try:
-            from pyproj.aoi import AreaOfInterest
-            from pyproj.database import query_utm_crs_info
-        except ImportError:
-            raise RuntimeError("pyproj 3+ required for estimate_utm_crs.")
+        from pyproj import CRS
+        from pyproj.aoi import AreaOfInterest
+        from pyproj.database import query_utm_crs_info
 
         if not self.crs:
             raise RuntimeError("crs must be set to estimate UTM CRS.")
 
         minx, miny, maxx, maxy = self.total_bounds
+        if self.crs.is_geographic:
+            x_center = np.mean([minx, maxx])
+            y_center = np.mean([miny, maxy])
         # ensure using geographic coordinates
-        if not self.crs.is_geographic:
-            lon, lat = Transformer.from_crs(
-                self.crs, "EPSG:4326", always_xy=True
-            ).transform((minx, maxx, minx, maxx), (miny, miny, maxy, maxy))
-            x_center = np.mean(lon)
-            y_center = np.mean(lat)
         else:
-            x_center = np.mean([minx, maxx])
+            transformer = TransformerFromCRS(self.crs, "EPSG:4326", always_xy=True)
+            minx, miny, maxx, maxy = transformer.transform_bounds(
+                minx, miny, maxx, maxy
+            )
             y_center = np.mean([miny, maxy])
+            # crossed the antimeridian
+            if minx > maxx:
+                # shift maxx from [-180,180] to [0,360]
+                # so both numbers are positive for center calculation
+                # Example: -175 to 185
+                maxx += 360
+                x_center = np.mean([minx, maxx])
+                # shift back to [-180,180]
+                x_center = ((x_center + 180) % 360) - 180
+            else:
+                x_center = np.mean([minx, maxx])
 
         utm_crs_list = query_utm_crs_info(
             datum_name=datum_name,
             area_of_interest=AreaOfInterest(
                 west_lon_degree=x_center,
                 south_lat_degree=y_center,
                 east_lon_degree=x_center,
@@ -874,151 +1082,182 @@
     # Coordinate related properties
     #
 
     @property
     def x(self):
         """Return the x location of point geometries in a GeoSeries"""
         if (self.geom_type[~self.isna()] == "Point").all():
-            return vectorized.get_x(self.data)
+            empty = self.is_empty
+            if empty.any():
+                nonempty = ~empty
+                coords = np.full_like(nonempty, dtype=float, fill_value=np.nan)
+                coords[nonempty] = shapely.get_x(self._data[nonempty])
+                return coords
+            else:
+                return shapely.get_x(self._data)
         else:
             message = "x attribute access only provided for Point geometries"
             raise ValueError(message)
 
     @property
     def y(self):
         """Return the y location of point geometries in a GeoSeries"""
         if (self.geom_type[~self.isna()] == "Point").all():
-            return vectorized.get_y(self.data)
+            empty = self.is_empty
+            if empty.any():
+                nonempty = ~empty
+                coords = np.full_like(nonempty, dtype=float, fill_value=np.nan)
+                coords[nonempty] = shapely.get_y(self._data[nonempty])
+                return coords
+            else:
+                return shapely.get_y(self._data)
         else:
             message = "y attribute access only provided for Point geometries"
             raise ValueError(message)
 
     @property
     def z(self):
         """Return the z location of point geometries in a GeoSeries"""
         if (self.geom_type[~self.isna()] == "Point").all():
-            return vectorized.get_z(self.data)
+            empty = self.is_empty
+            if empty.any():
+                nonempty = ~empty
+                coords = np.full_like(nonempty, dtype=float, fill_value=np.nan)
+                coords[nonempty] = shapely.get_z(self._data[nonempty])
+                return coords
+            else:
+                return shapely.get_z(self._data)
         else:
             message = "z attribute access only provided for Point geometries"
             raise ValueError(message)
 
     @property
     def bounds(self):
-        return vectorized.bounds(self.data)
+        return shapely.bounds(self._data)
 
     @property
     def total_bounds(self):
         if len(self) == 0:
             # numpy 'min' cannot handle empty arrays
             # TODO with numpy >= 1.15, the 'initial' argument can be used
             return np.array([np.nan, np.nan, np.nan, np.nan])
         b = self.bounds
-        return np.array(
-            (
-                np.nanmin(b[:, 0]),  # minx
-                np.nanmin(b[:, 1]),  # miny
-                np.nanmax(b[:, 2]),  # maxx
-                np.nanmax(b[:, 3]),  # maxy
+        with warnings.catch_warnings():
+            # if all rows are empty geometry / none, nan is expected
+            warnings.filterwarnings(
+                "ignore", r"All-NaN slice encountered", RuntimeWarning
+            )
+            return np.array(
+                (
+                    np.nanmin(b[:, 0]),  # minx
+                    np.nanmin(b[:, 1]),  # miny
+                    np.nanmax(b[:, 2]),  # maxx
+                    np.nanmax(b[:, 3]),  # maxy
+                )
             )
-        )
 
     # -------------------------------------------------------------------------
     # general array like compat
     # -------------------------------------------------------------------------
 
     @property
     def size(self):
-        return self.data.size
+        return self._data.size
 
     @property
     def shape(self):
         return (self.size,)
 
     @property
     def ndim(self):
         return len(self.shape)
 
     def copy(self, *args, **kwargs):
         # still taking args/kwargs for compat with pandas 0.24
-        return GeometryArray(self.data.copy(), crs=self._crs)
+        return GeometryArray(self._data.copy(), crs=self._crs)
 
     def take(self, indices, allow_fill=False, fill_value=None):
         from pandas.api.extensions import take
 
         if allow_fill:
             if fill_value is None or pd.isna(fill_value):
                 fill_value = None
-            elif isinstance(fill_value, BaseGeometry):
-                fill_value = _shapely_to_geom(fill_value)
             elif not _is_scalar_geometry(fill_value):
                 raise TypeError("provide geometry or None as fill value")
 
-        result = take(self.data, indices, allow_fill=allow_fill, fill_value=fill_value)
+        result = take(self._data, indices, allow_fill=allow_fill, fill_value=fill_value)
         if allow_fill and fill_value is None:
-            result[pd.isna(result)] = None
+            result[~shapely.is_valid_input(result)] = None
         return GeometryArray(result, crs=self.crs)
 
     def _fill(self, idx, value):
-        """Fill index locations with value
+        """
+        Fill index locations with ``value``.
 
-        Value should be a BaseGeometry
+        ``value`` should be a BaseGeometry or a GeometryArray.
         """
-        if not (_is_scalar_geometry(value) or value is None):
+        if isna(value):
+            value = [None]
+        elif _is_scalar_geometry(value):
+            value = [value]
+        elif isinstance(value, GeometryArray):
+            value = value[idx]
+        else:
             raise TypeError(
-                "Value should be either a BaseGeometry or None, got %s" % str(value)
+                "'value' parameter must be None, a scalar geometry, or a GeoSeries, "
+                f"but you passed a {type(value).__name__!r}"
             )
-        # self.data[idx] = value
-        value_arr = np.empty(1, dtype=object)
-        value_arr[:] = [value]
-        self.data[idx] = value_arr
+
+        value_arr = np.empty(len(value), dtype=object)
+        value_arr[:] = value
+
+        self._data[idx] = value_arr
         return self
 
-    def fillna(self, value=None, method=None, limit=None):
-        """Fill NA/NaN values using the specified method.
+    def fillna(self, value=None, method=None, limit=None, copy=True):
+        """
+        Fill NA values with geometry (or geometries) or using the specified method.
 
         Parameters
         ----------
-        value : scalar, array-like
-            If a scalar value is passed it is used to fill all missing values.
-            Alternatively, an array-like 'value' can be given. It's expected
-            that the array-like have the same length as 'self'.
+        value : shapely geometry object or GeometryArray
+            If a geometry value is passed it is used to fill all missing values.
+            Alternatively, an GeometryArray 'value' can be given. It's expected
+            that the GeometryArray has the same length as 'self'.
+
         method : {'backfill', 'bfill', 'pad', 'ffill', None}, default None
             Method to use for filling holes in reindexed Series
             pad / ffill: propagate last valid observation forward to next valid
             backfill / bfill: use NEXT valid observation to fill gap
+
         limit : int, default None
             If method is specified, this is the maximum number of consecutive
             NaN values to forward/backward fill. In other words, if there is
             a gap with more than this number of consecutive NaNs, it will only
             be partially filled. If method is not specified, this is the
             maximum number of entries along the entire axis where NaNs will be
             filled.
 
+        copy : bool, default True
+            Whether to make a copy of the data before filling. If False, then
+            the original should be modified and no new memory should be allocated.
+
         Returns
         -------
-        filled : ExtensionArray with NA/NaN filled
+        GeometryArray
         """
         if method is not None:
             raise NotImplementedError("fillna with a method is not yet supported")
 
         mask = self.isna()
-        new_values = self.copy()
-
-        if mask.any():
-            # fill with value
-            if _isna(value):
-                value = None
-            elif not isinstance(value, BaseGeometry):
-                raise NotImplementedError(
-                    "fillna currently only supports filling with a scalar geometry"
-                )
-            value = _shapely_to_geom(value)
-            new_values = new_values._fill(mask, value)
-
-        return new_values
+        if copy:
+            new_values = self.copy()
+        else:
+            new_values = self
+        return new_values._fill(mask, value) if mask.any() else new_values
 
     def astype(self, dtype, copy=True):
         """
         Cast to a NumPy array with 'dtype'.
 
         Parameters
         ----------
@@ -1039,31 +1278,65 @@
                 return self.copy()
             else:
                 return self
         elif pd.api.types.is_string_dtype(dtype) and not pd.api.types.is_object_dtype(
             dtype
         ):
             string_values = to_wkt(self)
-            if compat.PANDAS_GE_10:
-                pd_dtype = pd.api.types.pandas_dtype(dtype)
-                if isinstance(pd_dtype, pd.StringDtype):
-                    # ensure to return a pandas string array instead of numpy array
-                    return pd.array(string_values, dtype="string")
+            pd_dtype = pd.api.types.pandas_dtype(dtype)
+            if isinstance(pd_dtype, pd.StringDtype):
+                # ensure to return a pandas string array instead of numpy array
+                return pd.array(string_values, dtype=pd_dtype)
             return string_values.astype(dtype, copy=False)
         else:
-            return np.array(self, dtype=dtype, copy=copy)
+            # numpy 2.0 makes copy=False case strict (errors if cannot avoid the copy)
+            # -> in that case use `np.asarray` as backwards compatible alternative
+            # for `copy=None` (when requiring numpy 2+, this can be cleaned up)
+            if not copy:
+                return np.asarray(self, dtype=dtype)
+            else:
+                return np.array(self, dtype=dtype, copy=copy)
 
     def isna(self):
         """
         Boolean NumPy array indicating if each value is missing
         """
-        if compat.USE_PYGEOS:
-            return pygeos.is_missing(self.data)
-        else:
-            return np.array([g is None for g in self.data], dtype="bool")
+        return shapely.is_missing(self._data)
+
+    def value_counts(
+        self,
+        dropna: bool = True,
+    ):
+        """
+        Compute a histogram of the counts of non-null values.
+
+        Parameters
+        ----------
+        dropna : bool, default True
+            Don't include counts of NaN
+
+        Returns
+        -------
+        pd.Series
+        """
+
+        # note ExtensionArray usage of value_counts only specifies dropna,
+        # so sort, normalize and bins are not arguments
+        values = to_wkb(self)
+        from pandas import Index, Series
+
+        result = Series(values).value_counts(dropna=dropna)
+        # value_counts converts None to nan, need to convert back for from_wkb to work
+        # note result.index already has object dtype, not geometry
+        # Can't use fillna(None) or Index.putmask, as this gets converted back to nan
+        # for object dtypes
+        result.index = Index(
+            from_wkb(np.where(result.index.isna(), None, result.index))
+        )
+        return result
 
     def unique(self):
         """Compute the ExtensionArray of unique values.
 
         Returns
         -------
         uniques : ExtensionArray
@@ -1071,15 +1344,15 @@
         from pandas import factorize
 
         _, uniques = factorize(self)
         return uniques
 
     @property
     def nbytes(self):
-        return self.data.nbytes
+        return self._data.nbytes
 
     def shift(self, periods=1, fill_value=None):
         """
         Shift values by desired number.
 
         Newly introduced missing values are filled with
         ``self.dtype.na_value``.
@@ -1104,15 +1377,15 @@
         If ``self`` is empty or ``periods`` is 0, a copy of ``self`` is
         returned.
 
         If ``periods > len(self)``, then an array of size
         len(self) is returned, with all values filled with
         ``self.dtype.na_value``.
         """
-        shifted = super(GeometryArray, self).shift(periods, fill_value)
+        shifted = super().shift(periods, fill_value)
         shifted.crs = self.crs
         return shifted
 
     # -------------------------------------------------------------------------
     # ExtensionArray specific
     # -------------------------------------------------------------------------
 
@@ -1137,22 +1410,45 @@
         ExtensionArray
         """
         # GH 1413
         if isinstance(scalars, BaseGeometry):
             scalars = [scalars]
         return from_shapely(scalars)
 
+    @classmethod
+    def _from_sequence_of_strings(cls, strings, *, dtype=None, copy=False):
+        """
+        Construct a new ExtensionArray from a sequence of strings.
+
+        Parameters
+        ----------
+        strings : Sequence
+            Each element will be an instance of the scalar type for this
+            array, ``cls.dtype.type``.
+        dtype : dtype, optional
+            Construct for this particular dtype. This should be a Dtype
+            compatible with the ExtensionArray.
+        copy : bool, default False
+            If True, copy the underlying data.
+
+        Returns
+        -------
+        ExtensionArray
+        """
+        # GH 3099
+        return from_wkt(strings)
+
     def _values_for_factorize(self):
         # type: () -> Tuple[np.ndarray, Any]
         """Return an array and missing value suitable for factorization.
 
         Returns
         -------
         values : ndarray
-            An array suitable for factoraization. This should maintain order
+            An array suitable for factorization. This should maintain order
             and be a supported dtype (Float64, Int64, UInt64, String, Object).
             By default, the extension array is cast to object dtype.
         na_value : object
             The value in `values` to consider missing. This will be treated
             as NA in the factorization routines, so it will be coded as
             `na_sentinal` and not included in `uniques`. By default,
             ``np.nan`` is used.
@@ -1190,15 +1486,63 @@
             within the array.
 
         See Also
         --------
         ExtensionArray.argsort
         """
         # Note: this is used in `ExtensionArray.argsort`.
-        raise TypeError("geometries are not orderable")
+        from geopandas.tools.hilbert_curve import _hilbert_distance
+
+        if self.size == 0:
+            # TODO _hilbert_distance fails for empty array
+            return np.array([], dtype="uint32")
+
+        mask_empty = self.is_empty
+        has_empty = mask_empty.any()
+        mask = self.isna() | mask_empty
+        if mask.any():
+            # if there are missing or empty geometries, we fill those with
+            # a dummy geometry so that the _hilbert_distance function can
+            # process those. The missing values are handled separately by
+            # pandas regardless of the values we return here (to sort
+            # first/last depending on 'na_position'), the distances for the
+            # empty geometries are substitued below with an appropriate value
+            geoms = self.copy()
+            indices = np.nonzero(~mask)[0]
+            if indices.size:
+                geom = self[indices[0]]
+            else:
+                # for all-empty/NA, just take random geometry
+                geom = shapely.geometry.Point(0, 0)
+
+            geoms[mask] = geom
+        else:
+            geoms = self
+        if has_empty:
+            # in case we have empty geometries, we need to expand the total
+            # bounds with a small percentage, so the empties can be
+            # deterministically sorted first
+            total_bounds = geoms.total_bounds
+            xoff = (total_bounds[2] - total_bounds[0]) * 0.01
+            yoff = (total_bounds[3] - total_bounds[1]) * 0.01
+            total_bounds += np.array([-xoff, -yoff, xoff, yoff])
+        else:
+            total_bounds = None
+        distances = _hilbert_distance(geoms, total_bounds=total_bounds)
+        if has_empty:
+            # empty geometries are sorted first ("smallest"), so fill in
+            # smallest possible value for uints
+            distances[mask_empty] = 0
+        return distances
+
+    def argmin(self, skipna: bool = True) -> int:
+        raise TypeError("geometries have no minimum or maximum")
+
+    def argmax(self, skipna: bool = True) -> int:
+        raise TypeError("geometries have no minimum or maximum")
 
     def _formatter(self, boxed=False):
         """Formatting function for scalar values.
 
         This is used in the default '__repr__'. The returned formatting
         function receives instances of your scalar type.
 
@@ -1220,32 +1564,39 @@
             ``boxed=True``.
         """
         if boxed:
             import geopandas
 
             precision = geopandas.options.display_precision
             if precision is None:
-                # dummy heuristic based on 10 first geometries that should
-                # work in most cases
-                with warnings.catch_warnings():
-                    warnings.simplefilter("ignore", category=RuntimeWarning)
-                    xmin, ymin, xmax, ymax = self[~self.isna()][:10].total_bounds
-                if (
-                    (-180 <= xmin <= 180)
-                    and (-180 <= xmax <= 180)
-                    and (-90 <= ymin <= 90)
-                    and (-90 <= ymax <= 90)
-                ):
-                    # geographic coordinates
-                    precision = 5
+                if self.crs:
+                    if self.crs.is_projected:
+                        precision = 3
+                    else:
+                        precision = 5
                 else:
-                    # typically projected coordinates
-                    # (in case of unit meter: mm precision)
-                    precision = 3
-            return lambda geom: shapely.wkt.dumps(geom, rounding_precision=precision)
+                    # fallback
+                    # dummy heuristic based on 10 first geometries that should
+                    # work in most cases
+                    with warnings.catch_warnings():
+                        warnings.simplefilter("ignore", category=RuntimeWarning)
+                        xmin, ymin, xmax, ymax = self[~self.isna()][:10].total_bounds
+                    if (
+                        (-180 <= xmin <= 180)
+                        and (-180 <= xmax <= 180)
+                        and (-90 <= ymin <= 90)
+                        and (-90 <= ymax <= 90)
+                    ):
+                        # geographic coordinates
+                        precision = 5
+                    else:
+                        # typically projected coordinates
+                        # (in case of unit meter: mm precision)
+                        precision = 3
+            return lambda geom: shapely.to_wkt(geom, rounding_precision=precision)
         return repr
 
     @classmethod
     def _concat_same_type(cls, to_concat):
         """
         Concatenate multiple array
 
@@ -1253,38 +1604,38 @@
         ----------
         to_concat : sequence of this type
 
         Returns
         -------
         ExtensionArray
         """
-        data = np.concatenate([ga.data for ga in to_concat])
-        return GeometryArray(data, crs=to_concat[0].crs)
+        data = np.concatenate([ga._data for ga in to_concat])
+        return GeometryArray(data, crs=_get_common_crs(to_concat))
 
     def _reduce(self, name, skipna=True, **kwargs):
         # including the base class version here (that raises by default)
         # because this was not yet defined in pandas 0.23
-        if name == "any" or name == "all":
-            # TODO(pygeos)
+        if name in ("any", "all"):
             return getattr(to_shapely(self), name)()
         raise TypeError(
-            "cannot perform {name} with type {dtype}".format(
-                name=name, dtype=self.dtype
-            )
+            f"'{type(self).__name__}' with dtype {self.dtype} "
+            f"does not support reduction '{name}'"
         )
 
-    def __array__(self, dtype=None):
+    def __array__(self, dtype=None, copy=None):
         """
         The numpy array interface.
 
         Returns
         -------
         values : numpy array
         """
-        return to_shapely(self)
+        if copy and (dtype is None or dtype == np.dtype("object")):
+            return self._data.copy()
+        return self._data
 
     def _binop(self, other, op):
         def convert_values(param):
             if not _is_scalar_geometry(param) and (
                 isinstance(param, ExtensionArray) or pd.api.types.is_list_like(param)
             ):
                 ovalues = param
@@ -1315,17 +1666,69 @@
     def __ne__(self, other):
         return self._binop(other, operator.ne)
 
     def __contains__(self, item):
         """
         Return for `item in self`.
         """
-        if _isna(item):
+        if isna(item):
             if (
                 item is self.dtype.na_value
                 or isinstance(item, self.dtype.type)
                 or item is None
             ):
                 return self.isna().any()
             else:
                 return False
         return (self == item).any()
+
+
+def _get_common_crs(arr_seq):
+    # mask out all None arrays with no crs (most likely auto generated by pandas
+    # from concat with missing column)
+    arr_seq = [ga for ga in arr_seq if not (ga.isna().all() and ga.crs is None)]
+    # determine unique crs without using a set, because CRS hash can be different
+    # for objects with the same CRS
+    unique_crs = []
+    for arr in arr_seq:
+        if arr.crs not in unique_crs:
+            unique_crs.append(arr.crs)
+
+    crs_not_none = [crs for crs in unique_crs if crs is not None]
+    names = [crs.name for crs in crs_not_none]
+
+    if len(crs_not_none) == 0:
+        return None
+    if len(crs_not_none) == 1:
+        if len(unique_crs) != 1:
+            warnings.warn(
+                "CRS not set for some of the concatenation inputs. "
+                f"Setting output's CRS as {names[0]} "
+                "(the single non-null crs provided).",
+                stacklevel=2,
+            )
+        return crs_not_none[0]
+
+    raise ValueError(
+        f"Cannot determine common CRS for concatenation inputs, got {names}. "
+        "Use `to_crs()` to transform geometries to the same CRS before merging."
+    )
+
+
+def transform(data, func):
+    has_z = shapely.has_z(data)
+
+    result = np.empty_like(data)
+
+    coords = shapely.get_coordinates(data[~has_z], include_z=False)
+    new_coords_z = func(coords[:, 0], coords[:, 1])
+    result[~has_z] = shapely.set_coordinates(
+        data[~has_z].copy(), np.array(new_coords_z).T
+    )
+
+    coords_z = shapely.get_coordinates(data[has_z], include_z=True)
+    new_coords_z = func(coords_z[:, 0], coords_z[:, 1], coords_z[:, 2])
+    result[has_z] = shapely.set_coordinates(
+        data[has_z].copy(), np.array(new_coords_z).T
+    )
+
+    return result
```

### Comparing `geopandas-0.9.0/geopandas/geodataframe.py` & `geopandas-1.0.0a1/geopandas/geodataframe.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,76 @@
 import json
 import warnings
 
 import numpy as np
 import pandas as pd
+import shapely.errors
 from pandas import DataFrame, Series
+from pandas.core.accessor import CachedAccessor
 
 from shapely.geometry import mapping, shape
 from shapely.geometry.base import BaseGeometry
 
-
-from pyproj import CRS
-
 from geopandas.array import GeometryArray, GeometryDtype, from_shapely, to_wkb, to_wkt
 from geopandas.base import GeoPandasBase, is_geometry_type
-from geopandas.geoseries import GeoSeries, inherit_doc
+from geopandas.geoseries import GeoSeries
 import geopandas.io
-from geopandas.plotting import plot_dataframe
-from . import _compat as compat
+from geopandas.explore import _explore
+from ._decorator import doc
+from ._compat import HAS_PYPROJ
+
 
+def _geodataframe_constructor_with_fallback(*args, **kwargs):
+    """
+    A flexible constructor for GeoDataFrame._constructor, which falls back
+    to returning a DataFrame (if a certain operation does not preserve the
+    geometry column)
+    """
+    df = GeoDataFrame(*args, **kwargs)
+    geometry_cols_mask = df.dtypes == "geometry"
+    if len(geometry_cols_mask) == 0 or geometry_cols_mask.sum() == 0:
+        df = pd.DataFrame(df)
 
-DEFAULT_GEO_COLUMN_NAME = "geometry"
+    return df
 
 
 def _ensure_geometry(data, crs=None):
     """
     Ensure the data is of geometry dtype or converted to it.
 
     If input is a (Geo)Series, output is a GeoSeries, otherwise output
     is GeometryArray.
 
     If the input is a GeometryDtype with a set CRS, `crs` is ignored.
     """
     if is_geometry_type(data):
         if isinstance(data, Series):
-            return GeoSeries(data)
+            data = GeoSeries(data)
+        if data.crs is None and crs is not None:
+            # Avoids caching issues/crs sharing issues
+            data = data.copy()
+            data.crs = crs
         return data
     else:
         if isinstance(data, Series):
             out = from_shapely(np.asarray(data), crs=crs)
             return GeoSeries(out, index=data.index, name=data.name)
         else:
             out = from_shapely(data, crs=crs)
             return out
 
 
+crs_mismatch_error = (
+    "CRS mismatch between CRS of the passed geometries "
+    "and 'crs'. Use 'GeoDataFrame.set_crs(crs, "
+    "allow_override=True)' to overwrite CRS or "
+    "'GeoDataFrame.to_crs(crs)' to reproject geometries. "
+)
+
+
 class GeoDataFrame(GeoPandasBase, DataFrame):
     """
     A GeoDataFrame object is a pandas.DataFrame that has a column
     with geometry. In addition to the standard DataFrame constructor arguments,
     GeoDataFrame also accepts the following keyword arguments:
 
     Parameters
@@ -64,17 +87,17 @@
     --------
     Constructing GeoDataFrame from a dictionary.
 
     >>> from shapely.geometry import Point
     >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
     >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
     >>> gdf
-        col1                 geometry
-    0  name1  POINT (1.00000 2.00000)
-    1  name2  POINT (2.00000 1.00000)
+        col1     geometry
+    0  name1  POINT (1 2)
+    1  name2  POINT (2 1)
 
     Notice that the inferred dtype of 'geometry' columns is geometry.
 
     >>> gdf.dtypes
     col1          object
     geometry    geometry
     dtype: object
@@ -83,137 +106,170 @@
 
     >>> import pandas as pd
     >>> d = {'col1': ['name1', 'name2'], 'wkt': ['POINT (1 2)', 'POINT (2 1)']}
     >>> df = pd.DataFrame(d)
     >>> gs = geopandas.GeoSeries.from_wkt(df['wkt'])
     >>> gdf = geopandas.GeoDataFrame(df, geometry=gs, crs="EPSG:4326")
     >>> gdf
-        col1          wkt                 geometry
-    0  name1  POINT (1 2)  POINT (1.00000 2.00000)
-    1  name2  POINT (2 1)  POINT (2.00000 1.00000)
+        col1          wkt     geometry
+    0  name1  POINT (1 2)  POINT (1 2)
+    1  name2  POINT (2 1)  POINT (2 1)
 
     See also
     --------
     GeoSeries : Series object designed to store shapely geometry objects
     """
 
-    _metadata = ["_crs", "_geometry_column_name"]
+    _metadata = ["_geometry_column_name"]
 
-    _geometry_column_name = DEFAULT_GEO_COLUMN_NAME
+    _internal_names = DataFrame._internal_names + ["geometry"]
+    _internal_names_set = set(_internal_names)
 
-    def __init__(self, *args, geometry=None, crs=None, **kwargs):
-        with compat.ignore_shapely2_warnings():
-            super(GeoDataFrame, self).__init__(*args, **kwargs)
+    _geometry_column_name = None
 
-        # need to set this before calling self['geometry'], because
-        # getitem accesses crs
-        self._crs = CRS.from_user_input(crs) if crs else None
+    def __init__(self, data=None, *args, geometry=None, crs=None, **kwargs):
+        if (
+            kwargs.get("copy") is None
+            and isinstance(data, DataFrame)
+            and not isinstance(data, GeoDataFrame)
+        ):
+            kwargs.update(copy=True)
+        super().__init__(data, *args, **kwargs)
 
         # set_geometry ensures the geometry data have the proper dtype,
         # but is not called if `geometry=None` ('geometry' column present
         # in the data), so therefore need to ensure it here manually
         # but within a try/except because currently non-geometries are
         # allowed in that case
         # TODO do we want to raise / return normal DataFrame in this case?
-        if geometry is None and "geometry" in self.columns:
+
+        # if gdf passed in and geo_col is set, we use that for geometry
+        if geometry is None and isinstance(data, GeoDataFrame):
+            self._geometry_column_name = data._geometry_column_name
+            if crs is not None and data.crs != crs:
+                raise ValueError(crs_mismatch_error)
+
+        if (
+            geometry is None
+            and self.columns.nlevels == 1
+            and "geometry" in self.columns
+        ):
+            # Check for multiple columns with name "geometry". If there are,
+            # self["geometry"] is a gdf and constructor gets recursively recalled
+            # by pandas internals trying to access this
+            if (self.columns == "geometry").sum() > 1:
+                raise ValueError(
+                    "GeoDataFrame does not support multiple columns "
+                    "using the geometry column name 'geometry'."
+                )
+
             # only if we have actual geometry values -> call set_geometry
-            index = self.index
             try:
                 if (
                     hasattr(self["geometry"].values, "crs")
                     and self["geometry"].values.crs
                     and crs
                     and not self["geometry"].values.crs == crs
                 ):
-                    warnings.warn(
-                        "CRS mismatch between CRS of the passed geometries "
-                        "and 'crs'. Use 'GeoDataFrame.set_crs(crs, "
-                        "allow_override=True)' to overwrite CRS or "
-                        "'GeoDataFrame.to_crs(crs)' to reproject geometries. "
-                        "CRS mismatch will raise an error in the future versions "
-                        "of GeoPandas.",
-                        FutureWarning,
-                        stacklevel=2,
-                    )
-                    # TODO: raise error in 0.9 or 0.10.
+                    raise ValueError(crs_mismatch_error)
                 self["geometry"] = _ensure_geometry(self["geometry"].values, crs)
             except TypeError:
                 pass
             else:
-                if self.index is not index:
-                    # With pandas < 1.0 and an empty frame (no rows), the index
-                    # gets reset to a default RangeIndex -> set back the original
-                    # index if needed
-                    self.index = index
                 geometry = "geometry"
 
         if geometry is not None:
             if (
                 hasattr(geometry, "crs")
                 and geometry.crs
                 and crs
                 and not geometry.crs == crs
             ):
-                warnings.warn(
-                    "CRS mismatch between CRS of the passed geometries "
-                    "and 'crs'. Use 'GeoDataFrame.set_crs(crs, "
-                    "allow_override=True)' to overwrite CRS or "
-                    "'GeoDataFrame.to_crs(crs)' to reproject geometries. "
-                    "CRS mismatch will raise an error in the future versions "
-                    "of GeoPandas.",
-                    FutureWarning,
-                    stacklevel=2,
-                )
-                # TODO: raise error in 0.9 or 0.10.
-            self.set_geometry(geometry, inplace=True)
+                raise ValueError(crs_mismatch_error)
+
+            self.set_geometry(geometry, inplace=True, crs=crs)
 
         if geometry is None and crs:
-            warnings.warn(
-                "Assigning CRS to a GeoDataFrame without a geometry column is now "
-                "deprecated and will not be supported in the future.",
-                FutureWarning,
-                stacklevel=2,
+            raise ValueError(
+                "Assigning CRS to a GeoDataFrame without a geometry column is not "
+                "supported. Supply geometry using the 'geometry=' keyword argument, "
+                "or by providing a DataFrame with column name 'geometry'",
             )
 
     def __setattr__(self, attr, val):
         # have to special case geometry b/c pandas tries to use as column...
         if attr == "geometry":
             object.__setattr__(self, attr, val)
         else:
-            super(GeoDataFrame, self).__setattr__(attr, val)
+            super().__setattr__(attr, val)
 
     def _get_geometry(self):
         if self._geometry_column_name not in self:
-            raise AttributeError(
-                "No geometry data set yet (expected in"
-                " column '%s'.)" % self._geometry_column_name
-            )
+            if self._geometry_column_name is None:
+                msg = (
+                    "You are calling a geospatial method on the GeoDataFrame, "
+                    "but the active geometry column to use has not been set. "
+                )
+            else:
+                msg = (
+                    "You are calling a geospatial method on the GeoDataFrame, "
+                    f"but the active geometry column ('{self._geometry_column_name}') "
+                    "is not present. "
+                )
+            geo_cols = list(self.columns[self.dtypes == "geometry"])
+            if len(geo_cols) > 0:
+                msg += (
+                    f"\nThere are columns with geometry data type ({geo_cols}), and "
+                    "you can either set one as the active geometry with "
+                    'df.set_geometry("name") or access the column as a '
+                    'GeoSeries (df["name"]) and call the method directly on it.'
+                )
+            else:
+                msg += (
+                    "\nThere are no existing columns with geometry data type. You can "
+                    "add a geometry column as the active geometry column with "
+                    "df.set_geometry. "
+                )
+
+            raise AttributeError(msg)
         return self[self._geometry_column_name]
 
     def _set_geometry(self, col):
         if not pd.api.types.is_list_like(col):
             raise ValueError("Must use a list-like to set the geometry property")
+        self._persist_old_default_geometry_colname()
         self.set_geometry(col, inplace=True)
 
     geometry = property(
         fget=_get_geometry, fset=_set_geometry, doc="Geometry data for GeoDataFrame"
     )
 
-    def set_geometry(self, col, drop=False, inplace=False, crs=None):
+    def set_geometry(self, col, drop=None, inplace=False, crs=None):
         """
         Set the GeoDataFrame geometry using either an existing column or
         the specified input. By default yields a new object.
 
         The original geometry column is replaced with the input.
 
         Parameters
         ----------
-        col : column label or array
+        col : column label or array-like
+            An existing column name or values to set as the new geometry column.
+            If values (array-like, (Geo)Series) are passed, then if they are named
+            (Series) the new geometry column will have the corresponding name,
+            otherwise the existing geometry column will be replaced. If there is
+            no existing geometry column, the new geometry column will use the
+            default name "geometry".
         drop : boolean, default False
-            Delete column to be used as the new geometry
+            When specifying a named Series or an existing column name for `col`,
+            controls if the previous geometry column should be dropped from the
+            result. The default of False keeps both the old and new geometry column.
+
+            .. deprecated:: 1.0.0
+
         inplace : boolean, default False
             Modify the GeoDataFrame in place (do not create a new object)
         crs : pyproj.CRS, optional
             Coordinate system to use. The value can be anything accepted
             by :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
             such as an authority string (eg "EPSG:4326") or a WKT string.
             If passed, overrides both DataFrame and col's crs.
@@ -221,33 +277,33 @@
 
         Examples
         --------
         >>> from shapely.geometry import Point
         >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
         >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
         >>> gdf
-            col1                 geometry
-        0  name1  POINT (1.00000 2.00000)
-        1  name2  POINT (2.00000 1.00000)
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name2  POINT (2 1)
 
         Passing an array:
 
         >>> df1 = gdf.set_geometry([Point(0,0), Point(1,1)])
         >>> df1
-            col1                 geometry
-        0  name1  POINT (0.00000 0.00000)
-        1  name2  POINT (1.00000 1.00000)
+            col1     geometry
+        0  name1  POINT (0 0)
+        1  name2  POINT (1 1)
 
         Using existing column:
 
         >>> gdf["buffered"] = gdf.buffer(2)
         >>> df2 = gdf.set_geometry("buffered")
         >>> df2.geometry
-        0    POLYGON ((3.00000 2.00000, 2.99037 1.80397, 2....
-        1    POLYGON ((4.00000 1.00000, 3.99037 0.80397, 3....
+        0    POLYGON ((3 2, 2.99037 1.80397, 2.96157 1.6098...
+        1    POLYGON ((4 1, 3.99037 0.80397, 3.96157 0.6098...
         Name: buffered, dtype: geometry
 
         Returns
         -------
         GeoDataFrame
 
         See also
@@ -256,55 +312,84 @@
         """
         # Most of the code here is taken from DataFrame.set_index()
         if inplace:
             frame = self
         else:
             frame = self.copy()
 
-        to_remove = None
         geo_column_name = self._geometry_column_name
+
+        if geo_column_name is None:
+            geo_column_name = "geometry"
         if isinstance(col, (Series, list, np.ndarray, GeometryArray)):
+            if drop:
+                msg = (
+                    "The `drop` keyword argument is deprecated and has no effect when "
+                    "`col` is an array-like value. You should stop passing `drop` to "
+                    "`set_geometry` when this is the case."
+                )
+                warnings.warn(msg, category=FutureWarning, stacklevel=2)
+            if isinstance(col, Series) and col.name is not None:
+                geo_column_name = col.name
+
             level = col
-        elif hasattr(col, "ndim") and col.ndim != 1:
+        elif hasattr(col, "ndim") and col.ndim > 1:
             raise ValueError("Must pass array with one dimension only.")
-        else:
+        else:  # should be a colname
             try:
-                level = frame[col].values
+                level = frame[col]
             except KeyError:
                 raise ValueError("Unknown column %s" % col)
-            except Exception:
-                raise
+            if isinstance(level, DataFrame):
+                raise ValueError(
+                    "GeoDataFrame does not support setting the geometry column where "
+                    "the column name is shared by multiple columns."
+                )
+
+            given_colname_drop_msg = (
+                "The `drop` keyword argument is deprecated and in future the only "
+                "supported behaviour will match drop=False. To silence this "
+                "warning and adopt the future behaviour, stop providing "
+                "`drop` as a keyword to `set_geometry`. To replicate the "
+                "`drop=True` behaviour you should update "
+                "your code to\n`geo_col_name = gdf.active_geometry_name;"
+                " gdf.set_geometry(new_geo_col).drop("
+                "columns=geo_col_name).rename_geometry(geo_col_name)`."
+            )
+
+            if drop is False:  # specifically False, not falsy i.e. None
+                # User supplied False explicitly, but arg is deprecated
+                warnings.warn(
+                    given_colname_drop_msg,
+                    category=FutureWarning,
+                    stacklevel=2,
+                )
             if drop:
-                to_remove = col
-                geo_column_name = self._geometry_column_name
+                del frame[col]
+                warnings.warn(
+                    given_colname_drop_msg,
+                    category=FutureWarning,
+                    stacklevel=2,
+                )
             else:
+                # if not dropping, set the active geometry name to the given col name
                 geo_column_name = col
 
-        if to_remove:
-            del frame[to_remove]
-
         if not crs:
-            level_crs = getattr(level, "crs", None)
-            crs = level_crs if level_crs is not None else self._crs
-
-        if isinstance(level, (GeoSeries, GeometryArray)) and level.crs != crs:
-            # Avoids caching issues/crs sharing issues
-            level = level.copy()
-            level.crs = crs
+            crs = getattr(level, "crs", None)
 
         # Check that we are using a listlike of geometries
         level = _ensure_geometry(level, crs=crs)
-        index = frame.index
-        frame[geo_column_name] = level
-        if frame.index is not index and len(frame.index) == len(index):
-            # With pandas < 1.0 and an empty frame (no rows), the index gets reset
-            # to a default RangeIndex -> set back the original index if needed
-            frame.index = index
+        # ensure_geometry only sets crs on level if it has crs==None
+        level.crs = crs
+        # update _geometry_column_name prior to assignment
+        # to avoid default is None warning
         frame._geometry_column_name = geo_column_name
-        frame.crs = crs
+        frame[geo_column_name] = level
+
         if not inplace:
             return frame
 
     def rename_geometry(self, col, inplace=False):
         """
         Renames the GeoDataFrame geometry column to
         the specified name. By default yields a new object.
@@ -345,14 +430,34 @@
                 return self.rename(columns={geometry_col: col}).set_geometry(
                     col, inplace
                 )
             self.rename(columns={geometry_col: col}, inplace=inplace)
             self.set_geometry(col, inplace=inplace)
 
     @property
+    def active_geometry_name(self):
+        """Return the name of the active geometry column
+
+        Returns a string name if a GeoDataFrame has an active geometry column set.
+        Otherwise returns None. You can also access the active geometry column using the
+        ``.geometry`` property. You can set a GeoSeries to be an active geometry
+        using the :meth:`~GeoDataFrame.set_geometry` method.
+
+        Returns
+        -------
+        str
+            name of an active geometry column or None
+
+        See also
+        --------
+        GeoDataFrame.set_geometry : set the active geometry
+        """
+        return self._geometry_column_name
+
+    @property
     def crs(self):
         """
         The Coordinate Reference System (CRS) represented as a ``pyproj.CRS``
         object.
 
         Returns None if the CRS is not set, and to set the value it
         :getter: Returns a ``pyproj.CRS`` or None. When setting, the value
@@ -378,62 +483,78 @@
 
         See also
         --------
         GeoDataFrame.set_crs : assign CRS
         GeoDataFrame.to_crs : re-project to another CRS
 
         """
-        return self._crs
+        try:
+            return self.geometry.crs
+        except AttributeError:
+            raise AttributeError(
+                "The CRS attribute of a GeoDataFrame without an active "
+                "geometry column is not defined. Use GeoDataFrame.set_geometry "
+                "to set the active geometry column."
+            )
 
     @crs.setter
     def crs(self, value):
         """Sets the value of the crs"""
-        if self._geometry_column_name not in self:
-            warnings.warn(
-                "Assigning CRS to a GeoDataFrame without a geometry column is now "
-                "deprecated and will not be supported in the future.",
-                FutureWarning,
-                stacklevel=4,
+        if self._geometry_column_name is None:
+            raise ValueError(
+                "Assigning CRS to a GeoDataFrame without a geometry column is not "
+                "supported. Use GeoDataFrame.set_geometry to set the active "
+                "geometry column.",
             )
-            self._crs = None if not value else CRS.from_user_input(value)
+
+        if hasattr(self.geometry.values, "crs"):
+            self.geometry.values.crs = value
         else:
-            if hasattr(self.geometry.values, "crs"):
-                self.geometry.values.crs = value
-                self._crs = self.geometry.values.crs
-            else:
-                # column called 'geometry' without geometry
-                self._crs = None if not value else CRS.from_user_input(value)
+            # column called 'geometry' without geometry
+            raise ValueError(
+                "Assigning CRS to a GeoDataFrame without an active geometry "
+                "column is not supported. Use GeoDataFrame.set_geometry to set "
+                "the active geometry column.",
+            )
 
     def __setstate__(self, state):
         # overriding DataFrame method for compat with older pickles (CRS handling)
+        crs = None
         if isinstance(state, dict):
-            if "_metadata" in state and "crs" in state["_metadata"]:
-                metadata = state["_metadata"]
-                metadata[metadata.index("crs")] = "_crs"
             if "crs" in state and "_crs" not in state:
-                crs = state.pop("crs")
-                state["_crs"] = CRS.from_user_input(crs) if crs is not None else crs
+                crs = state.pop("crs", None)
+            else:
+                crs = state.pop("_crs", None)
+            if crs is not None and not HAS_PYPROJ:
+                raise ImportError(
+                    "Unpickling a GeoDataFrame with CRS requires the 'pyproj' package, "
+                    "but it is not installed or does not import correctly. "
+                )
+            elif crs is not None:
+                from pyproj import CRS
+
+                crs = CRS.from_user_input(crs)
 
         super().__setstate__(state)
 
         # for some versions that didn't yet have CRS at array level -> crs is set
         # at GeoDataFrame level with '_crs' (and not 'crs'), so without propagating
         # to the GeoSeries/GeometryArray
         try:
-            if self.crs is not None:
+            if crs is not None:
                 if self.geometry.values.crs is None:
-                    self.crs = self.crs
+                    self.crs = crs
         except Exception:
             pass
 
     @classmethod
     def from_dict(cls, data, geometry=None, crs=None, **kwargs):
         """
         Construct GeoDataFrame from dict of array-like or dicts by
-        overiding DataFrame.from_dict method with geometry and crs
+        overriding DataFrame.from_dict method with geometry and crs
 
         Parameters
         ----------
         data : dict
             Of the form {field : array-like} or {field : dict}.
         geometry : str or array (optional)
             If str, column to use as geometry. If array, will be set as 'geometry'
@@ -444,41 +565,41 @@
             These arguments are passed to DataFrame.from_dict
 
         Returns
         -------
         GeoDataFrame
 
         """
-        dataframe = super().from_dict(data, **kwargs)
-        return GeoDataFrame(dataframe, geometry=geometry, crs=crs)
+        dataframe = DataFrame.from_dict(data, **kwargs)
+        return cls(dataframe, geometry=geometry, crs=crs)
 
     @classmethod
     def from_file(cls, filename, **kwargs):
         """Alternate constructor to create a ``GeoDataFrame`` from a file.
 
         It is recommended to use :func:`geopandas.read_file` instead.
 
         Can load a ``GeoDataFrame`` from a file in any format recognized by
-        `fiona`. See http://fiona.readthedocs.io/en/latest/manual.html for details.
+        `pyogrio`. See http://pyogrio.readthedocs.io/ for details.
 
         Parameters
         ----------
         filename : str
             File path or file handle to read from. Depending on which kwargs
             are included, the content of filename may vary. See
-            http://fiona.readthedocs.io/en/latest/README.html#usage for usage details.
+            :func:`pyogrio.read_dataframe` for usage details.
         kwargs : key-word arguments
-            These arguments are passed to fiona.open, and can be used to
-            access multi-layer data, data stored within archives (zip files),
+            These arguments are passed to :func:`pyogrio.read_dataframe`, and can be
+            used to access multi-layer data, data stored within archives (zip files),
             etc.
 
         Examples
         --------
-
-        >>> path = geopandas.datasets.get_path('nybb')
+        >>> import geodatasets
+        >>> path = geodatasets.get_path('nybb')
         >>> gdf = geopandas.GeoDataFrame.from_file(path)
         >>> gdf  # doctest: +SKIP
            BoroCode       BoroName     Shape_Leng    Shape_Area                 \
                           geometry
         0         5  Staten Island  330470.010332  1.623820e+09  MULTIPOLYGON ((\
 (970217.022 145643.332, 970227....
         1         4         Queens  896344.047763  3.045213e+09  MULTIPOLYGON ((\
@@ -553,17 +674,17 @@
         ...             "bbox": (2.0, 1.0, 2.0, 1.0),
         ...         },
         ...     ],
         ...     "bbox": (1.0, 1.0, 2.0, 2.0),
         ... }
         >>> df = geopandas.GeoDataFrame.from_features(feature_coll)
         >>> df
-                          geometry   col1
-        0  POINT (1.00000 2.00000)  name1
-        1  POINT (2.00000 1.00000)  name2
+              geometry   col1
+        0  POINT (1 2)  name1
+        1  POINT (2 1)  name2
 
         """
         # Handle feature collections
         if hasattr(features, "__geo_interface__"):
             fs = features.__geo_interface__
         else:
             fs = features
@@ -578,17 +699,20 @@
             # load geometry
             if hasattr(feature, "__geo_interface__"):
                 feature = feature.__geo_interface__
             row = {
                 "geometry": shape(feature["geometry"]) if feature["geometry"] else None
             }
             # load properties
-            row.update(feature["properties"])
+            properties = feature["properties"]
+            if properties is None:
+                properties = {}
+            row.update(properties)
             rows.append(row)
-        return GeoDataFrame(rows, columns=columns, crs=crs)
+        return cls(rows, columns=columns, crs=crs)
 
     @classmethod
     def from_postgis(
         cls,
         sql,
         con,
         geom_col="geom",
@@ -632,15 +756,15 @@
             of rows to include in each chunk.
 
         Examples
         --------
         PostGIS
 
         >>> from sqlalchemy import create_engine  # doctest: +SKIP
-        >>> db_connection_url = "postgres://myusername:mypassword@myhost:5432/mydb"
+        >>> db_connection_url = "postgresql://myusername:mypassword@myhost:5432/mydb"
         >>> con = create_engine(db_connection_url)  # doctest: +SKIP
         >>> sql = "SELECT geom, highway FROM roads"
         >>> df = geopandas.GeoDataFrame.from_postgis(sql, con)  # doctest: +SKIP
 
         SpatiaLite
 
         >>> sql = "SELECT ST_Binary(geom) AS geom, highway FROM roads"
@@ -666,171 +790,222 @@
             parse_dates=parse_dates,
             params=params,
             chunksize=chunksize,
         )
 
         return df
 
-    def to_json(self, na="null", show_bbox=False, drop_id=False, **kwargs):
+    def to_json(
+        self, na="null", show_bbox=False, drop_id=False, to_wgs84=False, **kwargs
+    ):
         """
         Returns a GeoJSON representation of the ``GeoDataFrame`` as a string.
 
         Parameters
         ----------
         na : {'null', 'drop', 'keep'}, default 'null'
             Indicates how to output missing (NaN) values in the GeoDataFrame.
             See below.
         show_bbox : bool, optional, default: False
             Include bbox (bounds) in the geojson
         drop_id : bool, default: False
             Whether to retain the index of the GeoDataFrame as the id property
             in the generated GeoJSON. Default is False, but may want True
             if the index is just arbitrary row numbers.
+        to_wgs84: bool, optional, default: False
+            If the CRS is set on the active geometry column it is exported as
+            WGS84 (EPSG:4326) to meet the `2016 GeoJSON specification
+            <https://tools.ietf.org/html/rfc7946>`_.
+            Set to True to force re-projection and set to False to ignore CRS. False by
+            default.
 
         Notes
         -----
         The remaining *kwargs* are passed to json.dumps().
 
         Missing (NaN) values in the GeoDataFrame can be represented as follows:
 
         - ``null``: output the missing entries as JSON null.
         - ``drop``: remove the property from the feature. This applies to each
           feature individually so that features may have different properties.
         - ``keep``: output the missing entries as NaN.
 
+        If the GeoDataFrame has a defined CRS, its definition will be included
+        in the output unless it is equal to WGS84 (default GeoJSON CRS) or not
+        possible to represent in the URN OGC format, or unless ``to_wgs84=True``
+        is specified.
+
         Examples
         --------
 
         >>> from shapely.geometry import Point
         >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
-        >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
+        >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:3857")
         >>> gdf
-            col1                 geometry
-        0  name1  POINT (1.00000 2.00000)
-        1  name2  POINT (2.00000 1.00000)
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name2  POINT (2 1)
 
         >>> gdf.to_json()
         '{"type": "FeatureCollection", "features": [{"id": "0", "type": "Feature", \
 "properties": {"col1": "name1"}, "geometry": {"type": "Point", "coordinates": [1.0,\
  2.0]}}, {"id": "1", "type": "Feature", "properties": {"col1": "name2"}, "geometry"\
-: {"type": "Point", "coordinates": [2.0, 1.0]}}]}'
+: {"type": "Point", "coordinates": [2.0, 1.0]}}], "crs": {"type": "name", "properti\
+es": {"name": "urn:ogc:def:crs:EPSG::3857"}}}'
 
         Alternatively, you can write GeoJSON to file:
 
         >>> gdf.to_file(path, driver="GeoJSON")  # doctest: +SKIP
 
         See also
         --------
         GeoDataFrame.to_file : write GeoDataFrame to file
 
         """
-        return json.dumps(
-            self._to_geo(na=na, show_bbox=show_bbox, drop_id=drop_id), **kwargs
-        )
+        if to_wgs84:
+            if self.crs:
+                df = self.to_crs(epsg=4326)
+            else:
+                raise ValueError(
+                    "CRS is not set. Cannot re-project to WGS84 (EPSG:4326)."
+                )
+        else:
+            df = self
+
+        geo = df.to_geo_dict(na=na, show_bbox=show_bbox, drop_id=drop_id)
+
+        # if the geometry is not in WGS84, include CRS in the JSON
+        if df.crs is not None and not df.crs.equals("epsg:4326"):
+            auth_crsdef = self.crs.to_authority()
+            allowed_authorities = ["EDCS", "EPSG", "OGC", "SI", "UCUM"]
+
+            if auth_crsdef is None or auth_crsdef[0] not in allowed_authorities:
+                warnings.warn(
+                    "GeoDataFrame's CRS is not representable in URN OGC "
+                    "format. Resulting JSON will contain no CRS information.",
+                    stacklevel=2,
+                )
+            else:
+                authority, code = auth_crsdef
+                ogc_crs = f"urn:ogc:def:crs:{authority}::{code}"
+                geo["crs"] = {"type": "name", "properties": {"name": ogc_crs}}
+
+        return json.dumps(geo, **kwargs)
 
     @property
     def __geo_interface__(self):
         """Returns a ``GeoDataFrame`` as a python feature collection.
 
         Implements the `geo_interface`. The returned python data structure
         represents the ``GeoDataFrame`` as a GeoJSON-like
         ``FeatureCollection``.
 
-        This differs from `_to_geo()` only in that it is a property with
-        default args instead of a method
+        This differs from :meth:`to_geo_dict` only in that it is a property with
+        default args instead of a method.
+
+        CRS of the dataframe is not passed on to the output, unlike
+        :meth:`~GeoDataFrame.to_json()`.
 
         Examples
         --------
 
         >>> from shapely.geometry import Point
         >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
         >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
         >>> gdf
-            col1                 geometry
-        0  name1  POINT (1.00000 2.00000)
-        1  name2  POINT (2.00000 1.00000)
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name2  POINT (2 1)
 
         >>> gdf.__geo_interface__
         {'type': 'FeatureCollection', 'features': [{'id': '0', 'type': 'Feature', \
 'properties': {'col1': 'name1'}, 'geometry': {'type': 'Point', 'coordinates': (1.0\
 , 2.0)}, 'bbox': (1.0, 2.0, 1.0, 2.0)}, {'id': '1', 'type': 'Feature', 'properties\
 ': {'col1': 'name2'}, 'geometry': {'type': 'Point', 'coordinates': (2.0, 1.0)}, 'b\
 box': (2.0, 1.0, 2.0, 1.0)}], 'bbox': (1.0, 1.0, 2.0, 2.0)}
-
-
         """
-        return self._to_geo(na="null", show_bbox=True, drop_id=False)
+        return self.to_geo_dict(na="null", show_bbox=True, drop_id=False)
 
     def iterfeatures(self, na="null", show_bbox=False, drop_id=False):
         """
         Returns an iterator that yields feature dictionaries that comply with
         __geo_interface__
 
         Parameters
         ----------
         na : str, optional
             Options are {'null', 'drop', 'keep'}, default 'null'.
             Indicates how to output missing (NaN) values in the GeoDataFrame
-            * null: ouput the missing entries as JSON null
-            * drop: remove the property from the feature. This applies to
-                    each feature individually so that features may have
-                    different properties
-            * keep: output the missing entries as NaN
+
+            - null: output the missing entries as JSON null
+            - drop: remove the property from the feature. This applies to each feature \
+individually so that features may have different properties
+            - keep: output the missing entries as NaN
+
         show_bbox : bool, optional
             Include bbox (bounds) in the geojson. Default False.
         drop_id : bool, default: False
             Whether to retain the index of the GeoDataFrame as the id property
             in the generated GeoJSON. Default is False, but may want True
             if the index is just arbitrary row numbers.
 
         Examples
         --------
 
         >>> from shapely.geometry import Point
         >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
         >>> gdf = geopandas.GeoDataFrame(d, crs="EPSG:4326")
         >>> gdf
-            col1                 geometry
-        0  name1  POINT (1.00000 2.00000)
-        1  name2  POINT (2.00000 1.00000)
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name2  POINT (2 1)
 
         >>> feature = next(gdf.iterfeatures())
         >>> feature
         {'id': '0', 'type': 'Feature', 'properties': {'col1': 'name1'}, 'geometry': {\
 'type': 'Point', 'coordinates': (1.0, 2.0)}}
         """
         if na not in ["null", "drop", "keep"]:
             raise ValueError("Unknown na method {0}".format(na))
 
         if self._geometry_column_name not in self:
             raise AttributeError(
-                "No geometry data set (expected in"
-                " column '%s')." % self._geometry_column_name
+                "No geometry data set (expected in column '%s')."
+                % self._geometry_column_name
             )
 
         ids = np.array(self.index, copy=False)
         geometries = np.array(self[self._geometry_column_name], copy=False)
 
-        properties_cols = self.columns.difference([self._geometry_column_name])
+        if not self.columns.is_unique:
+            raise ValueError("GeoDataFrame cannot contain duplicated column names.")
+
+        properties_cols = self.columns.drop(self._geometry_column_name)
 
         if len(properties_cols) > 0:
             # convert to object to get python scalars.
-            properties = self[properties_cols].astype(object).values
+            properties_cols = self[properties_cols]
+            properties = properties_cols.astype(object)
+            na_mask = pd.isna(properties_cols).values
+
             if na == "null":
-                properties[pd.isnull(self[properties_cols]).values] = None
+                properties[na_mask] = None
 
-            for i, row in enumerate(properties):
+            for i, row in enumerate(properties.values):
                 geom = geometries[i]
 
                 if na == "drop":
+                    na_mask_row = na_mask[i]
                     properties_items = {
-                        k: v for k, v in zip(properties_cols, row) if not pd.isnull(v)
+                        k: v
+                        for k, v, na in zip(properties_cols, row, na_mask_row)
+                        if not na
                     }
                 else:
-                    properties_items = {k: v for k, v in zip(properties_cols, row)}
+                    properties_items = dict(zip(properties_cols, row))
 
                 if drop_id:
                     feature = {}
                 else:
                     feature = {"id": str(ids[i])}
 
                 feature["type"] = "Feature"
@@ -840,41 +1015,82 @@
                 if show_bbox:
                     feature["bbox"] = geom.bounds if geom else None
 
                 yield feature
 
         else:
             for fid, geom in zip(ids, geometries):
-
                 if drop_id:
                     feature = {}
                 else:
                     feature = {"id": str(fid)}
 
                 feature["type"] = "Feature"
                 feature["properties"] = {}
                 feature["geometry"] = mapping(geom) if geom else None
 
                 if show_bbox:
                     feature["bbox"] = geom.bounds if geom else None
 
                 yield feature
 
-    def _to_geo(self, **kwargs):
+    def to_geo_dict(self, na="null", show_bbox=False, drop_id=False):
         """
-        Returns a python feature collection (i.e. the geointerface)
-        representation of the GeoDataFrame.
+        Returns a python feature collection representation of the GeoDataFrame
+        as a dictionary with a list of features based on the ``__geo_interface__``
+        GeoJSON-like specification.
+
+        Parameters
+        ----------
+        na : str, optional
+            Options are {'null', 'drop', 'keep'}, default 'null'.
+            Indicates how to output missing (NaN) values in the GeoDataFrame
+
+            - null: output the missing entries as JSON null
+            - drop: remove the property from the feature. This applies to each feature \
+individually so that features may have different properties
+            - keep: output the missing entries as NaN
+
+        show_bbox : bool, optional
+            Include bbox (bounds) in the geojson. Default False.
+        drop_id : bool, default: False
+            Whether to retain the index of the GeoDataFrame as the id property
+            in the generated dictionary. Default is False, but may want True
+            if the index is just arbitrary row numbers.
+
+        Examples
+        --------
+
+        >>> from shapely.geometry import Point
+        >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
+        >>> gdf = geopandas.GeoDataFrame(d)
+        >>> gdf
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name2  POINT (2 1)
+
+        >>> gdf.to_geo_dict()
+        {'type': 'FeatureCollection', 'features': [{'id': '0', 'type': 'Feature', '\
+properties': {'col1': 'name1'}, 'geometry': {'type': 'Point', 'coordinates': (1.0, \
+2.0)}}, {'id': '1', 'type': 'Feature', 'properties': {'col1': 'name2'}, 'geometry':\
+ {'type': 'Point', 'coordinates': (2.0, 1.0)}}]}
+
+        See also
+        --------
+        GeoDataFrame.to_json : return a GeoDataFrame as a GeoJSON string
 
         """
         geo = {
             "type": "FeatureCollection",
-            "features": list(self.iterfeatures(**kwargs)),
+            "features": list(
+                self.iterfeatures(na=na, show_bbox=show_bbox, drop_id=drop_id)
+            ),
         }
 
-        if kwargs.get("show_bbox", False):
+        if show_bbox:
             geo["bbox"] = tuple(self.total_bounds)
 
         return geo
 
     def to_wkb(self, hex=False, **kwargs):
         """
         Encode all geometry columns in the GeoDataFrame to WKB.
@@ -882,15 +1098,15 @@
         Parameters
         ----------
         hex : bool
             If true, export the WKB as a hexadecimal string.
             The default is to return a binary bytes object.
         kwargs
             Additional keyword args will be passed to
-            :func:`pygeos.to_wkb` if pygeos is installed.
+            :func:`shapely.to_wkb`.
 
         Returns
         -------
         DataFrame
             geometry columns are encoded to WKB
         """
 
@@ -905,16 +1121,15 @@
     def to_wkt(self, **kwargs):
         """
         Encode all geometry columns in the GeoDataFrame to WKT.
 
         Parameters
         ----------
         kwargs
-            Keyword args will be passed to :func:`pygeos.to_wkt`
-            if pygeos is installed.
+            Keyword args will be passed to :func:`shapely.to_wkt`.
 
         Returns
         -------
         DataFrame
             geometry columns are encoded to WKT
         """
 
@@ -922,145 +1137,185 @@
 
         # Encode all geometry columns to WKT
         for col in df.columns[df.dtypes == "geometry"]:
             df[col] = to_wkt(df[col].values, **kwargs)
 
         return df
 
-    def to_parquet(self, path, index=None, compression="snappy", **kwargs):
+    def to_parquet(
+        self, path, index=None, compression="snappy", schema_version=None, **kwargs
+    ):
         """Write a GeoDataFrame to the Parquet format.
 
         Any geometry columns present are serialized to WKB format in the file.
 
         Requires 'pyarrow'.
 
-        WARNING: this is an initial implementation of Parquet file support and
-        associated metadata.  This is tracking version 0.1.0 of the metadata
-        specification at:
-        https://github.com/geopandas/geo-arrow-spec
-
-        This metadata specification does not yet make stability promises.  As such,
-        we do not yet recommend using this in a production setting unless you are
-        able to rewrite your Parquet files.
-
         .. versionadded:: 0.8
 
         Parameters
         ----------
         path : str, path object
         index : bool, default None
             If ``True``, always include the dataframe's index(es) as columns
             in the file output.
             If ``False``, the index(es) will not be written to the file.
             If ``None``, the index(ex) will be included as columns in the file
             output except `RangeIndex` which is stored as metadata only.
         compression : {'snappy', 'gzip', 'brotli', None}, default 'snappy'
             Name of the compression to use. Use ``None`` for no compression.
+        schema_version : {'0.1.0', '0.4.0', '1.0.0', None}
+            GeoParquet specification version; if not provided will default to
+            latest supported version.
         kwargs
-            Additional keyword arguments passed to to pyarrow.parquet.write_table().
+            Additional keyword arguments passed to :func:`pyarrow.parquet.write_table`.
 
         Examples
         --------
 
         >>> gdf.to_parquet('data.parquet')  # doctest: +SKIP
 
         See also
         --------
         GeoDataFrame.to_feather : write GeoDataFrame to feather
         GeoDataFrame.to_file : write GeoDataFrame to file
         """
 
+        # Accept engine keyword for compatibility with pandas.DataFrame.to_parquet
+        # The only engine currently supported by GeoPandas is pyarrow, so no
+        # other engine should be specified.
+        engine = kwargs.pop("engine", "auto")
+        if engine not in ("auto", "pyarrow"):
+            raise ValueError(
+                "GeoPandas only supports using pyarrow as the engine for "
+                f"to_parquet: {engine!r} passed instead."
+            )
+
         from geopandas.io.arrow import _to_parquet
 
-        _to_parquet(self, path, compression=compression, index=index, **kwargs)
+        _to_parquet(
+            self,
+            path,
+            compression=compression,
+            index=index,
+            schema_version=schema_version,
+            **kwargs,
+        )
 
-    def to_feather(self, path, index=None, compression=None, **kwargs):
+    def to_feather(
+        self, path, index=None, compression=None, schema_version=None, **kwargs
+    ):
         """Write a GeoDataFrame to the Feather format.
 
         Any geometry columns present are serialized to WKB format in the file.
 
         Requires 'pyarrow' >= 0.17.
 
-        WARNING: this is an initial implementation of Feather file support and
-        associated metadata.  This is tracking version 0.1.0 of the metadata
-        specification at:
-        https://github.com/geopandas/geo-arrow-spec
-
-        This metadata specification does not yet make stability promises.  As such,
-        we do not yet recommend using this in a production setting unless you are
-        able to rewrite your Feather files.
-
         .. versionadded:: 0.8
 
         Parameters
         ----------
         path : str, path object
         index : bool, default None
             If ``True``, always include the dataframe's index(es) as columns
             in the file output.
             If ``False``, the index(es) will not be written to the file.
             If ``None``, the index(ex) will be included as columns in the file
             output except `RangeIndex` which is stored as metadata only.
         compression : {'zstd', 'lz4', 'uncompressed'}, optional
             Name of the compression to use. Use ``"uncompressed"`` for no
             compression. By default uses LZ4 if available, otherwise uncompressed.
+        schema_version : {'0.1.0', '0.4.0', '1.0.0', None}
+            GeoParquet specification version; if not provided will default to
+            latest supported version.
         kwargs
-            Additional keyword arguments passed to to pyarrow.feather.write_feather().
+            Additional keyword arguments passed to to
+            :func:`pyarrow.feather.write_feather`.
 
         Examples
         --------
 
         >>> gdf.to_feather('data.feather')  # doctest: +SKIP
 
         See also
         --------
         GeoDataFrame.to_parquet : write GeoDataFrame to parquet
         GeoDataFrame.to_file : write GeoDataFrame to file
         """
 
         from geopandas.io.arrow import _to_feather
 
-        _to_feather(self, path, index=index, compression=compression, **kwargs)
+        _to_feather(
+            self,
+            path,
+            index=index,
+            compression=compression,
+            schema_version=schema_version,
+            **kwargs,
+        )
 
-    def to_file(
-        self, filename, driver="ESRI Shapefile", schema=None, index=None, **kwargs
-    ):
+    def to_file(self, filename, driver=None, schema=None, index=None, **kwargs):
         """Write the ``GeoDataFrame`` to a file.
 
         By default, an ESRI shapefile is written, but any OGR data source
-        supported by Fiona can be written. A dictionary of supported OGR
+        supported by Pyogrio or Fiona can be written. A dictionary of supported OGR
         providers is available via:
 
-        >>> import fiona
-        >>> fiona.supported_drivers  # doctest: +SKIP
+        >>> import pyogrio
+        >>> pyogrio.list_drivers()  # doctest: +SKIP
 
         Parameters
         ----------
         filename : string
-            File path or file handle to write to.
-        driver : string, default: 'ESRI Shapefile'
+            File path or file handle to write to. The path may specify a
+            GDAL VSI scheme.
+        driver : string, default None
             The OGR format driver used to write the vector file.
-        schema : dict, default: None
+            If not specified, it attempts to infer it from the file extension.
+            If no extension is specified, it saves ESRI Shapefile to a folder.
+        schema : dict, default None
             If specified, the schema dictionary is passed to Fiona to
-            better control how the file is written.
+            better control how the file is written. If None, GeoPandas
+            will determine the schema based on each column's dtype.
+            Not supported for the "pyogrio" engine.
         index : bool, default None
             If True, write index into one or more columns (for MultiIndex).
             Default None writes the index into one or more columns only if
             the index is named, is a MultiIndex, or has a non-integer data
             type. If False, no index is written.
 
             .. versionadded:: 0.7
                 Previously the index was not written.
+        mode : string, default 'w'
+            The write mode, 'w' to overwrite the existing file and 'a' to append.
+            Not all drivers support appending. The drivers that support appending
+            are listed in fiona.supported_drivers or
+            https://github.com/Toblerity/Fiona/blob/master/fiona/drvsupport.py
+        crs : pyproj.CRS, default None
+            If specified, the CRS is passed to Fiona to
+            better control how the file is written. If None, GeoPandas
+            will determine the crs based on crs df attribute.
+            The value can be anything accepted
+            by :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
+            such as an authority string (eg "EPSG:4326") or a WKT string. The keyword
+            is not supported for the "pyogrio" engine.
+        engine : str, "pyogrio" or "fiona"
+            The underlying library that is used to write the file. Currently, the
+            supported options are "pyogrio" and "fiona". Defaults to "pyogrio" if
+            installed, otherwise tries "fiona".
+        **kwargs :
+            Keyword args to be passed to the engine, and can be used to write
+            to multi-layer data, store data within archives (zip files), etc.
+            In case of the "pyogrio" engine, the keyword arguments are passed to
+            `pyogrio.write_dataframe`. In case of the "fiona" engine, the keyword
+            arguments are passed to fiona.open`. For more information on possible
+            keywords, type: ``import pyogrio; help(pyogrio.write_dataframe)``.
 
         Notes
         -----
-        The extra keyword arguments ``**kwargs`` are passed to fiona.open and
-        can be used to write to multi-layer data, store data within archives
-        (zip files), etc.
-
         The format drivers will attempt to detect the encoding of your data, but
         may fail. In this case, the proper encoding can be specified explicitly
         by using the encoding keyword parameter, e.g. ``encoding='utf-8'``.
 
         See Also
         --------
         GeoSeries.to_file
@@ -1076,14 +1331,22 @@
         >>> gdf.to_file('dataframe.gpkg', driver='GPKG', layer='name')  # doctest: +SKIP
 
         >>> gdf.to_file('dataframe.geojson', driver='GeoJSON')  # doctest: +SKIP
 
         With selected drivers you can also append to a file with `mode="a"`:
 
         >>> gdf.to_file('dataframe.shp', mode="a")  # doctest: +SKIP
+
+        Using the engine-specific keyword arguments it is possible to e.g. create a
+        spatialite file with a custom layer name:
+
+        >>> gdf.to_file(
+        ...     'dataframe.sqlite', driver='SQLite', spatialite=True, layer='test'
+        ... )  # doctest: +SKIP
+
         """
         from geopandas.io.file import _to_file
 
         _to_file(self, filename, driver, schema, index, **kwargs)
 
     def set_crs(self, crs=None, epsg=None, inplace=False, allow_override=False):
         """
@@ -1113,17 +1376,17 @@
 
         Examples
         --------
         >>> from shapely.geometry import Point
         >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
         >>> gdf = geopandas.GeoDataFrame(d)
         >>> gdf
-            col1                 geometry
-        0  name1  POINT (1.00000 2.00000)
-        1  name2  POINT (2.00000 1.00000)
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name2  POINT (2 1)
 
         Setting CRS to a GeoDataFrame without one:
 
         >>> gdf.crs is None
         True
 
         >>> gdf = gdf.set_crs('epsg:3857')
@@ -1168,15 +1431,15 @@
         """Transform geometries to a new coordinate reference system.
 
         Transform all geometries in an active geometry column to a different coordinate
         reference system.  The ``crs`` attribute on the current GeoSeries must
         be set.  Either ``crs`` or ``epsg`` may be specified for output.
 
         This method will transform all points in all objects. It has no notion
-        or projecting entire geometries.  All segments joining points are
+        of projecting entire geometries.  All segments joining points are
         assumed to be lines in the current projection, not geodesics. Objects
         crossing the dateline (or other projection boundary) will have
         undesirable behavior.
 
         Parameters
         ----------
         crs : pyproj.CRS, optional if `epsg` is specified
@@ -1195,17 +1458,17 @@
 
         Examples
         --------
         >>> from shapely.geometry import Point
         >>> d = {'col1': ['name1', 'name2'], 'geometry': [Point(1, 2), Point(2, 1)]}
         >>> gdf = geopandas.GeoDataFrame(d, crs=4326)
         >>> gdf
-            col1                 geometry
-        0  name1  POINT (1.00000 2.00000)
-        1  name2  POINT (2.00000 1.00000)
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name2  POINT (2 1)
         >>> gdf.crs  # doctest: +SKIP
         <Geographic 2D CRS: EPSG:4326>
         Name: WGS 84
         Axis Info [ellipsoidal]:
         - Lat[north]: Geodetic latitude (degree)
         - Lon[east]: Geodetic longitude (degree)
         Area of Use:
@@ -1242,183 +1505,284 @@
         """
         if inplace:
             df = self
         else:
             df = self.copy()
         geom = df.geometry.to_crs(crs=crs, epsg=epsg)
         df.geometry = geom
-        df.crs = geom.crs
         if not inplace:
             return df
 
     def estimate_utm_crs(self, datum_name="WGS 84"):
         """Returns the estimated UTM CRS based on the bounds of the dataset.
 
         .. versionadded:: 0.9
 
-        .. note:: Requires pyproj 3+
-
         Parameters
         ----------
         datum_name : str, optional
             The name of the datum to use in the query. Default is WGS 84.
 
         Returns
         -------
         pyproj.CRS
 
         Examples
         --------
-        >>> world = geopandas.read_file(
-        ...     geopandas.datasets.get_path("naturalearth_lowres")
+        >>> import geodatasets
+        >>> df = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.chicago_health")
         ... )
-        >>> germany = world.loc[world.name == "Germany"]
-        >>> germany.estimate_utm_crs()  # doctest: +SKIP
-        <Projected CRS: EPSG:32632>
-        Name: WGS 84 / UTM zone 32N
+        >>> df.estimate_utm_crs()  # doctest: +SKIP
+        <Derived Projected CRS: EPSG:32616>
+        Name: WGS 84 / UTM zone 16N
         Axis Info [cartesian]:
         - E[east]: Easting (metre)
         - N[north]: Northing (metre)
         Area of Use:
-        - name: World - N hemisphere - 6°E to 12°E - by country
-        - bounds: (6.0, 0.0, 12.0, 84.0)
+        - name: Between 90°W and 84°W, northern hemisphere between equator and 84°N...
+        - bounds: (-90.0, 0.0, -84.0, 84.0)
         Coordinate Operation:
-        - name: UTM zone 32N
+        - name: UTM zone 16N
         - method: Transverse Mercator
-        Datum: World Geodetic System 1984
+        Datum: World Geodetic System 1984 ensemble
         - Ellipsoid: WGS 84
         - Prime Meridian: Greenwich
         """
         return self.geometry.estimate_utm_crs(datum_name=datum_name)
 
     def __getitem__(self, key):
         """
         If the result is a column containing only 'geometry', return a
-        GeoSeries. If it's a DataFrame with a 'geometry' column, return a
-        GeoDataFrame.
+        GeoSeries. If it's a DataFrame with any columns of GeometryDtype,
+        return a GeoDataFrame.
         """
-        result = super(GeoDataFrame, self).__getitem__(key)
+        result = super().__getitem__(key)
+        # Custom logic to avoid waiting for pandas GH51895
+        # result is not geometry dtype for multi-indexes
+        if (
+            pd.api.types.is_scalar(key)
+            and key == ""
+            and isinstance(self.columns, pd.MultiIndex)
+            and isinstance(result, Series)
+            and not is_geometry_type(result)
+        ):
+            loc = self.columns.get_loc(key)
+            # squeeze stops multilevel columns from returning a gdf
+            result = self.iloc[:, loc].squeeze(axis="columns")
         geo_col = self._geometry_column_name
         if isinstance(result, Series) and isinstance(result.dtype, GeometryDtype):
             result.__class__ = GeoSeries
-        elif isinstance(result, DataFrame) and geo_col in result:
-            result.__class__ = GeoDataFrame
-            result._geometry_column_name = geo_col
-        elif isinstance(result, DataFrame) and geo_col not in result:
-            result.__class__ = DataFrame
+        elif isinstance(result, DataFrame):
+            if (result.dtypes == "geometry").sum() > 0:
+                result.__class__ = GeoDataFrame
+                if geo_col in result:
+                    result._geometry_column_name = geo_col
+            else:
+                result.__class__ = DataFrame
         return result
 
+    def _persist_old_default_geometry_colname(self):
+        """Internal util to temporarily persist the default geometry column
+        name of 'geometry' for backwards compatibility."""
+        # self.columns check required to avoid this warning in __init__
+        if self._geometry_column_name is None and "geometry" not in self.columns:
+            msg = (
+                "You are adding a column named 'geometry' to a GeoDataFrame "
+                "constructed without an active geometry column. Currently, "
+                "this automatically sets the active geometry column to 'geometry' "
+                "but in the future that will no longer happen. Instead, either "
+                "provide geometry to the GeoDataFrame constructor "
+                "(GeoDataFrame(... geometry=GeoSeries()) or use "
+                "`set_geometry('geometry')` "
+                "to explicitly set the active geometry column."
+            )
+            warnings.warn(msg, category=FutureWarning, stacklevel=3)
+            self._geometry_column_name = "geometry"
+
     def __setitem__(self, key, value):
         """
         Overwritten to preserve CRS of GeometryArray in cases like
         df['geometry'] = [geom... for geom in df.geometry]
         """
-        if not pd.api.types.is_list_like(key) and key == self._geometry_column_name:
+
+        if not pd.api.types.is_list_like(key) and (
+            key == self._geometry_column_name
+            or key == "geometry"
+            and self._geometry_column_name is None
+        ):
             if pd.api.types.is_scalar(value) or isinstance(value, BaseGeometry):
                 value = [value] * self.shape[0]
             try:
-                value = _ensure_geometry(value, crs=self.crs)
+                if self._geometry_column_name is not None:
+                    crs = getattr(self, "crs", None)
+                else:  # don't use getattr, because a col "crs" might exist
+                    crs = None
+                value = _ensure_geometry(value, crs=crs)
+                if key == "geometry":
+                    self._persist_old_default_geometry_colname()
             except TypeError:
-                warnings.warn("Geometry column does not contain geometry.")
-        super(GeoDataFrame, self).__setitem__(key, value)
+                warnings.warn(
+                    "Geometry column does not contain geometry.",
+                    stacklevel=2,
+                )
+        super().__setitem__(key, value)
 
     #
     # Implement pandas methods
     #
+    @doc(pd.DataFrame)
+    def copy(self, deep=True):
+        copied = super().copy(deep=deep)
+        if type(copied) is pd.DataFrame:
+            copied.__class__ = GeoDataFrame
+            copied._geometry_column_name = self._geometry_column_name
+        return copied
 
-    def merge(self, *args, **kwargs):
-        r"""Merge two ``GeoDataFrame`` objects with a database-style join.
-
-        Returns a ``GeoDataFrame`` if a geometry column is present; otherwise,
-        returns a pandas ``DataFrame``.
-
-        Returns
-        -------
-        GeoDataFrame or DataFrame
-
-        Notes
-        -----
-        The extra arguments ``*args`` and keyword arguments ``**kwargs`` are
-        passed to DataFrame.merge.
-
-        Reference
-        ---------
-        https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas\
-        .DataFrame.merge.html
-
-        """
-        result = DataFrame.merge(self, *args, **kwargs)
-        geo_col = self._geometry_column_name
-        if isinstance(result, DataFrame) and geo_col in result:
-            result.__class__ = GeoDataFrame
-            result.crs = self.crs
-            result._geometry_column_name = geo_col
-        elif isinstance(result, DataFrame) and geo_col not in result:
-            result.__class__ = DataFrame
-        return result
-
-    @inherit_doc(pd.DataFrame)
+    @doc(pd.DataFrame)
     def apply(self, func, axis=0, raw=False, result_type=None, args=(), **kwargs):
         result = super().apply(
             func, axis=axis, raw=raw, result_type=result_type, args=args, **kwargs
         )
+        # Reconstruct gdf if it was lost by apply
         if (
-            isinstance(result, GeoDataFrame)
+            isinstance(result, DataFrame)
             and self._geometry_column_name in result.columns
-            and any(isinstance(t, GeometryDtype) for t in result.dtypes)
         ):
-            if self.crs is not None and result.crs is None:
-                result.set_crs(self.crs, inplace=True)
+            # axis=1 apply will split GeometryDType to object, try and cast back
+            try:
+                result = result.set_geometry(self._geometry_column_name)
+            except TypeError:
+                pass
+            else:
+                if self.crs is not None and result.crs is None:
+                    result.set_crs(self.crs, inplace=True)
+        elif isinstance(result, Series) and result.dtype == "object":
+            # Try reconstruct series GeometryDtype if lost by apply
+            # If all none and object dtype assert list of nones is more likely
+            # intended than list of null geometry.
+            if not result.isna().all():
+                try:
+                    # not enough info about func to preserve CRS
+                    result = _ensure_geometry(result)
+
+                except (TypeError, shapely.errors.GeometryTypeError):
+                    pass
+
         return result
 
     @property
     def _constructor(self):
-        return GeoDataFrame
+        return _geodataframe_constructor_with_fallback
+
+    def _constructor_from_mgr(self, mgr, axes):
+        # replicate _geodataframe_constructor_with_fallback behaviour
+        # unless safe to skip
+        if not any(isinstance(block.dtype, GeometryDtype) for block in mgr.blocks):
+            return _geodataframe_constructor_with_fallback(
+                pd.DataFrame._from_mgr(mgr, axes)
+            )
+        return GeoDataFrame._from_mgr(mgr, axes)
+
+    @property
+    def _constructor_sliced(self):
+        def _geodataframe_constructor_sliced(*args, **kwargs):
+            """
+            A specialized (Geo)Series constructor which can fall back to a
+            Series if a certain operation does not produce geometries:
+
+            - We only return a GeoSeries if the data is actually of geometry
+              dtype (and so we don't try to convert geometry objects such as
+              the normal GeoSeries(..) constructor does with `_ensure_geometry`).
+            - When we get here from obtaining a row or column from a
+              GeoDataFrame, the goal is to only return a GeoSeries for a
+              geometry column, and not return a GeoSeries for a row that happened
+              to come from a DataFrame with only geometry dtype columns (and
+              thus could have a geometry dtype). Therefore, we don't return a
+              GeoSeries if we are sure we are in a row selection case (by
+              checking the identity of the index)
+            """
+            srs = pd.Series(*args, **kwargs)
+            is_row_proxy = srs.index.is_(self.columns)
+            if is_geometry_type(srs) and not is_row_proxy:
+                srs = GeoSeries(srs)
+            return srs
+
+        return _geodataframe_constructor_sliced
+
+    def _constructor_sliced_from_mgr(self, mgr, axes):
+        is_row_proxy = mgr.index.is_(self.columns)
+
+        if isinstance(mgr.blocks[0].dtype, GeometryDtype) and not is_row_proxy:
+            return GeoSeries._from_mgr(mgr, axes)
+        return Series._from_mgr(mgr, axes)
 
     def __finalize__(self, other, method=None, **kwargs):
-        """propagate metadata from other to self """
+        """propagate metadata from other to self"""
         self = super().__finalize__(other, method=method, **kwargs)
 
         # merge operation: using metadata of the left object
         if method == "merge":
             for name in self._metadata:
                 object.__setattr__(self, name, getattr(other.left, name, None))
         # concat operation: using metadata of the first object
         elif method == "concat":
             for name in self._metadata:
                 object.__setattr__(self, name, getattr(other.objs[0], name, None))
 
+            if (self.columns == self._geometry_column_name).sum() > 1:
+                raise ValueError(
+                    "Concat operation has resulted in multiple columns using "
+                    f"the geometry column name '{self._geometry_column_name}'.\n"
+                    "Please ensure this column from the first DataFrame is not "
+                    "repeated."
+                )
+        elif method == "unstack":
+            # unstack adds multiindex columns and reshapes data.
+            # it never makes sense to retain geometry column
+            self._geometry_column_name = None
+            self._crs = None
         return self
 
     def dissolve(
         self,
         by=None,
         aggfunc="first",
         as_index=True,
         level=None,
         sort=True,
         observed=False,
         dropna=True,
+        **kwargs,
     ):
         """
         Dissolve geometries within `groupby` into single observation.
-        This is accomplished by applying the `unary_union` method
+        This is accomplished by applying the `union_all` method
         to all geometries within a groupself.
 
         Observations associated with each `groupby` group will be aggregated
         using the `aggfunc`.
 
         Parameters
         ----------
-        by : string, default None
-            Column whose values define groups to be dissolved. If None,
-            whole GeoDataFrame is considered a single group.
+        by : str or list-like, default None
+            Column(s) whose values define the groups to be dissolved. If None,
+            the entire GeoDataFrame is considered as a single group. If a list-like
+            object is provided, the values in the list are treated as categorical
+            labels, and polygons will be combined based on the equality of
+            these categorical labels.
         aggfunc : function or string, default "first"
             Aggregation function for manipulation of data associated
             with each group. Passed to pandas `groupby.agg` method.
+            Accepted combinations are:
+
+            - function
+            - string function name
+            - list of functions and/or function names, e.g. [np.sum, 'mean']
+            - dict of axis labels -> functions, function names or list of such.
         as_index : boolean, default True
             If true, groupby columns become index of result.
         level : int or str or sequence of int or sequence of str, default None
             If the axis is a MultiIndex (hierarchical), group by a
             particular level or levels.
 
             .. versionadded:: 0.9.0
@@ -1435,70 +1799,90 @@
 
             .. versionadded:: 0.9.0
         dropna : bool, default True
             If True, and if group keys contain NA values, NA values
             together with row/column will be dropped. If False, NA
             values will also be treated as the key in groups.
 
-            This parameter is not supported for pandas < 1.1.0.
-            A warning will be emitted for earlier pandas versions
-            if a non-default value is given for this parameter.
-
             .. versionadded:: 0.9.0
+        **kwargs :
+            Keyword arguments to be passed to the pandas `DataFrameGroupby.agg` method
+            which is used by `dissolve`. In particular, `numeric_only` may be
+            supplied, which will be required in pandas 2.0 for certain aggfuncs.
 
+            .. versionadded:: 0.13.0
         Returns
         -------
         GeoDataFrame
 
         Examples
         --------
         >>> from shapely.geometry import Point
         >>> d = {
         ...     "col1": ["name1", "name2", "name1"],
         ...     "geometry": [Point(1, 2), Point(2, 1), Point(0, 1)],
         ... }
         >>> gdf = geopandas.GeoDataFrame(d, crs=4326)
         >>> gdf
-            col1                 geometry
-        0  name1  POINT (1.00000 2.00000)
-        1  name2  POINT (2.00000 1.00000)
-        2  name1  POINT (0.00000 1.00000)
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name2  POINT (2 1)
+        2  name1  POINT (0 1)
 
         >>> dissolved = gdf.dissolve('col1')
         >>> dissolved  # doctest: +SKIP
-                                                    geometry
+                                geometry
         col1
-        name1  MULTIPOINT (0.00000 1.00000, 1.00000 2.00000)
-        name2                        POINT (2.00000 1.00000)
+        name1  MULTIPOINT ((0 1), (1 2))
+        name2                POINT (2 1)
 
         See also
         --------
-        GeoDataFrame.explode : explode muti-part geometries into single geometries
+        GeoDataFrame.explode : explode multi-part geometries into single geometries
 
         """
 
         if by is None and level is None:
             by = np.zeros(len(self), dtype="int64")
 
-        groupby_kwargs = dict(
-            by=by, level=level, sort=sort, observed=observed, dropna=dropna
-        )
-        if not compat.PANDAS_GE_11:
-            groupby_kwargs.pop("dropna")
-
-            if not dropna:  # If they passed a non-default dropna value
-                warnings.warn("dropna kwarg is not supported for pandas < 1.1.0")
+        groupby_kwargs = {
+            "by": by,
+            "level": level,
+            "sort": sort,
+            "observed": observed,
+            "dropna": dropna,
+        }
 
         # Process non-spatial component
         data = self.drop(labels=self.geometry.name, axis=1)
-        aggregated_data = data.groupby(**groupby_kwargs).agg(aggfunc)
+        with warnings.catch_warnings(record=True) as record:
+            aggregated_data = data.groupby(**groupby_kwargs).agg(aggfunc, **kwargs)
+        for w in record:
+            if str(w.message).startswith("The default value of numeric_only"):
+                msg = (
+                    f"The default value of numeric_only in aggfunc='{aggfunc}' "
+                    "within pandas.DataFrameGroupBy.agg used in dissolve is "
+                    "deprecated. In pandas 2.0, numeric_only will default to False. "
+                    "Either specify numeric_only as additional argument in dissolve() "
+                    "or select only columns which should be valid for the function."
+                )
+                warnings.warn(msg, FutureWarning, stacklevel=2)
+            else:
+                # Only want to capture specific warning,
+                # other warnings from pandas should be passed through
+                # TODO this is not an ideal approach
+                warnings.showwarning(
+                    w.message, w.category, w.filename, w.lineno, w.file, w.line
+                )
+
+        aggregated_data.columns = aggregated_data.columns.to_flat_index()
 
         # Process spatial component
         def merge_geometries(block):
-            merged_geom = block.unary_union
+            merged_geom = block.union_all()
             return merged_geom
 
         g = self.groupby(group_keys=False, **groupby_kwargs)[self.geometry.name].agg(
             merge_geometries
         )
 
         # Aggregate
@@ -1509,26 +1893,36 @@
         # Reset if requested
         if not as_index:
             aggregated = aggregated.reset_index()
 
         return aggregated
 
     # overrides the pandas native explode method to break up features geometrically
-    def explode(self, column=None, **kwargs):
+    def explode(self, column=None, ignore_index=False, index_parts=False, **kwargs):
         """
-        Explode muti-part geometries into multiple single geometries.
+        Explode multi-part geometries into multiple single geometries.
 
         Each row containing a multi-part geometry will be split into
         multiple rows with single geometries, thereby increasing the vertical
         size of the GeoDataFrame.
 
-        The index of the input geodataframe is no longer unique and is
-        replaced with a multi-index (original index with additional level
-        indicating the multiple geometries: a new zero-based index for each
-        single part geometry per multi-part geometry).
+        Parameters
+        ----------
+        column : string, default None
+            Column to explode. In the case of a geometry column, multi-part
+            geometries are converted to single-part.
+            If None, the active geometry column is used.
+        ignore_index : bool, default False
+            If True, the resulting index will be labelled 0, 1, …, n - 1,
+            ignoring `index_parts`.
+        index_parts : boolean, default False
+            If True, the resulting index will be a multi-index (original
+            index with an additional level indicating the multiple
+            geometries: a new zero-based index for each single part geometry
+            per multi-part geometry).
 
         Returns
         -------
         GeoDataFrame
             Exploded geodataframe with each single geometry
             as a separate entry in the geodataframe.
 
@@ -1541,77 +1935,90 @@
         ...     "geometry": [
         ...         MultiPoint([(1, 2), (3, 4)]),
         ...         MultiPoint([(2, 1), (0, 0)]),
         ...     ],
         ... }
         >>> gdf = geopandas.GeoDataFrame(d, crs=4326)
         >>> gdf
-            col1                                       geometry
-        0  name1  MULTIPOINT (1.00000 2.00000, 3.00000 4.00000)
-        1  name2  MULTIPOINT (2.00000 1.00000, 0.00000 0.00000)
+            col1               geometry
+        0  name1  MULTIPOINT ((1 2), (3 4))
+        1  name2  MULTIPOINT ((2 1), (0 0))
+
+        >>> exploded = gdf.explode(index_parts=True)
+        >>> exploded
+              col1     geometry
+        0 0  name1  POINT (1 2)
+          1  name1  POINT (3 4)
+        1 0  name2  POINT (2 1)
+          1  name2  POINT (0 0)
+
+        >>> exploded = gdf.explode(index_parts=False)
+        >>> exploded
+            col1     geometry
+        0  name1  POINT (1 2)
+        0  name1  POINT (3 4)
+        1  name2  POINT (2 1)
+        1  name2  POINT (0 0)
 
-        >>> exploded = gdf.explode()
+        >>> exploded = gdf.explode(ignore_index=True)
         >>> exploded
-              col1                 geometry
-        0 0  name1  POINT (1.00000 2.00000)
-          1  name1  POINT (3.00000 4.00000)
-        1 0  name2  POINT (2.00000 1.00000)
-          1  name2  POINT (0.00000 0.00000)
+            col1     geometry
+        0  name1  POINT (1 2)
+        1  name1  POINT (3 4)
+        2  name2  POINT (2 1)
+        3  name2  POINT (0 0)
 
         See also
         --------
         GeoDataFrame.dissolve : dissolve geometries into a single observation.
 
         """
 
         # If no column is specified then default to the active geometry column
         if column is None:
             column = self.geometry.name
         # If the specified column is not a geometry dtype use pandas explode
         if not isinstance(self[column].dtype, GeometryDtype):
-            return super(GeoDataFrame, self).explode(column, **kwargs)
-            # TODO: make sure index behaviour is consistent
-
-        df_copy = self.copy()
-
-        if "level_1" in df_copy.columns:  # GH1393
-            df_copy = df_copy.rename(columns={"level_1": "__level_1"})
+            return super().explode(column, ignore_index=ignore_index, **kwargs)
 
-        exploded_geom = df_copy.geometry.explode().reset_index(level=-1)
-        exploded_index = exploded_geom.columns[0]
+        exploded_geom = self.geometry.reset_index(drop=True).explode(index_parts=True)
 
-        df = pd.concat(
-            [df_copy.drop(df_copy._geometry_column_name, axis=1), exploded_geom], axis=1
+        df = self.drop(self._geometry_column_name, axis=1).take(
+            exploded_geom.index.droplevel(-1)
         )
-        # reset to MultiIndex, otherwise df index is only first level of
-        # exploded GeoSeries index.
-        df.set_index(exploded_index, append=True, inplace=True)
-        df.index.names = list(self.index.names) + [None]
+        df[exploded_geom.name] = exploded_geom.values
+        df = df.set_geometry(self._geometry_column_name).__finalize__(self)
 
-        if "__level_1" in df.columns:
-            df = df.rename(columns={"__level_1": "level_1"})
+        if ignore_index:
+            df.reset_index(inplace=True, drop=True)
+        elif index_parts:
+            # reset to MultiIndex, otherwise df index is only first level of
+            # exploded GeoSeries index.
+            df = df.set_index(
+                exploded_geom.index.droplevel(
+                    list(range(exploded_geom.index.nlevels - 1))
+                ),
+                append=True,
+            )
 
-        geo_df = df.set_geometry(self._geometry_column_name)
-        return geo_df
+        return df
 
     # overrides the pandas astype method to ensure the correct return type
+    # should be removable when pandas 1.4 is dropped
     def astype(self, dtype, copy=True, errors="raise", **kwargs):
         """
         Cast a pandas object to a specified dtype ``dtype``.
-
         Returns a GeoDataFrame when the geometry column is kept as geometries,
         otherwise returns a pandas DataFrame.
-
         See the pandas.DataFrame.astype docstring for more details.
-
         Returns
         -------
         GeoDataFrame or DataFrame
         """
-        df = super(GeoDataFrame, self).astype(dtype, copy=copy, errors=errors, **kwargs)
+        df = super().astype(dtype, copy=copy, errors=errors, **kwargs)
 
         try:
             geoms = df[self._geometry_column_name]
             if is_geometry_type(geoms):
                 return geopandas.GeoDataFrame(df, geometry=self._geometry_column_name)
         except KeyError:
             pass
@@ -1626,20 +2033,23 @@
         schema=None,
         if_exists="fail",
         index=False,
         index_label=None,
         chunksize=None,
         dtype=None,
     ):
-
         """
         Upload GeoDataFrame into PostGIS database.
 
         This method requires SQLAlchemy and GeoAlchemy2, and a PostgreSQL
-        Python driver (e.g. psycopg2) to be installed.
+        Python driver (psycopg or psycopg2) to be installed.
+
+        It is also possible to use :meth:`~GeoDataFrame.to_file` to write to a database.
+        Especially for file geodatabases like GeoPackage or SpatiaLite this can be
+        easier.
 
         Parameters
         ----------
         name : str
             Name of the target table.
         con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
             Active connection to the PostGIS database.
@@ -1647,15 +2057,15 @@
             How to behave if the table already exists:
 
             - fail: Raise a ValueError.
             - replace: Drop the table before inserting new values.
             - append: Insert new values to the existing table.
         schema : string, optional
             Specify the schema. If None, use default schema: 'public'.
-        index : bool, default True
+        index : bool, default False
             Write DataFrame index as a column.
             Uses *index_label* as the column name in the table.
         index_label : string or sequence, default None
             Column label for index column(s).
             If None is given (default) and index is True,
             then the index names are used.
         chunksize : int, optional
@@ -1666,86 +2076,391 @@
             The keys should be the column names and the values
             should be the SQLAlchemy types.
 
         Examples
         --------
 
         >>> from sqlalchemy import create_engine
-        >>> engine = create_engine("postgres://myusername:mypassword@myhost:5432\
+        >>> engine = create_engine("postgresql://myusername:mypassword@myhost:5432\
 /mydatabase")  # doctest: +SKIP
         >>> gdf.to_postgis("my_table", engine)  # doctest: +SKIP
 
         See also
         --------
         GeoDataFrame.to_file : write GeoDataFrame to file
         read_postgis : read PostGIS database to GeoDataFrame
 
         """
         geopandas.io.sql._write_postgis(
             self, name, con, schema, if_exists, index, index_label, chunksize, dtype
         )
 
-        #
-        # Implement standard operators for GeoSeries
-        #
-
-    def __xor__(self, other):
-        """Implement ^ operator as for builtin set type"""
-        warnings.warn(
-            "'^' operator will be deprecated. Use the 'symmetric_difference' "
-            "method instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.geometry.symmetric_difference(other)
+    plot = CachedAccessor("plot", geopandas.plotting.GeoplotAccessor)
 
-    def __or__(self, other):
-        """Implement | operator as for builtin set type"""
-        warnings.warn(
-            "'|' operator will be deprecated. Use the 'union' method instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.geometry.union(other)
+    @doc(_explore)
+    def explore(self, *args, **kwargs):
+        return _explore(self, *args, **kwargs)
 
-    def __and__(self, other):
-        """Implement & operator as for builtin set type"""
-        warnings.warn(
-            "'&' operator will be deprecated. Use the 'intersection' method instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.geometry.intersection(other)
+    def sjoin(self, df, *args, **kwargs):
+        """Spatial join of two GeoDataFrames.
 
-    def __sub__(self, other):
-        """Implement - operator as for builtin set type"""
-        warnings.warn(
-            "'-' operator will be deprecated. Use the 'difference' method instead.",
-            DeprecationWarning,
-            stacklevel=2,
+        See the User Guide page :doc:`../../user_guide/mergingdata` for details.
+
+        Parameters
+        ----------
+        df : GeoDataFrame
+        how : string, default 'inner'
+            The type of join:
+
+            * 'left': use keys from left_df; retain only left_df geometry column
+            * 'right': use keys from right_df; retain only right_df geometry column
+            * 'inner': use intersection of keys from both dfs; retain only
+              left_df geometry column
+
+        predicate : string, default 'intersects'
+            Binary predicate. Valid values are determined by the spatial index used.
+            You can check the valid values in left_df or right_df as
+            ``left_df.sindex.valid_query_predicates`` or
+            ``right_df.sindex.valid_query_predicates``
+        lsuffix : string, default 'left'
+            Suffix to apply to overlapping column names (left GeoDataFrame).
+        rsuffix : string, default 'right'
+            Suffix to apply to overlapping column names (right GeoDataFrame).
+
+        Examples
+        --------
+        >>> import geodatasets
+        >>> chicago = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.chicago_commpop")
+        ... )
+        >>> groceries = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.groceries")
+        ... ).to_crs(chicago.crs)
+
+        >>> chicago.head()  # doctest: +SKIP
+                 community  ...                                           geometry
+        0          DOUGLAS  ...  MULTIPOLYGON (((-87.60914 41.84469, -87.60915 ...
+        1          OAKLAND  ...  MULTIPOLYGON (((-87.59215 41.81693, -87.59231 ...
+        2      FULLER PARK  ...  MULTIPOLYGON (((-87.62880 41.80189, -87.62879 ...
+        3  GRAND BOULEVARD  ...  MULTIPOLYGON (((-87.60671 41.81681, -87.60670 ...
+        4          KENWOOD  ...  MULTIPOLYGON (((-87.59215 41.81693, -87.59215 ...
+
+        [5 rows x 9 columns]
+
+        >>> groceries.head()  # doctest: +SKIP
+           OBJECTID     Ycoord  ...  Category                           geometry
+        0        16  41.973266  ...       NaN  MULTIPOINT ((-87.65661 41.97321))
+        1        18  41.696367  ...       NaN  MULTIPOINT ((-87.68136 41.69713))
+        2        22  41.868634  ...       NaN  MULTIPOINT ((-87.63918 41.86847))
+        3        23  41.877590  ...       new  MULTIPOINT ((-87.65495 41.87783))
+        4        27  41.737696  ...       NaN  MULTIPOINT ((-87.62715 41.73623))
+        [5 rows x 8 columns]
+
+        >>> groceries_w_communities = groceries.sjoin(chicago)
+        >>> groceries_w_communities[["OBJECTID", "community", "geometry"]].head()
+           OBJECTID       community                           geometry
+        0        16          UPTOWN  MULTIPOINT ((-87.65661 41.97321))
+        1        18     MORGAN PARK  MULTIPOINT ((-87.68136 41.69713))
+        2        22  NEAR WEST SIDE  MULTIPOINT ((-87.63918 41.86847))
+        3        23  NEAR WEST SIDE  MULTIPOINT ((-87.65495 41.87783))
+        4        27         CHATHAM  MULTIPOINT ((-87.62715 41.73623))
+
+        Notes
+        -----
+        Every operation in GeoPandas is planar, i.e. the potential third
+        dimension is not taken into account.
+
+        See also
+        --------
+        GeoDataFrame.sjoin_nearest : nearest neighbor join
+        sjoin : equivalent top-level function
+        """
+        return geopandas.sjoin(left_df=self, right_df=df, *args, **kwargs)  # noqa: B026
+
+    def sjoin_nearest(
+        self,
+        right,
+        how="inner",
+        max_distance=None,
+        lsuffix="left",
+        rsuffix="right",
+        distance_col=None,
+        exclusive=False,
+    ):
+        """
+        Spatial join of two GeoDataFrames based on the distance between their
+        geometries.
+
+        Results will include multiple output records for a single input record
+        where there are multiple equidistant nearest or intersected neighbors.
+
+        See the User Guide page
+        https://geopandas.readthedocs.io/en/latest/docs/user_guide/mergingdata.html
+        for more details.
+
+
+        Parameters
+        ----------
+        right : GeoDataFrame
+        how : string, default 'inner'
+            The type of join:
+
+            * 'left': use keys from left_df; retain only left_df geometry column
+            * 'right': use keys from right_df; retain only right_df geometry column
+            * 'inner': use intersection of keys from both dfs; retain only
+              left_df geometry column
+
+        max_distance : float, default None
+            Maximum distance within which to query for nearest geometry.
+            Must be greater than 0.
+            The max_distance used to search for nearest items in the tree may have a
+            significant impact on performance by reducing the number of input
+            geometries that are evaluated for nearest items in the tree.
+        lsuffix : string, default 'left'
+            Suffix to apply to overlapping column names (left GeoDataFrame).
+        rsuffix : string, default 'right'
+            Suffix to apply to overlapping column names (right GeoDataFrame).
+        distance_col : string, default None
+            If set, save the distances computed between matching geometries under a
+            column of this name in the joined GeoDataFrame.
+        exclusive : bool, optional, default False
+            If True, the nearest geometries that are equal to the input geometry
+            will not be returned, default False.
+            Requires Shapely >= 2.0
+
+        Examples
+        --------
+        >>> import geodatasets
+        >>> groceries = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.groceries")
+        ... )
+        >>> chicago = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.chicago_health")
+        ... ).to_crs(groceries.crs)
+
+        >>> chicago.head()  # doctest: +SKIP
+           ComAreaID  ...                                           geometry
+        0         35  ...  POLYGON ((-87.60914 41.84469, -87.60915 41.844...
+        1         36  ...  POLYGON ((-87.59215 41.81693, -87.59231 41.816...
+        2         37  ...  POLYGON ((-87.62880 41.80189, -87.62879 41.801...
+        3         38  ...  POLYGON ((-87.60671 41.81681, -87.60670 41.816...
+        4         39  ...  POLYGON ((-87.59215 41.81693, -87.59215 41.816...
+        [5 rows x 87 columns]
+
+        >>> groceries.head()  # doctest: +SKIP
+           OBJECTID     Ycoord  ...  Category                           geometry
+        0        16  41.973266  ...       NaN  MULTIPOINT ((-87.65661 41.97321))
+        1        18  41.696367  ...       NaN  MULTIPOINT ((-87.68136 41.69713))
+        2        22  41.868634  ...       NaN  MULTIPOINT ((-87.63918 41.86847))
+        3        23  41.877590  ...       new  MULTIPOINT ((-87.65495 41.87783))
+        4        27  41.737696  ...       NaN  MULTIPOINT ((-87.62715 41.73623))
+        [5 rows x 8 columns]
+
+        >>> groceries_w_communities = groceries.sjoin_nearest(chicago)
+        >>> groceries_w_communities[["Chain", "community", "geometry"]].head(2)
+                       Chain    community                                geometry
+        0     VIET HOA PLAZA       UPTOWN   MULTIPOINT ((1168268.672 1933554.35))
+        1  COUNTY FAIR FOODS  MORGAN PARK  MULTIPOINT ((1162302.618 1832900.224))
+
+
+        To include the distances:
+
+        >>> groceries_w_communities = groceries.sjoin_nearest(chicago, \
+distance_col="distances")
+        >>> groceries_w_communities[["Chain", "community", \
+"distances"]].head(2)
+                       Chain    community  distances
+        0     VIET HOA PLAZA       UPTOWN        0.0
+        1  COUNTY FAIR FOODS  MORGAN PARK        0.0
+
+        In the following example, we get multiple groceries for Uptown because all
+        results are equidistant (in this case zero because they intersect).
+        In fact, we get 4 results in total:
+
+        >>> chicago_w_groceries = groceries.sjoin_nearest(chicago, \
+distance_col="distances", how="right")
+        >>> uptown_results = \
+chicago_w_groceries[chicago_w_groceries["community"] == "UPTOWN"]
+        >>> uptown_results[["Chain", "community"]]
+                    Chain community
+        30  VIET HOA PLAZA    UPTOWN
+        30      JEWEL OSCO    UPTOWN
+        30          TARGET    UPTOWN
+        30       Mariano's    UPTOWN
+
+        See also
+        --------
+        GeoDataFrame.sjoin : binary predicate joins
+        sjoin_nearest : equivalent top-level function
+
+        Notes
+        -----
+        Since this join relies on distances, results will be inaccurate
+        if your geometries are in a geographic CRS.
+
+        Every operation in GeoPandas is planar, i.e. the potential third
+        dimension is not taken into account.
+        """
+        return geopandas.sjoin_nearest(
+            self,
+            right,
+            how=how,
+            max_distance=max_distance,
+            lsuffix=lsuffix,
+            rsuffix=rsuffix,
+            distance_col=distance_col,
+            exclusive=exclusive,
         )
-        return self.geometry.difference(other)
 
-    if compat.PANDAS_GE_025:
-        from pandas.core.accessor import CachedAccessor
+    def clip(self, mask, keep_geom_type=False):
+        """Clip points, lines, or polygon geometries to the mask extent.
 
-        plot = CachedAccessor("plot", geopandas.plotting.GeoplotAccessor)
-    else:
+        Both layers must be in the same Coordinate Reference System (CRS).
+        The GeoDataFrame will be clipped to the full extent of the ``mask`` object.
 
-        def plot(self, *args, **kwargs):
-            """Generate a plot of the geometries in the ``GeoDataFrame``.
-            If the ``column`` parameter is given, colors plot according to values
-            in that column, otherwise calls ``GeoSeries.plot()`` on the
-            ``geometry`` column.
-            Wraps the ``plot_dataframe()`` function, and documentation is copied
-            from there.
-            """
-            return plot_dataframe(self, *args, **kwargs)
+        If there are multiple polygons in mask, data from the GeoDataFrame will be
+        clipped to the total boundary of all polygons in mask.
+
+        Parameters
+        ----------
+        mask : GeoDataFrame, GeoSeries, (Multi)Polygon, list-like
+            Polygon vector layer used to clip the GeoDataFrame.
+            The mask's geometry is dissolved into one geometric feature
+            and intersected with GeoDataFrame.
+            If the mask is list-like with four elements ``(minx, miny, maxx, maxy)``,
+            ``clip`` will use a faster rectangle clipping
+            (:meth:`~GeoSeries.clip_by_rect`), possibly leading to slightly different
+            results.
+        keep_geom_type : boolean, default False
+            If True, return only geometries of original type in case of intersection
+            resulting in multiple geometry types or GeometryCollections.
+            If False, return all resulting geometries (potentially mixed types).
+
+        Returns
+        -------
+        GeoDataFrame
+            Vector data (points, lines, polygons) from the GeoDataFrame clipped to
+            polygon boundary from mask.
+
+        See also
+        --------
+        clip : equivalent top-level function
+
+        Examples
+        --------
+        Clip points (grocery stores) with polygons (the Near West Side community):
+
+        >>> import geodatasets
+        >>> chicago = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.chicago_health")
+        ... )
+        >>> near_west_side = chicago[chicago["community"] == "NEAR WEST SIDE"]
+        >>> groceries = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.groceries")
+        ... ).to_crs(chicago.crs)
+        >>> groceries.shape
+        (148, 8)
+
+        >>> nws_groceries = groceries.clip(near_west_side)
+        >>> nws_groceries.shape
+        (7, 8)
+        """
+        return geopandas.clip(self, mask=mask, keep_geom_type=keep_geom_type)
+
+    def overlay(self, right, how="intersection", keep_geom_type=None, make_valid=True):
+        """Perform spatial overlay between GeoDataFrames.
+
+        Currently only supports data GeoDataFrames with uniform geometry types,
+        i.e. containing only (Multi)Polygons, or only (Multi)Points, or a
+        combination of (Multi)LineString and LinearRing shapes.
+        Implements several methods that are all effectively subsets of the union.
 
-    plot.__doc__ = plot_dataframe.__doc__
+        See the User Guide page :doc:`../../user_guide/set_operations` for details.
+
+        Parameters
+        ----------
+        right : GeoDataFrame
+        how : string
+            Method of spatial overlay: 'intersection', 'union',
+            'identity', 'symmetric_difference' or 'difference'.
+        keep_geom_type : bool
+            If True, return only geometries of the same geometry type the GeoDataFrame
+            has, if False, return all resulting geometries. Default is None,
+            which will set keep_geom_type to True but warn upon dropping
+            geometries.
+        make_valid : bool, default True
+            If True, any invalid input geometries are corrected with a call to
+            make_valid(), if False, a `ValueError` is raised if any input geometries
+            are invalid.
+
+        Returns
+        -------
+        df : GeoDataFrame
+            GeoDataFrame with new set of polygons and attributes
+            resulting from the overlay
+
+        Examples
+        --------
+        >>> from shapely.geometry import Polygon
+        >>> polys1 = geopandas.GeoSeries([Polygon([(0,0), (2,0), (2,2), (0,2)]),
+        ...                               Polygon([(2,2), (4,2), (4,4), (2,4)])])
+        >>> polys2 = geopandas.GeoSeries([Polygon([(1,1), (3,1), (3,3), (1,3)]),
+        ...                               Polygon([(3,3), (5,3), (5,5), (3,5)])])
+        >>> df1 = geopandas.GeoDataFrame({'geometry': polys1, 'df1_data':[1,2]})
+        >>> df2 = geopandas.GeoDataFrame({'geometry': polys2, 'df2_data':[1,2]})
+
+        >>> df1.overlay(df2, how='union')
+           df1_data  df2_data                                           geometry
+        0       1.0       1.0                POLYGON ((2 2, 2 1, 1 1, 1 2, 2 2))
+        1       2.0       1.0                POLYGON ((2 2, 2 3, 3 3, 3 2, 2 2))
+        2       2.0       2.0                POLYGON ((4 4, 4 3, 3 3, 3 4, 4 4))
+        3       1.0       NaN      POLYGON ((2 0, 0 0, 0 2, 1 2, 1 1, 2 1, 2 0))
+        4       2.0       NaN  MULTIPOLYGON (((3 4, 3 3, 2 3, 2 4, 3 4)), ((4...
+        5       NaN       1.0  MULTIPOLYGON (((2 3, 2 2, 1 2, 1 3, 2 3)), ((3...
+        6       NaN       2.0      POLYGON ((3 5, 5 5, 5 3, 4 3, 4 4, 3 4, 3 5))
+
+        >>> df1.overlay(df2, how='intersection')
+           df1_data  df2_data                             geometry
+        0         1         1  POLYGON ((2 2, 2 1, 1 1, 1 2, 2 2))
+        1         2         1  POLYGON ((2 2, 2 3, 3 3, 3 2, 2 2))
+        2         2         2  POLYGON ((4 4, 4 3, 3 3, 3 4, 4 4))
+
+        >>> df1.overlay(df2, how='symmetric_difference')
+           df1_data  df2_data                                           geometry
+        0       1.0       NaN      POLYGON ((2 0, 0 0, 0 2, 1 2, 1 1, 2 1, 2 0))
+        1       2.0       NaN  MULTIPOLYGON (((3 4, 3 3, 2 3, 2 4, 3 4)), ((4...
+        2       NaN       1.0  MULTIPOLYGON (((2 3, 2 2, 1 2, 1 3, 2 3)), ((3...
+        3       NaN       2.0      POLYGON ((3 5, 5 5, 5 3, 4 3, 4 4, 3 4, 3 5))
+
+        >>> df1.overlay(df2, how='difference')
+                                                    geometry  df1_data
+        0      POLYGON ((2 0, 0 0, 0 2, 1 2, 1 1, 2 1, 2 0))         1
+        1  MULTIPOLYGON (((3 4, 3 3, 2 3, 2 4, 3 4)), ((4...         2
+
+        >>> df1.overlay(df2, how='identity')
+           df1_data  df2_data                                           geometry
+        0       1.0       1.0                POLYGON ((2 2, 2 1, 1 1, 1 2, 2 2))
+        1       2.0       1.0                POLYGON ((2 2, 2 3, 3 3, 3 2, 2 2))
+        2       2.0       2.0                POLYGON ((4 4, 4 3, 3 3, 3 4, 4 4))
+        3       1.0       NaN      POLYGON ((2 0, 0 0, 0 2, 1 2, 1 1, 2 1, 2 0))
+        4       2.0       NaN  MULTIPOLYGON (((3 4, 3 3, 2 3, 2 4, 3 4)), ((4...
+
+        See also
+        --------
+        GeoDataFrame.sjoin : spatial join
+        overlay : equivalent top-level function
+
+        Notes
+        -----
+        Every operation in GeoPandas is planar, i.e. the potential third
+        dimension is not taken into account.
+        """
+        return geopandas.overlay(
+            self, right, how=how, keep_geom_type=keep_geom_type, make_valid=make_valid
+        )
 
 
 def _dataframe_set_geometry(self, col, drop=False, inplace=False, crs=None):
     if inplace:
         raise ValueError(
             "Can't do inplace setting when converting from DataFrame to GeoDataFrame"
         )
```

### Comparing `geopandas-0.9.0/geopandas/geoseries.py` & `geopandas-1.0.0a1/geopandas/geoseries.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,82 @@
-import json
+from __future__ import annotations
+
+import typing
+from typing import Optional, Any, Callable, Dict
 import warnings
 
 import numpy as np
 import pandas as pd
-from pandas import Series, MultiIndex
+from pandas import Series
 from pandas.core.internals import SingleBlockManager
 
-from pyproj import CRS
+import shapely
 from shapely.geometry.base import BaseGeometry
+from shapely.geometry import GeometryCollection
 
 from geopandas.base import GeoPandasBase, _delegate_property
 from geopandas.plotting import plot_series
+from geopandas.explore import _explore_geoseries
+import geopandas
 
+from . import _compat as compat
+from ._decorator import doc
 from .array import (
     GeometryDtype,
     from_shapely,
     from_wkb,
     from_wkt,
+    points_from_xy,
     to_wkb,
     to_wkt,
 )
 from .base import is_geometry_type
-from . import _compat as compat
 
+if typing.TYPE_CHECKING:
+    import os
 
-_SERIES_WARNING_MSG = """\
-    You are passing non-geometry data to the GeoSeries constructor. Currently,
-    it falls back to returning a pandas Series. But in the future, we will start
-    to raise a TypeError instead."""
 
-
-def _geoseries_constructor_with_fallback(data=None, index=None, crs=None, **kwargs):
+def _geoseries_constructor_with_fallback(
+    data=None, index=None, crs: Optional[Any] = None, **kwargs
+):
     """
     A flexible constructor for GeoSeries._constructor, which needs to be able
     to fall back to a Series (if a certain operation does not produce
     geometries)
     """
     try:
-        with warnings.catch_warnings():
-            warnings.filterwarnings(
-                "ignore",
-                message=_SERIES_WARNING_MSG,
-                category=FutureWarning,
-                module="geopandas[.*]",
-            )
-            return GeoSeries(data=data, index=index, crs=crs, **kwargs)
+        return GeoSeries(data=data, index=index, crs=crs, **kwargs)
     except TypeError:
         return Series(data=data, index=index, **kwargs)
 
 
-def inherit_doc(cls):
-    """
-    A decorator adding a docstring from an existing method.
-    """
+def _expanddim_logic(df):
+    """Shared logic for _constructor_expanddim and _constructor_from_mgr_expanddim."""
+    from geopandas import GeoDataFrame
+
+    if (df.dtypes == "geometry").sum() > 0:
+        if df.shape[1] == 1:
+            geo_col_name = df.columns[0]
+        else:
+            geo_col_name = None
 
-    def decorator(decorated):
-        original_method = getattr(cls, decorated.__name__, None)
-        if original_method:
-            doc = original_method.__doc__ or ""
+        if geo_col_name is None or not is_geometry_type(df[geo_col_name]):
+            df = GeoDataFrame(df)
+            df._geometry_column_name = None
         else:
-            doc = ""
+            df = df.set_geometry(geo_col_name)
 
-        decorated.__doc__ = doc
-        return decorated
+    return df
 
-    return decorator
+
+def _geoseries_expanddim(data=None, *args, **kwargs):
+    # pd.Series._constructor_expanddim == pd.DataFrame, we start
+    # with that then specialize.
+    df = pd.DataFrame(data, *args, **kwargs)
+    return _expanddim_logic(df)
 
 
 class GeoSeries(GeoPandasBase, Series):
     """
     A Series object designed to store shapely geometry objects.
 
     Parameters
@@ -88,17 +96,17 @@
 
     Examples
     --------
 
     >>> from shapely.geometry import Point
     >>> s = geopandas.GeoSeries([Point(1, 1), Point(2, 2), Point(3, 3)])
     >>> s
-    0    POINT (1.00000 1.00000)
-    1    POINT (2.00000 2.00000)
-    2    POINT (3.00000 3.00000)
+    0    POINT (1 1)
+    1    POINT (2 2)
+    2    POINT (3 3)
     dtype: geometry
 
     >>> s = geopandas.GeoSeries(
     ...     [Point(1, 1), Point(2, 2), Point(3, 3)], crs="EPSG:3857"
     ... )
     >>> s.crs  # doctest: +SKIP
     <Projected CRS: EPSG:3857>
@@ -116,82 +124,59 @@
     - Ellipsoid: WGS 84
     - Prime Meridian: Greenwich
 
     >>> s = geopandas.GeoSeries(
     ...    [Point(1, 1), Point(2, 2), Point(3, 3)], index=["a", "b", "c"], crs=4326
     ... )
     >>> s
-    a    POINT (1.00000 1.00000)
-    b    POINT (2.00000 2.00000)
-    c    POINT (3.00000 3.00000)
+    a    POINT (1 1)
+    b    POINT (2 2)
+    c    POINT (3 3)
     dtype: geometry
 
     >>> s.crs
     <Geographic 2D CRS: EPSG:4326>
     Name: WGS 84
     Axis Info [ellipsoidal]:
     - Lat[north]: Geodetic latitude (degree)
     - Lon[east]: Geodetic longitude (degree)
     Area of Use:
-    - name: World
+    - name: World.
     - bounds: (-180.0, -90.0, 180.0, 90.0)
-    Datum: World Geodetic System 1984
+    Datum: World Geodetic System 1984 ensemble
     - Ellipsoid: WGS 84
     - Prime Meridian: Greenwich
 
     See Also
     --------
     GeoDataFrame
     pandas.Series
 
     """
 
-    _metadata = ["name"]
-
-    def __new__(cls, data=None, index=None, crs=None, **kwargs):
-        # we need to use __new__ because we want to return Series instance
-        # instead of GeoSeries instance in case of non-geometry data
-
+    def __init__(self, data=None, index=None, crs: Optional[Any] = None, **kwargs):
         if hasattr(data, "crs") and crs:
             if not data.crs:
                 # make a copy to avoid setting CRS to passed GeometryArray
                 data = data.copy()
             else:
                 if not data.crs == crs:
-                    warnings.warn(
+                    raise ValueError(
                         "CRS mismatch between CRS of the passed geometries "
-                        "and 'crs'. Use 'GeoDataFrame.set_crs(crs, "
+                        "and 'crs'. Use 'GeoSeries.set_crs(crs, "
                         "allow_override=True)' to overwrite CRS or "
                         "'GeoSeries.to_crs(crs)' to reproject geometries. "
-                        "CRS mismatch will raise an error in the future versions "
-                        "of GeoPandas.",
-                        FutureWarning,
-                        stacklevel=2,
                     )
-                    # TODO: raise error in 0.9 or 0.10.
 
         if isinstance(data, SingleBlockManager):
-            if isinstance(data.blocks[0].dtype, GeometryDtype):
-                if data.blocks[0].ndim == 2:
-                    # bug in pandas 0.23 where in certain indexing operations
-                    # (such as .loc) a 2D ExtensionBlock (still with 1D values
-                    # is created) which results in other failures
-                    # bug in pandas <= 0.25.0 when len(values) == 1
-                    #   (https://github.com/pandas-dev/pandas/issues/27785)
-                    from pandas.core.internals import ExtensionBlock
-
-                    values = data.blocks[0].values
-                    block = ExtensionBlock(values, slice(0, len(values), 1), ndim=1)
-                    data = SingleBlockManager([block], data.axes[0], fastpath=True)
-                self = super(GeoSeries, cls).__new__(cls)
-                super(GeoSeries, self).__init__(data, index=index, **kwargs)
-                self.crs = getattr(self.values, "crs", crs)
-                return self
-            warnings.warn(_SERIES_WARNING_MSG, FutureWarning, stacklevel=2)
-            return Series(data, index=index, **kwargs)
+            if not isinstance(data.blocks[0].dtype, GeometryDtype):
+                raise TypeError(
+                    "Non geometry data passed to GeoSeries constructor, "
+                    f"received data of dtype '{data.blocks[0].dtype}'"
+                )
 
         if isinstance(data, BaseGeometry):
             # fix problem for scalar geometries passed, ensure the list of
             # scalars is of correct length if index is specified
             n = len(index) if index is not None else 1
             data = [data] * n
 
@@ -199,53 +184,63 @@
 
         if not is_geometry_type(data):
             # if data is None and dtype is specified (eg from empty overlay
             # test), specifying dtype raises an error:
             # https://github.com/pandas-dev/pandas/issues/26469
             kwargs.pop("dtype", None)
             # Use Series constructor to handle input data
-            with compat.ignore_shapely2_warnings():
+            with warnings.catch_warnings():
+                # suppress additional warning from pandas for empty data
+                # (will always give object dtype instead of float dtype in the future,
+                # making the `if s.empty: s = s.astype(object)` below unnecessary)
+                empty_msg = "The default dtype for empty Series"
+                warnings.filterwarnings("ignore", empty_msg, DeprecationWarning)
+                warnings.filterwarnings("ignore", empty_msg, FutureWarning)
                 s = pd.Series(data, index=index, name=name, **kwargs)
             # prevent trying to convert non-geometry objects
             if s.dtype != object:
-                if s.empty or data is None:
+                if (s.empty and s.dtype == "float64") or data is None:
+                    # pd.Series with empty data gives float64 for older pandas versions
                     s = s.astype(object)
                 else:
-                    warnings.warn(_SERIES_WARNING_MSG, FutureWarning, stacklevel=2)
-                    return s
-            # try to convert to GeometryArray, if fails return plain Series
+                    raise TypeError(
+                        "Non geometry data passed to GeoSeries constructor, "
+                        f"received data of dtype '{s.dtype}'"
+                    )
+            # extract object-dtype numpy array from pandas Series; with CoW this
+            # gives a read-only array, so we try to set the flag back to writeable
+            data = s.to_numpy()
             try:
-                data = from_shapely(s.values, crs)
+                data.flags.writeable = True
+            except ValueError:
+                pass
+            # try to convert to GeometryArray
+            try:
+                data = from_shapely(data, crs)
             except TypeError:
-                warnings.warn(_SERIES_WARNING_MSG, FutureWarning, stacklevel=2)
-                return s
+                raise TypeError(
+                    "Non geometry data passed to GeoSeries constructor, "
+                    f"received data of dtype '{s.dtype}'"
+                )
             index = s.index
             name = s.name
 
-        self = super(GeoSeries, cls).__new__(cls)
-        super(GeoSeries, self).__init__(data, index=index, name=name, **kwargs)
-
+        super().__init__(data, index=index, name=name, **kwargs)
         if not self.crs:
             self.crs = crs
-        return self
-
-    def __init__(self, *args, **kwargs):
-        # need to overwrite Series init to prevent calling it for GeoSeries
-        # (doesn't know crs, all work is already done above)
-        pass
 
-    def append(self, *args, **kwargs):
+    def append(self, *args, **kwargs) -> GeoSeries:
         return self._wrapped_pandas_method("append", *args, **kwargs)
 
     @property
-    def geometry(self):
+    def geometry(self) -> GeoSeries:
         return self
 
     @property
-    def x(self):
+    def x(self) -> Series:
         """Return the x location of point geometries in a GeoSeries
 
         Returns
         -------
         pandas.Series
 
         Examples
@@ -265,15 +260,15 @@
         GeoSeries.y
         GeoSeries.z
 
         """
         return _delegate_property("x", self)
 
     @property
-    def y(self):
+    def y(self) -> Series:
         """Return the y location of point geometries in a GeoSeries
 
         Returns
         -------
         pandas.Series
 
         Examples
@@ -293,15 +288,15 @@
         GeoSeries.x
         GeoSeries.z
 
         """
         return _delegate_property("y", self)
 
     @property
-    def z(self):
+    def z(self) -> Series:
         """Return the z location of point geometries in a GeoSeries
 
         Returns
         -------
         pandas.Series
 
         Examples
@@ -321,58 +316,60 @@
         GeoSeries.x
         GeoSeries.y
 
         """
         return _delegate_property("z", self)
 
     @classmethod
-    def from_file(cls, filename, **kwargs):
+    def from_file(cls, filename: os.PathLike | typing.IO, **kwargs) -> GeoSeries:
         """Alternate constructor to create a ``GeoSeries`` from a file.
 
         Can load a ``GeoSeries`` from a file from any format recognized by
-        `fiona`. See http://fiona.readthedocs.io/en/latest/manual.html for details.
+        `pyogrio`. See http://pyogrio.readthedocs.io/ for details.
         From a file with attributes loads only geometry column. Note that to do
         that, GeoPandas first loads the whole GeoDataFrame.
 
         Parameters
         ----------
         filename : str
             File path or file handle to read from. Depending on which kwargs
             are included, the content of filename may vary. See
-            http://fiona.readthedocs.io/en/latest/README.html#usage for usage details.
+            :func:`pyogrio.read_dataframe` for usage details.
         kwargs : key-word arguments
-            These arguments are passed to fiona.open, and can be used to
-            access multi-layer data, data stored within archives (zip files),
+            These arguments are passed to :func:`pyogrio.read_dataframe`, and can be
+            used to access multi-layer data, data stored within archives (zip files),
             etc.
 
         Examples
         --------
-
-        >>> path = geopandas.datasets.get_path('nybb')
+        >>> import geodatasets
+        >>> path = geodatasets.get_path('nybb')
         >>> s = geopandas.GeoSeries.from_file(path)
         >>> s
         0    MULTIPOLYGON (((970217.022 145643.332, 970227....
         1    MULTIPOLYGON (((1029606.077 156073.814, 102957...
         2    MULTIPOLYGON (((1021176.479 151374.797, 102100...
         3    MULTIPOLYGON (((981219.056 188655.316, 980940....
         4    MULTIPOLYGON (((1012821.806 229228.265, 101278...
         Name: geometry, dtype: geometry
 
         See Also
         --------
-        read_file : read file to GeoDataFame
+        read_file : read file to GeoDataFrame
         """
         from geopandas import GeoDataFrame
 
         df = GeoDataFrame.from_file(filename, **kwargs)
 
         return GeoSeries(df.geometry, crs=df.crs)
 
     @classmethod
-    def from_wkb(cls, data, index=None, crs=None, **kwargs):
+    def from_wkb(
+        cls, data, index=None, crs: Optional[Any] = None, on_invalid="raise", **kwargs
+    ) -> GeoSeries:
         """
         Alternate constructor to create a ``GeoSeries``
         from a list or array of WKB objects
 
         Parameters
         ----------
         data : array-like or Series
@@ -380,31 +377,41 @@
         index : array-like or Index
             The index for the GeoSeries.
         crs : value, optional
             Coordinate Reference System of the geometry objects. Can be anything
             accepted by
             :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
             such as an authority string (eg "EPSG:4326") or a WKT string.
+        on_invalid: {"raise", "warn", "ignore"}, default "raise"
+            - raise: an exception will be raised if a WKB input geometry is invalid.
+            - warn: a warning will be raised and invalid WKB geometries will be returned
+              as None.
+            - ignore: invalid WKB geometries will be returned as None without a warning.
+
         kwargs
             Additional arguments passed to the Series constructor,
             e.g. ``name``.
 
         Returns
         -------
         GeoSeries
 
         See Also
         --------
         GeoSeries.from_wkt
 
         """
-        return cls._from_wkb_or_wkb(from_wkb, data, index=index, crs=crs, **kwargs)
+        return cls._from_wkb_or_wkt(
+            from_wkb, data, index=index, crs=crs, on_invalid=on_invalid, **kwargs
+        )
 
     @classmethod
-    def from_wkt(cls, data, index=None, crs=None, **kwargs):
+    def from_wkt(
+        cls, data, index=None, crs: Optional[Any] = None, on_invalid="raise", **kwargs
+    ) -> GeoSeries:
         """
         Alternate constructor to create a ``GeoSeries``
         from a list or array of WKT objects
 
         Parameters
         ----------
         data : array-like, Series
@@ -412,14 +419,21 @@
         index : array-like or Index
             The index for the GeoSeries.
         crs : value, optional
             Coordinate Reference System of the geometry objects. Can be anything
             accepted by
             :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
             such as an authority string (eg "EPSG:4326") or a WKT string.
+        on_invalid : {"raise", "warn", "ignore"}, default "raise"
+            - raise: an exception will be raised if a WKT input geometry is invalid.
+            - warn: a warning will be raised and invalid WKT geometries will be
+              returned as ``None``.
+            - ignore: invalid WKT geometries will be returned as ``None`` without a
+              warning.
+
         kwargs
             Additional arguments passed to the Series constructor,
             e.g. ``name``.
 
         Returns
         -------
         GeoSeries
@@ -434,36 +448,103 @@
         >>> wkts = [
         ... 'POINT (1 1)',
         ... 'POINT (2 2)',
         ... 'POINT (3 3)',
         ... ]
         >>> s = geopandas.GeoSeries.from_wkt(wkts)
         >>> s
-        0    POINT (1.00000 1.00000)
-        1    POINT (2.00000 2.00000)
-        2    POINT (3.00000 3.00000)
+        0    POINT (1 1)
+        1    POINT (2 2)
+        2    POINT (3 3)
         dtype: geometry
         """
-        return cls._from_wkb_or_wkb(from_wkt, data, index=index, crs=crs, **kwargs)
+        return cls._from_wkb_or_wkt(
+            from_wkt, data, index=index, crs=crs, on_invalid=on_invalid, **kwargs
+        )
 
     @classmethod
-    def _from_wkb_or_wkb(
-        cls, from_wkb_or_wkt_function, data, index=None, crs=None, **kwargs
-    ):
+    def from_xy(cls, x, y, z=None, index=None, crs=None, **kwargs) -> GeoSeries:
+        """
+        Alternate constructor to create a :class:`~geopandas.GeoSeries` of Point
+        geometries from lists or arrays of x, y(, z) coordinates
+
+        In case of geographic coordinates, it is assumed that longitude is captured
+        by ``x`` coordinates and latitude by ``y``.
+
+        Parameters
+        ----------
+        x, y, z : iterable
+        index : array-like or Index, optional
+            The index for the GeoSeries. If not given and all coordinate inputs
+            are Series with an equal index, that index is used.
+        crs : value, optional
+            Coordinate Reference System of the geometry objects. Can be anything
+            accepted by
+            :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
+            such as an authority string (eg "EPSG:4326") or a WKT string.
+        **kwargs
+            Additional arguments passed to the Series constructor,
+            e.g. ``name``.
+
+        Returns
+        -------
+        GeoSeries
+
+        See Also
+        --------
+        GeoSeries.from_wkt
+        points_from_xy
+
+        Examples
+        --------
+
+        >>> x = [2.5, 5, -3.0]
+        >>> y = [0.5, 1, 1.5]
+        >>> s = geopandas.GeoSeries.from_xy(x, y, crs="EPSG:4326")
+        >>> s
+        0    POINT (2.5 0.5)
+        1    POINT (5 1)
+        2    POINT (-3 1.5)
+        dtype: geometry
+        """
+        if index is None:
+            if (
+                isinstance(x, Series)
+                and isinstance(y, Series)
+                and x.index.equals(y.index)
+                and (z is None or (isinstance(z, Series) and x.index.equals(z.index)))
+            ):  # check if we can reuse index
+                index = x.index
+        return cls(points_from_xy(x, y, z, crs=crs), index=index, crs=crs, **kwargs)
+
+    @classmethod
+    def _from_wkb_or_wkt(
+        cls,
+        from_wkb_or_wkt_function: Callable,
+        data,
+        index=None,
+        crs: Optional[Any] = None,
+        on_invalid: str = "raise",
+        **kwargs,
+    ) -> GeoSeries:
         """Create a GeoSeries from either WKT or WKB values"""
         if isinstance(data, Series):
             if index is not None:
                 data = data.reindex(index)
             else:
                 index = data.index
             data = data.values
-        return cls(from_wkb_or_wkt_function(data, crs=crs), index=index, **kwargs)
+        return cls(
+            from_wkb_or_wkt_function(data, crs=crs, on_invalid=on_invalid),
+            index=index,
+            **kwargs,
+        )
 
     @property
-    def __geo_interface__(self):
+    def __geo_interface__(self) -> Dict:
         """Returns a ``GeoSeries`` as a python feature collection.
 
         Implements the `geo_interface`. The returned python data structure
         represents the ``GeoSeries`` as a GeoJSON-like ``FeatureCollection``.
         Note that the features will have an empty ``properties`` dict as they
         don't have associated attributes (geometry only).
 
@@ -481,45 +562,72 @@
 {}, 'geometry': {'type': 'Point', 'coordinates': (3.0, 3.0)}, 'bbox': (3.0, \
 3.0, 3.0, 3.0)}], 'bbox': (1.0, 1.0, 3.0, 3.0)}
         """
         from geopandas import GeoDataFrame
 
         return GeoDataFrame({"geometry": self}).__geo_interface__
 
-    def to_file(self, filename, driver="ESRI Shapefile", index=None, **kwargs):
+    def to_file(
+        self,
+        filename: os.PathLike | typing.IO,
+        driver: Optional[str] = None,
+        index: Optional[bool] = None,
+        **kwargs,
+    ):
         """Write the ``GeoSeries`` to a file.
 
         By default, an ESRI shapefile is written, but any OGR data source
-        supported by Fiona can be written.
+        supported by Pyogrio or Fiona can be written.
 
         Parameters
         ----------
         filename : string
-            File path or file handle to write to.
-        driver : string, default: 'ESRI Shapefile'
+            File path or file handle to write to. The path may specify a
+            GDAL VSI scheme.
+        driver : string, default None
             The OGR format driver used to write the vector file.
+            If not specified, it attempts to infer it from the file extension.
+            If no extension is specified, it saves ESRI Shapefile to a folder.
         index : bool, default None
             If True, write index into one or more columns (for MultiIndex).
             Default None writes the index into one or more columns only if
             the index is named, is a MultiIndex, or has a non-integer data
             type. If False, no index is written.
 
             .. versionadded:: 0.7
                 Previously the index was not written.
-
-        Notes
-        -----
-        The extra keyword arguments ``**kwargs`` are passed to fiona.open and
-        can be used to write to multi-layer data, store data within archives
-        (zip files), etc.
+        mode : string, default 'w'
+            The write mode, 'w' to overwrite the existing file and 'a' to append.
+            Not all drivers support appending. The drivers that support appending
+            are listed in fiona.supported_drivers or
+            https://github.com/Toblerity/Fiona/blob/master/fiona/drvsupport.py
+        crs : pyproj.CRS, default None
+            If specified, the CRS is passed to Fiona to
+            better control how the file is written. If None, GeoPandas
+            will determine the crs based on crs df attribute.
+            The value can be anything accepted
+            by :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
+            such as an authority string (eg "EPSG:4326") or a WKT string. The keyword
+            is not supported for the "pyogrio" engine.
+        engine : str, "pyogrio" or "fiona"
+            The underlying library that is used to write the file. Currently, the
+            supported options are "pyogrio" and "fiona". Defaults to "pyogrio" if
+            installed, otherwise tries "fiona".
+        **kwargs :
+            Keyword args to be passed to the engine, and can be used to write
+            to multi-layer data, store data within archives (zip files), etc.
+            In case of the "pyogrio" engine, the keyword arguments are passed to
+            `pyogrio.write_dataframe`. In case of the "fiona" engine, the keyword
+            arguments are passed to fiona.open`. For more information on possible
+            keywords, type: ``import pyogrio; help(pyogrio.write_dataframe)``.
 
         See Also
         --------
         GeoDataFrame.to_file : write GeoDataFrame to file
-        read_file : read file to GeoDataFame
+        read_file : read file to GeoDataFrame
 
         Examples
         --------
 
         >>> s.to_file('series.shp')  # doctest: +SKIP
 
         >>> s.to_file('series.gpkg', driver='GPKG', layer='name1')  # doctest: +SKIP
@@ -536,59 +644,71 @@
     # Implement pandas methods
     #
 
     @property
     def _constructor(self):
         return _geoseries_constructor_with_fallback
 
+    def _constructor_from_mgr(self, mgr, axes):
+        assert isinstance(mgr, SingleBlockManager)
+
+        if not isinstance(mgr.blocks[0].dtype, GeometryDtype):
+            return Series._from_mgr(mgr, axes)
+
+        return GeoSeries._from_mgr(mgr, axes)
+
     @property
     def _constructor_expanddim(self):
-        from geopandas import GeoDataFrame
+        return _geoseries_expanddim
 
-        return GeoDataFrame
+    def _constructor_expanddim_from_mgr(self, mgr, axes):
+        df = pd.DataFrame._from_mgr(mgr, axes)
+        return _expanddim_logic(df)
 
     def _wrapped_pandas_method(self, mtd, *args, **kwargs):
         """Wrap a generic pandas method to ensure it returns a GeoSeries"""
-        val = getattr(super(GeoSeries, self), mtd)(*args, **kwargs)
+        val = getattr(super(), mtd)(*args, **kwargs)
         if type(val) == Series:
             val.__class__ = GeoSeries
             val.crs = self.crs
         return val
 
     def __getitem__(self, key):
         return self._wrapped_pandas_method("__getitem__", key)
 
-    @inherit_doc(pd.Series)
+    @doc(pd.Series)
     def sort_index(self, *args, **kwargs):
         return self._wrapped_pandas_method("sort_index", *args, **kwargs)
 
-    @inherit_doc(pd.Series)
+    @doc(pd.Series)
     def take(self, *args, **kwargs):
         return self._wrapped_pandas_method("take", *args, **kwargs)
 
-    @inherit_doc(pd.Series)
+    @doc(pd.Series)
     def select(self, *args, **kwargs):
         return self._wrapped_pandas_method("select", *args, **kwargs)
 
-    @inherit_doc(pd.Series)
-    def apply(self, func, convert_dtype=True, args=(), **kwargs):
-        result = super().apply(func, convert_dtype=convert_dtype, args=args, **kwargs)
+    @doc(pd.Series)
+    def apply(self, func, convert_dtype: Optional[bool] = None, args=(), **kwargs):
+        if convert_dtype is not None:
+            kwargs["convert_dtype"] = convert_dtype
+        else:
+            # if compat.PANDAS_GE_21 don't pass through, use pandas default
+            # of true to avoid internally triggering the pandas warning
+            if not compat.PANDAS_GE_21:
+                kwargs["convert_dtype"] = True
+
+        # to avoid warning
+        result = super().apply(func, args=args, **kwargs)
         if isinstance(result, GeoSeries):
             if self.crs is not None:
                 result.set_crs(self.crs, inplace=True)
         return result
 
-    def __finalize__(self, other, method=None, **kwargs):
-        """ propagate metadata from other to self """
-        # NOTE: backported from pandas master (upcoming v0.13)
-        for name in self._metadata:
-            object.__setattr__(self, name, getattr(other, name, None))
-        return self
-
-    def isna(self):
+    def isna(self) -> Series:
         """
         Detect missing values.
 
         Historically, NA values in a GeoSeries could be represented by
         empty geometric objects, in addition to standard representations
         such as None and np.nan. This behaviour is changed in version 0.6.0,
         and now only actual missing values return True. To detect empty
@@ -603,51 +723,37 @@
         --------
 
         >>> from shapely.geometry import Polygon
         >>> s = geopandas.GeoSeries(
         ...     [Polygon([(0, 0), (1, 1), (0, 1)]), None, Polygon([])]
         ... )
         >>> s
-        0    POLYGON ((0.00000 0.00000, 1.00000 1.00000, 0....
-        1                                                 None
-        2                             GEOMETRYCOLLECTION EMPTY
+        0    POLYGON ((0 0, 1 1, 0 1, 0 0))
+        1                              None
+        2                     POLYGON EMPTY
         dtype: geometry
+
         >>> s.isna()
         0    False
         1     True
         2    False
         dtype: bool
 
         See Also
         --------
         GeoSeries.notna : inverse of isna
         GeoSeries.is_empty : detect empty geometries
         """
-        if self.is_empty.any():
-            warnings.warn(
-                "GeoSeries.isna() previously returned True for both missing (None) "
-                "and empty geometries. Now, it only returns True for missing values. "
-                "Since the calling GeoSeries contains empty geometries, the result "
-                "has changed compared to previous versions of GeoPandas.\n"
-                "Given a GeoSeries 's', you can use 's.is_empty | s.isna()' to get "
-                "back the old behaviour.\n\n"
-                "To further ignore this warning, you can do: \n"
-                "import warnings; warnings.filterwarnings('ignore', 'GeoSeries.isna', "
-                "UserWarning)",
-                UserWarning,
-                stacklevel=2,
-            )
-
-        return super(GeoSeries, self).isna()
+        return super().isna()
 
-    def isnull(self):
+    def isnull(self) -> Series:
         """Alias for `isna` method. See `isna` for more detail."""
         return self.isna()
 
-    def notna(self):
+    def notna(self) -> Series:
         """
         Detect non-missing values.
 
         Historically, NA values in a GeoSeries could be represented by
         empty geometric objects, in addition to standard representations
         such as None and np.nan. This behaviour is changed in version 0.6.0,
         and now only actual missing values return False. To detect empty
@@ -662,18 +768,19 @@
         --------
 
         >>> from shapely.geometry import Polygon
         >>> s = geopandas.GeoSeries(
         ...     [Polygon([(0, 0), (1, 1), (0, 1)]), None, Polygon([])]
         ... )
         >>> s
-        0    POLYGON ((0.00000 0.00000, 1.00000 1.00000, 0....
-        1                                                 None
-        2                             GEOMETRYCOLLECTION EMPTY
+        0    POLYGON ((0 0, 1 1, 0 1, 0 0))
+        1                              None
+        2                     POLYGON EMPTY
         dtype: geometry
+
         >>> s.notna()
         0     True
         1    False
         2     True
         dtype: bool
 
         See Also
@@ -691,176 +798,188 @@
                 "back the old behaviour.\n\n"
                 "To further ignore this warning, you can do: \n"
                 "import warnings; warnings.filterwarnings('ignore', "
                 "'GeoSeries.notna', UserWarning)",
                 UserWarning,
                 stacklevel=2,
             )
-        return super(GeoSeries, self).notna()
+        return super().notna()
 
-    def notnull(self):
+    def notnull(self) -> Series:
         """Alias for `notna` method. See `notna` for more detail."""
         return self.notna()
 
-    def fillna(self, value=None, method=None, inplace=False, **kwargs):
-        """Fill NA values with a geometry (empty polygon by default).
+    def fillna(self, value=None, inplace: bool = False, **kwargs):
+        """
+        Fill NA values with geometry (or geometries).
+
+        Parameters
+        ----------
+        value : shapely geometry or GeoSeries, default None
+            If None is passed, NA values will be filled with GEOMETRYCOLLECTION EMPTY.
+            If a shapely geometry object is passed, it will be
+            used to fill all missing values. If a ``GeoSeries`` or ``GeometryArray``
+            are passed, missing values will be filled based on the corresponding index
+            locations. If pd.NA or np.nan are passed, values will be filled with
+            ``None`` (not GEOMETRYCOLLECTION EMPTY).
 
-        "method" is currently not implemented for pandas <= 0.12.
+        Returns
+        -------
+        GeoSeries
 
         Examples
         --------
-
         >>> from shapely.geometry import Polygon
         >>> s = geopandas.GeoSeries(
         ...     [
         ...         Polygon([(0, 0), (1, 1), (0, 1)]),
         ...         None,
         ...         Polygon([(0, 0), (-1, 1), (0, -1)]),
         ...     ]
         ... )
         >>> s
-        0    POLYGON ((0.00000 0.00000, 1.00000 1.00000, 0....
-        1                                                 None
-        2    POLYGON ((0.00000 0.00000, -1.00000 1.00000, 0...
+        0      POLYGON ((0 0, 1 1, 0 1, 0 0))
+        1                                None
+        2    POLYGON ((0 0, -1 1, 0 -1, 0 0))
         dtype: geometry
 
+        Filled with an empty polygon.
+
         >>> s.fillna()
-        0    POLYGON ((0.00000 0.00000, 1.00000 1.00000, 0....
-        1                             GEOMETRYCOLLECTION EMPTY
-        2    POLYGON ((0.00000 0.00000, -1.00000 1.00000, 0...
+        0      POLYGON ((0 0, 1 1, 0 1, 0 0))
+        1            GEOMETRYCOLLECTION EMPTY
+        2    POLYGON ((0 0, -1 1, 0 -1, 0 0))
         dtype: geometry
 
+        Filled with a specific polygon.
+
         >>> s.fillna(Polygon([(0, 1), (2, 1), (1, 2)]))
-        0    POLYGON ((0.00000 0.00000, 1.00000 1.00000, 0....
-        1    POLYGON ((0.00000 1.00000, 2.00000 1.00000, 1....
-        2    POLYGON ((0.00000 0.00000, -1.00000 1.00000, 0...
+        0      POLYGON ((0 0, 1 1, 0 1, 0 0))
+        1      POLYGON ((0 1, 2 1, 1 2, 0 1))
+        2    POLYGON ((0 0, -1 1, 0 -1, 0 0))
+        dtype: geometry
+
+        Filled with another GeoSeries.
+
+        >>> from shapely.geometry import Point
+        >>> s_fill = geopandas.GeoSeries(
+        ...     [
+        ...         Point(0, 0),
+        ...         Point(1, 1),
+        ...         Point(2, 2),
+        ...     ]
+        ... )
+        >>> s.fillna(s_fill)
+        0      POLYGON ((0 0, 1 1, 0 1, 0 0))
+        1                         POINT (1 1)
+        2    POLYGON ((0 0, -1 1, 0 -1, 0 0))
         dtype: geometry
 
         See Also
         --------
         GeoSeries.isna : detect missing values
         """
         if value is None:
-            value = BaseGeometry()
-        return super(GeoSeries, self).fillna(
-            value=value, method=method, inplace=inplace, **kwargs
-        )
+            value = GeometryCollection()
+        return super().fillna(value=value, inplace=inplace, **kwargs)
 
-    def __contains__(self, other):
+    def __contains__(self, other) -> bool:
         """Allow tests of the form "geom in s"
 
         Tests whether a GeoSeries contains a geometry.
 
         Note: This is not the same as the geometric method "contains".
         """
         if isinstance(other, BaseGeometry):
             return np.any(self.geom_equals(other))
         else:
             return False
 
+    @doc(plot_series)
     def plot(self, *args, **kwargs):
-        """Generate a plot of the geometries in the ``GeoSeries``.
-
-        Wraps the ``plot_series()`` function, and documentation is copied from
-        there.
-        """
         return plot_series(self, *args, **kwargs)
 
-    plot.__doc__ = plot_series.__doc__
+    @doc(_explore_geoseries)
+    def explore(self, *args, **kwargs):
+        """Interactive map based on folium/leaflet.js"""
+        return _explore_geoseries(self, *args, **kwargs)
 
-    def explode(self):
+    def explode(self, ignore_index=False, index_parts=False) -> GeoSeries:
         """
         Explode multi-part geometries into multiple single geometries.
 
         Single rows can become multiple rows.
         This is analogous to PostGIS's ST_Dump(). The 'path' index is the
         second level of the returned MultiIndex
 
+        Parameters
+        ----------
+        ignore_index : bool, default False
+            If True, the resulting index will be labelled 0, 1, …, n - 1,
+            ignoring `index_parts`.
+        index_parts : boolean, default False
+            If True, the resulting index will be a multi-index (original
+            index with an additional level indicating the multiple
+            geometries: a new zero-based index for each single part geometry
+            per multi-part geometry).
+
         Returns
-        ------
+        -------
         A GeoSeries with a MultiIndex. The levels of the MultiIndex are the
         original index and a zero-based integer index that counts the
         number of single geometries within a multi-part geometry.
 
         Examples
         --------
         >>> from shapely.geometry import MultiPoint
         >>> s = geopandas.GeoSeries(
         ...     [MultiPoint([(0, 0), (1, 1)]), MultiPoint([(2, 2), (3, 3), (4, 4)])]
         ... )
         >>> s
-        0        MULTIPOINT (0.00000 0.00000, 1.00000 1.00000)
-        1    MULTIPOINT (2.00000 2.00000, 3.00000 3.00000, ...
+        0           MULTIPOINT ((0 0), (1 1))
+        1    MULTIPOINT ((2 2), (3 3), (4 4))
         dtype: geometry
 
-        >>> s.explode()
-        0  0    POINT (0.00000 0.00000)
-           1    POINT (1.00000 1.00000)
-        1  0    POINT (2.00000 2.00000)
-           1    POINT (3.00000 3.00000)
-           2    POINT (4.00000 4.00000)
+        >>> s.explode(index_parts=True)
+        0  0    POINT (0 0)
+           1    POINT (1 1)
+        1  0    POINT (2 2)
+           1    POINT (3 3)
+           2    POINT (4 4)
         dtype: geometry
 
         See also
         --------
         GeoDataFrame.explode
 
         """
+        from .base import _get_index_for_parts
 
-        if compat.USE_PYGEOS and compat.PYGEOS_GE_09:
-            import pygeos  # noqa
-
-            geometries, outer_idx = pygeos.get_parts(
-                self.values.data, return_index=True
-            )
-
-            if len(outer_idx):
-                # Generate inner index as a range per value of outer_idx
-                # 1. identify the start of each run of values in outer_idx
-                # 2. count number of values per run
-                # 3. use cumulative sums to create an incremental range
-                #    starting at 0 in each run
-                run_start = np.r_[True, outer_idx[:-1] != outer_idx[1:]]
-                counts = np.diff(np.r_[np.nonzero(run_start)[0], len(outer_idx)])
-                inner_index = (~run_start).cumsum()
-                inner_index -= np.repeat(inner_index[run_start], counts)
+        geometries, outer_idx = shapely.get_parts(self.values._data, return_index=True)
 
-            else:
-                inner_index = []
-
-            # extract original index values based on integer index
-            outer_index = self.index.take(outer_idx)
-
-            index = MultiIndex.from_arrays(
-                [outer_index, inner_index], names=self.index.names + [None]
-            )
-
-            return GeoSeries(geometries, index=index, crs=self.crs).__finalize__(self)
-
-        # else PyGEOS is not available or version <= 0.8
+        index = _get_index_for_parts(
+            self.index,
+            outer_idx,
+            ignore_index=ignore_index,
+            index_parts=index_parts,
+        )
 
-        index = []
-        geometries = []
-        for idx, s in self.geometry.iteritems():
-            if s.type.startswith("Multi") or s.type == "GeometryCollection":
-                geoms = s.geoms
-                idxs = [(idx, i) for i in range(len(geoms))]
-            else:
-                geoms = [s]
-                idxs = [(idx, 0)]
-            index.extend(idxs)
-            geometries.extend(geoms)
-        index = MultiIndex.from_tuples(index, names=self.index.names + [None])
         return GeoSeries(geometries, index=index, crs=self.crs).__finalize__(self)
 
     #
     # Additional methods
     #
-
-    def set_crs(self, crs=None, epsg=None, inplace=False, allow_override=False):
+    @compat.requires_pyproj
+    def set_crs(
+        self,
+        crs: Optional[Any] = None,
+        epsg: Optional[int] = None,
+        inplace: bool = False,
+        allow_override: bool = False,
+    ):
         """
         Set the Coordinate Reference System (CRS) of a ``GeoSeries``.
 
         NOTE: The underlying geometries are not transformed to this CRS. To
         transform the geometries to a new CRS, use the ``to_crs`` method.
 
         Parameters
@@ -884,17 +1003,17 @@
         GeoSeries
 
         Examples
         --------
         >>> from shapely.geometry import Point
         >>> s = geopandas.GeoSeries([Point(1, 1), Point(2, 2), Point(3, 3)])
         >>> s
-        0    POINT (1.00000 1.00000)
-        1    POINT (2.00000 2.00000)
-        2    POINT (3.00000 3.00000)
+        0    POINT (1 1)
+        1    POINT (2 2)
+        2    POINT (3 3)
         dtype: geometry
 
         Setting CRS to a GeoSeries without one:
 
         >>> s.crs is None
         True
 
@@ -923,14 +1042,16 @@
         override CRS.
 
         See Also
         --------
         GeoSeries.to_crs : re-project to another CRS
 
         """
+        from pyproj import CRS
+
         if crs is not None:
             crs = CRS.from_user_input(crs)
         elif epsg is not None:
             crs = CRS.from_epsg(epsg)
         else:
             raise ValueError("Must pass either crs or epsg.")
 
@@ -944,24 +1065,26 @@
         if not inplace:
             result = self.copy()
         else:
             result = self
         result.crs = crs
         return result
 
-    def to_crs(self, crs=None, epsg=None):
+    def to_crs(
+        self, crs: Optional[Any] = None, epsg: Optional[int] = None
+    ) -> GeoSeries:
         """Returns a ``GeoSeries`` with all geometries transformed to a new
         coordinate reference system.
 
         Transform all geometries in a GeoSeries to a different coordinate
         reference system.  The ``crs`` attribute on the current GeoSeries must
         be set.  Either ``crs`` or ``epsg`` may be specified for output.
 
         This method will transform all points in all objects.  It has no notion
-        or projecting entire geometries.  All segments joining points are
+        of projecting entire geometries.  All segments joining points are
         assumed to be lines in the current projection, not geodesics.  Objects
         crossing the dateline (or other projection boundary) will have
         undesirable behavior.
 
         Parameters
         ----------
         crs : pyproj.CRS, optional if `epsg` is specified
@@ -976,17 +1099,17 @@
         GeoSeries
 
         Examples
         --------
         >>> from shapely.geometry import Point
         >>> s = geopandas.GeoSeries([Point(1, 1), Point(2, 2), Point(3, 3)], crs=4326)
         >>> s
-        0    POINT (1.00000 1.00000)
-        1    POINT (2.00000 2.00000)
-        2    POINT (3.00000 3.00000)
+        0    POINT (1 1)
+        1    POINT (2 2)
+        2    POINT (3 3)
         dtype: geometry
         >>> s.crs  # doctest: +SKIP
         <Geographic 2D CRS: EPSG:4326>
         Name: WGS 84
         Axis Info [ellipsoidal]:
         - Lat[north]: Geodetic latitude (degree)
         - Lon[east]: Geodetic longitude (degree)
@@ -1024,184 +1147,216 @@
         GeoSeries.set_crs : assign CRS
 
         """
         return GeoSeries(
             self.values.to_crs(crs=crs, epsg=epsg), index=self.index, name=self.name
         )
 
-    def estimate_utm_crs(self, datum_name="WGS 84"):
+    def estimate_utm_crs(self, datum_name: str = "WGS 84"):
         """Returns the estimated UTM CRS based on the bounds of the dataset.
 
         .. versionadded:: 0.9
 
-        .. note:: Requires pyproj 3+
-
         Parameters
         ----------
         datum_name : str, optional
             The name of the datum to use in the query. Default is WGS 84.
 
         Returns
         -------
         pyproj.CRS
 
         Examples
         --------
-        >>> world = geopandas.read_file(
-        ...     geopandas.datasets.get_path("naturalearth_lowres")
+        >>> import geodatasets
+        >>> df = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.chicago_health")
         ... )
-        >>> germany = world.loc[world.name == "Germany"]
-        >>> germany.geometry.estimate_utm_crs()  # doctest: +SKIP
-        <Projected CRS: EPSG:32632>
-        Name: WGS 84 / UTM zone 32N
+        >>> df.geometry.estimate_utm_crs()  # doctest: +SKIP
+        <Derived Projected CRS: EPSG:32616>
+        Name: WGS 84 / UTM zone 16N
         Axis Info [cartesian]:
         - E[east]: Easting (metre)
         - N[north]: Northing (metre)
         Area of Use:
-        - name: World - N hemisphere - 6°E to 12°E - by country
-        - bounds: (6.0, 0.0, 12.0, 84.0)
+        - name: Between 90°W and 84°W, northern hemisphere between equator and 84°N, ...
+        - bounds: (-90.0, 0.0, -84.0, 84.0)
         Coordinate Operation:
-        - name: UTM zone 32N
+        - name: UTM zone 16N
         - method: Transverse Mercator
-        Datum: World Geodetic System 1984
+        Datum: World Geodetic System 1984 ensemble
         - Ellipsoid: WGS 84
         - Prime Meridian: Greenwich
         """
         return self.values.estimate_utm_crs(datum_name)
 
-    def to_json(self, **kwargs):
+    def to_json(
+        self,
+        show_bbox: bool = True,
+        drop_id: bool = False,
+        to_wgs84: bool = False,
+        **kwargs,
+    ) -> str:
         """
         Returns a GeoJSON string representation of the GeoSeries.
 
         Parameters
         ----------
+        show_bbox : bool, optional, default: True
+            Include bbox (bounds) in the geojson
+        drop_id : bool, default: False
+            Whether to retain the index of the GeoSeries as the id property
+            in the generated GeoJSON. Default is False, but may want True
+            if the index is just arbitrary row numbers.
+        to_wgs84: bool, optional, default: False
+            If the CRS is set on the active geometry column it is exported as
+            WGS84 (EPSG:4326) to meet the `2016 GeoJSON specification
+            <https://tools.ietf.org/html/rfc7946>`_.
+            Set to True to force re-projection and set to False to ignore CRS. False by
+            default.
+
         *kwargs* that will be passed to json.dumps().
 
         Returns
         -------
         JSON string
 
         Examples
         --------
         >>> from shapely.geometry import Point
         >>> s = geopandas.GeoSeries([Point(1, 1), Point(2, 2), Point(3, 3)])
         >>> s
-        0    POINT (1.00000 1.00000)
-        1    POINT (2.00000 2.00000)
-        2    POINT (3.00000 3.00000)
+        0    POINT (1 1)
+        1    POINT (2 2)
+        2    POINT (3 3)
         dtype: geometry
 
         >>> s.to_json()
         '{"type": "FeatureCollection", "features": [{"id": "0", "type": "Feature", "pr\
 operties": {}, "geometry": {"type": "Point", "coordinates": [1.0, 1.0]}, "bbox": [1.0,\
  1.0, 1.0, 1.0]}, {"id": "1", "type": "Feature", "properties": {}, "geometry": {"type"\
 : "Point", "coordinates": [2.0, 2.0]}, "bbox": [2.0, 2.0, 2.0, 2.0]}, {"id": "2", "typ\
 e": "Feature", "properties": {}, "geometry": {"type": "Point", "coordinates": [3.0, 3.\
 0]}, "bbox": [3.0, 3.0, 3.0, 3.0]}], "bbox": [1.0, 1.0, 3.0, 3.0]}'
 
         See Also
         --------
         GeoSeries.to_file : write GeoSeries to file
         """
-        return json.dumps(self.__geo_interface__, **kwargs)
+        return self.to_frame("geometry").to_json(
+            na="null", show_bbox=show_bbox, drop_id=drop_id, to_wgs84=to_wgs84, **kwargs
+        )
 
-    def to_wkb(self, hex=False, **kwargs):
+    def to_wkb(self, hex: bool = False, **kwargs) -> Series:
         """
         Convert GeoSeries geometries to WKB
 
         Parameters
         ----------
         hex : bool
             If true, export the WKB as a hexadecimal string.
             The default is to return a binary bytes object.
         kwargs
             Additional keyword args will be passed to
-            :func:`pygeos.to_wkb` if pygeos is installed.
+            :func:`shapely.to_wkb`.
 
         Returns
         -------
         Series
             WKB representations of the geometries
 
         See also
         --------
         GeoSeries.to_wkt
         """
         return Series(to_wkb(self.array, hex=hex, **kwargs), index=self.index)
 
-    def to_wkt(self, **kwargs):
+    def to_wkt(self, **kwargs) -> Series:
         """
         Convert GeoSeries geometries to WKT
 
         Parameters
         ----------
         kwargs
-            Keyword args will be passed to :func:`pygeos.to_wkt`
-            if pygeos is installed.
+            Keyword args will be passed to :func:`shapely.to_wkt`.
 
         Returns
         -------
         Series
             WKT representations of the geometries
 
         Examples
         --------
         >>> from shapely.geometry import Point
         >>> s = geopandas.GeoSeries([Point(1, 1), Point(2, 2), Point(3, 3)])
         >>> s
-        0    POINT (1.00000 1.00000)
-        1    POINT (2.00000 2.00000)
-        2    POINT (3.00000 3.00000)
+        0    POINT (1 1)
+        1    POINT (2 2)
+        2    POINT (3 3)
         dtype: geometry
 
         >>> s.to_wkt()
         0    POINT (1 1)
         1    POINT (2 2)
         2    POINT (3 3)
         dtype: object
 
         See also
         --------
         GeoSeries.to_wkb
         """
         return Series(to_wkt(self.array, **kwargs), index=self.index)
 
-    #
-    # Implement standard operators for GeoSeries
-    #
+    def clip(self, mask, keep_geom_type: bool = False) -> GeoSeries:
+        """Clip points, lines, or polygon geometries to the mask extent.
 
-    def __xor__(self, other):
-        """Implement ^ operator as for builtin set type"""
-        warnings.warn(
-            "'^' operator will be deprecated. Use the 'symmetric_difference' "
-            "method instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.symmetric_difference(other)
+        Both layers must be in the same Coordinate Reference System (CRS).
+        The GeoSeries will be clipped to the full extent of the `mask` object.
 
-    def __or__(self, other):
-        """Implement | operator as for builtin set type"""
-        warnings.warn(
-            "'|' operator will be deprecated. Use the 'union' method instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.union(other)
+        If there are multiple polygons in mask, data from the GeoSeries will be
+        clipped to the total boundary of all polygons in mask.
 
-    def __and__(self, other):
-        """Implement & operator as for builtin set type"""
-        warnings.warn(
-            "'&' operator will be deprecated. Use the 'intersection' method instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.intersection(other)
+        Parameters
+        ----------
+        mask : GeoDataFrame, GeoSeries, (Multi)Polygon, list-like
+            Polygon vector layer used to clip `gdf`.
+            The mask's geometry is dissolved into one geometric feature
+            and intersected with GeoSeries.
+            If the mask is list-like with four elements ``(minx, miny, maxx, maxy)``,
+            ``clip`` will use a faster rectangle clipping
+            (:meth:`~GeoSeries.clip_by_rect`), possibly leading to slightly different
+            results.
+        keep_geom_type : boolean, default False
+            If True, return only geometries of original type in case of intersection
+            resulting in multiple geometry types or GeometryCollections.
+            If False, return all resulting geometries (potentially mixed-types).
 
-    def __sub__(self, other):
-        """Implement - operator as for builtin set type"""
-        warnings.warn(
-            "'-' operator will be deprecated. Use the 'difference' method instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.difference(other)
+        Returns
+        -------
+        GeoSeries
+            Vector data (points, lines, polygons) from `gdf` clipped to
+            polygon boundary from mask.
+
+        See also
+        --------
+        clip : top-level function for clip
+
+        Examples
+        --------
+        Clip points (grocery stores) with polygons (the Near West Side community):
+
+        >>> import geodatasets
+        >>> chicago = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.chicago_health")
+        ... )
+        >>> near_west_side = chicago[chicago["community"] == "NEAR WEST SIDE"]
+        >>> groceries = geopandas.read_file(
+        ...     geodatasets.get_path("geoda.groceries")
+        ... ).to_crs(chicago.crs)
+        >>> groceries.shape
+        (148, 8)
+
+        >>> nws_groceries = groceries.geometry.clip(near_west_side)
+        >>> nws_groceries.shape
+        (7,)
+        """
+        return geopandas.clip(self, mask=mask, keep_geom_type=keep_geom_type)
```

### Comparing `geopandas-0.9.0/geopandas/io/sql.py` & `geopandas-1.0.0a1/geopandas/io/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import warnings
 from contextlib import contextmanager
 
 import pandas as pd
 
+import shapely
 import shapely.wkb
 
 from geopandas import GeoDataFrame
 
-from .. import _compat as compat
-
 
 @contextmanager
 def _get_conn(conn_or_engine):
     """
     Yield a connection within a transaction context.
 
     Engine.begin() returns a Connection with an implicit Transaction while
@@ -26,15 +25,18 @@
     Returns
     -------
     Connection
     """
     from sqlalchemy.engine.base import Engine, Connection
 
     if isinstance(conn_or_engine, Connection):
-        with conn_or_engine.begin():
+        if not conn_or_engine.in_transaction():
+            with conn_or_engine.begin():
+                yield conn_or_engine
+        else:
             yield conn_or_engine
     elif isinstance(conn_or_engine, Engine):
         with conn_or_engine.begin() as conn:
             yield conn
     else:
         raise ValueError(f"Unknown Connectable: {conn_or_engine}")
 
@@ -60,36 +62,38 @@
     -------
     GeoDataFrame
     """
 
     if geom_col not in df:
         raise ValueError("Query missing geometry column '{}'".format(geom_col))
 
+    if df.columns.to_list().count(geom_col) > 1:
+        raise ValueError(
+            f"Duplicate geometry column '{geom_col}' detected in SQL query output. Only"
+            "one geometry column is allowed."
+        )
+
     geoms = df[geom_col].dropna()
 
     if not geoms.empty:
         load_geom_bytes = shapely.wkb.loads
         """Load from Python 3 binary."""
 
-        def load_geom_buffer(x):
-            """Load from Python 2 binary."""
-            return shapely.wkb.loads(str(x))
-
         def load_geom_text(x):
             """Load from binary encoded as text."""
             return shapely.wkb.loads(str(x), hex=True)
 
         if isinstance(geoms.iat[0], bytes):
             load_geom = load_geom_bytes
         else:
             load_geom = load_geom_text
 
         df[geom_col] = geoms = geoms.apply(load_geom)
         if crs is None:
-            srid = shapely.geos.lgeos.GEOSGetSRID(geoms.iat[0]._geom)
+            srid = shapely.get_srid(geoms.iat[0])
             # if no defined SRID in geodatabase, returns SRID of 0
             if srid != 0:
                 crs = "epsg:{}".format(srid)
 
     return GeoDataFrame(df, crs=crs, geometry=geom_col)
 
 
@@ -104,14 +108,17 @@
     params=None,
     chunksize=None,
 ):
     """
     Returns a GeoDataFrame corresponding to the result of the query
     string, which must contain a geometry column in WKB representation.
 
+    It is also possible to use :meth:`~GeoDataFrame.read_file` to read from a database.
+    Especially for file geodatabases like GeoPackage or SpatiaLite this can be easier.
+
     Parameters
     ----------
     sql : string
         SQL query to execute in selecting entries from database, or name
         of the table to read from the database.
     con : sqlalchemy.engine.Connection or sqlalchemy.engine.Engine
         Active connection to the database to query.
@@ -134,22 +141,22 @@
     GeoDataFrame
 
     Examples
     --------
     PostGIS
 
     >>> from sqlalchemy import create_engine  # doctest: +SKIP
-    >>> db_connection_url = "postgres://myusername:mypassword@myhost:5432/mydatabase"
+    >>> db_connection_url = "postgresql://myusername:mypassword@myhost:5432/mydatabase"
     >>> con = create_engine(db_connection_url)  # doctest: +SKIP
     >>> sql = "SELECT geom, highway FROM roads"
     >>> df = geopandas.read_postgis(sql, con)  # doctest: +SKIP
 
     SpatiaLite
 
-    >>> sql = "SELECT ST_Binary(geom) AS geom, highway FROM roads"
+    >>> sql = "SELECT ST_AsBinary(geom) AS geom, highway FROM roads"
     >>> df = geopandas.read_postgis(sql, con)  # doctest: +SKIP
     """
 
     if chunksize is None:
         # read all in one chunk and return a single GeoDataFrame
         df = pd.read_sql(
             sql,
@@ -172,27 +179,14 @@
             parse_dates=parse_dates,
             params=params,
             chunksize=chunksize,
         )
         return (_df_to_geodf(df, geom_col=geom_col, crs=crs) for df in df_generator)
 
 
-def read_postgis(*args, **kwargs):
-    import warnings
-
-    warnings.warn(
-        "geopandas.io.sql.read_postgis() is intended for internal "
-        "use only, and will be deprecated. Use geopandas.read_postgis() instead.",
-        DeprecationWarning,
-        stacklevel=2,
-    )
-
-    return _read_postgis(*args, **kwargs)
-
-
 def _get_geometry_type(gdf):
     """
     Get basic geometry type of a GeoDataFrame. See more info from:
     https://geoalchemy-2.readthedocs.io/en/latest/types.html#geoalchemy2.types._GISType
 
     Following rules apply:
      - if geometries all share the same geometry-type,
@@ -226,68 +220,73 @@
             else:
                 target_geom_type = geom_types[0].upper()
     else:
         target_geom_type = "GEOMETRY"
 
     # Check for 3D-coordinates
     if any(gdf.geometry.has_z):
-        target_geom_type = target_geom_type + "Z"
+        target_geom_type += "Z"
 
     return target_geom_type, has_curve
 
 
 def _get_srid_from_crs(gdf):
     """
     Get EPSG code from CRS if available. If not, return -1.
     """
 
     # Use geoalchemy2 default for srid
     # Note: undefined srid in PostGIS is 0
-    srid = -1
+    srid = None
     warning_msg = (
         "Could not parse CRS from the GeoDataFrame. "
-        + "Inserting data without defined CRS.",
+        "Inserting data without defined CRS."
     )
     if gdf.crs is not None:
         try:
-            srid = gdf.crs.to_epsg(min_confidence=25)
-            if srid is None:
-                srid = -1
-                warnings.warn(warning_msg, UserWarning, stacklevel=2)
+            for confidence in (100, 70, 25):
+                srid = gdf.crs.to_epsg(min_confidence=confidence)
+                if srid is not None:
+                    break
+                auth_srid = gdf.crs.to_authority(
+                    auth_name="ESRI", min_confidence=confidence
+                )
+                if auth_srid is not None:
+                    srid = int(auth_srid[1])
+                    break
         except Exception:
             warnings.warn(warning_msg, UserWarning, stacklevel=2)
+
+    if srid is None:
+        srid = -1
+        warnings.warn(warning_msg, UserWarning, stacklevel=2)
+
     return srid
 
 
 def _convert_linearring_to_linestring(gdf, geom_name):
     from shapely.geometry import LineString
 
-    # Todo: Use Pygeos function once it's implemented:
-    #  https://github.com/pygeos/pygeos/issues/76
+    # Todo: Use shapely function once it's implemented:
+    # https://github.com/shapely/shapely/issues/1617
 
     mask = gdf.geom_type == "LinearRing"
     gdf.loc[mask, geom_name] = gdf.loc[mask, geom_name].apply(
         lambda geom: LineString(geom)
     )
     return gdf
 
 
 def _convert_to_ewkb(gdf, geom_name, srid):
-    """Convert geometries to ewkb. """
-    if compat.USE_PYGEOS:
-        from pygeos import set_srid, to_wkb
-
-        geoms = to_wkb(
-            set_srid(gdf[geom_name].values.data, srid=srid), hex=True, include_srid=True
-        )
-
-    else:
-        from shapely.wkb import dumps
-
-        geoms = [dumps(geom, srid=srid, hex=True) for geom in gdf[geom_name]]
+    """Convert geometries to ewkb."""
+    geoms = shapely.to_wkb(
+        shapely.set_srid(gdf[geom_name].values._data, srid=srid),
+        hex=True,
+        include_srid=True,
+    )
 
     # The gdf will warn that the geometry column doesn't hold in-memory geometries
     # now that they are EWKB, so convert back to a regular dataframe to avoid warning
     # the user that the dtypes are unexpected.
     df = pd.DataFrame(gdf, copy=False)
     df[geom_name] = geoms
     return df
@@ -301,19 +300,24 @@
     writer = csv.writer(s_buf)
     writer.writerows(data_iter)
     s_buf.seek(0)
 
     columns = ", ".join('"{}"'.format(k) for k in keys)
 
     dbapi_conn = conn.connection
+    sql = 'COPY "{}"."{}" ({}) FROM STDIN WITH CSV'.format(
+        tbl.table.schema, tbl.table.name, columns
+    )
     with dbapi_conn.cursor() as cur:
-        sql = 'COPY "{}"."{}" ({}) FROM STDIN WITH CSV'.format(
-            tbl.table.schema, tbl.table.name, columns
-        )
-        cur.copy_expert(sql=sql, file=s_buf)
+        # Use psycopg method if it's available
+        if hasattr(cur, "copy") and callable(cur.copy):
+            with cur.copy(sql) as copy:
+                copy.write(s_buf.read())
+        else:  # otherwise use psycopg2 method
+            cur.copy_expert(sql, s_buf)
 
 
 def _write_postgis(
     gdf,
     name,
     con,
     schema=None,
@@ -358,30 +362,23 @@
         The keys should be the column names and the values
         should be the SQLAlchemy types.
 
     Examples
     --------
 
     >>> from sqlalchemy import create_engine  # doctest: +SKIP
-    >>> engine = create_engine("postgres://myusername:mypassword@myhost:5432\
+    >>> engine = create_engine("postgresql://myusername:mypassword@myhost:5432\
 /mydatabase";)  # doctest: +SKIP
     >>> gdf.to_postgis("my_table", engine)  # doctest: +SKIP
     """
     try:
         from geoalchemy2 import Geometry
+        from sqlalchemy import text
     except ImportError:
-        raise ImportError("'to_postgis()' requires geoalchemy2 package. ")
-
-    if not compat.SHAPELY_GE_17:
-        raise ImportError(
-            "'to_postgis()' requires newer version of Shapely "
-            "(>= '1.7.0').\nYou can update the library using "
-            "'pip install shapely --upgrade' or using "
-            "'conda update shapely' if using conda package manager."
-        )
+        raise ImportError("'to_postgis()' requires geoalchemy2 package.")
 
     gdf = gdf.copy()
     geom_name = gdf.geometry.name
 
     # Get srid
     srid = _get_srid_from_crs(gdf)
 
@@ -408,36 +405,35 @@
 
     if if_exists == "append":
         # Check that the geometry srid matches with the current GeoDataFrame
         with _get_conn(con) as connection:
             # Only check SRID if table exists
             if connection.dialect.has_table(connection, name, schema):
                 target_srid = connection.execute(
-                    "SELECT Find_SRID('{schema}', '{table}', '{geom_col}');".format(
-                        schema=schema_name, table=name, geom_col=geom_name
+                    text(
+                        "SELECT Find_SRID('{schema}', '{table}', '{geom_col}');".format(
+                            schema=schema_name, table=name, geom_col=geom_name
+                        )
                     )
                 ).fetchone()[0]
 
                 if target_srid != srid:
                     msg = (
                         "The CRS of the target table (EPSG:{epsg_t}) differs from the "
                         "CRS of current GeoDataFrame (EPSG:{epsg_src}).".format(
                             epsg_t=target_srid, epsg_src=srid
                         )
                     )
                     raise ValueError(msg)
 
     with _get_conn(con) as connection:
-
         gdf.to_sql(
             name,
             connection,
             schema=schema_name,
             if_exists=if_exists,
             index=index,
             index_label=index_label,
             chunksize=chunksize,
             dtype=dtype,
             method=_psql_insert_copy,
         )
-
-    return
```

### Comparing `geopandas-0.9.0/geopandas/plotting.py` & `geopandas-1.0.0a1/geopandas/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,83 +1,74 @@
 import warnings
 
 import numpy as np
 import pandas as pd
+from pandas.plotting import PlotAccessor
+from pandas import CategoricalDtype
 
 import geopandas
 
-from distutils.version import LooseVersion
+from packaging.version import Version
 
+from ._decorator import doc
 
-def deprecated(new):
-    """Helper to provide deprecation warning."""
 
-    def old(*args, **kwargs):
-        warnings.warn(
-            "{} is intended for internal ".format(new.__name__[1:])
-            + "use only, and will be deprecated.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        new(*args, **kwargs)
-
-    return old
-
-
-def _flatten_multi_geoms(geoms, prefix="Multi"):
+def _sanitize_geoms(geoms, prefix="Multi"):
     """
     Returns Series like geoms and index, except that any Multi geometries
     are split into their components and indices are repeated for all component
-    in the same Multi geometry.  Maintains 1:1 matching of geometry to value.
+    in the same Multi geometry. At the same time, empty or missing geometries are
+    filtered out.  Maintains 1:1 matching of geometry to value.
 
     Prefix specifies type of geometry to be flatten. 'Multi' for MultiPoint and similar,
     "Geom" for GeometryCollection.
 
     Returns
     -------
     components : list of geometry
 
     component_index : index array
         indices are repeated for all components in the same Multi geometry
     """
+    # TODO(shapely) look into simplifying this with
+    # shapely.get_parts(geoms, return_index=True) from shapely 2.0
     components, component_index = [], []
 
-    if not geoms.geom_type.str.startswith(prefix).any():
+    if (
+        not geoms.geom_type.str.startswith(prefix).any()
+        and not geoms.is_empty.any()
+        and not geoms.isna().any()
+    ):
         return geoms, np.arange(len(geoms))
 
     for ix, geom in enumerate(geoms):
-        if geom is not None and geom.type.startswith(prefix) and not geom.is_empty:
+        if geom is not None and geom.geom_type.startswith(prefix) and not geom.is_empty:
             for poly in geom.geoms:
                 components.append(poly)
                 component_index.append(ix)
+        elif geom is None or geom.is_empty:
+            continue
         else:
             components.append(geom)
             component_index.append(ix)
 
     return components, np.array(component_index)
 
 
 def _expand_kwargs(kwargs, multiindex):
     """
     Most arguments to the plot functions must be a (single) value, or a sequence
     of values. This function checks each key-value pair in 'kwargs' and expands
     it (in place) to the correct length/formats with help of 'multiindex', unless
     the value appears to already be a valid (single) value for the key.
     """
-    import matplotlib
     from matplotlib.colors import is_color_like
     from typing import Iterable
 
-    mpl = matplotlib.__version__
-    if mpl >= LooseVersion("3.4") or (mpl > LooseVersion("3.3.2") and "+" in mpl):
-        # alpha is supported as array argument with matplotlib 3.4+
-        scalar_kwargs = ["marker"]
-    else:
-        scalar_kwargs = ["marker", "alpha"]
-
+    scalar_kwargs = ["marker", "path_effects"]
     for att, value in kwargs.items():
         if "color" in att:  # color(s), edgecolor(s), facecolor(s)
             if is_color_like(value):
                 continue
         elif "linestyle" in att:  # linestyle(s)
             # A single linestyle can be 2-tuple of a number and an iterable.
             if (
@@ -147,15 +138,15 @@
 
     Returns
     -------
     collection : matplotlib.collections.Collection that was plotted
     """
     from matplotlib.collections import PatchCollection
 
-    geoms, multiindex = _flatten_multi_geoms(geoms)
+    geoms, multiindex = _sanitize_geoms(geoms)
     if values is not None:
         values = np.take(values, multiindex, axis=0)
 
     # PatchCollection does not accept some kwargs.
     kwargs = {
         att: value
         for att, value in kwargs.items()
@@ -164,32 +155,27 @@
 
     # Add to kwargs for easier checking below.
     if color is not None:
         kwargs["color"] = color
 
     _expand_kwargs(kwargs, multiindex)
 
-    collection = PatchCollection(
-        [_PolygonPatch(poly) for poly in geoms if not poly.is_empty], **kwargs
-    )
+    collection = PatchCollection([_PolygonPatch(poly) for poly in geoms], **kwargs)
 
     if values is not None:
         collection.set_array(np.asarray(values))
         collection.set_cmap(cmap)
         if "norm" not in kwargs:
             collection.set_clim(vmin, vmax)
 
     ax.add_collection(collection, autolim=True)
     ax.autoscale_view()
     return collection
 
 
-plot_polygon_collection = deprecated(_plot_polygon_collection)
-
-
 def _plot_linestring_collection(
     ax, geoms, values=None, color=None, cmap=None, vmin=None, vmax=None, **kwargs
 ):
     """
     Plots a collection of LineString and MultiLineString geometries to `ax`
 
     Parameters
@@ -206,15 +192,15 @@
 
     Returns
     -------
     collection : matplotlib.collections.Collection that was plotted
     """
     from matplotlib.collections import LineCollection
 
-    geoms, multiindex = _flatten_multi_geoms(geoms)
+    geoms, multiindex = _sanitize_geoms(geoms)
     if values is not None:
         values = np.take(values, multiindex, axis=0)
 
     # LineCollection does not accept some kwargs.
     kwargs = {
         att: value
         for att, value in kwargs.items()
@@ -237,17 +223,14 @@
             collection.set_clim(vmin, vmax)
 
     ax.add_collection(collection, autolim=True)
     ax.autoscale_view()
     return collection
 
 
-plot_linestring_collection = deprecated(_plot_linestring_collection)
-
-
 def _plot_point_collection(
     ax,
     geoms,
     values=None,
     color=None,
     cmap=None,
     vmin=None,
@@ -276,15 +259,15 @@
     Returns
     -------
     collection : matplotlib.collections.Collection that was plotted
     """
     if values is not None and color is not None:
         raise ValueError("Can only specify one of 'values' and 'color' kwargs")
 
-    geoms, multiindex = _flatten_multi_geoms(geoms)
+    geoms, multiindex = _sanitize_geoms(geoms)
     # values are expanded below as kwargs["c"]
 
     x = [p.x if not p.is_empty else None for p in geoms]
     y = [p.y if not p.is_empty else None for p in geoms]
 
     # matplotlib 1.4 does not support c=None, and < 2.0 does not support s=None
     if values is not None:
@@ -303,40 +286,37 @@
         collection = ax.scatter(x, y, vmin=vmin, vmax=vmax, cmap=cmap, **kwargs)
     else:
         collection = ax.scatter(x, y, cmap=cmap, **kwargs)
 
     return collection
 
 
-plot_point_collection = deprecated(_plot_point_collection)
-
-
 def plot_series(
     s, cmap=None, color=None, ax=None, figsize=None, aspect="auto", **style_kwds
 ):
     """
     Plot a GeoSeries.
 
     Generate a plot of a GeoSeries geometry with matplotlib.
 
     Parameters
     ----------
     s : Series
         The GeoSeries to be plotted. Currently Polygon,
-        MultiPolygon, LineString, MultiLineString and Point
+        MultiPolygon, LineString, MultiLineString, Point and MultiPoint
         geometries can be plotted.
     cmap : str (default None)
         The name of a colormap recognized by matplotlib. Any
         colormap will work, but categorical colormaps are
         generally recommended. Examples of useful discrete
         colormaps include:
 
             tab10, tab20, Accent, Dark2, Paired, Pastel1, Set1, Set2
 
-    color : str (default None)
+    color : str, np.array, pd.Series, List (default None)
         If specified, all objects will be colored uniformly.
     ax : matplotlib.pyplot.Artist (default None)
         axes on which to draw the plot
     figsize : pair of floats (default None)
         Size of the resulting matplotlib.figure.Figure. If the argument
         ax is given explicitly, figsize is ignored.
     aspect : 'auto', 'equal', None or float (default 'auto')
@@ -352,28 +332,14 @@
         as ``edgecolor``, ``facecolor``, ``linewidth``, ``markersize``,
         ``alpha``.
 
     Returns
     -------
     ax : matplotlib axes instance
     """
-    if "colormap" in style_kwds:
-        warnings.warn(
-            "'colormap' is deprecated, please use 'cmap' instead "
-            "(for consistency with matplotlib)",
-            FutureWarning,
-        )
-        cmap = style_kwds.pop("colormap")
-    if "axes" in style_kwds:
-        warnings.warn(
-            "'axes' is deprecated, please use 'ax' instead "
-            "(for consistency with pandas)",
-            FutureWarning,
-        )
-        ax = style_kwds.pop("axes")
 
     try:
         import matplotlib.pyplot as plt
     except ImportError:
         raise ImportError(
             "The matplotlib package is required for plotting in geopandas. "
             "You can install it using 'conda install -c conda-forge matplotlib' or "
@@ -396,79 +362,93 @@
         ax.set_aspect(aspect)
 
     if s.empty:
         warnings.warn(
             "The GeoSeries you are attempting to plot is "
             "empty. Nothing has been displayed.",
             UserWarning,
+            stacklevel=3,
         )
         return ax
 
     if s.is_empty.all():
         warnings.warn(
             "The GeoSeries you are attempting to plot is "
             "composed of empty geometries. Nothing has been displayed.",
             UserWarning,
+            stacklevel=3,
         )
         return ax
 
+    # have colors been given for all geometries?
+    color_given = pd.api.types.is_list_like(color) and len(color) == len(s)
+
     # if cmap is specified, create range of colors based on cmap
     values = None
     if cmap is not None:
         values = np.arange(len(s))
         if hasattr(cmap, "N"):
             values = values % cmap.N
         style_kwds["vmin"] = style_kwds.get("vmin", values.min())
         style_kwds["vmax"] = style_kwds.get("vmax", values.max())
 
     # decompose GeometryCollections
-    geoms, multiindex = _flatten_multi_geoms(s.geometry, prefix="Geom")
+    geoms, multiindex = _sanitize_geoms(s.geometry, prefix="Geom")
     values = np.take(values, multiindex, axis=0) if cmap else None
+    # ensure indexes are consistent
+    if color_given and isinstance(color, pd.Series):
+        color = color.reindex(s.index)
+    expl_color = np.take(color, multiindex, axis=0) if color_given else color
     expl_series = geopandas.GeoSeries(geoms)
 
-    geom_types = expl_series.type
+    geom_types = expl_series.geom_type
     poly_idx = np.asarray((geom_types == "Polygon") | (geom_types == "MultiPolygon"))
     line_idx = np.asarray(
         (geom_types == "LineString")
         | (geom_types == "MultiLineString")
         | (geom_types == "LinearRing")
     )
     point_idx = np.asarray((geom_types == "Point") | (geom_types == "MultiPoint"))
 
     # plot all Polygons and all MultiPolygon components in the same collection
     polys = expl_series[poly_idx]
     if not polys.empty:
         # color overrides both face and edgecolor. As we want people to be
         # able to use edgecolor as well, pass color to facecolor
         facecolor = style_kwds.pop("facecolor", None)
+        color_ = expl_color[poly_idx] if color_given else color
         if color is not None:
-            facecolor = color
+            facecolor = color_
 
         values_ = values[poly_idx] if cmap else None
         _plot_polygon_collection(
             ax, polys, values_, facecolor=facecolor, cmap=cmap, **style_kwds
         )
 
     # plot all LineStrings and MultiLineString components in same collection
     lines = expl_series[line_idx]
     if not lines.empty:
         values_ = values[line_idx] if cmap else None
+        color_ = expl_color[line_idx] if color_given else color
+
         _plot_linestring_collection(
-            ax, lines, values_, color=color, cmap=cmap, **style_kwds
+            ax, lines, values_, color=color_, cmap=cmap, **style_kwds
         )
 
     # plot all Points in the same collection
     points = expl_series[point_idx]
     if not points.empty:
         values_ = values[point_idx] if cmap else None
+        color_ = expl_color[point_idx] if color_given else color
+
         _plot_point_collection(
-            ax, points, values_, color=color, cmap=cmap, **style_kwds
+            ax, points, values_, color=color_, cmap=cmap, **style_kwds
         )
 
-    plt.draw()
+    ax.figure.canvas.draw_idle()
     return ax
 
 
 def plot_dataframe(
     df,
     column=None,
     cmap=None,
@@ -501,31 +481,31 @@
     ----------
     column : str, np.array, pd.Series (default None)
         The name of the dataframe column, np.array, or pd.Series to be plotted.
         If np.array or pd.Series are used then it must have same length as
         dataframe. Values are used to color the plot. Ignored if `color` is
         also set.
     kind: str
-        The kind of plots to produce:
-         - 'geo': Map (default)
-         Pandas Kinds
-         - 'line' : line plot
-         - 'bar' : vertical bar plot
-         - 'barh' : horizontal bar plot
-         - 'hist' : histogram
-         - 'box' : BoxPlot
-         - 'kde' : Kernel Density Estimation plot
-         - 'density' : same as 'kde'
-         - 'area' : area plot
-         - 'pie' : pie plot
-         - 'scatter' : scatter plot
-         - 'hexbin' : hexbin plot.
+        The kind of plots to produce. The default is to create a map ("geo").
+        Other supported kinds of plots from pandas:
+
+        - 'line' : line plot
+        - 'bar' : vertical bar plot
+        - 'barh' : horizontal bar plot
+        - 'hist' : histogram
+        - 'box' : BoxPlot
+        - 'kde' : Kernel Density Estimation plot
+        - 'density' : same as 'kde'
+        - 'area' : area plot
+        - 'pie' : pie plot
+        - 'scatter' : scatter plot
+        - 'hexbin' : hexbin plot.
     cmap : str (default None)
         The name of a colormap recognized by matplotlib.
-    color : str (default None)
+    color : str, np.array, pd.Series (default None)
         If specified, all objects will be colored uniformly.
     ax : matplotlib.pyplot.Artist (default None)
         axes on which to draw the plot
     cax : matplotlib.pyplot Artist (default None)
         axes on which to draw the legend in case of color map.
     categorical : bool (default False)
         If False, cmap will reflect numerical values of the
@@ -556,16 +536,16 @@
         by markersize to set the size of markers. Otherwise can be a value
         to apply to all points, or a sequence of the same length as the
         number of points.
     figsize : tuple of integers (default None)
         Size of the resulting matplotlib.figure.Figure. If the argument
         axes is given explicitly, figsize is ignored.
     legend_kwds : dict (default None)
-        Keyword arguments to pass to matplotlib.pyplot.legend() or
-        matplotlib.pyplot.colorbar().
+        Keyword arguments to pass to :func:`matplotlib.pyplot.legend` or
+        :func:`matplotlib.pyplot.colorbar`.
         Additional accepted keywords when `scheme` is specified:
 
         fmt : string
             A formatting specification for the bin edges of the classes in the
             legend. For example, to have no decimals: ``{"fmt": "{:.0f}"}``.
         labels : list-like
             A list of legend labels to override the auto-generated labels.
@@ -599,51 +579,34 @@
 
     Returns
     -------
     ax : matplotlib axes instance
 
     Examples
     --------
-    >>> df = geopandas.read_file(geopandas.datasets.get_path("naturalearth_lowres"))
+    >>> import geodatasets
+    >>> df = geopandas.read_file(geodatasets.get_path("nybb"))
     >>> df.head()  # doctest: +SKIP
-        pop_est      continent                      name iso_a3  \
-gdp_md_est                                           geometry
-    0     920938        Oceania                      Fiji    FJI      8374.0  MULTIPOLY\
-GON (((180.00000 -16.06713, 180.00000...
-    1   53950935         Africa                  Tanzania    TZA    150600.0  POLYGON (\
-(33.90371 -0.95000, 34.07262 -1.05982...
-    2     603253         Africa                 W. Sahara    ESH       906.5  POLYGON (\
-(-8.66559 27.65643, -8.66512 27.58948...
-    3   35623680  North America                    Canada    CAN   1674000.0  MULTIPOLY\
-GON (((-122.84000 49.00000, -122.9742...
-    4  326625791  North America  United States of America    USA  18560000.0  MULTIPOLY\
-GON (((-122.84000 49.00000, -120.0000...
+       BoroCode  ...                                           geometry
+    0         5  ...  MULTIPOLYGON (((970217.022 145643.332, 970227....
+    1         4  ...  MULTIPOLYGON (((1029606.077 156073.814, 102957...
+    2         3  ...  MULTIPOLYGON (((1021176.479 151374.797, 102100...
+    3         1  ...  MULTIPOLYGON (((981219.056 188655.316, 980940....
+    4         2  ...  MULTIPOLYGON (((1012821.806 229228.265, 101278...
 
-    >>> df.plot("pop_est", cmap="Blues")  # doctest: +SKIP
+    >>> df.plot("BoroName", cmap="Set1")  # doctest: +SKIP
 
     See the User Guide page :doc:`../../user_guide/mapping` for details.
 
     """
-    if "colormap" in style_kwds:
-        warnings.warn(
-            "'colormap' is deprecated, please use 'cmap' instead "
-            "(for consistency with matplotlib)",
-            FutureWarning,
-        )
-        cmap = style_kwds.pop("colormap")
-    if "axes" in style_kwds:
-        warnings.warn(
-            "'axes' is deprecated, please use 'ax' instead "
-            "(for consistency with pandas)",
-            FutureWarning,
-        )
-        ax = style_kwds.pop("axes")
     if column is not None and color is not None:
         warnings.warn(
-            "Only specify one of 'column' or 'color'. Using 'color'.", UserWarning
+            "Only specify one of 'column' or 'color'. Using 'color'.",
+            UserWarning,
+            stacklevel=3,
         )
         column = None
 
     try:
         import matplotlib.pyplot as plt
     except ImportError:
         raise ImportError(
@@ -675,14 +638,15 @@
         legend_kwds = legend_kwds.copy()
 
     if df.empty:
         warnings.warn(
             "The GeoDataFrame you are attempting to plot is "
             "empty. Nothing has been displayed.",
             UserWarning,
+            stacklevel=3,
         )
         return ax
 
     if isinstance(markersize, str):
         markersize = df[markersize].values
 
     if column is None:
@@ -708,94 +672,122 @@
 
             # Make sure index of a Series matches index of df
             if isinstance(values, pd.Series):
                 values = values.reindex(df.index)
     else:
         values = df[column]
 
-    if pd.api.types.is_categorical_dtype(values.dtype):
+    if isinstance(values.dtype, CategoricalDtype):
         if categories is not None:
             raise ValueError(
                 "Cannot specify 'categories' when column has categorical dtype"
             )
         categorical = True
-    elif values.dtype is np.dtype("O") or categories:
+    elif (
+        pd.api.types.is_object_dtype(values.dtype)
+        or pd.api.types.is_bool_dtype(values.dtype)
+        or pd.api.types.is_string_dtype(values.dtype)
+        or categories
+    ):
         categorical = True
 
     nan_idx = np.asarray(pd.isna(values), dtype="bool")
 
-    # Define `values` as a Series
-    if categorical:
-        if cmap is None:
-            cmap = "tab10"
+    if scheme is not None:
+        mc_err = (
+            "The 'mapclassify' package (>= 2.4.0) is "
+            "required to use the 'scheme' keyword."
+        )
+        try:
+            import mapclassify
 
-        cat = pd.Categorical(values, categories=categories)
-        categories = list(cat.categories)
+        except ImportError:
+            raise ImportError(mc_err)
 
-        # values missing in the Categorical but not in original values
-        missing = list(np.unique(values[~nan_idx & cat.isna()]))
-        if missing:
-            raise ValueError(
-                "Column contains values not listed in categories. "
-                "Missing categories: {}.".format(missing)
-            )
+        if Version(mapclassify.__version__) < Version("2.4.0"):
+            raise ImportError(mc_err)
 
-        values = cat.codes[~nan_idx]
-        vmin = 0 if vmin is None else vmin
-        vmax = len(categories) - 1 if vmax is None else vmax
-
-    if scheme is not None:
         if classification_kwds is None:
             classification_kwds = {}
         if "k" not in classification_kwds:
             classification_kwds["k"] = k
 
-        binning = _mapclassify_choro(values[~nan_idx], scheme, **classification_kwds)
+        binning = mapclassify.classify(
+            np.asarray(values[~nan_idx]), scheme, **classification_kwds
+        )
         # set categorical to True for creating the legend
         categorical = True
         if legend_kwds is not None and "labels" in legend_kwds:
             if len(legend_kwds["labels"]) != binning.k:
                 raise ValueError(
                     "Number of labels must match number of bins, "
                     "received {} labels for {} bins".format(
                         len(legend_kwds["labels"]), binning.k
                     )
                 )
             else:
-                categories = list(legend_kwds.pop("labels"))
+                labels = list(legend_kwds.pop("labels"))
         else:
             fmt = "{:.2f}"
             if legend_kwds is not None and "fmt" in legend_kwds:
                 fmt = legend_kwds.pop("fmt")
 
-            categories = binning.get_legend_classes(fmt)
+            labels = binning.get_legend_classes(fmt)
             if legend_kwds is not None:
                 show_interval = legend_kwds.pop("interval", False)
             else:
                 show_interval = False
             if not show_interval:
-                categories = [c[1:-1] for c in categories]
-        values = np.array(binning.yb)
+                labels = [c[1:-1] for c in labels]
+
+        values = pd.Categorical(
+            [np.nan] * len(values), categories=binning.bins, ordered=True
+        )
+        values[~nan_idx] = pd.Categorical.from_codes(
+            binning.yb, categories=binning.bins, ordered=True
+        )
+        if cmap is None:
+            cmap = "viridis"
+
+    # Define `values` as a Series
+    if categorical:
+        if cmap is None:
+            cmap = "tab10"
+
+        cat = pd.Categorical(values, categories=categories)
+        categories = list(cat.categories)
+
+        # values missing in the Categorical but not in original values
+        missing = list(np.unique(values[~nan_idx & cat.isna()]))
+        if missing:
+            raise ValueError(
+                "Column contains values not listed in categories. "
+                "Missing categories: {}.".format(missing)
+            )
+
+        values = cat.codes[~nan_idx]
+        vmin = 0 if vmin is None else vmin
+        vmax = len(categories) - 1 if vmax is None else vmax
 
     # fill values with placeholder where were NaNs originally to map them properly
     # (after removing them in categorical or scheme)
     if categorical:
         for n in np.where(nan_idx)[0]:
             values = np.insert(values, n, values[0])
 
     mn = values[~np.isnan(values)].min() if vmin is None else vmin
     mx = values[~np.isnan(values)].max() if vmax is None else vmax
 
     # decompose GeometryCollections
-    geoms, multiindex = _flatten_multi_geoms(df.geometry, prefix="Geom")
+    geoms, multiindex = _sanitize_geoms(df.geometry, prefix="Geom")
     values = np.take(values, multiindex, axis=0)
     nan_idx = np.take(nan_idx, multiindex, axis=0)
     expl_series = geopandas.GeoSeries(geoms)
 
-    geom_types = expl_series.type
+    geom_types = expl_series.geom_type
     poly_idx = np.asarray((geom_types == "Polygon") | (geom_types == "MultiPolygon"))
     line_idx = np.asarray(
         (geom_types == "LineString")
         | (geom_types == "MultiLineString")
         | (geom_types == "LinearRing")
     )
     point_idx = np.asarray((geom_types == "Point") | (geom_types == "MultiPoint"))
@@ -830,55 +822,57 @@
             vmin=mn,
             vmax=mx,
             markersize=markersize,
             cmap=cmap,
             **style_kwds,
         )
 
-    if missing_kwds is not None and not expl_series[nan_idx].empty:
+    missing_data = not expl_series[nan_idx].empty
+    if missing_kwds is not None and missing_data:
         if color:
             if "color" not in missing_kwds:
                 missing_kwds["color"] = color
 
         merged_kwds = style_kwds.copy()
         merged_kwds.update(missing_kwds)
 
         plot_series(expl_series[nan_idx], ax=ax, **merged_kwds)
 
     if legend and not color:
-
         if legend_kwds is None:
             legend_kwds = {}
         if "fmt" in legend_kwds:
             legend_kwds.pop("fmt")
 
         from matplotlib.lines import Line2D
         from matplotlib.colors import Normalize
         from matplotlib import cm
 
         norm = style_kwds.get("norm", None)
         if not norm:
             norm = Normalize(vmin=mn, vmax=mx)
         n_cmap = cm.ScalarMappable(norm=norm, cmap=cmap)
         if categorical:
+            if scheme is not None:
+                categories = labels
             patches = []
             for value, cat in enumerate(categories):
                 patches.append(
                     Line2D(
                         [0],
                         [0],
                         linestyle="none",
                         marker="o",
                         alpha=style_kwds.get("alpha", 1),
                         markersize=10,
                         markerfacecolor=n_cmap.to_rgba(value),
                         markeredgewidth=0,
                     )
                 )
-            if missing_kwds is not None:
+            if missing_kwds is not None and missing_data:
                 if "color" in merged_kwds:
                     merged_kwds["facecolor"] = merged_kwds["color"]
                 patches.append(
                     Line2D(
                         [0],
                         [0],
                         linestyle="none",
@@ -891,141 +885,41 @@
                             "linewidth", 1 if merged_kwds.get("edgecolor", False) else 0
                         ),
                     )
                 )
                 categories.append(merged_kwds.get("label", "NaN"))
             legend_kwds.setdefault("numpoints", 1)
             legend_kwds.setdefault("loc", "best")
-            ax.legend(patches, categories, **legend_kwds)
+            legend_kwds.setdefault("handles", patches)
+            legend_kwds.setdefault("labels", categories)
+            ax.legend(**legend_kwds)
         else:
-
             if cax is not None:
                 legend_kwds.setdefault("cax", cax)
             else:
                 legend_kwds.setdefault("ax", ax)
 
-            n_cmap.set_array([])
+            n_cmap.set_array(np.array([]))
             ax.get_figure().colorbar(n_cmap, **legend_kwds)
 
-    plt.draw()
+    ax.figure.canvas.draw_idle()
     return ax
 
 
-if geopandas._compat.PANDAS_GE_025:
-    from pandas.plotting import PlotAccessor
-
-    class GeoplotAccessor(PlotAccessor):
-
-        __doc__ = plot_dataframe.__doc__
-        _pandas_kinds = PlotAccessor._all_kinds
-
-        def __call__(self, *args, **kwargs):
-            data = self._parent.copy()
-            kind = kwargs.pop("kind", "geo")
-            if kind == "geo":
-                return plot_dataframe(data, *args, **kwargs)
-            if kind in self._pandas_kinds:
-                # Access pandas plots
-                return PlotAccessor(data)(kind=kind, **kwargs)
-            else:
-                # raise error
-                raise ValueError(f"{kind} is not a valid plot kind")
-
-        def geo(self, *args, **kwargs):
-            return self(kind="geo", *args, **kwargs)
-
-
-def _mapclassify_choro(values, scheme, **classification_kwds):
-    """
-    Wrapper for choropleth schemes from mapclassify for use with plot_dataframe
-
-    Parameters
-    ----------
-    values
-        Series to be plotted
-    scheme : str
-        One of mapclassify classification schemes
-        Options are BoxPlot, EqualInterval, FisherJenks,
-        FisherJenksSampled, HeadTailBreaks, JenksCaspall,
-        JenksCaspallForced, JenksCaspallSampled, MaxP,
-        MaximumBreaks, NaturalBreaks, Quantiles, Percentiles, StdMean,
-        UserDefined
-
-    **classification_kwds : dict
-        Keyword arguments for classification scheme
-        For details see mapclassify documentation:
-        https://pysal.org/mapclassify/api.html
-
-    Returns
-    -------
-    binning
-        Binning objects that holds the Series with values replaced with
-        class identifier and the bins.
-    """
-    try:
-        import mapclassify.classifiers as classifiers
-
-    except ImportError:
-        raise ImportError(
-            "The 'mapclassify' >= 2.2.0 package is required to use the 'scheme' keyword"
-        )
-    from mapclassify import __version__ as mc_version
-
-    if mc_version < LooseVersion("2.2.0"):
-        raise ImportError(
-            "The 'mapclassify' >= 2.2.0 package is required to "
-            "use the 'scheme' keyword"
-        )
-    schemes = {}
-    for classifier in classifiers.CLASSIFIERS:
-        schemes[classifier.lower()] = getattr(classifiers, classifier)
-
-    scheme = scheme.lower()
-
-    # mapclassify < 2.1 cleaned up the scheme names (removing underscores)
-    # trying both to keep compatibility with older versions and provide
-    # compatibility with newer versions of mapclassify
-    oldnew = {
-        "Box_Plot": "BoxPlot",
-        "Equal_Interval": "EqualInterval",
-        "Fisher_Jenks": "FisherJenks",
-        "Fisher_Jenks_Sampled": "FisherJenksSampled",
-        "HeadTail_Breaks": "HeadTailBreaks",
-        "Jenks_Caspall": "JenksCaspall",
-        "Jenks_Caspall_Forced": "JenksCaspallForced",
-        "Jenks_Caspall_Sampled": "JenksCaspallSampled",
-        "Max_P_Plassifier": "MaxP",
-        "Maximum_Breaks": "MaximumBreaks",
-        "Natural_Breaks": "NaturalBreaks",
-        "Std_Mean": "StdMean",
-        "User_Defined": "UserDefined",
-    }
-    scheme_names_mapping = {}
-    scheme_names_mapping.update(
-        {old.lower(): new.lower() for old, new in oldnew.items()}
-    )
-    scheme_names_mapping.update(
-        {new.lower(): old.lower() for old, new in oldnew.items()}
-    )
-
-    try:
-        scheme_class = schemes[scheme]
-    except KeyError:
-        scheme = scheme_names_mapping.get(scheme, scheme)
-        try:
-            scheme_class = schemes[scheme]
-        except KeyError:
-            raise ValueError(
-                "Invalid scheme. Scheme must be in the set: %r" % schemes.keys()
-            )
-
-    if classification_kwds["k"] is not None:
-        from inspect import getfullargspec as getspec
+@doc(plot_dataframe)
+class GeoplotAccessor(PlotAccessor):
+    _pandas_kinds = PlotAccessor._all_kinds
+
+    def __call__(self, *args, **kwargs):
+        data = self._parent.copy()
+        kind = kwargs.pop("kind", "geo")
+        if kind == "geo":
+            return plot_dataframe(data, *args, **kwargs)
+        if kind in self._pandas_kinds:
+            # Access pandas plots
+            return PlotAccessor(data)(kind=kind, **kwargs)
+        else:
+            # raise error
+            raise ValueError(f"{kind} is not a valid plot kind")
 
-        spec = getspec(scheme_class.__init__)
-        if "k" not in spec.args:
-            del classification_kwds["k"]
-    try:
-        binning = scheme_class(np.asarray(values), **classification_kwds)
-    except TypeError:
-        raise TypeError("Invalid keyword argument for %r " % scheme)
-    return binning
+    def geo(self, *args, **kwargs):
+        return self(kind="geo", *args, **kwargs)  # noqa: B026
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_api.py` & `geopandas-1.0.0a1/geopandas/tests/test_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 import subprocess
 import sys
 
-from geopandas._compat import PANDAS_GE_10
-
 
 def test_no_additional_imports():
     # test that 'import geopandas' does not import any of the optional or
     # development dependencies
     blacklist = {
         "pytest",
         "py",
         "ipython",
         # fiona actually gets imported if installed (but error suppressed until used)
         # "fiona",
         # "matplotlib",  # matplotlib gets imported by pandas, see below
         "mapclassify",
-        # 'rtree',  # rtree actually gets imported if installed
         "sqlalchemy",
+        "psycopg",
         "psycopg2",
         "geopy",
         "geoalchemy2",
+        "matplotlib",
     }
-    if PANDAS_GE_10:
-        # pandas > 0.25 stopped importing matplotlib by default
-        blacklist.add("matplotlib")
 
     code = """
 import sys
 import geopandas
 blacklist = {0!r}
 
 mods = blacklist & set(m.split('.')[0] for m in sys.modules)
 if mods:
     sys.stderr.write('err: geopandas should not import: {{}}'.format(', '.join(mods)))
     sys.exit(len(mods))
 """.format(
         blacklist
     )
     call = [sys.executable, "-c", code]
-    returncode = subprocess.run(call).returncode
+    returncode = subprocess.run(call, check=False).returncode
     assert returncode == 0
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_array.py` & `geopandas-1.0.0a1/geopandas/tests/test_array.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import random
+import warnings
 
 import numpy as np
 import pandas as pd
-import six
 
-from pyproj import CRS
 import shapely
 import shapely.affinity
 import shapely.geometry
 from shapely.geometry.base import CAP_STYLE, JOIN_STYLE
 import shapely.wkb
-from shapely._buildcfg import geos_version
+import shapely.wkt
+from shapely import geos_version
 
 import geopandas
 from geopandas.array import (
     GeometryArray,
     from_shapely,
     from_wkb,
     from_wkt,
     points_from_xy,
     to_wkb,
     to_wkt,
     _check_crs,
     _crs_mismatch_warn,
 )
-import geopandas._compat as compat
+
+from geopandas._compat import HAS_PYPROJ
 
 import pytest
 
 triangle_no_missing = [
     shapely.geometry.Polygon([(random.random(), random.random()) for i in range(3)])
     for _ in range(10)
 ]
-triangles = triangle_no_missing + [shapely.geometry.Polygon(), None]
+triangles = triangle_no_missing + [shapely.wkt.loads("POLYGON EMPTY"), None]
 T = from_shapely(triangles)
 
 points_no_missing = [
     shapely.geometry.Point(random.random(), random.random()) for _ in range(20)
 ]
 points = points_no_missing + [None]
 P = from_shapely(points)
@@ -135,32 +136,56 @@
 
     # array
     res = from_wkb(np.array(L_wkb, dtype=object))
     assert isinstance(res, GeometryArray)
     assert all(v.equals(t) for v, t in zip(res, points_no_missing))
 
     # missing values
-    # TODO(pygeos) does not support empty strings
-    if compat.USE_PYGEOS:
-        L_wkb.extend([None])
-    else:
-        L_wkb.extend([b"", None])
-    res = from_wkb(L_wkb)
-    assert res[-1] is None
-    if not compat.USE_PYGEOS:
-        assert res[-2] is None
+    # TODO(shapely) does not support empty strings, np.nan, or pd.NA
+    missing_values = [None]
+
+    res = from_wkb(missing_values)
+    np.testing.assert_array_equal(res, np.full(len(missing_values), None))
 
     # single MultiPolygon
     multi_poly = shapely.geometry.MultiPolygon(
         [shapely.geometry.box(0, 0, 1, 1), shapely.geometry.box(3, 3, 4, 4)]
     )
     res = from_wkb([multi_poly.wkb])
     assert res[0] == multi_poly
 
 
+def test_from_wkb_hex():
+    geometry_hex = ["0101000000CDCCCCCCCCCC1440CDCCCCCCCC0C4A40"]
+    res = from_wkb(geometry_hex)
+    assert isinstance(res, GeometryArray)
+
+    # array
+    res = from_wkb(np.array(geometry_hex, dtype=object))
+    assert isinstance(res, GeometryArray)
+
+
+def test_from_wkb_on_invalid():
+    # Single point LineString hex WKB: invalid
+    invalid_wkb_hex = "01020000000100000000000000000008400000000000000840"
+    message = "point array must contain 0 or >1 elements"
+
+    with pytest.raises(Exception, match=message):
+        from_wkb([invalid_wkb_hex], on_invalid="raise")
+
+    with pytest.warns(Warning, match=message):
+        res = from_wkb([invalid_wkb_hex], on_invalid="warn")
+    assert res == [None]
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        res = from_wkb([invalid_wkb_hex], on_invalid="ignore")
+    assert res == [None]
+
+
 def test_to_wkb():
     P = from_shapely(points_no_missing)
     res = to_wkb(P)
     exp = np.array([p.wkb for p in points_no_missing], dtype=object)
     assert isinstance(res, np.ndarray)
     np.testing.assert_array_equal(res, exp)
 
@@ -174,69 +199,87 @@
     res = to_wkb(a)
     assert res[0] is None
 
 
 @pytest.mark.parametrize("string_type", ["str", "bytes"])
 def test_from_wkt(string_type):
     if string_type == "str":
-        f = six.text_type
+        f = str
     else:
-        if six.PY3:
 
-            def f(x):
-                return bytes(x, "utf8")
-
-        else:
-
-            def f(x):
-                return x
+        def f(x):
+            return bytes(x, "utf8")
 
     # list
     L_wkt = [f(p.wkt) for p in points_no_missing]
     res = from_wkt(L_wkt)
     assert isinstance(res, GeometryArray)
-    assert all(v.almost_equals(t) for v, t in zip(res, points_no_missing))
+    tol = 0.5 * 10 ** (-6)
+    assert all(v.equals_exact(t, tolerance=tol) for v, t in zip(res, points_no_missing))
+    assert all(v.equals_exact(t, tolerance=tol) for v, t in zip(res, points_no_missing))
 
     # array
     res = from_wkt(np.array(L_wkt, dtype=object))
     assert isinstance(res, GeometryArray)
-    assert all(v.almost_equals(t) for v, t in zip(res, points_no_missing))
+    assert all(v.equals_exact(t, tolerance=tol) for v, t in zip(res, points_no_missing))
 
     # missing values
-    # TODO(pygeos) does not support empty strings
-    if compat.USE_PYGEOS:
-        L_wkt.extend([None])
-    else:
-        L_wkt.extend([f(""), None])
-    res = from_wkt(L_wkt)
-    assert res[-1] is None
-    if not compat.USE_PYGEOS:
-        assert res[-2] is None
+    # TODO(shapely) does not support empty strings, np.nan, or pd.NA
+    missing_values = [None]
+
+    res = from_wkt(missing_values)
+    np.testing.assert_array_equal(res, np.full(len(missing_values), None))
 
     # single MultiPolygon
     multi_poly = shapely.geometry.MultiPolygon(
         [shapely.geometry.box(0, 0, 1, 1), shapely.geometry.box(3, 3, 4, 4)]
     )
     res = from_wkt([f(multi_poly.wkt)])
     assert res[0] == multi_poly
 
 
+def test_from_wkt_on_invalid():
+    # Single point LineString WKT: invalid
+    invalid_wkt = "LINESTRING(0 0)"
+    message = "point array must contain 0 or >1 elements"
+
+    with pytest.raises(Exception, match=message):
+        from_wkt([invalid_wkt], on_invalid="raise")
+
+    with pytest.warns(Warning, match=message):
+        res = from_wkt([invalid_wkt], on_invalid="warn")
+    assert res == [None]
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        res = from_wkt([invalid_wkt], on_invalid="ignore")
+    assert res == [None]
+
+
 def test_to_wkt():
     P = from_shapely(points_no_missing)
     res = to_wkt(P, rounding_precision=-1)
     exp = np.array([p.wkt for p in points_no_missing], dtype=object)
     assert isinstance(res, np.ndarray)
     np.testing.assert_array_equal(res, exp)
 
     # missing values
     a = from_shapely([None, points_no_missing[0]])
     res = to_wkt(a)
     assert res[0] is None
 
 
+def test_as_array():
+    arr = from_shapely(points_no_missing)
+    np_arr1 = np.asarray(arr)
+    np_arr2 = arr.to_numpy()
+    assert np_arr1[0] == arr[0]
+    np.testing.assert_array_equal(np_arr1, np_arr2)
+
+
 @pytest.mark.parametrize(
     "attr,args",
     [
         ("contains", ()),
         ("covers", ()),
         ("crosses", ()),
         ("disjoint", ()),
@@ -245,29 +288,34 @@
         ("overlaps", ()),
         ("touches", ()),
         ("within", ()),
         ("geom_equals_exact", (0.1,)),
         ("geom_almost_equals", (3,)),
     ],
 )
+# filters required for attr=geom_almost_equals only
+@pytest.mark.filterwarnings(r"ignore:The \'geom_almost_equals\(\)\' method is deprecat")
+@pytest.mark.filterwarnings(r"ignore:The \'almost_equals\(\)\' method is deprecated")
 def test_predicates_vector_scalar(attr, args):
     na_value = False
 
     point = points[0]
     tri = triangles[0]
 
     for other in [point, tri, shapely.geometry.Polygon()]:
         result = getattr(T, attr)(other, *args)
         assert isinstance(result, np.ndarray)
         assert result.dtype == bool
 
         expected = [
-            getattr(tri, attr if "geom" not in attr else attr[5:])(other, *args)
-            if tri is not None
-            else na_value
+            (
+                getattr(tri, attr if "geom" not in attr else attr[5:])(other, *args)
+                if tri is not None
+                else na_value
+            )
             for tri in triangles
         ]
 
         assert result.tolist() == expected
 
     # TODO other is missing
 
@@ -284,14 +332,17 @@
         ("overlaps", ()),
         ("touches", ()),
         ("within", ()),
         ("geom_equals_exact", (0.1,)),
         ("geom_almost_equals", (3,)),
     ],
 )
+# filters required for attr=geom_almost_equals only
+@pytest.mark.filterwarnings(r"ignore:The \'geom_almost_equals\(\)\' method is deprecat")
+@pytest.mark.filterwarnings(r"ignore:The \'almost_equals\(\)\' method is deprecated")
 def test_predicates_vector_vector(attr, args):
     na_value = False
     empty_value = True if attr == "disjoint" else False
 
     A = (
         [shapely.geometry.Polygon(), None]
         + [
@@ -325,65 +376,29 @@
                 getattr(a, attr if "geom" not in attr else attr[5:])(b, *args)
             )
 
     assert result.tolist() == expected
 
 
 @pytest.mark.parametrize(
-    "attr,args", [("equals_exact", (0.1,)), ("almost_equals", (3,))]
-)
-def test_equals_deprecation(attr, args):
-    point = points[0]
-    tri = triangles[0]
-
-    for other in [point, tri, shapely.geometry.Polygon()]:
-        with pytest.warns(FutureWarning):
-            result = getattr(T, attr)(other, *args)
-        assert result.tolist() == getattr(T, "geom_" + attr)(other, *args).tolist()
-
-
-@pytest.mark.parametrize(
     "attr",
     [
         "boundary",
         "centroid",
         "convex_hull",
         "envelope",
         "exterior",
         # 'interiors',
     ],
 )
 def test_unary_geo(attr):
     na_value = None
 
-    if attr == "boundary":
-        # pygeos returns None for empty geometries
-        if not compat.USE_PYGEOS:
-            # boundary raises for empty geometry
-            with pytest.raises(Exception):
-                T.boundary
-
-        values = triangle_no_missing + [None]
-        A = from_shapely(values)
-    else:
-        values = triangles
-        A = T
-
-    result = getattr(A, attr)
-    if attr == "exterior" and compat.USE_PYGEOS:
-        # TODO(pygeos)
-        # empty Polygon() has an exterior with shapely > 1.7, which gives
-        # empty LinearRing instead of None,
-        # but conversion to pygeos still results in empty GeometryCollection
-        expected = [
-            getattr(t, attr) if t is not None and not t.is_empty else na_value
-            for t in values
-        ]
-    else:
-        expected = [getattr(t, attr) if t is not None else na_value for t in values]
+    result = getattr(T, attr)
+    expected = [getattr(t, attr) if t is not None else na_value for t in triangles]
 
     assert equal_geometries(result, expected)
 
 
 @pytest.mark.parametrize("attr", ["representative_point"])
 def test_unary_geo_callable(attr):
     na_value = None
@@ -441,62 +456,60 @@
             getattr(t, attr)(other) if t is not None else na_value for t in triangles
         ]
 
     assert equal_geometries(result, expected)
 
 
 @pytest.mark.parametrize(
-    "attr", ["is_closed", "is_valid", "is_empty", "is_simple", "has_z", "is_ring"]
+    "attr",
+    [
+        "is_closed",
+        "is_valid",
+        "is_empty",
+        "is_simple",
+        "has_z",
+        # for is_ring we raise a warning about the value for Polygon changing
+        "is_ring",
+    ],
 )
 def test_unary_predicates(attr):
     na_value = False
-    if attr == "is_simple" and geos_version < (3, 8) and not compat.USE_PYGEOS:
+    if attr == "is_simple" and geos_version < (3, 8):
         # poly.is_simple raises an error for empty polygon for GEOS < 3.8
-        with pytest.raises(Exception):
+        with pytest.raises(Exception):  # noqa: B017
             T.is_simple
         vals = triangle_no_missing
         V = from_shapely(vals)
     else:
         vals = triangles
         V = T
 
     result = getattr(V, attr)
 
-    if attr == "is_simple" and (geos_version < (3, 8) or compat.USE_PYGEOS):
-        # poly.is_simple raises an error for empty polygon for GEOS < 3.8
-        # with shapely, pygeos always returns False for all GEOS versions
-        # But even for Shapely with GEOS >= 3.8, empty GeometryCollection
-        # returns True instead of False
-        expected = [
-            getattr(t, attr) if t is not None and not t.is_empty else na_value
-            for t in vals
-        ]
-    elif attr == "is_ring":
+    if attr == "is_ring":
         expected = [
-            getattr(t.exterior, attr)
-            if t is not None and t.exterior is not None
-            else na_value
+            getattr(t, attr) if t is not None and t.exterior is not None else na_value
             for t in vals
         ]
     else:
         expected = [getattr(t, attr) if t is not None else na_value for t in vals]
+
     assert result.tolist() == expected
 
 
 def test_is_ring():
     g = [
         shapely.geometry.LinearRing([(0, 0), (1, 1), (1, -1)]),
         shapely.geometry.LineString([(0, 0), (1, 1), (1, -1)]),
         shapely.geometry.LineString([(0, 0), (1, 1), (1, -1), (0, 0)]),
         shapely.geometry.Polygon([(0, 0), (1, 1), (1, -1)]),
-        shapely.geometry.Polygon(),
+        shapely.wkt.loads("POLYGON EMPTY"),
         None,
     ]
-    expected = [True, False, True, True, False, False]
-
+    expected = [True, False, True, False, False, False]
     result = from_shapely(g).is_ring
 
     assert result.tolist() == expected
 
 
 @pytest.mark.parametrize("attr", ["area", "length"])
 def test_unary_float(attr):
@@ -507,15 +520,15 @@
     expected = [getattr(t, attr) if t is not None else na_value for t in triangles]
     np.testing.assert_allclose(result, expected)
 
 
 def test_geom_types():
     cat = T.geom_type
     # empty polygon has GeometryCollection type
-    assert list(cat) == ["Polygon"] * (len(T) - 2) + ["GeometryCollection", None]
+    assert list(cat) == ["Polygon"] * (len(T) - 1) + [None]
 
 
 def test_geom_types_null_mixed():
     geoms = [
         shapely.geometry.Polygon([(0, 0), (0, 1), (1, 1)]),
         None,
         shapely.geometry.Point(0, 1),
@@ -531,17 +544,19 @@
     attr = "distance"
     na_value = np.nan
     # also use nan for empty
 
     # vector - vector
     result = P[: len(T)].distance(T[::-1])
     expected = [
-        getattr(p, attr)(t)
-        if not ((t is None or t.is_empty) or (p is None or p.is_empty))
-        else na_value
+        (
+            getattr(p, attr)(t)
+            if not ((t is None or t.is_empty) or (p is None or p.is_empty))
+            else na_value
+        )
         for t, p in zip(triangles[::-1], points)
     ]
     np.testing.assert_allclose(result, expected)
 
     # vector - scalar
     p = points[0]
     result = T.distance(p)
@@ -590,36 +605,37 @@
         ]
         + [None]
     )
     L = from_shapely(lines)
 
     result = L.project(P, normalized=normalized)
     expected = [
-        l.project(p, normalized=normalized)
-        if l is not None and p is not None
-        else na_value
-        for p, l in zip(points, lines)
+        (
+            line.project(p, normalized=normalized)
+            if line is not None and p is not None
+            else na_value
+        )
+        for p, line in zip(points, lines)
     ]
     np.testing.assert_allclose(result, expected)
 
 
 @pytest.mark.parametrize("cap_style", [CAP_STYLE.round, CAP_STYLE.square])
 @pytest.mark.parametrize("join_style", [JOIN_STYLE.round, JOIN_STYLE.bevel])
 @pytest.mark.parametrize("resolution", [16, 25])
 def test_buffer(resolution, cap_style, join_style):
-    if compat.USE_PYGEOS:
-        # TODO(pygeos) need to further investigate why this test fails
-        if cap_style == 1 and join_style == 3:
-            pytest.skip("failing TODO")
-
     na_value = None
     expected = [
-        p.buffer(0.1, resolution=resolution, cap_style=cap_style, join_style=join_style)
-        if p is not None
-        else na_value
+        (
+            p.buffer(
+                0.1, resolution=resolution, cap_style=cap_style, join_style=join_style
+            )
+            if p is not None
+            else na_value
+        )
         for p in points
     ]
     result = P.buffer(
         0.1, resolution=resolution, cap_style=cap_style, join_style=join_style
     )
     assert equal_geometries(expected, result)
 
@@ -646,15 +662,29 @@
 
 def test_unary_union():
     geoms = [
         shapely.geometry.Polygon([(0, 0), (0, 1), (1, 1)]),
         shapely.geometry.Polygon([(0, 0), (1, 0), (1, 1)]),
     ]
     G = from_shapely(geoms)
-    u = G.unary_union()
+    with pytest.warns(FutureWarning, match="The 'unary_union' attribute is deprecated"):
+        u = G.unary_union()
+
+    expected = shapely.geometry.Polygon([(0, 0), (1, 0), (1, 1), (0, 1)])
+    assert u.equals(expected)
+    assert u.equals(G.union_all())
+
+
+def test_union_all():
+    geoms = [
+        shapely.geometry.Polygon([(0, 0), (0, 1), (1, 1)]),
+        shapely.geometry.Polygon([(0, 0), (1, 0), (1, 1)]),
+    ]
+    G = from_shapely(geoms)
+    u = G.union_all()
 
     expected = shapely.geometry.Polygon([(0, 0), (1, 0), (1, 1), (0, 1)])
     assert u.equals(expected)
 
 
 @pytest.mark.parametrize(
     "attr, arg",
@@ -755,14 +785,37 @@
     assert [p.x for p in P4] == [1, 3, 5, 7, 9]
 
     P5 = P[1]
     assert isinstance(P5, shapely.geometry.Point)
     assert P5.equals(points[1])
 
 
+@pytest.mark.parametrize(
+    "item",
+    [
+        geopandas.GeoDataFrame(
+            geometry=[shapely.geometry.Polygon([(0, 0), (2, 0), (2, 2), (0, 2)])]
+        ),
+        geopandas.GeoSeries(
+            [shapely.geometry.Polygon([(0, 0), (2, 0), (2, 2), (0, 2)])]
+        ),
+        np.array([shapely.geometry.Polygon([(0, 0), (2, 0), (2, 2), (0, 2)])]),
+        [shapely.geometry.Polygon([(0, 0), (2, 0), (2, 2), (0, 2)])],
+        shapely.geometry.Polygon([(0, 0), (2, 0), (2, 2), (0, 2)]),
+    ],
+)
+def test_setitem(item):
+    points = [shapely.geometry.Point(i, i) for i in range(10)]
+    P = from_shapely(points)
+
+    P[[0]] = item
+
+    assert isinstance(P[0], shapely.geometry.Polygon)
+
+
 def test_equality_ops():
     with pytest.raises(ValueError):
         P[:5] == P[:7]
 
     a1 = from_shapely([points[1], points[2], points[3]])
     a2 = from_shapely([points[1], points[0], points[3]])
 
@@ -780,15 +833,15 @@
 
     res = a3 == multi_poly
     assert res.tolist() == [False, False, False, True]
 
 
 def test_dir():
     assert "contains" in dir(P)
-    assert "data" in dir(P)
+    assert "to_numpy" in dir(P)
 
 
 def test_chaining():
     # contains will give False for empty / missing
     T = from_shapely(triangle_no_missing)
     assert T.contains(T.centroid).all()
 
@@ -841,22 +894,24 @@
 
     # astype(np_dtype) honors the dtype
     result = arr.astype(np.dtype("U10"))
     assert result.dtype == np.dtype("U10")
     assert result[0] == multi_poly.wkt[:10]
 
 
+@pytest.mark.skipif(not HAS_PYPROJ, reason="pyproj not installed")
 def test_check_crs():
     t1 = T.copy()
     t1.crs = 4326
     assert _check_crs(t1, T) is False
     assert _check_crs(t1, t1) is True
     assert _check_crs(t1, T, allow_none=True) is True
 
 
+@pytest.mark.skipif(not HAS_PYPROJ, reason="pyproj not installed")
 def test_crs_mismatch_warn():
     t1 = T.copy()
     t2 = T.copy()
     t1.crs = 4326
     t2.crs = 3857
 
     # two different CRS
@@ -868,71 +923,106 @@
         _crs_mismatch_warn(T, t2)
 
     # right None
     with pytest.warns(UserWarning, match="CRS mismatch between the CRS"):
         _crs_mismatch_warn(t1, T)
 
 
+@pytest.mark.skipif(HAS_PYPROJ, reason="pyproj installed")
+def test_missing_pyproj():
+    with pytest.warns(UserWarning, match="Cannot set the CRS, falling back to None"):
+        t = T.copy()
+        t.crs = 4326
+    assert t.crs is None
+
+
 @pytest.mark.parametrize("NA", [None, np.nan])
 def test_isna(NA):
     t1 = T.copy()
     t1[0] = NA
     assert t1[0] is None
 
 
-@pytest.mark.skipif(not compat.PANDAS_GE_10, reason="pd.NA introduced in pandas 1.0")
 def test_isna_pdNA():
     t1 = T.copy()
     t1[0] = pd.NA
     assert t1[0] is None
 
 
 def test_shift_has_crs():
     t = T.copy()
     t.crs = 4326
     assert t.shift(1).crs == t.crs
     assert t.shift(0).crs == t.crs
     assert t.shift(-1).crs == t.crs
 
 
-@pytest.mark.skipif(
-    not compat.PANDAS_GE_115, reason="crs only preserved in unique after pandas 1.1.5"
-)
 def test_unique_has_crs():
     t = T.copy()
     t.crs = 4326
     assert t.unique().crs == t.crs
 
 
+@pytest.mark.skipif(HAS_PYPROJ, reason="pyproj installed")
+def test_to_crs_pyproj_error():
+    t = T.copy()
+    t.crs = 4326
+    with pytest.raises(
+        ImportError, match="The 'pyproj' package is required for to_crs"
+    ):
+        t.to_crs(3857)
+
+
+@pytest.mark.skipif(HAS_PYPROJ, reason="pyproj installed")
+def test_estimate_utm_crs_pyproj_error():
+    with pytest.raises(
+        ImportError, match="The 'pyproj' package is required for estimate_utm_crs"
+    ):
+        T.estimate_utm_crs()
+
+
 class TestEstimateUtmCrs:
     def setup_method(self):
         self.esb = shapely.geometry.Point(-73.9847, 40.7484)
         self.sol = shapely.geometry.Point(-74.0446, 40.6893)
         self.landmarks = from_shapely([self.esb, self.sol], crs="epsg:4326")
 
     def test_estimate_utm_crs__geographic(self):
-        if compat.PYPROJ_LT_3:
-            with pytest.raises(RuntimeError, match=r"pyproj 3\+ required"):
-                self.landmarks.estimate_utm_crs()
-        else:
-            assert self.landmarks.estimate_utm_crs() == CRS("EPSG:32618")
-            assert self.landmarks.estimate_utm_crs("NAD83") == CRS("EPSG:26918")
+        pyproj = pytest.importorskip("pyproj")
+
+        assert self.landmarks.estimate_utm_crs() == pyproj.CRS("EPSG:32618")
+        assert self.landmarks.estimate_utm_crs("NAD83") == pyproj.CRS("EPSG:26918")
 
-    @pytest.mark.skipif(compat.PYPROJ_LT_3, reason="requires pyproj 3 or higher")
     def test_estimate_utm_crs__projected(self):
-        assert self.landmarks.to_crs("EPSG:3857").estimate_utm_crs() == CRS(
+        pyproj = pytest.importorskip("pyproj")
+
+        assert self.landmarks.to_crs("EPSG:3857").estimate_utm_crs() == pyproj.CRS(
             "EPSG:32618"
         )
 
-    @pytest.mark.skipif(compat.PYPROJ_LT_3, reason="requires pyproj 3 or higher")
+    def test_estimate_utm_crs__antimeridian(self):
+        pyproj = pytest.importorskip("pyproj")
+
+        antimeridian = from_shapely(
+            [
+                shapely.geometry.Point(1722483.900174921, 5228058.6143420935),
+                shapely.geometry.Point(4624385.494808555, 8692574.544944234),
+            ],
+            crs="EPSG:3851",
+        )
+        assert antimeridian.estimate_utm_crs() == pyproj.CRS("EPSG:32760")
+
     def test_estimate_utm_crs__out_of_bounds(self):
+        pytest.importorskip("pyproj")
+
         with pytest.raises(RuntimeError, match="Unable to determine UTM CRS"):
             from_shapely(
                 [shapely.geometry.Polygon([(0, 90), (1, 90), (2, 90)])], crs="EPSG:4326"
             ).estimate_utm_crs()
 
-    @pytest.mark.skipif(compat.PYPROJ_LT_3, reason="requires pyproj 3 or higher")
     def test_estimate_utm_crs__missing_crs(self):
+        pytest.importorskip("pyproj")
+
         with pytest.raises(RuntimeError, match="crs must be set"):
             from_shapely(
                 [shapely.geometry.Polygon([(0, 90), (1, 90), (2, 90)])]
             ).estimate_utm_crs()
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_compat.py` & `geopandas-1.0.0a1/geopandas/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.9.0/geopandas/tests/test_config.py` & `geopandas-1.0.0a1/geopandas/tests/test_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import pytest
 
 
 def test_options():
     assert "display_precision: " in repr(geopandas.options)
 
-    assert dir(geopandas.options) == ["display_precision", "use_pygeos"]
+    assert set(dir(geopandas.options)) == {
+        "display_precision",
+        "use_pygeos",
+        "io_engine",
+    }
 
     with pytest.raises(AttributeError):
         geopandas.options.non_existing_option
 
     with pytest.raises(AttributeError):
         geopandas.options.non_existing_option = 10
 
@@ -23,7 +27,21 @@
     with pytest.raises(ValueError):
         geopandas.options.display_precision = "abc"
 
     with pytest.raises(ValueError):
         geopandas.options.display_precision = -1
 
     geopandas.options.display_precision = None
+
+
+def test_options_io_engine():
+    assert geopandas.options.io_engine is None
+    geopandas.options.io_engine = "pyogrio"
+    assert geopandas.options.io_engine == "pyogrio"
+
+    with pytest.raises(ValueError):
+        geopandas.options.io_engine = "abc"
+
+    with pytest.raises(ValueError):
+        geopandas.options.io_engine = -1
+
+    geopandas.options.io_engine = None
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_crs.py` & `geopandas-1.0.0a1/geopandas/tests/test_crs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-from distutils.version import LooseVersion
-import os
-
 import random
+import warnings
 
 import numpy as np
 import pandas as pd
-
+import pytest
 from shapely.geometry import Point, Polygon, LineString
-import pyproj
 
-from geopandas import GeoSeries, GeoDataFrame, points_from_xy, datasets, read_file
+from geopandas import GeoSeries, GeoDataFrame, points_from_xy, read_file
 from geopandas.array import from_shapely, from_wkb, from_wkt, GeometryArray
-
 from geopandas.testing import assert_geodataframe_equal
-import pytest
 
-
-# pyproj 2.3.1 fixed a segfault for the case working in an environment with
-# 'init' dicts (https://github.com/pyproj4/pyproj/issues/415)
-PYPROJ_LT_231 = LooseVersion(pyproj.__version__) < LooseVersion("2.3.1")
+pyproj = pytest.importorskip("pyproj")
 
 
 def _create_df(x, y=None, crs=None):
     y = y or x
     x = np.asarray(x)
     y = np.asarray(y)
 
@@ -54,14 +46,21 @@
     df = df_epsg26918()
     df.loc[3, "geometry"] = None
     lonlat = df.to_crs(epsg=4326)
     utm = lonlat.to_crs(epsg=26918)
     assert_geodataframe_equal(df, utm, check_less_precise=True)
 
 
+def test_to_crs_transform__empty_data():
+    df = df_epsg26918().iloc[:0]
+    lonlat = df.to_crs(epsg=4326)
+    utm = lonlat.to_crs(epsg=26918)
+    assert_geodataframe_equal(df, utm, check_less_precise=True)
+
+
 def test_to_crs_inplace():
     df = df_epsg26918()
     lonlat = df.to_crs(epsg=4326)
     df.to_crs(epsg=4326, inplace=True)
     assert_geodataframe_equal(df, lonlat, check_less_precise=True)
 
 
@@ -73,71 +72,96 @@
     lonlat = df.to_crs(epsg=4326)
     utm = lonlat.to_crs(epsg=26918)
     assert lonlat.geometry.name == "geom"
     assert utm.geometry.name == "geom"
     assert_geodataframe_equal(df, utm, check_less_precise=True)
 
 
+def test_to_crs_dimension_z():
+    # preserve z dimension
+    arr = points_from_xy([1, 2], [2, 3], [3, 4], crs=4326)
+    assert arr.has_z.all()
+    result = arr.to_crs(epsg=3857)
+    assert result.has_z.all()
+
+
+# pyproj + numpy 1.25 trigger warning for single-element array -> recommdation is to
+# ignore the warning for now (https://github.com/pyproj4/pyproj/issues/1307)
+@pytest.mark.filterwarnings("ignore:Conversion of an array with:DeprecationWarning")
+def test_to_crs_dimension_mixed():
+    s = GeoSeries([Point(1, 2), LineString([(1, 2, 3), (4, 5, 6)])], crs=2056)
+    result = s.to_crs(epsg=4326)
+    assert not result[0].is_empty
+    assert result.has_z.tolist() == [False, True]
+    roundtrip = result.to_crs(epsg=2056)
+    # TODO replace with assert_geoseries_equal once we expose tolerance keyword
+    # assert_geoseries_equal(roundtrip, s, check_less_precise=True)
+    for a, b in zip(roundtrip, s):
+        np.testing.assert_allclose(a.coords[:], b.coords[:], atol=0.01)
+
+
 # -----------------------------------------------------------------------------
 # Test different supported formats for CRS specification
 
 
 @pytest.fixture(
     params=[
         4326,
         "epsg:4326",
         pytest.param(
             {"init": "epsg:4326"},
-            marks=pytest.mark.skipif(PYPROJ_LT_231, reason="segfault"),
         ),
         "+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs",
         {"proj": "latlong", "ellps": "WGS84", "datum": "WGS84", "no_defs": True},
     ],
     ids=["epsg_number", "epsg_string", "epsg_dict", "proj4_string", "proj4_dict"],
 )
 def epsg4326(request):
     if isinstance(request.param, int):
-        return dict(epsg=request.param)
-    return dict(crs=request.param)
+        return {"epsg": request.param}
+    return {"crs": request.param}
 
 
 @pytest.fixture(
     params=[
         26918,
         "epsg:26918",
         pytest.param(
             {"init": "epsg:26918", "no_defs": True},
-            marks=pytest.mark.skipif(PYPROJ_LT_231, reason="segfault"),
         ),
         "+proj=utm +zone=18 +ellps=GRS80 +datum=NAD83 +units=m +no_defs ",
         {"proj": "utm", "zone": 18, "datum": "NAD83", "units": "m", "no_defs": True},
     ],
     ids=["epsg_number", "epsg_string", "epsg_dict", "proj4_string", "proj4_dict"],
 )
 def epsg26918(request):
     if isinstance(request.param, int):
-        return dict(epsg=request.param)
-    return dict(crs=request.param)
+        return {"epsg": request.param}
+    return {"crs": request.param}
 
 
 @pytest.mark.filterwarnings("ignore:'\\+init:DeprecationWarning")
 @pytest.mark.filterwarnings("ignore:'\\+init:FutureWarning")
 def test_transform2(epsg4326, epsg26918):
     # with PROJ >= 7, the transformation using EPSG code vs proj4 string is
     # slightly different due to use of grid files or not -> turn off network
     # to not use grid files at all for this test
-    os.environ["PROJ_NETWORK"] = "OFF"
+    pyproj.network.set_network_enabled(False)
+
     df = df_epsg26918()
     lonlat = df.to_crs(**epsg4326)
     utm = lonlat.to_crs(**epsg26918)
     # can't check for CRS equality, as the formats differ although representing
     # the same CRS
     assert_geodataframe_equal(df, utm, check_less_precise=True, check_crs=False)
 
 
+# pyproj + numpy 1.25 trigger warning for single-element array -> recommdation is to
+# ignore the warning for now (https://github.com/pyproj4/pyproj/issues/1307)
+@pytest.mark.filterwarnings("ignore:Conversion of an array with:DeprecationWarning")
 def test_crs_axis_order__always_xy():
     df = GeoDataFrame(geometry=[Point(-1683723, 6689139)], crs="epsg:26918")
     lonlat = df.to_crs("epsg:4326")
     test_lonlat = GeoDataFrame(
         geometry=[Point(-110.1399901, 55.1350011)], crs="epsg:4326"
     )
     assert_geodataframe_equal(lonlat, test_lonlat, check_less_precise=True)
@@ -196,84 +220,85 @@
         assert s.values.crs == self.osgb
 
         arr = from_shapely(self.geoms, crs=27700)
         s = GeoSeries(arr)
         assert s.crs == self.osgb
         assert s.values.crs == self.osgb
 
-        with pytest.warns(FutureWarning):
+        with pytest.raises(
+            ValueError,
+            match="CRS mismatch between CRS of the passed geometries and 'crs'",
+        ):
             s = GeoSeries(arr, crs=4326)
         assert s.crs == self.osgb
 
-    @pytest.mark.filterwarnings("ignore:Assigning CRS")
     def test_dataframe(self):
         arr = from_shapely(self.geoms, crs=27700)
         df = GeoDataFrame(geometry=arr)
         assert df.crs == self.osgb
         assert df.geometry.crs == self.osgb
         assert df.geometry.values.crs == self.osgb
 
         arr = from_shapely(self.geoms)
         s = GeoSeries(arr, crs=27700)
         df = GeoDataFrame(geometry=s)
         assert df.crs == self.osgb
         assert df.geometry.crs == self.osgb
         assert df.geometry.values.crs == self.osgb
 
-        # different passed CRS than array CRS is ignored
-        with pytest.warns(FutureWarning):
+        # different passed CRS than array CRS is now an error
+        match_str = "CRS mismatch between CRS of the passed geometries and 'crs'"
+        with pytest.raises(ValueError, match=match_str):
             df = GeoDataFrame(geometry=s, crs=4326)
-        assert df.crs == self.osgb
-        assert df.geometry.crs == self.osgb
-        assert df.geometry.values.crs == self.osgb
-        with pytest.warns(FutureWarning):
+        with pytest.raises(ValueError, match=match_str):
             GeoDataFrame(geometry=s, crs=4326)
-        with pytest.warns(FutureWarning):
+        with pytest.raises(ValueError, match=match_str):
             GeoDataFrame({"data": [1, 2], "geometry": s}, crs=4326)
-        with pytest.warns(FutureWarning):
+        with pytest.raises(ValueError, match=match_str):
             GeoDataFrame(df, crs=4326).crs
 
         # manually change CRS
         arr = from_shapely(self.geoms)
         s = GeoSeries(arr, crs=27700)
         df = GeoDataFrame(geometry=s)
         df.crs = 4326
         assert df.crs == self.wgs
         assert df.geometry.crs == self.wgs
         assert df.geometry.values.crs == self.wgs
 
-        df = GeoDataFrame(self.geoms, columns=["geom"], crs=27700)
-        assert df.crs == self.osgb
-        df = df.set_geometry("geom")
+        with pytest.raises(ValueError, match="Assigning CRS to a GeoDataFrame without"):
+            GeoDataFrame(self.geoms, columns=["geom"], crs=27700)
+        with pytest.raises(ValueError, match="Assigning CRS to a GeoDataFrame without"):
+            GeoDataFrame(crs=27700)
+
+        df = GeoDataFrame(self.geoms, columns=["geom"])
+        df = df.set_geometry("geom", crs=27700)
         assert df.crs == self.osgb
         assert df.geometry.crs == self.osgb
         assert df.geometry.values.crs == self.osgb
         assert df.geom.crs == self.osgb
         assert df.geom.values.crs == self.osgb
 
         df = GeoDataFrame(geometry=self.geoms, crs=27700)
         assert df.crs == self.osgb
         assert df.geometry.crs == self.osgb
         assert df.geometry.values.crs == self.osgb
 
-        df = GeoDataFrame(crs=27700)
-        df = df.set_geometry(self.geoms)
-        assert df.crs == self.osgb
-        assert df.geometry.crs == self.osgb
-        assert df.geometry.values.crs == self.osgb
-
         # new geometry with set CRS has priority over GDF CRS
-        df = GeoDataFrame(crs=27700)
+        df = GeoDataFrame(geometry=self.geoms, crs=27700)
         df = df.set_geometry(self.geoms, crs=4326)
         assert df.crs == self.wgs
         assert df.geometry.crs == self.wgs
         assert df.geometry.values.crs == self.wgs
 
+        arr = from_shapely(self.geoms)
+        s = GeoSeries(arr, crs=27700)
         df = GeoDataFrame()
         df = df.set_geometry(s)
+        assert df._geometry_column_name == "geometry"
         assert df.crs == self.osgb
         assert df.geometry.crs == self.osgb
         assert df.geometry.values.crs == self.osgb
 
         arr = from_shapely(self.geoms, crs=27700)
         df = GeoDataFrame()
         df = df.set_geometry(arr)
@@ -289,33 +314,124 @@
 
         arr = from_shapely(self.geoms, crs=4326)
         df = GeoDataFrame({"col1": [1, 2], "geometry": arr})
         assert df.crs == self.wgs
         assert df.geometry.crs == self.wgs
         assert df.geometry.values.crs == self.wgs
 
-        # geometry column without geometry
+        # geometry column name None on init
         df = GeoDataFrame({"geometry": [0, 1]})
-        df.crs = 27700
+        with pytest.raises(
+            ValueError,
+            match="Assigning CRS to a GeoDataFrame without a geometry",
+        ):
+            df.crs = 27700
+
+        # geometry column without geometry
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore", "Geometry column does not contain geometry", UserWarning
+            )
+            df = GeoDataFrame({"geometry": [Point(0, 1)]}).assign(geometry=[0])
+        with pytest.raises(
+            ValueError,
+            match="Assigning CRS to a GeoDataFrame without an active geometry",
+        ):
+            df.crs = 27700
+        with pytest.raises(
+            AttributeError,
+            match="The CRS attribute of a GeoDataFrame without an active",
+        ):
+            assert df.crs == self.osgb
+
+    def test_dataframe_getitem_without_geometry_column(self):
+        df = GeoDataFrame({"col": range(10)}, geometry=self.arr)
+        df["geom2"] = df.geometry.centroid
+        subset = df[["col", "geom2"]]
+        with pytest.raises(
+            AttributeError,
+            match="The CRS attribute of a GeoDataFrame without an active",
+        ):
+            assert subset.crs == self.osgb
+
+    def test_dataframe_setitem(self):
+        # new geometry CRS has priority over GDF CRS
+        arr = from_shapely(self.geoms)
+        s = GeoSeries(arr, crs=27700)
+        df = GeoDataFrame()
+        with pytest.warns(
+            FutureWarning, match="You are adding a column named 'geometry'"
+        ):
+            df["geometry"] = s
         assert df.crs == self.osgb
+        assert df.geometry.crs == self.osgb
+        assert df.geometry.values.crs == self.osgb
+
+        arr = from_shapely(self.geoms, crs=27700)
+        df = GeoDataFrame()
+        with pytest.warns(
+            FutureWarning, match="You are adding a column named 'geometry'"
+        ):
+            df["geometry"] = arr
+        assert df.crs == self.osgb
+        assert df.geometry.crs == self.osgb
+        assert df.geometry.values.crs == self.osgb
+
+        # test to_crs case (GH1960)
+        arr = from_shapely(self.geoms)
+        df = GeoDataFrame({"col1": [1, 2], "geometry": arr}, crs=4326)
+        df["geometry"] = df["geometry"].to_crs(27700)
+        assert df.crs == self.osgb
+        assert df.geometry.crs == self.osgb
+        assert df.geometry.values.crs == self.osgb
+
+        # test changing geometry crs not in the geometry column doesn't change the crs
+        arr = from_shapely(self.geoms)
+        df = GeoDataFrame(
+            {"col1": [1, 2], "geometry": arr, "other_geom": arr}, crs=4326
+        )
+        df["other_geom"] = from_shapely(self.geoms, crs=27700)
+        assert df.crs == self.wgs
+        assert df.geometry.crs == self.wgs
+        assert df["geometry"].crs == self.wgs
+        assert df["other_geom"].crs == self.osgb
+
+    def test_dataframe_setitem_without_geometry_column(self):
+        arr = from_shapely(self.geoms)
+        df = GeoDataFrame({"col1": [1, 2], "geometry": arr}, crs=4326)
+
+        # override geometry with non geometry
+        with pytest.warns(UserWarning):
+            df["geometry"] = 1
+
+        # assigning a list of geometry object doesn't have cached access to 4326
+        df["geometry"] = self.geoms
+        assert df.crs is None
 
     @pytest.mark.parametrize(
         "scalar", [None, Point(0, 0), LineString([(0, 0), (1, 1)])]
     )
     def test_scalar(self, scalar):
-        with pytest.warns(FutureWarning):
-            df = GeoDataFrame()
-            df.crs = 4326
-        df["geometry"] = scalar
+        df = GeoDataFrame()
+        with pytest.warns(
+            FutureWarning, match="You are adding a column named 'geometry'"
+        ):
+            df["geometry"] = scalar
+        df.crs = 4326
         assert df.crs == self.wgs
         assert df.geometry.crs == self.wgs
         assert df.geometry.values.crs == self.wgs
 
-    def test_read_file(self):
-        nybb_filename = datasets.get_path("nybb")
+    @pytest.mark.filterwarnings("ignore:Accessing CRS")
+    def test_crs_with_no_geom_fails(self):
+        with pytest.raises(ValueError, match="Assigning CRS to a GeoDataFrame without"):
+            df = GeoDataFrame()
+            df.crs = 4326
+
+    def test_read_file(self, nybb_filename):
         df = read_file(nybb_filename)
         assert df.crs == pyproj.CRS(2263)
         assert df.geometry.crs == pyproj.CRS(2263)
         assert df.geometry.values.crs == pyproj.CRS(2263)
 
     def test_multiple_geoms(self):
         arr = from_shapely(self.geoms, crs=27700)
@@ -536,35 +652,20 @@
         merged = df.merge(df2, left_index=True, right_index=True)
         assert merged.col1.values.crs == self.wgs
         assert merged.geometry.values.crs == self.osgb
         assert merged.col2.values.crs == self.wgs
         assert merged.geom.values.crs == self.osgb
         assert merged.crs == self.osgb
 
-    # CRS should be assigned to geometry
-    def test_deprecation(self):
-        with pytest.warns(FutureWarning):
-            df = GeoDataFrame([], crs=27700)
-
-        # https://github.com/geopandas/geopandas/issues/1548
-        # ensure we still have converted the crs value to a CRS object
-        assert isinstance(df.crs, pyproj.CRS)
-
-        with pytest.warns(FutureWarning):
-            df = GeoDataFrame([])
-            df.crs = 27700
-
-        assert isinstance(df.crs, pyproj.CRS)
-
     # make sure that geometry column from list has CRS (__setitem__)
     def test_setitem_geometry(self):
         arr = from_shapely(self.geoms, crs=27700)
         df = GeoDataFrame({"col1": [0, 1]}, geometry=arr)
 
-        df["geometry"] = [g for g in df.geometry]
+        df["geometry"] = list(df.geometry)
         assert df.geometry.values.crs == self.osgb
 
         df2 = GeoDataFrame({"col1": [0, 1]}, geometry=arr)
         df2["geometry"] = from_shapely(self.geoms, crs=4326)
         assert df2.geometry.values.crs == self.wgs
 
     def test_astype(self):
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_dissolve.py` & `geopandas-1.0.0a1/geopandas/tests/test_dissolve.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,41 @@
+import warnings
+
 import numpy as np
 import pandas as pd
 
 import geopandas
 from geopandas import GeoDataFrame, read_file
-from geopandas import _compat as compat
 
 from pandas.testing import assert_frame_equal
 import pytest
 
+from geopandas._compat import PANDAS_GE_15, PANDAS_GE_20, PANDAS_GE_30, HAS_PYPROJ
+from geopandas.testing import assert_geodataframe_equal, geom_almost_equals
+
 
 @pytest.fixture
-def nybb_polydf():
-    nybb_filename = geopandas.datasets.get_path("nybb")
+def nybb_polydf(nybb_filename):
     nybb_polydf = read_file(nybb_filename)
     nybb_polydf = nybb_polydf[["geometry", "BoroName", "BoroCode"]]
     nybb_polydf = nybb_polydf.rename(columns={"geometry": "myshapes"})
     nybb_polydf = nybb_polydf.set_geometry("myshapes")
     nybb_polydf["manhattan_bronx"] = 5
     nybb_polydf.loc[3:4, "manhattan_bronx"] = 6
+    nybb_polydf["BoroCode"] = nybb_polydf["BoroCode"].astype("int64")
     return nybb_polydf
 
 
 @pytest.fixture
 def merged_shapes(nybb_polydf):
     # Merged geometry
     manhattan_bronx = nybb_polydf.loc[3:4]
     others = nybb_polydf.loc[0:2]
 
-    collapsed = [others.geometry.unary_union, manhattan_bronx.geometry.unary_union]
+    collapsed = [others.geometry.union_all(), manhattan_bronx.geometry.union_all()]
     merged_shapes = GeoDataFrame(
         {"myshapes": collapsed},
         geometry="myshapes",
         index=pd.Index([5, 6], name="manhattan_bronx"),
         crs=nybb_polydf.crs,
     )
 
@@ -52,40 +56,82 @@
     test_mean["BoroCode"] = [4, 1.5]
     return test_mean
 
 
 def test_geom_dissolve(nybb_polydf, first):
     test = nybb_polydf.dissolve("manhattan_bronx")
     assert test.geometry.name == "myshapes"
-    assert test.geom_almost_equals(first).all()
+    assert geom_almost_equals(test, first)
 
 
+@pytest.mark.skipif(not HAS_PYPROJ, reason="pyproj not installed")
 def test_dissolve_retains_existing_crs(nybb_polydf):
     assert nybb_polydf.crs is not None
     test = nybb_polydf.dissolve("manhattan_bronx")
     assert test.crs is not None
 
 
 def test_dissolve_retains_nonexisting_crs(nybb_polydf):
     nybb_polydf.crs = None
     test = nybb_polydf.dissolve("manhattan_bronx")
     assert test.crs is None
 
 
-def first_dissolve(nybb_polydf, first):
+def test_first_dissolve(nybb_polydf, first):
     test = nybb_polydf.dissolve("manhattan_bronx")
     assert_frame_equal(first, test, check_column_type=False)
 
 
 def test_mean_dissolve(nybb_polydf, first, expected_mean):
-    test = nybb_polydf.dissolve("manhattan_bronx", aggfunc="mean")
-    assert_frame_equal(expected_mean, test, check_column_type=False)
+    if not PANDAS_GE_15:
+        test = nybb_polydf.dissolve("manhattan_bronx", aggfunc="mean")
+        test2 = nybb_polydf.dissolve("manhattan_bronx", aggfunc=np.mean)
+    elif PANDAS_GE_15 and not PANDAS_GE_20:
+        with pytest.warns(FutureWarning, match=".*used in dissolve is deprecated.*"):
+            test = nybb_polydf.dissolve("manhattan_bronx", aggfunc="mean")
+            test2 = nybb_polydf.dissolve("manhattan_bronx", aggfunc=np.mean)
+    else:  # pandas 2.0
+        test = nybb_polydf.dissolve(
+            "manhattan_bronx", aggfunc="mean", numeric_only=True
+        )
+        # for non pandas "mean", numeric only cannot be applied. Drop columns manually
+        test2 = nybb_polydf.drop(columns=["BoroName"]).dissolve(
+            "manhattan_bronx", aggfunc="mean"
+        )
 
-    test = nybb_polydf.dissolve("manhattan_bronx", aggfunc=np.mean)
     assert_frame_equal(expected_mean, test, check_column_type=False)
+    assert_frame_equal(expected_mean, test2, check_column_type=False)
+
+
+@pytest.mark.skipif(not PANDAS_GE_15 or PANDAS_GE_20, reason="warning for pandas 1.5.x")
+def test_mean_dissolve_warning_capture(nybb_polydf, first, expected_mean):
+    with pytest.warns(
+        FutureWarning,
+        match=".*used in dissolve is deprecated.*",
+    ):
+        nybb_polydf.dissolve("manhattan_bronx", aggfunc="mean")
+
+    # test no warning for aggfunc first which doesn't have numeric only semantics
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        nybb_polydf.dissolve("manhattan_bronx", aggfunc="first")
+
+
+def test_dissolve_emits_other_warnings(nybb_polydf):
+    # we only do something special for pandas 1.5.x, but expect this
+    # test to be true on any version
+    def sum_and_warn(group):
+        warnings.warn("foo")  # noqa: B028
+        if PANDAS_GE_20:
+            return group.sum(numeric_only=False)
+        else:
+            return group.sum()
+
+    with pytest.warns(UserWarning, match="foo"):
+        nybb_polydf.dissolve("manhattan_bronx", aggfunc=sum_and_warn)
 
 
 def test_multicolumn_dissolve(nybb_polydf, first):
     multi = nybb_polydf.copy()
     multi["dup_col"] = multi.manhattan_bronx
     multi_test = multi.dissolve(["manhattan_bronx", "dup_col"], aggfunc="first")
 
@@ -102,30 +148,30 @@
     assert_frame_equal(comparison, test, check_column_type=False)
 
 
 def test_dissolve_none(nybb_polydf):
     test = nybb_polydf.dissolve(by=None)
     expected = GeoDataFrame(
         {
-            nybb_polydf.geometry.name: [nybb_polydf.geometry.unary_union],
+            nybb_polydf.geometry.name: [nybb_polydf.geometry.union_all()],
             "BoroName": ["Staten Island"],
             "BoroCode": [5],
             "manhattan_bronx": [5],
         },
         geometry=nybb_polydf.geometry.name,
         crs=nybb_polydf.crs,
     )
     assert_frame_equal(expected, test, check_column_type=False)
 
 
 def test_dissolve_none_mean(nybb_polydf):
-    test = nybb_polydf.dissolve(aggfunc="mean")
+    test = nybb_polydf.dissolve(aggfunc="mean", numeric_only=True)
     expected = GeoDataFrame(
         {
-            nybb_polydf.geometry.name: [nybb_polydf.geometry.unary_union],
+            nybb_polydf.geometry.name: [nybb_polydf.geometry.union_all()],
             "BoroCode": [3.0],
             "manhattan_bronx": [5.4],
         },
         geometry=nybb_polydf.geometry.name,
         crs=nybb_polydf.crs,
     )
     assert_frame_equal(expected, test, check_column_type=False)
@@ -197,40 +243,37 @@
     ).set_index("a")
     expected_sorted = expected_unsorted.sort_index()
 
     assert_frame_equal(expected_sorted, gdf.dissolve("a"))
     assert_frame_equal(expected_unsorted, gdf.dissolve("a", sort=False))
 
 
-@pytest.mark.skipif(
-    not compat.PANDAS_GE_025,
-    reason="'observed' param behavior changed in pandas 0.25.0",
-)
 def test_dissolve_categorical():
     gdf = geopandas.GeoDataFrame(
         {
             "cat": pd.Categorical(["a", "a", "b", "b"]),
             "noncat": [1, 1, 1, 2],
             "to_agg": [1, 2, 3, 4],
             "geometry": geopandas.array.from_wkt(
                 ["POINT (0 0)", "POINT (1 1)", "POINT (2 2)", "POINT (3 3)"]
             ),
         }
     )
 
     # when observed=False we get an additional observation
     # that wasn't in the original data
+    none_val = "GEOMETRYCOLLECTION EMPTY" if PANDAS_GE_30 else None
     expected_gdf_observed_false = geopandas.GeoDataFrame(
         {
             "cat": pd.Categorical(["a", "a", "b", "b"]),
             "noncat": [1, 2, 1, 2],
             "geometry": geopandas.array.from_wkt(
                 [
                     "MULTIPOINT (0 0, 1 1)",
-                    None,
+                    none_val,
                     "POINT (2 2)",
                     "POINT (3 3)",
                 ]
             ),
             "to_agg": [1, None, 3, 4],
         }
     ).set_index(["cat", "noncat"])
@@ -249,17 +292,14 @@
 
     assert_frame_equal(expected_gdf_observed_false, gdf.dissolve(["cat", "noncat"]))
     assert_frame_equal(
         expected_gdf_observed_true, gdf.dissolve(["cat", "noncat"], observed=True)
     )
 
 
-@pytest.mark.skipif(
-    not compat.PANDAS_GE_11, reason="dropna groupby kwarg added in pandas 1.1.0"
-)
 def test_dissolve_dropna():
     gdf = geopandas.GeoDataFrame(
         {
             "a": [1, 1, None],
             "geometry": geopandas.array.from_wkt(
                 ["POINT (0 0)", "POINT (1 1)", "POINT (2 2)"]
             ),
@@ -281,23 +321,31 @@
         }
     ).set_index("a")
 
     assert_frame_equal(expected_with_na, gdf.dissolve("a", dropna=False))
     assert_frame_equal(expected_no_na, gdf.dissolve("a"))
 
 
-@pytest.mark.skipif(
-    compat.PANDAS_GE_11, reason="dropna warning is only emitted if pandas < 1.1.0"
-)
 def test_dissolve_dropna_warn(nybb_polydf):
     # No warning with default params
-    with pytest.warns(None) as record:
+    with warnings.catch_warnings(record=True) as record:
         nybb_polydf.dissolve()
 
     for r in record:
         assert "dropna kwarg is not supported" not in str(r.message)
 
-    # Warning is emitted with non-default dropna value
-    with pytest.warns(
-        UserWarning, match="dropna kwarg is not supported for pandas < 1.1.0"
-    ):
-        nybb_polydf.dissolve(dropna=False)
+
+def test_dissolve_multi_agg(nybb_polydf, merged_shapes):
+    merged_shapes[("BoroCode", "min")] = [3, 1]
+    merged_shapes[("BoroCode", "max")] = [5, 2]
+    merged_shapes[("BoroName", "count")] = [3, 2]
+
+    with warnings.catch_warnings(record=True) as record:
+        test = nybb_polydf.dissolve(
+            by="manhattan_bronx",
+            aggfunc={
+                "BoroCode": ["min", "max"],
+                "BoroName": "count",
+            },
+        )
+    assert_geodataframe_equal(test, merged_shapes)
+    assert len(record) == 0
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_extension_array.py` & `geopandas-1.0.0a1/geopandas/tests/test_extension_array.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,34 +9,38 @@
 minimal tweaks should be applied to get the tests passing (by overwriting a
 parent method).
 
 A set of fixtures are defined to provide data for the tests (the fixtures
 expected to be available to pytest by the inherited pandas tests).
 
 """
+
+import itertools
 import operator
 
 import numpy as np
-from numpy.testing import assert_array_equal
 import pandas as pd
+from pandas.testing import assert_series_equal, assert_frame_equal
 from pandas.tests.extension import base as extension_tests
 
 import shapely.geometry
+from shapely.geometry import Point
 
 from geopandas.array import GeometryArray, GeometryDtype, from_shapely
+from geopandas._compat import PANDAS_GE_15, PANDAS_GE_22
 
 import pytest
 
 # -----------------------------------------------------------------------------
 # Compat with extension tests in older pandas versions
 # -----------------------------------------------------------------------------
 
 
 not_yet_implemented = pytest.mark.skip(reason="Not yet implemented")
-no_sorting = pytest.mark.skip(reason="Sorting not supported")
+no_minmax = pytest.mark.skip(reason="Min/max not supported")
 
 
 # -----------------------------------------------------------------------------
 # Required fixtures
 # -----------------------------------------------------------------------------
 
 
@@ -110,25 +114,25 @@
 @pytest.fixture
 def data_for_sorting():
     """Length-3 array with a known sort order.
 
     This should be three items [B, C, A] with
     A < B < C
     """
-    raise NotImplementedError
+    return from_shapely([Point(0, 1), Point(1, 1), Point(0, 0)])
 
 
 @pytest.fixture
 def data_missing_for_sorting():
     """Length-3 array with a known sort order.
 
     This should be three items [B, NA, A] with
     A < B and NA missing.
     """
-    raise NotImplementedError
+    return from_shapely([Point(1, 2), None, Point(0, 0)])
 
 
 @pytest.fixture
 def na_cmp():
     """Binary operator for comparing NA values.
     Should return a function of two arguments that returns
     True if both arguments are (scalar) NA for your type.
@@ -225,14 +229,26 @@
 def as_array(request):
     """
     Boolean fixture to support ExtensionDtype _from_sequence method testing.
     """
     return request.param
 
 
+@pytest.fixture
+def invalid_scalar(data):
+    """
+    A scalar that *cannot* be held by this ExtensionArray.
+
+    The default should work for most subclasses, but is not guaranteed.
+
+    If the array can hold any item (i.e. object dtype), then use pytest.skip.
+    """
+    return object.__new__(object)
+
+
 # Fixtures defined in pandas/conftest.py that are also needed: defining them
 # here instead of importing for compatibility
 
 
 @pytest.fixture(
     params=["sum", "max", "min", "mean", "prod", "std", "var", "median", "kurt", "skew"]
 )
@@ -264,50 +280,45 @@
     * !=
     * <
     * <=
     """
     return request.param
 
 
+@pytest.fixture(params=[None, lambda x: x])
+def sort_by_key(request):
+    """
+    Simple fixture for testing keys in sorting methods.
+    Tests None (no key) and the identity key.
+    """
+    return request.param
+
+
 # -----------------------------------------------------------------------------
 # Inherited tests
 # -----------------------------------------------------------------------------
 
 
 class TestDtype(extension_tests.BaseDtypeTests):
-
     # additional tests
 
     def test_array_type_with_arg(self, data, dtype):
         assert dtype.construct_array_type() is GeometryArray
 
     def test_registry(self, data, dtype):
         s = pd.Series(np.asarray(data), dtype=object)
         result = s.astype("geometry")
         assert isinstance(result.array, GeometryArray)
         expected = pd.Series(data)
-        self.assert_series_equal(result, expected)
+        assert_series_equal(result, expected)
 
 
 class TestInterface(extension_tests.BaseInterfaceTests):
-    def test_array_interface(self, data):
-        # we are overriding this base test because the creation of `expected`
-        # potentionally doesn't work for shapely geometries
-        # TODO can be removed with Shapely 2.0
-        result = np.array(data)
-        assert result[0] == data[0]
-
-        result = np.array(data, dtype=object)
-        # expected = np.array(list(data), dtype=object)
-        expected = np.empty(len(data), dtype=object)
-        expected[:] = list(data)
-        assert_array_equal(result, expected)
-
     def test_contains(self, data, data_missing):
-        # overrided due to the inconsistency between
+        # overridden due to the inconsistency between
         # GeometryDtype.na_value = np.nan
         # and None being used as NA in array
 
         # ensure data without missing values
         data = data[~data.isna()]
 
         # first elements are non-missing
@@ -320,15 +331,82 @@
 
 
 class TestConstructors(extension_tests.BaseConstructorsTests):
     pass
 
 
 class TestReshaping(extension_tests.BaseReshapingTests):
-    pass
+
+    # NOTE: this test is copied from pandas/tests/extension/base/reshaping.py
+    # because starting with pandas 3.0 the assert_frame_equal is strict regarding
+    # the exact missing value (None vs NaN)
+    # Our `result` uses None, but the way the `expected` is created results in
+    # NaNs (and specifying to use None as fill value in unstack also does not
+    # help)
+    # -> the only change compared to the upstream test is marked
+    @pytest.mark.parametrize(
+        "index",
+        [
+            # Two levels, uniform.
+            pd.MultiIndex.from_product(([["A", "B"], ["a", "b"]]), names=["a", "b"]),
+            # non-uniform
+            pd.MultiIndex.from_tuples([("A", "a"), ("A", "b"), ("B", "b")]),
+            # three levels, non-uniform
+            pd.MultiIndex.from_product([("A", "B"), ("a", "b", "c"), (0, 1, 2)]),
+            pd.MultiIndex.from_tuples(
+                [
+                    ("A", "a", 1),
+                    ("A", "b", 0),
+                    ("A", "a", 0),
+                    ("B", "a", 0),
+                    ("B", "c", 1),
+                ]
+            ),
+        ],
+    )
+    @pytest.mark.parametrize("obj", ["series", "frame"])
+    def test_unstack(self, data, index, obj):
+        data = data[: len(index)]
+        if obj == "series":
+            ser = pd.Series(data, index=index)
+        else:
+            ser = pd.DataFrame({"A": data, "B": data}, index=index)
+
+        n = index.nlevels
+        levels = list(range(n))
+        # [0, 1, 2]
+        # [(0,), (1,), (2,), (0, 1), (0, 2), (1, 0), (1, 2), (2, 0), (2, 1)]
+        combinations = itertools.chain.from_iterable(
+            itertools.permutations(levels, i) for i in range(1, n)
+        )
+
+        for level in combinations:
+            result = ser.unstack(level=level)
+            assert all(
+                isinstance(result[col].array, type(data)) for col in result.columns
+            )
+
+            if obj == "series":
+                # We should get the same result with to_frame+unstack+droplevel
+                df = ser.to_frame()
+
+                alt = df.unstack(level=level).droplevel(0, axis=1)
+                assert_frame_equal(result, alt)
+
+            obj_ser = ser.astype(object)
+
+            expected = obj_ser.unstack(level=level, fill_value=data.dtype.na_value)
+            if obj == "series":
+                assert (expected.dtypes == object).all()
+            # <------------ next line is added
+            expected[expected.isna()] = None
+            # ------------->
+
+            result = result.astype(object)
+            assert_frame_equal(result, expected)
 
 
 class TestGetitem(extension_tests.BaseGetitemTests):
     pass
 
 
 class TestSetitem(extension_tests.BaseSetitemTests):
@@ -336,44 +414,81 @@
 
 
 class TestMissing(extension_tests.BaseMissingTests):
     def test_fillna_series(self, data_missing):
         fill_value = data_missing[1]
         ser = pd.Series(data_missing)
 
+        # Fill with a scalar
         result = ser.fillna(fill_value)
         expected = pd.Series(data_missing._from_sequence([fill_value, fill_value]))
-        self.assert_series_equal(result, expected)
+        assert_series_equal(result, expected)
 
-        # filling with array-like not yet supported
+        # Fill with a series
+        filler = pd.Series(
+            from_shapely(
+                [
+                    shapely.geometry.Point(1, 1),
+                    shapely.geometry.Point(2, 2),
+                ],
+            )
+        )
+        result = ser.fillna(filler)
+        expected = pd.Series(data_missing._from_sequence([fill_value, fill_value]))
+        assert_series_equal(result, expected)
 
-        # # Fill with a series
-        # result = ser.fillna(expected)
-        # self.assert_series_equal(result, expected)
+        # Fill with a series not affecting the missing values
+        filler = pd.Series(
+            from_shapely(
+                [
+                    shapely.geometry.Point(2, 2),
+                    shapely.geometry.Point(1, 1),
+                ]
+            ),
+            index=[10, 11],
+        )
+        result = ser.fillna(filler)
+        assert_series_equal(result, ser)
 
-        # # Fill with a series not affecting the missing values
-        # result = ser.fillna(ser)
-        # self.assert_series_equal(result, ser)
+        # More `GeoSeries.fillna` testcases are in
+        # `geopandas\tests\test_pandas_methods.py::test_fillna_scalar`
+        # and `geopandas\tests\test_pandas_methods.py::test_fillna_series`.
 
     @pytest.mark.skip("fillna method not supported")
     def test_fillna_limit_pad(self, data_missing):
         pass
 
     @pytest.mark.skip("fillna method not supported")
     def test_fillna_limit_backfill(self, data_missing):
         pass
 
     @pytest.mark.skip("fillna method not supported")
     def test_fillna_series_method(self, data_missing, method):
         pass
 
+    @pytest.mark.skip("fillna method not supported")
+    def test_fillna_no_op_returns_copy(self, data):
+        pass
+
+    @pytest.mark.skip("fillna method not supported")
+    def test_ffill_limit_area(
+        self, data_missing, limit_area, input_ilocs, expected_ilocs
+    ):
+        pass
+
+
+if PANDAS_GE_22:
+    from pandas.tests.extension.base import BaseReduceTests
+else:
+    from pandas.tests.extension.base import BaseNoReduceTests as BaseReduceTests
 
-class TestReduce(extension_tests.BaseNoReduceTests):
+
+class TestReduce(BaseReduceTests):
     @pytest.mark.skip("boolean reduce (any/all) tested in test_pandas_methods")
-    def test_reduce_series_boolean():
+    def test_reduce_series_boolean(self):
         pass
 
 
 _all_arithmetic_operators = [
     "__add__",
     "__radd__",
     # '__sub__', '__rsub__',
@@ -391,103 +506,77 @@
 
 
 @pytest.fixture(params=_all_arithmetic_operators)
 def all_arithmetic_operators(request):
     """
     Fixture for dunder names for common arithmetic operations
 
-    Adapted to excluse __sub__, as this is implemented as "difference".
+    Adapted to exclude __sub__, as this is implemented as "difference".
     """
     return request.param
 
 
+# an inherited test from pandas creates a Series from a list of geometries, which
+# triggers the warning from Shapely, out of control of GeoPandas, so ignoring here
+@pytest.mark.filterwarnings(
+    "ignore:The array interface is deprecated and will no longer work in Shapely 2.0"
+)
 class TestArithmeticOps(extension_tests.BaseArithmeticOpsTests):
     @pytest.mark.skip(reason="not applicable")
     def test_divmod_series_array(self, data, data_for_twos):
         pass
 
     @pytest.mark.skip(reason="not applicable")
     def test_add_series_with_extension_array(self, data):
         pass
 
 
+# an inherited test from pandas creates a Series from a list of geometries, which
+# triggers the warning from Shapely, out of control of GeoPandas, so ignoring here
+@pytest.mark.filterwarnings(
+    "ignore:The array interface is deprecated and will no longer work in Shapely 2.0"
+)
 class TestComparisonOps(extension_tests.BaseComparisonOpsTests):
     def _compare_other(self, s, data, op_name, other):
         op = getattr(operator, op_name.strip("_"))
         result = op(s, other)
         expected = s.combine(other, op)
-        self.assert_series_equal(result, expected)
+        assert_series_equal(result, expected)
 
-    def test_compare_scalar(self, data, all_compare_operators):  # noqa
+    def test_compare_scalar(self, data, all_compare_operators):
         op_name = all_compare_operators
         s = pd.Series(data)
         self._compare_other(s, data, op_name, data[0])
 
-    def test_compare_array(self, data, all_compare_operators):  # noqa
+    def test_compare_array(self, data, all_compare_operators):
         op_name = all_compare_operators
         s = pd.Series(data)
         other = pd.Series([data[0]] * len(data))
         self._compare_other(s, data, op_name, other)
 
 
 class TestMethods(extension_tests.BaseMethodsTests):
-    @not_yet_implemented
+    @pytest.mark.skipif(
+        not PANDAS_GE_15, reason="sorting index not yet working with older pandas"
+    )
     @pytest.mark.parametrize("dropna", [True, False])
     def test_value_counts(self, all_data, dropna):
         pass
 
-    @not_yet_implemented
+    @pytest.mark.skipif(
+        not PANDAS_GE_15, reason="sorting index not yet working with older pandas"
+    )
     def test_value_counts_with_normalize(self, data):
         pass
 
-    @no_sorting
-    def test_argsort(self, data_for_sorting):
-        result = pd.Series(data_for_sorting).argsort()
-        expected = pd.Series(np.array([2, 0, 1], dtype=np.int64))
-        self.assert_series_equal(result, expected)
-
-    @no_sorting
-    def test_argsort_missing(self, data_missing_for_sorting):
-        result = pd.Series(data_missing_for_sorting).argsort()
-        expected = pd.Series(np.array([1, -1, 0], dtype=np.int64))
-        self.assert_series_equal(result, expected)
-
-    @no_sorting
-    @pytest.mark.parametrize("ascending", [True, False])
-    def test_sort_values(self, data_for_sorting, ascending):
-        ser = pd.Series(data_for_sorting)
-        result = ser.sort_values(ascending=ascending)
-        expected = ser.iloc[[2, 0, 1]]
-        if not ascending:
-            expected = expected[::-1]
-
-        self.assert_series_equal(result, expected)
-
-    @no_sorting
-    @pytest.mark.parametrize("ascending", [True, False])
-    def test_sort_values_missing(self, data_missing_for_sorting, ascending):
-        ser = pd.Series(data_missing_for_sorting)
-        result = ser.sort_values(ascending=ascending)
-        if ascending:
-            expected = ser.iloc[[2, 0, 1]]
-        else:
-            expected = ser.iloc[[0, 2, 1]]
-        self.assert_series_equal(result, expected)
-
-    @no_sorting
     @pytest.mark.parametrize("ascending", [True, False])
     def test_sort_values_frame(self, data_for_sorting, ascending):
-        df = pd.DataFrame({"A": [1, 2, 1], "B": data_for_sorting})
-        result = df.sort_values(["A", "B"])
-        expected = pd.DataFrame(
-            {"A": [1, 1, 2], "B": data_for_sorting.take([2, 0, 1])}, index=[2, 0, 1]
-        )
-        self.assert_frame_equal(result, expected)
+        super().test_sort_values_frame(data_for_sorting, ascending)
 
-    @no_sorting
+    @pytest.mark.skip(reason="searchsorted not supported")
     def test_searchsorted(self, data_for_sorting, as_series):
         pass
 
     @not_yet_implemented
     def test_combine_le(self):
         pass
 
@@ -497,70 +586,59 @@
 
     @not_yet_implemented
     def test_fillna_length_mismatch(self, data_missing):
         msg = "Length of 'value' does not match."
         with pytest.raises(ValueError, match=msg):
             data_missing.fillna(data_missing.take([1]))
 
-    @no_sorting
-    def test_nargsort(self):
-        pass
-
-    @no_sorting
-    def test_argsort_missing_array(self):
-        pass
-
-    @no_sorting
+    @no_minmax
     def test_argmin_argmax(self):
         pass
 
-    @no_sorting
+    @no_minmax
     def test_argmin_argmax_empty_array(self):
         pass
 
-    @no_sorting
+    @no_minmax
     def test_argmin_argmax_all_na(self):
         pass
 
-    @no_sorting
+    @no_minmax
     def test_argreduce_series(self):
         pass
 
-    @no_sorting
+    @no_minmax
     def test_argmax_argmin_no_skipna_notimplemented(self):
         pass
 
 
 class TestCasting(extension_tests.BaseCastingTests):
     pass
 
 
 class TestGroupby(extension_tests.BaseGroupbyTests):
-    @no_sorting
     @pytest.mark.parametrize("as_index", [True, False])
     def test_groupby_extension_agg(self, as_index, data_for_grouping):
-        pass
+        super().test_groupby_extension_agg(as_index, data_for_grouping)
 
-    @no_sorting
     def test_groupby_extension_transform(self, data_for_grouping):
-        pass
+        super().test_groupby_extension_transform(data_for_grouping)
 
-    @no_sorting
     @pytest.mark.parametrize(
         "op",
         [
             lambda x: 1,
             lambda x: [1] * len(x),
             lambda x: pd.Series([1] * len(x)),
             lambda x: x,
         ],
         ids=["scalar", "list", "series", "object"],
     )
     def test_groupby_extension_apply(self, data_for_grouping, op):
-        pass
+        super().test_groupby_extension_apply(data_for_grouping, op)
 
 
 class TestPrinting(extension_tests.BasePrintingTests):
     pass
 
 
 @not_yet_implemented
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_geocode.py` & `geopandas-1.0.0a1/geopandas/tests/test_geocode.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,51 +7,53 @@
 from geopandas.tools.geocoding import _prepare_geocode_result
 
 from geopandas.tests.util import assert_geoseries_equal, mock
 from pandas.testing import assert_series_equal
 from geopandas.testing import assert_geodataframe_equal
 import pytest
 
+from geopandas._compat import HAS_PYPROJ
+
 geopy = pytest.importorskip("geopy")
 
 
 class ForwardMock(mock.MagicMock):
     """
     Mock the forward geocoding function.
     Returns the passed in address and (p, p+.5) where p increases
     at each call
 
     """
 
     def __init__(self, *args, **kwargs):
-        super(ForwardMock, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._n = 0.0
 
     def __call__(self, *args, **kwargs):
         self.return_value = args[0], (self._n, self._n + 0.5)
         self._n += 1
-        return super(ForwardMock, self).__call__(*args, **kwargs)
+        return super().__call__(*args, **kwargs)
 
 
 class ReverseMock(mock.MagicMock):
     """
     Mock the reverse geocoding function.
     Returns the passed in point and 'address{p}' where p increases
     at each call
 
     """
 
     def __init__(self, *args, **kwargs):
-        super(ReverseMock, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._n = 0
 
     def __call__(self, *args, **kwargs):
         self.return_value = "address{0}".format(self._n), args[0]
         self._n += 1
-        return super(ReverseMock, self).__call__(*args, **kwargs)
+        return super().__call__(*args, **kwargs)
 
 
 @pytest.fixture
 def locations():
     locations = ["260 Broadway, New York, NY", "77 Massachusetts Ave, Cambridge, MA"]
     return locations
 
@@ -67,15 +69,16 @@
     # loop
     p0 = Point(12.3, -45.6)  # Treat these as lat/lon
     p1 = Point(-23.4, 56.7)
     d = {"a": ("address0", p0.coords[0]), "b": ("address1", p1.coords[0])}
 
     df = _prepare_geocode_result(d)
     assert type(df) is GeoDataFrame
-    assert df.crs == "EPSG:4326"
+    if HAS_PYPROJ:
+        assert df.crs == "EPSG:4326"
     assert len(df) == 2
     assert "address" in df
 
     coords = df.loc["a"]["geometry"].coords[0]
     test = p0.coords[0]
     # Output from the df should be lon/lat
     assert coords[0] == pytest.approx(test[1])
@@ -89,33 +92,29 @@
 
 def test_prepare_result_none():
     p0 = Point(12.3, -45.6)  # Treat these as lat/lon
     d = {"a": ("address0", p0.coords[0]), "b": (None, None)}
 
     df = _prepare_geocode_result(d)
     assert type(df) is GeoDataFrame
-    assert df.crs == "EPSG:4326"
+    if HAS_PYPROJ:
+        assert df.crs == "EPSG:4326"
     assert len(df) == 2
     assert "address" in df
 
     row = df.loc["b"]
-    # The shapely.geometry.Point() is actually a GeometryCollection, and thus
-    # gets converted to that in conversion to pygeos. When converting back
-    # on access, you now get a GeometryCollection object instead of Point,
-    # which has no coords
-    # see https://github.com/Toblerity/Shapely/issues/742/#issuecomment-545296708
+
     # TODO we should probably replace this with a missing value instead of point?
-    # assert len(row["geometry"].coords) == 0
+    assert len(row["geometry"].coords) == 0
     assert row["geometry"].is_empty
     assert row["address"] is None
 
 
 @pytest.mark.parametrize("geocode_result", (None, (None, None)))
 def test_prepare_geocode_result_when_result_is(geocode_result):
-
     result = {0: geocode_result}
     expected_output = GeoDataFrame(
         {"geometry": [Point()], "address": [None]},
         crs="EPSG:4326",
     )
 
     output = _prepare_geocode_result(result)
@@ -130,39 +129,39 @@
         geocode(["cambridge, ma"], "badprovider")
 
 
 def test_bad_provider_reverse():
     from geopy.exc import GeocoderNotFound
 
     with pytest.raises(GeocoderNotFound):
-        reverse_geocode(["cambridge, ma"], "badprovider")
+        reverse_geocode([Point(0, 0)], "badprovider")
 
 
 def test_forward(locations, points):
-    from geopy.geocoders import GeocodeFarm
+    from geopy.geocoders import Photon
 
-    for provider in ["geocodefarm", GeocodeFarm]:
-        with mock.patch("geopy.geocoders.GeocodeFarm.geocode", ForwardMock()) as m:
+    for provider in ["photon", Photon]:
+        with mock.patch("geopy.geocoders.Photon.geocode", ForwardMock()) as m:
             g = geocode(locations, provider=provider, timeout=2)
             assert len(locations) == m.call_count
 
         n = len(locations)
         assert isinstance(g, GeoDataFrame)
         expected = GeoSeries(
             [Point(float(x) + 0.5, float(x)) for x in range(n)], crs="EPSG:4326"
         )
         assert_geoseries_equal(expected, g["geometry"])
         assert_series_equal(g["address"], pd.Series(locations, name="address"))
 
 
 def test_reverse(locations, points):
-    from geopy.geocoders import GeocodeFarm
+    from geopy.geocoders import Photon
 
-    for provider in ["geocodefarm", GeocodeFarm]:
-        with mock.patch("geopy.geocoders.GeocodeFarm.reverse", ReverseMock()) as m:
+    for provider in ["photon", Photon]:
+        with mock.patch("geopy.geocoders.Photon.reverse", ReverseMock()) as m:
             g = reverse_geocode(points, provider=provider, timeout=2)
             assert len(points) == m.call_count
 
         assert isinstance(g, GeoDataFrame)
 
         expected = GeoSeries(points, crs="EPSG:4326")
         assert_geoseries_equal(expected, g["geometry"])
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_geodataframe.py` & `geopandas-1.0.0a1/geopandas/tests/test_geodataframe.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,61 @@
 import json
 import os
 import shutil
 import tempfile
-from distutils.version import LooseVersion
 
 import numpy as np
 import pandas as pd
 
-import pyproj
-from pyproj import CRS
-from pyproj.exceptions import CRSError
-from shapely.geometry import Point
+from shapely.geometry import Point, Polygon, box
 
 import geopandas
-from geopandas import GeoDataFrame, GeoSeries, read_file
+from geopandas import GeoDataFrame, GeoSeries, points_from_xy, read_file
 from geopandas.array import GeometryArray, GeometryDtype, from_shapely
 
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 from geopandas.tests.util import PACKAGE_DIR, validate_boro_df
 from pandas.testing import assert_frame_equal, assert_index_equal, assert_series_equal
+import geopandas._compat as compat
 import pytest
 
 
-PYPROJ_LT_3 = LooseVersion(pyproj.__version__) < LooseVersion("3")
+@pytest.fixture
+def dfs(request):
+    s1 = GeoSeries(
+        [
+            Polygon([(0, 0), (2, 0), (2, 2), (0, 2)]),
+            Polygon([(2, 2), (4, 2), (4, 4), (2, 4)]),
+        ]
+    )
+    s2 = GeoSeries(
+        [
+            Polygon([(1, 1), (3, 1), (3, 3), (1, 3)]),
+            Polygon([(3, 3), (5, 3), (5, 5), (3, 5)]),
+        ]
+    )
+    df1 = GeoDataFrame({"col1": [1, 2], "geometry": s1})
+    df2 = GeoDataFrame({"col2": [1, 2], "geometry": s2})
+    return df1, df2
+
+
+@pytest.fixture(
+    params=["union", "intersection", "difference", "symmetric_difference", "identity"]
+)
+def how(request):
+    return request.param
 
 
+@pytest.mark.usefixtures("_setup_class_nybb_filename")
 class TestDataFrame:
     def setup_method(self):
         N = 10
-
-        nybb_filename = geopandas.datasets.get_path("nybb")
-        self.df = read_file(nybb_filename)
+        # self.nybb_filename attached via _setup_class_nybb_filename
+        self.df = read_file(self.nybb_filename)
+        # TODO re-write instance variables to be fixtures
         self.tempdir = tempfile.mkdtemp()
         self.crs = "epsg:4326"
         self.df2 = GeoDataFrame(
             [
                 {"geometry": Point(x, y), "value1": x + y, "value2": x * y}
                 for x, y in zip(range(N), range(N))
             ],
@@ -45,17 +66,21 @@
         )
 
     def teardown_method(self):
         shutil.rmtree(self.tempdir)
 
     def test_df_init(self):
         assert type(self.df2) is GeoDataFrame
-        assert self.df2.crs == self.crs
+        if compat.HAS_PYPROJ:
+            assert self.df2.crs == self.crs
 
+    @pytest.mark.skipif(not compat.HAS_PYPROJ, reason="Requires pyproj")
     def test_different_geo_colname(self):
+        from pyproj.exceptions import CRSError
+
         data = {
             "A": range(5),
             "B": range(-5, 0),
             "location": [Point(x, y) for x, y in zip(range(5), range(5))],
         }
         df = GeoDataFrame(data, crs=self.crs, geometry="location")
         locs = GeoSeries(data["location"], crs=self.crs)
@@ -168,18 +193,19 @@
         ]
         df.geometry = new_geom
 
         new_geom = GeoSeries(new_geom, index=df.index, crs=df.crs)
         assert_geoseries_equal(df.geometry, new_geom)
         assert_geoseries_equal(df["geometry"], new_geom)
 
-        # new crs
-        gs = new_geom.to_crs(crs="epsg:3857")
-        df.geometry = gs
-        assert df.crs == "epsg:3857"
+        if compat.HAS_PYPROJ:
+            # new crs
+            gs = new_geom.to_crs(crs="epsg:3857")
+            df.geometry = gs
+            assert df.crs == "epsg:3857"
 
     def test_geometry_property_errors(self):
         with pytest.raises(AttributeError):
             df = self.df.copy()
             del df["geometry"]
             df.geometry
 
@@ -236,14 +262,18 @@
         with pytest.raises(ValueError):
             self.df.set_geometry("nonexistent-column")
 
         # ndim error
         with pytest.raises(ValueError):
             self.df.set_geometry(self.df)
 
+    @pytest.mark.skipif(not compat.HAS_PYPROJ, reason="Requires pyproj")
+    def test_set_geometry_crs(self):
+        geom = GeoSeries([Point(x, y) for x, y in zip(range(5), range(5))])
+
         # new crs - setting should default to GeoSeries' crs
         gs = GeoSeries(geom, crs="epsg:3857")
         new_df = self.df.set_geometry(gs)
         assert new_df.crs == "epsg:3857"
 
         # explicit crs overrides self and dataframe
         new_df = self.df.set_geometry(gs, crs="epsg:26909")
@@ -300,33 +330,87 @@
 
     def test_set_geometry_empty(self):
         df = pd.DataFrame(columns=["a", "geometry"], index=pd.DatetimeIndex([]))
         result = df.set_geometry("geometry")
         assert isinstance(result, GeoDataFrame)
         assert isinstance(result.index, pd.DatetimeIndex)
 
+    def test_set_geometry_np_int(self):
+        self.df.loc[:, 0] = self.df.geometry
+        df = self.df.set_geometry(np.int64(0))
+        assert df.geometry.name == 0
+
+    def test_get_geometry_invalid(self):
+        df = GeoDataFrame()
+        # no column "geometry" ever added
+        df["geom"] = self.df.geometry
+        msg_geo_col_none = "active geometry column to use has not been set. "
+
+        with pytest.raises(AttributeError, match=msg_geo_col_none):
+            df.geometry
+        # "geometry" originally present but dropped (but still a gdf)
+        col_subset_drop_geometry = ["BoroCode", "BoroName", "geom2"]
+        df2 = self.df.copy().assign(geom2=self.df.geometry)[col_subset_drop_geometry]
+        with pytest.raises(AttributeError, match="is not present."):
+            df2.geometry
+
+        msg_other_geo_cols_present = "There are columns with geometry data type"
+        msg_no_other_geo_cols = "There are no existing columns with geometry data type"
+        with pytest.raises(AttributeError, match=msg_other_geo_cols_present):
+            df2.geometry
+
+        with pytest.raises(AttributeError, match=msg_no_other_geo_cols):
+            GeoDataFrame().geometry
+
+    def test_get_geometry_geometry_inactive(self):
+        # https://github.com/geopandas/geopandas/issues/2574
+        df = self.df.assign(geom2=self.df.geometry).set_geometry("geom2")
+        df = df.loc[:, ["BoroName", "geometry"]]
+        assert df._geometry_column_name == "geom2"
+        msg_geo_col_missing = "is not present. "
+        # Check that df.geometry raises if active geometry column is missing,
+        # it should not fall back to column named "geometry"
+        with pytest.raises(AttributeError, match=msg_geo_col_missing):
+            df.geometry
+
+    def test_active_geometry_name(self):
+        # default single active called "geometry"
+        assert self.df.active_geometry_name == "geometry"
+
+        # one GeoSeries, not active
+        no_active = GeoDataFrame({"foo": self.df.BoroName, "bar": self.df.geometry})
+        assert no_active.active_geometry_name is None
+        assert no_active.set_geometry("bar").active_geometry_name == "bar"
+
+        # multiple, none active
+        multiple = GeoDataFrame({"foo": self.df.geometry, "bar": self.df.geometry})
+        assert multiple.active_geometry_name is None
+        assert multiple.set_geometry("foo").active_geometry_name == "foo"
+        assert multiple.set_geometry("bar").active_geometry_name == "bar"
+
     def test_align(self):
         df = self.df2
 
         res1, res2 = df.align(df)
         assert_geodataframe_equal(res1, df)
         assert_geodataframe_equal(res2, df)
 
         res1, res2 = df.align(df.copy())
         assert_geodataframe_equal(res1, df)
         assert_geodataframe_equal(res2, df)
 
-        # assert crs is / is not preserved on mixed dataframes
-        df_nocrs = df.copy()
-        df_nocrs.crs = None
-        res1, res2 = df.align(df_nocrs)
-        assert_geodataframe_equal(res1, df)
-        assert res1.crs is not None
-        assert_geodataframe_equal(res2, df_nocrs)
-        assert res2.crs is None
+        if compat.HAS_PYPROJ:
+            # assert crs is / is not preserved on mixed dataframes
+            df_nocrs = df.copy()
+            df_nocrs.crs = None
+            res1, res2 = df.align(df_nocrs)
+            assert_geodataframe_equal(res1, df)
+            assert res1.crs is not None
+            assert_geodataframe_equal(res2, df_nocrs)
+            assert res2.crs is None
 
         # mixed GeoDataFrame / DataFrame
         df_nogeom = pd.DataFrame(df.drop("geometry", axis=1))
         res1, res2 = df.align(df_nogeom, axis=0)
         assert_geodataframe_equal(res1, df)
         assert type(res2) == pd.DataFrame
         assert_frame_equal(res2, df_nogeom)
@@ -339,38 +423,59 @@
         exp1.iloc[0] = np.nan
         exp2 = df.copy()
         exp2.iloc[-1] = np.nan
         res1, res2 = df1.align(df2)
         assert_geodataframe_equal(res1, exp1)
         assert_geodataframe_equal(res2, exp2)
 
-        df2_nocrs = df2.copy()
-        df2_nocrs.crs = None
-        exp2_nocrs = exp2.copy()
-        exp2_nocrs.crs = None
-        res1, res2 = df1.align(df2_nocrs)
-        assert_geodataframe_equal(res1, exp1)
-        assert res1.crs is not None
-        assert_geodataframe_equal(res2, exp2_nocrs)
-        assert res2.crs is None
+        if compat.HAS_PYPROJ:
+            df2_nocrs = df2.copy()
+            df2_nocrs.crs = None
+            exp2_nocrs = exp2.copy()
+            exp2_nocrs.crs = None
+            res1, res2 = df1.align(df2_nocrs)
+            assert_geodataframe_equal(res1, exp1)
+            assert res1.crs is not None
+            assert_geodataframe_equal(res2, exp2_nocrs)
+            assert res2.crs is None
 
         df2_nogeom = pd.DataFrame(df2.drop("geometry", axis=1))
         exp2_nogeom = pd.DataFrame(exp2.drop("geometry", axis=1))
         res1, res2 = df1.align(df2_nogeom, axis=0)
         assert_geodataframe_equal(res1, exp1)
         assert type(res2) == pd.DataFrame
         assert_frame_equal(res2, exp2_nogeom)
 
+    @pytest.mark.skipif(not compat.HAS_PYPROJ, reason="Requires pyproj")
     def test_to_json(self):
-        text = self.df.to_json()
+        text = self.df.to_json(to_wgs84=True)
         data = json.loads(text)
         assert data["type"] == "FeatureCollection"
         assert len(data["features"]) == 5
         assert "id" in data["features"][0].keys()
 
+        # check it converts to WGS84
+        coord = data["features"][0]["geometry"]["coordinates"][0][0][0]
+        np.testing.assert_allclose(coord, [-74.0505080640324, 40.5664220341941])
+
+    def test_to_json_wgs84_false(self):
+        text = self.df.to_json()
+        data = json.loads(text)
+        # check it doesn't convert to WGS84
+        coord = data["features"][0]["geometry"]["coordinates"][0][0][0]
+        assert coord == [970217.0223999023, 145643.33221435547]
+
+    def test_to_json_no_crs(self):
+        self.df.crs = None
+        with pytest.raises(ValueError, match="CRS is not set"):
+            self.df.to_json(to_wgs84=True)
+
+    @pytest.mark.filterwarnings(
+        "ignore:Geometry column does not contain geometry:UserWarning"
+    )
     def test_to_json_geom_col(self):
         df = self.df.copy()
         df["geom"] = df["geometry"]
         df["geometry"] = np.arange(len(df))
         df.set_geometry("geom", inplace=True)
 
         text = df.to_json()
@@ -453,41 +558,40 @@
     def test_to_json_drop_id_only_geom_column(self):
         text = self.df[["geometry"]].to_json(drop_id=True)
         data = json.loads(text)
         assert len(data["features"]) == 5
         for f in data["features"]:
             assert "id" not in f.keys()
 
+    def test_to_json_with_duplicate_columns(self):
+        df = GeoDataFrame(
+            data=[[1, 2, 3]], columns=["a", "b", "a"], geometry=[Point(1, 1)]
+        )
+        with pytest.raises(
+            ValueError, match="GeoDataFrame cannot contain duplicated column names."
+        ):
+            df.to_json()
+
     def test_copy(self):
         df2 = self.df.copy()
         assert type(df2) is GeoDataFrame
         assert self.df.crs == df2.crs
 
-    def test_to_file_crs(self):
-        """
-        Ensure that the file is written according to the crs
-        if it is specified
-
-        """
-        tempfilename = os.path.join(self.tempdir, "crs.shp")
-        # save correct CRS
-        self.df.to_file(tempfilename)
-        df = GeoDataFrame.from_file(tempfilename)
-        assert df.crs == self.df.crs
-        # overwrite CRS
-        self.df.to_file(tempfilename, crs=3857)
-        df = GeoDataFrame.from_file(tempfilename)
-        assert df.crs == "epsg:3857"
+    def test_empty_copy(self):
+        # https://github.com/geopandas/geopandas/issues/2765
+        df = GeoDataFrame()
+        df2 = df.copy()
+        assert type(df2) is GeoDataFrame
+        df3 = df.copy(deep=True)
+        assert type(df3) is GeoDataFrame
 
-        # specify CRS for gdf without one
-        df2 = self.df.copy()
-        df2.crs = None
-        df2.to_file(tempfilename, crs=2263)
-        df = GeoDataFrame.from_file(tempfilename)
-        assert df.crs == "epsg:2263"
+    def test_no_geom_copy(self):
+        df = GeoDataFrame(pd.DataFrame({"a": [1, 2, 3]}))
+        assert type(df) is GeoDataFrame
+        assert type(df.copy()) is GeoDataFrame
 
     def test_bool_index(self):
         # Find boros with 'B' in their name
         df = self.df[self.df["BoroName"].str.contains("B")]
         assert len(df) == 2
         boros = df["BoroName"].values
         assert "Brooklyn" in boros
@@ -500,31 +604,36 @@
         assert_frame_equal(self.df2.loc[5:], self.df2.cx[5:, :])
         assert_frame_equal(self.df2.loc[5:], self.df2.cx[:, 5:])
         assert_frame_equal(self.df2.loc[5:], self.df2.cx[5:, 5:])
 
     def test_from_dict(self):
         data = {"A": [1], "geometry": [Point(0.0, 0.0)]}
         df = GeoDataFrame.from_dict(data, crs=3857)
-        assert df.crs == "epsg:3857"
+        if compat.HAS_PYPROJ:
+            assert df.crs == "epsg:3857"
+        else:
+            assert df.crs is None
         assert df._geometry_column_name == "geometry"
 
         data = {"B": [1], "location": [Point(0.0, 0.0)]}
         df = GeoDataFrame.from_dict(data, geometry="location")
         assert df._geometry_column_name == "location"
 
-    def test_from_features(self):
+    def test_from_features(self, nybb_filename):
         fiona = pytest.importorskip("fiona")
-        nybb_filename = geopandas.datasets.get_path("nybb")
         with fiona.open(nybb_filename) as f:
             features = list(f)
             crs = f.crs_wkt
 
         df = GeoDataFrame.from_features(features, crs=crs)
         validate_boro_df(df, case_sensitive=True)
-        assert df.crs == crs
+        if compat.HAS_PYPROJ:
+            assert df.crs == crs
+        else:
+            assert df.crs is None
 
     def test_from_features_unaligned_properties(self):
         p1 = Point(1, 1)
         f1 = {
             "type": "Feature",
             "properties": {"a": 0},
             "geometry": p1.__geo_interface__,
@@ -536,26 +645,119 @@
             "properties": {"b": 1},
             "geometry": p2.__geo_interface__,
         }
 
         p3 = Point(3, 3)
         f3 = {
             "type": "Feature",
-            "properties": {"a": 2},
+            "properties": None,
             "geometry": p3.__geo_interface__,
         }
 
         df = GeoDataFrame.from_features([f1, f2, f3])
 
         result = df[["a", "b"]]
         expected = pd.DataFrame.from_dict(
-            [{"a": 0, "b": np.nan}, {"a": np.nan, "b": 1}, {"a": 2, "b": np.nan}]
+            [{"a": 0, "b": np.nan}, {"a": np.nan, "b": 1}, {"a": np.nan, "b": np.nan}]
         )
         assert_frame_equal(expected, result)
 
+    def test_from_features_empty_properties(self):
+        geojson_properties_object = """{
+          "type": "FeatureCollection",
+          "features": [
+            {
+              "type": "Feature",
+              "properties": {},
+              "geometry": {
+                "type": "Polygon",
+                "coordinates": [
+                  [
+                    [
+                      11.3456529378891,
+                      46.49461446367692
+                    ],
+                    [
+                      11.345674395561216,
+                      46.494097442978195
+                    ],
+                    [
+                      11.346918940544128,
+                      46.49385370294394
+                    ],
+                    [
+                      11.347616314888,
+                      46.4938352377453
+                    ],
+                    [
+                      11.347514390945435,
+                      46.49466985846028
+                    ],
+                    [
+                      11.3456529378891,
+                      46.49461446367692
+                    ]
+                  ]
+                ]
+              }
+            }
+          ]
+        }"""
+
+        geojson_properties_null = """{
+          "type": "FeatureCollection",
+          "features": [
+            {
+              "type": "Feature",
+              "properties": null,
+              "geometry": {
+                "type": "Polygon",
+                "coordinates": [
+                  [
+                    [
+                      11.3456529378891,
+                      46.49461446367692
+                    ],
+                    [
+                      11.345674395561216,
+                      46.494097442978195
+                    ],
+                    [
+                      11.346918940544128,
+                      46.49385370294394
+                    ],
+                    [
+                      11.347616314888,
+                      46.4938352377453
+                    ],
+                    [
+                      11.347514390945435,
+                      46.49466985846028
+                    ],
+                    [
+                      11.3456529378891,
+                      46.49461446367692
+                    ]
+                  ]
+                ]
+              }
+            }
+          ]
+        }"""
+
+        # geoJSON with empty properties
+        gjson_po = json.loads(geojson_properties_object)
+        gdf1 = GeoDataFrame.from_features(gjson_po)
+
+        # geoJSON with null properties
+        gjson_null = json.loads(geojson_properties_null)
+        gdf2 = GeoDataFrame.from_features(gjson_null)
+
+        assert_frame_equal(gdf1, gdf2)
+
     def test_from_features_geom_interface_feature(self):
         class Placemark(object):
             def __init__(self, geom, val):
                 self.__geo_interface__ = {
                     "type": "Feature",
                     "properties": {"a": val},
                     "geometry": geom.__geo_interface__,
@@ -576,15 +778,15 @@
             "lon": [-120, -121.2, -122.9],
         }
 
         df = pd.DataFrame(data)
         geometry = [Point(xy) for xy in zip(df["lon"], df["lat"])]
         gdf = GeoDataFrame(df, geometry=geometry)
         # from_features returns sorted columns
-        expected = gdf[["geometry", "lat", "lon", "name"]]
+        expected = gdf[["geometry", "name", "lat", "lon"]]
 
         # test FeatureCollection
         res = GeoDataFrame.from_features(gdf.__geo_interface__)
         assert_frame_equal(res, expected)
 
         # test list of Features
         res = GeoDataFrame.from_features(gdf.__geo_interface__["features"])
@@ -618,71 +820,124 @@
         df.loc[0, "A"] = 100
         assert gf.loc[0, "A"] == 0
         assert gf2.loc[0, "A"] == 0
 
         with pytest.raises(ValueError):
             df.set_geometry("location", inplace=True)
 
+    def test_dataframe_not_manipulated(self):
+        df = pd.DataFrame(
+            {
+                "A": range(len(self.df)),
+                "latitude": self.df.geometry.centroid.y,
+                "longitude": self.df.geometry.centroid.x,
+            },
+            index=self.df.index,
+        )
+        df_copy = df.copy()
+        gf = GeoDataFrame(
+            df,
+            geometry=points_from_xy(df["longitude"], df["latitude"]),
+            crs=self.df.crs,
+        )
+        assert type(df) == pd.DataFrame
+        assert "geometry" not in df
+        assert_frame_equal(df, df_copy)
+        assert isinstance(gf, GeoDataFrame)
+        assert hasattr(gf, "geometry")
+
+        # ensure mutating columns in gf doesn't update df
+        gf.loc[0, "A"] = 7
+        assert_frame_equal(df, df_copy)
+        gf["A"] = 3
+        assert_frame_equal(df, df_copy)
+
     def test_geodataframe_geointerface(self):
         assert self.df.__geo_interface__["type"] == "FeatureCollection"
         assert len(self.df.__geo_interface__["features"]) == self.df.shape[0]
 
     def test_geodataframe_iterfeatures(self):
         df = self.df.iloc[:1].copy()
         df.loc[0, "BoroName"] = np.nan
         # when containing missing values
-        # null: ouput the missing entries as JSON null
-        result = list(df.iterfeatures(na="null"))[0]["properties"]
+        # null: output the missing entries as JSON null
+        result = next(iter(df.iterfeatures(na="null")))["properties"]
         assert result["BoroName"] is None
         # drop: remove the property from the feature.
-        result = list(df.iterfeatures(na="drop"))[0]["properties"]
+        result = next(iter(df.iterfeatures(na="drop")))["properties"]
         assert "BoroName" not in result.keys()
         # keep: output the missing entries as NaN
-        result = list(df.iterfeatures(na="keep"))[0]["properties"]
+        result = next(iter(df.iterfeatures(na="keep")))["properties"]
         assert np.isnan(result["BoroName"])
 
         # test for checking that the (non-null) features are python scalars and
         # not numpy scalars
         assert type(df.loc[0, "Shape_Leng"]) is np.float64
         # null
-        result = list(df.iterfeatures(na="null"))[0]
-        assert type(result["properties"]["Shape_Leng"]) is float
+        result = next(iter(df.iterfeatures(na="null")))
+        assert isinstance(result["properties"]["Shape_Leng"], float)
         # drop
-        result = list(df.iterfeatures(na="drop"))[0]
-        assert type(result["properties"]["Shape_Leng"]) is float
+        result = next(iter(df.iterfeatures(na="drop")))
+        assert isinstance(result["properties"]["Shape_Leng"], float)
         # keep
-        result = list(df.iterfeatures(na="keep"))[0]
-        assert type(result["properties"]["Shape_Leng"]) is float
+        result = next(iter(df.iterfeatures(na="keep")))
+        assert isinstance(result["properties"]["Shape_Leng"], float)
 
         # when only having numerical columns
         df_only_numerical_cols = df[["Shape_Leng", "Shape_Area", "geometry"]]
         assert type(df_only_numerical_cols.loc[0, "Shape_Leng"]) is np.float64
         # null
-        result = list(df_only_numerical_cols.iterfeatures(na="null"))[0]
-        assert type(result["properties"]["Shape_Leng"]) is float
+        result = next(iter(df_only_numerical_cols.iterfeatures(na="null")))
+        assert isinstance(result["properties"]["Shape_Leng"], float)
         # drop
-        result = list(df_only_numerical_cols.iterfeatures(na="drop"))[0]
-        assert type(result["properties"]["Shape_Leng"]) is float
+        result = next(iter(df_only_numerical_cols.iterfeatures(na="drop")))
+        assert isinstance(result["properties"]["Shape_Leng"], float)
         # keep
-        result = list(df_only_numerical_cols.iterfeatures(na="keep"))[0]
-        assert type(result["properties"]["Shape_Leng"]) is float
+        result = next(iter(df_only_numerical_cols.iterfeatures(na="keep")))
+        assert isinstance(result["properties"]["Shape_Leng"], float)
+
+        with pytest.raises(
+            ValueError, match="GeoDataFrame cannot contain duplicated column names."
+        ):
+            df_with_duplicate_columns = df[
+                ["Shape_Leng", "Shape_Leng", "Shape_Area", "geometry"]
+            ]
+            list(df_with_duplicate_columns.iterfeatures())
 
         # geometry not set
         df = GeoDataFrame({"values": [0, 1], "geom": [Point(0, 1), Point(1, 0)]})
         with pytest.raises(AttributeError):
             list(df.iterfeatures())
 
+    def test_geodataframe_iterfeatures_non_scalars(self):
+        # When some features in geodataframe are non-scalar values
+        df = GeoDataFrame(
+            {"geometry": [Point(1, 2)], "non-scalar": [[1, 2]], "test_col": None}
+        )
+        # null
+        expected = {"non-scalar": [1, 2], "test_col": None}
+        result = next(iter(df.iterfeatures(na="null"))).get("properties")
+        assert expected == result
+        # drop
+        expected = {"non-scalar": [1, 2]}
+        result = next(iter(df.iterfeatures(na="drop"))).get("properties")
+        assert expected == result
+        # keep
+        expected = {"non-scalar": [1, 2], "test_col": None}
+        result = next(iter(df.iterfeatures(na="keep"))).get("properties")
+        assert expected == result
+
     def test_geodataframe_geojson_no_bbox(self):
-        geo = self.df._to_geo(na="null", show_bbox=False)
+        geo = self.df.to_geo_dict(na="null", show_bbox=False)
         assert "bbox" not in geo.keys()
         for feature in geo["features"]:
             assert "bbox" not in feature.keys()
 
     def test_geodataframe_geojson_bbox(self):
-        geo = self.df._to_geo(na="null", show_bbox=True)
+        geo = self.df.to_geo_dict(na="null", show_bbox=True)
         assert "bbox" in geo.keys()
         assert len(geo["bbox"]) == 4
         assert isinstance(geo["bbox"], tuple)
         for feature in geo["features"]:
             assert "bbox" in feature.keys()
 
     def test_pickle(self):
@@ -695,41 +950,39 @@
         filename = os.path.join(self.tempdir, "df.pkl")
         self.df.to_pickle(filename)
         unpickled = pd.read_pickle(filename)
         assert_frame_equal(self.df, unpickled)
         assert self.df.crs == unpickled.crs
 
     def test_estimate_utm_crs(self):
-        if PYPROJ_LT_3:
-            with pytest.raises(RuntimeError, match=r"pyproj 3\+ required"):
-                self.df.estimate_utm_crs()
-        else:
-            assert self.df.estimate_utm_crs() == CRS("EPSG:32618")
-            assert self.df.estimate_utm_crs("NAD83") == CRS("EPSG:26918")
+        pyproj = pytest.importorskip("pyproj")
+
+        assert self.df.estimate_utm_crs() == pyproj.CRS("EPSG:32618")
+        assert self.df.estimate_utm_crs("NAD83") == pyproj.CRS("EPSG:26918")
 
     def test_to_wkb(self):
         wkbs0 = [
-            (
+            (  # POINT (0 0)
                 b"\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00"
                 b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
-            ),  # POINT (0 0)
-            (
+            ),
+            (  # POINT (1 1)
                 b"\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00"
                 b"\x00\xf0?\x00\x00\x00\x00\x00\x00\xf0?"
-            ),  # POINT (1 1)
+            ),
         ]
         wkbs1 = [
-            (
+            (  # POINT (2 2)
                 b"\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00"
                 b"\x00\x00@\x00\x00\x00\x00\x00\x00\x00@"
-            ),  # POINT (2 2)
-            (
+            ),
+            (  # POINT (3 3)
                 b"\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00"
                 b"\x00\x08@\x00\x00\x00\x00\x00\x00\x08@"
-            ),  # POINT (3 3)
+            ),
         ]
         gs0 = GeoSeries.from_wkb(wkbs0)
         gs1 = GeoSeries.from_wkb(wkbs1)
         gdf = GeoDataFrame({"geom_col0": gs0, "geom_col1": gs1})
 
         expected_df = pd.DataFrame({"geom_col0": wkbs0, "geom_col1": wkbs1})
         assert_frame_equal(expected_df, gdf.to_wkb())
@@ -740,14 +993,94 @@
         gs0 = GeoSeries.from_wkt(wkts0)
         gs1 = GeoSeries.from_wkt(wkts1)
         gdf = GeoDataFrame({"gs0": gs0, "gs1": gs1})
 
         expected_df = pd.DataFrame({"gs0": wkts0, "gs1": wkts1})
         assert_frame_equal(expected_df, gdf.to_wkt())
 
+    @pytest.mark.parametrize("how", ["left", "inner", "right"])
+    @pytest.mark.parametrize("predicate", ["intersects", "within", "contains"])
+    def test_sjoin(self, how, predicate, naturalearth_cities, naturalearth_lowres):
+        """
+        Basic test for availability of the GeoDataFrame method. Other
+        sjoin tests are located in /tools/tests/test_sjoin.py
+        """
+        left = read_file(naturalearth_cities)
+        right = read_file(naturalearth_lowres)
+
+        expected = geopandas.sjoin(left, right, how=how, predicate=predicate)
+        result = left.sjoin(right, how=how, predicate=predicate)
+        assert_geodataframe_equal(result, expected)
+
+    @pytest.mark.parametrize("how", ["left", "inner", "right"])
+    @pytest.mark.parametrize("distance", [0, 3])
+    @pytest.mark.skipif(
+        not compat.GEOS_GE_310,
+        reason="`dwithin` requires GEOS 3.10",
+    )
+    def test_sjoin_dwithin(self, how, distance):
+        """
+        Basic test for predicate='dwithin' availability of the GeoDataFrame method.
+        Other sjoin tests are located in /tools/tests/test_sjoin.py
+        """
+        left = GeoDataFrame(geometry=points_from_xy([0, 1, 2], [0, 1, 1]))
+        right = GeoDataFrame(geometry=[box(0, 0, 1, 1)])
+
+        expected = geopandas.sjoin(
+            left, right, how=how, predicate="dwithin", distance=distance
+        )
+        result = left.sjoin(right, how=how, predicate="dwithin", distance=distance)
+        assert_geodataframe_equal(result, expected)
+
+    @pytest.mark.parametrize("how", ["left", "inner", "right"])
+    @pytest.mark.parametrize("max_distance", [None, 1])
+    @pytest.mark.parametrize("distance_col", [None, "distance"])
+    @pytest.mark.filterwarnings("ignore:Geometry is in a geographic CRS:UserWarning")
+    def test_sjoin_nearest(
+        self, how, max_distance, distance_col, naturalearth_cities, naturalearth_lowres
+    ):
+        """
+        Basic test for availability of the GeoDataFrame method. Other
+        sjoin tests are located in /tools/tests/test_sjoin.py
+        """
+        left = read_file(naturalearth_cities)
+        right = read_file(naturalearth_lowres)
+
+        expected = geopandas.sjoin_nearest(
+            left, right, how=how, max_distance=max_distance, distance_col=distance_col
+        )
+        result = left.sjoin_nearest(
+            right, how=how, max_distance=max_distance, distance_col=distance_col
+        )
+        assert_geodataframe_equal(result, expected)
+
+    def test_clip(self, naturalearth_cities, naturalearth_lowres):
+        """
+        Basic test for availability of the GeoDataFrame method. Other
+        clip tests are located in /tools/tests/test_clip.py
+        """
+        left = read_file(naturalearth_cities)
+        world = read_file(naturalearth_lowres)
+        south_america = world[world["continent"] == "South America"]
+
+        expected = geopandas.clip(left, south_america)
+        result = left.clip(south_america)
+        assert_geodataframe_equal(result, expected)
+
+    def test_overlay(self, dfs, how):
+        """
+        Basic test for availability of the GeoDataFrame method. Other
+        overlay tests are located in tests/test_overlay.py
+        """
+        df1, df2 = dfs
+
+        expected = geopandas.overlay(df1, df2, how=how)
+        result = df1.overlay(df2, how=how)
+        assert_geodataframe_equal(result, expected)
+
 
 def check_geodataframe(df, geometry_column="geometry"):
     assert isinstance(df, GeoDataFrame)
     assert isinstance(df.geometry, GeoSeries)
     assert isinstance(df[geometry_column], GeoSeries)
     assert df._geometry_column_name == geometry_column
     assert df.geometry.name == geometry_column
@@ -776,15 +1109,14 @@
 
         df = GeoDataFrame(data, columns=["A", "geometry"])
         check_geodataframe(df)
         assert_index_equal(df.columns, pd.Index(["A", "geometry"]))
         assert_series_equal(df["A"], pd.Series(range(3), name="A"))
 
     def test_dict_of_series(self):
-
         data = {
             "A": pd.Series(range(3)),
             "B": pd.Series(np.arange(3.0)),
             "geometry": GeoSeries([Point(x, x) for x in range(3)]),
         }
 
         df = GeoDataFrame(data)
@@ -801,15 +1133,14 @@
             "B": np.arange(3.0),
             "geometry": GeoSeries([Point(x, x) for x in range(3)]),
         }
         with pytest.raises(ValueError):
             GeoDataFrame(data, index=[1, 2])
 
     def test_dict_specified_geometry(self):
-
         data = {
             "A": range(3),
             "B": np.arange(3.0),
             "other_geom": [Point(x, x) for x in range(3)],
         }
 
         df = GeoDataFrame(data, geometry="other_geom")
@@ -861,15 +1192,14 @@
         }
         gpdf = GeoDataFrame(data)
         pddf = pd.DataFrame(data)
         check_geodataframe(gpdf)
         assert type(pddf) == pd.DataFrame
 
         for df in [gpdf, pddf]:
-
             res = GeoDataFrame(df)
             check_geodataframe(res)
 
             res = GeoDataFrame(df, index=pd.Index([0, 2]))
             check_geodataframe(res)
             assert_index_equal(res.index, pd.Index([0, 2]))
             assert res["A"].tolist() == [0, 2]
@@ -892,19 +1222,17 @@
         check_geodataframe(gpdf, "other_geom")
         pddf = pd.DataFrame(data)
 
         for df in [gpdf, pddf]:
             res = GeoDataFrame(df, geometry="other_geom")
             check_geodataframe(res, "other_geom")
 
-        # when passing GeoDataFrame with custom geometry name to constructor
-        # an invalid geodataframe is the result TODO is this desired ?
+        # gdf from gdf should preserve active geometry column name
         df = GeoDataFrame(gpdf)
-        with pytest.raises(AttributeError):
-            df.geometry
+        check_geodataframe(df, "other_geom")
 
     def test_only_geometry(self):
         exp = GeoDataFrame(
             {"geometry": [Point(x, x) for x in range(3)], "other": range(3)}
         )[["geometry"]]
 
         df = GeoDataFrame(geometry=[Point(x, x) for x in range(3)])
@@ -955,15 +1283,14 @@
             columns=["geometry", "a"],
             index=pd.Index([0, 0, 1]),
             geometry="geometry",
         )
         check_geodataframe(gdf)
         gdf.columns == ["geometry", "a"]
 
-    @pytest.mark.xfail
     def test_preserve_series_name(self):
         geoms = [Point(1, 1), Point(2, 2), Point(3, 3)]
         gs = GeoSeries(geoms)
         gdf = GeoDataFrame({"a": [1, 2, 3]}, geometry=gs)
 
         check_geodataframe(gdf, geometry_column="geometry")
 
@@ -977,12 +1304,282 @@
         # GH602
         data = pd.DataFrame({"geometry": [1, 2, 3], "col1": [4, 5, 6]})
         geoms = pd.Series([Point(i, i) for i in range(3)])
         # passed geometry kwarg should overwrite geometry column in data
         res = GeoDataFrame(data, geometry=geoms)
         assert_geoseries_equal(res.geometry, GeoSeries(geoms))
 
+    def test_repeat_geo_col(self):
+        df = pd.DataFrame(
+            [
+                {"geometry": Point(x, y), "geom": Point(x, y)}
+                for x, y in zip(range(3), range(3))
+            ],
+        )
+        # explicitly prevent construction of gdf with repeat geometry column names
+        # two columns called "geometry", geom col inferred
+        df2 = df.rename(columns={"geom": "geometry"})
+        with pytest.raises(ValueError):
+            GeoDataFrame(df2)
+        # ensure case is caught when custom geom column name is used
+        # two columns called "geom", geom col explicit
+        df3 = df.rename(columns={"geometry": "geom"})
+        with pytest.raises(ValueError):
+            GeoDataFrame(df3, geometry="geom")
+
+    @pytest.mark.parametrize("dtype", ["geometry", "object"])
+    def test_multiindex_with_geometry_label(self, dtype):
+        # DataFrame with MultiIndex where "geometry" label corresponds to
+        # multiple columns
+        df = pd.DataFrame([[Point(0, 0), Point(1, 1)], [Point(2, 2), Point(3, 3)]])
+        df = df.astype(dtype)
+        df.columns = pd.MultiIndex.from_product([["geometry"], [0, 1]])
+        # don't error in constructor
+        gdf = GeoDataFrame(df)
+        with pytest.raises(AttributeError, match=".*geometry .* has not been set.*"):
+            gdf.geometry
+        res_gdf = gdf.set_geometry(("geometry", 0))
+        assert res_gdf.shape == gdf.shape
+        assert isinstance(res_gdf.geometry, GeoSeries)
+
+    def test_default_geo_colname_none(self):
+        match = "You are adding a column named 'geometry' to a GeoDataFrame"
+        gdf = GeoDataFrame({"a": [1, 2]})
+
+        gdf2 = gdf.copy()
+        geo_col = GeoSeries.from_xy([1, 3], [3, 3])
+        with pytest.warns(FutureWarning, match=match):
+            gdf2["geometry"] = geo_col
+        assert gdf2._geometry_column_name == "geometry"
+        gdf4 = gdf.copy()
+        with pytest.warns(FutureWarning, match=match):
+            gdf4.geometry = geo_col
+        assert gdf4._geometry_column_name == "geometry"
+
+        # geo col name should only change if we add geometry
+        gdf5 = gdf.copy()
+        with pytest.warns(
+            UserWarning, match="Geometry column does not contain geometry"
+        ):
+            gdf5["geometry"] = "foo"
+        assert gdf5._geometry_column_name is None
+        with pytest.warns(FutureWarning, match=match):
+            gdf3 = gdf.copy().assign(geometry=geo_col)
+        assert gdf3._geometry_column_name == "geometry"
+
+        # Check that adding a GeoSeries to a column called "geometry" to a
+        # gdf without an active geometry column some time after the init does not
+        # warn / set the active geometry column
+        gdf6 = gdf.copy()
+        gdf6["geom2"] = geo_col
+        gdf6["geom3"] = geo_col
+        gdf6 = gdf6.set_geometry("geom2")
+        subset = gdf6[["a", "geom3"]]  # this has a missing active geometry col
+        assert subset._geometry_column_name == "geom2"
+        subset["geometry"] = geo_col
+        # adding column called geometry shouldn't auto-set
+        assert subset._geometry_column_name == "geom2"
+
+    def test_multiindex_geometry_colname_2_level(self):
+        # GH1763 https://github.com/geopandas/geopandas/issues/1763
+        crs = "EPSG:4326"
+        df = pd.DataFrame(
+            [[1, 0], [0, 1]], columns=[["location", "location"], ["x", "y"]]
+        )
+        x_col = df["location", "x"]
+        y_col = df["location", "y"]
 
+        gdf = GeoDataFrame(df, crs=crs, geometry=points_from_xy(x_col, y_col))
+        if compat.HAS_PYPROJ:
+            assert gdf.crs == crs
+            assert gdf.geometry.crs == crs
+        assert gdf.geometry.dtype == "geometry"
+        assert gdf._geometry_column_name == "geometry"
+        assert gdf.geometry.name == "geometry"
+
+    def test_multiindex_geometry_colname_3_level(self):
+        # GH1763 https://github.com/geopandas/geopandas/issues/1763
+        # Note 3-level case uses different code paths in pandas, it is not redundant
+        crs = "EPSG:4326"
+        df = pd.DataFrame(
+            [[1, 0], [0, 1]],
+            columns=[
+                ["foo", "foo"],
+                ["location", "location"],
+                ["x", "y"],
+            ],
+        )
+
+        x_col = df["foo", "location", "x"]
+        y_col = df["foo", "location", "y"]
+
+        gdf = GeoDataFrame(df, crs=crs, geometry=points_from_xy(x_col, y_col))
+        if compat.HAS_PYPROJ:
+            assert gdf.crs == crs
+            assert gdf.geometry.crs == crs
+        assert gdf.geometry.dtype == "geometry"
+        assert gdf._geometry_column_name == "geometry"
+        assert gdf.geometry.name == "geometry"
+
+    def test_multiindex_geometry_colname_3_level_new_col(self):
+        crs = "EPSG:4326"
+        df = pd.DataFrame(
+            [[1, 0], [0, 1]],
+            columns=[
+                ["foo", "foo"],
+                ["location", "location"],
+                ["x", "y"],
+            ],
+        )
+
+        x_col = df["foo", "location", "x"]
+        y_col = df["foo", "location", "y"]
+        df["geometry"] = GeoSeries.from_xy(x_col, y_col)
+        df2 = df.copy()
+        gdf = df.set_geometry("geometry", crs=crs)
+        if compat.HAS_PYPROJ:
+            assert gdf.crs == crs
+        assert gdf._geometry_column_name == "geometry"
+        assert gdf.geometry.name == "geometry"
+        # test again setting with tuple col name
+        gdf = df2.set_geometry(("geometry", "", ""), crs=crs)
+        if compat.HAS_PYPROJ:
+            assert gdf.crs == crs
+        assert gdf._geometry_column_name == ("geometry", "", "")
+        assert gdf.geometry.name == ("geometry", "", "")
+
+    def test_assign_cols_using_index(self, nybb_filename):
+        df = read_file(nybb_filename)
+        other_df = pd.DataFrame({"foo": range(5), "bar": range(5)})
+        expected = pd.concat([df, other_df], axis=1)
+        df[other_df.columns] = other_df
+        assert_geodataframe_equal(df, expected)
+
+
+@pytest.mark.skipif(not compat.HAS_PYPROJ, reason="pyproj not available")
 def test_geodataframe_crs():
-    gdf = GeoDataFrame()
+    gdf = GeoDataFrame(columns=["geometry"])
     gdf.crs = "IGNF:ETRS89UTM28"
     assert gdf.crs.to_authority() == ("IGNF", "ETRS89UTM28")
+
+
+def test_geodataframe_nocrs_json():
+    # no CRS, no crs field
+    gdf = GeoDataFrame(columns=["geometry"])
+    gdf_geojson = json.loads(gdf.to_json())
+    assert "crs" not in gdf_geojson
+
+    # WGS84, no crs field (default as per spec)
+    gdf.crs = 4326
+    gdf_geojson = json.loads(gdf.to_json())
+    assert "crs" not in gdf_geojson
+
+
+@pytest.mark.skipif(not compat.HAS_PYPROJ, reason="pyproj not available")
+def test_geodataframe_crs_json():
+    gdf = GeoDataFrame(columns=["geometry"])
+    gdf.crs = 25833
+    gdf_geojson = json.loads(gdf.to_json())
+    assert "crs" in gdf_geojson
+    assert gdf_geojson["crs"] == {
+        "type": "name",
+        "properties": {"name": "urn:ogc:def:crs:EPSG::25833"},
+    }
+    gdf_geointerface = gdf.__geo_interface__
+    assert "crs" not in gdf_geointerface
+
+
+@pytest.mark.skipif(not compat.HAS_PYPROJ, reason="pyproj not available")
+@pytest.mark.parametrize(
+    "crs",
+    ["+proj=cea +lon_0=0 +lat_ts=45 +x_0=0 +y_0=0 +ellps=WGS84 +units=m", "IGNF:WGS84"],
+)
+def test_geodataframe_crs_nonrepresentable_json(crs):
+    gdf = GeoDataFrame(
+        [Point(1000, 1000)],
+        columns=["geometry"],
+        crs=crs,
+    )
+    with pytest.warns(
+        UserWarning, match="GeoDataFrame's CRS is not representable in URN OGC"
+    ):
+        gdf_geojson = json.loads(gdf.to_json())
+    assert "crs" not in gdf_geojson
+
+
+def test_geodataframe_crs_colname():
+    # https://github.com/geopandas/geopandas/issues/2942
+    gdf = GeoDataFrame({"crs": [1], "geometry": [Point(1, 1)]})
+    assert gdf.crs is None
+    assert gdf["crs"].iloc[0] == 1
+    assert getattr(gdf, "crs") is None
+
+
+@pytest.fixture
+def nybb2(nybb_filename):
+    yield read_file(nybb_filename).head(2)
+
+
+@pytest.mark.parametrize("geo_col_name", ["geometry", "polygons"])
+def test_set_geometry_supply_colname(nybb2, geo_col_name):
+    if geo_col_name != "geometry":
+        nybb2 = nybb2.rename_geometry(geo_col_name)
+    nybb2["centroid"] = nybb2.geometry.centroid
+    res = nybb2.set_geometry("centroid")
+    assert res.active_geometry_name == "centroid"
+    assert geo_col_name in res.columns
+
+    # Test that drop=False explicitly warns
+    deprecated = "The `drop` keyword argument is deprecated"
+    with pytest.warns(FutureWarning, match=deprecated):
+        res2 = nybb2.set_geometry("centroid", drop=False)
+    assert_geodataframe_equal(res, res2)
+
+    with pytest.warns(FutureWarning, match=deprecated):
+        res3 = nybb2.set_geometry("centroid", drop=True)
+    # drop=True should preserve previous geometry col name (keep old behaviour)
+    assert res3.active_geometry_name == geo_col_name
+    assert "centroid" not in res3.columns
+
+    # Test that alternative suggested without using drop=True is equivalent
+    assert_geodataframe_equal(
+        res3,
+        nybb2.set_geometry("centroid")
+        .drop(columns=geo_col_name)
+        .rename_geometry(geo_col_name),
+    )
+
+
+@pytest.mark.parametrize("geo_col_name", ["geometry", "polygons"])
+def test_set_geometry_supply_arraylike(nybb2, geo_col_name):
+    if geo_col_name != "geometry":
+        nybb2 = nybb2.rename_geometry(geo_col_name)
+    centroids = nybb2.geometry.centroid
+    res = nybb2.set_geometry(centroids)
+    assert res.active_geometry_name == geo_col_name
+    # drop should do nothing if the column already exists
+    match_str = (
+        "The `drop` keyword argument is deprecated and has no effect when "
+        "`col` is an array-like value"
+    )
+    with pytest.warns(
+        FutureWarning,
+        match=match_str,
+    ):
+        res2 = nybb2.set_geometry(centroids, drop=True)
+    assert res2.active_geometry_name == geo_col_name
+
+    centroids = centroids.rename("centroids")
+    res3 = nybb2.set_geometry(centroids)
+    # Should preserve the geoseries name
+    # (and old geometry column should be kept)
+    assert res3.active_geometry_name == "centroids"
+    assert geo_col_name in res3.columns
+
+    # Drop should not remove previous active geometry colname for arraylike inputs
+    with pytest.warns(
+        FutureWarning,
+        match=match_str,
+    ):
+        res4 = nybb2.set_geometry(centroids, drop=True)
+    assert res4.active_geometry_name == "centroids"
+    assert geo_col_name in res4.columns
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_overlay.py` & `geopandas-1.0.0a1/geopandas/tests/test_overlay.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import os
 
+import numpy as np
 import pandas as pd
 
+from shapely import make_valid
 from shapely.geometry import Point, Polygon, LineString, GeometryCollection, box
-from fiona.errors import DriverError
 
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries, overlay, read_file
+from geopandas._compat import PANDAS_GE_20, HAS_PYPROJ
 
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 import pytest
 
-DATA = os.path.join(os.path.abspath(os.path.dirname(__file__)), "data", "overlay")
+try:
+    from fiona.errors import DriverError
+except ImportError:
+
+    class DriverError(Exception):
+        pass
 
 
-pytestmark = pytest.mark.skip_no_sindex
+DATA = os.path.join(os.path.abspath(os.path.dirname(__file__)), "data", "overlay")
 
 
 @pytest.fixture
 def dfs(request):
     s1 = GeoSeries(
         [
             Polygon([(0, 0), (2, 0), (2, 2), (0, 2)]),
@@ -71,14 +78,16 @@
     # construction of result
 
     def _read(name):
         expected = read_file(
             os.path.join(DATA, "polys", "df1_df2-{0}.geojson".format(name))
         )
         expected.crs = None
+        for col in expected.columns[expected.dtypes == "int32"]:
+            expected[col] = expected[col].astype("int64")
         return expected
 
     if how == "identity":
         expected_intersection = _read("intersection")
         expected_difference = _read("difference")
         expected = pd.concat(
             [expected_intersection, expected_difference], ignore_index=True, sort=False
@@ -100,16 +109,16 @@
         result = overlay(df2, df1, how=how)
         result = result.reset_index(drop=True)
         expected = _read("difference-inverse")
         assert_geodataframe_equal(result, expected, check_column_type=False)
 
 
 @pytest.mark.filterwarnings("ignore:GeoSeries crs mismatch:UserWarning")
-def test_overlay_nybb(how):
-    polydf = read_file(geopandas.datasets.get_path("nybb"))
+def test_overlay_nybb(how, nybb_filename):
+    polydf = read_file(nybb_filename)
 
     # The circles have been constructed and saved at the time the expected
     # results were created (exact output of buffer algorithm can slightly
     # change over time -> use saved ones)
     # # construct circles dataframe
     # N = 10
     # b = [int(x) for x in polydf.total_bounds]
@@ -179,31 +188,36 @@
     # since the order of the constituent polygons depends on
     # the ordering of spatial indexing results, we cannot
     # compare symmetric_difference results directly when the
     # resultant geometry is a multipolygon
 
     # first, check that all bounds and areas are approx equal
     # this is a very rough check for multipolygon equality
+    kwargs = {}
     pd.testing.assert_series_equal(
-        result.geometry.area, expected.geometry.area, check_less_precise=True
+        result.geometry.area, expected.geometry.area, **kwargs
     )
     pd.testing.assert_frame_equal(
-        result.geometry.bounds, expected.geometry.bounds, check_less_precise=True
+        result.geometry.bounds, expected.geometry.bounds, **kwargs
     )
 
     # There are two cases where the multipolygon have a different number
     # of sub-geometries -> not solved by normalize (and thus drop for now)
     if how == "symmetric_difference":
         expected.loc[9, "geometry"] = None
         result.loc[9, "geometry"] = None
 
     if how == "union":
         expected.loc[24, "geometry"] = None
         result.loc[24, "geometry"] = None
 
+    # missing values get read as None in read_file for a string column, but
+    # are introduced as NaN by overlay
+    expected["BoroName"] = expected["BoroName"].fillna(np.nan)
+
     assert_geodataframe_equal(
         result,
         expected,
         normalize=True,
         check_crs=False,
         check_column_type=False,
         check_less_precise=True,
@@ -315,39 +329,43 @@
 
 def test_bad_how(dfs):
     df1, df2 = dfs
     with pytest.raises(ValueError):
         overlay(df1, df2, how="spandex")
 
 
-def test_duplicate_column_name(dfs):
+def test_duplicate_column_name(dfs, how):
+    if how == "difference":
+        pytest.skip("Difference uses columns from one df only.")
     df1, df2 = dfs
     df2r = df2.rename(columns={"col2": "col1"})
-    res = overlay(df1, df2r, how="union")
+    res = overlay(df1, df2r, how=how)
     assert ("col1_1" in res.columns) and ("col1_2" in res.columns)
 
 
 def test_geoseries_warning(dfs):
     df1, df2 = dfs
     # Issue #305
     with pytest.raises(NotImplementedError):
         overlay(df1, df2.geometry, how="union")
 
 
+@pytest.mark.skipif(not HAS_PYPROJ, reason="pyproj not available")
 def test_preserve_crs(dfs, how):
     df1, df2 = dfs
     result = overlay(df1, df2, how=how)
     assert result.crs is None
     crs = "epsg:4326"
     df1.crs = crs
     df2.crs = crs
     result = overlay(df1, df2, how=how)
     assert result.crs == crs
 
 
+@pytest.mark.skipif(not HAS_PYPROJ, reason="pyproj not available")
 def test_crs_mismatch(dfs, how):
     df1, df2 = dfs
     df1.crs = 4326
     df2.crs = 3857
     with pytest.warns(UserWarning, match="CRS mismatch between the CRS"):
         overlay(df1, df2, how=how)
 
@@ -359,15 +377,15 @@
             Polygon([(-1, -1), (-3, -1), (-3, -3), (-1, -3)]),
             Polygon([(-3, -3), (-5, -3), (-5, -5), (-3, -5)]),
         ]
     )
     df3 = GeoDataFrame({"geometry": polys3, "col3": [1, 2]})
     expected = GeoDataFrame([], columns=["col1", "col3", "geometry"])
     result = overlay(df1, df3)
-    assert_geodataframe_equal(result, expected, check_like=True)
+    assert_geodataframe_equal(result, expected, check_dtype=False)
 
 
 def test_correct_index(dfs):
     # GH883 - case where the index was not properly reset
     df1, df2 = dfs
     polys3 = GeoSeries(
         [
@@ -383,15 +401,14 @@
         [[1, 1, i1], [3, 2, i2]], columns=["col3", "col2", "geometry"]
     )
     result = overlay(df3, df2, keep_geom_type=True)
     assert_geodataframe_equal(result, expected)
 
 
 def test_warn_on_keep_geom_type(dfs):
-
     df1, df2 = dfs
     polys3 = GeoSeries(
         [
             Polygon([(1, 1), (3, 1), (3, 3), (1, 3)]),
             Polygon([(-1, 1), (1, 1), (1, 3), (-1, 3)]),
             Polygon([(3, 3), (5, 3), (5, 5), (3, 5)]),
         ]
@@ -493,18 +510,24 @@
             )
         )
 
         # the order depends on the spatial index used
         # so we sort the resultant dataframes to get a consistent order
         # independently of the spatial index implementation
         assert all(expected.columns == result.columns), "Column name mismatch"
-        cols = list(set(result.columns) - set(["geometry"]))
+        cols = list(set(result.columns) - {"geometry"})
         expected = expected.sort_values(cols, axis=0).reset_index(drop=True)
         result = result.sort_values(cols, axis=0).reset_index(drop=True)
 
+        # some columns are all-NaN in the result, but get read as object dtype
+        # column of None values in read_file
+        for col in ["col1", "col3", "col4"]:
+            if col in expected.columns and expected[col].isna().all():
+                expected[col] = expected[col].astype("float64")
+
         assert_geodataframe_equal(
             result,
             expected,
             normalize=True,
             check_column_type=False,
             check_less_precise=True,
             check_crs=False,
@@ -513,14 +536,17 @@
 
     except DriverError:  # fiona >= 1.8
         assert result.empty
 
     except OSError:  # fiona < 1.8
         assert result.empty
 
+    except RuntimeError:  # pyogrio.DataSourceError
+        assert result.empty
+
 
 def test_mixed_geom_error():
     polys1 = GeoSeries(
         [
             Polygon([(1, 1), (3, 1), (3, 3), (1, 3)]),
             Polygon([(3, 3), (5, 3), (5, 5), (3, 5)]),
         ]
@@ -560,35 +586,306 @@
 
 def test_keep_geom_type_geometry_collection():
     # GH 1581
 
     df1 = read_file(os.path.join(DATA, "geom_type", "df1.geojson"))
     df2 = read_file(os.path.join(DATA, "geom_type", "df2.geojson"))
 
+    with pytest.warns(UserWarning, match="`keep_geom_type=True` in overlay"):
+        intersection = overlay(df1, df2, keep_geom_type=None)
+    assert len(intersection) == 1
+    assert (intersection.geom_type == "Polygon").all()
+
     intersection = overlay(df1, df2, keep_geom_type=True)
     assert len(intersection) == 1
     assert (intersection.geom_type == "Polygon").all()
 
     intersection = overlay(df1, df2, keep_geom_type=False)
     assert len(intersection) == 1
     assert (intersection.geom_type == "GeometryCollection").all()
 
 
-@pytest.mark.parametrize("make_valid", [True, False])
-def test_overlap_make_valid(make_valid):
+def test_keep_geom_type_geometry_collection2():
+    polys1 = [
+        box(0, 0, 1, 1),
+        box(1, 1, 3, 3).union(box(1, 3, 5, 5)),
+    ]
+
+    polys2 = [
+        box(0, 0, 1, 1),
+        box(3, 1, 4, 2).union(box(4, 1, 5, 4)),
+    ]
+    df1 = GeoDataFrame({"left": [0, 1], "geometry": polys1})
+    df2 = GeoDataFrame({"right": [0, 1], "geometry": polys2})
+
+    result1 = overlay(df1, df2, keep_geom_type=True)
+    expected1 = GeoDataFrame(
+        {
+            "left": [0, 1],
+            "right": [0, 1],
+            "geometry": [box(0, 0, 1, 1), box(4, 3, 5, 4)],
+        }
+    )
+    assert_geodataframe_equal(result1, expected1)
+
+    result1 = overlay(df1, df2, keep_geom_type=False)
+    expected1 = GeoDataFrame(
+        {
+            "left": [0, 1, 1],
+            "right": [0, 0, 1],
+            "geometry": [
+                box(0, 0, 1, 1),
+                Point(1, 1),
+                GeometryCollection([box(4, 3, 5, 4), LineString([(3, 1), (3, 2)])]),
+            ],
+        }
+    )
+    assert_geodataframe_equal(result1, expected1)
+
+
+def test_keep_geom_type_geomcoll_different_types():
+    polys1 = [box(0, 1, 1, 3), box(10, 10, 12, 12)]
+    polys2 = [
+        Polygon([(1, 0), (3, 0), (3, 3), (1, 3), (1, 2), (2, 2), (2, 1), (1, 1)]),
+        box(11, 11, 13, 13),
+    ]
+    df1 = GeoDataFrame({"left": [0, 1], "geometry": polys1})
+    df2 = GeoDataFrame({"right": [0, 1], "geometry": polys2})
+    result1 = overlay(df1, df2, keep_geom_type=True)
+    expected1 = GeoDataFrame(
+        {
+            "left": [1],
+            "right": [1],
+            "geometry": [box(11, 11, 12, 12)],
+        }
+    )
+    assert_geodataframe_equal(result1, expected1)
+
+    result2 = overlay(df1, df2, keep_geom_type=False)
+    expected2 = GeoDataFrame(
+        {
+            "left": [0, 1],
+            "right": [0, 1],
+            "geometry": [
+                GeometryCollection([LineString([(1, 2), (1, 3)]), Point(1, 1)]),
+                box(11, 11, 12, 12),
+            ],
+        }
+    )
+    assert_geodataframe_equal(result2, expected2)
+
+
+def test_keep_geom_type_geometry_collection_difference():
+    # GH 2163
+
+    polys1 = [
+        box(0, 0, 1, 1),
+        box(1, 1, 2, 2),
+    ]
+
+    # the tiny sliver in the second geometry may be converted to a
+    # linestring during the overlay process due to floating point errors
+    # on some platforms
+    polys2 = [
+        box(0, 0, 1, 1),
+        box(1, 1, 2, 3).union(box(2, 2, 3, 2.00000000000000001)),
+    ]
+    df1 = GeoDataFrame({"left": [0, 1], "geometry": polys1})
+    df2 = GeoDataFrame({"right": [0, 1], "geometry": polys2})
+
+    result1 = overlay(df2, df1, keep_geom_type=True, how="difference")
+    expected1 = GeoDataFrame(
+        {
+            "right": [1],
+            "geometry": [box(1, 2, 2, 3)],
+        },
+    )
+
+    assert_geodataframe_equal(result1, expected1)
+
+
+@pytest.mark.parametrize("should_make_valid", [True, False])
+def test_overlap_make_valid(should_make_valid):
     bowtie = Polygon([(1, 1), (9, 9), (9, 1), (1, 9), (1, 1)])
     assert not bowtie.is_valid
-    fixed_bowtie = bowtie.buffer(0)
+    fixed_bowtie = make_valid(bowtie)
     assert fixed_bowtie.is_valid
 
     df1 = GeoDataFrame({"col1": ["region"], "geometry": GeoSeries([box(0, 0, 10, 10)])})
     df_bowtie = GeoDataFrame(
         {"col1": ["invalid", "valid"], "geometry": GeoSeries([bowtie, fixed_bowtie])}
     )
 
-    if make_valid:
-        df_overlay_bowtie = overlay(df1, df_bowtie, make_valid=make_valid)
+    if should_make_valid:
+        df_overlay_bowtie = overlay(df1, df_bowtie, make_valid=should_make_valid)
         assert df_overlay_bowtie.at[0, "geometry"].equals(fixed_bowtie)
         assert df_overlay_bowtie.at[1, "geometry"].equals(fixed_bowtie)
     else:
         with pytest.raises(ValueError, match="1 invalid input geometries"):
-            overlay(df1, df_bowtie, make_valid=make_valid)
+            overlay(df1, df_bowtie, make_valid=should_make_valid)
+
+
+def test_empty_overlay_return_non_duplicated_columns(nybb_filename):
+    nybb = geopandas.read_file(nybb_filename)
+    nybb2 = nybb.copy()
+    nybb2.geometry = nybb2.translate(20000000)
+
+    result = geopandas.overlay(nybb, nybb2)
+
+    expected = GeoDataFrame(
+        columns=[
+            "BoroCode_1",
+            "BoroName_1",
+            "Shape_Leng_1",
+            "Shape_Area_1",
+            "BoroCode_2",
+            "BoroName_2",
+            "Shape_Leng_2",
+            "Shape_Area_2",
+            "geometry",
+        ],
+        crs=nybb.crs,
+    )
+    assert_geodataframe_equal(result, expected, check_dtype=False)
+
+
+def test_non_overlapping(how):
+    p1 = Polygon([(0, 0), (2, 0), (2, 2), (0, 2)])
+    p2 = Polygon([(3, 3), (5, 3), (5, 5), (3, 5)])
+    df1 = GeoDataFrame({"col1": [1], "geometry": [p1]})
+    df2 = GeoDataFrame({"col2": [2], "geometry": [p2]})
+    result = overlay(df1, df2, how=how)
+
+    if how == "intersection":
+        if PANDAS_GE_20:
+            index = None
+        else:
+            index = pd.Index([], dtype="object")
+
+        expected = GeoDataFrame(
+            {
+                "col1": np.array([], dtype="int64"),
+                "col2": np.array([], dtype="int64"),
+                "geometry": [],
+            },
+            index=index,
+        )
+    elif how == "union":
+        expected = GeoDataFrame(
+            {
+                "col1": [1, np.nan],
+                "col2": [np.nan, 2],
+                "geometry": [p1, p2],
+            }
+        )
+    elif how == "identity":
+        expected = GeoDataFrame(
+            {
+                "col1": [1.0],
+                "col2": [np.nan],
+                "geometry": [p1],
+            }
+        )
+    elif how == "symmetric_difference":
+        expected = GeoDataFrame(
+            {
+                "col1": [1, np.nan],
+                "col2": [np.nan, 2],
+                "geometry": [p1, p2],
+            }
+        )
+    elif how == "difference":
+        expected = GeoDataFrame(
+            {
+                "col1": [1],
+                "geometry": [p1],
+            }
+        )
+
+    assert_geodataframe_equal(result, expected)
+
+
+def test_no_intersection():
+    # overlapping bounds but non-overlapping geometries
+    gs = GeoSeries([Point(x, x).buffer(0.1) for x in range(3)])
+    gdf1 = GeoDataFrame({"foo": ["a", "b", "c"]}, geometry=gs)
+    gdf2 = GeoDataFrame({"bar": ["1", "3", "5"]}, geometry=gs.translate(1))
+
+    expected = GeoDataFrame(columns=["foo", "bar", "geometry"])
+    result = overlay(gdf1, gdf2, how="intersection")
+    assert_geodataframe_equal(result, expected, check_index_type=False)
+
+
+class TestOverlayWikiExample:
+    def setup_method(self):
+        self.layer_a = GeoDataFrame(geometry=[box(0, 2, 6, 6)])
+
+        self.layer_b = GeoDataFrame(geometry=[box(4, 0, 10, 4)])
+
+        self.intersection = GeoDataFrame(geometry=[box(4, 2, 6, 4)])
+
+        self.union = GeoDataFrame(
+            geometry=[
+                box(4, 2, 6, 4),
+                Polygon([(4, 2), (0, 2), (0, 6), (6, 6), (6, 4), (4, 4), (4, 2)]),
+                Polygon([(10, 0), (4, 0), (4, 2), (6, 2), (6, 4), (10, 4), (10, 0)]),
+            ]
+        )
+
+        self.a_difference_b = GeoDataFrame(
+            geometry=[Polygon([(4, 2), (0, 2), (0, 6), (6, 6), (6, 4), (4, 4), (4, 2)])]
+        )
+
+        self.b_difference_a = GeoDataFrame(
+            geometry=[
+                Polygon([(10, 0), (4, 0), (4, 2), (6, 2), (6, 4), (10, 4), (10, 0)])
+            ]
+        )
+
+        self.symmetric_difference = GeoDataFrame(
+            geometry=[
+                Polygon([(4, 2), (0, 2), (0, 6), (6, 6), (6, 4), (4, 4), (4, 2)]),
+                Polygon([(10, 0), (4, 0), (4, 2), (6, 2), (6, 4), (10, 4), (10, 0)]),
+            ]
+        )
+
+        self.a_identity_b = GeoDataFrame(
+            geometry=[
+                box(4, 2, 6, 4),
+                Polygon([(4, 2), (0, 2), (0, 6), (6, 6), (6, 4), (4, 4), (4, 2)]),
+            ]
+        )
+
+        self.b_identity_a = GeoDataFrame(
+            geometry=[
+                box(4, 2, 6, 4),
+                Polygon([(10, 0), (4, 0), (4, 2), (6, 2), (6, 4), (10, 4), (10, 0)]),
+            ]
+        )
+
+    def test_intersection(self):
+        df_result = overlay(self.layer_a, self.layer_b, how="intersection")
+        assert df_result.geom_equals(self.intersection).all()
+
+    def test_union(self):
+        df_result = overlay(self.layer_a, self.layer_b, how="union")
+        assert_geodataframe_equal(df_result, self.union)
+
+    def test_a_difference_b(self):
+        df_result = overlay(self.layer_a, self.layer_b, how="difference")
+        assert_geodataframe_equal(df_result, self.a_difference_b)
+
+    def test_b_difference_a(self):
+        df_result = overlay(self.layer_b, self.layer_a, how="difference")
+        assert_geodataframe_equal(df_result, self.b_difference_a)
+
+    def test_symmetric_difference(self):
+        df_result = overlay(self.layer_a, self.layer_b, how="symmetric_difference")
+        assert_geodataframe_equal(df_result, self.symmetric_difference)
+
+    def test_a_identity_b(self):
+        df_result = overlay(self.layer_a, self.layer_b, how="identity")
+        assert_geodataframe_equal(df_result, self.a_identity_b)
+
+    def test_b_identity_a(self):
+        df_result = overlay(self.layer_b, self.layer_a, how="identity")
+        assert_geodataframe_equal(df_result, self.b_identity_a)
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_pandas_methods.py` & `geopandas-1.0.0a1/geopandas/tests/test_pandas_methods.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
+from packaging.version import Version
+import warnings
 
 import numpy as np
 from numpy.testing import assert_array_equal
 import pandas as pd
 
 import shapely
-from shapely.geometry import Point, GeometryCollection
+from shapely.geometry import Point, GeometryCollection, LineString, LinearRing
 
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries
 import geopandas._compat as compat
 from geopandas.array import from_shapely
 
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
@@ -35,27 +37,36 @@
 
 def test_repr(s, df):
     assert "POINT" in repr(s)
     assert "POINT" in repr(df)
     assert "POINT" in df._repr_html_()
 
 
+@pytest.mark.skipif(shapely.geos_version < (3, 9, 0), reason="requires GEOS>=3.9")
 def test_repr_boxed_display_precision():
     # geographic coordinates
     p1 = Point(10.123456789, 50.123456789)
     p2 = Point(4.123456789, 20.123456789)
     s1 = GeoSeries([p1, p2, None])
     assert "POINT (10.12346 50.12346)" in repr(s1)
 
+    # geographic coordinates 4326
+    s3 = GeoSeries([p1, p2], crs=4326)
+    assert "POINT (10.12346 50.12346)" in repr(s3)
+
     # projected coordinates
     p1 = Point(3000.123456789, 3000.123456789)
     p2 = Point(4000.123456789, 4000.123456789)
     s2 = GeoSeries([p1, p2, None])
     assert "POINT (3000.123 3000.123)" in repr(s2)
 
+    # projected geographic coordinate
+    s4 = GeoSeries([p1, p2], crs=3857)
+    assert "POINT (3000.123 3000.123)" in repr(s4)
+
     geopandas.options.display_precision = 1
     assert "POINT (10.1 50.1)" in repr(s1)
 
     geopandas.options.display_precision = 9
     assert "POINT (10.123456789 50.123456789)" in repr(s1)
 
 
@@ -67,28 +78,41 @@
     assert "None" in repr(df)
     assert "geometry" in df._repr_html_()
 
 
 def test_repr_empty():
     # https://github.com/geopandas/geopandas/issues/1195
     s = GeoSeries([])
-    if compat.PANDAS_GE_025:
-        # repr with correct name fixed in pandas 0.25
-        assert repr(s) == "GeoSeries([], dtype: geometry)"
-    else:
-        assert repr(s) == "Series([], dtype: geometry)"
+    assert repr(s) == "GeoSeries([], dtype: geometry)"
     df = GeoDataFrame({"a": [], "geometry": s})
     assert "Empty GeoDataFrame" in repr(df)
     # https://github.com/geopandas/geopandas/issues/1184
     assert "geometry" in df._repr_html_()
 
 
-def test_indexing(s, df):
+def test_repr_linearring():
+    # https://github.com/geopandas/geopandas/pull/2689
+    # specifically, checking internal shapely/wkt/wkb conversions
+    # preserve LinearRing
+    s = GeoSeries([LinearRing([(0, 0), (1, 1), (1, -1)])])
+    assert "LINEARRING" in str(s.iloc[0])  # shapely scalar repr
+    assert "LINEARRING" in str(s)  # GeoSeries repr
+
+    # check something coercible to linearring is not converted
+    s2 = GeoSeries(
+        [
+            LineString([(0, 0), (1, 1), (1, -1)]),
+            LineString([(0, 0), (1, 1), (1, -1), (0, 0)]),
+        ]
+    )
+    assert "LINEARRING" not in str(s2)
+
 
-    # accessing scalar from the geometry (colunm)
+def test_indexing(s, df):
+    # accessing scalar from the geometry (column)
     exp = Point(1, 1)
     assert s[1] == exp
     assert s.loc[1] == exp
     assert s.iloc[1] == exp
     assert df.loc[1, "geometry"] == exp
     assert df.iloc[1, 0] == exp
 
@@ -131,16 +155,17 @@
 
     # GeoDataFrame reindex columns
     res = df.reindex(columns=["value1", "geometry"])
     assert isinstance(res, GeoDataFrame)
     assert isinstance(res.geometry, GeoSeries)
     assert_frame_equal(res, df[["value1", "geometry"]])
 
-    # TODO df.reindex(columns=['value1', 'value2']) still returns GeoDataFrame,
-    # should it return DataFrame instead ?
+    res = df.reindex(columns=["value1", "value2"])
+    assert type(res) == pd.DataFrame
+    assert_frame_equal(res, df[["value1", "value2"]])
 
 
 def test_take(s, df):
     inds = np.array([0, 2])
 
     # GeoSeries take
     result = s.take(inds)
@@ -216,32 +241,36 @@
     exp = df.copy()
     exp["new"] = 1
     assert isinstance(res, GeoDataFrame)
     assert_frame_equal(res, exp)
 
 
 def test_astype(s, df):
-
     # check geoseries functionality
     with pytest.raises(TypeError):
         s.astype(int)
 
     assert s.astype(str)[0] == "POINT (0 0)"
 
     res = s.astype(object)
-    assert isinstance(res, pd.Series) and not isinstance(res, GeoSeries)
-    assert res.dtype == object
+    if not (
+        (Version(pd.__version__) == Version("2.1.0"))
+        or (Version(pd.__version__) == Version("2.1.1"))
+    ):
+        # https://github.com/geopandas/geopandas/issues/2948 - bug in pandas 2.1.0
+        assert isinstance(res, pd.Series) and not isinstance(res, GeoSeries)
+        assert res.dtype == object
 
     df = df.rename_geometry("geom_list")
 
     # check whether returned object is a geodataframe
     res = df.astype({"value1": float})
     assert isinstance(res, GeoDataFrame)
 
-    # check whether returned object is a datafrane
+    # check whether returned object is a dataframe
     res = df.astype(str)
     assert isinstance(res, pd.DataFrame) and not isinstance(res, GeoDataFrame)
 
     res = df.astype({"geom_list": str})
     assert isinstance(res, pd.DataFrame) and not isinstance(res, GeoDataFrame)
 
     res = df.astype(object)
@@ -254,27 +283,64 @@
     # a GeoDataFrame without geometry column should not error in astype
     df = GeoDataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
     res = df.astype(object)
     assert isinstance(res, pd.DataFrame) and not isinstance(res, GeoDataFrame)
     assert res["a"].dtype == object
 
 
-def test_to_csv(df):
+def test_convert_dtypes(df):
+    # https://github.com/geopandas/geopandas/issues/1870
 
+    # Test geometry col is first col, first, geom_col_name=geometry
+    # (order is important in concat, used internally)
+    res1 = df.convert_dtypes()
+
+    expected1 = GeoDataFrame(
+        pd.DataFrame(df).convert_dtypes(), crs=df.crs, geometry=df.geometry.name
+    )
+
+    # Checking type and metadata are right
+    assert_geodataframe_equal(expected1, res1)
+
+    # Test geom last, geom_col_name=geometry
+    res2 = df[["value1", "value2", "geometry"]].convert_dtypes()
+    assert_geodataframe_equal(expected1[["value1", "value2", "geometry"]], res2)
+
+    if compat.HAS_PYPROJ:
+        # Test again with crs set and custom geom col name
+        df2 = df.set_crs(epsg=4326).rename_geometry("points")
+        expected2 = GeoDataFrame(
+            pd.DataFrame(df2).convert_dtypes(), crs=df2.crs, geometry=df2.geometry.name
+        )
+        res3 = df2.convert_dtypes()
+        assert_geodataframe_equal(expected2, res3)
+
+        # Test geom last, geom_col=geometry
+        res4 = df2[["value1", "value2", "points"]].convert_dtypes()
+        assert_geodataframe_equal(expected2[["value1", "value2", "points"]], res4)
+
+
+def test_to_csv(df):
     exp = (
         "geometry,value1,value2\nPOINT (0 0),0,1\nPOINT (1 1),1,2\nPOINT (2 2),2,1\n"
     ).replace("\n", os.linesep)
     assert df.to_csv(index=False) == exp
 
 
+@pytest.mark.filterwarnings(
+    "ignore:Dropping of nuisance columns in DataFrame reductions"
+)
 def test_numerical_operations(s, df):
-
     # df methods ignore the geometry column
     exp = pd.Series([3, 4], index=["value1", "value2"])
-    assert_series_equal(df.sum(), exp)
+    if not compat.PANDAS_GE_20:
+        res = df.sum()
+    else:
+        res = df.sum(numeric_only=True)
+    assert_series_equal(res, exp)
 
     # series methods raise error (not supported for geometry)
     with pytest.raises(TypeError):
         s.sum()
 
     with pytest.raises(TypeError):
         s.max()
@@ -283,16 +349,15 @@
         # TODO: remove ValueError after pandas-dev/pandas#32749
         s.idxmax()
 
     # numerical ops raise an error
     with pytest.raises(TypeError):
         df + 1
 
-    with pytest.raises((TypeError, AssertionError)):
-        # TODO(pandas 0.23) remove AssertionError -> raised in 0.23
+    with pytest.raises(TypeError):
         s + 1
 
     # boolean comparisons work
     res = df == 100
     exp = pd.DataFrame(False, index=df.index, columns=df.columns)
     assert_frame_equal(res, exp)
 
@@ -324,40 +389,73 @@
     df2.loc[0, "value1"] = 10
     assert df.equals(df2) is False
 
 
 # Missing values
 
 
-def test_fillna(s, df):
+def test_fillna_scalar(s, df):
     s2 = GeoSeries([Point(0, 0), None, Point(2, 2)])
+
     res = s2.fillna(Point(1, 1))
     assert_geoseries_equal(res, s)
 
     # allow np.nan although this does not change anything
     # https://github.com/geopandas/geopandas/issues/1149
     res = s2.fillna(np.nan)
     assert_geoseries_equal(res, s2)
 
     # raise exception if trying to fill missing geometry w/ non-geometry
     df2 = df.copy()
     df2["geometry"] = s2
     res = df2.fillna(Point(1, 1))
     assert_geodataframe_equal(res, df)
-    with pytest.raises(NotImplementedError):
+    with pytest.raises((NotImplementedError, TypeError)):  # GH2351
         df2.fillna(0)
 
     # allow non-geometry fill value if there are no missing values
     # https://github.com/geopandas/geopandas/issues/1149
     df3 = df.copy()
     df3.loc[0, "value1"] = np.nan
     res = df3.fillna(0)
     assert_geodataframe_equal(res.astype({"value1": "int64"}), df)
 
 
+def test_fillna_series(s):
+    # fill na with another GeoSeries
+    s2 = GeoSeries([Point(0, 0), None, Point(2, 2)])
+
+    # check na filled with the same index
+    res = s2.fillna(GeoSeries([Point(1, 1)] * 3))
+    assert_geoseries_equal(res, s)
+
+    # check na filled based on index, not position
+    index = [3, 2, 1]
+    res = s2.fillna(GeoSeries([Point(i, i) for i in index], index=index))
+    assert_geoseries_equal(res, s)
+
+    # check na filled but the input length is different
+    res = s2.fillna(GeoSeries([Point(1, 1)], index=[1]))
+    assert_geoseries_equal(res, s)
+
+    # check na filled but the inputting index is different
+    res = s2.fillna(GeoSeries([Point(1, 1)], index=[9]))
+    assert_geoseries_equal(res, s2)
+
+
+def test_fillna_inplace(s):
+    s2 = GeoSeries([Point(0, 0), None, Point(2, 2)])
+    arr = s2.array
+    s2.fillna(Point(1, 1), inplace=True)
+    assert_geoseries_equal(s2, s)
+    if compat.PANDAS_GE_21:
+        # starting from pandas 2.1, there is support to do this actually inplace
+        assert s2.array is arr
+
+
 def test_dropna():
     s2 = GeoSeries([Point(0, 0), None, Point(2, 2)])
     res = s2.dropna()
     exp = s2.loc[[0, 2]]
     assert_geoseries_equal(res, exp)
 
 
@@ -393,28 +491,108 @@
     assert not s.all()
     assert not s.any()
 
 
 # Groupby / algos
 
 
+def test_sort_values():
+    s = GeoSeries([Point(0, 0), Point(2, 2), Point(0, 2)])
+    res = s.sort_values()
+    assert res.index.tolist() == [0, 2, 1]
+    res2 = s.sort_values(ascending=False)
+    assert res2.index.tolist() == [1, 2, 0]
+
+    # empty geoseries
+    assert_geoseries_equal(s.iloc[:0].sort_values(), s.iloc[:0])
+
+
+def test_sort_values_empty_missing():
+    s = GeoSeries([Point(0, 0), None, Point(), Point(1, 1)])
+    # default: NA sorts last, empty first
+    res = s.sort_values()
+    assert res.index.tolist() == [2, 0, 3, 1]
+
+    # descending: NA sorts last, empty last
+    res = s.sort_values(ascending=False)
+    assert res.index.tolist() == [3, 0, 2, 1]
+
+    # NAs first, empty first after NAs
+    res = s.sort_values(na_position="first")
+    assert res.index.tolist() == [1, 2, 0, 3]
+
+    # NAs first, descending with empyt last
+    res = s.sort_values(ascending=False, na_position="first")
+    assert res.index.tolist() == [1, 3, 0, 2]
+
+    # all missing / empty
+    s = GeoSeries([None, None, None])
+    res = s.sort_values()
+    assert res.index.tolist() == [0, 1, 2]
+
+    s = GeoSeries([Point(), Point(), Point()])
+    res = s.sort_values()
+    assert res.index.tolist() == [0, 1, 2]
+
+    s = GeoSeries([Point(), None, Point()])
+    res = s.sort_values()
+    assert res.index.tolist() == [0, 2, 1]
+
+
 def test_unique():
     s = GeoSeries([Point(0, 0), Point(0, 0), Point(2, 2)])
     exp = from_shapely([Point(0, 0), Point(2, 2)])
     # TODO should have specialized GeometryArray assert method
     assert_array_equal(s.unique(), exp)
 
 
-@pytest.mark.xfail
+def pd14_compat_index(index):
+    if compat.PANDAS_GE_14:
+        return from_shapely(index)
+    else:
+        return index
+
+
 def test_value_counts():
     # each object is considered unique
     s = GeoSeries([Point(0, 0), Point(1, 1), Point(0, 0)])
     res = s.value_counts()
-    exp = pd.Series([2, 1], index=[Point(0, 0), Point(1, 1)])
+    if compat.PANDAS_GE_20:
+        name = "count"
+    else:
+        name = None
+    exp = pd.Series(
+        [2, 1], index=pd14_compat_index([Point(0, 0), Point(1, 1)]), name=name
+    )
     assert_series_equal(res, exp)
+    # Check crs doesn't make a difference - note it is not kept in output index anyway
+    s2 = GeoSeries([Point(0, 0), Point(1, 1), Point(0, 0)], crs="EPSG:4326")
+    res2 = s2.value_counts()
+    assert_series_equal(res2, exp)
+    if compat.PANDAS_GE_14:
+        # TODO should/ can we fix CRS being lost
+        assert s2.value_counts().index.array.crs is None
+
+    # check mixed geometry
+    s3 = GeoSeries([Point(0, 0), LineString([[1, 1], [2, 2]]), Point(0, 0)])
+    res3 = s3.value_counts()
+    index = pd14_compat_index([Point(0, 0), LineString([[1, 1], [2, 2]])])
+    exp3 = pd.Series([2, 1], index=index, name=name)
+    assert_series_equal(res3, exp3)
+
+    # check None is handled
+    s4 = GeoSeries([Point(0, 0), None, Point(0, 0)])
+    res4 = s4.value_counts(dropna=True)
+    exp4_dropna = pd.Series([2], index=pd14_compat_index([Point(0, 0)]), name=name)
+    assert_series_equal(res4, exp4_dropna)
+    exp4_keepna = pd.Series(
+        [2, 1], index=pd14_compat_index([Point(0, 0), None]), name=name
+    )
+    res4_keepna = s4.value_counts(dropna=False)
+    assert_series_equal(res4_keepna, exp4_keepna)
 
 
 @pytest.mark.xfail(strict=False)
 def test_drop_duplicates_series():
     # duplicated does not yet use EA machinery
     # (https://github.com/pandas-dev/pandas/issues/27264)
     # but relies on unstable hashing of unhashable objects in numpy array
@@ -434,60 +612,112 @@
     dropped_geometry = dup_gdf.drop_duplicates(subset="geometry")
     assert len(dropped_geometry) == 1
     dropped_all = dup_gdf.drop_duplicates()
     assert len(dropped_all) == gdf_len
 
 
 def test_groupby(df):
-
     # counts work fine
     res = df.groupby("value2").count()
     exp = pd.DataFrame(
         {"geometry": [2, 1], "value1": [2, 1], "value2": [1, 2]}
     ).set_index("value2")
     assert_frame_equal(res, exp)
 
     # reductions ignore geometry column
-    res = df.groupby("value2").sum()
+    if not compat.PANDAS_GE_20:
+        res = df.groupby("value2").sum()
+    else:
+        res = df.groupby("value2").sum(numeric_only=True)
     exp = pd.DataFrame({"value1": [2, 1], "value2": [1, 2]}, dtype="int64").set_index(
         "value2"
     )
     assert_frame_equal(res, exp)
 
     # applying on the geometry column
-    res = df.groupby("value2")["geometry"].apply(lambda x: x.cascaded_union)
-    if compat.PANDAS_GE_11:
-        exp = GeoSeries(
-            [shapely.geometry.MultiPoint([(0, 0), (2, 2)]), Point(1, 1)],
-            index=pd.Index([1, 2], name="value2"),
-            name="geometry",
-        )
-    else:
-        exp = pd.Series(
-            [shapely.geometry.MultiPoint([(0, 0), (2, 2)]), Point(1, 1)],
-            index=pd.Index([1, 2], name="value2"),
-            name="geometry",
-        )
+    res = df.groupby("value2")["geometry"].apply(lambda x: x.union_all())
+
+    exp = GeoSeries(
+        [shapely.geometry.MultiPoint([(0, 0), (2, 2)]), Point(1, 1)],
+        index=pd.Index([1, 2], name="value2"),
+        name="geometry",
+    )
     assert_series_equal(res, exp)
 
     # apply on geometry column not resulting in new geometry
-    res = df.groupby("value2")["geometry"].apply(lambda x: x.unary_union.area)
+    res = df.groupby("value2")["geometry"].apply(lambda x: x.union_all().area)
     exp = pd.Series([0.0, 0.0], index=pd.Index([1, 2], name="value2"), name="geometry")
 
     assert_series_equal(res, exp)
 
 
 def test_groupby_groups(df):
     g = df.groupby("value2")
     res = g.get_group(1)
     assert isinstance(res, GeoDataFrame)
     exp = df.loc[[0, 2]]
     assert_frame_equal(res, exp)
 
 
+@pytest.mark.parametrize("crs", [None, "EPSG:4326"])
+@pytest.mark.parametrize("geometry_name", ["geometry", "geom"])
+def test_groupby_metadata(crs, geometry_name):
+    if crs and not compat.HAS_PYPROJ:
+        pytest.skip("requires pyproj")
+    # https://github.com/geopandas/geopandas/issues/2294
+    df = GeoDataFrame(
+        {
+            geometry_name: [Point(0, 0), Point(1, 1), Point(0, 0)],
+            "value1": np.arange(3, dtype="int64"),
+            "value2": np.array([1, 2, 1], dtype="int64"),
+        },
+        crs=crs,
+        geometry=geometry_name,
+    )
+
+    kwargs = {}
+    if compat.PANDAS_GE_22:
+        # pandas is deprecating that the group key is present as column in the
+        # dataframe passed to `func`. To suppress this warning, it introduced
+        # a new include_groups keyword
+        kwargs = dict(include_groups=False)
+
+    # dummy test asserting we can access the crs
+    def func(group):
+        assert isinstance(group, GeoDataFrame)
+        assert group.crs == crs
+
+    df.groupby("value2").apply(func, **kwargs)
+    # selecting the non-group columns -> no need to pass the keyword
+    if (
+        compat.PANDAS_GE_21 if geometry_name == "geometry" else compat.PANDAS_GE_20
+    ) and not compat.PANDAS_GE_22:
+        # https://github.com/geopandas/geopandas/pull/2966#issuecomment-1878816712
+        # with pandas 2.0 and 2.1 this is failing
+        with pytest.raises(AttributeError):
+            df.groupby("value2")[[geometry_name, "value1"]].apply(func)
+    else:
+        df.groupby("value2")[[geometry_name, "value1"]].apply(func)
+
+    # actual test with functionality
+    res = df.groupby("value2").apply(
+        lambda x: geopandas.sjoin(x, x[[geometry_name, "value1"]], how="inner"),
+        **kwargs,
+    )
+
+    expected = (
+        df.take([0, 0, 2, 2, 1])
+        .set_index("value2", drop=compat.PANDAS_GE_22, append=True)
+        .swaplevel()
+        .rename(columns={"value1": "value1_left"})
+        .assign(value1_right=[0, 2, 0, 2, 1])
+    )
+    assert_geodataframe_equal(res.drop(columns=["index_right"]), expected)
+
+
 def test_apply(s):
     # function that returns geometry preserves GeoSeries class
     def geom_func(geom):
         assert isinstance(geom, Point)
         return geom
 
     result = s.apply(geom_func)
@@ -510,52 +740,120 @@
     # https://github.com/geopandas/geopandas/issues/1078
     subset = df.loc[[0], "geometry"]
     result = subset.apply(lambda geom: geom.is_empty)
     expected = subset.is_empty
     np.testing.assert_allclose(result, expected)
 
 
+@pytest.mark.skipif(compat.PANDAS_GE_30, reason="convert_dtype is removed in pandas 3")
 def test_apply_convert_dtypes_keyword(s):
     # ensure the convert_dtypes keyword is accepted
-    res = s.apply(lambda x: x, convert_dtype=True, args=())
+    if not compat.PANDAS_GE_21:
+        recorder = warnings.catch_warnings(record=True)
+    else:
+        recorder = pytest.warns()
+
+    with recorder as record:
+        res = s.apply(lambda x: x, convert_dtype=True, args=())
     assert_geoseries_equal(res, s)
 
+    if compat.PANDAS_GE_21:
+        assert len(record) == 1
+        assert "the convert_dtype parameter" in str(record[0].message)
+    else:
+        assert len(record) == 0
+
 
 @pytest.mark.parametrize("crs", [None, "EPSG:4326"])
 def test_apply_no_geometry_result(df, crs):
     if crs:
+        if not compat.HAS_PYPROJ:
+            pytest.skip("requires pyproj")
         df = df.set_crs(crs)
     result = df.apply(lambda col: col.astype(str), axis=0)
-    # TODO this should actually not return a GeoDataFrame
-    assert isinstance(result, GeoDataFrame)
+    assert type(result) is pd.DataFrame
     expected = df.astype(str)
     assert_frame_equal(result, expected)
 
     result = df.apply(lambda col: col.astype(str), axis=1)
-    assert isinstance(result, GeoDataFrame)
+    assert type(result) is pd.DataFrame
     assert_frame_equal(result, expected)
 
 
-@pytest.mark.skipif(not compat.PANDAS_GE_10, reason="attrs introduced in pandas 1.0")
+def test_apply_preserves_geom_col_name(df):
+    df = df.rename_geometry("geom")
+    result = df.apply(lambda col: col, axis=0)
+    assert result.geometry.name == "geom"
+
+
+def test_df_apply_returning_series(df):
+    # https://github.com/geopandas/geopandas/issues/2283
+    result = df.apply(lambda row: row.geometry, axis=1)
+    assert_geoseries_equal(result, df.geometry, check_crs=False)
+
+    result = df.apply(lambda row: row.value1, axis=1)
+    assert_series_equal(result, df["value1"].rename(None))
+    # https://github.com/geopandas/geopandas/issues/2480
+    result = df.apply(lambda x: float("NaN"), axis=1)
+    assert result.dtype == "float64"
+    # assert list of nones is not promoted to GeometryDtype
+    result = df.apply(lambda x: None, axis=1)
+    assert result.dtype == "object"
+
+    # https://github.com/geopandas/geopandas/issues/2889
+    # contrived case such that `from_shapely` receives an array of geodataframes
+    res = df.apply(lambda row: df.geometry.to_frame(), axis=1)
+    assert res.dtype == "object"
+
+
+def test_df_apply_geometry_dtypes(df):
+    # https://github.com/geopandas/geopandas/issues/1852
+    apply_types = []
+
+    def get_dtypes(srs):
+        apply_types.append((srs.name, type(srs)))
+
+    df["geom2"] = df.geometry
+    df.apply(get_dtypes)
+    expected = [
+        ("geometry", GeoSeries),
+        ("value1", pd.Series),
+        ("value2", pd.Series),
+        ("geom2", GeoSeries),
+    ]
+    assert apply_types == expected
+
+
+def test_pivot(df):
+    # https://github.com/geopandas/geopandas/issues/2057
+    # pivot failing due to creating a MultiIndex
+    result = df.pivot(columns="value1")
+    expected = GeoDataFrame(pd.DataFrame(df).pivot(columns="value1"))
+    assert_geodataframe_equal(result, expected)
+
+
 def test_preserve_attrs(df):
     # https://github.com/geopandas/geopandas/issues/1654
     df.attrs["name"] = "my_name"
     attrs = {"name": "my_name"}
     assert df.attrs == attrs
 
     # preserve attrs in indexing operations
     for subset in [df[:2], df[df["value1"] > 2], df[["value2", "geometry"]]]:
         assert df.attrs == attrs
 
     # preserve attrs in methods
     df2 = df.reset_index()
     assert df2.attrs == attrs
 
+    # https://github.com/geopandas/geopandas/issues/1875
+    df3 = df2.explode(index_parts=True)
+    assert df3.attrs == attrs
+
 
-@pytest.mark.skipif(not compat.PANDAS_GE_12, reason="attrs introduced in pandas 1.0")
 def test_preserve_flags(df):
     # https://github.com/geopandas/geopandas/issues/1654
     df = df.set_flags(allows_duplicate_labels=False)
     assert df.flags.allows_duplicate_labels is False
 
     # preserve flags in indexing operations
     for subset in [df[:2], df[df["value1"] > 2], df[["value2", "geometry"]]]:
@@ -570,7 +868,21 @@
         df.reindex([0, 0, 1])
 
     with pytest.raises(ValueError):
         df[["value1", "value1", "geometry"]]
 
     with pytest.raises(ValueError):
         pd.concat([df, df])
+
+
+def test_ufunc():
+    # this is calling a shapely ufunc, but we currently rely on pandas' implementation
+    # of `__array_ufunc__` to wrap the result back into a GeoSeries
+    ser = GeoSeries([Point(1, 1), Point(2, 2), Point(3, 3)])
+    result = shapely.buffer(ser, 2)
+    assert isinstance(result, GeoSeries)
+
+    # ensure the result is still writeable
+    # (https://github.com/geopandas/geopandas/issues/3178)
+    assert result.array._data.flags.writeable
+    result.loc[0] = Point(10, 10)
+    assert result.iloc[0] == Point(10, 10)
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_plotting.py` & `geopandas-1.0.0a1/geopandas/tests/test_plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from distutils.version import LooseVersion
 import itertools
+from packaging.version import Version
 import warnings
 
 import numpy as np
 import pandas as pd
 
-from shapely import wkt
 from shapely.affinity import rotate
 from shapely.geometry import (
     MultiPolygon,
     Polygon,
     LineString,
     LinearRing,
     Point,
     MultiPoint,
     MultiLineString,
     GeometryCollection,
+    box,
 )
 
 
 from geopandas import GeoDataFrame, GeoSeries, read_file
-from geopandas.datasets import get_path
 import geopandas._compat as compat
+from geopandas.plotting import GeoplotAccessor
 
 import pytest
 
 matplotlib = pytest.importorskip("matplotlib")
 matplotlib.use("Agg")
-import matplotlib.pyplot as plt  # noqa
+import matplotlib.pyplot as plt
 
 try:  # skipif and importorskip do not work for decorators
     from matplotlib.testing.decorators import check_figures_equal
 
     MPL_DECORATORS = True
 except ImportError:
     MPL_DECORATORS = False
@@ -65,23 +65,21 @@
         multipoint1 = MultiPoint(self.points)
         multipoint2 = rotate(multipoint1, 90)
         self.df2 = GeoDataFrame(
             {"geometry": [multipoint1, multipoint2], "values": [0, 1]}
         )
 
     def test_figsize(self):
-
         ax = self.points.plot(figsize=(1, 1))
         np.testing.assert_array_equal(ax.figure.get_size_inches(), (1, 1))
 
         ax = self.df.plot(figsize=(1, 1))
         np.testing.assert_array_equal(ax.figure.get_size_inches(), (1, 1))
 
     def test_default_colors(self):
-
         # # without specifying values -> uniform color
 
         # GeoSeries
         ax = self.points.plot()
         _check_colors(
             self.N, ax.collections[0].get_facecolors(), [MPL_DFT_COLOR] * self.N
         )
@@ -95,15 +93,14 @@
         # # with specifying values -> different colors for all 10 values
         ax = self.df.plot(column="values")
         cmap = plt.get_cmap()
         expected_colors = cmap(np.arange(self.N) / (self.N - 1))
         _check_colors(self.N, ax.collections[0].get_facecolors(), expected_colors)
 
     def test_series_color_no_index(self):
-
         # Color order with ordered index
         colors_ord = pd.Series(["a", "b", "c", "a", "b", "c", "a", "b", "c", "a"])
 
         # Plot using Series as color
         ax1 = self.df.plot(colors_ord)
 
         # Correct answer: Add as column to df and plot
@@ -112,15 +109,14 @@
 
         # Confirm out-of-order index re-sorted
         point_colors1 = ax1.collections[0].get_facecolors()
         point_colors2 = ax2.collections[0].get_facecolors()
         np.testing.assert_array_equal(point_colors1[1], point_colors2[1])
 
     def test_series_color_index(self):
-
         # Color order with out-of-order index
         colors_ord = pd.Series(
             ["a", "a", "a", "a", "b", "b", "b", "c", "c", "c"],
             index=[0, 3, 6, 9, 1, 4, 7, 2, 5, 8],
         )
 
         # Plot using Series as color
@@ -132,15 +128,14 @@
 
         # Confirm out-of-order index re-sorted
         point_colors1 = ax1.collections[0].get_facecolors()
         point_colors2 = ax2.collections[0].get_facecolors()
         np.testing.assert_array_equal(point_colors1[1], point_colors2[1])
 
     def test_colormap(self):
-
         # without specifying values but cmap specified -> no uniform color
         # but different colors for all points
 
         # GeoSeries
         ax = self.points.plot(cmap="RdYlGn")
         cmap = plt.get_cmap("RdYlGn")
         exp_colors = cmap(np.arange(self.N) / (self.N - 1))
@@ -158,15 +153,14 @@
         # colors
         ax = self.points.plot(cmap=plt.get_cmap("Set1", lut=5))
         cmap = plt.get_cmap("Set1", lut=5)
         exp_colors = cmap(list(range(5)) * 2)
         _check_colors(self.N, ax.collections[0].get_facecolors(), exp_colors)
 
     def test_single_color(self):
-
         ax = self.points.plot(color="green")
         _check_colors(self.N, ax.collections[0].get_facecolors(), ["green"] * self.N)
 
         ax = self.df.plot(color="green")
         _check_colors(self.N, ax.collections[0].get_facecolors(), ["green"] * self.N)
 
         # check rgba tuple GH1178
@@ -185,15 +179,14 @@
             # 'color' overrides 'column'
             ax = self.df.plot(column="values", color="green")
             _check_colors(
                 self.N, ax.collections[0].get_facecolors(), ["green"] * self.N
             )
 
     def test_markersize(self):
-
         ax = self.points.plot(markersize=10)
         assert ax.collections[0].get_sizes() == [10]
 
         ax = self.df.plot(markersize=10)
         assert ax.collections[0].get_sizes() == [10]
 
         ax = self.df.plot(column="values", markersize=10)
@@ -209,15 +202,14 @@
         ax = self.df2.plot(marker="+")
         expected = _style_to_vertices("+")
         np.testing.assert_array_equal(
             expected, ax.collections[0].get_paths()[0].vertices
         )
 
     def test_style_kwargs(self):
-
         ax = self.points.plot(edgecolors="k")
         assert (ax.collections[0].get_edgecolor() == [0, 0, 0, 1]).all()
 
     def test_style_kwargs_alpha(self):
         ax = self.df.plot(alpha=0.7)
         np.testing.assert_array_equal([0.7], ax.collections[0].get_alpha())
         try:
@@ -226,14 +218,21 @@
             # no list allowed for alpha up to matplotlib 3.3
             pass
         else:
             np.testing.assert_array_equal(
                 np.linspace(0, 0.0, 1.0, self.N), ax.collections[0].get_alpha()
             )
 
+    # TODO temporary skip for mpl 3.8.0.dev
+    # (https://github.com/matplotlib/matplotlib/issues/25162)
+    @pytest.mark.skipif(
+        Version(matplotlib.__version__) >= Version("3.8.0.dev")
+        and Version(matplotlib.__version__) < Version("3.8.0"),
+        reason="failing with matplotlib dev",
+    )
     def test_legend(self):
         with warnings.catch_warnings(record=True) as _:  # don't print warning
             # legend ignored if color is given.
             ax = self.df.plot(column="values", color="green", legend=True)
             assert len(ax.get_figure().axes) == 1  # no separate legend axis
 
         # legend ignored if no column is given.
@@ -285,56 +284,82 @@
         np.testing.assert_array_equal(exp_colors, actual_colors_orig)
         fig, ax = plt.subplots()
         self.df[1:].plot(column="values", ax=ax, norm=norm, cmap=cmap)
         actual_colors_sub = ax.collections[0].get_facecolors()
         np.testing.assert_array_equal(actual_colors_orig[1], actual_colors_sub[0])
 
     def test_empty_plot(self):
-
         s = GeoSeries([Polygon()])
         with pytest.warns(UserWarning):
             ax = s.plot()
         assert len(ax.collections) == 0
         s = GeoSeries([])
         with pytest.warns(UserWarning):
             ax = s.plot()
         assert len(ax.collections) == 0
-        df = GeoDataFrame([])
+        df = GeoDataFrame([], columns=["geometry"])
         with pytest.warns(UserWarning):
             ax = df.plot()
         assert len(ax.collections) == 0
 
     def test_empty_geometry(self):
-
-        if compat.USE_PYGEOS:
-            s = GeoSeries([wkt.loads("POLYGON EMPTY")])
-            s = GeoSeries(
-                [Polygon([(0, 0), (1, 0), (1, 1)]), wkt.loads("POLYGON EMPTY")]
-            )
-            ax = s.plot()
-            assert len(ax.collections) == 1
-        if not compat.USE_PYGEOS:
-            s = GeoSeries([Polygon([(0, 0), (1, 0), (1, 1)]), Polygon()])
-            ax = s.plot()
-            assert len(ax.collections) == 1
+        s = GeoSeries([Polygon([(0, 0), (1, 0), (1, 1)]), Polygon()])
+        ax = s.plot()
+        assert len(ax.collections) == 1
 
         # more complex case with GEOMETRYCOLLECTION EMPTY, POINT EMPTY and NONE
         poly = Polygon([(-1, -1), (-1, 2), (2, 2), (2, -1), (-1, -1)])
         point = Point(0, 1)
         point_ = Point(10, 10)
         empty_point = Point()
 
         gdf = GeoDataFrame(geometry=[point, empty_point, point_])
         gdf["geometry"] = gdf.intersection(poly)
-        gdf.loc[3] = [None]
+        with warnings.catch_warnings():
+            # loc to add row calls concat internally, warning for pandas >=2.1
+            warnings.filterwarnings(
+                "ignore",
+                "The behavior of DataFrame concatenation with empty",
+                FutureWarning,
+            )
+            gdf.loc[3] = [None]
         ax = gdf.plot()
         assert len(ax.collections) == 1
 
-    def test_multipoints(self):
+    @pytest.mark.parametrize(
+        "geoms",
+        [
+            [
+                box(0, 0, 1, 1),
+                box(7, 7, 8, 8),
+            ],
+            [
+                LineString([(1, 1), (1, 2)]),
+                LineString([(7, 1), (7, 2)]),
+            ],
+            [
+                Point(1, 1),
+                Point(7, 7),
+            ],
+        ],
+    )
+    def test_empty_geometry_colors(self, geoms):
+        s = GeoSeries(
+            geoms,
+            index=["r", "b"],
+        )
+        s2 = s.intersection(box(5, 0, 10, 10))
+        ax = s2.plot(color=["red", "blue"])
+        blue = np.array([0.0, 0.0, 1.0, 1.0])
+        if s.geom_type["r"] == "LineString":
+            np.testing.assert_array_equal(ax.get_children()[0].get_edgecolor()[0], blue)
+        else:
+            np.testing.assert_array_equal(ax.get_children()[0].get_facecolor()[0], blue)
 
+    def test_multipoints(self):
         # MultiPoints
         ax = self.df2.plot()
         _check_colors(4, ax.collections[0].get_facecolors(), [MPL_DFT_COLOR] * 4)
 
         ax = self.df2.plot(column="values")
         cmap = plt.get_cmap(lut=2)
         expected_colors = [cmap(0)] * self.N + [cmap(1)] * self.N
@@ -364,29 +389,35 @@
         self.df["cats"] = pd.Categorical(["cat1", "cat2"] * 5)
         self.df["singlecat"] = pd.Categorical(
             ["cat2"] * 10, categories=["cat1", "cat2"]
         )
         self.df["cats_ordered"] = pd.Categorical(
             ["cat2", "cat1"] * 5, categories=["cat2", "cat1"]
         )
+        self.df["bool"] = [False, True] * 5
+        self.df["bool_extension"] = pd.array([False, True] * 5)
+        self.df["cats_string"] = pd.array(["cat1", "cat2"] * 5, dtype="string")
 
         ax1 = self.df.plot("cats_object", legend=True)
         ax2 = self.df.plot("cats", legend=True)
         ax3 = self.df.plot("singlecat_object", categories=["cat1", "cat2"], legend=True)
         ax4 = self.df.plot("singlecat", legend=True)
         ax5 = self.df.plot("cats_ordered", legend=True)
         ax6 = self.df.plot("nums", categories=[1, 2], legend=True)
+        ax7 = self.df.plot("bool", legend=True)
+        ax8 = self.df.plot("bool_extension", legend=True)
+        ax9 = self.df.plot("cats_string", legend=True)
 
         point_colors1 = ax1.collections[0].get_facecolors()
-        for ax in [ax2, ax3, ax4, ax5, ax6]:
+        for ax in [ax2, ax3, ax4, ax5, ax6, ax7, ax8, ax9]:
             point_colors2 = ax.collections[0].get_facecolors()
             np.testing.assert_array_equal(point_colors1[1], point_colors2[1])
 
         legend1 = [x.get_markerfacecolor() for x in ax1.get_legend().get_lines()]
-        for ax in [ax2, ax3, ax4, ax5, ax6]:
+        for ax in [ax2, ax3, ax4, ax5, ax6, ax7, ax8, ax9]:
             legend2 = [x.get_markerfacecolor() for x in ax.get_legend().get_lines()]
             np.testing.assert_array_equal(legend1, legend2)
 
         with pytest.raises(TypeError):
             self.df.plot(column="cats_object", categories="non_list")
 
         with pytest.raises(
@@ -395,15 +426,15 @@
             self.df.plot(column="cats_object", categories=["cat1"])
 
         with pytest.raises(
             ValueError, match="Cannot specify 'categories' when column has"
         ):
             self.df.plot(column="cats", categories=["cat1"])
 
-    def test_misssing(self):
+    def test_missing(self):
         self.df.loc[0, "values"] = np.nan
         ax = self.df.plot("values")
         cmap = plt.get_cmap()
         expected_colors = cmap(np.arange(self.N - 1) / (self.N - 2))
         _check_colors(self.N - 1, ax.collections[0].get_facecolors(), expected_colors)
 
         ax = self.df.plot("values", missing_kwds={"color": "r"})
@@ -419,14 +450,20 @@
         point_colors = ax.collections[0].get_facecolors()
         nan_color = ax.collections[1].get_facecolors()
         leg_colors = ax.get_legend().axes.collections[0].get_facecolors()
         leg_colors1 = ax.get_legend().axes.collections[1].get_facecolors()
         np.testing.assert_array_equal(point_colors[0], leg_colors[0])
         np.testing.assert_array_equal(nan_color[0], leg_colors1[0])
 
+    def test_no_missing_and_missing_kwds(self):
+        # GH2210
+        df = self.df.copy()
+        df["category"] = df["values"].astype("str")
+        df.plot("category", missing_kwds={"facecolor": "none"}, legend=True)
+
 
 class TestPointZPlotting:
     def setup_method(self):
         self.N = 10
         self.points = GeoSeries(Point(i, i, i) for i in range(self.N))
         values = np.arange(self.N)
         self.df = GeoDataFrame({"geometry": self.points, "values": values})
@@ -455,15 +492,14 @@
         self.linearrings = GeoSeries(
             [LinearRing([(0, i), (4, i + 0.5), (9, i)]) for i in range(self.N)],
             index=list("ABCDEFGHIJ"),
         )
         self.df3 = GeoDataFrame({"geometry": self.linearrings, "values": values})
 
     def test_single_color(self):
-
         ax = self.lines.plot(color="green")
         _check_colors(self.N, ax.collections[0].get_colors(), ["green"] * self.N)
 
         ax = self.df.plot(color="green")
         _check_colors(self.N, ax.collections[0].get_colors(), ["green"] * self.N)
 
         ax = self.linearrings.plot(color="green")
@@ -507,15 +543,15 @@
         exp_ls = [_style_to_linestring_onoffseq(st, 1) for st in ls]
         for ax in [
             self.lines.plot(linestyle=ls, linewidth=1),
             self.lines.plot(linestyles=ls, linewidth=1),
             self.df.plot(linestyle=ls, linewidth=1),
             self.df.plot(column="values", linestyle=ls, linewidth=1),
         ]:
-            np.testing.assert_array_equal(exp_ls, ax.collections[0].get_linestyle())
+            assert exp_ls == ax.collections[0].get_linestyle()
 
     def test_style_kwargs_linewidth(self):
         # single
         for ax in [
             self.lines.plot(linewidth=2),
             self.df.plot(linewidth=2),
             self.df.plot(column="values", linewidth=2),
@@ -541,29 +577,38 @@
             # no list allowed for alpha up to matplotlib 3.3
             pass
         else:
             np.testing.assert_array_equal(
                 np.linspace(0, 0.0, 1.0, self.N), ax.collections[0].get_alpha()
             )
 
+    def test_style_kwargs_path_effects(self):
+        from matplotlib.patheffects import withStroke
+
+        effects = [withStroke(linewidth=8, foreground="b")]
+        ax = self.df.plot(color="orange", path_effects=effects)
+        assert ax.collections[0].get_path_effects()[0].__dict__["_gc"] == {
+            "linewidth": 8,
+            "foreground": "b",
+        }
+
     def test_subplots_norm(self):
         # colors of subplots are the same as for plot (norm is applied)
         cmap = matplotlib.cm.viridis_r
         norm = matplotlib.colors.Normalize(vmin=0, vmax=20)
         ax = self.df.plot(column="values", cmap=cmap, norm=norm)
         actual_colors_orig = ax.collections[0].get_edgecolors()
         exp_colors = cmap(np.arange(10) / (20))
         np.testing.assert_array_equal(exp_colors, actual_colors_orig)
         fig, ax = plt.subplots()
         self.df[1:].plot(column="values", ax=ax, norm=norm, cmap=cmap)
         actual_colors_sub = ax.collections[0].get_edgecolors()
         np.testing.assert_array_equal(actual_colors_orig[1], actual_colors_sub[0])
 
     def test_multilinestrings(self):
-
         # MultiLineStrings
         ax = self.df2.plot()
         assert len(ax.collections[0].get_paths()) == 4
         _check_colors(4, ax.collections[0].get_edgecolors(), [MPL_DFT_COLOR] * 4)
 
         ax = self.df2.plot("values")
         cmap = plt.get_cmap(lut=2)
@@ -574,32 +619,30 @@
         ax = self.df2.plot(color=["r", "b"])
         # colors are repeated for all components within a MultiLineString
         _check_colors(4, ax.collections[0].get_edgecolors(), ["r", "r", "b", "b"])
 
 
 class TestPolygonPlotting:
     def setup_method(self):
-
         t1 = Polygon([(0, 0), (1, 0), (1, 1)])
         t2 = Polygon([(1, 0), (2, 0), (2, 1)])
         self.polys = GeoSeries([t1, t2], index=list("AB"))
         self.df = GeoDataFrame({"geometry": self.polys, "values": [0, 1]})
 
         multipoly1 = MultiPolygon([t1, t2])
         multipoly2 = rotate(multipoly1, 180)
         self.df2 = GeoDataFrame(
             {"geometry": [multipoly1, multipoly2], "values": [0, 1]}
         )
 
         t3 = Polygon([(2, 0), (3, 0), (3, 1)])
         df_nan = GeoDataFrame({"geometry": t3, "values": [np.nan]})
-        self.df3 = self.df.append(df_nan)
+        self.df3 = pd.concat([self.df, df_nan])
 
     def test_single_color(self):
-
         ax = self.polys.plot(color="green")
         _check_colors(2, ax.collections[0].get_facecolors(), ["green"] * 2)
         # color only sets facecolor
         assert len(ax.collections[0].get_edgecolors()) == 0
 
         ax = self.df.plot(color="green")
         _check_colors(2, ax.collections[0].get_facecolors(), ["green"] * 2)
@@ -633,15 +676,14 @@
 
         # vmin vmax set correctly for array with NaN (GitHub issue 877)
         ax = self.df3.plot(column="values")
         actual_colors = ax.collections[0].get_facecolors()
         assert np.any(np.not_equal(actual_colors[0], actual_colors[1]))
 
     def test_style_kwargs_color(self):
-
         # facecolor overrides default cmap when color is not set
         ax = self.polys.plot(facecolor="k")
         _check_colors(2, ax.collections[0].get_facecolors(), ["k"] * 2)
 
         # facecolor overrides more general-purpose color when both are set
         ax = self.polys.plot(color="red", facecolor="k")
         # TODO with new implementation, color overrides facecolor
@@ -708,21 +750,28 @@
         except TypeError:
             # no list allowed for alpha up to matplotlib 3.3
             pass
         else:
             np.testing.assert_array_equal([0.7, 0.2], ax.collections[0].get_alpha())
 
     def test_legend_kwargs(self):
-
+        categories = list(self.df["values"].unique())
+        prefix = "LABEL_FOR_"
         ax = self.df.plot(
             column="values",
             categorical=True,
+            categories=categories,
             legend=True,
-            legend_kwds={"frameon": False},
+            legend_kwds={
+                "labels": [prefix + str(c) for c in categories],
+                "frameon": False,
+            },
         )
+        assert len(categories) == len(ax.get_legend().get_texts())
+        assert ax.get_legend().get_texts()[0].get_text().startswith(prefix)
         assert ax.get_legend().get_frame_on() is False
 
     def test_colorbar_kwargs(self):
         # Test if kwargs are passed to colorbar
 
         label_txt = "colorbar test"
 
@@ -755,15 +804,14 @@
             legend=True,
             legend_kwds={"fmt": "{:.0f}"},
         )
 
         self.df.plot(column="values", legend=True, legend_kwds={"fmt": "{:.0f}"})
 
     def test_multipolygons_color(self):
-
         # MultiPolygons
         ax = self.df2.plot()
         assert len(ax.collections[0].get_paths()) == 4
         _check_colors(4, ax.collections[0].get_facecolors(), [MPL_DFT_COLOR] * 4)
 
         ax = self.df2.plot("values")
         cmap = plt.get_cmap(lut=2)
@@ -829,15 +877,14 @@
         self.df[1:].plot(column="values", ax=ax, norm=norm, cmap=cmap)
         actual_colors_sub = ax.collections[0].get_facecolors()
         np.testing.assert_array_equal(actual_colors_orig[1], actual_colors_sub[0])
 
 
 class TestPolygonZPlotting:
     def setup_method(self):
-
         t1 = Polygon([(0, 0, 0), (1, 0, 0), (1, 1, 1)])
         t2 = Polygon([(1, 0, 0), (2, 0, 0), (2, 1, 1)])
         self.polys = GeoSeries([t1, t2], index=list("AB"))
         self.df = GeoDataFrame({"geometry": self.polys, "values": [0, 1]})
 
         multipoly1 = MultiPolygon([t1, t2])
         multipoly2 = rotate(multipoly1, 180)
@@ -846,14 +893,55 @@
         )
 
     def test_plot(self):
         # basic test that points with z coords don't break plotting
         self.df.plot()
 
 
+class TestColorParamArray:
+    def setup_method(self):
+        geom = []
+        color = []
+        for a, b in [(0, 2), (4, 6)]:
+            b = box(a, a, b, b)
+            geom += [b, b.buffer(0.8).exterior, b.centroid]
+            color += ["red", "green", "blue"]
+
+        self.gdf = GeoDataFrame({"geometry": geom, "color_rgba": color})
+        self.mgdf = self.gdf.dissolve(self.gdf.geom_type)
+
+    def test_color_single(self):
+        ax = self.gdf.plot(color=self.gdf["color_rgba"])
+
+        _check_colors(
+            4,
+            np.concatenate([c.get_edgecolor() for c in ax.collections]),
+            ["green"] * 2 + ["blue"] * 2,
+        )
+        _check_colors(
+            4,
+            np.concatenate([c.get_facecolor() for c in ax.collections]),
+            ["red"] * 2 + ["blue"] * 2,
+        )
+
+    def test_color_multi(self):
+        ax = self.mgdf.plot(color=self.mgdf["color_rgba"])
+
+        _check_colors(
+            4,
+            np.concatenate([c.get_edgecolor() for c in ax.collections]),
+            ["green"] * 2 + ["blue"] * 2,
+        )
+        _check_colors(
+            4,
+            np.concatenate([c.get_facecolor() for c in ax.collections]),
+            ["red"] * 2 + ["blue"] * 2,
+        )
+
+
 class TestGeometryCollectionPlotting:
     def setup_method(self):
         coll1 = GeometryCollection(
             [
                 Polygon([(1, 0), (2, 0), (2, 1)]),
                 MultiLineString([((0.5, 0.5), (1, 1)), ((1, 0.5), (1.5, 1))]),
             ]
@@ -885,15 +973,15 @@
             2, ax.collections[1].get_edgecolors(), [exp_colors[0]] * 2
         )  # line
         _check_colors(1, ax.collections[2].get_facecolors(), [exp_colors[1]])  # point
 
 
 class TestNonuniformGeometryPlotting:
     def setup_method(self):
-        pytest.importorskip("matplotlib", "1.5.0")
+        pytest.importorskip("matplotlib")
 
         poly = Polygon([(1, 0), (2, 0), (2, 1)])
         line = LineString([(0.5, 0.5), (1, 1), (1, 0.5), (1.5, 1)])
         point = Point(0.75, 0.25)
         self.series = GeoSeries([poly, line, point])
         self.df = GeoDataFrame({"geometry": self.series, "values": [1, 2, 3]})
 
@@ -938,15 +1026,15 @@
         ls = ["solid", "dotted", "dashdot"]
         exp_ls = [_style_to_linestring_onoffseq(style, 1) for style in ls]
         for ax in [
             self.series.plot(linestyle=ls, linewidth=1),
             self.series.plot(linestyles=ls, linewidth=1),
             self.df.plot(linestyles=ls, linewidth=1),
         ]:
-            np.testing.assert_array_equal(exp_ls, ax.collections[0].get_linestyle())
+            assert exp_ls == ax.collections[0].get_linestyle()
 
     def test_style_kwargs_linewidth(self):
         # single
         ax = self.df.plot(linewidth=2)
         np.testing.assert_array_equal([2], ax.collections[0].get_linewidths())
 
     @pytest.mark.skip(
@@ -975,24 +1063,28 @@
         #     pass
         # else:
         #     np.testing.assert_array_equal(
         #         [0.7, 0.2, 0.9], ax.collections[0].get_alpha()
         #     )
 
 
-class TestGeographicAspect:
-    def setup_class(self):
-        pth = get_path("naturalearth_lowres")
-        df = read_file(pth)
-        self.north = df.loc[df.continent == "North America"]
-        self.north_proj = self.north.to_crs("ESRI:102008")
-        bounds = self.north.total_bounds
-        y_coord = np.mean([bounds[1], bounds[3]])
-        self.exp = 1 / np.cos(y_coord * np.pi / 180)
+@pytest.fixture(scope="class")
+def _setup_class_geographic_aspect(naturalearth_lowres, request):
+    """Attach naturalearth_lowres class attribute for unittest style setup_method"""
+    df = read_file(naturalearth_lowres)
+    request.cls.north = df.loc[df.continent == "North America"]
+    request.cls.north_proj = request.cls.north.to_crs("ESRI:102008")
+    bounds = request.cls.north.total_bounds
+    y_coord = np.mean([bounds[1], bounds[3]])
+    request.cls.exp = 1 / np.cos(y_coord * np.pi / 180)
+
 
+@pytest.mark.usefixtures("_setup_class_geographic_aspect")
+@pytest.mark.skipif(not compat.HAS_PYPROJ, reason="pyproj not available")
+class TestGeographicAspect:
     def test_auto(self):
         ax = self.north.geometry.plot()
         assert ax.get_aspect() == self.exp
         ax2 = self.north_proj.geometry.plot()
         assert ax2.get_aspect() in ["equal", 1.0]
         ax = self.north.plot()
         assert ax.get_aspect() == self.exp
@@ -1038,184 +1130,344 @@
         assert ax2.get_aspect() == 0.5
         ax3 = self.north_proj.plot("pop_est", aspect=0.5)
         assert ax3.get_aspect() == 0.5
         self.north_proj.plot("pop_est", ax=ax3, aspect=None)
         assert ax3.get_aspect() == 0.5
 
 
+@pytest.mark.filterwarnings(
+    "ignore:Numba not installed. Using slow pure python version.:UserWarning"
+)
 class TestMapclassifyPlotting:
     @classmethod
     def setup_class(cls):
         try:
-            import mapclassify  # noqa
+            import mapclassify
         except ImportError:
             pytest.importorskip("mapclassify")
+        cls.mc = mapclassify
         cls.classifiers = list(mapclassify.classifiers.CLASSIFIERS)
         cls.classifiers.remove("UserDefined")
-        pth = get_path("naturalearth_lowres")
-        cls.df = read_file(pth)
-        cls.df["NEGATIVES"] = np.linspace(-10, 10, len(cls.df.index))
 
-    def test_legend(self):
+    @pytest.fixture
+    def df(self, naturalearth_lowres):
+        # version of naturalearth_lowres for mapclassify plotting tests
+        df = read_file(naturalearth_lowres)
+        df["NEGATIVES"] = np.linspace(-10, 10, len(df.index))
+        df["low_vals"] = np.linspace(0, 0.3, df.shape[0])
+        df["mid_vals"] = np.linspace(0.3, 0.7, df.shape[0])
+        df["high_vals"] = np.linspace(0.7, 1.0, df.shape[0])
+        df.loc[df.index[:20:2], "high_vals"] = np.nan
+        return df
+
+    @pytest.fixture
+    def nybb(self, nybb_filename):
+        # version of nybb for mapclassify plotting tests
+        df = read_file(nybb_filename)
+        df["vals"] = [0.001, 0.002, 0.003, 0.004, 0.005]
+        return df
+
+    def test_legend(self, df):
         with warnings.catch_warnings(record=True) as _:  # don't print warning
             # warning coming from scipy.stats
-            ax = self.df.plot(
+            ax = df.plot(
                 column="pop_est", scheme="QUANTILES", k=3, cmap="OrRd", legend=True
             )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
         expected = [
-            u"       140.00,    5217064.00",
-            u"   5217064.00,   19532732.33",
-            u"  19532732.33, 1379302771.00",
+            s.split("|")[0][1:-2]
+            for s in str(self.mc.Quantiles(df["pop_est"], k=3)).split("\n")[4:]
         ]
         assert labels == expected
 
-    def test_bin_labels(self):
-        ax = self.df.plot(
+    def test_bin_labels(self, df):
+        ax = df.plot(
             column="pop_est",
             scheme="QUANTILES",
             k=3,
             cmap="OrRd",
             legend=True,
             legend_kwds={"labels": ["foo", "bar", "baz"]},
         )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
         expected = ["foo", "bar", "baz"]
         assert labels == expected
 
-    def test_invalid_labels_length(self):
+    def test_invalid_labels_length(self, df):
         with pytest.raises(ValueError):
-            self.df.plot(
+            df.plot(
                 column="pop_est",
                 scheme="QUANTILES",
                 k=3,
                 cmap="OrRd",
                 legend=True,
                 legend_kwds={"labels": ["foo", "bar"]},
             )
 
-    def test_negative_legend(self):
-        ax = self.df.plot(
+    def test_negative_legend(self, df):
+        ax = df.plot(
             column="NEGATIVES", scheme="FISHER_JENKS", k=3, cmap="OrRd", legend=True
         )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
-        expected = [u"-10.00,  -3.41", u" -3.41,   3.30", u"  3.30,  10.00"]
+        expected = ["-10.00,  -3.41", " -3.41,   3.30", "  3.30,  10.00"]
         assert labels == expected
 
-    def test_fmt(self):
-        ax = self.df.plot(
+    def test_fmt(self, df):
+        ax = df.plot(
             column="NEGATIVES",
             scheme="FISHER_JENKS",
             k=3,
             cmap="OrRd",
             legend=True,
             legend_kwds={"fmt": "{:.0f}"},
         )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
-        expected = [u"-10,  -3", u" -3,   3", u"  3,  10"]
+        expected = ["-10,  -3", " -3,   3", "  3,  10"]
         assert labels == expected
 
-    def test_interval(self):
-        ax = self.df.plot(
+    def test_interval(self, df):
+        ax = df.plot(
             column="NEGATIVES",
             scheme="FISHER_JENKS",
             k=3,
             cmap="OrRd",
             legend=True,
             legend_kwds={"interval": True},
         )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
-        expected = [u"[-10.00,  -3.41]", u"( -3.41,   3.30]", u"(  3.30,  10.00]"]
+        expected = ["[-10.00,  -3.41]", "( -3.41,   3.30]", "(  3.30,  10.00]"]
         assert labels == expected
 
     @pytest.mark.parametrize("scheme", ["FISHER_JENKS", "FISHERJENKS"])
-    def test_scheme_name_compat(self, scheme):
-        ax = self.df.plot(column="NEGATIVES", scheme=scheme, k=3, legend=True)
+    def test_scheme_name_compat(self, scheme, df):
+        ax = df.plot(column="NEGATIVES", scheme=scheme, k=3, legend=True)
         assert len(ax.get_legend().get_texts()) == 3
 
-    def test_schemes(self):
+    def test_schemes(self, df):
         # test if all available classifiers pass
         for scheme in self.classifiers:
-            self.df.plot(column="pop_est", scheme=scheme, legend=True)
+            df.plot(column="pop_est", scheme=scheme, legend=True)
 
-    def test_classification_kwds(self):
-        ax = self.df.plot(
+    def test_classification_kwds(self, df):
+        ax = df.plot(
             column="pop_est",
             scheme="percentiles",
             k=3,
             classification_kwds={"pct": [50, 100]},
             cmap="OrRd",
             legend=True,
         )
         labels = [t.get_text() for t in ax.get_legend().get_texts()]
-        expected = ["       140.00,    9961396.00", "   9961396.00, 1379302771.00"]
+        expected = [
+            s.split("|")[0][1:-2]
+            for s in str(self.mc.Percentiles(df["pop_est"], pct=[50, 100])).split("\n")[
+                4:
+            ]
+        ]
+
         assert labels == expected
 
-    def test_invalid_scheme(self):
+    def test_invalid_scheme(self, df):
         with pytest.raises(ValueError):
             scheme = "invalid_scheme_*#&)(*#"
-            self.df.plot(
-                column="gdp_md_est", scheme=scheme, k=3, cmap="OrRd", legend=True
-            )
+            df.plot(column="gdp_md_est", scheme=scheme, k=3, cmap="OrRd", legend=True)
 
-    def test_cax_legend_passing(self):
+    def test_cax_legend_passing(self, df):
         """Pass a 'cax' argument to 'df.plot(.)', that is valid only if 'ax' is
         passed as well (if not, a new figure is created ad hoc, and 'cax' is
         ignored)
         """
         ax = plt.axes()
         from mpl_toolkits.axes_grid1 import make_axes_locatable
 
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("right", size="5%", pad=0.1)
         with pytest.raises(ValueError):
-            ax = self.df.plot(column="pop_est", cmap="OrRd", legend=True, cax=cax)
+            ax = df.plot(column="pop_est", cmap="OrRd", legend=True, cax=cax)
 
-    def test_cax_legend_height(self):
+    def test_cax_legend_height(self, df):
         """Pass a cax argument to 'df.plot(.)', the legend location must be
         aligned with those of main plot
         """
         # base case
         with warnings.catch_warnings(record=True) as _:  # don't print warning
-            ax = self.df.plot(column="pop_est", cmap="OrRd", legend=True)
+            ax = df.plot(column="pop_est", cmap="OrRd", legend=True)
         plot_height = _get_ax(ax.get_figure(), "").get_position().height
         legend_height = _get_ax(ax.get_figure(), "<colorbar>").get_position().height
         assert abs(plot_height - legend_height) >= 1e-6
         # fix heights with cax argument
         fig, ax2 = plt.subplots()
         from mpl_toolkits.axes_grid1 import make_axes_locatable
 
         divider = make_axes_locatable(ax2)
         cax = divider.append_axes("right", size="5%", pad=0.1, label="fixed_colorbar")
         with warnings.catch_warnings(record=True) as _:
-            ax2 = self.df.plot(
-                column="pop_est", cmap="OrRd", legend=True, cax=cax, ax=ax2
-            )
+            ax2 = df.plot(column="pop_est", cmap="OrRd", legend=True, cax=cax, ax=ax2)
         plot_height = _get_ax(fig, "").get_position().height
         legend_height = _get_ax(fig, "fixed_colorbar").get_position().height
         assert abs(plot_height - legend_height) < 1e-6
 
+    def test_empty_bins(self, df):
+        bins = np.arange(1, 11) / 10
+        ax = df.plot(
+            "low_vals",
+            scheme="UserDefined",
+            classification_kwds={"bins": bins},
+            legend=True,
+        )
+        expected = np.array(
+            [
+                [0.281412, 0.155834, 0.469201, 1.0],
+                [0.267004, 0.004874, 0.329415, 1.0],
+                [0.244972, 0.287675, 0.53726, 1.0],
+            ]
+        )
+        assert all(
+            (z == expected).all(axis=1).any()
+            for z in ax.collections[0].get_facecolors()
+        )
+        labels = [
+            "0.00, 0.10",
+            "0.10, 0.20",
+            "0.20, 0.30",
+            "0.30, 0.40",
+            "0.40, 0.50",
+            "0.50, 0.60",
+            "0.60, 0.70",
+            "0.70, 0.80",
+            "0.80, 0.90",
+            "0.90, 1.00",
+        ]
+        legend = [t.get_text() for t in ax.get_legend().get_texts()]
+        assert labels == legend
+
+        legend_colors_exp = [
+            (0.267004, 0.004874, 0.329415, 1.0),
+            (0.281412, 0.155834, 0.469201, 1.0),
+            (0.244972, 0.287675, 0.53726, 1.0),
+            (0.190631, 0.407061, 0.556089, 1.0),
+            (0.147607, 0.511733, 0.557049, 1.0),
+            (0.119699, 0.61849, 0.536347, 1.0),
+            (0.20803, 0.718701, 0.472873, 1.0),
+            (0.430983, 0.808473, 0.346476, 1.0),
+            (0.709898, 0.868751, 0.169257, 1.0),
+            (0.993248, 0.906157, 0.143936, 1.0),
+        ]
+
+        assert [
+            line.get_markerfacecolor() for line in ax.get_legend().get_lines()
+        ] == legend_colors_exp
+
+        ax2 = df.plot(
+            "mid_vals",
+            scheme="UserDefined",
+            classification_kwds={"bins": bins},
+            legend=True,
+        )
+        expected = np.array(
+            [
+                [0.244972, 0.287675, 0.53726, 1.0],
+                [0.190631, 0.407061, 0.556089, 1.0],
+                [0.147607, 0.511733, 0.557049, 1.0],
+                [0.119699, 0.61849, 0.536347, 1.0],
+                [0.20803, 0.718701, 0.472873, 1.0],
+            ]
+        )
+        assert all(
+            (z == expected).all(axis=1).any()
+            for z in ax2.collections[0].get_facecolors()
+        )
+
+        labels = [
+            "-inf, 0.10",
+            "0.10, 0.20",
+            "0.20, 0.30",
+            "0.30, 0.40",
+            "0.40, 0.50",
+            "0.50, 0.60",
+            "0.60, 0.70",
+            "0.70, 0.80",
+            "0.80, 0.90",
+            "0.90, 1.00",
+        ]
+        legend = [t.get_text() for t in ax2.get_legend().get_texts()]
+        assert labels == legend
+        assert [
+            line.get_markerfacecolor() for line in ax2.get_legend().get_lines()
+        ] == legend_colors_exp
+
+        ax3 = df.plot(
+            "high_vals",
+            scheme="UserDefined",
+            classification_kwds={"bins": bins},
+            legend=True,
+        )
+        expected = np.array(
+            [
+                [0.709898, 0.868751, 0.169257, 1.0],
+                [0.993248, 0.906157, 0.143936, 1.0],
+                [0.430983, 0.808473, 0.346476, 1.0],
+            ]
+        )
+        assert all(
+            (z == expected).all(axis=1).any()
+            for z in ax3.collections[0].get_facecolors()
+        )
+
+        legend = [t.get_text() for t in ax3.get_legend().get_texts()]
+        assert labels == legend
+
+        assert [
+            line.get_markerfacecolor() for line in ax3.get_legend().get_lines()
+        ] == legend_colors_exp
+
+    def test_equally_formatted_bins(self, nybb):
+        ax = nybb.plot(
+            "vals",
+            scheme="quantiles",
+            legend=True,
+        )
+        labels = [t.get_text() for t in ax.get_legend().get_texts()]
+        expected = [
+            "0.00, 0.00",
+            "0.00, 0.00",
+            "0.00, 0.00",
+            "0.00, 0.00",
+            "0.00, 0.01",
+        ]
+        assert labels == expected
+
+        ax2 = nybb.plot(
+            "vals", scheme="quantiles", legend=True, legend_kwds={"fmt": "{:.3f}"}
+        )
+        labels = [t.get_text() for t in ax2.get_legend().get_texts()]
+        expected = [
+            "0.001, 0.002",
+            "0.002, 0.003",
+            "0.003, 0.003",
+            "0.003, 0.004",
+            "0.004, 0.005",
+        ]
+        assert labels == expected
+
 
 class TestPlotCollections:
     def setup_method(self):
         self.N = 3
         self.values = np.arange(self.N)
         self.points = GeoSeries(Point(i, i) for i in range(self.N))
         self.lines = GeoSeries(
             [LineString([(0, i), (4, i + 0.5), (9, i)]) for i in range(self.N)]
         )
         self.polygons = GeoSeries(
             [Polygon([(0, i), (4, i + 0.5), (9, i)]) for i in range(self.N)]
         )
 
     def test_points(self):
-        # failing with matplotlib 1.4.3 (edge stays black even when specified)
-        pytest.importorskip("matplotlib", "1.5.0")
-
-        from geopandas.plotting import _plot_point_collection, plot_point_collection
+        from geopandas.plotting import _plot_point_collection
         from matplotlib.collections import PathCollection
 
         fig, ax = plt.subplots()
         coll = _plot_point_collection(ax, self.points)
         assert isinstance(coll, PathCollection)
         ax.cla()
 
@@ -1261,36 +1513,29 @@
         )
         ax.cla()
 
         # not a color
         with pytest.raises((TypeError, ValueError)):
             _plot_point_collection(ax, self.points, color="not color")
 
-        # check DeprecationWarning
-        with pytest.warns(DeprecationWarning):
-            plot_point_collection(ax, self.points)
-
     def test_points_values(self):
         from geopandas.plotting import _plot_point_collection
 
         # default colormap
         fig, ax = plt.subplots()
         coll = _plot_point_collection(ax, self.points, self.values)
         fig.canvas.draw_idle()
         cmap = plt.get_cmap()
         expected_colors = cmap(np.arange(self.N) / (self.N - 1))
         _check_colors(self.N, coll.get_facecolors(), expected_colors)
         # edgecolor depends on matplotlib version
         # _check_colors(self.N, coll.get_edgecolors(), expected_colors)
 
     def test_linestrings(self):
-        from geopandas.plotting import (
-            _plot_linestring_collection,
-            plot_linestring_collection,
-        )
+        from geopandas.plotting import _plot_linestring_collection
         from matplotlib.collections import LineCollection
 
         fig, ax = plt.subplots()
         coll = _plot_linestring_collection(ax, self.lines)
         assert isinstance(coll, LineCollection)
         ax.cla()
 
@@ -1334,17 +1579,14 @@
         assert res_ls[0] == exp_ls[0]
         assert res_ls[1] == exp_ls[1]
         ax.cla()
 
         # not a color
         with pytest.raises((TypeError, ValueError)):
             _plot_linestring_collection(ax, self.lines, color="not color")
-        # check DeprecationWarning
-        with pytest.warns(DeprecationWarning):
-            plot_linestring_collection(ax, self.lines)
 
     def test_linestrings_values(self):
         from geopandas.plotting import _plot_linestring_collection
 
         fig, ax = plt.subplots()
 
         # default colormap
@@ -1368,15 +1610,15 @@
         fig.canvas.draw_idle()
         cmap = plt.get_cmap()
         expected_colors = [cmap(0)]
         _check_colors(self.N, coll.get_color(), expected_colors * 3)
         ax.cla()
 
     def test_polygons(self):
-        from geopandas.plotting import _plot_polygon_collection, plot_polygon_collection
+        from geopandas.plotting import _plot_polygon_collection
         from matplotlib.collections import PatchCollection
 
         fig, ax = plt.subplots()
         coll = _plot_polygon_collection(ax, self.polygons)
         assert isinstance(coll, PatchCollection)
         ax.cla()
 
@@ -1426,17 +1668,14 @@
         _check_colors(self.N, coll.get_facecolor(), ["g"] * self.N)
         _check_colors(self.N, coll.get_edgecolor(), ["r"] * self.N)
         ax.cla()
 
         # not a color
         with pytest.raises((TypeError, ValueError)):
             _plot_polygon_collection(ax, self.polygons, color="not color")
-        # check DeprecationWarning
-        with pytest.warns(DeprecationWarning):
-            plot_polygon_collection(ax, self.polygons)
 
     def test_polygons_values(self):
         from geopandas.plotting import _plot_polygon_collection
 
         fig, ax = plt.subplots()
 
         # default colormap, edge is still black by default
@@ -1471,15 +1710,14 @@
         cmap = plt.get_cmap()
         exp_colors = cmap(np.arange(self.N) / (self.N - 1))
         _check_colors(self.N, coll.get_facecolor(), exp_colors)
         _check_colors(self.N, coll.get_edgecolor(), ["g"] * self.N)
         ax.cla()
 
 
-@pytest.mark.skipif(not compat.PANDAS_GE_025, reason="requires pandas > 0.24")
 class TestGeoplotAccessor:
     def setup_method(self):
         geometries = [Polygon([(0, 0), (1, 0), (1, 1)]), Point(1, 3)]
         x = [1, 2]
         y = [10, 20]
         self.gdf = GeoDataFrame(
             {"geometry": geometries, "x": x, "y": y}, crs="EPSG:4326"
@@ -1494,19 +1732,15 @@
         self.gdf.plot(kind=kind, ax=ax_geopandas_1, **kwargs)
 
         ax_pandas_2 = fig_test.subplots()
         getattr(self.df.plot, kind)(ax=ax_pandas_2, **kwargs)
         ax_geopandas_2 = fig_ref.subplots()
         getattr(self.gdf.plot, kind)(ax=ax_geopandas_2, **kwargs)
 
-    _pandas_kinds = []
-    if compat.PANDAS_GE_025:
-        from geopandas.plotting import GeoplotAccessor
-
-        _pandas_kinds = GeoplotAccessor._pandas_kinds
+    _pandas_kinds = GeoplotAccessor._pandas_kinds
 
     if MPL_DECORATORS:
 
         @pytest.mark.parametrize("kind", _pandas_kinds)
         @check_figures_equal(extensions=["png", "pdf"])
         def test_pandas_kind(self, kind, fig_test, fig_ref):
             """Test Pandas kind."""
@@ -1518,18 +1752,21 @@
             kwargs = {}
             if kind in _scipy_dependent_kinds:
                 if not importlib.util.find_spec("scipy"):
                     with pytest.raises(
                         ModuleNotFoundError, match="No module named 'scipy'"
                     ):
                         self.gdf.plot(kind=kind)
+                    return
             elif kind in _y_kinds:
                 kwargs = {"y": "y"}
             elif kind in _xy_kinds:
                 kwargs = {"x": "x", "y": "y"}
+                if kind == "hexbin":  # increase gridsize to reduce duration
+                    kwargs["gridsize"] = 10
 
             self.compare_figures(kind, fig_test, fig_ref, kwargs)
             plt.close("all")
 
         @check_figures_equal(extensions=["png", "pdf"])
         def test_geo_kind(self, fig_test, fig_ref):
             """Test Geo kind."""
@@ -1557,15 +1794,15 @@
     """
     # Build test data
     t1 = Polygon([(0, 0), (1, 0), (1, 1)])
     t2 = Polygon([(1, 0), (2, 0), (2, 1)])
     polys = GeoSeries([t1, t2], index=list("AB"))
     df = GeoDataFrame({"geometry": polys, "values": [0, 1]})
 
-    # Test with continous values
+    # Test with continuous values
     ax = df.plot(column="values")
     colors = ax.collections[0].get_facecolors()
     ax = df.plot(column=df["values"])
     colors_series = ax.collections[0].get_facecolors()
     np.testing.assert_array_equal(colors, colors_series)
     ax = df.plot(column=df["values"].values)
     colors_array = ax.collections[0].get_facecolors()
@@ -1577,15 +1814,15 @@
     ax = df.plot(column=df["values"], categorical=True)
     colors_series = ax.collections[0].get_facecolors()
     np.testing.assert_array_equal(colors, colors_series)
     ax = df.plot(column=df["values"].values, categorical=True)
     colors_array = ax.collections[0].get_facecolors()
     np.testing.assert_array_equal(colors, colors_array)
 
-    # Check raised error: is df rows number equal to column legth?
+    # Check raised error: is df rows number equal to column length?
     with pytest.raises(ValueError, match="different number of rows"):
         ax = df.plot(column=np.array([1, 2, 3]))
 
 
 def test_polygon_patch():
     # test adapted from descartes by Sean Gillies
     # (BSD license, https://pypi.org/project/descartes).
@@ -1623,25 +1860,25 @@
         `collection.get_facecolors()`
     expected_colors : sequence of RGBA tuples
     alpha : float (optional)
         If set, this alpha transparency will be applied to the
         `expected_colors`. (Any transparency on the `collection` is assumed
         to be set in its own facecolor RGBA tuples.)
     """
-    import matplotlib.colors as colors
+    from matplotlib import colors
 
     conv = colors.colorConverter
 
     # Convert 2D numpy array to a list of RGBA tuples.
     actual_colors = map(tuple, actual_colors)
     all_actual_colors = list(itertools.islice(itertools.cycle(actual_colors), N))
 
-    assert len(all_actual_colors) == len(expected_colors), (
-        "Different " "lengths of actual and expected colors!"
-    )
+    assert len(all_actual_colors) == len(
+        expected_colors
+    ), "Different lengths of actual and expected colors!"
 
     for actual, expected in zip(all_actual_colors, expected_colors):
         assert actual == conv.to_rgba(expected, alpha=alpha), "{} != {}".format(
             actual, conv.to_rgba(expected, alpha=alpha)
         )
 
 
@@ -1652,33 +1889,27 @@
     to the form `onoffseq`.
     """
     offset, dashes = matplotlib.lines._get_dash_pattern(linestyle)
     return matplotlib.lines._scale_dashes(offset, dashes, linewidth)
 
 
 def _style_to_vertices(markerstyle):
-    """ Converts a markerstyle string to a path. """
+    """Converts a markerstyle string to a path."""
     # TODO: Vertices values are twice the actual path; unclear, why.
     path = matplotlib.markers.MarkerStyle(markerstyle).get_path()
     return path.vertices / 2
 
 
 def _get_ax(fig, label):
     """
     Helper function to not rely on the order of `fig.axes`.
     Previously, we did `fig.axes[1]`, but in matplotlib 3.4 the order switched
     and the colorbar ax was first and subplot ax second.
     """
-    if matplotlib.__version__ < LooseVersion("3.0.0"):
-        if label == "<colorbar>":
-            return fig.axes[1]
-        elif label == "":
-            return fig.axes[0]
     for ax in fig.axes:
         if ax.get_label() == label:
             return ax
-    else:
-        raise ValueError("no ax found with label {0}".format(label))
+    raise ValueError("no ax found with label {0}".format(label))
 
 
 def _get_colorbar_ax(fig):
     return _get_ax(fig, "<colorbar>")
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_show_versions.py` & `geopandas-1.0.0a1/geopandas/tests/test_show_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     deps_info = _get_deps_info()
 
     assert "geopandas" in deps_info
     assert "pandas" in deps_info
     assert "fiona" in deps_info
     assert "numpy" in deps_info
     assert "shapely" in deps_info
-    assert "rtree" in deps_info
     assert "pyproj" in deps_info
     assert "matplotlib" in deps_info
     assert "mapclassify" in deps_info
     assert "geopy" in deps_info
+    assert "psycopg" in deps_info
     assert "psycopg2" in deps_info
     assert "geoalchemy2" in deps_info
 
 
 def test_show_versions(capsys):
     show_versions()
     out, err = capsys.readouterr()
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_sindex.py` & `geopandas-1.0.0a1/geopandas/tests/test_sindex.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-import sys
+from math import sqrt
 
+import numpy as np
+import pandas as pd
+import pytest
+import shapely
+from numpy.testing import assert_array_equal
 from shapely.geometry import (
+    GeometryCollection,
+    LineString,
+    MultiPolygon,
     Point,
     Polygon,
-    MultiPolygon,
     box,
-    GeometryCollection,
-    LineString,
 )
-from numpy.testing import assert_array_equal
 
 import geopandas
+from geopandas import GeoDataFrame, GeoSeries, read_file
 from geopandas import _compat as compat
-from geopandas import GeoDataFrame, GeoSeries, read_file, datasets
-
-import pytest
-import numpy as np
 
 
-@pytest.mark.skipif(sys.platform.startswith("win"), reason="fails on AppVeyor")
-@pytest.mark.skip_no_sindex
 class TestSeriesSindex:
     def test_has_sindex(self):
         """Test the has_sindex method."""
         t1 = Polygon([(0, 0), (1, 0), (1, 1)])
         t2 = Polygon([(0, 0), (1, 1), (0, 1)])
 
         d = GeoDataFrame({"geom": [t1, t2]}, geometry="geom")
@@ -67,14 +66,16 @@
     def test_polygons(self):
         t1 = Polygon([(0, 0), (1, 0), (1, 1)])
         t2 = Polygon([(0, 0), (1, 1), (0, 1)])
         sq = Polygon([(0, 0), (1, 0), (1, 1), (0, 1)])
         s = GeoSeries([t1, t2, sq])
         assert s.sindex.size == 3
 
+    @pytest.mark.filterwarnings("ignore:The series.append method is deprecated")
+    @pytest.mark.skipif(compat.PANDAS_GE_20, reason="append removed in pandas 2.0")
     def test_polygons_append(self):
         t1 = Polygon([(0, 0), (1, 0), (1, 1)])
         t2 = Polygon([(0, 0), (1, 1), (0, 1)])
         sq = Polygon([(0, 0), (1, 0), (1, 1), (0, 1)])
         s = GeoSeries([t1, t2, sq])
         t = GeoSeries([t1, t2, sq], [3, 4, 5])
         s = s.append(t)
@@ -103,16 +104,14 @@
         sliced = s.iloc[:]
         assert sliced.sindex is original_index
         # Select all rows and flip
         sliced = s.iloc[::-1]
         assert sliced.sindex is not original_index
 
 
-@pytest.mark.skipif(sys.platform.startswith("win"), reason="fails on AppVeyor")
-@pytest.mark.skip_no_sindex
 class TestFrameSindex:
     def setup_method(self):
         data = {
             "A": range(5),
             "B": range(-5, 0),
             "geom": [Point(x, y) for x, y in zip(range(5), range(5))],
         }
@@ -157,33 +156,62 @@
         # Selecting geometry column preserves the index
         original_index = self.df.sindex
         geometry_col = self.df["geom"]
         assert geometry_col.sindex is original_index
         geometry_col = self.df.geometry
         assert geometry_col.sindex is original_index
 
-    @pytest.mark.skipif(
-        not compat.PANDAS_GE_10, reason="Column selection returns a copy on pd<=1.0.0"
-    )
     def test_rebuild_on_multiple_col_selection(self):
         """Selecting a subset of columns preserves the index."""
         original_index = self.df.sindex
-        # Selecting a subset of columns preserves the index
+        # Selecting a subset of columns preserves the index for pandas < 2.0
+        # with pandas 2.0, the column is now copied, losing the index (although
+        # with Copy-on-Write, this will again be preserved)
         subset1 = self.df[["geom", "A"]]
-        assert subset1.sindex is original_index
+        if compat.PANDAS_GE_20 and not pd.options.mode.copy_on_write:
+            assert subset1.sindex is not original_index
+        else:
+            assert subset1.sindex is original_index
         subset2 = self.df[["A", "geom"]]
-        assert subset2.sindex is original_index
+        if compat.PANDAS_GE_20 and not pd.options.mode.copy_on_write:
+            assert subset2.sindex is not original_index
+        else:
+            assert subset2.sindex is original_index
+
+    def test_rebuild_on_update_inplace(self):
+        gdf = self.df.copy()
+        old_sindex = gdf.sindex
+        # sorting in place
+        gdf.sort_values("A", ascending=False, inplace=True)
+        # spatial index should be invalidated
+        assert not gdf.has_sindex
+        new_sindex = gdf.sindex
+        # and should be different
+        assert new_sindex is not old_sindex
+
+        # sorting should still have happened though
+        assert gdf.index.tolist() == [4, 3, 2, 1, 0]
+
+    def test_update_inplace_no_rebuild(self):
+        gdf = self.df.copy()
+        old_sindex = gdf.sindex
+        gdf.rename(columns={"A": "AA"}, inplace=True)
+        # a rename shouldn't invalidate the index
+        assert gdf.has_sindex
+        # and the "new" should be the same
+        new_sindex = gdf.sindex
+        assert old_sindex is new_sindex
 
 
-# Skip to accommodate Shapely geometries being unhashable
+# Skip to accommodate Shapely geometries being unhashable # TODO unskip?
 @pytest.mark.skip
+@pytest.mark.usefixtures("_setup_class_nybb_filename")
 class TestJoinSindex:
     def setup_method(self):
-        nybb_filename = geopandas.datasets.get_path("nybb")
-        self.boros = read_file(nybb_filename)
+        self.boros = read_file(self.nybb_filename)
 
     def test_merge_geo(self):
         # First check that we gets hits from the boros frame.
         tree = self.boros.sindex
         hits = tree.intersection((1012821.80, 229228.26))
         res = [self.boros.iloc[hit]["BoroName"] for hit in hits]
         assert res == ["Bronx", "Queens"]
@@ -208,16 +236,15 @@
         assert merged.sindex.size == 5
         tree = merged.sindex
         hits = tree.intersection((1012821.80, 229228.26))
         res = [merged.iloc[hit]["BoroName"] for hit in hits]
         assert res == ["Bronx", "Queens"]
 
 
-@pytest.mark.skip_no_sindex
-class TestPygeosInterface:
+class TestShapelyInterface:
     def setup_method(self):
         data = {
             "geom": [Point(x, y) for x, y in zip(range(5), range(5))]
             + [box(10, 10, 20, 20)]  # include a box geometry
         }
         self.df = GeoDataFrame(data, geometry="geom")
         self.expected_size = len(data["geom"])
@@ -236,23 +263,17 @@
         """Tests the `intersection` method with valid inputs."""
         res = list(self.df.sindex.intersection(test_geom))
         assert_array_equal(res, expected)
 
     @pytest.mark.parametrize("test_geom", ((-1, -1, -0.5), -0.5, None, Point(0, 0)))
     def test_intersection_invalid_bounds_tuple(self, test_geom):
         """Tests the `intersection` method with invalid inputs."""
-        if compat.USE_PYGEOS:
-            with pytest.raises(TypeError):
-                # we raise a useful TypeError
-                self.df.sindex.intersection(test_geom)
-        else:
-            with pytest.raises((TypeError, Exception)):
-                # catch a general exception
-                # rtree raises an RTreeError which we need to catch
-                self.df.sindex.intersection(test_geom)
+        with pytest.raises(TypeError):
+            # we raise a useful TypeError
+            self.df.sindex.intersection(test_geom)
 
     # ------------------------------ `query` tests ------------------------------ #
     @pytest.mark.parametrize(
         "predicate, test_geom, expected",
         (
             (None, box(-1, -1, -0.5, -0.5), []),  # bbox does not intersect
             (None, box(-0.5, -0.5, 0.5, 0.5), [0]),  # bbox intersects
@@ -355,14 +376,116 @@
         assert_array_equal(res, expected)
 
     def test_query_invalid_geometry(self):
         """Tests the `query` method with invalid geometry."""
         with pytest.raises(TypeError):
             self.df.sindex.query("notavalidgeom")
 
+    @pytest.mark.skipif(not compat.GEOS_GE_310, reason="Requires GEOS 3.10")
+    @pytest.mark.parametrize(
+        "distance, test_geom, expected",
+        (
+            # bounds don't intersect and not within distance=0
+            (
+                0,
+                box(9.0, 9.0, 9.9, 9.9),
+                [],
+            ),
+            # bounds don't intersect but is within distance=1
+            (
+                1,
+                box(9.0, 9.0, 9.9, 9.9),
+                [5],
+            ),
+            # within 1-D absolute distance in both axes, but not euclidean distance
+            (
+                0.5,
+                Point(0.5, 0.5),
+                [],
+            ),
+            # same as before but within euclidean distance
+            (
+                sqrt(2 * 0.5**2) + 1e-9,
+                Point(0.5, 0.5),
+                [0, 1],
+            ),
+            # less than euclidean distance between points, multi-object
+            (
+                sqrt(2) - 1e-9,
+                [
+                    Polygon([(0, 0), (1, 0), (1, 1)]),
+                    Polygon([(1, 1), (2, 1), (2, 2)]),
+                ],  # multi-object test
+                [[0, 0, 1, 1], [0, 1, 1, 2]],
+            ),
+            # more than euclidean distance between points, multi-object
+            (
+                sqrt(2) + 1e-9,
+                [
+                    Polygon([(0, 0), (1, 0), (1, 1)]),
+                    Polygon([(1, 1), (2, 1), (2, 2)]),
+                ],
+                [[0, 0, 0, 1, 1, 1, 1], [0, 1, 2, 0, 1, 2, 3]],
+            ),
+            # distance is array-like, broadcastable to geometry
+            (
+                [2, 10],
+                [Point(0.5, 0.5), Point(1, 1)],
+                [[0, 0, 1, 1, 1, 1, 1], [0, 1, 0, 1, 2, 3, 4]],
+            ),
+        ),
+    )
+    def test_query_dwithin(self, distance, test_geom, expected):
+        """Tests the `query` method with predicates that require keyword arguments."""
+        res = self.df.sindex.query(test_geom, predicate="dwithin", distance=distance)
+        assert_array_equal(res, expected)
+
+    @pytest.mark.skipif(not compat.GEOS_GE_310, reason="Requires GEOS 3.10")
+    def test_dwithin_no_distance(self):
+        """Tests the `query` method with keyword arguments that are
+        invalid for certain predicates."""
+        with pytest.raises(
+            ValueError, match="'distance' parameter is required for 'dwithin' predicate"
+        ):
+            self.df.sindex.query(Point(0, 0), predicate="dwithin")
+
+    @pytest.mark.parametrize(
+        "predicate",
+        [
+            None,
+            "contains",
+            "contains_properly",
+            "covered_by",
+            "covers",
+            "crosses",
+            "intersects",
+            "overlaps",
+            "touches",
+            "within",
+        ],
+    )
+    def test_query_distance_invalid(self, predicate):
+        """Tests the `query` method with keyword arguments that are
+        invalid for certain predicates."""
+        msg = "'distance' parameter is only supported in combination with 'dwithin'"
+        with pytest.raises(ValueError, match=msg):
+            self.df.sindex.query(Point(0, 0), predicate=predicate, distance=0)
+
+    @pytest.mark.skipif(
+        compat.GEOS_GE_310, reason="Test for 'dwithin'-incompatible versions of GEOS"
+    )
+    def test_dwithin_requirements(self):
+        """Tests whether a ValueError is raised when trying to use dwithin with
+        incompatible versions of shapely or pyGEOS
+        """
+        with pytest.raises(
+            ValueError, match="predicate = 'dwithin' requires GEOS >= 3.10.0"
+        ):
+            self.df.sindex.query(Point(0, 0), predicate="dwithin", distance=0)
+
     @pytest.mark.parametrize(
         "test_geom, expected_value",
         [
             (None, []),
             (GeometryCollection(), []),
             (Point(), []),
             (MultiPolygon(), []),
@@ -401,21 +524,16 @@
                 Polygon([(1, 1), (3, 1), (3, 3), (1, 3)]),
                 Polygon([(-1, 1), (1, 1), (1, 3), (-1, 3)]),
                 Polygon([(3, 3), (5, 3), (5, 5), (3, 5)]),
             ]
         )
         expected = [0, 1, 2]
 
-        # pass through GeoSeries to have GeoPandas
-        # determine if it should use shapely or pygeos geometry objects
-        tree_df = geopandas.GeoDataFrame(geometry=tree_polys)
-        test_df = geopandas.GeoDataFrame(geometry=test_polys)
-
-        test_geo = test_df.geometry.values.data[0]
-        res = tree_df.sindex.query(test_geo, sort=sort)
+        test_geo = test_polys.values[0]
+        res = tree_polys.sindex.query(test_geo, sort=sort)
 
         # asserting the same elements
         assert sorted(res) == sorted(expected)
         # asserting the exact array can fail if sort=False
         try:
             assert_array_equal(res, expected)
         except AssertionError as e:
@@ -525,138 +643,121 @@
                 "contains_properly",
                 [(10, 10, 20, 20)],
                 [[], []],
             ),  # contains but does not contains_properly
         ),
     )
     def test_query_bulk(self, predicate, test_geom, expected):
-        """Tests the `query_bulk` method with valid
+        """Tests the `query` method with valid
         inputs and valid predicates.
         """
-        # pass through GeoSeries to have GeoPandas
-        # determine if it should use shapely or pygeos geometry objects
-        test_geom = geopandas.GeoSeries(
-            [box(*geom) for geom in test_geom], index=range(len(test_geom))
+        res = self.df.sindex.query(
+            [box(*geom) for geom in test_geom], predicate=predicate
         )
-        res = self.df.sindex.query_bulk(test_geom, predicate=predicate)
         assert_array_equal(res, expected)
 
     @pytest.mark.parametrize(
         "test_geoms, expected_value",
         [
             # single empty geometry
             ([GeometryCollection()], [[], []]),
             # None should be skipped
             ([GeometryCollection(), None], [[], []]),
             ([None], [[], []]),
             ([None, box(-0.5, -0.5, 0.5, 0.5), None], [[1], [0]]),
         ],
     )
     def test_query_bulk_empty_geometry(self, test_geoms, expected_value):
-        """Tests the `query_bulk` method with an empty geometry."""
-        # pass through GeoSeries to have GeoPandas
-        # determine if it should use shapely or pygeos geometry objects
-        # note: for this test, test_geoms (note plural) is a list already
-        test_geoms = geopandas.GeoSeries(test_geoms, index=range(len(test_geoms)))
-        res = self.df.sindex.query_bulk(test_geoms)
+        """Tests the `query` method with an empty geometries."""
+        res = self.df.sindex.query(test_geoms)
         assert_array_equal(res, expected_value)
 
     def test_query_bulk_empty_input_array(self):
-        """Tests the `query_bulk` method with an empty input array."""
+        """Tests the `query` method with an empty input array."""
         test_array = np.array([], dtype=object)
         expected_value = [[], []]
-        res = self.df.sindex.query_bulk(test_array)
+        res = self.df.sindex.query(test_array)
         assert_array_equal(res, expected_value)
 
     def test_query_bulk_invalid_input_geometry(self):
         """
-        Tests the `query_bulk` method with invalid input for the `geometry` parameter.
+        Tests the `query` method with invalid input for the `geometry` parameter.
         """
         test_array = "notanarray"
         with pytest.raises(TypeError):
-            self.df.sindex.query_bulk(test_array)
+            self.df.sindex.query(test_array)
 
     def test_query_bulk_invalid_predicate(self):
-        """Tests the `query_bulk` method with invalid predicates."""
+        """Tests the `query` method with invalid predicates."""
         test_geom_bounds = (-1, -1, -0.5, -0.5)
         test_predicate = "test"
 
-        # pass through GeoSeries to have GeoPandas
-        # determine if it should use shapely or pygeos geometry objects
-        test_geom = geopandas.GeoSeries([box(*test_geom_bounds)], index=["0"])
-
         with pytest.raises(ValueError):
-            self.df.sindex.query_bulk(test_geom.geometry, predicate=test_predicate)
+            self.df.sindex.query([box(*test_geom_bounds)], predicate=test_predicate)
 
     @pytest.mark.parametrize(
         "predicate, test_geom, expected",
         (
             (None, (-1, -1, -0.5, -0.5), [[], []]),
             ("intersects", (-1, -1, -0.5, -0.5), [[], []]),
             ("contains", (-1, -1, 1, 1), [[0], [0]]),
         ),
     )
     def test_query_bulk_input_type(self, predicate, test_geom, expected):
-        """Tests that query_bulk can accept a GeoSeries, GeometryArray or
+        """Tests that query can accept a GeoSeries, GeometryArray or
         numpy array.
         """
-        # pass through GeoSeries to have GeoPandas
-        # determine if it should use shapely or pygeos geometry objects
+        # pass through GeoSeries to test input type
         test_geom = geopandas.GeoSeries([box(*test_geom)], index=["0"])
 
         # test GeoSeries
-        res = self.df.sindex.query_bulk(test_geom, predicate=predicate)
+        res = self.df.sindex.query(test_geom, predicate=predicate)
         assert_array_equal(res, expected)
 
         # test GeometryArray
-        res = self.df.sindex.query_bulk(test_geom.geometry, predicate=predicate)
+        res = self.df.sindex.query(test_geom.geometry, predicate=predicate)
         assert_array_equal(res, expected)
-        res = self.df.sindex.query_bulk(test_geom.geometry.values, predicate=predicate)
+        res = self.df.sindex.query(test_geom.geometry.values, predicate=predicate)
         assert_array_equal(res, expected)
 
         # test numpy array
-        res = self.df.sindex.query_bulk(
-            test_geom.geometry.values.data, predicate=predicate
+        res = self.df.sindex.query(
+            test_geom.geometry.values.to_numpy(), predicate=predicate
         )
         assert_array_equal(res, expected)
-        res = self.df.sindex.query_bulk(
-            test_geom.geometry.values.data, predicate=predicate
+        res = self.df.sindex.query(
+            test_geom.geometry.values.to_numpy(), predicate=predicate
         )
         assert_array_equal(res, expected)
 
     @pytest.mark.parametrize(
         "sort, expected",
         (
             (True, [[0, 0, 0], [0, 1, 2]]),
             # False could be anything, at least we'll know if it changes
             (False, [[0, 0, 0], [0, 1, 2]]),
         ),
     )
     def test_query_bulk_sorting(self, sort, expected):
-        """Check that results from `query_bulk` don't depend
+        """Check that results from `query` don't depend
         on the order of geometries.
         """
         # these geometries come from a reported issue:
         # https://github.com/geopandas/geopandas/issues/1337
         # there is no theoretical reason they were chosen
         test_polys = GeoSeries([Polygon([(1, 1), (3, 1), (3, 3), (1, 3)])])
         tree_polys = GeoSeries(
             [
                 Polygon([(1, 1), (3, 1), (3, 3), (1, 3)]),
                 Polygon([(-1, 1), (1, 1), (1, 3), (-1, 3)]),
                 Polygon([(3, 3), (5, 3), (5, 5), (3, 5)]),
             ]
         )
 
-        # pass through GeoSeries to have GeoPandas
-        # determine if it should use shapely or pygeos geometry objects
-        tree_df = geopandas.GeoDataFrame(geometry=tree_polys)
-        test_df = geopandas.GeoDataFrame(geometry=test_polys)
-
-        res = tree_df.sindex.query_bulk(test_df.geometry, sort=sort)
+        res = tree_polys.sindex.query(test_polys, sort=sort)
 
         # asserting the same elements
         assert sorted(res[0]) == sorted(expected[0])
         assert sorted(res[1]) == sorted(expected[1])
         # asserting the exact array can fail if sort=False
         try:
             assert_array_equal(res, expected)
@@ -666,14 +767,149 @@
                     "rtree results are known to be unordered, see "
                     "https://github.com/geopandas/geopandas/issues/1337\n"
                     "Expected:\n {}\n".format(expected)
                     + "Got:\n {}\n".format(res.tolist())
                 )
             raise e
 
+    # ------------------------- `nearest` tests ------------------------- #
+    @pytest.mark.parametrize("return_all", [True, False])
+    @pytest.mark.parametrize(
+        "geometry,expected",
+        [
+            ([0.25, 0.25], [[0], [0]]),
+            ([0.75, 0.75], [[0], [1]]),
+        ],
+    )
+    def test_nearest_single(self, geometry, expected, return_all):
+        geoms = shapely.points(np.arange(10), np.arange(10))
+        df = geopandas.GeoDataFrame({"geometry": geoms})
+
+        p = Point(geometry)
+        res = df.sindex.nearest(p, return_all=return_all)
+        assert_array_equal(res, expected)
+
+        p = shapely.points(geometry)
+        res = df.sindex.nearest(p, return_all=return_all)
+        assert_array_equal(res, expected)
+
+    @pytest.mark.parametrize("return_all", [True, False])
+    @pytest.mark.parametrize(
+        "geometry,expected",
+        [
+            ([(1, 1), (0, 0)], [[0, 1], [1, 0]]),
+            ([(1, 1), (0.25, 1)], [[0, 1], [1, 1]]),
+        ],
+    )
+    def test_nearest_multi(self, geometry, expected, return_all):
+        geoms = shapely.points(np.arange(10), np.arange(10))
+        df = geopandas.GeoDataFrame({"geometry": geoms})
+
+        ps = [Point(p) for p in geometry]
+        res = df.sindex.nearest(ps, return_all=return_all)
+        assert_array_equal(res, expected)
+
+        ps = shapely.points(geometry)
+        res = df.sindex.nearest(ps, return_all=return_all)
+        assert_array_equal(res, expected)
+
+        s = geopandas.GeoSeries(ps)
+        res = df.sindex.nearest(s, return_all=return_all)
+        assert_array_equal(res, expected)
+
+        x, y = zip(*geometry)
+        ga = geopandas.points_from_xy(x, y)
+        res = df.sindex.nearest(ga, return_all=return_all)
+        assert_array_equal(res, expected)
+
+    @pytest.mark.parametrize("return_all", [True, False])
+    @pytest.mark.parametrize(
+        "geometry,expected",
+        [
+            (None, [[], []]),
+            ([None], [[], []]),
+        ],
+    )
+    def test_nearest_none(self, geometry, expected, return_all):
+        geoms = shapely.points(np.arange(10), np.arange(10))
+        df = geopandas.GeoDataFrame({"geometry": geoms})
+
+        res = df.sindex.nearest(geometry, return_all=return_all)
+        assert_array_equal(res, expected)
+
+    @pytest.mark.parametrize("return_distance", [True, False])
+    @pytest.mark.parametrize(
+        "return_all,max_distance,expected",
+        [
+            (True, None, ([[0, 0, 1], [0, 1, 5]], [sqrt(0.5), sqrt(0.5), sqrt(50)])),
+            (False, None, ([[0, 1], [0, 5]], [sqrt(0.5), sqrt(50)])),
+            (True, 1, ([[0, 0], [0, 1]], [sqrt(0.5), sqrt(0.5)])),
+            (False, 1, ([[0], [0]], [sqrt(0.5)])),
+        ],
+    )
+    def test_nearest_max_distance(
+        self, expected, max_distance, return_all, return_distance
+    ):
+        geoms = shapely.points(np.arange(10), np.arange(10))
+        df = geopandas.GeoDataFrame({"geometry": geoms})
+
+        ps = [Point(0.5, 0.5), Point(0, 10)]
+        res = df.sindex.nearest(
+            ps,
+            return_all=return_all,
+            max_distance=max_distance,
+            return_distance=return_distance,
+        )
+        if return_distance:
+            assert_array_equal(res[0], expected[0])
+            assert_array_equal(res[1], expected[1])
+        else:
+            assert_array_equal(res, expected[0])
+
+    @pytest.mark.parametrize("return_distance", [True, False])
+    @pytest.mark.parametrize(
+        "return_all,max_distance,exclusive,expected",
+        [
+            (False, None, False, ([[0, 1, 2, 3, 4], [0, 1, 2, 3, 4]], 5 * [0])),
+            (False, None, True, ([[0, 1, 2, 3, 4], [1, 0, 1, 2, 3]], 5 * [sqrt(2)])),
+            (True, None, False, ([[0, 1, 2, 3, 4], [0, 1, 2, 3, 4]], 5 * [0])),
+            (
+                True,
+                None,
+                True,
+                ([[0, 1, 1, 2, 2, 3, 3, 4], [1, 0, 2, 1, 3, 2, 4, 3]], 8 * [sqrt(2)]),
+            ),
+            (False, 1.1, True, ([[1, 2, 5], [5, 5, 1]], 3 * [1])),
+            (True, 1.1, True, ([[1, 2, 5, 5], [5, 5, 1, 2]], 4 * [1])),
+        ],
+    )
+    def test_nearest_exclusive(
+        self, expected, max_distance, return_all, return_distance, exclusive
+    ):
+        geoms = shapely.points(np.arange(5), np.arange(5))
+        if max_distance:
+            # add a non grid point
+            geoms = np.append(geoms, [Point(1, 2)])
+
+        df = geopandas.GeoDataFrame({"geometry": geoms})
+
+        ps = geoms
+        res = df.sindex.nearest(
+            ps,
+            return_all=return_all,
+            max_distance=max_distance,
+            return_distance=return_distance,
+            exclusive=exclusive,
+        )
+        if return_distance:
+            assert_array_equal(res[0], expected[0])
+            assert_array_equal(res[1], expected[1])
+        else:
+            assert_array_equal(res, expected[0])
+
     # --------------------------- misc tests ---------------------------- #
 
     def test_empty_tree_geometries(self):
         """Tests building sindex with interleaved empty geometries."""
         geoms = [Point(0, 0), None, Point(), Point(1, 1), Point()]
         df = geopandas.GeoDataFrame(geometry=geoms)
         assert df.sindex.query(Point(1, 1))[0] == 3
@@ -698,36 +934,25 @@
         # create a non-empty tree
         non_empty = geopandas.GeoSeries([Point(0, 0)])
         assert not non_empty.sindex.is_empty
 
     @pytest.mark.parametrize(
         "predicate, expected_shape",
         [
-            (None, (2, 396)),
-            ("intersects", (2, 172)),
-            ("within", (2, 172)),
+            (None, (2, 471)),
+            ("intersects", (2, 213)),
+            ("within", (2, 213)),
             ("contains", (2, 0)),
             ("overlaps", (2, 0)),
             ("crosses", (2, 0)),
             ("touches", (2, 0)),
         ],
     )
-    def test_integration_natural_earth(self, predicate, expected_shape):
+    def test_integration_natural_earth(
+        self, predicate, expected_shape, naturalearth_lowres, naturalearth_cities
+    ):
         """Tests output sizes for the naturalearth datasets."""
-        world = read_file(datasets.get_path("naturalearth_lowres"))
-        capitals = read_file(datasets.get_path("naturalearth_cities"))
+        world = read_file(naturalearth_lowres)
+        capitals = read_file(naturalearth_cities)
 
-        res = world.sindex.query_bulk(capitals.geometry, predicate)
+        res = world.sindex.query(capitals.geometry, predicate)
         assert res.shape == expected_shape
-
-
-@pytest.mark.skipif(not compat.HAS_RTREE, reason="no rtree installed")
-def test_old_spatial_index_deprecated():
-    t1 = Polygon([(0, 0), (1, 0), (1, 1)])
-    t2 = Polygon([(0, 0), (1, 1), (0, 1)])
-
-    stream = ((i, item.bounds, None) for i, item in enumerate([t1, t2]))
-
-    with pytest.warns(FutureWarning):
-        idx = geopandas.sindex.SpatialIndex(stream)
-
-    assert list(idx.intersection((0, 0, 1, 1))) == [0, 1]
```

### Comparing `geopandas-0.9.0/geopandas/tests/test_types.py` & `geopandas-1.0.0a1/geopandas/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `geopandas-0.9.0/geopandas/tests/util.py` & `geopandas-1.0.0a1/geopandas/tests/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 import os.path
 
 from pandas import Series
 
 from geopandas import GeoDataFrame
 
-from geopandas.testing import (  # noqa
+from geopandas.testing import (  # noqa: F401
     assert_geoseries_equal,
     geom_almost_equals,
     geom_equals,
 )
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 PACKAGE_DIR = os.path.dirname(os.path.dirname(HERE))
 
+_TEST_DATA_DIR = os.path.join(PACKAGE_DIR, "geopandas", "tests", "data")
+_NYBB = "zip://" + os.path.join(_TEST_DATA_DIR, "nybb_16a.zip")
+_NATURALEARTH_CITIES = os.path.join(
+    _TEST_DATA_DIR, "naturalearth_cities", "naturalearth_cities.shp"
+)
+_NATURALEARTH_LOWRES = os.path.join(
+    _TEST_DATA_DIR, "naturalearth_lowres", "naturalearth_lowres.shp"
+)
+
 
 # mock not used here, but the import from here is used in other modules
 try:
-    import unittest.mock as mock  # noqa
+    from unittest import mock
 except ImportError:
-    import mock  # noqa
+    import mock  # noqa: F401
 
 
 def validate_boro_df(df, case_sensitive=False):
     """Tests a GeoDataFrame that has been read in from the nybb dataset."""
     assert isinstance(df, GeoDataFrame)
     # Make sure all the columns are there and the geometries
     # were properly loaded as MultiPolygons
@@ -30,15 +39,15 @@
     columns = ("BoroCode", "BoroName", "Shape_Leng", "Shape_Area")
     if case_sensitive:
         for col in columns:
             assert col in df.columns
     else:
         for col in columns:
             assert col.lower() in (dfcol.lower() for dfcol in df.columns)
-    assert Series(df.geometry.type).dropna().eq("MultiPolygon").all()
+    assert Series(df.geometry.geom_type).dropna().eq("MultiPolygon").all()
 
 
 def get_srid(df):
     """Return srid from `df.crs`."""
     if df.crs is not None:
         return df.crs.to_epsg() or 0
     return 0
```

### Comparing `geopandas-0.9.0/geopandas/tools/_show_versions.py` & `geopandas-1.0.0a1/geopandas/tools/_show_versions.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,30 +44,46 @@
 
     try:
         import shapely._buildcfg
 
         geos_version = "{}.{}.{}".format(*shapely._buildcfg.geos_version)
         geos_dir = shapely._buildcfg.geos_library_path
     except Exception:
-        geos_version = None
-        geos_dir = None
+        try:
+            from shapely import geos_version_string
 
-    try:
-        import fiona
+            geos_version = geos_version_string
+            geos_dir = None
+        except Exception:
+            geos_version = None
+            geos_dir = None
 
-        gdal_version = fiona.env.get_gdal_release_name()
-    except Exception:
-        gdal_version = None
     try:
-        import fiona
+        import pyogrio
 
-        gdal_dir = fiona.env.GDALDataFinder().search()
+        gdal_version = pyogrio.__gdal_version_string__
+        gdal_dir = pyogrio.get_gdal_data_path()
     except Exception:
+        gdal_version = None
         gdal_dir = None
 
+    if gdal_version is None:
+        try:
+            import fiona
+
+            gdal_version = fiona.env.get_gdal_release_name()
+        except Exception:
+            gdal_version = None
+        try:
+            import fiona
+
+            gdal_dir = fiona.env.GDALDataFinder().search()
+        except Exception:
+            gdal_dir = None
+
     blob = [
         ("GEOS", geos_version),
         ("GEOS lib", geos_dir),
         ("GDAL", gdal_version),
         ("GDAL data dir", gdal_dir),
         ("PROJ", proj_version),
         ("PROJ data dir", proj_dir),
@@ -82,27 +98,29 @@
     Returns
     -------
     deps_info: dict
         version information on relevant Python libraries
     """
     deps = [
         "geopandas",
-        "pandas",
-        "fiona",
+        # required deps
         "numpy",
-        "shapely",
-        "rtree",
+        "pandas",
         "pyproj",
+        "shapely",
+        # optional deps
+        "pyogrio",
+        "geoalchemy2",
+        "geopy",
         "matplotlib",
         "mapclassify",
-        "geopy",
+        "fiona",
+        "psycopg",
         "psycopg2",
-        "geoalchemy2",
         "pyarrow",
-        "pygeos",
     ]
 
     def get_version(module):
         return module.__version__
 
     deps_info = {}
```

### Comparing `geopandas-0.9.0/geopandas/tools/geocoding.py` & `geopandas-1.0.0a1/geopandas/tools/geocoding.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,21 +27,20 @@
     Geocode a set of strings and get a GeoDataFrame of the resulting points.
 
     Parameters
     ----------
     strings : list or Series of addresses to geocode
     provider : str or geopy.geocoder
         Specifies geocoding service to use. If none is provided,
-        will use 'geocodefarm' with a rate limit applied (see the geocodefarm
-        terms of service at:
-        https://geocode.farm/geocoding/free-api-documentation/ ).
+        will use 'photon' (see the Photon's terms of service at:
+        https://photon.komoot.io).
 
         Either the string name used by geopy (as specified in
         geopy.geocoders.SERVICE_TO_GEOCODER) or a geopy Geocoder instance
-        (e.g., geopy.geocoders.GeocodeFarm) may be used.
+        (e.g., geopy.geocoders.Photon) may be used.
 
         Some providers require additional arguments such as access keys
         See each geocoder's specific parameters in geopy.geocoders
 
     Notes
     -----
     Ensure proper use of the results by consulting the Terms of Service for
@@ -58,19 +57,16 @@
     >>> df  # doctest: +SKIP
                         geometry                                            address
     0  POINT (-71.05863 42.35899)                          Boston, MA, United States
     1  POINT (-77.03651 38.89766)  1600 Pennsylvania Ave NW, Washington, DC 20006...
     """
 
     if provider is None:
-        # https://geocode.farm/geocoding/free-api-documentation/
-        provider = "geocodefarm"
-        throttle_time = 0.25
-    else:
-        throttle_time = _get_throttle_time(provider)
+        provider = "photon"
+    throttle_time = _get_throttle_time(provider)
 
     return _query(strings, True, provider, throttle_time, **kwargs)
 
 
 def reverse_geocode(points, provider=None, **kwargs):
     """
     Reverse geocode a set of points and get a GeoDataFrame of the resulting
@@ -81,21 +77,20 @@
     Parameters
     ----------
     points : list or Series of Shapely Point objects.
         x coordinate is longitude
         y coordinate is latitude
     provider : str or geopy.geocoder (opt)
         Specifies geocoding service to use. If none is provided,
-        will use 'geocodefarm' with a rate limit applied (see the geocodefarm
-        terms of service at:
-        https://geocode.farm/geocoding/free-api-documentation/ ).
+        will use 'photon' (see the Photon's terms of service at:
+        https://photon.komoot.io).
 
         Either the string name used by geopy (as specified in
         geopy.geocoders.SERVICE_TO_GEOCODER) or a geopy Geocoder instance
-        (e.g., geopy.geocoders.GeocodeFarm) may be used.
+        (e.g., geopy.geocoders.Photon) may be used.
 
         Some providers require additional arguments such as access keys
         See each geocoder's specific parameters in geopy.geocoders
 
     Notes
     -----
     Ensure proper use of the results by consulting the Terms of Service for
@@ -113,30 +108,31 @@
     >>> df  # doctest: +SKIP
                          geometry                                            address
     0  POINT (-71.05941 42.35837)       29 Court Sq, Boston, MA 02108, United States
     1  POINT (-77.03641 38.89766)  1600 Pennsylvania Ave NW, Washington, DC 20006...
     """
 
     if provider is None:
-        # https://geocode.farm/geocoding/free-api-documentation/
-        provider = "geocodefarm"
-        throttle_time = 0.25
-    else:
-        throttle_time = _get_throttle_time(provider)
+        provider = "photon"
+    throttle_time = _get_throttle_time(provider)
 
     return _query(points, False, provider, throttle_time, **kwargs)
 
 
 def _query(data, forward, provider, throttle_time, **kwargs):
     # generic wrapper for calls over lists to geopy Geocoders
     from geopy.geocoders.base import GeocoderQueryError
     from geopy.geocoders import get_geocoder_for_service
 
-    if not isinstance(data, pd.Series):
-        data = pd.Series(data)
+    if forward:
+        if not isinstance(data, pd.Series):
+            data = pd.Series(data)
+    else:
+        if not isinstance(data, geopandas.GeoSeries):
+            data = geopandas.GeoSeries(data)
 
     if isinstance(provider, str):
         provider = get_geocoder_for_service(provider)
 
     coder = provider(**kwargs)
     results = {}
     for i, s in data.items():
@@ -162,15 +158,14 @@
 
     """
     # Prepare the data for the DataFrame as a dict of lists
     d = defaultdict(list)
     index = []
 
     for i, s in results.items():
-
         if s is None:
             p = Point()
             address = None
 
         else:
             address, loc = s
```

### Comparing `geopandas-0.9.0/geopandas/tools/overlay.py` & `geopandas-1.0.0a1/geopandas/tools/overlay.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 
 
 def _overlay_intersection(df1, df2):
     """
     Overlay Intersection operation used in overlay function
     """
     # Spatial Index to create intersections
-    idx1, idx2 = df2.sindex.query_bulk(df1.geometry, predicate="intersects", sort=True)
+    idx1, idx2 = df2.sindex.query(df1.geometry, predicate="intersects", sort=True)
     # Create pairs of geometries in both dataframes to be intersected
     if idx1.size > 0 and idx2.size > 0:
         left = df1.geometry.take(idx1)
         left.reset_index(drop=True, inplace=True)
         right = df2.geometry.take(idx2)
         right.reset_index(drop=True, inplace=True)
         intersections = left.intersection(right)
-        poly_ix = intersections.type.isin(["Polygon", "MultiPolygon"])
-        intersections.loc[poly_ix] = intersections[poly_ix].buffer(0)
+        poly_ix = intersections.geom_type.isin(["Polygon", "MultiPolygon"])
+        intersections.loc[poly_ix] = intersections[poly_ix].make_valid()
 
         # only keep actual intersecting geometries
         pairs_intersect = pd.DataFrame({"__idx1": idx1, "__idx2": idx2})
         geom_intersect = intersections
 
         # merge data for intersecting geometries
         df1 = df1.reset_index(drop=True)
@@ -55,43 +55,49 @@
             left_on="__idx2",
             right_index=True,
             suffixes=("_1", "_2"),
         )
 
         return GeoDataFrame(dfinter, geometry=geom_intersect, crs=df1.crs)
     else:
-        return GeoDataFrame(
-            [],
-            columns=list(set(df1.columns).union(df2.columns)) + ["__idx1", "__idx2"],
-            crs=df1.crs,
+        result = df1.iloc[:0].merge(
+            df2.iloc[:0].drop(df2.geometry.name, axis=1),
+            left_index=True,
+            right_index=True,
+            suffixes=("_1", "_2"),
         )
+        result["__idx1"] = np.nan
+        result["__idx2"] = np.nan
+        return result[
+            result.columns.drop(df1.geometry.name).tolist() + [df1.geometry.name]
+        ]
 
 
 def _overlay_difference(df1, df2):
     """
     Overlay Difference operation used in overlay function
     """
     # spatial index query to find intersections
-    idx1, idx2 = df2.sindex.query_bulk(df1.geometry, predicate="intersects", sort=True)
+    idx1, idx2 = df2.sindex.query(df1.geometry, predicate="intersects", sort=True)
     idx1_unique, idx1_unique_indices = np.unique(idx1, return_index=True)
     idx2_split = np.split(idx2, idx1_unique_indices[1:])
     sidx = [
         idx2_split.pop(0) if idx in idx1_unique else []
         for idx in range(df1.geometry.size)
     ]
     # Create differences
     new_g = []
     for geom, neighbours in zip(df1.geometry, sidx):
         new = reduce(
             lambda x, y: x.difference(y), [geom] + list(df2.geometry.iloc[neighbours])
         )
         new_g.append(new)
     differences = GeoSeries(new_g, index=df1.index, crs=df1.crs)
-    poly_ix = differences.type.isin(["Polygon", "MultiPolygon"])
-    differences.loc[poly_ix] = differences[poly_ix].buffer(0)
+    poly_ix = differences.geom_type.isin(["Polygon", "MultiPolygon"])
+    differences.loc[poly_ix] = differences[poly_ix].make_valid()
     geom_diff = differences[~differences.is_empty].copy()
     dfdiff = df1[~differences.is_empty].copy()
     dfdiff[dfdiff._geometry_column_name] = geom_diff
     return dfdiff
 
 
 def _overlay_symmetric_diff(df1, df2):
@@ -129,15 +135,15 @@
     """
     dfinter = _overlay_intersection(df1, df2)
     dfsym = _overlay_symmetric_diff(df1, df2)
     dfunion = pd.concat([dfinter, dfsym], ignore_index=True, sort=False)
     # keep geometry column last
     columns = list(dfunion.columns)
     columns.remove("geometry")
-    columns = columns + ["geometry"]
+    columns.append("geometry")
     return dfunion.reindex(columns=columns)
 
 
 def overlay(df1, df2, how="intersection", keep_geom_type=None, make_valid=True):
     """Perform spatial overlay between two GeoDataFrames.
 
     Currently only supports data GeoDataFrames with uniform geometry types,
@@ -156,15 +162,15 @@
         'identity', 'symmetric_difference' or 'difference'.
     keep_geom_type : bool
         If True, return only geometries of the same geometry type as df1 has,
         if False, return all resulting geometries. Default is None,
         which will set keep_geom_type to True but warn upon dropping
         geometries.
     make_valid : bool, default True
-        If True, any invalid input geometries are corrected with a call to `buffer(0)`,
+        If True, any invalid input geometries are corrected with a call to make_valid(),
         if False, a `ValueError` is raised if any input geometries are invalid.
 
     Returns
     -------
     df : GeoDataFrame
         GeoDataFrame with new set of polygons and attributes
         resulting from the overlay
@@ -176,55 +182,56 @@
     ...                               Polygon([(2,2), (4,2), (4,4), (2,4)])])
     >>> polys2 = geopandas.GeoSeries([Polygon([(1,1), (3,1), (3,3), (1,3)]),
     ...                               Polygon([(3,3), (5,3), (5,5), (3,5)])])
     >>> df1 = geopandas.GeoDataFrame({'geometry': polys1, 'df1_data':[1,2]})
     >>> df2 = geopandas.GeoDataFrame({'geometry': polys2, 'df2_data':[1,2]})
 
     >>> geopandas.overlay(df1, df2, how='union')
-       df1_data  df2_data                                           geometry
-    0       1.0       1.0  POLYGON ((1.00000 2.00000, 2.00000 2.00000, 2....
-    1       2.0       1.0  POLYGON ((3.00000 2.00000, 2.00000 2.00000, 2....
-    2       2.0       2.0  POLYGON ((3.00000 4.00000, 4.00000 4.00000, 4....
-    3       1.0       NaN  POLYGON ((2.00000 1.00000, 2.00000 0.00000, 0....
-    4       2.0       NaN  MULTIPOLYGON (((3.00000 3.00000, 4.00000 3.000...
-    5       NaN       1.0  MULTIPOLYGON (((2.00000 2.00000, 3.00000 2.000...
-    6       NaN       2.0  POLYGON ((3.00000 4.00000, 3.00000 5.00000, 5....
+        df1_data  df2_data                                           geometry
+    0       1.0       1.0                POLYGON ((2 2, 2 1, 1 1, 1 2, 2 2))
+    1       2.0       1.0                POLYGON ((2 2, 2 3, 3 3, 3 2, 2 2))
+    2       2.0       2.0                POLYGON ((4 4, 4 3, 3 3, 3 4, 4 4))
+    3       1.0       NaN      POLYGON ((2 0, 0 0, 0 2, 1 2, 1 1, 2 1, 2 0))
+    4       2.0       NaN  MULTIPOLYGON (((3 4, 3 3, 2 3, 2 4, 3 4)), ((4...
+    5       NaN       1.0  MULTIPOLYGON (((2 3, 2 2, 1 2, 1 3, 2 3)), ((3...
+    6       NaN       2.0      POLYGON ((3 5, 5 5, 5 3, 4 3, 4 4, 3 4, 3 5))
 
     >>> geopandas.overlay(df1, df2, how='intersection')
-       df1_data  df2_data                                           geometry
-    0         1         1  POLYGON ((1.00000 2.00000, 2.00000 2.00000, 2....
-    1         2         1  POLYGON ((3.00000 2.00000, 2.00000 2.00000, 2....
-    2         2         2  POLYGON ((3.00000 4.00000, 4.00000 4.00000, 4....
+       df1_data  df2_data                             geometry
+    0         1         1  POLYGON ((2 2, 2 1, 1 1, 1 2, 2 2))
+    1         2         1  POLYGON ((2 2, 2 3, 3 3, 3 2, 2 2))
+    2         2         2  POLYGON ((4 4, 4 3, 3 3, 3 4, 4 4))
 
     >>> geopandas.overlay(df1, df2, how='symmetric_difference')
-       df1_data  df2_data                                           geometry
-    0       1.0       NaN  POLYGON ((2.00000 1.00000, 2.00000 0.00000, 0....
-    1       2.0       NaN  MULTIPOLYGON (((3.00000 3.00000, 4.00000 3.000...
-    2       NaN       1.0  MULTIPOLYGON (((2.00000 2.00000, 3.00000 2.000...
-    3       NaN       2.0  POLYGON ((3.00000 4.00000, 3.00000 5.00000, 5....
+        df1_data  df2_data                                           geometry
+    0       1.0       NaN      POLYGON ((2 0, 0 0, 0 2, 1 2, 1 1, 2 1, 2 0))
+    1       2.0       NaN  MULTIPOLYGON (((3 4, 3 3, 2 3, 2 4, 3 4)), ((4...
+    2       NaN       1.0  MULTIPOLYGON (((2 3, 2 2, 1 2, 1 3, 2 3)), ((3...
+    3       NaN       2.0      POLYGON ((3 5, 5 5, 5 3, 4 3, 4 4, 3 4, 3 5))
 
     >>> geopandas.overlay(df1, df2, how='difference')
                                                 geometry  df1_data
-    0  POLYGON ((2.00000 1.00000, 2.00000 0.00000, 0....         1
-    1  MULTIPOLYGON (((2.00000 3.00000, 2.00000 4.000...         2
+    0      POLYGON ((2 0, 0 0, 0 2, 1 2, 1 1, 2 1, 2 0))         1
+    1  MULTIPOLYGON (((3 4, 3 3, 2 3, 2 4, 3 4)), ((4...         2
 
     >>> geopandas.overlay(df1, df2, how='identity')
        df1_data  df2_data                                           geometry
-    0       1.0       1.0  POLYGON ((1.00000 2.00000, 2.00000 2.00000, 2....
-    1       2.0       1.0  POLYGON ((3.00000 2.00000, 2.00000 2.00000, 2....
-    2       2.0       2.0  POLYGON ((3.00000 4.00000, 4.00000 4.00000, 4....
-    3       1.0       NaN  POLYGON ((2.00000 1.00000, 2.00000 0.00000, 0....
-    4       2.0       NaN  MULTIPOLYGON (((3.00000 3.00000, 4.00000 3.000...
+    0       1.0       1.0                POLYGON ((2 2, 2 1, 1 1, 1 2, 2 2))
+    1       2.0       1.0                POLYGON ((2 2, 2 3, 3 3, 3 2, 2 2))
+    2       2.0       2.0                POLYGON ((4 4, 4 3, 3 3, 3 4, 4 4))
+    3       1.0       NaN      POLYGON ((2 0, 0 0, 0 2, 1 2, 1 1, 2 1, 2 0))
+    4       2.0       NaN  MULTIPOLYGON (((3 4, 3 3, 2 3, 2 4, 3 4)), ((4...
 
     See also
     --------
     sjoin : spatial join
+    GeoDataFrame.overlay : equivalent method
 
     Notes
-    ------
+    -----
     Every operation in GeoPandas is planar, i.e. the potential third
     dimension is not taken into account.
     """
     # Allowed operations
     allowed_hows = [
         "intersection",
         "union",
@@ -236,15 +243,15 @@
     if how not in allowed_hows:
         raise ValueError(
             "`how` was '{0}' but is expected to be in {1}".format(how, allowed_hows)
         )
 
     if isinstance(df1, GeoSeries) or isinstance(df2, GeoSeries):
         raise NotImplementedError(
-            "overlay currently only implemented for " "GeoDataFrames"
+            "overlay currently only implemented for GeoDataFrames"
         )
 
     if not _check_crs(df1, df2):
         _crs_mismatch_warn(df1, df2, stacklevel=3)
 
     if keep_geom_type is None:
         keep_geom_type = True
@@ -260,75 +267,129 @@
         lines_check = df.geom_type.isin(lines).any()
         points_check = df.geom_type.isin(points).any()
         if sum([poly_check, lines_check, points_check]) > 1:
             raise NotImplementedError(
                 "df{} contains mixed geometry types.".format(i + 1)
             )
 
+    if how == "intersection":
+        box_gdf1 = df1.total_bounds
+        box_gdf2 = df2.total_bounds
+
+        if not (
+            ((box_gdf1[0] <= box_gdf2[2]) and (box_gdf2[0] <= box_gdf1[2]))
+            and ((box_gdf1[1] <= box_gdf2[3]) and (box_gdf2[1] <= box_gdf1[3]))
+        ):
+            result = df1.iloc[:0].merge(
+                df2.iloc[:0].drop(df2.geometry.name, axis=1),
+                left_index=True,
+                right_index=True,
+                suffixes=("_1", "_2"),
+            )
+            return result[
+                result.columns.drop(df1.geometry.name).tolist() + [df1.geometry.name]
+            ]
+
     # Computations
     def _make_valid(df):
         df = df.copy()
         if df.geom_type.isin(polys).all():
             mask = ~df.geometry.is_valid
             col = df._geometry_column_name
             if make_valid:
-                df.loc[mask, col] = df.loc[mask, col].buffer(0)
+                df.loc[mask, col] = df.loc[mask, col].make_valid()
             elif mask.any():
                 raise ValueError(
                     "You have passed make_valid=False along with "
                     f"{mask.sum()} invalid input geometries. "
                     "Use make_valid=True or make sure that all geometries "
                     "are valid before using overlay."
                 )
         return df
 
     df1 = _make_valid(df1)
     df2 = _make_valid(df2)
 
-    with warnings.catch_warnings():  # CRS checked above, supress array-level warning
+    with warnings.catch_warnings():  # CRS checked above, suppress array-level warning
         warnings.filterwarnings("ignore", message="CRS mismatch between the CRS")
         if how == "difference":
-            return _overlay_difference(df1, df2)
+            result = _overlay_difference(df1, df2)
         elif how == "intersection":
             result = _overlay_intersection(df1, df2)
         elif how == "symmetric_difference":
             result = _overlay_symmetric_diff(df1, df2)
         elif how == "union":
             result = _overlay_union(df1, df2)
         elif how == "identity":
             dfunion = _overlay_union(df1, df2)
             result = dfunion[dfunion["__idx1"].notnull()].copy()
 
+        if how in ["intersection", "symmetric_difference", "union", "identity"]:
+            result.drop(["__idx1", "__idx2"], axis=1, inplace=True)
+
     if keep_geom_type:
-        key_order = result.keys()
-        exploded = result.reset_index(drop=True).explode()
-        exploded = exploded.reset_index(level=0)
+        geom_type = df1.geom_type.iloc[0]
+
+        # First we filter the geometry types inside GeometryCollections objects
+        # (e.g. GeometryCollection([polygon, point]) -> polygon)
+        # we do this separately on only the relevant rows, as this is an expensive
+        # operation (an expensive no-op for geometry types other than collections)
+        is_collection = result.geom_type == "GeometryCollection"
+        if is_collection.any():
+            geom_col = result._geometry_column_name
+            collections = result[[geom_col]][is_collection]
+
+            exploded = collections.reset_index(drop=True).explode(index_parts=True)
+            exploded = exploded.reset_index(level=0)
+
+            orig_num_geoms_exploded = exploded.shape[0]
+            if geom_type in polys:
+                exploded.loc[~exploded.geom_type.isin(polys), geom_col] = None
+            elif geom_type in lines:
+                exploded.loc[~exploded.geom_type.isin(lines), geom_col] = None
+            elif geom_type in points:
+                exploded.loc[~exploded.geom_type.isin(points), geom_col] = None
+            else:
+                raise TypeError(
+                    "`keep_geom_type` does not support {}.".format(geom_type)
+                )
+            num_dropped_collection = (
+                orig_num_geoms_exploded - exploded.geometry.isna().sum()
+            )
 
+            # level_0 created with above reset_index operation
+            # and represents the original geometry collections
+            # TODO avoiding dissolve to call union_all in this case could further
+            # improve performance (we only need to collect geometries in their
+            # respective Multi version)
+            dissolved = exploded.dissolve(by="level_0")
+            result.loc[is_collection, geom_col] = dissolved[geom_col].values
+        else:
+            num_dropped_collection = 0
+
+        # Now we filter all geometries (in theory we don't need to do this
+        # again for the rows handled above for GeometryCollections, but filtering
+        # them out is probably more expensive as simply including them when this
+        # is typically about only a few rows)
         orig_num_geoms = result.shape[0]
-        geom_type = df1.geom_type.iloc[0]
         if geom_type in polys:
-            exploded = exploded.loc[exploded.geom_type.isin(polys)]
+            result = result.loc[result.geom_type.isin(polys)]
         elif geom_type in lines:
-            exploded = exploded.loc[exploded.geom_type.isin(lines)]
+            result = result.loc[result.geom_type.isin(lines)]
         elif geom_type in points:
-            exploded = exploded.loc[exploded.geom_type.isin(points)]
+            result = result.loc[result.geom_type.isin(points)]
         else:
             raise TypeError("`keep_geom_type` does not support {}.".format(geom_type))
+        num_dropped = orig_num_geoms - result.shape[0]
 
-        # level_0 created with above reset_index operation
-        # and represents the original geometry collections
-        result = exploded.dissolve(by="level_0")[key_order]
-
-        if (result.shape[0] != orig_num_geoms) and keep_geom_type_warning:
-            num_dropped = orig_num_geoms - result.shape[0]
+        if (num_dropped > 0 or num_dropped_collection > 0) and keep_geom_type_warning:
             warnings.warn(
                 "`keep_geom_type=True` in overlay resulted in {} dropped "
                 "geometries of different geometry types than df1 has. "
                 "Set `keep_geom_type=False` to retain all "
-                "geometries".format(num_dropped),
+                "geometries".format(num_dropped + num_dropped_collection),
                 UserWarning,
                 stacklevel=2,
             )
 
     result.reset_index(drop=True, inplace=True)
-    result.drop(["__idx1", "__idx2"], axis=1, inplace=True)
     return result
```

### Comparing `geopandas-0.9.0/geopandas/tools/tests/test_clip.py` & `geopandas-1.0.0a1/geopandas/tools/tests/test_clip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,116 @@
 """Tests for the clip module."""
 
-import warnings
-
 import numpy as np
 
 import shapely
-from shapely.geometry import Polygon, Point, LineString, LinearRing, GeometryCollection
+from shapely.geometry import (
+    Polygon,
+    Point,
+    LineString,
+    LinearRing,
+    GeometryCollection,
+    MultiPoint,
+    box,
+)
 
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries, clip
+from geopandas._compat import HAS_PYPROJ
 
 from geopandas.testing import assert_geodataframe_equal, assert_geoseries_equal
 import pytest
 
+from geopandas.tools.clip import _mask_is_list_like_rectangle
 
-pytestmark = pytest.mark.skip_no_sindex
+mask_variants_single_rectangle = [
+    "single_rectangle_gdf",
+    "single_rectangle_gdf_list_bounds",
+    "single_rectangle_gdf_tuple_bounds",
+    "single_rectangle_gdf_array_bounds",
+]
+mask_variants_large_rectangle = [
+    "larger_single_rectangle_gdf",
+    "larger_single_rectangle_gdf_bounds",
+]
 
 
 @pytest.fixture
 def point_gdf():
     """Create a point GeoDataFrame."""
     pts = np.array([[2, 2], [3, 4], [9, 8], [-12, -15]])
-    gdf = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:4326")
+    gdf = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:3857")
     return gdf
 
 
 @pytest.fixture
 def pointsoutside_nooverlap_gdf():
     """Create a point GeoDataFrame. Its points are all outside the single
     rectangle, and its bounds are outside the single rectangle's."""
     pts = np.array([[5, 15], [15, 15], [15, 20]])
-    gdf = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:4326")
+    gdf = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:3857")
     return gdf
 
 
 @pytest.fixture
 def pointsoutside_overlap_gdf():
     """Create a point GeoDataFrame. Its points are all outside the single
     rectangle, and its bounds are overlapping the single rectangle's."""
     pts = np.array([[5, 15], [15, 15], [15, 5]])
-    gdf = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:4326")
+    gdf = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:3857")
     return gdf
 
 
 @pytest.fixture
 def single_rectangle_gdf():
     """Create a single rectangle for clipping."""
     poly_inters = Polygon([(0, 0), (0, 10), (10, 10), (10, 0), (0, 0)])
-    gdf = GeoDataFrame([1], geometry=[poly_inters], crs="EPSG:4326")
+    gdf = GeoDataFrame([1], geometry=[poly_inters], crs="EPSG:3857")
     gdf["attr2"] = "site-boundary"
     return gdf
 
 
 @pytest.fixture
+def single_rectangle_gdf_tuple_bounds(single_rectangle_gdf):
+    """Bounds of the created single rectangle"""
+    return tuple(single_rectangle_gdf.total_bounds)
+
+
+@pytest.fixture
+def single_rectangle_gdf_list_bounds(single_rectangle_gdf):
+    """Bounds of the created single rectangle"""
+    return list(single_rectangle_gdf.total_bounds)
+
+
+@pytest.fixture
+def single_rectangle_gdf_array_bounds(single_rectangle_gdf):
+    """Bounds of the created single rectangle"""
+    return single_rectangle_gdf.total_bounds
+
+
+@pytest.fixture
 def larger_single_rectangle_gdf():
     """Create a slightly larger rectangle for clipping.
     The smaller single rectangle is used to test the edge case where slivers
     are returned when you clip polygons. This fixture is larger which
     eliminates the slivers in the clip return.
     """
     poly_inters = Polygon([(-5, -5), (-5, 15), (15, 15), (15, -5), (-5, -5)])
-    gdf = GeoDataFrame([1], geometry=[poly_inters], crs="EPSG:4326")
+    gdf = GeoDataFrame([1], geometry=[poly_inters], crs="EPSG:3857")
     gdf["attr2"] = ["study area"]
     return gdf
 
 
 @pytest.fixture
+def larger_single_rectangle_gdf_bounds(larger_single_rectangle_gdf):
+    """Bounds of the created single rectangle"""
+    return tuple(larger_single_rectangle_gdf.total_bounds)
+
+
+@pytest.fixture
 def buffered_locations(point_gdf):
     """Buffer points to create a multi-polygon."""
     buffered_locs = point_gdf
     buffered_locs["geometry"] = buffered_locs.buffer(4)
     buffered_locs["type"] = "plot"
     return buffered_locs
 
@@ -84,306 +125,338 @@
 
 
 @pytest.fixture
 def two_line_gdf():
     """Create Line Objects For Testing"""
     linea = LineString([(1, 1), (2, 2), (3, 2), (5, 3)])
     lineb = LineString([(3, 4), (5, 7), (12, 2), (10, 5), (9, 7.5)])
-    gdf = GeoDataFrame([1, 2], geometry=[linea, lineb], crs="EPSG:4326")
+    gdf = GeoDataFrame([1, 2], geometry=[linea, lineb], crs="EPSG:3857")
     return gdf
 
 
 @pytest.fixture
 def multi_poly_gdf(donut_geometry):
     """Create a multi-polygon GeoDataFrame."""
-    multi_poly = donut_geometry.unary_union
-    out_df = GeoDataFrame(geometry=GeoSeries(multi_poly), crs="EPSG:4326")
+    multi_poly = donut_geometry.union_all()
+    out_df = GeoDataFrame(geometry=GeoSeries(multi_poly), crs="EPSG:3857")
     out_df["attr"] = ["pool"]
     return out_df
 
 
 @pytest.fixture
 def multi_line(two_line_gdf):
     """Create a multi-line GeoDataFrame.
     This GDF has one multiline and one regular line."""
     # Create a single and multi line object
-    multiline_feat = two_line_gdf.unary_union
+    multiline_feat = two_line_gdf.union_all()
     linec = LineString([(2, 1), (3, 1), (4, 1), (5, 2)])
-    out_df = GeoDataFrame(geometry=GeoSeries([multiline_feat, linec]), crs="EPSG:4326")
+    out_df = GeoDataFrame(geometry=GeoSeries([multiline_feat, linec]), crs="EPSG:3857")
     out_df["attr"] = ["road", "stream"]
     return out_df
 
 
 @pytest.fixture
 def multi_point(point_gdf):
     """Create a multi-point GeoDataFrame."""
-    multi_point = point_gdf.unary_union
+    multi_point = point_gdf.union_all()
     out_df = GeoDataFrame(
         geometry=GeoSeries(
             [multi_point, Point(2, 5), Point(-11, -14), Point(-10, -12)]
         ),
-        crs="EPSG:4326",
+        crs="EPSG:3857",
     )
     out_df["attr"] = ["tree", "another tree", "shrub", "berries"]
     return out_df
 
 
 @pytest.fixture
 def mixed_gdf():
     """Create a Mixed Polygon and LineString For Testing"""
-    point = Point([(2, 3), (11, 4), (7, 2), (8, 9), (1, 13)])
+    point = Point(2, 3)
     line = LineString([(1, 1), (2, 2), (3, 2), (5, 3), (12, 1)])
     poly = Polygon([(3, 4), (5, 2), (12, 2), (10, 5), (9, 7.5)])
     ring = LinearRing([(1, 1), (2, 2), (3, 2), (5, 3), (12, 1)])
     gdf = GeoDataFrame(
-        [1, 2, 3, 4], geometry=[point, poly, line, ring], crs="EPSG:4326"
+        [1, 2, 3, 4], geometry=[point, poly, line, ring], crs="EPSG:3857"
     )
     return gdf
 
 
 @pytest.fixture
 def geomcol_gdf():
     """Create a Mixed Polygon and LineString For Testing"""
-    point = Point([(2, 3), (11, 4), (7, 2), (8, 9), (1, 13)])
+    point = Point(2, 3)
     poly = Polygon([(3, 4), (5, 2), (12, 2), (10, 5), (9, 7.5)])
     coll = GeometryCollection([point, poly])
-    gdf = GeoDataFrame([1], geometry=[coll], crs="EPSG:4326")
+    gdf = GeoDataFrame([1], geometry=[coll], crs="EPSG:3857")
     return gdf
 
 
 @pytest.fixture
 def sliver_line():
     """Create a line that will create a point when clipped."""
     linea = LineString([(10, 5), (13, 5), (15, 5)])
     lineb = LineString([(1, 1), (2, 2), (3, 2), (5, 3), (12, 1)])
-    gdf = GeoDataFrame([1, 2], geometry=[linea, lineb], crs="EPSG:4326")
+    gdf = GeoDataFrame([1, 2], geometry=[linea, lineb], crs="EPSG:3857")
     return gdf
 
 
 def test_not_gdf(single_rectangle_gdf):
     """Non-GeoDataFrame inputs raise attribute errors."""
     with pytest.raises(TypeError):
         clip((2, 3), single_rectangle_gdf)
     with pytest.raises(TypeError):
-        clip(single_rectangle_gdf, (2, 3))
-
-
-def test_returns_gdf(point_gdf, single_rectangle_gdf):
-    """Test that function returns a GeoDataFrame (or GDF-like) object."""
-    out = clip(point_gdf, single_rectangle_gdf)
-    assert isinstance(out, GeoDataFrame)
-
-
-def test_returns_series(point_gdf, single_rectangle_gdf):
-    """Test that function returns a GeoSeries if GeoSeries is passed."""
-    out = clip(point_gdf.geometry, single_rectangle_gdf)
-    assert isinstance(out, GeoSeries)
+        clip(single_rectangle_gdf, "foobar")
+    with pytest.raises(TypeError):
+        clip(single_rectangle_gdf, (1, 2, 3))
+    with pytest.raises(TypeError):
+        clip(single_rectangle_gdf, (1, 2, 3, 4, 5))
 
 
 def test_non_overlapping_geoms():
     """Test that a bounding box returns empty if the extents don't overlap"""
     unit_box = Polygon([(0, 0), (0, 1), (1, 1), (1, 0), (0, 0)])
-    unit_gdf = GeoDataFrame([1], geometry=[unit_box], crs="EPSG:4326")
+    unit_gdf = GeoDataFrame([1], geometry=[unit_box], crs="EPSG:3857")
     non_overlapping_gdf = unit_gdf.copy()
     non_overlapping_gdf = non_overlapping_gdf.geometry.apply(
         lambda x: shapely.affinity.translate(x, xoff=20)
     )
     out = clip(unit_gdf, non_overlapping_gdf)
     assert_geodataframe_equal(out, unit_gdf.iloc[:0])
     out2 = clip(unit_gdf.geometry, non_overlapping_gdf)
     assert_geoseries_equal(out2, GeoSeries(crs=unit_gdf.crs))
 
 
-def test_clip_points(point_gdf, single_rectangle_gdf):
-    """Test clipping a points GDF with a generic polygon geometry."""
-    clip_pts = clip(point_gdf, single_rectangle_gdf)
-    pts = np.array([[2, 2], [3, 4], [9, 8]])
-    exp = GeoDataFrame([Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:4326")
-    assert_geodataframe_equal(clip_pts, exp)
-
-
-def test_clip_points_geom_col_rename(point_gdf, single_rectangle_gdf):
-    """Test clipping a points GDF with a generic polygon geometry."""
-    point_gdf_geom_col_rename = point_gdf.rename_geometry("geometry2")
-    clip_pts = clip(point_gdf_geom_col_rename, single_rectangle_gdf)
-    pts = np.array([[2, 2], [3, 4], [9, 8]])
-    exp = GeoDataFrame(
-        [Point(xy) for xy in pts],
-        columns=["geometry2"],
-        crs="EPSG:4326",
-        geometry="geometry2",
-    )
-    assert_geodataframe_equal(clip_pts, exp)
+@pytest.mark.parametrize("mask_fixture_name", mask_variants_single_rectangle)
+class TestClipWithSingleRectangleGdf:
+    @pytest.fixture
+    def mask(self, mask_fixture_name, request):
+        return request.getfixturevalue(mask_fixture_name)
+
+    def test_returns_gdf(self, point_gdf, mask):
+        """Test that function returns a GeoDataFrame (or GDF-like) object."""
+        out = clip(point_gdf, mask)
+        assert isinstance(out, GeoDataFrame)
+
+    def test_returns_series(self, point_gdf, mask):
+        """Test that function returns a GeoSeries if GeoSeries is passed."""
+        out = clip(point_gdf.geometry, mask)
+        assert isinstance(out, GeoSeries)
+
+    def test_clip_points(self, point_gdf, mask):
+        """Test clipping a points GDF with a generic polygon geometry."""
+        clip_pts = clip(point_gdf, mask)
+        pts = np.array([[2, 2], [3, 4], [9, 8]])
+        exp = GeoDataFrame(
+            [Point(xy) for xy in pts], columns=["geometry"], crs="EPSG:3857"
+        )
+        assert_geodataframe_equal(clip_pts, exp)
 
+    def test_clip_points_geom_col_rename(self, point_gdf, mask):
+        """Test clipping a points GDF with a generic polygon geometry."""
+        point_gdf_geom_col_rename = point_gdf.rename_geometry("geometry2")
+        clip_pts = clip(point_gdf_geom_col_rename, mask)
+        pts = np.array([[2, 2], [3, 4], [9, 8]])
+        exp = GeoDataFrame(
+            [Point(xy) for xy in pts],
+            columns=["geometry2"],
+            crs="EPSG:3857",
+            geometry="geometry2",
+        )
+        assert_geodataframe_equal(clip_pts, exp)
 
-def test_clip_poly(buffered_locations, single_rectangle_gdf):
-    """Test clipping a polygon GDF with a generic polygon geometry."""
-    clipped_poly = clip(buffered_locations, single_rectangle_gdf)
-    assert len(clipped_poly.geometry) == 3
-    assert all(clipped_poly.geom_type == "Polygon")
+    def test_clip_poly(self, buffered_locations, mask):
+        """Test clipping a polygon GDF with a generic polygon geometry."""
+        clipped_poly = clip(buffered_locations, mask)
+        assert len(clipped_poly.geometry) == 3
+        assert all(clipped_poly.geom_type == "Polygon")
+
+    def test_clip_poly_geom_col_rename(self, buffered_locations, mask):
+        """Test clipping a polygon GDF with a generic polygon geometry."""
+
+        poly_gdf_geom_col_rename = buffered_locations.rename_geometry("geometry2")
+        clipped_poly = clip(poly_gdf_geom_col_rename, mask)
+        assert len(clipped_poly.geometry) == 3
+        assert "geometry" not in clipped_poly.keys()
+        assert "geometry2" in clipped_poly.keys()
+
+    def test_clip_poly_series(self, buffered_locations, mask):
+        """Test clipping a polygon GDF with a generic polygon geometry."""
+        clipped_poly = clip(buffered_locations.geometry, mask)
+        assert len(clipped_poly) == 3
+        assert all(clipped_poly.geom_type == "Polygon")
+
+    def test_clip_multipoly_keep_geom_type(self, multi_poly_gdf, mask):
+        """Test a multi poly object where the return includes a sliver.
+        Also the bounds of the object should == the bounds of the clip object
+        if they fully overlap (as they do in these fixtures)."""
+        clipped = clip(multi_poly_gdf, mask, keep_geom_type=True)
+        expected_bounds = (
+            mask if _mask_is_list_like_rectangle(mask) else mask.total_bounds
+        )
+        assert np.array_equal(clipped.total_bounds, expected_bounds)
+        # Assert returned data is a not geometry collection
+        assert (clipped.geom_type.isin(["Polygon", "MultiPolygon"])).all()
+
+    def test_clip_multiline(self, multi_line, mask):
+        """Test that clipping a multiline feature with a poly returns expected
+        output."""
+        clipped = clip(multi_line, mask)
+        assert clipped.geom_type[0] == "MultiLineString"
+
+    def test_clip_multipoint(self, multi_point, mask):
+        """Clipping a multipoint feature with a polygon works as expected.
+        should return a geodataframe with a single multi point feature"""
+        clipped = clip(multi_point, mask)
+        assert clipped.geom_type[0] == "MultiPoint"
+        assert hasattr(clipped, "attr")
+        # All points should intersect the clip geom
+        assert len(clipped) == 2
+        clipped_mutltipoint = MultiPoint(
+            [
+                Point(2, 2),
+                Point(3, 4),
+                Point(9, 8),
+            ]
+        )
+        assert clipped.iloc[0].geometry.wkt == clipped_mutltipoint.wkt
+        shape_for_points = (
+            box(*mask) if _mask_is_list_like_rectangle(mask) else mask.union_all()
+        )
+        assert all(clipped.intersects(shape_for_points))
 
+    def test_clip_lines(self, two_line_gdf, mask):
+        """Test what happens when you give the clip_extent a line GDF."""
+        clip_line = clip(two_line_gdf, mask)
+        assert len(clip_line.geometry) == 2
+
+    def test_mixed_geom(self, mixed_gdf, mask):
+        """Test clipping a mixed GeoDataFrame"""
+        clipped = clip(mixed_gdf, mask)
+        assert (
+            clipped.geom_type[0] == "Point"
+            and clipped.geom_type[1] == "Polygon"
+            and clipped.geom_type[2] == "LineString"
+        )
 
-def test_clip_poly_geom_col_rename(buffered_locations, single_rectangle_gdf):
-    """Test clipping a polygon GDF with a generic polygon geometry."""
+    def test_mixed_series(self, mixed_gdf, mask):
+        """Test clipping a mixed GeoSeries"""
+        clipped = clip(mixed_gdf.geometry, mask)
+        assert (
+            clipped.geom_type[0] == "Point"
+            and clipped.geom_type[1] == "Polygon"
+            and clipped.geom_type[2] == "LineString"
+        )
 
-    poly_gdf_geom_col_rename = buffered_locations.rename_geometry("geometry2")
-    clipped_poly = clip(poly_gdf_geom_col_rename, single_rectangle_gdf)
-    assert len(clipped_poly.geometry) == 3
-    assert "geometry" not in clipped_poly.keys()
-    assert "geometry2" in clipped_poly.keys()
+    def test_clip_with_line_extra_geom(self, sliver_line, mask):
+        """When the output of a clipped line returns a geom collection,
+        and keep_geom_type is True, no geometry collections should be returned."""
+        clipped = clip(sliver_line, mask, keep_geom_type=True)
+        assert len(clipped.geometry) == 1
+        # Assert returned data is a not geometry collection
+        assert not (clipped.geom_type == "GeometryCollection").any()
+
+    def test_clip_no_box_overlap(self, pointsoutside_nooverlap_gdf, mask):
+        """Test clip when intersection is empty and boxes do not overlap."""
+        clipped = clip(pointsoutside_nooverlap_gdf, mask)
+        assert len(clipped) == 0
+
+    def test_clip_box_overlap(self, pointsoutside_overlap_gdf, mask):
+        """Test clip when intersection is empty and boxes do overlap."""
+        clipped = clip(pointsoutside_overlap_gdf, mask)
+        assert len(clipped) == 0
+
+    def test_warning_extra_geoms_mixed(self, mixed_gdf, mask):
+        """Test the correct warnings are raised if keep_geom_type is
+        called on a mixed GDF"""
+        with pytest.warns(UserWarning):
+            clip(mixed_gdf, mask, keep_geom_type=True)
+
+    def test_warning_geomcoll(self, geomcol_gdf, mask):
+        """Test the correct warnings are raised if keep_geom_type is
+        called on a GDF with GeometryCollection"""
+        with pytest.warns(UserWarning):
+            clip(geomcol_gdf, mask, keep_geom_type=True)
 
 
-def test_clip_poly_series(buffered_locations, single_rectangle_gdf):
-    """Test clipping a polygon GDF with a generic polygon geometry."""
-    clipped_poly = clip(buffered_locations.geometry, single_rectangle_gdf)
-    assert len(clipped_poly) == 3
-    assert all(clipped_poly.geom_type == "Polygon")
+def test_clip_line_keep_slivers(sliver_line, single_rectangle_gdf):
+    """Test the correct output if a point is returned
+    from a line only geometry type."""
+    clipped = clip(sliver_line, single_rectangle_gdf)
+    # Assert returned data is a geometry collection given sliver geoms
+    assert "Point" == clipped.geom_type[0]
+    assert "LineString" == clipped.geom_type[1]
 
 
 def test_clip_multipoly_keep_slivers(multi_poly_gdf, single_rectangle_gdf):
     """Test a multi poly object where the return includes a sliver.
     Also the bounds of the object should == the bounds of the clip object
     if they fully overlap (as they do in these fixtures)."""
     clipped = clip(multi_poly_gdf, single_rectangle_gdf)
     assert np.array_equal(clipped.total_bounds, single_rectangle_gdf.total_bounds)
     # Assert returned data is a geometry collection given sliver geoms
     assert "GeometryCollection" in clipped.geom_type[0]
 
 
-def test_clip_multipoly_keep_geom_type(multi_poly_gdf, single_rectangle_gdf):
-    """Test a multi poly object where the return includes a sliver.
-    Also the bounds of the object should == the bounds of the clip object
-    if they fully overlap (as they do in these fixtures)."""
-    clipped = clip(multi_poly_gdf, single_rectangle_gdf, keep_geom_type=True)
-    assert np.array_equal(clipped.total_bounds, single_rectangle_gdf.total_bounds)
-    # Assert returned data is a not geometry collection
-    assert (clipped.geom_type == "Polygon").any()
-
-
-def test_clip_single_multipoly_no_extra_geoms(
-    buffered_locations, larger_single_rectangle_gdf
-):
-    """When clipping a multi-polygon feature, no additional geom types
-    should be returned."""
-    multi = buffered_locations.dissolve(by="type").reset_index()
-    clipped = clip(multi, larger_single_rectangle_gdf)
-    assert clipped.geom_type[0] == "Polygon"
-
-
-def test_clip_multiline(multi_line, single_rectangle_gdf):
-    """Test that clipping a multiline feature with a poly returns expected output."""
-    clipped = clip(multi_line, single_rectangle_gdf)
-    assert clipped.geom_type[0] == "MultiLineString"
-
-
-def test_clip_multipoint(single_rectangle_gdf, multi_point):
-    """Clipping a multipoint feature with a polygon works as expected.
-    should return a geodataframe with a single multi point feature"""
-    clipped = clip(multi_point, single_rectangle_gdf)
-    assert clipped.geom_type[0] == "MultiPoint"
-    assert hasattr(clipped, "attr")
-    # All points should intersect the clip geom
-    assert all(clipped.intersects(single_rectangle_gdf.unary_union))
-
-
-def test_clip_lines(two_line_gdf, single_rectangle_gdf):
-    """Test what happens when you give the clip_extent a line GDF."""
-    clip_line = clip(two_line_gdf, single_rectangle_gdf)
-    assert len(clip_line.geometry) == 2
-
-
-def test_clip_with_multipolygon(buffered_locations, single_rectangle_gdf):
-    """Test clipping a polygon with a multipolygon."""
-    multi = buffered_locations.dissolve(by="type").reset_index()
-    clipped = clip(single_rectangle_gdf, multi)
-    assert clipped.geom_type[0] == "Polygon"
-
-
-def test_mixed_geom(mixed_gdf, single_rectangle_gdf):
-    """Test clipping a mixed GeoDataFrame"""
-    clipped = clip(mixed_gdf, single_rectangle_gdf)
-    assert (
-        clipped.geom_type[0] == "Point"
-        and clipped.geom_type[1] == "Polygon"
-        and clipped.geom_type[2] == "LineString"
-    )
-
-
-def test_mixed_series(mixed_gdf, single_rectangle_gdf):
-    """Test clipping a mixed GeoSeries"""
-    clipped = clip(mixed_gdf.geometry, single_rectangle_gdf)
-    assert (
-        clipped.geom_type[0] == "Point"
-        and clipped.geom_type[1] == "Polygon"
-        and clipped.geom_type[2] == "LineString"
-    )
-
-
-def test_clip_warning_no_extra_geoms(buffered_locations, single_rectangle_gdf):
-    """Test a user warning is provided if no new geometry types are found."""
-    with pytest.warns(UserWarning):
-        clip(buffered_locations, single_rectangle_gdf, True)
-        warnings.warn(
-            "keep_geom_type was called when no extra geometry types existed.",
-            UserWarning,
-        )
+@pytest.mark.skipif(not HAS_PYPROJ, reason="pyproj not available")
+def test_warning_crs_mismatch(point_gdf, single_rectangle_gdf):
+    with pytest.warns(UserWarning, match="CRS mismatch between the CRS"):
+        clip(point_gdf, single_rectangle_gdf.to_crs(4326))
 
 
 def test_clip_with_polygon(single_rectangle_gdf):
     """Test clip when using a shapely object"""
     polygon = Polygon([(0, 0), (5, 12), (10, 0), (0, 0)])
     clipped = clip(single_rectangle_gdf, polygon)
     exp_poly = polygon.intersection(
         Polygon([(0, 0), (0, 10), (10, 10), (10, 0), (0, 0)])
     )
-    exp = GeoDataFrame([1], geometry=[exp_poly], crs="EPSG:4326")
+    exp = GeoDataFrame([1], geometry=[exp_poly], crs="EPSG:3857")
     exp["attr2"] = "site-boundary"
     assert_geodataframe_equal(clipped, exp)
 
 
-def test_clip_with_line_extra_geom(single_rectangle_gdf, sliver_line):
-    """When the output of a clipped line returns a geom collection,
-    and keep_geom_type is True, no geometry collections should be returned."""
-    clipped = clip(sliver_line, single_rectangle_gdf, keep_geom_type=True)
-    assert len(clipped.geometry) == 1
-    # Assert returned data is a not geometry collection
-    assert not (clipped.geom_type == "GeometryCollection").any()
-
-
-def test_clip_line_keep_slivers(single_rectangle_gdf, sliver_line):
-    """Test the correct output if a point is returned
-    from a line only geometry type."""
-    clipped = clip(sliver_line, single_rectangle_gdf)
-    # Assert returned data is a geometry collection given sliver geoms
-    assert "Point" == clipped.geom_type[0]
-    assert "LineString" == clipped.geom_type[1]
+def test_clip_with_multipolygon(buffered_locations, single_rectangle_gdf):
+    """Test clipping a polygon with a multipolygon."""
+    multi = buffered_locations.dissolve(by="type").reset_index()
+    clipped = clip(single_rectangle_gdf, multi)
+    assert clipped.geom_type[0] == "Polygon"
 
 
-def test_clip_no_box_overlap(pointsoutside_nooverlap_gdf, single_rectangle_gdf):
-    """Test clip when intersection is empty and boxes do not overlap."""
-    clipped = clip(pointsoutside_nooverlap_gdf, single_rectangle_gdf)
-    assert len(clipped) == 0
-
-
-def test_clip_box_overlap(pointsoutside_overlap_gdf, single_rectangle_gdf):
-    """Test clip when intersection is emtpy and boxes do overlap."""
-    clipped = clip(pointsoutside_overlap_gdf, single_rectangle_gdf)
-    assert len(clipped) == 0
-
-
-def test_warning_extra_geoms_mixed(single_rectangle_gdf, mixed_gdf):
-    """Test the correct warnings are raised if keep_geom_type is
-    called on a mixed GDF"""
-    with pytest.warns(UserWarning):
-        clip(mixed_gdf, single_rectangle_gdf, keep_geom_type=True)
-
-
-def test_warning_geomcoll(single_rectangle_gdf, geomcol_gdf):
-    """Test the correct warnings are raised if keep_geom_type is
-    called on a GDF with GeometryCollection"""
-    with pytest.warns(UserWarning):
-        clip(geomcol_gdf, single_rectangle_gdf, keep_geom_type=True)
+@pytest.mark.parametrize(
+    "mask_fixture_name",
+    mask_variants_large_rectangle,
+)
+def test_clip_single_multipoly_no_extra_geoms(
+    buffered_locations, mask_fixture_name, request
+):
+    """When clipping a multi-polygon feature, no additional geom types
+    should be returned."""
+    masks = request.getfixturevalue(mask_fixture_name)
+    multi = buffered_locations.dissolve(by="type").reset_index()
+    clipped = clip(multi, masks)
+    assert clipped.geom_type[0] == "Polygon"
 
 
-def test_warning_crs_mismatch(point_gdf, single_rectangle_gdf):
-    with pytest.warns(UserWarning, match="CRS mismatch between the CRS"):
-        clip(point_gdf, single_rectangle_gdf.to_crs(3857))
+@pytest.mark.filterwarnings("ignore:All-NaN slice encountered")
+@pytest.mark.parametrize(
+    "mask",
+    [
+        Polygon(),
+        (np.nan,) * 4,
+        (np.nan, 0, np.nan, 1),
+        GeoSeries([Polygon(), Polygon()], crs="EPSG:3857"),
+        GeoSeries([Polygon(), Polygon()], crs="EPSG:3857").to_frame(),
+        GeoSeries([], crs="EPSG:3857"),
+        GeoSeries([], crs="EPSG:3857").to_frame(),
+    ],
+)
+def test_clip_empty_mask(buffered_locations, mask):
+    """Test that clipping with empty mask returns an empty result."""
+    clipped = clip(buffered_locations, mask)
+    assert_geodataframe_equal(
+        clipped,
+        GeoDataFrame([], columns=["geometry", "type"], crs="EPSG:3857"),
+        check_index_type=False,
+    )
+    clipped = clip(buffered_locations.geometry, mask)
+    assert_geoseries_equal(clipped, GeoSeries([], crs="EPSG:3857"))
```

### Comparing `geopandas-0.9.0/geopandas/tools/util.py` & `geopandas-1.0.0a1/geopandas/tools/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     elif isinstance(x, pd.Series):
         x = list(x)
 
     # We cannot create GeometryCollection here so all types
     # must be the same. If there is more than one element,
     # they cannot be Multi*, i.e., can't pass in combination of
     # Point and MultiPoint... or even just MultiPoint
-    t = x[0].type
-    if not all(g.type == t for g in x):
-        raise ValueError("Geometry type must be homogenous")
+    t = x[0].geom_type
+    if not all(g.geom_type == t for g in x):
+        raise ValueError("Geometry type must be homogeneous")
     if len(x) > 1 and t.startswith("Multi"):
         raise ValueError("Cannot collect {0}. Must have single geometries".format(t))
 
     if len(x) == 1 and (t.startswith("Multi") or not multi):
         # If there's only one single part geom and we're not forcing to
         # multi, then just return it
         return x[0]
```

### Comparing `geopandas-0.9.0/versioneer.py` & `geopandas-1.0.0a1/versioneer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,63 @@
-
-# Version: 0.16
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.3, 3.4, 3.5, and pypy
-* [![Latest Version]
-(https://pypip.in/version/versioneer/badge.svg?style=flat)
-](https://pypi.python.org/pypi/versioneer/)
-* [![Build Status]
-(https://travis-ci.org/warner/python-versioneer.png?branch=master)
-](https://travis-ci.org/warner/python-versioneer)
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -57,15 +81,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -84,135 +108,15 @@
 that configures it. This overrides several distutils/setuptools commands to
 compute the version when invoked, and changes `setup.py build` and `setup.py
 sdist` to replace `_version.py` with a small static file that contains just
 the generated version data.
 
 ## Installation
 
-First, decide on values for the following configuration variables:
-
-* `VCS`: the version control system you use. Currently accepts "git".
-
-* `style`: the style of version string to be produced. See "Styles" below for
-  details. Defaults to "pep440", which looks like
-  `TAG[+DISTANCE.gSHORTHASH[.dirty]]`.
-
-* `versionfile_source`:
-
-  A project-relative pathname into which the generated version strings should
-  be written. This is usually a `_version.py` next to your project's main
-  `__init__.py` file, so it can be imported at runtime. If your project uses
-  `src/myproject/__init__.py`, this should be `src/myproject/_version.py`.
-  This file should be checked in to your VCS as usual: the copy created below
-  by `setup.py setup_versioneer` will include code that parses expanded VCS
-  keywords in generated tarballs. The 'build' and 'sdist' commands will
-  replace it with a copy that has just the calculated version string.
-
-  This must be set even if your project does not have any modules (and will
-  therefore never import `_version.py`), since "setup.py sdist" -based trees
-  still need somewhere to record the pre-calculated version strings. Anywhere
-  in the source tree should do. If there is a `__init__.py` next to your
-  `_version.py`, the `setup.py setup_versioneer` command (described below)
-  will append some `__version__`-setting assignments, if they aren't already
-  present.
-
-* `versionfile_build`:
-
-  Like `versionfile_source`, but relative to the build directory instead of
-  the source directory. These will differ when your setup.py uses
-  'package_dir='. If you have `package_dir={'myproject': 'src/myproject'}`,
-  then you will probably have `versionfile_build='myproject/_version.py'` and
-  `versionfile_source='src/myproject/_version.py'`.
-
-  If this is set to None, then `setup.py build` will not attempt to rewrite
-  any `_version.py` in the built tree. If your project does not have any
-  libraries (e.g. if it only builds a script), then you should use
-  `versionfile_build = None`. To actually use the computed version string,
-  your `setup.py` will need to override `distutils.command.build_scripts`
-  with a subclass that explicitly inserts a copy of
-  `versioneer.get_version()` into your script file. See
-  `test/demoapp-script-only/setup.py` for an example.
-
-* `tag_prefix`:
-
-  a string, like 'PROJECTNAME-', which appears at the start of all VCS tags.
-  If your tags look like 'myproject-1.2.0', then you should use
-  tag_prefix='myproject-'. If you use unprefixed tags like '1.2.0', this
-  should be an empty string, using either `tag_prefix=` or `tag_prefix=''`.
-
-* `parentdir_prefix`:
-
-  a optional string, frequently the same as tag_prefix, which appears at the
-  start of all unpacked tarball filenames. If your tarball unpacks into
-  'myproject-1.2.0', this should be 'myproject-'. To disable this feature,
-  just omit the field from your `setup.cfg`.
-
-This tool provides one script, named `versioneer`. That script has one mode,
-"install", which writes a copy of `versioneer.py` into the current directory
-and runs `versioneer.py setup` to finish the installation.
-
-To versioneer-enable your project:
-
-* 1: Modify your `setup.cfg`, adding a section named `[versioneer]` and
-  populating it with the configuration values you decided earlier (note that
-  the option names are not case-sensitive):
-
-  ````
-  [versioneer]
-  VCS = git
-  style = pep440
-  versionfile_source = src/myproject/_version.py
-  versionfile_build = myproject/_version.py
-  tag_prefix =
-  parentdir_prefix = myproject-
-  ````
-
-* 2: Run `versioneer install`. This will do the following:
-
-  * copy `versioneer.py` into the top of your source tree
-  * create `_version.py` in the right place (`versionfile_source`)
-  * modify your `__init__.py` (if one exists next to `_version.py`) to define
-    `__version__` (by calling a function from `_version.py`)
-  * modify your `MANIFEST.in` to include both `versioneer.py` and the
-    generated `_version.py` in sdist tarballs
-
-  `versioneer install` will complain about any problems it finds with your
-  `setup.py` or `setup.cfg`. Run it multiple times until you have fixed all
-  the problems.
-
-* 3: add a `import versioneer` to your setup.py, and add the following
-  arguments to the setup() call:
-
-        version=versioneer.get_version(),
-        cmdclass=versioneer.get_cmdclass(),
-
-* 4: commit these changes to your VCS. To make sure you won't forget,
-  `versioneer install` will mark everything it touched for addition using
-  `git add`. Don't forget to add `setup.py` and `setup.cfg` too.
-
-## Post-Installation Usage
-
-Once established, all uses of your tree from a VCS checkout should get the
-current version string. All generated tarballs should include an embedded
-version string (so users who unpack them will not need a VCS tool installed).
-
-If you distribute your project through PyPI, then the release process should
-boil down to two steps:
-
-* 1: git tag 1.0
-* 2: python setup.py register sdist upload
-
-If you distribute it through github (i.e. users use github to generate
-tarballs with `git archive`), the process is:
-
-* 1: git tag 1.0
-* 2: git push; git push --tags
-
-Versioneer will report "0+untagged.NUMCOMMITS.gHASH" until your tree has at
-least one tag in its history.
+See [INSTALL.md](./INSTALL.md) for detailed installation instructions.
 
 ## Version-String Flavors
 
 Code which uses Versioneer can learn about its version string at runtime by
 importing `_version` from your main `__init__.py` file and running the
 `get_versions()` function. From the "outside" (e.g. in `setup.py`), you can
 import the top-level `versioneer.py` and run `get_versions()`.
@@ -225,14 +129,18 @@
   string. The default "pep440" style yields strings like `0.11`,
   `0.11+2.g1076c97`, or `0.11+2.g1076c97.dirty`. See the "Styles" section
   below for alternative styles.
 
 * `['full-revisionid']`: detailed revision identifier. For Git, this is the
   full SHA1 commit id, e.g. "1076c978a8d3cfc70f408fe5974aa6c092c949ac".
 
+* `['date']`: Date and time of the latest `HEAD` commit. For Git, it is the
+  commit date in ISO 8601 format. This will be None if the date is not
+  available.
+
 * `['dirty']`: a boolean, True if the tree has uncommitted changes. Note that
   this is only accurate if run in a VCS checkout, otherwise it is likely to
   be False or None
 
 * `['error']`: if the version string could not be computed, this will be set
   to a string describing the problem, otherwise it will be None. It may be
   useful to throw an exception in setup.py if this is set, to avoid e.g.
@@ -263,265 +171,402 @@
 TAG[+DISTANCE.gHEX[.dirty]] , using information from `git describe --tags
 --dirty --always`. For example "0.11+2.g1076c97.dirty" indicates that the
 tree is like the "1076c97" commit but has uncommitted changes (".dirty"), and
 that this commit is two revisions ("+2") beyond the "0.11" tag. For released
 software (exactly equal to a known tag), the identifier will only contain the
 stripped tag, e.g. "0.11".
 
-Other styles are available. See details.md in the Versioneer source tree for
-descriptions.
+Other styles are available. See [details.md](details.md) in the Versioneer
+source tree for descriptions.
 
 ## Debugging
 
 Versioneer tries to avoid fatal errors: if something goes wrong, it will tend
 to return a version of "0+unknown". To investigate the problem, run `setup.py
 version`, which will run the version-lookup code in a verbose mode, and will
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
+## Known Limitations
+
+Some situations are known to cause problems for Versioneer. This details the
+most significant ones. More can be found on Github
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
+
+### Subprojects
+
+Versioneer has limited support for source trees in which `setup.py` is not in
+the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
+two common reasons why `setup.py` might not be in the root:
+
+* Source trees which contain multiple subprojects, such as
+  [Buildbot](https://github.com/buildbot/buildbot), which contains both
+  "master" and "slave" subprojects, each with their own `setup.py`,
+  `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
+  distributions (and upload multiple independently-installable tarballs).
+* Source trees whose main purpose is to contain a C library, but which also
+  provide bindings to Python (and perhaps other languages) in subdirectories.
+
+Versioneer will look for `.git` in parent directories, and most operations
+should get the right version string. However `pip` and `setuptools` have bugs
+and implementation details which frequently cause `pip install .` from a
+subproject directory to fail to find a correct version string (so it usually
+defaults to `0+unknown`).
+
+`pip install --editable .` should work correctly. `setup.py install` might
+work too.
+
+Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
+some later version.
+
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
+this issue. The discussion in
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
+issue from the Versioneer side in more detail.
+[pip PR#3176](https://github.com/pypa/pip/pull/3176) and
+[pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
+pip to let Versioneer work correctly.
+
+Versioneer-0.16 and earlier only looked for a `.git` directory next to the
+`setup.cfg`, so subprojects were completely unsupported with those releases.
+
+### Editable installs with setuptools <= 18.5
+
+`setup.py develop` and `pip install --editable .` allow you to install a
+project into a virtualenv once, then continue editing the source code (and
+test) without re-installing after every change.
+
+"Entry-point scripts" (`setup(entry_points={"console_scripts": ..})`) are a
+convenient way to specify executable scripts that should be installed along
+with the python package.
+
+These both work as expected when using modern setuptools. When using
+setuptools-18.5 or earlier, however, certain operations will cause
+`pkg_resources.DistributionNotFound` errors when running the entrypoint
+script, which must be resolved by re-installing the package. This happens
+when the install happens with one version, then the egg_info data is
+regenerated while a different version is checked out. Many setup.py commands
+cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
+a different virtualenv), so this can be surprising.
+
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
+this one, but upgrading to a newer version of setuptools should probably
+resolve it.
+
+
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
-### Upgrading to 0.16
-
-Nothing special.
-
-### Upgrading to 0.15
-
-Starting with this version, Versioneer is configured with a `[versioneer]`
-section in your `setup.cfg` file. Earlier versions required the `setup.py` to
-set attributes on the `versioneer` module immediately after import. The new
-version will refuse to run (raising an exception during import) until you
-have provided the necessary `setup.cfg` section.
-
-In addition, the Versioneer package provides an executable named
-`versioneer`, and the installation process is driven by running `versioneer
-install`. In 0.14 and earlier, the executable was named
-`versioneer-installer` and was run without an argument.
-
-### Upgrading to 0.14
-
-0.14 changes the format of the version string. 0.13 and earlier used
-hyphen-separated strings like "0.11-2-g1076c97-dirty". 0.14 and beyond use a
-plus-separated "local version" section strings, with dot-separated
-components, like "0.11+2.g1076c97". PEP440-strict tools did not like the old
-format, but should be ok with the new one.
-
-### Upgrading from 0.11 to 0.12
-
-Nothing special.
-
-### Upgrading from 0.10 to 0.11
-
-You must add a `versioneer.VCS = "git"` to your `setup.py` before re-running
-`setup.py setup_versioneer`. This will enable the use of additional
-version-control systems (SVN, etc) in the future.
-
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
 src/git/ . The top-level `versioneer.py` script is assembled from these
 components by running make-versioneer.py . In the future, make-versioneer.py
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
+
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-from __future__ import print_function
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import NoReturn
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
 
-def get_root():
+
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        if os.path.splitext(me)[0] != os.path.splitext(versioneer_py)[0]:
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
+        vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(my_path), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, "rb") as fobj:
+                pp = tomllib.load(fobj)
+            section = pp["tool"]["versioneer"]
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
+
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section["VCS"]
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
+
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
+
 
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
 
-def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen(
+                [command] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
+            )
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
-            return None
+            return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
-        return None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+        return None, None
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
-        return None
-    return stdout
-LONG_VERSION_PY['git'] = '''
+            print("stdout was %s" % stdout)
+        return None, process.returncode
+    return stdout, process.returncode
+
+
+LONG_VERSION_PY[
+    "git"
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.16 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
-    keywords = {"refnames": git_refnames, "full": git_full}
+    git_date = "%(DOLLAR)sFormat:%%ci%(DOLLAR)s"
+    keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
+
 
-def get_config():
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -531,187 +576,285 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
-    def decorate(f):
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
-            return None
+            return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
-        return None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+        return None, None
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
-        return None
-    return stdout
+            print("stdout was %%s" %% stdout)
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
-    Source tarballs conventionally unpack into a directory that includes
-    both the project name and a version string.
+    Source tarballs conventionally unpack into a directory that includes both
+    the project name and a version string. We will also support searching up
+    two directory levels for an appropriately named parent directory
     """
-    dirname = os.path.basename(root)
-    if not dirname.startswith(parentdir_prefix):
-        if verbose:
-            print("guessing rootdir is '%%s', but '%%s' doesn't start with "
-                  "prefix '%%s'" %% (root, dirname, parentdir_prefix))
-        raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
-    return {"version": dirname[len(parentdir_prefix):],
-            "full-revisionid": None,
-            "dirty": False, "error": None}
+    rootdirs = []
+
+    for _ in range(3):
+        dirname = os.path.basename(root)
+        if dirname.startswith(parentdir_prefix):
+            return {"version": dirname[len(parentdir_prefix):],
+                    "full-revisionid": None,
+                    "dirty": False, "error": None, "date": None}
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
+
+    if verbose:
+        print("Tried directories %%s but none started with prefix %%s" %%
+              (str(rootdirs), parentdir_prefix))
+    raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
+    date = keywords.get("date")
+    if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
+        # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
+        # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
+        # -like" string, which we must then edit to make compliant), because
+        # it's been around since git-1.5.3, and it's too difficult to
+        # discover which version we're using, or to work around using an
+        # older one.
+        date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
-            print("discarding '%%s', no digits" %% ",".join(refs-tags))
+            print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None
-                    }
+                    "dirty": False, "error": None,
+                    "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags"}
+            "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
-    if not os.path.exists(os.path.join(root, ".git")):
-        if verbose:
-            print("no .git in %%s" %% root)
-        raise NotThisMethod("no .git directory")
-
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
+
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
+    if rc != 0:
+        if verbose:
+            print("Directory %%s not under git control" %% root)
+        raise NotThisMethod("'git rev-parse --git-dir' returned error")
+
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out = run_command(GITS, ["describe", "--tags", "--dirty",
-                                      "--always", "--long",
-                                      "--match", "%%s*" %% tag_prefix],
-                               cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -720,15 +863,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -745,29 +888,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
+
+    # commit date: see ISO-8601 comment in git_versions_from_keywords()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
+    pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -784,31 +933,79 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -827,20 +1024,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -849,15 +1075,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -869,15 +1095,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -889,45 +1115,51 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
-                "error": pieces["error"]}
+                "error": pieces["error"],
+                "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None}
+            "dirty": pieces["dirty"], "error": None,
+            "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -940,20 +1172,21 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
-                "error": "unable to find root of source tree"}
+                "error": "unable to find root of source tree",
+                "date": None}
 
     try:
         pieces = git_pieces_from_vcs(cfg.tag_prefix, root, verbose)
         return render(pieces, cfg.style)
     except NotThisMethod:
         pass
 
@@ -961,279 +1194,390 @@
         if cfg.parentdir_prefix:
             return versions_from_parentdir(cfg.parentdir_prefix, root, verbose)
     except NotThisMethod:
         pass
 
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
-            "error": "unable to compute version"}
+            "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
+    date = keywords.get("date")
+    if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
+        # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
+        # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
+        # -like" string, which we must then edit to make compliant), because
+        # it's been around since git-1.5.3, and it's too difficult to
+        # discover which version we're using, or to work around using an
+        # older one.
+        date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
-            print("discarding '%s', no digits" % ",".join(refs-tags))
+            print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r"\d", r):
+                continue
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None
-                    }
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags"}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str, root: str, verbose: bool, runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
-    if not os.path.exists(os.path.join(root, ".git")):
-        if verbose:
-            print("no .git in %s" % root)
-        raise NotThisMethod("no .git directory")
-
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
+
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
+    if rc != 0:
+        if verbose:
+            print("Directory %s not under git control" % root)
+        raise NotThisMethod("'git rev-parse --git-dir' returned error")
+
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out = run_command(GITS, ["describe", "--tags", "--dirty",
-                                      "--always", "--long",
-                                      "--match", "%s*" % tag_prefix],
-                               cwd=root)
+    describe_out, rc = runner(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            f"{tag_prefix}[[:digit:]]*",
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            # unparsable. Maybe git-describe is misbehaving?
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
+
+    # commit date: see ISO-8601 comment in git_versions_from_keywords()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
+    pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
-    for export-time keyword substitution.
+    for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
-    Source tarballs conventionally unpack into a directory that includes
-    both the project name and a version string.
+    Source tarballs conventionally unpack into a directory that includes both
+    the project name and a version string. We will also support searching up
+    two directory levels for an appropriately named parent directory
     """
-    dirname = os.path.basename(root)
-    if not dirname.startswith(parentdir_prefix):
-        if verbose:
-            print("guessing rootdir is '%s', but '%s' doesn't start with "
-                  "prefix '%s'" % (root, dirname, parentdir_prefix))
-        raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
-    return {"version": dirname[len(parentdir_prefix):],
-            "full-revisionid": None,
-            "dirty": False, "error": None}
+    rootdirs = []
+
+    for _ in range(3):
+        dirname = os.path.basename(root)
+        if dirname.startswith(parentdir_prefix):
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
+
+    if verbose:
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
+    raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
+
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.16) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
-import sys
 
 version_json = '''
 %s
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+    )
+    if not mo:
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1243,38 +1587,84 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1293,20 +1683,49 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1315,15 +1734,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1335,15 +1754,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1355,66 +1774,79 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"]}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1460,148 +1892,290 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version"}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools/distutils subclasses used by Versioneer."""
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
+            print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
+    #  pip install:
+    #   copies source tree to a tempdir before running egg_info/etc
+    #   if .git isn't copied too, 'git describe' will fail
+    #   then does setup.py bdist_wheel, or sometimes setup.py install
+    #  setup.py egg_info -> ?
+
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
 
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if "build_py" in cmds:
+        _build_py: Any = cmds["build_py"]
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
+    if "build_ext" in cmds:
+        _build_ext: Any = cmds["build_ext"]
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self) -> None:
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
+
+        # nczeczulin reports that py2exe won't like the pep440-style string
+        # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
+        # setup(console=[{
+        #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
+        #   "product_version": versioneer.get_version(),
+        #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
+    if "py2exe" in sys.modules:  # py2exe enabled?
+        try:
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
+        except ImportError:
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
+
+        class cmd_py2exe(_py2exe):
+            def run(self) -> None:
+                root = get_root()
+                cfg = get_config_from_root(root)
+                versions = get_versions()
+                target_versionfile = cfg.versionfile_source
+                print("UPDATING %s" % target_versionfile)
+                write_to_version_file(target_versionfile, versions)
+
+                _py2exe.run(self)
+                os.unlink(target_versionfile)
+                with open(cfg.versionfile_source, "w") as f:
+                    LONG = LONG_VERSION_PY[cfg.VCS]
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
+        cmds["py2exe"] = cmd_py2exe
+
+    # sdist farms its file list building out to egg_info
+    if "egg_info" in cmds:
+        _egg_info: Any = cmds["egg_info"]
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append("versioneer.py")
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/")
+                for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
+
+    cmds["egg_info"] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if "sdist" in cmds:
+        _sdist: Any = cmds["sdist"]
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1636,104 +2210,85 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
+
 
-def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+def do_setup() -> int:
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
+        if isinstance(e, (OSError, configparser.NoSectionError)):
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
-    # .gitattributes to mark _version.py for export-time keyword
+    # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -1761,14 +2316,19 @@
         print("You should remove lines like 'versioneer.VCS = ' and")
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
+
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

