# Comparing `tmp/pix2text-1.0.2.3.tar.gz` & `tmp/pix2text-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2text-1.0.2.3.tar", last modified: Fri Mar 29 23:37:12 2024, max compression
+gzip compressed data, was "pix2text-1.1.tar", last modified: Sun Apr 28 15:17:52 2024, max compression
```

## Comparing `pix2text-1.0.2.3.tar` & `pix2text-1.1.tar`

### file list

```diff
@@ -1,52 +1,88 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-03-29 23:37:12.968266 pix2text-1.0.2.3/
--rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.0.2.3/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    35769 2024-03-29 23:37:12.968090 pix2text-1.0.2.3/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    34655 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-03-29 23:37:12.963428 pix2text-1.0.2.3/pix2text/
--rw-r--r--   0 king       (501) staff       (20)      303 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/pix2text/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      203 2024-03-29 23:26:06.000000 pix2text-1.0.2.3/pix2text/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.0.2.3/pix2text/app.py
--rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.0.2.3/pix2text/category_mapping.py
--rw-r--r--   0 king       (501) staff       (20)     8858 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/pix2text/cli.py
--rw-r--r--   0 king       (501) staff       (20)     3710 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/pix2text/consts.py
--rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.0.2.3/pix2text/element.py
--rw-r--r--   0 king       (501) staff       (20)    17680 2024-03-29 16:02:24.000000 pix2text-1.0.2.3/pix2text/latex_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.0.2.3/pix2text/latex_ocr0.py
--rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.0.2.3/pix2text/latex_recog.py
--rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.0.2.3/pix2text/object_detector.py
--rw-r--r--   0 king       (501) staff       (20)     7151 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/pix2text/ocr_engine.py
--rw-r--r--   0 king       (501) staff       (20)    27161 2024-03-29 16:06:34.000000 pix2text-1.0.2.3/pix2text/pix_to_text.py
--rw-r--r--   0 king       (501) staff       (20)     5395 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/pix2text/render.py
--rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.0.2.3/pix2text/screenshot_daemon_with_server2.py
--rw-r--r--   0 king       (501) staff       (20)     2191 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/pix2text/serve.py
--rw-r--r--   0 king       (501) staff       (20)     4164 2024-03-27 11:51:46.000000 pix2text-1.0.2.3/pix2text/table_element.py
--rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.0.2.3/pix2text/table_inference.py
--rw-r--r--   0 king       (501) staff       (20)    25447 2024-03-29 15:25:54.000000 pix2text-1.0.2.3/pix2text/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-03-29 23:37:12.964535 pix2text-1.0.2.3/pix2text.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    35769 2024-03-29 23:37:12.000000 pix2text-1.0.2.3/pix2text.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     1157 2024-03-29 23:37:12.000000 pix2text-1.0.2.3/pix2text.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2024-03-29 23:37:12.000000 pix2text-1.0.2.3/pix2text.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       42 2024-03-29 23:37:12.000000 pix2text-1.0.2.3/pix2text.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.0.2.3/pix2text.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      246 2024-03-29 23:37:12.000000 pix2text-1.0.2.3/pix2text.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)       17 2024-03-29 23:37:12.000000 pix2text-1.0.2.3/pix2text.egg-info/top_level.txt
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-03-29 23:37:12.967302 pix2text-1.0.2.3/scripts/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.0.2.3/scripts/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.0.2.3/scripts/convert_label_studio_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.0.2.3/scripts/extract_p2t_results.py
--rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.0.2.3/scripts/gen_label_studio_json.py
--rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.0.2.3/scripts/gen_pure_formula_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.0.2.3/scripts/merge_label_studio_anno_pred_json.py
--rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.0.2.3/scripts/object_detection3.py
--rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.0.2.3/scripts/screenshot_daemon.py
--rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.0.2.3/scripts/try_easyocr.py
--rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.0.2.3/scripts/try_latex_correction.py
--rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.0.2.3/scripts/try_layout.py
--rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/scripts/try_pix2text_mfr.py
--rw-r--r--   0 king       (501) staff       (20)      736 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/scripts/try_service.py
--rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.0.2.3/scripts/try_texify.py
--rw-r--r--   0 king       (501) staff       (20)       38 2024-03-29 23:37:12.968309 pix2text-1.0.2.3/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     2377 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-03-29 23:37:12.967849 pix2text-1.0.2.3/tests/
--rw-r--r--   0 king       (501) staff       (20)     4249 2024-03-29 15:11:40.000000 pix2text-1.0.2.3/tests/test_pix2text.py
--rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.0.2.3/tests/test_sort_boxes.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.802331 pix2text-1.1/
+-rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    14010 2024-04-28 15:17:52.802182 pix2text-1.1/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    12900 2024-04-28 15:01:52.000000 pix2text-1.1/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.790881 pix2text-1.1/pix2text/
+-rw-r--r--   0 king       (501) staff       (20)      456 2024-04-02 11:11:40.000000 pix2text-1.1/pix2text/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      199 2024-04-23 07:32:19.000000 pix2text-1.1/pix2text/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1/pix2text/app.py
+-rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1/pix2text/category_mapping.py
+-rw-r--r--   0 king       (501) staff       (20)    10451 2024-04-22 00:51:42.000000 pix2text-1.1/pix2text/cli.py
+-rw-r--r--   0 king       (501) staff       (20)     3710 2024-04-16 14:50:16.000000 pix2text-1.1/pix2text/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.793545 pix2text-1.1/pix2text/doc_xl_layout/
+-rw-r--r--   0 king       (501) staff       (20)      192 2024-04-03 01:13:56.000000 pix2text-1.1/pix2text/doc_xl_layout/__init__.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.794415 pix2text-1.1/pix2text/doc_xl_layout/detectors/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/detectors/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     8390 2024-04-02 08:34:16.000000 pix2text-1.1/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     8722 2024-04-02 07:16:21.000000 pix2text-1.1/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)      137 2024-04-02 06:45:51.000000 pix2text-1.1/pix2text/doc_xl_layout/detectors/detector_factory.py
+-rw-r--r--   0 king       (501) staff       (20)    17874 2024-04-23 15:41:22.000000 pix2text-1.1/pix2text/doc_xl_layout/doc_xl_layout_parser.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.794748 pix2text-1.1/pix2text/doc_xl_layout/external/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/external/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2510 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/external/shapelyNMS.py
+-rw-r--r--   0 king       (501) staff       (20)      365 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/huntie_subfield.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.796266 pix2text-1.1/pix2text/doc_xl_layout/models/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     5178 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/data_parallel.py
+-rw-r--r--   0 king       (501) staff       (20)    23840 2024-04-02 07:32:06.000000 pix2text-1.1/pix2text/doc_xl_layout/models/decode.py
+-rw-r--r--   0 king       (501) staff       (20)     3443 2024-04-10 11:32:17.000000 pix2text-1.1/pix2text/doc_xl_layout/models/model.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.796593 pix2text-1.1/pix2text/doc_xl_layout/models/networks/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/networks/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    24395 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     1528 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/scatter_gather.py
+-rw-r--r--   0 king       (501) staff       (20)     1800 2024-04-02 07:31:48.000000 pix2text-1.1/pix2text/doc_xl_layout/models/utils.py
+-rw-r--r--   0 king       (501) staff       (20)    23801 2024-04-02 00:43:23.000000 pix2text-1.1/pix2text/doc_xl_layout/opts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.798435 pix2text-1.1/pix2text/doc_xl_layout/utils/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4818 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/ddd_utils.py
+-rw-r--r--   0 king       (501) staff       (20)    26623 2024-04-02 06:59:29.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/debugger.py
+-rw-r--r--   0 king       (501) staff       (20)    18383 2024-04-02 06:47:12.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/evaluation_bk.py
+-rw-r--r--   0 king       (501) staff       (20)     7851 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/image.py
+-rw-r--r--   0 king       (501) staff       (20)     5368 2024-04-02 06:47:54.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/post_process.py
+-rw-r--r--   0 king       (501) staff       (20)      533 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/utils.py
+-rw-r--r--   0 king       (501) staff       (20)     8844 2024-04-02 06:20:49.000000 pix2text-1.1/pix2text/doc_xl_layout/wrapper.py
+-rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1/pix2text/element.py
+-rw-r--r--   0 king       (501) staff       (20)    17431 2024-04-22 02:21:39.000000 pix2text-1.1/pix2text/latex_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1/pix2text/latex_ocr0.py
+-rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1/pix2text/latex_recog.py
+-rw-r--r--   0 king       (501) staff       (20)     4016 2024-04-06 13:32:28.000000 pix2text-1.1/pix2text/layout_parser.py
+-rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1/pix2text/object_detector.py
+-rw-r--r--   0 king       (501) staff       (20)     7285 2024-04-27 13:58:01.000000 pix2text-1.1/pix2text/ocr_engine.py
+-rw-r--r--   0 king       (501) staff       (20)    10461 2024-04-26 06:27:40.000000 pix2text-1.1/pix2text/page_elements.py
+-rw-r--r--   0 king       (501) staff       (20)    28192 2024-04-24 14:01:37.000000 pix2text-1.1/pix2text/pix_to_text.py
+-rw-r--r--   0 king       (501) staff       (20)     5395 2024-03-29 15:11:40.000000 pix2text-1.1/pix2text/render.py
+-rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1/pix2text/screenshot_daemon_with_server2.py
+-rw-r--r--   0 king       (501) staff       (20)     2776 2024-04-21 15:29:44.000000 pix2text-1.1/pix2text/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1/pix2text/table_inference.py
+-rw-r--r--   0 king       (501) staff       (20)    38298 2024-04-22 02:22:30.000000 pix2text-1.1/pix2text/table_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    37328 2024-03-29 23:43:03.000000 pix2text-1.1/pix2text/table_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)    24628 2024-04-22 00:24:28.000000 pix2text-1.1/pix2text/text_formula_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    31700 2024-04-21 13:52:16.000000 pix2text-1.1/pix2text/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.792208 pix2text-1.1/pix2text.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    14010 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     2405 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       42 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1/pix2text.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      269 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)       17 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/top_level.txt
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.801470 pix2text-1.1/scripts/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1/scripts/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1/scripts/convert_label_studio_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1/scripts/extract_p2t_results.py
+-rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1/scripts/gen_label_studio_json.py
+-rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1/scripts/gen_pure_formula_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1/scripts/merge_label_studio_anno_pred_json.py
+-rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1/scripts/object_detection3.py
+-rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1/scripts/screenshot_daemon.py
+-rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1/scripts/try_easyocr.py
+-rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1/scripts/try_latex_correction.py
+-rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1/scripts/try_layout.py
+-rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1/scripts/try_pix2text_mfr.py
+-rw-r--r--   0 king       (501) staff       (20)      845 2024-04-21 15:31:13.000000 pix2text-1.1/scripts/try_service.py
+-rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1/scripts/try_texify.py
+-rw-r--r--   0 king       (501) staff       (20)       38 2024-04-28 15:17:52.802375 pix2text-1.1/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     2424 2024-04-28 15:13:23.000000 pix2text-1.1/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.801961 pix2text-1.1/tests/
+-rw-r--r--   0 king       (501) staff       (20)     5861 2024-04-10 11:52:24.000000 pix2text-1.1/tests/test_pix2text.py
+-rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1/tests/test_sort_boxes.py
```

### Comparing `pix2text-1.0.2.3/LICENSE` & `pix2text-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/app.py` & `pix2text-1.1/pix2text/app.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/category_mapping.py` & `pix2text-1.1/pix2text/category_mapping.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/consts.py` & `pix2text-1.1/pix2text/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from typing import Set, Tuple, Dict, Any, Optional
 
 from .__version__ import __version__
 
 logger = logging.getLogger(__name__)
 
 # 模型版本只对应到第二层，第三层的改动表示模型兼容。
-# 如: __version__ = '0.1.*'，对应的 MODEL_VERSION 都是 '0.1'
+# 如: __version__ = '1.0.*'，对应的 MODEL_VERSION 都是 '1.0'
 MODEL_VERSION = '.'.join(__version__.split('.', maxsplit=2)[:2])
-DOWNLOAD_SOURCE = os.environ.get('PIX2TEXT_DOWNLOAD_SOURCE', 'CN')
+DOWNLOAD_SOURCE = os.environ.get('PIX2TEXT_DOWNLOAD_SOURCE', 'HF')
 
 CN_OSS_ENDPOINT = (
         "https://sg-models.oss-cn-beijing.aliyuncs.com/pix2text/%s/" % MODEL_VERSION
 )
 
 
 def format_model_info(info: dict) -> dict:
```

### Comparing `pix2text-1.0.2.3/pix2text/element.py` & `pix2text-1.1/pix2text/element.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/latex_ocr.py` & `pix2text-1.1/pix2text/latex_ocr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # coding: utf-8
 # [Pix2Text](https://github.com/breezedeus/pix2text): an Open-Source Alternative to Mathpix.
 # Copyright (C) 2022-2024, [Breezedeus](https://www.breezedeus.com).
+import os
+import shutil
 import string
 from typing import Optional, Union, List, Dict, Any
 import logging
 from pathlib import Path
 import re
 
 import torch
@@ -48,23 +50,24 @@
             model_backend (str, optional): The model backend, either 'onnx' or 'pytorch'. Defaults to 'onnx'.
             device (str, optional): What device to use for computation, supports `['cpu', 'cuda', 'gpu']`; defaults to None, which selects the device automatically.
             context (str, optional): Deprecated, use `device` instead. What device to use for computation, supports `['cpu', 'cuda', 'gpu']`; defaults to None, which selects the device automatically.
             model_dir (Optional[Union[str, Path]], optional): The model file directory. Defaults to None.
             root (Union[str, Path], optional): The model root directory. Defaults to data_dir().
             more_processor_configs (Optional[Dict[str, Any]], optional): Additional processor configurations. Defaults to None.
             more_model_configs (Optional[Dict[str, Any]], optional): Additional model configurations. Defaults to None.
-             - provider (`str`, defaults to `None`, which means to select one provider automatically):
-                 ONNX Runtime provider to use for loading the model. See https://onnxruntime.ai/docs/execution-providers/ for
-                 possible providers.
-             - session_options (`Optional[onnxruntime.SessionOptions]`, defaults to `None`),:
-                 ONNX Runtime session options to use for loading the model.
-             - provider_options (`Optional[Dict[str, Any]]`, defaults to `None`):
-                 Provider option dictionaries corresponding to the provider used. See available options
-                 for each provider: https://onnxruntime.ai/docs/api/c/group___global.html .
-             - ...: see more information here: optimum.onnxruntime.modeling_ort.ORTModel.from_pretrained()
+
+                - provider (`str`, defaults to `None`, which means to select one provider automatically):
+                    ONNX Runtime provider to use for loading the model. See https://onnxruntime.ai/docs/execution-providers/ for
+                    possible providers.
+                - session_options (`Optional[onnxruntime.SessionOptions]`, defaults to `None`),:
+                    ONNX Runtime session options to use for loading the model.
+                - provider_options (`Optional[Dict[str, Any]]`, defaults to `None`):
+                    Provider option dictionaries corresponding to the provider used. See available options
+                    for each provider: https://onnxruntime.ai/docs/api/c/group___global.html .
+                - ...: see more information here: optimum.onnxruntime.modeling_ort.ORTModel.from_pretrained()
             **kwargs: Additional arguments, currently not used.
         """
 
         if context is not None:
             logger.warning(f'`context` is deprecated, please use `device` instead')
         if device is None and context is not None:
             device = context
@@ -96,32 +99,22 @@
 
     def _prepare_model_files(self, root, model_backend, model_info):
         model_root_dir = Path(root) / MODEL_VERSION
         model_dir = model_root_dir / model_info['local_model_id']
         if model_dir.is_dir():
             return str(model_dir)
         assert 'hf_model_id' in model_info
-        try:
-            more_model_configs = (
-                {'provider': 'CPUExecutionProvider'} if model_backend == 'onnx' else {}
-            )
-            model, processor = self._init_model(
-                model_backend,
-                model_info['hf_model_id'],
-                more_model_config=more_model_configs,
-            )
-            model.save_pretrained(model_dir)
-            processor.save_pretrained(model_dir)
-            logger.info(f'Saved Pix2Text MFR model to: {model_dir}')
-        except Exception as e:
-            logger.warning(f'Failed to download model from HuggingFace: {e}')
-            logger.warning(f'Downloading model from CN OSS ...')
-            get_model_file(
-                model_info, model_dir, download_source='CN'
-            )  # download the .zip file and unzip
+        model_dir.mkdir(parents=True)
+        download_cmd = f'huggingface-cli download --repo-type model --resume-download --local-dir-use-symlinks False {model_info["hf_model_id"]} --local-dir {model_dir}'
+        os.system(download_cmd)
+        # 如果当前目录下无文件，就从huggingface上下载
+        if not list(model_dir.glob('**/[!.]*')):
+            if model_dir.exists():
+                shutil.rmtree(str(model_dir))
+            os.system('HF_ENDPOINT=https://hf-mirror.com ' + download_cmd)
         return model_dir
 
     def _init_model(
         self,
         model_backend,
         model_dir,
         more_processor_config=None,
```

### Comparing `pix2text-1.0.2.3/pix2text/latex_ocr0.py` & `pix2text-1.1/pix2text/latex_ocr0.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/latex_recog.py` & `pix2text-1.1/pix2text/latex_recog.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/object_detector.py` & `pix2text-1.1/pix2text/object_detector.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/ocr_engine.py` & `pix2text-1.1/pix2text/ocr_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 import cv2
 
 
 def clip(x, min_value, max_value):
     return min(max(x, min_value), max_value)
 
 
-class OcrEngineWrapper:
+class TextOcrEngine:
     """Text OCR Engine Wrapper"""
 
     name = 'unknown'
 
-    def __init__(self, ocr_engine):
+    def __init__(self, languages: Sequence[str], ocr_engine):
+        self.languages = languages
         self.ocr_engine = ocr_engine
 
     def detect_only(self, img: np.ndarray, **kwargs):
         """
         Only detect the texts from the input image.
         Args:
             img (np.ndarray): RGB image with shape: (height, width, 3)
@@ -98,19 +99,19 @@
               }]
             ```
         """
 
         pass
 
 
-class CnOCREngineWrapper(OcrEngineWrapper):
+class CnOCREngine(TextOcrEngine):
     name = 'cnocr'
 
     def detect_only(self, img: np.ndarray, **kwargs):
-        outs = self.ocr_engine.det_model.detect(img)
+        outs = self.ocr_engine.det_model.detect(img, **kwargs)
         for out in outs['detected_texts']:
             out['position'] = out.pop('box')
         return outs
 
     def recognize_only(self, img: np.ndarray, **kwargs):
         try:
             return self.ocr_engine.ocr_for_single_line(img)
@@ -119,18 +120,20 @@
 
     def ocr(self, img: np.ndarray, rec_config: Optional[dict] = None, **kwargs) -> str:
         rec_config = rec_config or {}
         outs = self.ocr_engine.ocr(img, **rec_config)
         return outs
 
 
-class EasyOCREngineWrapper(OcrEngineWrapper):
+class EasyOCREngine(TextOcrEngine):
     name = 'easyocr'
 
     def detect_only(self, img: np.ndarray, **kwargs):
+        if 'resized_shape' in kwargs:
+            kwargs.pop('resized_shape')
         img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
         height, width = img.shape[:2]
         horizontal_list, free_list = self.ocr_engine.detect(img, **kwargs)
         horizontal_list, free_list = horizontal_list[0], free_list[0]
         bboxes = []
         for x1x2_y1y2 in horizontal_list:
             xmin, xmax, ymin, ymax = x1x2_y1y2
@@ -171,20 +174,20 @@
 
 
 def prepare_ocr_engine(languages: Sequence[str], ocr_engine_config):
     if len(set(languages).difference({'en', 'ch_sim'})) == 0:
         from cnocr import CnOcr
 
         ocr_engine = CnOcr(**ocr_engine_config)
-        engine_wrapper = CnOCREngineWrapper(ocr_engine)
+        engine_wrapper = CnOCREngine(languages, ocr_engine)
     else:
         try:
             from easyocr import Reader
         except:
             raise ImportError('Please install easyocr first: pip install easyocr')
         gpu = False
         if 'context' in ocr_engine_config:
             context = ocr_engine_config.pop('context').lower()
             gpu = 'gpu' in context or 'cuda' in context
         ocr_engine = Reader(lang_list=list(languages), gpu=gpu, **ocr_engine_config)
-        engine_wrapper = EasyOCREngineWrapper(ocr_engine)
+        engine_wrapper = EasyOCREngine(languages, ocr_engine)
     return engine_wrapper
```

### Comparing `pix2text-1.0.2.3/pix2text/pix_to_text.py` & `pix2text-1.1/pix2text/text_formula_ocr.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # Copyright (C) 2022-2024, [Breezedeus](https://www.breezedeus.com).
 
 import logging
 import re
 from itertools import chain
 from pathlib import Path
 from typing import Dict, Any, Optional, Union, List, Sequence
-from copy import copy
+from copy import copy, deepcopy
 
 from PIL import Image
 import numpy as np
 import torch
 from cnstd import LayoutAnalyzer
-from cnstd.yolov7.consts import CATEGORY_DICT
 from cnstd.yolov7.general import box_partial_overlap
+from spellchecker import SpellChecker
 
 from .utils import (
     sort_boxes,
     merge_adjacent_bboxes,
     adjust_line_height,
     adjust_line_width,
     rotated_box_to_horizontal,
@@ -26,207 +26,239 @@
     list2box,
     select_device,
     prepare_imgs,
     merge_line_texts,
     remove_overlap_text_bbox,
     y_overlap,
 )
-from .ocr_engine import prepare_ocr_engine
-
-from .consts import MODEL_VERSION
+from .ocr_engine import prepare_ocr_engine, TextOcrEngine
 from .latex_ocr import LatexOCR
 from .utils import (
     read_img,
     save_layout_img,
 )
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_CONFIGS = {
-    'analyzer': {'model_name': 'mfd'},
+    'mfd': {},
     'text': {},
     'formula': {},
 }
+# see: https://pypi.org/project/pyspellchecker
+CHECKER_SUPPORTED_LANGUAGES = {
+    'en',
+    'es',
+    'fr',
+    'pt',
+    'de',
+    'it',
+    'ru',
+    'ar',
+    'eu',
+    'lv',
+    'nl',
+}
 
 
-class Pix2Text(object):
-    MODEL_FILE_PREFIX = 'pix2text-v{}'.format(MODEL_VERSION)
-
+class TextFormulaOCR(object):
     def __init__(
         self,
         *,
-        languages: Union[str, Sequence[str]] = ('en', 'ch_sim'),
-        analyzer_config: Dict[str, Any] = None,
-        text_config: Dict[str, Any] = None,
-        formula_config: Dict[str, Any] = None,
+        text_ocr: Optional[TextOcrEngine] = None,
+        mfd: Optional[LayoutAnalyzer] = None,
+        latex_ocr: Optional[LatexOCR] = None,
+        spellchecker: Optional[SpellChecker] = None,
+        **kwargs,
+    ):
+        if text_ocr is None:
+            text_config = deepcopy(DEFAULT_CONFIGS['text'])
+            device = select_device(device=None)
+            text_config['context'] = device
+            logger.warning(
+                f'text_ocr must not be None. Using default text_ocr engine instead, with config: {text_config}.'
+            )
+            text_ocr = prepare_ocr_engine(
+                languages=('en', 'ch_sim'), ocr_engine_config=text_config
+            )
+        # if mfd is None or latex_ocr is None:
+        #     default_ocr = TextFormulaOCR.from_config()
+        #     mfd = default_ocr.mfd if mfd is None else mfd
+        #     text_ocr = default_ocr.text_ocr if text_ocr is None else text_ocr
+        #     latex_ocr = default_ocr.latex_ocr if latex_ocr is None else latex_ocr
+        #     del default_ocr
+
+        self.text_ocr = text_ocr
+        self.mfd = mfd
+        self.latex_ocr = latex_ocr
+        self.spellchecker = spellchecker
+
+    @classmethod
+    def from_config(
+        cls,
+        total_configs: Optional[dict] = None,
+        enable_formula: bool = True,
+        enable_spell_checker: bool = True,
         device: str = None,
         **kwargs,
     ):
         """
         Args:
-            languages (str or Sequence[str]): The language code(s) of the text to be recognized; defaults to `('en', 'ch_sim')`.
-            analyzer_config (dict): Configuration information for the Analyzer model; defaults to `None`, which means using the default configuration.
-            text_config (dict): Configuration information for the Text OCR model; defaults to `None`, which means using the default configuration.
-            formula_config (dict): Configuration information for Math Formula OCR model; defaults to `None`, which means using the default configuration.
+            total_configs (dict): Configuration information for Pix2Text; defaults to `None`, which means using the default configuration. Usually the following keys are used:
+
+                * languages (str or Sequence[str]): The language code(s) of the text to be recognized; defaults to `('en', 'ch_sim')`.
+                * mfd (dict): Configuration information for the Analyzer model; defaults to `None`, which means using the default configuration.
+                * text (dict): Configuration information for the Text OCR model; defaults to `None`, which means using the default configuration.
+                * formula (dict): Configuration information for Math Formula OCR model; defaults to `None`, which means using the default configuration.
+            enable_formula (bool): Whether to enable the capability of Math Formula Detection (MFD) and Recognition (MFR); defaults to True.
+            enable_spell_checker (bool): Whether to enable the capability of Spell Checker; defaults to True.
             device (str, optional): What device to use for computation, supports `['cpu', 'cuda', 'gpu', 'mps']`; defaults to None, which selects the device automatically.
             **kwargs (): Reserved for other parameters; not currently used.
         """
-        self.device = select_device(device)
-
-        analyzer_config, text_config, formula_config = self._prepare_configs(
-            analyzer_config, text_config, formula_config, self.device,
+        total_configs = total_configs or DEFAULT_CONFIGS
+        languages = total_configs.get('languages', ('en', 'ch_sim'))
+        text_config = total_configs.get('text', dict())
+        mfd_config = total_configs.get('mfd', dict())
+        formula_config = total_configs.get('formula', dict())
+
+        device = select_device(device)
+        mfd_config, text_config, formula_config = cls.prepare_configs(
+            mfd_config, text_config, formula_config, device,
         )
 
-        self.analyzer = LayoutAnalyzer(**analyzer_config)
+        text_ocr = prepare_ocr_engine(languages, text_config)
+
+        if enable_formula:
+            if 'model_name' in mfd_config:
+                mfd_config.pop('model_name')
+            mfd = LayoutAnalyzer(model_name='mfd', **mfd_config)
+            latex_ocr = LatexOCR(**formula_config)
+        else:
+            mfd = None
+            latex_ocr = None
+
+        spellchecker = None
+        if enable_spell_checker:
+            checker_languages = set(languages) & CHECKER_SUPPORTED_LANGUAGES
+            if checker_languages:
+                spellchecker = SpellChecker(language=checker_languages)
 
-        self.languages = languages
-        self.text_ocr = prepare_ocr_engine(languages, text_config)
-        self.latex_model = LatexOCR(**formula_config)
+        return cls(
+            text_ocr=text_ocr,
+            mfd=mfd,
+            latex_ocr=latex_ocr,
+            spellchecker=spellchecker,
+            **kwargs,
+        )
 
-    def _prepare_configs(
-        self, analyzer_config, text_config, formula_config, device,
+    @classmethod
+    def prepare_configs(
+        cls, mfd_config, text_config, formula_config, device,
     ):
         def _to_default(_conf, _def_val):
             if not _conf:
                 _conf = _def_val
             return _conf
 
-        analyzer_config = _to_default(analyzer_config, DEFAULT_CONFIGS['analyzer'])
+        mfd_config = _to_default(mfd_config, DEFAULT_CONFIGS['mfd'])
         # FIXME
-        analyzer_config['device'] = device if device != 'mps' else 'cpu'
+        mfd_config['device'] = device if device != 'mps' else 'cpu'
         text_config = _to_default(text_config, DEFAULT_CONFIGS['text'])
         text_config['context'] = device
         formula_config = _to_default(formula_config, DEFAULT_CONFIGS['formula'])
         formula_config['device'] = device
         return (
-            analyzer_config,
+            mfd_config,
             text_config,
             formula_config,
         )
 
-    @classmethod
-    def from_config(cls, total_configs: Optional[dict] = None, device: str = 'cpu'):
-        total_configs = total_configs or DEFAULT_CONFIGS
-        return cls(
-            analyzer_config=total_configs.get('analyzer', dict()),
-            text_config=total_configs.get('text', dict()),
-            formula_config=total_configs.get('formula', dict()),
-            device=device,
-        )
+    @property
+    def languages(self):
+        return self.text_ocr.languages
 
     def __call__(
         self, img: Union[str, Path, Image.Image], **kwargs
     ) -> List[Dict[str, Any]]:
         return self.recognize(img, **kwargs)
 
     def recognize(
         self, img: Union[str, Path, Image.Image], return_text: bool = True, **kwargs
     ) -> Union[str, List[Dict[str, Any]]]:
         """
-        Analyze the layout of the image, and then recognize the information contained in each section.
-
-        Args:
-            img (str or Image.Image): an image path, or `Image.Image` loaded by `Image.open()`
-            return_text (bool): Whether to return only the recognized text; default value is `True`
-            kwargs ():
-                * resized_shape (int): Resize the image width to this size for processing; default value is `608`
-                * save_analysis_res (str): Save the analysis result image in this file; default is `None`, which means not to save
-                * mfr_batch_size (int): batch size for MFR; When running on GPU, this value is suggested to be set to greater than 1; default value is `1`
-                * embed_sep (tuple): Prefix and suffix for embedding latex; only effective when `return_text` is `True`; default value is `(' $', '$ ')`
-                * isolated_sep (tuple): Prefix and suffix for isolated latex; only effective when `return_text` is `True`; default value is `('$$\n', '\n$$')`
-                * line_sep (str): The separator between lines of text; only effective when `return_text` is `True`; default value is `'\n'`
-                * auto_line_break (bool): Automatically line break the recognized text; only effective when `return_text` is `True`; default value is `True`
-                * det_text_bbox_max_width_expand_ratio (float): Expand the width of the detected text bbox. This value represents the maximum expansion ratio above and below relative to the original bbox height; default value is `0.3`
-                * det_text_bbox_max_height_expand_ratio (float): Expand the height of the detected text bbox. This value represents the maximum expansion ratio above and below relative to the original bbox height; default value is `0.2`
-                * embed_ratio_threshold (float): The overlap threshold for embed formulas and text lines; default value is `0.6`.
-                    When the overlap between an embed formula and a text line is greater than or equal to this threshold,
-                    the embed formula and the text line are considered to be on the same line;
-                    otherwise, they are considered to be on different lines.
-                * formula_rec_kwargs (dict): generation arguments passed to formula recognizer `latex_ocr`; default value is `{}`
-
-        Returns: a str when `return_text` is `True`; or a list of ordered (top to bottom, left to right) dicts when `return_text` is `False`,
-            with each dict representing one detected box, containing keys:
-               * `type`: The category of the image; Optional: 'text', 'isolated', 'embedding'
-               * `text`: The recognized text or Latex formula
-               * `score`: The confidence score [0, 1]; the higher, the more confident
-               * `position`: Position information of the block, `np.ndarray`, with shape of [4, 2]
-               * `line_number`: The line number of the box (first line `line_number==0`), boxes with the same value indicate they are on the same line
-
-        """
-        if self.analyzer._model_name == 'mfd':
-            out = self.recognize_by_mfd(img, return_text=return_text, **kwargs)
-        else:
-            out = self.recognize_by_layout(img, **kwargs)
-        return out
-
-    def recognize_by_mfd(
-        self, img: Union[str, Path, Image.Image], return_text: bool = True, **kwargs
-    ) -> Union[str, List[Dict[str, Any]]]:
-        """
         Perform Mathematical Formula Detection (MFD) on the image, and then recognize the information contained in each section.
 
         Args:
             img (str or Image.Image): an image path, or `Image.Image` loaded by `Image.open()`
             return_text (bool): Whether to return only the recognized text; default value is `True`
             kwargs ():
-                * resized_shape (int): Resize the image width to this size for processing; default value is `608`
+                * contain_formula (bool): If `True`, the image will be recognized as a mixed image (text and formula). If `False`, it will be recognized as a text; default value is `True`
+                * resized_shape (int): Resize the image width to this size for processing; default value is `768`
                 * save_analysis_res (str): Save the parsed result image in this file; default value is `None`, which means not to save
                 * mfr_batch_size (int): batch size for MFR; When running on GPU, this value is suggested to be set to greater than 1; default value is `1`
                 * embed_sep (tuple): Prefix and suffix for embedding latex; only effective when `return_text` is `True`; default value is `(' $', '$ ')`
-                * isolated_sep (tuple): Prefix and suffix for isolated latex; only effective when `return_text` is `True`; default value is `('$$\n', '\n$$')`
-                * line_sep (str): The separator between lines of text; only effective when `return_text` is `True`; default value is `'\n'`
+                * isolated_sep (tuple): Prefix and suffix for isolated latex; only effective when `return_text` is `True`; default value is two-dollar signs
+                * line_sep (str): The separator between lines of text; only effective when `return_text` is `True`; default value is a line break
                 * auto_line_break (bool): Automatically line break the recognized text; only effective when `return_text` is `True`; default value is `True`
                 * det_text_bbox_max_width_expand_ratio (float): Expand the width of the detected text bbox. This value represents the maximum expansion ratio above and below relative to the original bbox height; default value is `0.3`
                 * det_text_bbox_max_height_expand_ratio (float): Expand the height of the detected text bbox. This value represents the maximum expansion ratio above and below relative to the original bbox height; default value is `0.2`
                 * embed_ratio_threshold (float): The overlap threshold for embed formulas and text lines; default value is `0.6`.
                     When the overlap between an embed formula and a text line is greater than or equal to this threshold,
                     the embed formula and the text line are considered to be on the same line;
                     otherwise, they are considered to be on different lines.
                 * formula_rec_kwargs (dict): generation arguments passed to formula recognizer `latex_ocr`; default value is `{}`
 
         Returns: a str when `return_text` is `True`, or a list of ordered (top to bottom, left to right) dicts when `return_text` is `False`,
             with each dict representing one detected box, containing keys:
-               * `type`: The category of the image; Optional: 'text', 'isolated', 'embedding'
-               * `text`: The recognized text or Latex formula
-               * `score`: The confidence score [0, 1]; the higher, the more confident
-               * `position`: Position information of the block, `np.ndarray`, with shape of [4, 2]
-               * `line_number`: The line number of the box (first line `line_number==0`), boxes with the same value indicate they are on the same line
+
+                * `type`: The category of the image; Optional: 'text', 'isolated', 'embedding'
+                * `text`: The recognized text or Latex formula
+                * `score`: The confidence score [0, 1]; the higher, the more confident
+                * `position`: Position information of the block, `np.ndarray`, with shape of [4, 2]
+                * `line_number`: The line number of the box (first line `line_number==0`), boxes with the same value indicate they are on the same line
 
         """
         # 对于大图片，把图片宽度resize到此大小；宽度比此小的图片，其实不会放大到此大小，
         # 具体参考：cnstd.yolov7.layout_analyzer.LayoutAnalyzer._preprocess_images 中的 `letterbox` 行
-        resized_shape = kwargs.get('resized_shape', 608)
+        resized_shape = kwargs.get('resized_shape', 768)
         if isinstance(img, Image.Image):
             img0 = img.convert('RGB')
         else:
             img0 = read_img(img, return_type='Image')
         w, h = img0.size
         ratio = resized_shape / w
         resized_shape = (int(h * ratio), resized_shape)  # (H, W)
-        analyzer_outs = self.analyzer(img0.copy(), resized_shape=resized_shape)
         # logger.debug('MFD Result: %s', analyzer_outs)
-
+        analyzer_outs = []
         crop_patches = []
-        for mf_box_info in analyzer_outs:
-            box = mf_box_info['box']
-            xmin, ymin, xmax, ymax = (
-                int(box[0][0]),
-                int(box[0][1]),
-                int(box[2][0]),
-                int(box[2][1]),
+        mf_results = []
+        if (
+            kwargs.get('contain_formula', True)
+            and self.mfd is not None
+            and self.latex_ocr is not None
+        ):
+            analyzer_outs = self.mfd(img0.copy(), resized_shape=resized_shape)
+            for mf_box_info in analyzer_outs:
+                box = mf_box_info['box']
+                xmin, ymin, xmax, ymax = (
+                    int(box[0][0]),
+                    int(box[0][1]),
+                    int(box[2][0]),
+                    int(box[2][1]),
+                )
+                crop_patch = img0.crop((xmin, ymin, xmax, ymax))
+                crop_patches.append(crop_patch)
+
+            mfr_batch_size = kwargs.get('mfr_batch_size', 1)
+            formula_rec_kwargs = kwargs.get('formula_rec_kwargs', {})
+            mf_results = self.latex_ocr.recognize(
+                crop_patches, batch_size=mfr_batch_size, **formula_rec_kwargs
             )
-            crop_patch = img0.crop((xmin, ymin, xmax, ymax))
-            crop_patches.append(crop_patch)
 
-        mfr_batch_size = kwargs.get('mfr_batch_size', 1)
-        formula_rec_kwargs = kwargs.get('formula_rec_kwargs', {})
-        mf_results = self.latex_model.recognize(
-            crop_patches, batch_size=mfr_batch_size, **formula_rec_kwargs
-        )
         assert len(mf_results) == len(analyzer_outs)
 
         mf_outs = []
         for mf_box_info, patch_out in zip(analyzer_outs, mf_results):
             text = patch_out['text']
             mf_outs.append(
                 {
@@ -246,15 +278,17 @@
                 xmax, ymax = (
                     min(img0.size[0], int(box[2][0]) + 1),
                     min(img0.size[1], int(box[2][1]) + 1),
                 )
                 masked_img[ymin:ymax, xmin:xmax, :] = 255
         masked_img = Image.fromarray(masked_img)
 
-        text_box_infos = self.text_ocr.detect_only(np.array(img0))
+        text_box_infos = self.text_ocr.detect_only(
+            np.array(img0), resized_shape=resized_shape
+        )
         box_infos = []
         for line_box_info in text_box_infos['detected_texts']:
             # crop_img_info['box'] 可能是一个带角度的矩形框，需要转换成水平的矩形框
             _text_box = rotated_box_to_horizontal(line_box_info['position'])
             if not is_valid_box(_text_box, min_height=8, min_width=2):
                 continue
             box_infos.append({'position': _text_box})
@@ -344,15 +378,20 @@
 
         if return_text:
             embed_sep = kwargs.get('embed_sep', (' $', '$ '))
             isolated_sep = kwargs.get('isolated_sep', ('$$\n', '\n$$'))
             line_sep = kwargs.get('line_sep', '\n')
             auto_line_break = kwargs.get('auto_line_break', True)
             outs = merge_line_texts(
-                outs, auto_line_break, line_sep, embed_sep, isolated_sep
+                outs,
+                auto_line_break,
+                line_sep,
+                embed_sep,
+                isolated_sep,
+                self.spellchecker,
             )
 
         return outs
 
     def _post_process(self, outs):
         match_pairs = [
             (',', ',，'),
@@ -392,15 +431,15 @@
                             line_boxes[_idx2]['text'] = line_boxes[_idx2]['text'][:-1]
                 # 把 公式 tag 合并到公式里面去
                 for _idx2, box in enumerate(line_boxes[1:]):
                     if (
                         box['type'] == 'text'
                         and line_boxes[_idx2]['type'] == 'isolated'
                     ):  # if the current box is text and the previous box is embedding
-                        if y_overlap(line_boxes[_idx2], box, key='position') > 0.85:
+                        if y_overlap(line_boxes[_idx2], box, key='position') > 0.9:
                             if re.match(formula_tag, box['text']):
                                 # 去掉开头和结尾的括号
                                 tag_text = box['text'][1:-1]
                                 line_boxes[_idx2]['text'] = line_boxes[_idx2][
                                     'text'
                                 ] + ' \\tag{{{}}}'.format(tag_text)
                                 new_xmax = max(
@@ -433,68 +472,14 @@
             start = int(mf['position'][2])
             if _xmax >= xmax:
                 break
         if start < xmax:
             outs.append({'position': [start, ymin, xmax, ymax], 'type': 'text'})
         return outs
 
-    def recognize_by_layout(
-        self, img: Union[str, Path, Image.Image], **kwargs
-    ) -> List[Dict[str, Any]]:
-        """
-        Perform Layout Analysis (LA) on the image, then recognize the information contained in each section.
-
-        Args:
-            img (str or Image.Image): an image path, or `Image.Image` loaded by `Image.open()`
-            kwargs ():
-                * resized_shape (int): Resize the image width to this size for processing; default value is `500`
-                * save_analysis_res (str): Save the parsed result image in this file; default value is `None`, which means not to save
-
-        Returns: a list of dicts, with keys:
-           `type`: The category of the image;
-           `text`: The recognized text or Latex formula
-           `position`: Position information of the block, `np.ndarray`, with a shape of [4, 2]
-
-        """
-        if isinstance(img, Image.Image):
-            img0 = img.convert('RGB')
-        else:
-            img0 = read_img(img, return_type='Image')
-        resized_shape = kwargs.get('resized_shape', 500)
-        layout_out = self.analyzer(img0.copy(), resized_shape=resized_shape)
-        logger.debug('Layout Analysis Result: %s', layout_out)
-
-        out = []
-        for box_info in layout_out:
-            box = box_info['box']
-            xmin, ymin, xmax, ymax = (
-                int(box[0][0]),
-                int(box[0][1]),
-                int(box[2][0]),
-                int(box[2][1]),
-            )
-            crop_patch = img0.crop((xmin, ymin, xmax, ymax))
-            image_type = box_info['type']
-            if image_type == 'Equation':
-                patch_out = self.recognize_formula(crop_patch)
-            else:
-                patch_out = self.recognize_text(crop_patch)
-            out.append({'type': image_type, 'text': patch_out, 'position': box})
-
-        if kwargs.get('save_analysis_res'):
-            save_layout_img(
-                img0,
-                CATEGORY_DICT['layout'],
-                layout_out,
-                kwargs.get('save_analysis_res'),
-                key='box',
-            )
-
-        return out
-
     def recognize_text(
         self,
         imgs: Union[str, Path, Image.Image, List[str], List[Path], List[Image.Image]],
         return_text: bool = True,
         rec_config: Optional[dict] = None,
         **kwargs,
     ) -> Union[str, List[str], List[Any], List[List[Any]]]:
@@ -503,35 +488,41 @@
         Args:
             imgs (Union[str, Path, Image.Image], List[str], List[Path], List[Image.Image]): The image or list of images
             return_text (bool): Whether to return only the recognized text; default value is `True`
             rec_config (Optional[dict]): The config for recognition
             kwargs (): Other parameters for `text_ocr.ocr()`
 
         Returns: Text str or list of text strs when `return_text` is True;
-                 `List[Any]` or `List[List[Any]]` when `return_text` is False, with the same length as `imgs` and the following keys:
+                `List[Any]` or `List[List[Any]]` when `return_text` is False, with the same length as `imgs` and the following keys:
+
                     * `position`: Position information of the block, `np.ndarray`, with a shape of [4, 2]
                     * `text`: The recognized text
                     * `score`: The confidence score [0, 1]; the higher, the more confident
 
         """
         is_single_image = False
         if isinstance(imgs, (str, Path, Image.Image)):
             imgs = [imgs]
             is_single_image = True
 
         input_imgs = prepare_imgs(imgs)
 
         outs = []
         for image in input_imgs:
-            result = self.text_ocr.ocr(np.array(image), **kwargs)
+            result = self.text_ocr.ocr(np.array(image), rec_config=rec_config, **kwargs)
             if return_text:
                 texts = [_one['text'] for _one in result]
                 result = '\n'.join(texts)
             outs.append(result)
 
+        if kwargs.get('save_analysis_res'):
+            save_layout_img(
+                input_imgs[0], ['text'], outs[0], kwargs.get('save_analysis_res'),
+            )
+
         if is_single_image:
             return outs[0]
         return outs
 
     def recognize_formula(
         self,
         imgs: Union[str, Path, Image.Image, List[str], List[Path], List[Image.Image]],
@@ -546,21 +537,24 @@
             imgs (Union[str, Path, Image.Image, List[str], List[Path], List[Image.Image]): The image or list of images
             batch_size (int): The batch size
             return_text (bool): Whether to return only the recognized text; default value is `True`
             rec_config (Optional[dict]): The config for recognition
             **kwargs (): Special model parameters. Not used for now
 
         Returns: The LaTeX Expression or list of LaTeX Expressions;
-                 str or List[str] when `return_text` is True;
-                 Dict[str, Any] or List[Dict[str, Any]] when `return_text` is False, with the following keys:
+                str or List[str] when `return_text` is True;
+                Dict[str, Any] or List[Dict[str, Any]] when `return_text` is False, with the following keys:
+
                     * `text`: The recognized LaTeX text
                     * `score`: The confidence score [0, 1]; the higher, the more confident
 
         """
-        outs = self.latex_model.recognize(
+        if self.latex_ocr is None:
+            raise RuntimeError('`latex_ocr` model MUST NOT be None')
+        outs = self.latex_ocr.recognize(
             imgs, batch_size=batch_size, rec_config=rec_config, **kwargs
         )
         if return_text:
             if isinstance(outs, dict):
                 outs = outs['text']
             elif isinstance(outs, list):
                 outs = [one['text'] for one in outs]
@@ -569,12 +563,12 @@
 
 
 if __name__ == '__main__':
     from .utils import set_logger
 
     logger = set_logger(log_level='DEBUG')
 
-    p2t = Pix2Text()
+    p2t = TextFormulaOCR()
     img = 'docs/examples/english.jpg'
     img = read_img(img, return_type='Image')
     out = p2t.recognize(img)
     logger.info(out)
```

### Comparing `pix2text-1.0.2.3/pix2text/render.py` & `pix2text-1.1/pix2text/render.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/screenshot_daemon_with_server2.py` & `pix2text-1.1/pix2text/screenshot_daemon_with_server2.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/table_inference.py` & `pix2text-1.1/pix2text/table_inference.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/pix2text/utils.py` & `pix2text-1.1/pix2text/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import re
 from copy import deepcopy
 from functools import cmp_to_key
 from pathlib import Path
 import logging
 import platform
 from typing import Union, List, Any, Dict
+from collections import Counter, defaultdict
 
 from PIL import Image, ImageOps
 import numpy as np
 from numpy import random
 import torch
 from torchvision.utils import save_image
 
@@ -162,14 +163,60 @@
     # img *= 255
     # img = img.to(dtype=torch.uint8)
     save_image(img, path)
 
     # Image.fromarray(img).save(path)
 
 
+def get_background_color(image: Image.Image, margin=2):
+    width, height = image.size
+
+    # 边缘区域的像素采样
+    edge_pixels = []
+    for x in range(width):
+        for y in range(height):
+            if (
+                x <= margin
+                or y <= margin
+                or x >= width - margin
+                or y >= height - margin
+            ):
+                edge_pixels.append(image.getpixel((x, y)))
+
+    # 统计边缘像素颜色频率
+    color_counter = Counter(edge_pixels)
+
+    # 获取频率最高的颜色
+    background_color = color_counter.most_common(1)[0][0]
+
+    return background_color
+
+
+def add_img_margin(
+    image: Image.Image, left_right_margin, top_bottom_margin, background_color=None
+):
+    if background_color is None:
+        background_color = get_background_color(image)
+
+    # 获取原始图片尺寸
+    width, height = image.size
+
+    # 计算新图片的尺寸
+    new_width = width + left_right_margin * 2
+    new_height = height + top_bottom_margin * 2
+
+    # 创建新图片对象，并填充指定背景色
+    new_image = Image.new("RGB", (new_width, new_height), background_color)
+
+    # 将原始图片粘贴到新图片中央
+    new_image.paste(image, (left_right_margin, top_bottom_margin))
+
+    return new_image
+
+
 def prepare_imgs(imgs: List[Union[str, Path, Image.Image]]) -> List[Image.Image]:
     output_imgs = []
     for img in imgs:
         if isinstance(img, (str, Path)):
             img = read_img(img, return_type='Image')
         elif isinstance(img, Image.Image):
             img = img.convert('RGB')
@@ -187,34 +234,37 @@
     [180, 105, 255],  # 粉红色
     [128, 0, 128],  # 紫色
     [0, 255, 255],  # 黄色
     [255, 191, 0],  # 深天蓝色
     [50, 205, 50],  # 石灰绿色
     [60, 20, 220],  # 猩红色
     [130, 0, 75],  # 靛蓝色
+    [255, 0, 0],  # 红色
+    [0, 255, 0],  # 绿色
+    [0, 0, 255],  # 蓝色
 ]
 
 
 def save_layout_img(img0, categories, one_out, save_path, key='position'):
     import cv2
     from cnstd.yolov7.plots import plot_one_box
 
     """可视化版面分析结果。"""
     if isinstance(img0, Image.Image):
         img0 = cv2.cvtColor(np.asarray(img0.convert('RGB')), cv2.COLOR_RGB2BGR)
 
-    if len(categories) > 10:
+    if len(categories) > 13:
         colors = [[random.randint(0, 255) for _ in range(3)] for _ in categories]
     else:
         colors = COLOR_LIST
     for one_box in one_out:
-        _type = one_box['type']
+        _type = one_box.get('type', 'text')
         box = one_box[key]
         xyxy = [box[0, 0], box[0, 1], box[2, 0], box[2, 1]]
-        label = f'{_type}'
+        label = str(_type)
         plot_one_box(
             xyxy,
             img0,
             label=label,
             color=colors[categories.index(_type)],
             line_thickness=1,
         )
@@ -252,14 +302,25 @@
 
 def list2box(xmin, ymin, xmax, ymax, dtype=float):
     return np.array(
         [[xmin, ymin], [xmax, ymin], [xmax, ymax], [xmin, ymax]], dtype=dtype
     )
 
 
+def box2list(bbox):
+    return [int(bbox[0, 0]), int(bbox[0, 1]), int(bbox[2, 0]), int(bbox[2, 1])]
+
+
+def clipbox(box, img_height, img_width):
+    new_box = np.zeros_like(box)
+    new_box[:, 0] = np.clip(box[:, 0], 0, img_width - 1)
+    new_box[:, 1] = np.clip(box[:, 1], 0, img_height - 1)
+    return new_box
+
+
 def y_overlap(box1, box2, key='position'):
     # 计算它们在y轴上的IOU: Interaction / min(height1, height2)
     if key:
         box1 = [box1[key][0][0], box1[key][0][1], box1[key][2][0], box1[key][2][1]]
         box2 = [box2[key][0][0], box2[key][0][1], box2[key][2][0], box2[key][2][1]]
     else:
         box1 = [box1[0][0], box1[0][1], box1[2][0], box1[2][1]]
@@ -385,14 +446,37 @@
         left_box['line_number'] = line_number
         res_boxes.insert(0, left_box)
         anchor = left_box
 
     return res_boxes
 
 
+def merge_boxes(bbox1, bbox2):
+    """
+    Merge two bounding boxes to get a bounding box that encompasses both.
+
+    Parameters:
+    - bbox1, bbox2: The bounding boxes to merge. Each box is np.ndarray, with shape of [4, 2]
+
+    Returns: new merged box, with shape of [4, 2]
+    """
+    # 解包两个边界框的坐标
+    x_min1, y_min1, x_max1, y_max1 = box2list(bbox1)
+    x_min2, y_min2, x_max2, y_max2 = box2list(bbox2)
+
+    # 计算合并后边界框的坐标
+    x_min = min(x_min1, x_min2)
+    y_min = min(y_min1, y_min2)
+    x_max = max(x_max1, x_max2)
+    y_max = max(y_max1, y_max2)
+
+    # 返回合并后的边界框
+    return list2box(x_min, y_min, x_max, y_max)
+
+
 def sort_boxes(boxes: List[dict], key='position') -> List[List[dict]]:
     # 按y坐标排序所有的框
     boxes.sort(key=lambda box: box[key][0, 1])
     for box in boxes:
         box['line_number'] = -1  # 所在行号，-1表示未分配
 
     def get_anchor():
@@ -639,15 +723,17 @@
 
         if max_overlap_val < 0.1:  # overlap 太少的情况不做任何处理
             new_text_box_infos.append(text_box)
             continue
         # if max_overlap_val > 0.8:  # overlap 太多的情况，直接扔掉 text box
         #     continue
 
-        cropped_text_boxes = crop_box(text_box['position'], max_overlap_fbox['position'])
+        cropped_text_boxes = crop_box(
+            text_box['position'], max_overlap_fbox['position']
+        )
         if cropped_text_boxes:
             for _box in cropped_text_boxes:
                 new_box = deepcopy(text_box)
                 new_box['position'] = _box
                 new_text_box_infos.append(new_box)
 
     return new_text_box_infos
@@ -656,15 +742,25 @@
 def is_chinese(ch):
     """
     判断一个字符是否为中文字符
     """
     return '\u4e00' <= ch <= '\u9fff'
 
 
-def smart_join(str_list):
+def find_first_punctuation_position(text):
+    # 匹配常见标点符号的正则表达式
+    pattern = re.compile(r'[,.!?;:()\[\]{}\'\"\\/-]')
+    match = pattern.search(text)
+    if match:
+        return match.start()
+    else:
+        return len(text)
+
+
+def smart_join(str_list, spellchecker=None):
     """
     对字符串列表进行拼接，如果相邻的两个字符串都是中文或包含空白符号，则不加空格；其他情况则加空格
     """
 
     def contain_whitespace(s):
         if re.search(r'\s', s):
             return True
@@ -676,90 +772,171 @@
         return ''
     res = str_list[0]
     for i in range(1, len(str_list)):
         if (is_chinese(res[-1]) and is_chinese(str_list[i][0])) or contain_whitespace(
             res[-1] + str_list[i][0]
         ):
             res += str_list[i]
+        elif spellchecker is not None and res.endswith('-'):
+            fields = res.rsplit(' ', maxsplit=1)
+            if len(fields) > 1:
+                new_res, prev_word = fields[0], fields[1]
+            else:
+                new_res, prev_word = '', res
+
+            fields = str_list[i].split(' ', maxsplit=1)
+            if len(fields) > 1:
+                next_word, new_next = fields[0], fields[1]
+            else:
+                next_word, new_next = str_list[i], ''
+
+            punct_idx = find_first_punctuation_position(next_word)
+            next_word = next_word[:punct_idx]
+            new_next = str_list[i][len(next_word) :]
+            new_word = prev_word[:-1] + next_word
+            if (
+                next_word
+                and spellchecker.unknown([prev_word + next_word])
+                and spellchecker.known([new_word])
+            ):
+                res = new_res + ' ' + new_word + new_next
+            else:
+                new_word = prev_word + next_word
+                res = new_res + ' ' + new_word + new_next
         else:
             res += ' ' + str_list[i]
     return res
 
 
+def cal_block_xmin_xmax(lines, indentation_thrsh):
+    total_min_x, total_max_x = min(lines[:, 0]), max(lines[:, 1])
+    if lines.shape[0] < 2:
+        return total_min_x, total_max_x
+
+    min_x, max_x = min(lines[1:, 0]), max(lines[1:, 1])
+    first_line_is_full = total_max_x > max_x - indentation_thrsh
+    if first_line_is_full:
+        return min_x, total_max_x
+
+    return total_min_x, total_max_x
+
+
 def merge_line_texts(
     outs: List[Dict[str, Any]],
     auto_line_break: bool = True,
     line_sep='\n',
     embed_sep=(' $', '$ '),
     isolated_sep=('$$\n', '\n$$'),
+    spellchecker=None,
 ) -> str:
     """
     把 Pix2Text.recognize_by_mfd() 的返回结果，合并成单个字符串
     Args:
         outs (List[Dict[str, Any]]):
         auto_line_break: 基于box位置自动判断是否该换行
         line_sep: 行与行之间的分隔符
         embed_sep (tuple): Prefix and suffix for embedding latex; default value is `(' $', '$ ')`
         isolated_sep (tuple): Prefix and suffix for isolated latex; default value is `('$$\n', '\n$$')`
+        spellchecker: Spell Checker
 
     Returns: 合并后的字符串
 
     """
     if not outs:
         return ''
     out_texts = []
     line_margin_list = []  # 每行的最左边和最右边的x坐标
     isolated_included = []  # 每行是否包含了 `isolated` 类型的数学公式
+    line_height_dict = defaultdict(list)  # 每行中每个块对应的高度
+    line_ymin_ymax_list = []  # 每行的最上边和最下边的y坐标
     for _out in outs:
         line_number = _out.get('line_number', 0)
         while len(out_texts) <= line_number:
             out_texts.append([])
-            line_margin_list.append([0, 0])
+            line_margin_list.append([100000, 0])
             isolated_included.append(False)
+            line_ymin_ymax_list.append([100000, 0])
         cur_text = _out['text']
-        if _out['type'] in ('embedding', 'isolated'):
+        cur_type = _out.get('type', 'text')
+        box = _out['position']
+        if cur_type in ('embedding', 'isolated'):
             sep = isolated_sep if _out['type'] == 'isolated' else embed_sep
             cur_text = sep[0] + cur_text + sep[1]
-        if _out['type'] == 'isolated':
+        if cur_type == 'isolated':
             isolated_included[line_number] = True
             cur_text = line_sep + cur_text + line_sep
         out_texts[line_number].append(cur_text)
         line_margin_list[line_number][1] = max(
-            line_margin_list[line_number][1], float(_out['position'][2, 0])
+            line_margin_list[line_number][1], float(box[2, 0])
         )
         line_margin_list[line_number][0] = min(
-            line_margin_list[line_number][0], float(_out['position'][0, 0])
+            line_margin_list[line_number][0], float(box[0, 0])
         )
+        if cur_type == 'text':
+            line_height_dict[line_number].append(box[2, 1] - box[1, 1])
+            line_ymin_ymax_list[line_number][0] = min(
+                line_ymin_ymax_list[line_number][0], float(box[0, 1])
+            )
+            line_ymin_ymax_list[line_number][1] = max(
+                line_ymin_ymax_list[line_number][1], float(box[2, 1])
+            )
 
     line_text_list = [smart_join(o) for o in out_texts]
 
+    for _line_number in line_height_dict.keys():
+        if line_height_dict[_line_number]:
+            line_height_dict[_line_number] = np.mean(line_height_dict[_line_number])
+    _line_heights = list(line_height_dict.values())
+    mean_height = np.mean(_line_heights) if _line_heights else None
+
+    default_res = re.sub(rf'{line_sep}+', line_sep, line_sep.join(line_text_list))
     if not auto_line_break:
-        return re.sub(rf'{line_sep}+', line_sep, line_sep.join(line_text_list))
+        return default_res
 
     line_lengths = [rx - lx for lx, rx in line_margin_list]
     line_length_thrsh = max(line_lengths) * 0.3
+    if line_length_thrsh < 1:
+        return default_res
 
     lines = np.array(
         [
             margin
             for idx, margin in enumerate(line_margin_list)
             if isolated_included[idx] or line_lengths[idx] >= line_length_thrsh
         ]
     )
-    min_x, max_x = lines.max(axis=0)
+    if lines.shape[0] < 1:
+        return default_res
+    min_x, max_x = min(lines[:, 0]), max(lines[:, 1])
 
     indentation_thrsh = (max_x - min_x) * 0.1
+    if mean_height is not None:
+        indentation_thrsh = 1.5 * mean_height
+
+    min_x, max_x = cal_block_xmin_xmax(lines, indentation_thrsh)
+
+    line_text_list = [(idx, txt) for idx, txt in enumerate(line_text_list) if txt]
     res_line_texts = [''] * len(line_text_list)
-    for idx, txt in enumerate(line_text_list):
-        if isolated_included[idx]:
-            res_line_texts[idx] = line_sep + txt + line_sep
+    for idx, (line_number, txt) in enumerate(line_text_list):
+        if isolated_included[line_number]:
+            res_line_texts[line_number] = line_sep + txt + line_sep
             continue
 
         tmp = txt
-        if line_margin_list[idx][0] > min_x + indentation_thrsh:
+        if line_margin_list[line_number][0] > min_x + indentation_thrsh:
             tmp = line_sep + txt
-        if line_margin_list[idx][1] < max_x - indentation_thrsh:
+        if line_margin_list[line_number][1] < max_x - indentation_thrsh:
             tmp = tmp + line_sep
+        if idx < len(line_text_list) - 1:
+            cur_height = line_ymin_ymax_list[line_number][1] - line_ymin_ymax_list[line_number][0]
+            next_line_number = line_text_list[idx + 1][0]
+            if (
+                cur_height > 0
+                and line_ymin_ymax_list[next_line_number][0] < line_ymin_ymax_list[next_line_number][1]
+                and line_ymin_ymax_list[next_line_number][0] - line_ymin_ymax_list[line_number][1]
+                > cur_height
+            ):  # 当前行与下一行的间距超过了一行的行高，则认为它们之间应该是不同的段落
+                tmp = tmp + line_sep
         res_line_texts[idx] = tmp
 
-    outs = smart_join(res_line_texts)
+    outs = smart_join(res_line_texts, spellchecker)
     return re.sub(rf'{line_sep}+', line_sep, outs)  # 把多个 '\n' 替换为 '\n'
```

### Comparing `pix2text-1.0.2.3/scripts/convert_label_studio_to_yolov7.py` & `pix2text-1.1/scripts/convert_label_studio_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/extract_p2t_results.py` & `pix2text-1.1/scripts/extract_p2t_results.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/gen_label_studio_json.py` & `pix2text-1.1/scripts/gen_label_studio_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/gen_pure_formula_to_yolov7.py` & `pix2text-1.1/scripts/gen_pure_formula_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/merge_label_studio_anno_pred_json.py` & `pix2text-1.1/scripts/merge_label_studio_anno_pred_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/object_detection3.py` & `pix2text-1.1/scripts/object_detection3.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/screenshot_daemon.py` & `pix2text-1.1/scripts/screenshot_daemon.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/try_latex_correction.py` & `pix2text-1.1/scripts/try_latex_correction.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/try_layout.py` & `pix2text-1.1/scripts/try_layout.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/try_pix2text_mfr.py` & `pix2text-1.1/scripts/try_pix2text_mfr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/scripts/try_service.py` & `pix2text-1.1/scripts/try_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 
 import requests
 
 
 def main():
     url = 'http://0.0.0.0:8503/pix2text'
 
-    image_fp = 'docs/examples/mixed.jpg'
+    image_fp = 'docs/examples/page2.png'
+    # image_fp = 'docs/examples/mixed.jpg'
     # image_fp = 'docs/examples/math-formula-42.png'
     # image_fp = 'docs/examples/english.jpg'
     data = {
-        "image_type": "mixed",
+        "file_type": "page",
         "resized_shape": 768,
         "embed_sep": " $,$ ",
         "isolated_sep": "$$\n, \n$$"
     }
     files = {
         "image": (image_fp, open(image_fp, 'rb'), 'image/jpeg')
     }
 
     r = requests.post(url, data=data, files=files)
 
     outs = r.json()['results']
+    out_md_dir = r.json()['output_dir']
     if isinstance(outs, str):
         only_text = outs
     else:
         only_text = '\n'.join([out['text'] for out in outs])
     print(f'{only_text=}')
+    print(f'{out_md_dir=}')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pix2text-1.0.2.3/scripts/try_texify.py` & `pix2text-1.1/scripts/try_texify.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.0.2.3/setup.py` & `pix2text-1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     "cnocr[ort-cpu]>=2.3.0.1",
     "cnstd>=1.2.3.5",
     "pillow",
     "torch",
     "torchvision",
     "transformers>=4.37.0",
     "optimum[onnxruntime]",
+    "PyMuPDF",
+    "pyspellchecker",
 ]
 extras_require = {
     "multilingual": ["easyocr"],
     "dev": ["pip-tools", "pytest"],
     "serve": ["uvicorn[standard]", "fastapi", "python-multipart", "pydantic"],
 }
 
@@ -55,15 +57,15 @@
     author='breezedeus',
     author_email='breezedeus@163.com',
     license='MIT',
     url='https://github.com/breezedeus/pix2text',
     platforms=["Mac", "Linux", "Windows"],
     packages=find_packages(),
     include_package_data=True,
-    # data_files=[('', ['pix2text/latex_config.yaml',],)],
+    # data_files=[('', ['pix2text/doc_xl_layout/map_info.json',],)],
     entry_points=entry_points,
     install_requires=required,
     extras_require=extras_require,
     zip_safe=False,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
```

### Comparing `pix2text-1.0.2.3/tests/test_pix2text.py` & `pix2text-1.1/tests/test_pix2text.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,175 @@
 # coding: utf-8
 
 import os
 
-from pix2text import Pix2Text, merge_line_texts
+from pix2text import Pix2Text, set_logger
 
+set_logger()
 
-def test_mfd():
-    config = dict(analyzer=dict(model_name='mfd'))
-    p2t = Pix2Text.from_config(config)
 
-    res = p2t.recognize(
-        './docs/examples/zh1.jpg', save_analysis_res='./analysis_res.jpg',
+def test_recognize_pdf():
+    pdf_fn = '1804.07821'
+    img_fp = f'./docs/examples/{pdf_fn}.pdf'
+    text_formula_config = dict(
+        languages=('en', 'ch_sim'),
+        mfd=dict(  # 声明 LayoutAnalyzer 的初始化参数
+            model_type='yolov7',  # 表示使用的是 YoloV7 模型，而不是 YoloV7_Tiny 模型
+            model_fp=os.path.expanduser(
+                '~/.cnstd/1.2/analysis/mfd-yolov7-epoch224-20230613.pt'
+            ),  # 注：修改成你的模型文件所存储的路径
+        ),
+        formula=dict(
+            model_name='mfr-pro',
+            model_backend='onnx',
+            model_dir=os.path.expanduser(
+                '~/.pix2text/1.0/mfr-pro-onnx'
+            ),  # 注：修改成你的模型文件所存储的路径
+        ),
+        text=dict(
+            rec_model_name='doc-densenet_lite_666-gru_large',
+            rec_model_backend='onnx',
+            rec_model_fp=os.path.expanduser(
+                '~/.cnocr/2.3/doc-densenet_lite_666-gru_large/cnocr-v2.3-doc-densenet_lite_666-gru_large-epoch=005-ft-model.onnx'
+                # noqa
+            ),  # 注：修改成你的模型文件所存储的路径
+        ),
+    )
+    total_config = {
+        'layout': {'scores_thresh': 0.45},
+        'text_formula': text_formula_config,
+    }
+    p2t = Pix2Text.from_config(total_configs=total_config)
+    out_md = p2t.recognize_pdf(
+        img_fp,
+        page_numbers=[0, 7, 8],
+        table_as_image=True,
+        save_debug_res=f'./outputs-{pdf_fn}',
     )
-    print(res)
+    out_md.to_markdown('page-output')
+    # print(out_page)
+    # out_page.to_markdown('page-output')
 
 
-def test_example():
+def test_recognize_page():
     # img_fp = './docs/examples/formula.jpg'
-    img_fp = './docs/examples/mixed.jpg'
-    formula_config = {
-        'model_name': 'mfr-pro',
-        'model_backend': 'onnx',
+    img_fp = './docs/examples/page3.png'
+    # img_fp = './docs/examples/mixed.jpg'
+    total_config = {
+        'layout': {'scores_thresh': 0.45},
+        'text_formula': {'formula': {'model_name': 'mfr-pro', 'model_backend': 'onnx'}},
     }
-    p2t = Pix2Text(formula_config=formula_config)
-    print(p2t.recognize(img_fp))
-    # print(p2t.recognize_formula(img_fp))
-    # outs = p2t(img_fp, resized_shape=608, save_analysis_res='./analysis_res.jpg')  # can also use `p2t.recognize(img_fp)`
-    # print(outs)
-    # # To get just the text contents, use:
-    # only_text = merge_line_texts(outs, auto_line_break=True)
-    # print(only_text)
+    p2t = Pix2Text.from_config(total_configs=total_config)
+    out_page = p2t.recognize_page(
+        img_fp,
+        page_id='test_page_1',
+        title_contain_formula=False,
+        text_contain_formula=False,
+        save_debug_res='./outputs',
+    )
+    # print(out_page)
+    out_page.to_markdown('page-output')
+
+
+def test_spell_checker():
+    from spellchecker import SpellChecker
+
+    spell = SpellChecker()
+
+    # 找到拼写错误
+    misspelled = spell.unknown(["speci-fied"])
+
+    for word in misspelled:
+        # Get the one `most likely` answer
+        print('word:', word, ' ->', spell.correction(word))
+
+        # Get a list of `likely` options
+        print('suggestions:', spell.candidates(word))
 
 
 def test_blog_example():
     img_fp = './docs/examples/mixed.jpg'
 
-    p2t = Pix2Text(
-        analyzer_config=dict(  # 声明 LayoutAnalyzer 的初始化参数
-            model_name='mfd',
+    text_formula_config = dict(
+        mfd=dict(  # 声明 LayoutAnalyzer 的初始化参数
             model_type='yolov7',  # 表示使用的是 YoloV7 模型，而不是 YoloV7_Tiny 模型
             model_fp=os.path.expanduser(
                 '~/.cnstd/1.2/analysis/mfd-yolov7-epoch224-20230613.pt'
             ),  # 注：修改成你的模型文件所存储的路径
         ),
-        formula_config=dict(
+        formula=dict(
             model_name='mfr-pro',
             model_backend='onnx',
             model_dir=os.path.expanduser(
                 '~/.pix2text/1.0/mfr-pro-onnx'
             ),  # 注：修改成你的模型文件所存储的路径
         ),
     )
-    outs = p2t.recognize(img_fp, resized_shape=608)  # 也可以使用 `p2t(img_fp)` 获得相同的结果
+    total_config = {
+        'layout': {'scores_thresh': 0.2},
+        'text_formula': text_formula_config,
+    }
+    p2t = Pix2Text.from_config(total_configs=total_config)
+    outs = p2t.recognize_page(
+        img_fp,
+        resized_shape=608,
+        page_id='test_page_2',
+        save_layout_res='./layout_res-mixed.jpg',
+    )  # 也可以使用 `p2t(img_fp)` 获得相同的结果
     print(outs)
-    # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-    only_text = merge_line_texts(outs, auto_line_break=True)
-    print(only_text)
 
 
 def test_blog_pro_example():
     img_fp = './docs/examples/mixed.jpg'
 
-    p2t = Pix2Text(
+    text_formula_config = dict(
         languages=('en', 'ch_sim'),
-        analyzer_config=dict(  # 声明 LayoutAnalyzer 的初始化参数
-            model_name='mfd',
+        mfd=dict(  # 声明 LayoutAnalyzer 的初始化参数
             model_type='yolov7',  # 表示使用的是 YoloV7 模型，而不是 YoloV7_Tiny 模型
             model_fp=os.path.expanduser(
                 '~/.cnstd/1.2/analysis/mfd-yolov7-epoch224-20230613.pt'
             ),  # 注：修改成你的模型文件所存储的路径
         ),
-        formula_config=dict(
+        formula=dict(
             model_name='mfr-pro',
             model_backend='onnx',
             model_dir=os.path.expanduser(
                 '~/.pix2text/1.0/mfr-pro-onnx'
             ),  # 注：修改成你的模型文件所存储的路径
         ),
-        text_config=dict(
+        text=dict(
             rec_model_name='doc-densenet_lite_666-gru_large',
             rec_model_backend='onnx',
             rec_model_fp=os.path.expanduser(
-                '~/.cnocr/2.3/doc-densenet_lite_666-gru_large/cnocr-v2.3-doc-densenet_lite_666-gru_large-epoch=005-ft-model.onnx'  # noqa
+                '~/.cnocr/2.3/doc-densenet_lite_666-gru_large/cnocr-v2.3-doc-densenet_lite_666-gru_large-epoch=005-ft-model.onnx'
+                # noqa
             ),  # 注：修改成你的模型文件所存储的路径
         ),
     )
-    outs = p2t.recognize(img_fp, resized_shape=608)  # 也可以使用 `p2t(img_fp)` 获得相同的结果
+    p2t = Pix2Text.from_config(total_configs={'text_formula': text_formula_config})
+    outs = p2t.recognize_page(
+        img_fp, resized_shape=608, page_id='test_page_3'
+    )  # 也可以使用 `p2t(img_fp)` 获得相同的结果
     print(outs)
-    # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-    only_text = merge_line_texts(outs, auto_line_break=True)
-    print(only_text)
 
 
 def test_example_mixed():
     img_fp = './docs/examples/en1.jpg'
-    p2t = Pix2Text()
-    outs = p2t.recognize(img_fp, resized_shape=608)  # 也可以使用 `p2t(img_fp)` 获得相同的结果
+    p2t = Pix2Text.from_config()
+    outs = p2t.recognize_page(
+        img_fp, resized_shape=608, page_id='test_page_4'
+    )  # 也可以使用 `p2t(img_fp)` 获得相同的结果
     print(outs)
-    # 如果只需要识别出的文字和Latex表示，可以使用下面行的代码合并所有结果
-    only_text = merge_line_texts(outs, auto_line_break=True)
-    print(only_text)
 
 
 def test_example_formula():
-    from pix2text import Pix2Text
-
     img_fp = './docs/examples/math-formula-42.png'
-    p2t = Pix2Text()
+    p2t = Pix2Text.from_config()
     outs = p2t.recognize_formula(img_fp)
     print(outs)
 
 
 def test_example_text():
-    from pix2text import Pix2Text
-
     img_fp = './docs/examples/general.jpg'
     p2t = Pix2Text()
     outs = p2t.recognize_text(img_fp)
     print(outs)
```

### Comparing `pix2text-1.0.2.3/tests/test_sort_boxes.py` & `pix2text-1.1/tests/test_sort_boxes.py`

 * *Files identical despite different names*

