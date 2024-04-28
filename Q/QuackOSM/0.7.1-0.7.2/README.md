# Comparing `tmp/quackosm-0.7.1.tar.gz` & `tmp/quackosm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quackosm-0.7.1.tar", last modified: Fri Apr 26 00:20:06 2024, max compression
+gzip compressed data, was "quackosm-0.7.2.tar", last modified: Sun Apr 28 17:24:01 2024, max compression
```

## Comparing `quackosm-0.7.1.tar` & `quackosm-0.7.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0    11339 2024-04-26 00:19:40.357647 quackosm-0.7.1/LICENSE
--rw-r--r--   0        0        0    27879 2024-04-26 00:19:40.357647 quackosm-0.7.1/README.md
--rw-r--r--   0        0        0     4378 2024-04-26 00:20:06.373754 quackosm-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      560 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/__init__.py
--rw-r--r--   0        0        0      464 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/__main__.py
--rw-r--r--   0        0        0      127 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/_constants.py
--rw-r--r--   0        0        0      181 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/_exceptions.py
--rw-r--r--   0        0        0     6497 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/_osm_tags_filters.py
--rw-r--r--   0        0        0     1188 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/_osm_way_polygon_features.py
--rw-r--r--   0        0        0    12674 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/_rich_progress.py
--rw-r--r--   0        0        0      717 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/_typing.py
--rw-r--r--   0        0        0    24446 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/cli.py
--rw-r--r--   0        0        0     1875 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/conftest.py
--rw-r--r--   0        0        0    52502 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/functions.py
--rw-r--r--   0        0        0    19193 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/osm_extracts/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/osm_extracts/_poly_parser.py
--rw-r--r--   0        0        0     2941 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/osm_extracts/bbbike.py
--rw-r--r--   0        0        0      251 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/osm_extracts/extract.py
--rw-r--r--   0        0        0     1709 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/osm_extracts/geofabrik.py
--rw-r--r--   0        0        0     4376 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/osm_extracts/osm_fr.py
--rw-r--r--   0        0        0     3362 2024-04-26 00:19:40.365647 quackosm-0.7.1/quackosm/osm_way_polygon_features.json
--rw-r--r--   0        0        0   116504 2024-04-26 00:19:40.369647 quackosm-0.7.1/quackosm/pbf_file_reader.py
--rw-r--r--   0        0        0       33 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/base/__init__.py
--rw-r--r--   0        0        0      746 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/base/conftest.py
--rw-r--r--   0        0        0    24831 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/base/test_cli.py
--rw-r--r--   0        0        0     5422 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/base/test_osm_extracts.py
--rw-r--r--   0        0        0    29285 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/base/test_osm_tags_filtering.py
--rw-r--r--   0        0        0    36504 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/base/test_pbf_file_reader.py
--rw-r--r--   0        0        0       43 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/benchmark/__init__.py
--rw-r--r--   0        0        0      945 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/benchmark/test_big_file.py
--rw-r--r--   0        0        0     1472 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/optional_imports/test_optional_cli_dependency.py
--rw-r--r--   0        0        0      342 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0    91717 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/test_files/monaco_boundary.geojson
--rw-r--r--   0        0        0      112 2024-04-26 00:19:40.369647 quackosm-0.7.1/tests/test_files/osm_tags_filter.json
--rw-r--r--   0        0        0    29715 1970-01-01 00:00:00.000000 quackosm-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-04-28 17:23:35.371569 quackosm-0.7.2/LICENSE
+-rw-r--r--   0        0        0    27879 2024-04-28 17:23:35.371569 quackosm-0.7.2/README.md
+-rw-r--r--   0        0        0     4378 2024-04-28 17:24:01.651726 quackosm-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      560 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/__init__.py
+-rw-r--r--   0        0        0      464 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/__main__.py
+-rw-r--r--   0        0        0      127 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_constants.py
+-rw-r--r--   0        0        0      181 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_exceptions.py
+-rw-r--r--   0        0        0     6497 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_osm_tags_filters.py
+-rw-r--r--   0        0        0     1188 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_osm_way_polygon_features.py
+-rw-r--r--   0        0        0    12674 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_rich_progress.py
+-rw-r--r--   0        0        0      717 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_typing.py
+-rw-r--r--   0        0        0    24446 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/cli.py
+-rw-r--r--   0        0        0     2031 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/conftest.py
+-rw-r--r--   0        0        0    52502 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/functions.py
+-rw-r--r--   0        0        0    19193 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/__init__.py
+-rw-r--r--   0        0        0     2320 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/_poly_parser.py
+-rw-r--r--   0        0        0     2941 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/bbbike.py
+-rw-r--r--   0        0        0      251 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/extract.py
+-rw-r--r--   0        0        0     1709 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/geofabrik.py
+-rw-r--r--   0        0        0     4376 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/osm_fr.py
+-rw-r--r--   0        0        0     3362 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_way_polygon_features.json
+-rw-r--r--   0        0        0   108664 2024-04-28 17:23:35.383570 quackosm-0.7.2/quackosm/pbf_file_reader.py
+-rw-r--r--   0        0        0       33 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/conftest.py
+-rw-r--r--   0        0        0    24831 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/test_cli.py
+-rw-r--r--   0        0        0     5422 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/test_osm_extracts.py
+-rw-r--r--   0        0        0    29285 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/test_osm_tags_filtering.py
+-rw-r--r--   0        0        0    36504 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/test_pbf_file_reader.py
+-rw-r--r--   0        0        0       43 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/benchmark/__init__.py
+-rw-r--r--   0        0        0      945 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/benchmark/test_big_file.py
+-rw-r--r--   0        0        0      238 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/conftest.py
+-rw-r--r--   0        0        0     1472 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/optional_imports/test_optional_cli_dependency.py
+-rw-r--r--   0        0        0      342 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0    91717 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/monaco_boundary.geojson
+-rw-r--r--   0        0        0      112 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/osm_tags_filter.json
+-rw-r--r--   0        0        0    29715 1970-01-01 00:00:00.000000 quackosm-0.7.2/PKG-INFO
```

### Comparing `quackosm-0.7.1/LICENSE` & `quackosm-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/README.md` & `quackosm-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/pyproject.toml` & `quackosm-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "QuackOSM"
-version = "0.7.1"
+version = "0.7.2"
 description = "An open-source tool for reading OpenStreetMap PBF files using DuckDB"
 authors = [
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
 ]
 dependencies = [
     "geopandas",
     "shapely>=2",
@@ -185,15 +185,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.7.1"
+current_version = "0.7.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `quackosm-0.7.1/quackosm/__init__.py` & `quackosm-0.7.2/quackosm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     convert_pbf_to_gpq,
     get_features_gdf,
     get_features_gdf_from_geometry,
 )
 from quackosm.pbf_file_reader import PbfFileReader
 
 __app_name__ = "QuackOSM"
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 __all__ = [
     "PbfFileReader",
     "convert_pbf_to_gpq",
     "convert_geometry_to_gpq",
     "get_features_gdf",
     "get_features_gdf_from_geometry",
```

### Comparing `quackosm-0.7.1/quackosm/_osm_tags_filters.py` & `quackosm-0.7.2/quackosm/_osm_tags_filters.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/_osm_way_polygon_features.py` & `quackosm-0.7.2/quackosm/_osm_way_polygon_features.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/_rich_progress.py` & `quackosm-0.7.2/quackosm/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/_typing.py` & `quackosm-0.7.2/quackosm/_typing.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/cli.py` & `quackosm-0.7.2/quackosm/cli.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/conftest.py` & `quackosm-0.7.2/quackosm/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Fixtures for doctests."""
 
+import shutil
 import sys
 import urllib.request
 from pathlib import Path
 
 import pytest
 
 LFS_DIRECTORY_URL = "https://github.com/kraina-ai/srai-test-files/raw/main/files/"
 
+EXTRACTS_NAMES = ["monaco", "kiribati", "maldives"]
+
 
 @pytest.fixture(autouse=True)
 def add_pbf_files(doctest_namespace):  # type: ignore
     """Download PBF files used in doctests."""
-    extracts = ["monaco", "kiribati", "maldives"]
-    download_directory = Path(__file__).parent / "files"
+    download_directory = Path("files")
     download_directory.mkdir(parents=True, exist_ok=True)
-    for extract_name in extracts:
+    for extract_name in EXTRACTS_NAMES:
         pbf_file_download_url = LFS_DIRECTORY_URL + f"{extract_name}-latest.osm.pbf"
         pbf_file_path = download_directory / f"{extract_name}.osm.pbf"
+        geofabrik_pbf_file_path = download_directory / f"Geofabrik_{extract_name}.osm.pbf"
         urllib.request.urlretrieve(pbf_file_download_url, pbf_file_path)
         doctest_namespace[f"{extract_name}_pbf_path"] = pbf_file_path
+        shutil.copy(pbf_file_path, geofabrik_pbf_file_path)
 
 
 @pytest.fixture  # type: ignore
 def optional_packages() -> list[str]:
     """Get a list with optional packages."""
     return [
         "rich",
```

### Comparing `quackosm-0.7.1/quackosm/functions.py` & `quackosm-0.7.2/quackosm/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         │ way/952068832    │ {attraction=water_…  │ LINESTRING (7.4221748 43.7343815, 7.422173…  │
         │ way/952419569    │ {highway=primary, …  │ LINESTRING (7.4171229 43.7316079, 7.417117…  │
         │ way/952419570    │ {highway=primary, …  │ LINESTRING (7.4171473 43.7315034, 7.417166…  │
         │ way/952419571    │ {highway=primary, …  │ LINESTRING (7.4171671 43.731656, 7.4171486…  │
         │ way/952419572    │ {highway=primary, …  │ LINESTRING (7.4173054 43.7316813, 7.417276…  │
         │ way/952419573    │ {highway=primary, …  │ LINESTRING (7.4173897 43.7316435, 7.417372…  │
         ├──────────────────┴──────────────────────┴──────────────────────────────────────────────┤
-        │ 1388 rows (20 shown)                                                                   │
+        │ 1384 rows (20 shown)                                                                   │
         └────────────────────────────────────────────────────────────────────────────────────────┘
 
         Making sure that you are using specific OSM extract source - here Geofabrik.
 
         >>> gpq_path = qosm.convert_geometry_to_gpq(
         ...     from_wkt(wkt),
         ...     osm_extract_source='Geofabrik',
@@ -399,15 +399,15 @@
         │ way/952068832    │ {attraction=water_…  │ LINESTRING (7.4221748 43.7343815, 7.422173…  │
         │ way/952419569    │ {highway=primary, …  │ LINESTRING (7.4171229 43.7316079, 7.417117…  │
         │ way/952419570    │ {highway=primary, …  │ LINESTRING (7.4171473 43.7315034, 7.417166…  │
         │ way/952419571    │ {highway=primary, …  │ LINESTRING (7.4171671 43.731656, 7.4171486…  │
         │ way/952419572    │ {highway=primary, …  │ LINESTRING (7.4173054 43.7316813, 7.417276…  │
         │ way/952419573    │ {highway=primary, …  │ LINESTRING (7.4173897 43.7316435, 7.417372…  │
         ├──────────────────┴──────────────────────┴──────────────────────────────────────────────┤
-        │ 1388 rows (20 shown)                                                                   │
+        │ 1384 rows (20 shown)                                                                   │
         └────────────────────────────────────────────────────────────────────────────────────────┘
     """
     return PbfFileReader(
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
@@ -692,15 +692,15 @@
         ...                                        ...                                           ...
         way/952419569     {'highway': 'primary', 'j...  LINESTRING (7.41712 43.73161, 7.41712 43....
         way/952419570     {'highway': 'primary', 'j...  LINESTRING (7.41715 43.73150, 7.41717 43....
         way/952419571     {'highway': 'primary', 'j...  LINESTRING (7.41717 43.73166, 7.41715 43....
         way/952419572     {'highway': 'primary', 'j...  LINESTRING (7.41731 43.73168, 7.41728 43....
         way/952419573     {'highway': 'primary', 'j...  LINESTRING (7.41739 43.73164, 7.41737 43....
         <BLANKLINE>
-        [1388 rows x 2 columns]
+        [1384 rows x 2 columns]
 
         Making sure that you are using specific OSM extract source - here Geofabrik.
 
         >>> qosm.get_features_gdf_from_geometry(
         ...     from_wkt(wkt),
         ...     osm_extract_source='Geofabrik',
         ... ).sort_index()
@@ -714,15 +714,15 @@
         ...                                        ...                                           ...
         way/952419569     {'highway': 'primary', 'j...   LINESTRING (7.41712 43.73161, 7.41712 43...
         way/952419570     {'highway': 'primary', 'j...   LINESTRING (7.41715 43.73150, 7.41717 43...
         way/952419571     {'highway': 'primary', 'j...   LINESTRING (7.41717 43.73166, 7.41715 43...
         way/952419572     {'highway': 'primary', 'j...   LINESTRING (7.41731 43.73168, 7.41728 43...
         way/952419573     {'highway': 'primary', 'j...   LINESTRING (7.41739 43.73164, 7.41737 43...
         <BLANKLINE>
-        [1388 rows x 2 columns]
+        [1384 rows x 2 columns]
     """
     return PbfFileReader(
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
```

### Comparing `quackosm-0.7.1/quackosm/osm_extracts/__init__.py` & `quackosm-0.7.2/quackosm/osm_extracts/__init__.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/osm_extracts/_poly_parser.py` & `quackosm-0.7.2/quackosm/osm_extracts/_poly_parser.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/osm_extracts/bbbike.py` & `quackosm-0.7.2/quackosm/osm_extracts/bbbike.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/osm_extracts/geofabrik.py` & `quackosm-0.7.2/quackosm/osm_extracts/geofabrik.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/osm_extracts/osm_fr.py` & `quackosm-0.7.2/quackosm/osm_extracts/osm_fr.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/osm_way_polygon_features.json` & `quackosm-0.7.2/quackosm/osm_way_polygon_features.json`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/quackosm/pbf_file_reader.py` & `quackosm-0.7.2/quackosm/pbf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1974,28 +1974,26 @@
             FROM ({valid_relation_parts_parquet.sql_query()})
             WHERE ref_role = 'inner'
             """
         )
         relation_inner_parts_parquet = self._save_parquet_file_with_geometry(
             relation=relation_inner_parts,
             file_path=self.tmp_dir_path / "relation_inner_parts",
-            fix_geometries=True,
             step_name="Saving relations inner parts",
         )
         relation_outer_parts = self.connection.sql(
             f"""
             SELECT id, geometry_id, ST_MakePolygon(geometry) geometry
             FROM ({valid_relation_parts_parquet.sql_query()})
             WHERE ref_role = 'outer'
             """
         )
         relation_outer_parts_parquet = self._save_parquet_file_with_geometry(
             relation=relation_outer_parts,
             file_path=self.tmp_dir_path / "relation_outer_parts",
-            fix_geometries=True,
             step_name="Saving relations outer parts",
         )
         relation_outer_parts_with_holes = self.connection.sql(
             f"""
             SELECT
                 og.id,
                 og.geometry_id,
@@ -2058,121 +2056,30 @@
 
     def _save_parquet_file_with_geometry(
         self,
         relation: "duckdb.DuckDBPyRelation",
         file_path: Path,
         step_name: str,
         with_minor_step: bool = False,
-        fix_geometries: bool = False,
     ) -> "duckdb.DuckDBPyRelation":
-        if not fix_geometries:
-            with self.task_progress_tracker.get_spinner(step_name, with_minor_step=with_minor_step):
-                self.connection.sql(
-                    f"""
-                    COPY (
-                        SELECT
-                            * EXCLUDE (geometry), ST_AsWKB(geometry) geometry_wkb
-                        FROM ({relation.sql_query()})
-                    ) TO '{file_path}' (
-                        FORMAT 'parquet',
-                        PER_THREAD_OUTPUT true,
-                        ROW_GROUP_SIZE 25000,
-                        COMPRESSION '{self.parquet_compression}'
-                    )
-                    """
+        with self.task_progress_tracker.get_spinner(step_name, with_minor_step=with_minor_step):
+            self.connection.sql(
+                f"""
+                COPY (
+                    SELECT
+                        * EXCLUDE (geometry), ST_AsWKB(ST_MakeValid(geometry)) geometry_wkb
+                    FROM ({relation.sql_query()})
+                ) TO '{file_path}' (
+                    FORMAT 'parquet',
+                    PER_THREAD_OUTPUT true,
+                    ROW_GROUP_SIZE 25000,
+                    COMPRESSION '{self.parquet_compression}'
                 )
-        else:
-            valid_path = file_path / "valid"
-            invalid_path = file_path / "invalid"
-            fixed_path = file_path / "fixed"
-
-            valid_path.mkdir(parents=True, exist_ok=True)
-            invalid_path.mkdir(parents=True, exist_ok=True)
-            fixed_path.mkdir(parents=True, exist_ok=True)
-
-            # Save valid features
-            with self.task_progress_tracker.get_spinner(
-                f"{step_name} - valid geometries", with_minor_step=True
-            ):
-                self.connection.sql(
-                    f"""
-                    COPY (
-                        SELECT
-                            * EXCLUDE (geometry), ST_AsWKB(geometry) geometry_wkb
-                        FROM ({relation.sql_query()})
-                        WHERE ST_IsValid(geometry)
-                    ) TO '{valid_path}' (
-                        FORMAT 'parquet',
-                        PER_THREAD_OUTPUT true,
-                        ROW_GROUP_SIZE 25000,
-                        COMPRESSION '{self.parquet_compression}'
-                    )
-                    """
-                )
-
-            # Save invalid features
-            with self.task_progress_tracker.get_spinner(
-                f"{step_name} - invalid geometries", next_step="minor"
-            ):
-                self.connection.sql(
-                    f"""
-                    COPY (
-                        SELECT
-                            * EXCLUDE (geometry), ST_AsWKB(geometry) geometry_wkb,
-                            floor(
-                                row_number() OVER () / {self.rows_per_group}
-                            )::INTEGER as "group",
-                        FROM ({relation.sql_query()})
-                        WHERE NOT ST_IsValid(geometry)
-                    ) TO '{invalid_path}' (
-                        FORMAT 'parquet',
-                        PARTITION_BY ("group"),
-                        ROW_GROUP_SIZE 25000,
-                        COMPRESSION '{self.parquet_compression}'
-                    )
-                    """
-                )
-
-            # Fix invalid features
-            total_groups = 0
-            while (invalid_path / f"group={total_groups}").exists():
-                total_groups += 1
-
-            if total_groups > 0:
-                with self.task_progress_tracker.get_bar(
-                    f"{step_name} - fixing invalid geometries", next_step="minor"
-                ) as bar:
-                    for group_id in bar.track(range(total_groups)):
-                        current_invalid_features_group_path = invalid_path / f"group={group_id}"
-                        current_invalid_features_group_table = pq.read_table(
-                            current_invalid_features_group_path
-                        ).drop("group")
-                        valid_geometry_column = ga.as_wkb(
-                            ga.to_geopandas(
-                                ga.with_crs(
-                                    current_invalid_features_group_table.column("geometry_wkb"),
-                                    WGS84_CRS,
-                                )
-                            ).make_valid(),
-                        )
-                        current_invalid_features_group_table = (
-                            current_invalid_features_group_table.drop("geometry_wkb")
-                        )
-
-                        current_invalid_features_group_table = (
-                            current_invalid_features_group_table.append_column(
-                                "geometry_wkb", valid_geometry_column
-                            )
-                        )
-                        pq.write_table(
-                            current_invalid_features_group_table,
-                            fixed_path / f"data_{group_id}.parquet",
-                        )
-
-            self._delete_directories(invalid_path)
+                """
+            )
 
         return self.connection.sql(
             f"""
             SELECT * EXCLUDE (geometry_wkb), ST_GeomFromWKB(geometry_wkb) geometry
             FROM read_parquet('{file_path}/**')
             """
         )
@@ -2200,157 +2107,75 @@
             """
         )
 
         grouped_features = self._parse_features_relation_to_groups(
             unioned_features, keep_all_tags=keep_all_tags, explode_tags=explode_tags
         )
 
-        valid_features_full_relation = self.connection.sql(
+        features_full_relation = self.connection.sql(
             f"""
-            SELECT * FROM ({grouped_features.sql_query()})
-            WHERE ST_IsValid(geometry)
+            SELECT
+                * EXCLUDE (geometry),
+                ST_MakeValid(geometry) geometry
+            FROM ({grouped_features.sql_query()})
             """
         )
 
-        valid_features_parquet_path = self.tmp_dir_path / "osm_valid_elements"
-        valid_features_parquet_relation = self._save_parquet_file_with_geometry(
-            valid_features_full_relation,
-            valid_features_parquet_path,
-            step_name="Saving valid features",
-            with_minor_step=True,
+        features_parquet_path = self.tmp_dir_path / "osm_valid_elements"
+        self._save_parquet_file_with_geometry(
+            features_full_relation,
+            features_parquet_path,
+            step_name="Saving all features",
         )
 
-        valid_features_parquet_table = pq.read_table(valid_features_parquet_path)
+        features_parquet_table = pq.read_table(features_parquet_path)
 
-        is_empty = valid_features_parquet_table.num_rows == 0
+        is_empty = features_parquet_table.num_rows == 0
 
         if not is_empty and save_as_wkt:
             geometry_column = ga.as_wkt(
-                ga.with_crs(valid_features_parquet_table.column("geometry_wkb"), WGS84_CRS)
+                ga.with_crs(features_parquet_table.column("geometry_wkb"), WGS84_CRS)
             )
         elif not is_empty:
             geometry_column = ga.as_wkb(
-                ga.with_crs(valid_features_parquet_table.column("geometry_wkb"), WGS84_CRS)
+                ga.with_crs(features_parquet_table.column("geometry_wkb"), WGS84_CRS)
             )
         elif save_as_wkt:
             geometry_column = ga.as_wkt(gpd.GeoSeries([], crs=WGS84_CRS))
         else:
             geometry_column = ga.as_wkb(gpd.GeoSeries([], crs=WGS84_CRS))
 
-        valid_features_parquet_table = valid_features_parquet_table.append_column(
+        features_parquet_table = features_parquet_table.append_column(
             GEOMETRY_COLUMN, geometry_column
         ).drop("geometry_wkb")
 
-        parquet_tables = [valid_features_parquet_table]
-
-        invalid_features_full_relation = self.connection.sql(
-            f"""
-            SELECT * FROM ({grouped_features.sql_query()}) a
-            ANTI JOIN ({valid_features_parquet_relation.sql_query()}) b
-            ON a.feature_id = b.feature_id
-            """
-        )
-
-        total_features = parsed_geometries.count("feature_id").fetchone()[0]
-
-        valid_features = valid_features_parquet_relation.count("feature_id").fetchone()[0]
-
-        invalid_features = total_features - valid_features
-
-        if invalid_features > 0:
-            with self.task_progress_tracker.get_spinner(
-                "Grouping invalid features", next_step="minor"
-            ):
-                groups = floor(invalid_features / self.rows_per_group)
-                grouped_invalid_features_result_parquet = (
-                    self.tmp_dir_path / "osm_invalid_elements_grouped"
-                )
-                self.connection.sql(
-                    f"""
-                    COPY (
-                        SELECT
-                            * EXCLUDE (geometry), ST_AsWKB(geometry) geometry_wkb,
-                            floor(
-                                row_number() OVER () / {self.rows_per_group}
-                            )::INTEGER as "group",
-                        FROM ({invalid_features_full_relation.sql_query()})
-                    ) TO '{grouped_invalid_features_result_parquet}' (
-                        FORMAT 'parquet',
-                        PARTITION_BY ("group"),
-                        ROW_GROUP_SIZE 25000,
-                        COMPRESSION '{self.parquet_compression}'
-                    )
-                    """
-                )
-
-            with self.task_progress_tracker.get_bar(
-                "Fixing invalid features", next_step="minor"
-            ) as bar:
-                for group in bar.track(range(groups + 1)):
-                    current_invalid_features_group_path = (
-                        grouped_invalid_features_result_parquet / f"group={group}"
-                    )
-                    current_invalid_features_group_table = pq.read_table(
-                        current_invalid_features_group_path
-                    ).drop("group")
-                    if save_as_wkt:
-                        valid_geometry_column = ga.as_wkt(
-                            ga.to_geopandas(
-                                ga.with_crs(
-                                    current_invalid_features_group_table.column("geometry_wkb"),
-                                    WGS84_CRS,
-                                )
-                            ).make_valid()
-                        )
-                    else:
-                        valid_geometry_column = ga.as_wkb(
-                            ga.to_geopandas(
-                                ga.with_crs(
-                                    current_invalid_features_group_table.column("geometry_wkb"),
-                                    WGS84_CRS,
-                                )
-                            ).make_valid()
-                        )
-
-                    current_invalid_features_group_table = (
-                        current_invalid_features_group_table.append_column(
-                            GEOMETRY_COLUMN, valid_geometry_column
-                        )
-                    )
-                    current_invalid_features_group_table = (
-                        current_invalid_features_group_table.drop("geometry_wkb")
-                    )
-                    parquet_tables.append(current_invalid_features_group_table)
-
-        joined_parquet_table: pa.Table = pa.concat_tables(parquet_tables)
-
-        is_empty = joined_parquet_table.num_rows == 0
+        is_empty = features_parquet_table.num_rows == 0
 
         empty_columns = []
-        for column_name in joined_parquet_table.column_names:
+        for column_name in features_parquet_table.column_names:
             if column_name in (FEATURES_INDEX, GEOMETRY_COLUMN):
                 continue
             if (
                 is_empty
                 or pa.compute.all(
-                    pa.compute.is_null(joined_parquet_table.column(column_name))
+                    pa.compute.is_null(features_parquet_table.column(column_name))
                 ).as_py()
             ):
                 empty_columns.append(column_name)
 
         if empty_columns:
-            joined_parquet_table = joined_parquet_table.drop(empty_columns)
+            features_parquet_table = features_parquet_table.drop(empty_columns)
 
         if save_as_wkt:
             with self.task_progress_tracker.get_spinner("Saving final parquet file"):
-                pq.write_table(joined_parquet_table, save_file_path)
+                pq.write_table(features_parquet_table, save_file_path)
         else:
             with self.task_progress_tracker.get_spinner("Saving final geoparquet file"):
                 io.write_geoparquet_table(
-                    joined_parquet_table, save_file_path, primary_geometry_column=GEOMETRY_COLUMN
+                    features_parquet_table, save_file_path, primary_geometry_column=GEOMETRY_COLUMN
                 )
 
     def _generate_osm_tags_sql_select(
         self, parsed_geometries: "duckdb.DuckDBPyRelation", keep_all_tags: bool, explode_tags: bool
     ) -> list[str]:
         """Prepare features filter clauses based on tags filter."""
         osm_tag_keys_select_clauses = []
```

### Comparing `quackosm-0.7.1/tests/base/conftest.py` & `quackosm-0.7.2/tests/base/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/base/test_cli.py` & `quackosm-0.7.2/tests/base/test_cli.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/base/test_osm_extracts.py` & `quackosm-0.7.2/tests/base/test_osm_extracts.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/base/test_osm_tags_filtering.py` & `quackosm-0.7.2/tests/base/test_osm_tags_filtering.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/base/test_pbf_file_reader.py` & `quackosm-0.7.2/tests/base/test_pbf_file_reader.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/benchmark/test_big_file.py` & `quackosm-0.7.2/tests/benchmark/test_big_file.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/optional_imports/test_optional_cli_dependency.py` & `quackosm-0.7.2/tests/optional_imports/test_optional_cli_dependency.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `quackosm-0.7.2/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `quackosm-0.7.2/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `quackosm-0.7.2/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/test_files/monaco.osm.pbf` & `quackosm-0.7.2/tests/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/tests/test_files/monaco_boundary.geojson` & `quackosm-0.7.2/tests/test_files/monaco_boundary.geojson`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.1/PKG-INFO` & `quackosm-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuackOSM
-Version: 0.7.1
+Version: 0.7.2
 Summary: An open-source tool for reading OpenStreetMap PBF files using DuckDB
 Author-Email: Kamil Raczycki <kraczycki@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: QuackOSM Version: 0.7.1 Summary: An open-source
+Metadata-Version: 2.1 Name: QuackOSM Version: 0.7.2 Summary: An open-source
 tool for reading OpenStreetMap PBF files using DuckDB Author-Email: Kamil
 Raczycki
 kraina.ai> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
```

