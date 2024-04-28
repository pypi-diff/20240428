# Comparing `tmp/txm_sandbox-0.3.0.post4.tar.gz` & `tmp/txm_sandbox-0.3.0.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.0.post4.tar", last modified: Fri Apr 19 10:58:15 2024, max compression
+gzip compressed data, was "txm_sandbox-0.3.0.post5.tar", last modified: Sun Apr 28 16:59:24 2024, max compression
```

## Comparing `txm_sandbox-0.3.0.post4.tar` & `txm_sandbox-0.3.0.post5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.358183 txm_sandbox-0.3.0.post4/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1070 2024-04-18 03:35:27.000000 txm_sandbox-0.3.0.post4/LICENSE
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      147 2024-04-18 03:34:56.000000 txm_sandbox-0.3.0.post4/MANIFEST.in
--rw-r--r--   0 xiao      (1000) xiao      (1000)      712 2024-04-19 10:58:15.358183 txm_sandbox-0.3.0.post4/PKG-INFO
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1639 2024-04-18 03:35:09.000000 txm_sandbox-0.3.0.post4/README.md
--rwxrwxr-x   0 xiao      (1000) xiao      (1000)     2565 2024-04-18 11:27:34.000000 txm_sandbox-0.3.0.post4/TXM_GUI2.ipynb
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       38 2024-04-19 10:58:15.358183 txm_sandbox-0.3.0.post4/setup.cfg
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1130 2024-04-19 10:56:06.000000 txm_sandbox-0.3.0.post4/setup.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.322183 txm_sandbox-0.3.0.post4/txm_sandbox/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.326182 txm_sandbox-0.3.0.post4/txm_sandbox/config/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     5092 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/config/XANES2D_GUI_config.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/config/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       45 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/config/analysis_tool_gui_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      497 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/config/io_tomo_h5_data_structure.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      500 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/config/io_xanes2D_h5_data_structure.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      616 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/config/io_xanes3D_h5_data_structure.json
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.330182 txm_sandbox-0.3.0.post4/txm_sandbox/dicts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/dicts/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3848 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/dicts/config_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    61110 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      755 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      583 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/dicts/xanes_analysis_dict.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.330182 txm_sandbox-0.3.0.post4/txm_sandbox/external/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/external/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      253 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/external/user_io.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.338183 txm_sandbox-0.3.0.post4/txm_sandbox/gui/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    32500 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    74137 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    79463 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/gui_components.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    36752 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15709 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/main_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      795 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/misc_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   169879 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   204783 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   202060 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    91679 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   203257 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/gui/xanes_fitting_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.338183 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.342182 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      879 2024-04-19 10:38:38.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      957 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      899 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2389 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1362 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.342182 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/dicts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/dicts/__init__.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     5528 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/dicts/data_struct_dict.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.346183 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      106 2024-04-18 19:44:50.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15328 2024-04-19 02:30:59.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/appl_mask_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     9587 2024-04-18 19:52:32.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/convert_data_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    25806 2024-04-18 19:53:16.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/tomo_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    23088 2024-04-19 10:54:30.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    48430 2024-04-18 19:54:08.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15803 2024-04-18 19:54:19.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.346183 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      605 2024-04-18 20:05:13.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      599 2024-04-18 20:05:03.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15251 2024-04-18 19:59:48.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2428 2024-04-18 20:01:32.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    16707 2024-04-18 20:01:56.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1197 2024-04-18 20:04:22.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2029 2024-04-18 20:04:35.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     1533 2024-04-18 20:23:11.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/txm_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.350183 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/utils/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/utils/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1264 2024-04-18 20:05:59.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/utils/io.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    10590 2024-04-18 20:06:46.000000 txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/utils/misc.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.350183 txm_sandbox-0.3.0.post4/txm_sandbox/tmp/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/tmp/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       69 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/tmp/readme.txt
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.354183 txm_sandbox-0.3.0.post4/txm_sandbox/utils/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    16672 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/io.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    14410 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xiao      (1000) xiao      (1000)     4246 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/misc.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1439 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/plotlib.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    61837 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/reg_algs.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    70498 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    36738 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2342 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    23436 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_math.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     6083 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    84774 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3266 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_spectra_filters.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-19 10:58:15.354183 txm_sandbox-0.3.0.post4/txm_sandbox.egg-info/
--rw-r--r--   0 xiao      (1000) xiao      (1000)      712 2024-04-19 10:58:15.000000 txm_sandbox-0.3.0.post4/txm_sandbox.egg-info/PKG-INFO
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3045 2024-04-19 10:58:15.000000 txm_sandbox-0.3.0.post4/txm_sandbox.egg-info/SOURCES.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-19 10:58:15.000000 txm_sandbox-0.3.0.post4/txm_sandbox.egg-info/dependency_links.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-19 10:58:15.000000 txm_sandbox-0.3.0.post4/txm_sandbox.egg-info/not-zip-safe
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      170 2024-04-19 10:58:15.000000 txm_sandbox-0.3.0.post4/txm_sandbox.egg-info/requires.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       12 2024-04-19 10:58:15.000000 txm_sandbox-0.3.0.post4/txm_sandbox.egg-info/top_level.txt
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.920873 txm_sandbox-0.3.0.post5/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post5/LICENSE
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      147 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post5/MANIFEST.in
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      257 2024-04-28 16:59:24.920873 txm_sandbox-0.3.0.post5/PKG-INFO
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1639 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post5/README.md
+-rwxrwxr-x   0 xiao      (1000) xiao      (1000)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post5/TXM_GUI2.ipynb
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       38 2024-04-28 16:59:24.920873 txm_sandbox-0.3.0.post5/setup.cfg
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1130 2024-04-28 16:58:54.000000 txm_sandbox-0.3.0.post5/setup.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.892873 txm_sandbox-0.3.0.post5/txm_sandbox/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.896873 txm_sandbox-0.3.0.post5/txm_sandbox/config/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/XANES2D_GUI_config.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/analysis_tool_gui_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/io_tomo_h5_data_structure.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/io_xanes2D_h5_data_structure.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/io_xanes3D_h5_data_structure.json
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.896873 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/xanes_analysis_dict.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.896873 txm_sandbox-0.3.0.post5/txm_sandbox/external/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/external/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/external/user_io.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.904873 txm_sandbox-0.3.0.post5/txm_sandbox/gui/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    79463 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/gui_components.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/main_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   203257 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes_fitting_gui.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.904873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.908873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      786 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      957 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      899 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2389 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1362 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.908873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/dicts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/dicts/__init__.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)     5528 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/dicts/data_struct_dict.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.908873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      106 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15328 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/appl_mask_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     9587 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/convert_data_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    25747 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/tomo_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    23715 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    49041 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15803 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.912873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      605 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      599 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15251 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2428 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    16610 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1197 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2029 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)     1533 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/txm_gui.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.912873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1264 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/io.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    10590 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/misc.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.912873 txm_sandbox-0.3.0.post5/txm_sandbox/tmp/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/tmp/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/tmp/readme.txt
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.916873 txm_sandbox-0.3.0.post5/txm_sandbox/utils/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/io.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xiao      (1000) xiao      (1000)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/misc.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/plotlib.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    41021 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    23436 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    84774 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_spectra_filters.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.892873 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      257 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/PKG-INFO
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     3045 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/not-zip-safe
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      170 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/requires.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       12 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/top_level.txt
```

### Comparing `txm_sandbox-0.3.0.post4/LICENSE` & `txm_sandbox-0.3.0.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/README.md` & `txm_sandbox-0.3.0.post5/README.md`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/TXM_GUI2.ipynb` & `txm_sandbox-0.3.0.post5/TXM_GUI2.ipynb`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/setup.py` & `txm_sandbox-0.3.0.post5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: xiao
 """
 
 from setuptools import setup, find_packages
 
 setup(name='txm_sandbox',
-      version='0.3.0.post4',
+      version='0.3.0.post5',
       description='Integrated Spectro-Imaging Analysis Toolbox',
       url='https://github.com/xianghuix/TXM_Sandbox',
       author='Xianghui Xiao',
       author_email='xianghuix@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
```

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/config/XANES2D_GUI_config.json` & `txm_sandbox-0.3.0.post5/txm_sandbox/config/XANES2D_GUI_config.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/config/io_xanes3D_h5_data_structure.json` & `txm_sandbox-0.3.0.post5/txm_sandbox/config/io_xanes3D_h5_data_structure.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/dicts/config_dict.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/dicts/customized_struct_dict.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/dicts/sklearn_opt_dict.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/dicts/xanes_analysis_dict.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/conv_data_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/gen_algn_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/gui_components.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/gui_components.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/io_config_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/io_config_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/main_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/misc_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/tomo_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/xanes2D_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/xanes3D_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/xanes_analysis_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/gui/xanes_fitting_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/dicts/data_struct_dict.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/dicts/data_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/appl_mask_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/appl_mask_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/convert_data_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/convert_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/tomo_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/tomo_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,21 +242,21 @@
                 self.pick_cen.enabled = True
             else:
                 self.pick_cen.enabled = False
             if self._cen is None:
                 self.vol_rec.enabled = False
             else:
                 self.vol_rec.enabled = True
+            self.trial_cen_done.enabled = False
         self.close_file.enabled = True
 
     def __preset_dflt(self):
         self._data_dim = info_reader(self.scn_fn, dtype="data", cfg=self._tomo_cfg)
         if (self._data_dim[2] / 2 - self.cen_sch_s.value) > (self._data_dim[2] / 6):
             self.cen_sch_s.value = int(self._data_dim[2] / 2 - 40)
-        # if self._data_dim[1] < self.cen_sch_s.value:
         self.ref_sli.value = int(self._data_dim[1] / 2)
 
     def _sel_file_type(self):
         self._cen = None
         self._trial_cen_rec_done = False
         if self.file_type.value == "tomo_zfly":
             self._tomo_cfg = ZFLY_CFG["io_data_structure_tomo"]
@@ -284,45 +284,43 @@
                 tem = json.load(f)
                 tem["tomo_batch_recon"]["cfg_file"] = str(
                     self.top_dir.value
                     / f"tomo_batch_trial_cen_cfg_{datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S')}.json"
                 )
             with open(cfg_fn, "w") as f:
                 json.dump(tem, f, indent=4, separators=(",", ": "))
+        else:
+            self._trial_cen_rec_done = False
+            self.pick_cen.enabled = False
+            self.vol_rec.enabled = False
+            self.trial_cen_done.value = "No"
 
     def _sel_scn_id(self):
         self._cen = None
         self._trial_cen_rec_done = False
         self.proj_prev.value = False
         self.__comp_scn_fn()
-        # self.__set_trial_cen_rec_widgets()
         self.__set_vol_rec_widgets()
 
     @disp_progress_info("data file read")
     def _proj_prev(self):
         rm_gui_viewers(self.viewer, ["proj_prev"])
         if self.proj_prev.value:
             if self.file_type.value == "tomo_zfly":
-                # self.viewer.add_image(
-                #     h5py.File(self.scn_fn, "r")["/Exchange/data"], name="proj_prev"
-                # )
                 update_layer_in_viewer(
                     self.viewer,
                     h5py.File(self.scn_fn, "r")[
                         ZFLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
                             "io_data_structure"
                         ]["data_path"]
                     ],
                     "proj_prev",
                 )
                 show_layers_in_viewer(self.viewer, ["proj_prev"])
             else:
-                # self.viewer.add_image(
-                #     h5py.File(self.scn_fn, "r")["/img_tomo"], name="proj_prev"
-                # )
                 update_layer_in_viewer(
                     self.viewer,
                     h5py.File(self.scn_fn, "r")[
                         FLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
                             "io_data_structure"
                         ]["data_path"]
                     ],
@@ -584,25 +582,27 @@
                 tem = json.load(ft)
             with open(batch_tplt_fn, "w") as ft:
                 tem[str(self.scan_id.value)]["data_params"]["rot_cen"] = self._cen
                 tem[str(self.scan_id.value)]["data_params"]["sli_s"] = 0
                 tem[str(self.scan_id.value)]["data_params"]["sli_e"] = self._data_dim[1]
                 tem[str(self.scan_id.value)]["recon_config"]["recon_type"] = "Vol Recon"
                 json.dump(tem, ft, indent=4, separators=(",", ": "))
+            self.trial_cen_done.enabled = True
         else:
             with open(cfg_fn, "r") as f:
                 tomo_tplt_fn = json.load(f)["tomo_recon"]["cfg_file"]
             with open(tomo_tplt_fn, "r") as ft:
                 tem = json.load(ft)
             tem[list(tem.keys())[0]]["data_params"]["rot_cen"] = self._cen
             tem[list(tem.keys())[0]]["data_params"]["sli_s"] = 0
             tem[list(tem.keys())[0]]["data_params"]["sli_e"] = self._data_dim[1]
             tem[list(tem.keys())[0]]["recon_config"]["recon_type"] = "Vol Recon"
             with open(tomo_tplt_fn, "w") as ft:
                 json.dump(tem, ft, indent=4, separators=(",", ": "))
+            self.trial_cen_done.enabled = False
 
         self.__set_vol_rec_widgets()
 
     def _trial_cen_done(self):
         if self.trial_cen_done.value == "Yes":
             self._multi_trial_cen_rec_done = True
         else:
```

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/xanes_fit_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_fit_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,27 +123,27 @@
         self.analysis_type.changed.connect(self._xanes_fit_type_chgd)
         self.fit.changed.connect(self._xanes_fit)
         self.close_file.changed.connect(self._close_file)
 
         self.gui_layout = widgets.VBox(
             widgets=[
                 self.label0,
-                # self.label1,
+                self.label1,
                 self.data_type,
-                # self.label2,
+                self.label2,
                 self.xanes_file,
                 self.reload,
                 self.eng_eV,
                 self.sli,
                 self.E,
                 self.spec_in_roi,
                 self.roi_cen_x,
                 self.roi_cen_y,
                 self.def_fit_range,
-                # self.label3,
+                self.label3,
                 self.element,
                 self.analysis_type,
                 self.edge_eng,
                 self.wl_s,
                 self.wl_e,
                 self.edge_s,
                 self.edge_e,
@@ -548,14 +548,26 @@
                 f[
                     "/processed_XANES/proc_parameters/wl_fit method/params"
                 ].create_dataset(
                     "eng_offset",
                     data=(float(self.wl_s.value) + float(self.wl_e.value)) / 2.0,
                 )
             else:
+                del f["/processed_XANES/proc_parameters/edge_eng"]
+                f["/processed_XANES/proc_parameters"].create_dataset(
+                    "edge_eng", data=float(self.edge_eng.value)
+                )
+                del f["/processed_XANES/proc_parameters/edge50_fit_s"]
+                f["/processed_XANES/proc_parameters"].create_dataset(
+                    "edge50_fit_s", data="None"
+                )
+                del f["/processed_XANES/proc_parameters/edge50_fit_e"]
+                f["/processed_XANES/proc_parameters"].create_dataset(
+                    "edge50_fit_e", data="None"
+                )
                 del f["/processed_XANES/proc_parameters/wl_fit method/params/spec"]
                 f[
                     "/processed_XANES/proc_parameters/wl_fit method/params"
                 ].create_dataset("spec", data="raw")
                 del f[
                     "/processed_XANES/proc_parameters/wl_fit method/params/eng_offset"
                 ]
```

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/xanes_reg_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_reg_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,15 @@
                 )
             except Exception as e:
                 self.op_status.value = (
                     "Something is wrong. Please check terminal for more information."
                 )
                 print(f"{str(e)=}")
         elif mode == "recon_roi":
+            print("signature")
             if self._3dxanes_rec_roiz_old_val[0] != self.rec_roiz.value[0]:
                 try:
                     update_layer_in_viewer(
                         self.viewer,
                         tifffile.imread(
                             str(self.rec_fntpl).format(
                                 self.ref_scan_id.value,
@@ -1030,14 +1031,28 @@
         overlap_roi(self.viewer, self, mode="recon_roi")
         show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
         if self.data_type.value == "2D XANES":
             self.confirm_test_run.value = "No"
 
     def _xanes_tomo_rec_roiz(self):
         if self.data_type.value == "3D XANES":
+            if self.rec_roiz.value[0] > (
+                self.ref_sli.value - self.sli_srch_range.value
+            ):
+                self.rec_roiz.value = [
+                    self.ref_sli.value - self.sli_srch_range.value,
+                    self.rec_roiz.value[1],
+                ]
+            if self.rec_roiz.value[1] < (
+                self.ref_sli.value + self.sli_srch_range.value
+            ):
+                self.rec_roiz.value = [
+                    self.rec_roiz.value[0],
+                    self.ref_sli.value + self.sli_srch_range.value,
+                ]
             self.__3dxanes_tomo_show_sli(mode="recon_roi")
         else:
             self.__2dxanes_show_sli(mode="auto_algn")
             self.confirm_test_run.value = "No"
         overlap_roi(self.viewer, self, mode="recon_roi")
         show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
```

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/guis/xanes_vis_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_vis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,14 @@
     return output
 
 
 with open(cfg_fn, "r") as f:
     xanes3d_data_fn = json.load(f)["xanes3d_fit"]["cfg_file"]
 
 with h5py.File(xanes3d_data_fn, "a") as f:
-    # if "/processed_XANES3D" in f:
-    #     proc_xanes_path = "/processed_XANES3D"
-    # else:
     proc_xanes_path = "/processed_XANES"
     bin_fact = f[f"/{proc_xanes_path}/proc_parameters/bin_fact"][()]
     if bin_fact == 1:
         imgs = f["/registration_results/reg_results/registered_xanes3D"][:, 0, :, :]
     else:
         imgs = zoom(
             f["/registration_results/reg_results/registered_xanes3D"][
```

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/txm_gui.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/txm_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/utils/io.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/napari_gui/utils/misc.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/io.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/lineshapes.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/misc.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/plotlib.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/reg_algs.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/tomo_recon_tools.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/tomo_recon_tools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_analysis.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from copy import deepcopy
 import multiprocess as mp
 from tomopy.util.mproc import distribute_jobs
 
 from .misc import msgit
 from . import xanes_math as xm
 
-N_CPU = os.cpu_count()-1 if os.cpu_count()>1 else os.cpu_count()
+N_CPU = os.cpu_count() - 1 if os.cpu_count() > 1 else os.cpu_count()
 """
     This class include xanes spectrum analyses. These analyses are based on
     filtered xanes spectra. The basic functions include:
         1. curve fitting
         2. peak fitting
     The analyses in this package include:
 
@@ -34,30 +34,41 @@
         5. Calculating pre_edge and post_edge statistics
         6. Finding peak (whiteline)
         7, PCA analysis
         8. Linear Combinatiotn analysis
 """
 
 
-class xanes_analysis():
-    def __init__(self, spectrum, eng, preset_edge_eng,
-                 pre_es=None, pre_ee=-50,
-                 post_es=100, post_ee=None,
-                 edge_jump_threshold=5,
-                 pre_edge_threshold=1):
+class xanes_analysis:
+    def __init__(
+        self,
+        spectrum,
+        eng,
+        preset_edge_eng,
+        pre_es=None,
+        pre_ee=-50,
+        post_es=100,
+        post_ee=None,
+        edge_jump_threshold=5,
+        pre_edge_threshold=1,
+    ):
         self.spec = spectrum
         self.eng = eng
         self.preset_edge_eng = preset_edge_eng
-        self.model = {'edge': {}, 'wl': {}}
+        self.model = {"edge": {}, "wl": {}}
         self.lcf_use = False
         self.lcf_constr_use = True
         self.lcf_ref_spec = None
         self.lcf_ref = None
         self.lcf_fit = None
-        self.lcf_model = {'constr': self.lcf_constr_use, 'ref': self.lcf_ref, 'rlt': None}
+        self.lcf_model = {
+            "constr": self.lcf_constr_use,
+            "ref": self.lcf_ref,
+            "rlt": None,
+        }
 
         if pre_es is None:
             pre_es = eng[0] - preset_edge_eng
         self.pre_es = preset_edge_eng + pre_es
         self.pre_ee = preset_edge_eng + pre_ee
         self.pre_es_idx = xm.index_of(self.eng, self.pre_es)
         self.pre_ee_idx = xm.index_of(self.eng, self.pre_ee)
@@ -123,36 +134,41 @@
         """
         return self.spec * self.fitted_edge_mask
 
     def cal_pre_edge_sd(self):
         """
         return: ndarray, pre_edge_sd has dimension of spectrum.shape[1:]
         """
-        self.pre_edge_sd_map = self.spec[self.pre_es_idx:self.pre_ee_idx,
-                               :].std(axis=0)
+        self.pre_edge_sd_map = self.spec[self.pre_es_idx : self.pre_ee_idx, :].std(
+            axis=0
+        )
 
     def cal_post_edge_sd(self):
         """
         return: ndarray, post_edge_sd has dimension of spectrum.shape[1:]
         """
-        self.post_edge_sd_map = self.spec[self.post_es_idx:self.post_ee_idx,
-                                :].std(axis=0)
+        self.post_edge_sd_map = self.spec[self.post_es_idx : self.post_ee_idx, :].std(
+            axis=0
+        )
 
     def cal_pre_edge_mean(self):
         """
         return: ndarray, pre_edge_sd has dimension of spectrum.shape[1:]
         """
-        self.pre_edge_mean_map = self.spec[self.pre_es_idx:self.pre_ee_idx, :].mean(axis=0)
+        self.pre_edge_mean_map = self.spec[self.pre_es_idx : self.pre_ee_idx, :].mean(
+            axis=0
+        )
 
     def cal_post_edge_mean(self):
         """
         return: ndarray, post_edge_sd has dimension of spectrum.shape[1:]
         """
-        self.post_edge_mean_map = self.spec[self.post_es_idx:self.post_ee_idx,
-                                  :].mean(axis=0)
+        self.post_edge_mean_map = self.spec[
+            self.post_es_idx : self.post_ee_idx, :
+        ].mean(axis=0)
 
     def cal_fit(self, fit_coef, eng=None, reshape=True):
         if eng is None:
             eng = self.eng
         if not isinstance(eng, np.ndarray):
             eng = np.array(eng)
         fit = xm.eval_polynd(fit_coef, eng)
@@ -160,214 +176,288 @@
             if eng.shape:
                 return fit.reshape([eng.shape[0], *self.spec.shape[1:]])
             else:
                 return fit.reshape([*self.spec.shape[1:]])
         else:
             return fit
 
-    @msgit(wd=100, fill='+')
+    @msgit(wd=100, fill="+")
     def cal_pre_edge_fit(self, eng=None, reshape=True):
         """
         inputs:
             eng: 1D array-like; full energy list of the spectrum
             pre_edge_fit_coef: array-like; pixel-wise pre_edge fit coef
         ouputs:
             pre_edge_fit: array-like; pixel-wise line profile over eng
         """
         self.fit_pre_edge()
         return self.cal_fit(self.pre_edge_fit_rlt[0], eng=eng, reshape=reshape)
 
-    @msgit(wd=100, fill='+')
+    @msgit(wd=100, fill="+")
     def cal_post_edge_fit(self, eng=None, reshape=True):
         """
         inputs:
             eng: 1D array-like; full energy list of the spectrum
             post_edge_fit_coef: array-like; pixel-wise post_edge fit coef
         ouputs:
             post_edge_fit: array-like; pixel-wise line profile over eng
         """
         self.fit_post_edge()
         return self.cal_fit(self.post_edge_fit_rlt[0], eng=eng, reshape=reshape)
 
-    @msgit(wd=100, fill='+')
+    @msgit(wd=100, fill="+")
     def cal_edge_jump_map(self):
         """
         return: ndarray, edge_jump_map has dimension of spectrum.shape[1:]
         """
-        self.edge_jump_map = (self.cal_post_edge_fit(np.array([self.preset_edge_eng])) -
-                              self.cal_pre_edge_fit(np.array([self.preset_edge_eng])))
+        self.edge_jump_map = self.cal_post_edge_fit(
+            np.array([self.preset_edge_eng])
+        ) - self.cal_pre_edge_fit(np.array([self.preset_edge_eng]))
 
     def cal_drt_wl_peak_hgt(self, peak_es, peak_ee):
         self.wl_es_idx = xm.index_of(self.eng, peak_es)
         self.wl_ee_idx = xm.index_of(self.eng, peak_ee)
 
-        eng = self.eng[self.wl_es_idx:self.wl_ee_idx]
+        eng = self.eng[self.wl_es_idx : self.wl_ee_idx]
         for ii in range(1, len(self.spec.shape)):
             eng = eng[:, np.newaxis]
-        self.wl_ph_dir = np.squeeze(np.max(self.spec[self.wl_es_idx:self.wl_ee_idx, :], axis=0))
+        self.wl_ph_dir = np.squeeze(
+            np.max(self.spec[self.wl_es_idx : self.wl_ee_idx, :], axis=0)
+        )
 
     def cal_wgt_eng(self, eng_s, eng_e=None):
+        print(f"{self.eng=}\n{eng_s=}\n{eng_e=}\n{self.spec.shape=}")
         if (not self.wl_ph_dir.shape) and (not self.wl_ph_fit.shape):
-            print('Please calculate the whiteline peak height first. Quit!')
+            print("Please calculate the whiteline peak height first. Quit!")
             self.centroid_of_eng = np.empty([0])
             self.centroid_of_eng_rel_wl = np.empty([0])
             self.weighted_atten = np.empty([0])
             self.weighted_eng = np.empty([0])
             return
         if (not self.wl_pos_dir.shape) and (not self.wl_pos_fit.shape):
-            print('Please calculate the whiteline energy first. Quit!')
+            print("Please calculate the whiteline energy first. Quit!")
             self.centroid_of_eng = np.empty([0])
             self.centroid_of_eng_rel_wl = np.empty([0])
             self.weighted_atten = np.empty([0])
             self.weighted_eng = np.empty([0])
             return
         if eng_e is None:
             if self.wl_pos_fit.shape:
                 eng_e = self.wl_pos_fit
             else:
                 eng_e = self.wl_pos_dir
         eng = np.squeeze(deepcopy(self.eng))
-        for ii in range(0, len(self.spec.shape)-1):
+        for ii in range(0, len(self.spec.shape) - 1):
             eng = eng[:, np.newaxis]
-        
+
         if self.wl_ph_fit.shape:
             wl_ph = self.wl_ph_fit
         else:
             wl_ph = self.wl_ph_dir
 
-        a = (eng >= eng_s) & (eng <= eng_e + 0.0002)
-        b = (np.where(a, self.spec, 0) * eng * (np.roll(eng, -1, axis=0) - eng)).sum(axis=0)
-        c = (np.where(a, self.spec, 0) * (np.roll(eng, -1, axis=0) - eng)).sum(axis=0)
-        d = np.where(a, eng * (np.roll(eng, -1, axis=0) - eng), 0).sum(axis=0)
-        e = (np.where(a, self.spec, 0) * np.abs(eng - eng_e) * (np.roll(eng, -1, axis=0) - eng)).sum(axis=0)
+        a = (eng >= eng_s - 0.0002) & (eng <= eng_e + 0.0002)
+        b = (
+            np.where(a, self.spec, 0) * eng * np.abs(np.roll(eng, -1, axis=0) - eng)
+        ).sum(axis=0)
+        c = (np.where(a, self.spec, 0) * np.abs(np.roll(eng, -1, axis=0) - eng)).sum(
+            axis=0
+        )
+        d = np.where(a, eng * np.abs(np.roll(eng, -1, axis=0) - eng), 0).sum(axis=0)
+        e = (
+            np.where(a, self.spec, 0)
+            * np.abs(eng - eng_e)
+            * np.abs(np.roll(eng, -1, axis=0) - eng)
+        ).sum(axis=0)
 
         self.centroid_of_eng = b / c
         self.centroid_of_eng_rel_wl = e / c
         self.weighted_atten = b / d
         self.weighted_eng = b / wl_ph
 
-    @msgit(wd=100, fill='+')
+    @msgit(wd=100, fill="+")
     def create_edge_jump_filter(self, eng0=None):
         """
         return: ndarray, same dimension as spectrum.shape
         """
         if eng0 is None:
             eng0 = self.edge_eng
-        self.edge_jump_mask = ((self.cal_post_edge_fit(eng0) -
-                                self.cal_pre_edge_fit(eng0))
-                               > self.edge_jump_thres * self.pre_edge_sd_map).astype(np.int8)
+        self.edge_jump_mask = (
+            (self.cal_post_edge_fit(eng0) - self.cal_pre_edge_fit(eng0))
+            > self.edge_jump_thres * self.pre_edge_sd_map
+        ).astype(np.int8)
 
-    @msgit(wd=100, fill='+')
+    @msgit(wd=100, fill="+")
     def create_fitted_edge_filter(self):
         """
         return: ndarray, same dimension as spectrum.shape
         """
-        self.fitted_edge_mask = np.any((self.cal_post_edge_fit(self.eng) -
-                                        self.cal_pre_edge_fit(self.eng))
-                                       > self.fitted_edge_thres * self.pre_edge_sd_map, axis=0).astype(np.int8)
+        self.fitted_edge_mask = np.any(
+            (self.cal_post_edge_fit(self.eng) - self.cal_pre_edge_fit(self.eng))
+            > self.fitted_edge_thres * self.pre_edge_sd_map,
+            axis=0,
+        ).astype(np.int8)
 
-    @msgit(wd=100, fill='$')
-    def find_edge_0p5(self, es, ee, optimizer='model', ufac=20):
+    @msgit(wd=100, fill="$")
+    def find_edge_0p5(self, es, ee, optimizer="model", ufac=20):
         idx_s = xm.index_of(self.eng, es)
         idx_e = xm.index_of(self.eng, ee)
-        us_eng = np.linspace(self.eng[idx_s], self.eng[idx_e],
-                             num=(idx_e - idx_s + 1) * ufac) - self.model['edge']['eoff']
-        if optimizer == 'model':
-            self.edge0p5_pos_fit = xm.find_fit_val(self.model['edge']['model'],
-                                                   np.array(self.model['edge']['fit_rlt'][0]),
-                                                   us_eng, v=0.5).reshape(self.spec.shape[1:]) + \
-                                   self.model['edge']['eoff']
-        elif optimizer == 'direct':
-            self.edge0p5_pos_dir = xm.lookup(self.eng[idx_s:idx_e],
-                                             self.norm_spec[idx_s:idx_e].reshape(idx_e - idx_s, -1), 0.5). \
-                reshape(self.spec.shape[1:])
+        us_eng = (
+            np.linspace(
+                self.eng[idx_s], self.eng[idx_e], num=(idx_e - idx_s + 1) * ufac
+            )
+            - self.model["edge"]["eoff"]
+        )
+        if optimizer == "model":
+            self.edge0p5_pos_fit = (
+                xm.find_fit_val(
+                    self.model["edge"]["model"],
+                    np.array(self.model["edge"]["fit_rlt"][0]),
+                    us_eng,
+                    v=0.5,
+                ).reshape(self.spec.shape[1:])
+                + self.model["edge"]["eoff"]
+            )
+        elif optimizer == "direct":
+            self.edge0p5_pos_dir = xm.lookup(
+                self.eng[idx_s:idx_e],
+                self.norm_spec[idx_s:idx_e].reshape(idx_e - idx_s, -1),
+                0.5,
+            ).reshape(self.spec.shape[1:])
 
-    @msgit(wd=100, fill='$')
-    def find_edge_50(self, ees, eee, pes, pee, optimizer='model', ufac=20):
+    @msgit(wd=100, fill="$")
+    def find_edge_50(self, ees, eee, pes, pee, optimizer="model", ufac=20):
         idx_es = xm.index_of(self.eng, ees)
         idx_ee = xm.index_of(self.eng, eee)
         idx_ps = xm.index_of(self.eng, pes)
         idx_pe = xm.index_of(self.eng, pee)
-        us_e_eng = np.linspace(self.eng[idx_es], self.eng[idx_ee], num=(idx_ee - idx_es) * ufac + 1)
-        us_p_eng = np.linspace(self.eng[idx_ps], self.eng[idx_pe], num=(idx_pe - idx_ps) * ufac + 1)
-        if optimizer == 'both':
-            print('both')
-            self.edge50_pos_fit = xm.find_50_peak(self.model['edge']['model'], us_e_eng-self.model['edge']['eoff'],
-                                                  np.array(self.model['edge']['fit_rlt'][0]),
-                                                  self.model['wl']['model'], us_p_eng-self.model['wl']['eoff'],
-                                                  np.array(self.model['wl']['fit_rlt'][0]), ftype=optimizer). \
-                    reshape(self.spec.shape[1:]) + self.model['edge']['eoff']
-        elif optimizer == 'wl':
-            print('wl')
-            self.edge50_pos_fit = xm.find_50_peak(us_e_eng, self.eng[idx_es:idx_ee+1],
-                                                  self.norm_spec[idx_es:idx_ee+1].reshape([idx_ee-idx_es+1, -1]),
-                                                  self.model['wl']['model'], us_p_eng-self.model['wl']['eoff'],
-                                                  np.array(self.model['wl']['fit_rlt'][0]), ftype=optimizer). \
-                    reshape(self.spec.shape[1:])
-        elif optimizer == 'edge':
-            print('edge')
-            self.edge50_pos_fit = xm.find_50_peak(self.model['edge']['model'], us_e_eng-self.model['edge']['eoff'],
-                                                  np.array(self.model['edge']['fit_rlt'][0]),
-                                                  us_p_eng, self.eng[idx_ps:idx_pe+1],
-                                                  self.norm_spec[idx_ps:idx_pe+1].reshape([idx_pe-idx_ps+1, -1]),
-                                                  ftype=optimizer). \
-                    reshape(self.spec.shape[1:]) + self.model['edge']['eoff']
-        elif optimizer == 'none':
-            print('none')
-            self.edge50_pos_fit_none = xm.find_50_peak(us_e_eng, self.eng[idx_es:idx_ee+1],
-                                                  self.norm_spec[idx_es:idx_ee+1].reshape([idx_ee-idx_es+1, -1]),
-                                                  us_p_eng, self.eng[idx_ps:idx_pe + 1],
-                                                  self.norm_spec[idx_ps:idx_pe+1].reshape([idx_pe-idx_ps+1, -1]),
-                                                  ftype=optimizer). \
-                    reshape(self.spec.shape[1:])
-        elif optimizer == 'direct':
-            print('dir')
-            self.edge50_pos_dir = xm.lookup(self.eng[idx_es:idx_ee],
-                                            self.norm_spec[idx_es:idx_ee].reshape([idx_ee-idx_es, -1]),
-                                            0.5*self.norm_spec[idx_ps:idx_pe].reshape([idx_pe-idx_ps, -1]).max(axis=0)). \
-                    reshape(self.spec.shape[1:])
+        us_e_eng = np.linspace(
+            self.eng[idx_es], self.eng[idx_ee], num=(idx_ee - idx_es) * ufac + 1
+        )
+        us_p_eng = np.linspace(
+            self.eng[idx_ps], self.eng[idx_pe], num=(idx_pe - idx_ps) * ufac + 1
+        )
+        if optimizer == "both":
+            print("both")
+            self.edge50_pos_fit = (
+                xm.find_50_peak(
+                    self.model["edge"]["model"],
+                    us_e_eng - self.model["edge"]["eoff"],
+                    np.array(self.model["edge"]["fit_rlt"][0]),
+                    self.model["wl"]["model"],
+                    us_p_eng - self.model["wl"]["eoff"],
+                    np.array(self.model["wl"]["fit_rlt"][0]),
+                    ftype=optimizer,
+                ).reshape(self.spec.shape[1:])
+                + self.model["edge"]["eoff"]
+            )
+        elif optimizer == "wl":
+            print("wl")
+            self.edge50_pos_fit = xm.find_50_peak(
+                us_e_eng,
+                self.eng[idx_es : idx_ee + 1],
+                self.norm_spec[idx_es : idx_ee + 1].reshape([idx_ee - idx_es + 1, -1]),
+                self.model["wl"]["model"],
+                us_p_eng - self.model["wl"]["eoff"],
+                np.array(self.model["wl"]["fit_rlt"][0]),
+                ftype=optimizer,
+            ).reshape(self.spec.shape[1:])
+        elif optimizer == "edge":
+            print("edge")
+            self.edge50_pos_fit = (
+                xm.find_50_peak(
+                    self.model["edge"]["model"],
+                    us_e_eng - self.model["edge"]["eoff"],
+                    np.array(self.model["edge"]["fit_rlt"][0]),
+                    us_p_eng,
+                    self.eng[idx_ps : idx_pe + 1],
+                    self.norm_spec[idx_ps : idx_pe + 1].reshape(
+                        [idx_pe - idx_ps + 1, -1]
+                    ),
+                    ftype=optimizer,
+                ).reshape(self.spec.shape[1:])
+                + self.model["edge"]["eoff"]
+            )
+        elif optimizer == "none":
+            print("none")
+            self.edge50_pos_fit_none = xm.find_50_peak(
+                us_e_eng,
+                self.eng[idx_es : idx_ee + 1],
+                self.norm_spec[idx_es : idx_ee + 1].reshape([idx_ee - idx_es + 1, -1]),
+                us_p_eng,
+                self.eng[idx_ps : idx_pe + 1],
+                self.norm_spec[idx_ps : idx_pe + 1].reshape([idx_pe - idx_ps + 1, -1]),
+                ftype=optimizer,
+            ).reshape(self.spec.shape[1:])
+        elif optimizer == "direct":
+            print("dir")
+            self.edge50_pos_dir = xm.lookup(
+                self.eng[idx_es:idx_ee],
+                self.norm_spec[idx_es:idx_ee].reshape([idx_ee - idx_es, -1]),
+                0.5
+                * self.norm_spec[idx_ps:idx_pe]
+                .reshape([idx_pe - idx_ps, -1])
+                .max(axis=0),
+            ).reshape(self.spec.shape[1:])
 
-    @msgit(wd=100, fill='$')
-    def find_wl(self, es, ee, optimizer='model', ufac=20):
+    @msgit(wd=100, fill="$")
+    def find_wl(self, es, ee, optimizer="model", ufac=20):
         idx_s = xm.index_of(self.eng, es)
         idx_e = xm.index_of(self.eng, ee)
-        if optimizer == 'model':
-            us_eng = np.linspace(self.eng[idx_s], self.eng[idx_e],
-                                 num=(idx_e - idx_s) * ufac) - self.model['wl']['eoff']
-            self.wl_pos_fit, self.wl_ph_fit = xm.find_fit_peak(self.model['wl']['model'],
-                                               np.array(self.model['wl']['fit_rlt'][0]), us_eng) 
-            self.wl_pos_fit += self.model['wl']['eoff']
+        if optimizer == "model":
+            us_eng = (
+                np.linspace(
+                    self.eng[idx_s], self.eng[idx_e], num=(idx_e - idx_s) * ufac
+                )
+                - self.model["wl"]["eoff"]
+            )
+            self.wl_pos_fit, self.wl_ph_fit = xm.find_fit_peak(
+                self.model["wl"]["model"],
+                np.array(self.model["wl"]["fit_rlt"][0]),
+                us_eng,
+            )
+            self.wl_pos_fit += self.model["wl"]["eoff"]
             self.wl_pos_fit = self.wl_pos_fit.reshape(self.spec.shape[1:])
             self.wl_ph_fit = self.wl_ph_fit.reshape(self.spec.shape[1:])
-            print(f"{self.wl_pos_fit.shape=}, {self.wl_ph_fit.shape=}") 
-        elif optimizer == 'direct':
+            print(f"{self.wl_pos_fit.shape=}, {self.wl_ph_fit.shape=}")
+        elif optimizer == "direct":
             if self.norm_spec is None:
-                self.wl_pos_dir = xm.lookup(self.eng[idx_s:idx_e],
-                                            self.spec[idx_s:idx_e].reshape(idx_e - idx_s, -1),
-                                            self.spec[idx_s:idx_e].reshape(idx_e - idx_s, -1).max(axis=0)) \
-                    .reshape(self.spec.shape[1:])
+                self.wl_pos_dir = xm.lookup(
+                    self.eng[idx_s:idx_e],
+                    self.spec[idx_s:idx_e].reshape(idx_e - idx_s, -1),
+                    self.spec[idx_s:idx_e].reshape(idx_e - idx_s, -1).max(axis=0),
+                ).reshape(self.spec.shape[1:])
                 self.wl_ph_dir = np.squeeze(np.max(self.spec[idx_s:idx_e, :], axis=0))
             else:
-                self.wl_pos_dir = xm.lookup(self.eng[idx_s:idx_e],
-                                            self.norm_spec[idx_s:idx_e].reshape(idx_e - idx_s, -1),
-                                            self.norm_spec[idx_s:idx_e].reshape(idx_e - idx_s, -1).max(axis=0)) \
-                    .reshape(self.spec.shape[1:])
-                self.wl_ph_dir = np.squeeze(np.max(self.norm_spec[idx_s:idx_e, :], axis=0))
+                self.wl_pos_dir = xm.lookup(
+                    self.eng[idx_s:idx_e],
+                    self.norm_spec[idx_s:idx_e].reshape(idx_e - idx_s, -1),
+                    self.norm_spec[idx_s:idx_e].reshape(idx_e - idx_s, -1).max(axis=0),
+                ).reshape(self.spec.shape[1:])
+                self.wl_ph_dir = np.squeeze(
+                    np.max(self.norm_spec[idx_s:idx_e, :], axis=0)
+                )
 
-    @msgit(wd=100, fill='$')
-    def find_edge_deriv(self, es, ee, optimizer='model', ufac=20):
+    @msgit(wd=100, fill="$")
+    def find_edge_deriv(self, es, ee, optimizer="model", ufac=20):
         idx_s = xm.index_of(self.eng, es)
         idx_e = xm.index_of(self.eng, ee)
-        us_eng = np.linspace(self.eng[idx_s], self.eng[idx_e],
-                             num=(idx_e - idx_s) * ufac) - self.model['edge']['eoff']
-        if optimizer == 'model':
-            self.edge_pos_fit = xm.find_deriv_peak(self.model['edge']['model'],
-                                                   np.array(self.model['edge']['fit_rlt'][0]), us_eng) \
-                                    .reshape(self.spec.shape[1:]) + self.model['edge']['eoff']
-        elif optimizer == 'direct':
+        us_eng = (
+            np.linspace(self.eng[idx_s], self.eng[idx_e], num=(idx_e - idx_s) * ufac)
+            - self.model["edge"]["eoff"]
+        )
+        if optimizer == "model":
+            self.edge_pos_fit = (
+                xm.find_deriv_peak(
+                    self.model["edge"]["model"],
+                    np.array(self.model["edge"]["fit_rlt"][0]),
+                    us_eng,
+                ).reshape(self.spec.shape[1:])
+                + self.model["edge"]["eoff"]
+            )
+        elif optimizer == "direct":
             if self.norm_spec is None:
                 self.edge_pos_dir = self.spec[idx_s:idx_e].max(axis=0)
             else:
                 self.edge_pos_dir = self.norm_spec[idx_s:idx_e].max(axis=0)
 
     def _finde0(energy, mu):
         if len(energy.shape) > 1:
@@ -380,17 +470,19 @@
         nmin = max(3, int(len(dmu) * 0.05))
         maxdmu = max(dmu[nmin:-nmin])
         high_deriv_pts = np.where(dmu > maxdmu * 0.1)[0]
         idmu_max, dmu_max = 0, 0
         for i in high_deriv_pts:
             if i < nmin or i > len(energy) - nmin:
                 continue
-            if (dmu[i] > dmu_max and
-                    (i + 1 in high_deriv_pts) and
-                    (i - 1 in high_deriv_pts)):
+            if (
+                dmu[i] > dmu_max
+                and (i + 1 in high_deriv_pts)
+                and (i - 1 in high_deriv_pts)
+            ):
                 idmu_max, dmu_max = i, dmu[i]
         return energy[idmu_max]
 
     def find_edge(self):
         """
         ### adopted from larch
         calculate :math:`E_0`, the energy threshold of absorption, or
@@ -414,15 +506,18 @@
         """
         ids = xm.index_of(self.eng, self.pre_ee)
         ide = xm.index_of(self.eng, self.post_es)
         eng = self.eng[ids:ide]
         dim = self.spec[ids:ide, ...].shape
         spec = self.spec[ids:ide, ...].reshape([dim[0], -1])
         with mp.Pool(N_CPU) as pool:
-            rlt = pool.starmap(_finde0, [(eng, spec[:, ii]) for ii in np.int32(np.arange(spec.shape[1]))])
+            rlt = pool.starmap(
+                _finde0,
+                [(eng, spec[:, ii]) for ii in np.int32(np.arange(spec.shape[1]))],
+            )
         pool.close()
         pool.join()
         self.edge_pos_dir = np.array(rlt).reshape(dim[1:])
 
     def find_edge_t(self):
         """calculate :math:`E_0`, the energy threshold of absorption, or
         'edge energy', given :math:`\mu(E)`.
@@ -445,51 +540,172 @@
             2. Supports :ref:`Set XAFS Group` convention within Larch or if `_larch` is set.
         """
         ids = xm.index_of(self.eng, self.pre_ee)
         ide = xm.index_of(self.eng, self.post_es)
         eng = self.eng[ids:ide]
 
         self.edge_pos_dir = np.ndarray(self.spec.shape[1:])
-        distribute_jobs(self.spec[ids:ide, ...], _finde0, 0, kwargs={'energy': eng}, out=self.edge_pos_dir)
+        distribute_jobs(
+            self.spec[ids:ide, ...],
+            _finde0,
+            0,
+            kwargs={"energy": eng},
+            out=self.edge_pos_dir,
+        )
 
     def fit_pre_edge(self):
         """
         return: ndarray, pre_edge_fit has dimension of [2].append(list(spectrum.shape[1:]))
         """
         try:
             kernel = 5 * np.ones([len(self.spec.shape)])
             kernel[0] = 1
-            self.pre_edge_fit_rlt = xm.fit_curv_polynd(self.eng[self.pre_es_idx:self.pre_ee_idx],
-                                                       uniform_filter(self.spec[self.pre_es_idx:self.pre_ee_idx],
-                                                                     size=kernel), 1)
+            self.pre_edge_fit_rlt = xm.fit_curv_polynd(
+                self.eng[self.pre_es_idx : self.pre_ee_idx],
+                uniform_filter(
+                    self.spec[self.pre_es_idx : self.pre_ee_idx], size=kernel
+                ),
+                1,
+            )
             self.pre_edge_fitted = True
         except Exception as e:
             self.pre_edge_fitted = False
             print(str(e))
             print("pre_edge fitting went wrong")
 
     def fit_post_edge(self):
         """
         return: ndarray, post_edge_fit has dimension of [2].append(list(spectrum.shape[1:]))
         """
         try:
-            kernel = 5*np.ones([len(self.spec.shape)])
+            kernel = 5 * np.ones([len(self.spec.shape)])
             kernel[0] = 1
-            self.post_edge_fit_rlt = xm.fit_curv_polynd(self.eng[self.post_es_idx:self.post_ee_idx],
-                                                        uniform_filter(self.spec[self.post_es_idx:self.post_ee_idx],
-                                                                      size=kernel), 1)
+            self.post_edge_fit_rlt = xm.fit_curv_polynd(
+                self.eng[self.post_es_idx : self.post_ee_idx],
+                uniform_filter(
+                    self.spec[self.post_es_idx : self.post_ee_idx], size=kernel
+                ),
+                1,
+            )
             self.post_edge_fitted = True
         except Exception as e:
             print(type(e))
             print(e.args)
             print(e)
             self.post_edge_fitted = False
             print("post_edge fitting went wrong")
 
-    def fit_spec(self, es, ee, eoff, optimizer, flt_spec, on, *args, **kwargs):
+    # def fit_spec(self, es, ee, eoff, optimizer, on, *args, flt_spec=False, **kwargs):
+    #     """
+    #     Provide curve fitting api to that are based on numpy.ployfit and
+    #     scipy.optimize.lsq.
+    #     Parameters
+    #     ----------
+    #     es : flot
+    #         energy starting point in eV.
+    #     ee : flot
+    #         energy end point in eV.
+    #     eoff: float
+    #         energy value offset in eV; for 'numpy' option, a meaningful value, e.g.,
+    #         edge energy, is necessary to obtain good results
+    #     optimizer : str
+    #         'scipy': lsq based
+    #         'numpy': numpy.polyfit based.
+    #     flt_spec: boolean
+    #         if median filtering the spectrum before fitting,
+    #     on: str
+    #         fitting on either 'raw' or 'norm'(alized) spectrum data
+    #     *args: positional arguments to fitting functions
+    #         'scipy':
+    #             model: model function name
+    #             fvars: model function's initial argument values
+    #         'numpy':
+    #             order: order of the polynomial fitting function
+    #     **kwargs : keyword arguments to fitting functions
+    #         'scipy': least_squares arguments
+    #             bnds=None,
+    #             ftol=1e-7,
+    #             xtol=1e-7,
+    #             gtol=1e-7,
+    #             jac='3-point',
+    #             method='trf'
+    #         'numpy': NA
+
+    #     Returns
+    #     -------
+    #     rlt: ndarray of object
+    #         rlt[0]: coef of fitting curve.
+    #         rlt[1:4]: residuals, rank, singular_values, rcond in numpy.polyfit case
+    #         rlt[1:3]: cost, status, success in scipy.optimize.lsq case
+
+    #     """
+    #     idx_s = xm.index_of(self.eng, es)
+    #     idx_e = xm.index_of(self.eng, ee)
+    #     if flt_spec or (flt_spec == "True"):
+    #         flt_kernal = np.ones(len(self.spec.shape), dtype=np.int32)
+    #         flt_kernal[0] = 3
+
+    #         if on == "raw":
+    #             if optimizer == "scipy":
+    #                 fit_rlt = xm.fit_curv_scipy(
+    #                     self.eng[idx_s:idx_e] - eoff,
+    #                     median_filter(self.spec[idx_s:idx_e, :], size=flt_kernal),
+    #                     *args,
+    #                     **kwargs,
+    #                 )
+    #             elif optimizer == "numpy":
+    #                 fit_rlt = xm.fit_curv_polynd(
+    #                     self.eng[idx_s:idx_e] - eoff,
+    #                     median_filter(self.spec[idx_s:idx_e, :], size=flt_kernal),
+    #                     *args,
+    #                 )
+    #         elif on == "norm":
+    #             if optimizer == "scipy":
+    #                 fit_rlt = xm.fit_curv_scipy(
+    #                     self.eng[idx_s:idx_e] - eoff,
+    #                     median_filter(self.norm_spec[idx_s:idx_e, :], size=flt_kernal),
+    #                     *args,
+    #                     **kwargs,
+    #                 )
+    #             elif optimizer == "numpy":
+    #                 fit_rlt = xm.fit_curv_polynd(
+    #                     self.eng[idx_s:idx_e] - eoff,
+    #                     median_filter(self.norm_spec[idx_s:idx_e, :], size=flt_kernal),
+    #                     *args,
+    #                 )
+    #     else:
+    #         if on == "raw":
+    #             if optimizer == "scipy":
+    #                 fit_rlt = xm.fit_curv_scipy(
+    #                     self.eng[idx_s:idx_e] - eoff,
+    #                     self.spec[idx_s:idx_e, :],
+    #                     *args,
+    #                     **kwargs,
+    #                 )
+    #             elif optimizer == "numpy":
+    #                 fit_rlt = xm.fit_curv_polynd(
+    #                     self.eng[idx_s:idx_e] - eoff, self.spec[idx_s:idx_e, :], *args
+    #                 )
+    #         elif on == "norm":
+    #             if optimizer == "scipy":
+    #                 fit_rlt = xm.fit_curv_scipy(
+    #                     self.eng[idx_s:idx_e] - eoff,
+    #                     self.norm_spec[idx_s:idx_e, :],
+    #                     *args,
+    #                     **kwargs,
+    #                 )
+    #             elif optimizer == "numpy":
+    #                 fit_rlt = xm.fit_curv_polynd(
+    #                     self.eng[idx_s:idx_e] - eoff,
+    #                     self.norm_spec[idx_s:idx_e, :],
+    #                     *args,
+    #                 )
+    #     return fit_rlt
+
+    def _fit_spec(self, es, ee, eoff, optimizer, on, *args, **kwargs):
         """
         Provide curve fitting api to that are based on numpy.ployfit and
         scipy.optimize.lsq.
         Parameters
         ----------
         es : flot
             energy starting point in eV.
@@ -527,145 +743,196 @@
             rlt[0]: coef of fitting curve.
             rlt[1:4]: residuals, rank, singular_values, rcond in numpy.polyfit case
             rlt[1:3]: cost, status, success in scipy.optimize.lsq case
 
         """
         idx_s = xm.index_of(self.eng, es)
         idx_e = xm.index_of(self.eng, ee)
-        if flt_spec or (flt_spec == 'True'):
-            flt_kernal = np.ones(len(self.spec.shape), dtype=np.int32)
-            flt_kernal[0] = 3
-
-            if on == "raw":
-                if optimizer == "scipy":
-                    fit_rlt = xm.fit_curv_scipy(self.eng[idx_s:idx_e] - eoff,
-                                                median_filter(self.spec[idx_s:idx_e, :],
-                                                              size=flt_kernal),
-                                                *args, **kwargs)
-                elif optimizer == "numpy":
-                    fit_rlt = xm.fit_curv_polynd(self.eng[idx_s:idx_e] - eoff,
-                                                 median_filter(self.spec[idx_s:idx_e, :],
-                                                               size=flt_kernal),
-                                                 *args)
-            elif on == "norm":
-                if optimizer == "scipy":
-                    fit_rlt = xm.fit_curv_scipy(self.eng[idx_s:idx_e] - eoff,
-                                                median_filter(self.norm_spec[idx_s:idx_e, :],
-                                                              size=flt_kernal),
-                                                *args, **kwargs)
-                elif optimizer == "numpy":
-                    fit_rlt = xm.fit_curv_polynd(self.eng[idx_s:idx_e] - eoff,
-                                                 median_filter(self.norm_spec[idx_s:idx_e, :],
-                                                               size=flt_kernal),
-                                                 *args)
-        else:
-            if on == "raw":
-                if optimizer == "scipy":
-                    fit_rlt = xm.fit_curv_scipy(self.eng[idx_s:idx_e] - eoff,
-                                                self.spec[idx_s:idx_e, :],
-                                                *args, **kwargs)
-                elif optimizer == "numpy":
-                    fit_rlt = xm.fit_curv_polynd(self.eng[idx_s:idx_e] - eoff,
-                                                 self.spec[idx_s:idx_e, :],
-                                                 *args)
-            elif on == "norm":
-                if optimizer == "scipy":
-                    fit_rlt = xm.fit_curv_scipy(self.eng[idx_s:idx_e] - eoff,
-                                                self.norm_spec[idx_s:idx_e, :],
-                                                *args, **kwargs)
-                elif optimizer == "numpy":
-                    fit_rlt = xm.fit_curv_polynd(self.eng[idx_s:idx_e] - eoff,
-                                                 self.norm_spec[idx_s:idx_e, :],
-                                                 *args)
+        if on == "raw":
+            if optimizer == "scipy":
+                fit_rlt = xm.fit_curv_scipy(
+                    self.eng[idx_s:idx_e] - eoff,
+                    self.spec[idx_s:idx_e, :],
+                    *args,
+                    **kwargs,
+                )
+            elif optimizer == "numpy":
+                fit_rlt = xm.fit_curv_polynd(
+                    self.eng[idx_s:idx_e] - eoff, self.spec[idx_s:idx_e, :], *args
+                )
+        elif on == "norm":
+            if optimizer == "scipy":
+                fit_rlt = xm.fit_curv_scipy(
+                    self.eng[idx_s:idx_e] - eoff,
+                    self.norm_spec[idx_s:idx_e, :],
+                    *args,
+                    **kwargs,
+                )
+            elif optimizer == "numpy":
+                fit_rlt = xm.fit_curv_polynd(
+                    self.eng[idx_s:idx_e] - eoff,
+                    self.norm_spec[idx_s:idx_e, :],
+                    *args,
+                )
         return fit_rlt
 
-    def fit_edge(self, es, ee, eoff=None, optimizer='numpy',
-                 flt_spec=False, on='norm', ftype='edge', order=3,
-                 model='lorentzian', fvars=None,
-                 bnds=None, ftol=1e-7, xtol=1e-7,
-                 gtol=1e-7, jac='3-point',
-                 method='trf'):
+    def fit_spec(
+        self,
+        es,
+        ee,
+        eoff=None,
+        optimizer="numpy",
+        on="norm",
+        ftype="edge",
+        order=3,
+        model="lorentzian",
+        fvars=None,
+        bnds=None,
+        ftol=1e-7,
+        xtol=1e-7,
+        gtol=1e-7,
+        jac="3-point",
+        method="trf",
+    ):
+        print(f"{optimizer=}")
         if eoff is None:
             eoff = self.preset_edge_eng
         if optimizer == "numpy":
-            self.model[ftype]['model'] = 'polynd'
+            self.model[ftype]["model"] = "polynd"
             args = [order]
             kwargs = {}
         elif optimizer == "scipy":
-            self.model[ftype]['model'] = model
+            self.model[ftype]["model"] = model
             args = [model, fvars]
-            kwargs = {'bnds': bnds, 'ftol': ftol, 'xtol': xtol, 'gtol': gtol,
-                      'jac': jac, 'method': method}
-        self.model[ftype]['eoff'] = eoff
-        self.model[ftype]['fit_rlt'] = self.fit_spec(es, ee, eoff, optimizer, flt_spec, on,
-                                                     *args, **kwargs)
+            kwargs = {
+                "bnds": bnds,
+                "ftol": ftol,
+                "xtol": xtol,
+                "gtol": gtol,
+                "jac": jac,
+                "method": method,
+            }
+        self.model[ftype]["eoff"] = eoff
+        self.model[ftype]["fit_rlt"] = self._fit_spec(
+            es, ee, eoff, optimizer, on, *args, **kwargs
+        )
+
+    def fit_edge(
+        self,
+        es,
+        ee,
+        eoff=None,
+        optimizer="numpy",
+        flt_spec=False,
+        on="norm",
+        ftype="edge",
+        order=3,
+        model="lorentzian",
+        fvars=None,
+        bnds=None,
+        ftol=1e-7,
+        xtol=1e-7,
+        gtol=1e-7,
+        jac="3-point",
+        method="trf",
+    ):
+        if eoff is None:
+            eoff = self.preset_edge_eng
+        if optimizer == "numpy":
+            self.model[ftype]["model"] = "polynd"
+            args = [order]
+            kwargs = {}
+        elif optimizer == "scipy":
+            self.model[ftype]["model"] = model
+            args = [model, fvars]
+            kwargs = {
+                "bnds": bnds,
+                "ftol": ftol,
+                "xtol": xtol,
+                "gtol": gtol,
+                "jac": jac,
+                "method": method,
+            }
+        self.model[ftype]["eoff"] = eoff
+        self.model[ftype]["fit_rlt"] = self.fit_spec(
+            es, ee, eoff, optimizer, flt_spec, on, *args, **kwargs
+        )
 
-    @msgit(wd=100, fill='$')
+    @msgit(wd=100, fill="$")
     def full_spec_preprocess(self, eng0, order=1, save_pre_post=False):
         e0_idx = xm.index_of(self.eng, eng0)
         pre = self.cal_pre_edge_fit(self.eng)
         post = self.cal_post_edge_fit(self.eng)
 
-        self.edge_jump_mask = np.squeeze((post[e0_idx] - pre[e0_idx])
-                                         > self.edge_jump_thres * self.pre_edge_sd_map).astype(np.int8)
-        self.fitted_edge_mask = np.any((post - pre) > self.fitted_edge_thres * self.pre_edge_sd_map, axis=0).astype(
-            np.int8)
-
-        self.norm_spec = (self.spec - pre) / (self.cal_post_edge_fit(eng0) - self.cal_pre_edge_fit(eng0))
+        self.edge_jump_mask = np.squeeze(
+            (post[e0_idx] - pre[e0_idx]) > self.edge_jump_thres * self.pre_edge_sd_map
+        ).astype(np.int8)
+        self.fitted_edge_mask = np.any(
+            (post - pre) > self.fitted_edge_thres * self.pre_edge_sd_map, axis=0
+        ).astype(np.int8)
+
+        self.norm_spec = (self.spec - pre) / (
+            self.cal_post_edge_fit(eng0) - self.cal_pre_edge_fit(eng0)
+        )
         self.norm_spec[np.isnan(self.norm_spec)] = 0
         self.norm_spec[np.isinf(self.norm_spec)] = 0
 
     def interp_ref_spec(self):
         self.lcf_ref_spec = np.ndarray([self.eng.shape[0], self.lcf_ref.index.size])
         for ii in range(self.lcf_ref.index.size):
-            c = splrep(self.lcf_ref.iloc[ii]['eng'], self.lcf_ref.iloc[ii]['mu'])
+            c = splrep(self.lcf_ref.iloc[ii]["eng"], self.lcf_ref.iloc[ii]["mu"])
             self.lcf_ref_spec[:, ii] = splev(self.eng, c)
 
-    @msgit(wd=100, fill='+')
+    @msgit(wd=100, fill="+")
     def lcf(self):
-        self.lcf_model['constr'] = self.lcf_constr_use
-        self.lcf_model['ref'] = self.lcf_ref
-        self.lcf_model['rlt'] = xm.lcf(self.lcf_ref_spec, self.norm_spec, constr=self.lcf_constr_use)
-        self.lcf_fit = self.lcf_model['rlt'][0].reshape(self.lcf_model['rlt'][0].shape[0], *self.spec.shape[1:])
-        self.lcf_fit_err = self.lcf_model['rlt'][1].reshape(*self.spec.shape[1:])
+        self.lcf_model["constr"] = self.lcf_constr_use
+        self.lcf_model["ref"] = self.lcf_ref
+        self.lcf_model["rlt"] = xm.lcf(
+            self.lcf_ref_spec, self.norm_spec, constr=self.lcf_constr_use
+        )
+        self.lcf_fit = self.lcf_model["rlt"][0].reshape(
+            self.lcf_model["rlt"][0].shape[0], *self.spec.shape[1:]
+        )
+        self.lcf_fit_err = self.lcf_model["rlt"][1].reshape(*self.spec.shape[1:])
 
-    @msgit(wd=100, fill='+')
+    @msgit(wd=100, fill="+")
     def normalize_xanes(self, eng0, order=1, save_pre_post=False):
         """
         For 2D XANES, self.spec dimensions are [eng, 2D_space]
         For 3D XANES, self.spec dimensions are [eng, 3D_space]
 
         normalize_xanes includes two steps: 1) pre-edge background subtraction (order = 0)),
                                             2) post-edge fitted or average mu normalization (order = 1)
         return: ndarray, same dimension as spectrum.shape
         """
         eng = deepcopy(self.eng)
         for ii in range(1, self.pre_edge_fit_rlt[0].ndim):
             eng = eng[:, np.newaxis]
 
         if order == 0:
-            self.norm_spec = (self.spec - self.pre_edge_mean_map) / \
-                             (self.post_edge_mean_map - self.pre_edge_mean_map)
+            self.norm_spec = (self.spec - self.pre_edge_mean_map) / (
+                self.post_edge_mean_map - self.pre_edge_mean_map
+            )
             self.norm_spec[np.isnan(self.norm_spec)] = 0
             self.norm_spec[np.isinf(self.norm_spec)] = 0
             self.spec_normalized = True
         elif order == 1:
             if save_pre_post:
                 e0_idx = xm.index_of(self.eng, eng0)
                 self.pre_edge_fit = self.cal_pre_edge_fit(self.eng)
                 self.post_edge_fit = self.cal_post_edge_fit([eng])
                 self.norm_spec = (self.spec - self.pre_edge_fit) / (
-                        self.post_edge_fit[e0_idx] - self.pre_edge_fit[e0_idx])
+                    self.post_edge_fit[e0_idx] - self.pre_edge_fit[e0_idx]
+                )
                 self.norm_spec[np.isnan(self.norm_spec)] = 0
                 self.norm_spec[np.isinf(self.norm_spec)] = 0
             else:
-                self.norm_spec = (self.spec -
-                                  self.cal_pre_edge_fit([eng0])) / (
-                                         self.cal_post_edge_fit([eng0]) -
-                                         self.cal_pre_edge_fit([eng0]))
+                self.norm_spec = (self.spec - self.cal_pre_edge_fit([eng0])) / (
+                    self.cal_post_edge_fit([eng0]) - self.cal_pre_edge_fit([eng0])
+                )
                 self.norm_spec[np.isnan(self.norm_spec)] = 0
                 self.norm_spec[np.isinf(self.norm_spec)] = 0
             self.spec_normalized = True
         else:
             print('Order can only be "1" or "0".')
             self.spec_normalized = False
 
@@ -674,123 +941,137 @@
         self.eng = np.delete(self.eng, id_list, axis=0)
         self.removed_img_ids = id_list
         self.pre_es_idx = xm.index_of(self.eng, self.pre_es)
         self.pre_ee_idx = xm.index_of(self.eng, self.pre_ee)
         self.post_es_idx = xm.index_of(self.eng, self.post_es)
         self.post_ee_idx = xm.index_of(self.eng, self.post_ee)
 
-    def save_results(self, filename, dtype='2D_XANES', **kwargs):
+    def save_results(self, filename, dtype="2D_XANES", **kwargs):
         filename = Path(filename)
-        assert filename.suffix.lower() in ['.h5', '.hdf', '.hdf5'], \
-            'unsupported file format...'
+        assert filename.suffix.lower() in [
+            ".h5",
+            ".hdf",
+            ".hdf5",
+        ], "unsupported file format..."
         if not filename.parent.exists():
             filename.parent.Path.mkdir(parents=True)
 
-        if dtype == '2D_XANES':
-            f = h5py.File(filename, 'a')
-            if 'XANES_preprocessing' not in f:
-                g1 = f.create_group('XANES_preprocessing')
+        if dtype == "2D_XANES":
+            f = h5py.File(filename, "a")
+            if "XANES_preprocessing" not in f:
+                g1 = f.create_group("XANES_preprocessing")
             else:
-                del f['XANES_preprocessing']
-                g1 = f.create_group('XANES_preprocessing')
+                del f["XANES_preprocessing"]
+                g1 = f.create_group("XANES_preprocessing")
 
-            g1.create_dataset('preset_edge_eng', data=self.preset_edge_eng)
-            g1.create_dataset('removed_img_ids', data=self.removed_img_ids)
-            g1.create_dataset('pre_edge_fit_coef', data=self.pre_edge_fit_rlt[0])
-            g1.create_dataset('post_edge_fit_coef', data=self.post_edge_fit_rlt[0])
-            g1.create_dataset('pre_edge_sd_map', data=self.pre_edge_sd_map)
-            g1.create_dataset('post_edge_sd_map', data=self.post_edge_sd_map)
-            g1.create_dataset('pre_edge_avg', data=self.pre_avg)
-            g1.create_dataset('post_edge_avg', data=self.post_avg)
-            g1.create_dataset('edge_jump_map', data=self.edge_jump_map)
-            g11 = g1.create_group('fitting_configurations')
-            g11.create_dataset('pre_edge_energy_range', data=[self.pre_es, self.pre_ee])
-            g11.create_dataset('post_edge_energy_range', data=[self.post_es, self.post_ee])
+            g1.create_dataset("preset_edge_eng", data=self.preset_edge_eng)
+            g1.create_dataset("removed_img_ids", data=self.removed_img_ids)
+            g1.create_dataset("pre_edge_fit_coef", data=self.pre_edge_fit_rlt[0])
+            g1.create_dataset("post_edge_fit_coef", data=self.post_edge_fit_rlt[0])
+            g1.create_dataset("pre_edge_sd_map", data=self.pre_edge_sd_map)
+            g1.create_dataset("post_edge_sd_map", data=self.post_edge_sd_map)
+            g1.create_dataset("pre_edge_avg", data=self.pre_avg)
+            g1.create_dataset("post_edge_avg", data=self.post_avg)
+            g1.create_dataset("edge_jump_map", data=self.edge_jump_map)
+            g11 = g1.create_group("fitting_configurations")
+            g11.create_dataset("pre_edge_energy_range", data=[self.pre_es, self.pre_ee])
+            g11.create_dataset(
+                "post_edge_energy_range", data=[self.post_es, self.post_ee]
+            )
 
-            if 'XANES_filtering' not in f:
-                g2 = f.create_group('XANES_filtering')
+            if "XANES_filtering" not in f:
+                g2 = f.create_group("XANES_filtering")
             else:
-                del f['XANES_filtering']
-                g2 = f.create_group('XANES_filtering')
+                del f["XANES_filtering"]
+                g2 = f.create_group("XANES_filtering")
 
-            g21 = g2.create_group('edge_jump_filter')
-            g21.create_dataset('edge_jump_threshold', data=self.edge_jump_thres)
-            g21.create_dataset('edge_jump_mask', data=self.edge_jump_mask.astype(np.int8))
-            g22 = g2.create_group('fitted_edge_fitler')
-            g22.create_dataset('fitted_edge_threshold', data=self.fitted_edge_thres)
-            g22.create_dataset('fitted_edge_mask', data=self.fitted_edge_mask.astype(np.int8))
+            g21 = g2.create_group("edge_jump_filter")
+            g21.create_dataset("edge_jump_threshold", data=self.edge_jump_thres)
+            g21.create_dataset(
+                "edge_jump_mask", data=self.edge_jump_mask.astype(np.int8)
+            )
+            g22 = g2.create_group("fitted_edge_fitler")
+            g22.create_dataset("fitted_edge_threshold", data=self.fitted_edge_thres)
+            g22.create_dataset(
+                "fitted_edge_mask", data=self.fitted_edge_mask.astype(np.int8)
+            )
 
-            if 'XANES_results' not in f:
-                g3 = f.create_group('XANES_results')
+            if "XANES_results" not in f:
+                g3 = f.create_group("XANES_results")
             else:
-                del f['XANES_results']
-                g3 = f.create_group('XANES_results')
+                del f["XANES_results"]
+                g3 = f.create_group("XANES_results")
 
-            g3.create_dataset('eng', data=self.eng.astype(np.float32), dtype=np.float32)
-            g3.create_dataset('normalized_spectrum', data=self.norm_spec.astype(np.float32), dtype=np.float32)
-            g3.create_dataset('edge_pos', data=self.auto_e0.astype(np.float32), dtype=np.float32)
-            g3.create_dataset('edge_0.5_pos', data=self.edge_pos.astype(np.float32), dtype=np.float32)
-            g3.create_dataset('whiteline_pos_fit', data=self.wl_pos_fit.astype(np.float32), dtype=np.float32)
-            g3.create_dataset('whiteline_pos_direct', data=self.wl_pos_dir.astype(np.float32), dtype=np.float32)
+            g3.create_dataset("eng", data=self.eng.astype(np.float32), dtype=np.float32)
+            g3.create_dataset(
+                "normalized_spectrum",
+                data=self.norm_spec.astype(np.float32),
+                dtype=np.float32,
+            )
+            g3.create_dataset(
+                "edge_pos", data=self.auto_e0.astype(np.float32), dtype=np.float32
+            )
+            g3.create_dataset(
+                "edge_0.5_pos", data=self.edge_pos.astype(np.float32), dtype=np.float32
+            )
+            g3.create_dataset(
+                "whiteline_pos_fit",
+                data=self.wl_pos_fit.astype(np.float32),
+                dtype=np.float32,
+            )
+            g3.create_dataset(
+                "whiteline_pos_direct",
+                data=self.wl_pos_dir.astype(np.float32),
+                dtype=np.float32,
+            )
 
             f.close()
-        elif dtype == '3D_XANES':
-            f = h5py.File(filename, 'a')
-            if 'processed_XANES3D' not in f:
-                g1 = f.create_group('processed_XANES3D')
+        elif dtype == "3D_XANES":
+            f = h5py.File(filename, "a")
+            if "processed_XANES3D" not in f:
+                g1 = f.create_group("processed_XANES3D")
             else:
-                del f['processed_XANES3D']
-                g1 = f.create_group('processed_XANES3D')
+                del f["processed_XANES3D"]
+                g1 = f.create_group("processed_XANES3D")
 
-            g1.create_dataset('removed_img_ids',
-                              data=self.removed_img_ids)
-            g1.create_dataset('pre_edge_fit_coef',
-                              data=self.pre_edge_fit_rlt[0])
-            g1.create_dataset('post_edge_fit_coef',
-                              data=self.post_edge_fit_rlt[0])
-            g1.create_dataset('pre_edge_sd_map',
-                              data=self.pre_edge_sd_map)
-            g1.create_dataset('post_edge_sd_map',
-                              data=self.post_edge_sd_map)
-            g1.create_dataset('pre_edge_avg',
-                              data=self.pre_avg)
-            g1.create_dataset('post_edge_avg',
-                              data=self.post_avg)
-            g1.create_dataset('edge_jump_map',
-                              data=self.edge_jump_map)
-            g1.create_dataset('edge_jump_threshold',
-                              data=self.edge_jump_thres)
-            g1.create_dataset('fitted_edge_threshold',
-                              data=self.fitted_edge_thres)
-            g11 = g1.create_group('fitting_configurations')
-            g11.create_dataset('pre_edge_energy_range',
-                               data=[self.pre_es, self.pre_ee])
-            g11.create_dataset('post_edge_energy_range',
-                               data=[self.post_es, self.post_ee])
+            g1.create_dataset("removed_img_ids", data=self.removed_img_ids)
+            g1.create_dataset("pre_edge_fit_coef", data=self.pre_edge_fit_rlt[0])
+            g1.create_dataset("post_edge_fit_coef", data=self.post_edge_fit_rlt[0])
+            g1.create_dataset("pre_edge_sd_map", data=self.pre_edge_sd_map)
+            g1.create_dataset("post_edge_sd_map", data=self.post_edge_sd_map)
+            g1.create_dataset("pre_edge_avg", data=self.pre_avg)
+            g1.create_dataset("post_edge_avg", data=self.post_avg)
+            g1.create_dataset("edge_jump_map", data=self.edge_jump_map)
+            g1.create_dataset("edge_jump_threshold", data=self.edge_jump_thres)
+            g1.create_dataset("fitted_edge_threshold", data=self.fitted_edge_thres)
+            g11 = g1.create_group("fitting_configurations")
+            g11.create_dataset("pre_edge_energy_range", data=[self.pre_es, self.pre_ee])
+            g11.create_dataset(
+                "post_edge_energy_range", data=[self.post_es, self.post_ee]
+            )
 
-            if 'XANES_results' not in f:
-                g3 = f.create_group('XANES_results')
+            if "XANES_results" not in f:
+                g3 = f.create_group("XANES_results")
             else:
-                del f['XANES_results']
-                g3 = f.create_group('XANES_results')
+                del f["XANES_results"]
+                g3 = f.create_group("XANES_results")
 
-            g3.create_dataset('eng',
-                              data=self.eng.astype(np.float32),
-                              dtype=np.float32)
+            g3.create_dataset("eng", data=self.eng.astype(np.float32), dtype=np.float32)
             for key, item in kwargs.items():
-                g3.create_dataset(key,
-                                  data=item.astype(np.float32),
-                                  dtype=np.float32)
+                g3.create_dataset(key, data=item.astype(np.float32), dtype=np.float32)
             f.close()
         else:
-            print('Unrecognized data type!')
+            print("Unrecognized data type!")
 
     def set_external_mask(self, mask):
         self.ext_mask = mask
 
+    def smooth_spec(self):
+        pass
+
     def update_with_auto_e0(self):
         self.find_edge()
 
         self.pre_ee = self.auto_e0 + (self.pre_ee - self.preset_edge_eng)
         self.pre_ee_idx = xm.index_of(self.eng, self.pre_ee)
 
         self.post_es = self.auto_e0 + (self.post_es - self.preset_edge_eng)
```

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_image_utils.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_math.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_post_analysis.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_regtools.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_regtools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox/utils/xanes_spectra_filters.py` & `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post4/txm_sandbox.egg-info/SOURCES.txt` & `txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

