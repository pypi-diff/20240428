# Comparing `tmp/vollseg_napari_trackmate-2.5.5.tar.gz` & `tmp/vollseg_napari_trackmate-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vollseg_napari_trackmate-2.5.5.tar", last modified: Sat Apr 27 17:09:23 2024, max compression
+gzip compressed data, was "vollseg_napari_trackmate-2.5.6.tar", last modified: Sat Apr 27 19:41:16 2024, max compression
```

## Comparing `vollseg_napari_trackmate-2.5.5.tar` & `vollseg_napari_trackmate-2.5.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.695421 vollseg_napari_trackmate-2.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.699421 vollseg_napari_trackmate-2.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.github/workflows/napari-hub-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.699421 vollseg_napari_trackmate-2.5.5/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/ALGORITHM.md
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/MITOSIS.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/RADIAL_ANGLE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.699421 vollseg_napari_trackmate-2.5.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/annotate_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/apply_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/create_oneat_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/train_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/visualize_point_clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.695421 vollseg_napari_trackmate-2.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.699421 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    95277 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.368697 vollseg_napari_trackmate-2.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.372696 vollseg_napari_trackmate-2.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.github/workflows/napari-hub-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.372696 vollseg_napari_trackmate-2.5.6/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/ALGORITHM.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/MITOSIS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/RADIAL_ANGLE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.372696 vollseg_napari_trackmate-2.5.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/annotate_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/apply_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/create_oneat_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/train_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-27 19:41:03.000000 vollseg_napari_trackmate-2.5.6/examples/visualize_point_clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.368697 vollseg_napari_trackmate-2.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93320 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:41:16.376697 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-27 19:41:16.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 19:41:15.000000 vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-27 19:41:04.000000 vollseg_napari_trackmate-2.5.6/update_version.py
```

### Comparing `vollseg_napari_trackmate-2.5.5/.github/workflows/deploy.yml` & `vollseg_napari_trackmate-2.5.6/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/.github/workflows/napari-hub-preview.yml` & `vollseg_napari_trackmate-2.5.6/.github/workflows/napari-hub-preview.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/.github/workflows/test_and_deploy.yml` & `vollseg_napari_trackmate-2.5.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/.gitignore` & `vollseg_napari_trackmate-2.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/.napari-hub/DESCRIPTION.md` & `vollseg_napari_trackmate-2.5.6/.napari-hub/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/.napari-hub/config.yml` & `vollseg_napari_trackmate-2.5.6/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/.pre-commit-config.yaml` & `vollseg_napari_trackmate-2.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/ALGORITHM.md` & `vollseg_napari_trackmate-2.5.6/ALGORITHM.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/LICENSE` & `vollseg_napari_trackmate-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/MITOSIS.md` & `vollseg_napari_trackmate-2.5.6/MITOSIS.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/PKG-INFO` & `vollseg_napari_trackmate-2.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.5
+Version: 2.5.6
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg_napari_trackmate-2.5.5/README.md` & `vollseg_napari_trackmate-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/_config.yml` & `vollseg_napari_trackmate-2.5.6/_config.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/examples/apply_autoencoder.py` & `vollseg_napari_trackmate-2.5.6/examples/apply_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/examples/create_oneat_patches.py` & `vollseg_napari_trackmate-2.5.6/examples/create_oneat_patches.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/examples/train_oneat.py` & `vollseg_napari_trackmate-2.5.6/examples/train_oneat.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/examples/visualize_point_clouds.py` & `vollseg_napari_trackmate-2.5.6/examples/visualize_point_clouds.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/setup.cfg` & `vollseg_napari_trackmate-2.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_data_model.py` & `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_widget.py` & `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,18 +696,18 @@
         ),
         edges_csv_path=dict(
             widget_type="FileEdit",
             visible=True,
             label="Edges/Links csv",
             mode="r",
         ),
-        cluster_csv_path=dict(
+        oneat_csv_path=dict(
             widget_type="FileEdit",
             visible=True,
-            label="Cluster Labels csv",
+            label="Oneat Mitosis csv",
             mode="r",
         ),
         axes=dict(
             widget_type="LineEdit",
             label="Image Axes",
             value=DEFAULTS_MODEL["axes"],
         ),
@@ -737,15 +737,15 @@
         channel_seg_image: Union[napari.layers.Labels, None],
         mask_image: Union[napari.layers.Labels, None],
         xml_path,
         master_xml_path,
         track_csv_path,
         spot_csv_path,
         edges_csv_path,
-        cluster_csv_path,
+        oneat_csv_path,
         axes,
         batch_size,
         device_type,
         compute_button,
     ) -> List[napari.types.LayerDataTuple]:
 
         pass
@@ -2239,33 +2239,14 @@
                 ]
             )
             unique_tracklet_ids_list = []
             for unique_track_id in _to_analyze:
                 track_object = _trackmate_objects.unique_tracks[unique_track_id]
                 unique_tracklet_ids_list.append(int(track_object[0, 0]) + 1)
 
-            cluster_class_dataset = _cluster_csv_path_change(
-                plugin_data.cluster_csv_path.value
-            )
-            if not cluster_class_dataset.empty:
-                for layer in list(plugin.viewer.value.layers):
-                    if "Cluster Classes" == layer.name:
-                        plugin.viewer.value.layers.remove(layer)
-                print("refreshing cluster classes")
-                mask = cluster_class_dataset["Track ID"].isin(unique_tracklet_ids_list)
-                chosen_track_data = cluster_class_dataset[mask]
-                chosen_track_data["Cluster"].fillna(-1, inplace=True)
-                if not chosen_track_data.empty:
-                    properties = {"cluster_class": chosen_track_data.values[..., -1]}
-                    plugin.viewer.value.add_tracks(
-                        chosen_track_data.values[..., :-1],
-                        name="Cluster Classes",
-                        properties=properties,
-                    )
-
             pred = unique_tracks, unique_tracks_properties, track_id
 
             _refreshTrackData(pred)
 
     @change_handler(plugin_data.batch_size)
     def _batch_size_change(value: int):
 
@@ -2311,20 +2292,14 @@
             w.hide()
 
         selected.show()
 
         # Trigger model change
         selected.changed(selected.value)
 
-    # widget_for_cluster_modeltype = {
-    # DeepEmbeddedClustering: plugin.cluster_model,
-    # "No(Cluster)": plugin.cluster_model_none,
-    # CUSTOM_MODEL_CLUSTER: plugin.model_folder_cluster,
-    # }
-
     plugin_data.compute_button.native.setStyleSheet("background-color: orange")
 
     @change_handler(plugin_data.compute_button)
     def _compute():
 
         _actual_computer()
 
@@ -2396,20 +2371,23 @@
         if plugin_data.device_type.value == "GPU":
             accelerator = "gpu"
         else:
             accelerator = "cpu"
         spot_csv_path = plugin_data.spot_csv_path.value
         track_csv_path = plugin_data.track_csv_path.value
         edges_csv_path = plugin_data.edges_csv_path.value
+        oneat_csv_path = plugin_data.oneat_csv_path.value
         if os.path.isdir(plugin_data.spot_csv_path.value):
             spot_csv_path = None
         if os.path.isdir(plugin_data.track_csv_path.value):
             track_csv_path = None
         if os.path.isdir(plugin_data.edges_csv_path.value):
             edges_csv_path = None
+        if os.path.isdir(plugin_data.oneat_csv_path.value):
+            oneat_csv_path = None
 
         _trackmate_objects = TrackMate(
             plugin_data.xml_path.value,
             spot_csv_path,
             track_csv_path,
             edges_csv_path,
             AttributeBoxname,
@@ -2426,33 +2404,24 @@
             progress_bar=plugin.progress_bar,
             batch_size=plugin_data.batch_size.value,
             accelerator=accelerator,
             devices=1,
             scale_z=scale_z,
             scale_xy=scale_xy,
             compute_with_autoencoder=False,
+            oneat_csv_file=oneat_csv_path,
+            oneat_threshold_cutoff=0.9999,
         )
         nonlocal track_centroid_tree, track_centroid_list
         track_centroid_list = [
             k for k in _trackmate_objects.unique_track_centroid.keys()
         ]
         track_centroid_tree = spatial.cKDTree(track_centroid_list)
         _refreshStatPlotData()
-        cluster_class_dataset = _cluster_csv_path_change(
-            plugin_data.cluster_csv_path.value
-        )
-        if not cluster_class_dataset.empty:
-            print("adding cluster classes to viewer")
-            cluster_class_dataset["Cluster"].fillna(-1, inplace=True)
-            properties = {"cluster_class": cluster_class_dataset.values[..., -1]}
-            plugin.viewer.value.add_tracks(
-                cluster_class_dataset.values[..., :-1],
-                name="Cluster Classes",
-                properties=properties,
-            )
+
         select_track_nature()
         plugin_data.compute_button.enabled = True
 
     @change_handler(plugin_data.track_csv_path, init=False)
     def _track_csv_path_change(value):
 
         plugin_data.compute_button.enabled = True
@@ -2463,28 +2432,17 @@
         plugin_data.compute_button.enabled = True
 
     @change_handler(plugin_data.edges_csv_path, init=False)
     def _edges_csv_path_change(value):
 
         plugin_data.compute_button.enabled = True
 
-    @change_handler(plugin_data.cluster_csv_path, init=False)
-    def _cluster_csv_path_change(value):
-        if plugin_data.cluster_csv_path.value.is_file():
-            cluster_class_dataset = pd.read_csv(
-                plugin_data.cluster_csv_path.value,
-                delimiter=",",
-                encoding="unicode_escape",
-                low_memory=False,
-            )
-            plugin_data.compute_button.enabled = True
-            return cluster_class_dataset
-        else:
-            plugin_data.compute_button.enabled = True
-            return pd.DataFrame()
+    @change_handler(plugin_data.oneat_csv_path, init=False)
+    def _oneat_csv_path_change(value):
+        plugin_data.compute_button.enabled = True
 
     @change_handler(plugin_data.master_xml_path, init=False)
     def _master_xml_path_change(value):
 
         plugin_data.compute_button.enabled = True
 
     @change_handler(plugin_data.xml_path, init=False)
```

### Comparing `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/napari.yaml` & `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.5
+Version: 2.5.6
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg_napari_trackmate-2.5.6/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/tox.ini` & `vollseg_napari_trackmate-2.5.6/tox.ini`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.5/update_version.py` & `vollseg_napari_trackmate-2.5.6/update_version.py`

 * *Files identical despite different names*

