# Comparing `tmp/vollseg_napari_trackmate-2.5.6.tar.gz` & `tmp/vollseg_napari_trackmate-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vollseg_napari_trackmate-2.5.6.tar", last modified: Sat Apr 27 19:41:16 2024, max compression
+gzip compressed data, was "vollseg_napari_trackmate-2.5.7.tar", last modified: Sun Apr 28 11:03:24 2024, max compression
```

## Comparing `vollseg_napari_trackmate-2.5.6.tar` & `vollseg_napari_trackmate-2.5.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.368697 vollseg_napari_trackmate-2.5.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.372696 vollseg_napari_trackmate-2.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.github/workflows/napari-hub-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.372696 vollseg_napari_trackmate-2.5.6/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/ALGORITHM.md
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/MITOSIS.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/RADIAL_ANGLE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.372696 vollseg_napari_trackmate-2.5.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/annotate_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/apply_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/create_oneat_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/train_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/visualize_point_clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.368697 vollseg_napari_trackmate-2.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    93320 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-27 19:41:16.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:24.002816 vollseg_napari_trackmate-2.5.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:23.994816 vollseg_napari_trackmate-2.5.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:23.998816 vollseg_napari_trackmate-2.5.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/.github/workflows/napari-hub-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:23.998816 vollseg_napari_trackmate-2.5.7/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/ALGORITHM.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/MITOSIS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-28 11:03:24.002816 vollseg_napari_trackmate-2.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/RADIAL_ANGLE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:23.998816 vollseg_napari_trackmate-2.5.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/examples/annotate_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-28 11:03:11.000000 vollseg_napari_trackmate-2.5.7/examples/apply_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/examples/create_oneat_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/examples/train_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/examples/visualize_point_clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-28 11:03:24.002816 vollseg_napari_trackmate-2.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:23.994816 vollseg_napari_trackmate-2.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:23.998816 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:24.002816 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72916 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:24.002816 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:03:24.002816 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-28 11:03:23.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-28 11:03:23.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:03:23.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-28 11:03:23.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-28 11:03:23.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-28 11:03:23.000000 vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-28 11:03:12.000000 vollseg_napari_trackmate-2.5.7/update_version.py
```

### Comparing `vollseg_napari_trackmate-2.5.6/.github/workflows/deploy.yml` & `vollseg_napari_trackmate-2.5.7/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/.github/workflows/napari-hub-preview.yml` & `vollseg_napari_trackmate-2.5.7/.github/workflows/napari-hub-preview.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/.github/workflows/test_and_deploy.yml` & `vollseg_napari_trackmate-2.5.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/.gitignore` & `vollseg_napari_trackmate-2.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/.napari-hub/DESCRIPTION.md` & `vollseg_napari_trackmate-2.5.7/.napari-hub/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/.napari-hub/config.yml` & `vollseg_napari_trackmate-2.5.7/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/.pre-commit-config.yaml` & `vollseg_napari_trackmate-2.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/ALGORITHM.md` & `vollseg_napari_trackmate-2.5.7/ALGORITHM.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/LICENSE` & `vollseg_napari_trackmate-2.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/MITOSIS.md` & `vollseg_napari_trackmate-2.5.7/MITOSIS.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/PKG-INFO` & `vollseg_napari_trackmate-2.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.6
+Version: 2.5.7
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg_napari_trackmate-2.5.6/README.md` & `vollseg_napari_trackmate-2.5.7/README.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/_config.yml` & `vollseg_napari_trackmate-2.5.7/_config.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/examples/apply_autoencoder.py` & `vollseg_napari_trackmate-2.5.7/examples/apply_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/examples/create_oneat_patches.py` & `vollseg_napari_trackmate-2.5.7/examples/create_oneat_patches.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/examples/train_oneat.py` & `vollseg_napari_trackmate-2.5.7/examples/train_oneat.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/examples/visualize_point_clouds.py` & `vollseg_napari_trackmate-2.5.7/examples/visualize_point_clouds.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/setup.cfg` & `vollseg_napari_trackmate-2.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_data_model.py` & `vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/napari.yaml` & `vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.6
+Version: 2.5.7
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg_napari_trackmate-2.5.7/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/tox.ini` & `vollseg_napari_trackmate-2.5.7/tox.ini`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.6/update_version.py` & `vollseg_napari_trackmate-2.5.7/update_version.py`

 * *Files identical despite different names*

