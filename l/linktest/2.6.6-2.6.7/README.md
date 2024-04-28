# Comparing `tmp/linktest-2.6.6.tar.gz` & `tmp/linktest-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.6.6.tar", last modified: Sat Apr 27 08:06:52 2024, max compression
+gzip compressed data, was "linktest-2.6.7.tar", last modified: Sun Apr 28 15:00:18 2024, max compression
```

## Comparing `linktest-2.6.6.tar` & `linktest-2.6.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-27 08:06:52.429140 linktest-2.6.6/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-27 08:06:52.428533 linktest-2.6.6/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-27 08:06:52.418372 linktest-2.6.6/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-27 06:06:42.000000 linktest-2.6.6/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-27 06:08:07.000000 linktest-2.6.6/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16095 2024-04-27 07:53:31.000000 linktest-2.6.6/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34827 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106822 2024-04-27 05:54:38.000000 linktest-2.6.6/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9047 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-27 06:06:49.000000 linktest-2.6.6/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-27 06:08:43.000000 linktest-2.6.6/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13822 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13840 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13810 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-26 09:02:47.000000 linktest-2.6.6/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-27 08:06:52.427252 linktest-2.6.6/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-27 08:06:51.000000 linktest-2.6.6/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-04-27 08:06:51.000000 linktest-2.6.6/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-27 08:06:51.000000 linktest-2.6.6/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-27 08:06:51.000000 linktest-2.6.6/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-27 08:06:51.000000 linktest-2.6.6/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-27 08:06:52.429262 linktest-2.6.6/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-27 08:06:02.000000 linktest-2.6.6/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-28 15:00:18.815640 linktest-2.6.7/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-28 15:00:18.815348 linktest-2.6.7/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-28 15:00:18.812588 linktest-2.6.7/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-28 14:56:51.000000 linktest-2.6.7/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16095 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33114 2024-04-28 14:55:18.000000 linktest-2.6.7/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106863 2024-04-27 08:18:49.000000 linktest-2.6.7/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9047 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-28 14:56:58.000000 linktest-2.6.7/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13822 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13840 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13810 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-27 08:09:28.000000 linktest-2.6.7/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-28 15:00:18.814974 linktest-2.6.7/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-28 15:00:18.000000 linktest-2.6.7/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-04-28 15:00:18.000000 linktest-2.6.7/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-28 15:00:18.000000 linktest-2.6.7/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-28 15:00:18.000000 linktest-2.6.7/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-28 15:00:18.000000 linktest-2.6.7/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-28 15:00:18.815708 linktest-2.6.7/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-28 15:00:13.000000 linktest-2.6.7/setup.py
```

### Comparing `linktest-2.6.6/linktest/appium_utils.py` & `linktest-2.6.7/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/auto_generate_testcase_list.py` & `linktest-2.6.7/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.6.7/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/base_testcase.py` & `linktest-2.6.7/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/clean_data.py` & `linktest-2.6.7/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/conver_xml_into_db.py` & `linktest-2.6.7/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/database_helper.py` & `linktest-2.6.7/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/date_utilities.py` & `linktest-2.6.7/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/doctor.py` & `linktest-2.6.7/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/framework_log.py` & `linktest-2.6.7/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/generate_html_log.py` & `linktest-2.6.7/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/get_adb_devices.py` & `linktest-2.6.7/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/get_ios_devices_list.py` & `linktest-2.6.7/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/get_platform_info.py` & `linktest-2.6.7/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/get_project_info.py` & `linktest-2.6.7/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/html_report.py` & `linktest-2.6.7/linktest/html_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -460,42 +460,25 @@
                                 failed_testcase.log_file_path)
                             report_file_handler.write(
                                 " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> HTML]</font></a>" %
                                 failed_testcase.log_file_path.replace("test.log", "test.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
-                        # try:
-                        #     if isinstance(failed_testcase, UITestCase):
-                        #         report_file_handler.write(
-                        #             "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='click to see the Screenshot' href='%s'> <font color='#DC3912'> - Screenshot</font> </a>" %
-                        #             failed_testcase.screenshot)
-                        #
-                        # except BaseException:
-                        #     print(traceback.format_exc())
-
                     elif failed_testcase.rerun_tag == 1:
                         try:
                             report_file_handler.write(
                                 "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> &nbsp; [TXT </font> </a>" %
                                 failed_testcase.log_file_path)
                             report_file_handler.write(
                                 " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> HTML]</font> </a>" %
                                 failed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
-                        # try:
-                        #     if isinstance(failed_testcase, UITestCase):
-                        #         report_file_handler.write(
-                        #             "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='Click to see the rerun_Screenshot' href='%s'> <font color='#DC3912'> - rerun_Screenshot</font> </a>" %
-                        #             failed_testcase.rerun_screenshot)
-                        # except BaseException:
-                        #     print(traceback.format_exc())
-
                     report_file_handler.write("</td>")
 
                     report_file_handler.write("<td width='200' align='center' >")
                     report_file_handler.write("<font>")
                     if not hasattr(failed_testcase, "execution_time"):
                         failed_testcase.execution_time = ""
                     report_file_handler.write("%s" % failed_testcase.execution_time)
@@ -552,63 +535,51 @@
                     report_file_handler.write(
                         "'><font color='%s'>" % (
                             "#333" if passed_testcase.rerun_tag == 0 else "green"))
                     report_file_handler.write(module_name_display)
 
                     # show re-run got passed in report
                     if passed_testcase.rerun_tag == 1:
-                        report_file_handler.write("<font color='chocolate'> - rerun Passed</font>")
+                        report_file_handler.write("<font color='orange'> - rerun Passed</font>")
 
                     if passed_testcase in error_cases:
                         report_file_handler.write("<font color='orange'> - Miss Attribute</font>")
 
                     report_file_handler.write("</font>")
                     report_file_handler.write("</font></a>")
 
                     try:
-                        report_file_handler.write(
-                            "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp; [TXT </font> </a>" %
-                            passed_testcase.log_file_path)
-                        report_file_handler.write(
-                            " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'> HTML]</font> </a>" %
-                            passed_testcase.log_file_path.replace("test.log", "test.html"))
+                        if passed_testcase.rerun_tag == 0:
+                            report_file_handler.write(
+                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp; [TXT </font> </a>" %
+                                passed_testcase.log_file_path)
+                            report_file_handler.write(
+                                " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'> HTML]</font> </a>" %
+                                passed_testcase.log_file_path.replace("test.log", "test.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
-                    # try:
-                    #     if isinstance(passed_testcase, UITestCase):
-                    #         if getattr(passed_testcase, "screenshot"):
-                    #             report_file_handler.write(
-                    #                 "<a title='Screenshot' href='%s'> <font color='green'> - Screenshot</font> </a>" %
-                    #                 passed_testcase.screenshot)
-                    # except BaseException:
-                    #     traceback.print_exc()
-                    #     print(traceback.format_exc())
-
                     try:
                         if passed_testcase.rerun_tag == 1:
                             report_file_handler.write(
+                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a title='Log' href='%s'> &nbsp;[TXT </a>" %
+                                passed_testcase.log_file_path.replace("test.rerun.log", "test.log"))
+                            report_file_handler.write(
+                                " | <a target='_blank' title='HTML Log' href='%s'> HTML] </a>" %
+                                passed_testcase.log_file_path.replace("test.rerun.log", "test.html"))
+
+                            report_file_handler.write(
                                 "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a title='rerun_Log' href='%s'> &nbsp;[TXT </a>" %
                                 passed_testcase.log_file_path)
                             report_file_handler.write(
-                                " | <a title='rerun_Log' href='%s'> HTML] </a>" %
-                                passed_testcase.log_file_path.replace("test.log", "test.html"))
+                                " | <a target='_blank' title='rerun_Log' href='%s'> HTML] </a>" %
+                                passed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
-                    # try:
-                    #     if getattr(settings, "SAVE_SCREENSHOT_FOR_PASSED_TESTS", False):
-                    #         if isinstance(passed_testcase, UITestCase):
-                    #             if passed_testcase.rerun_tag == 1:
-                    #                 report_file_handler.write(
-                    #                     "<a title='rerun_Screenshot' href='%s'> - rerun_Screenshot </a>" %
-                    #                     passed_testcase.rerun_screenshot)
-                    # except BaseException:
-                    #     print(traceback.format_exc())
-
                     report_file_handler.write("</td>")
 
                     report_file_handler.write("<td width='200' align='center'>")
                     report_file_handler.write("<font color='#333'>")
 
                     if not hasattr(passed_testcase, "execution_time"):
                         passed_testcase.execution_time = ""
```

### Comparing `linktest-2.6.6/linktest/logged_requests.py` & `linktest-2.6.7/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/main.py` & `linktest-2.6.7/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -954,27 +954,27 @@
                     executing_testcase.run_test()
 
             except BaseException:
                 executing_testcase.ExecutionStatusSetByFramework = "failed"
                 traceback.print_exc()
                 traceback_info = traceback.format_exc()
 
-                if issubclass(testcase, ui_testcase.UITestCase):
-
-                    try:
-                        # save the current URL and all the browser's related information when got error.
-                        executing_testcase.logger.error(
-                            "---------------- Error URL & Browser Info Start --------------" +
-                            executing_testcase.browser.current_url() + os.linesep)
-                        executing_testcase.logger.error(testcase.browser.__dict__)
-                        executing_testcase.logger.error(
-                            "---------------- Error URL & Browser Info End --------------" + os.linesep)
-                    except BaseException:
-                        # todo: MacOS executing_testcase.browser.current_url() windows: ?
-                        pass
+                # if issubclass(testcase, ui_testcase.UITestCase):
+                #
+                #     try:
+                #         # save the current URL and all the browser's related information when got error.
+                #         executing_testcase.logger.error(
+                #             "---------------- Error URL & Browser Info Start --------------" +
+                #             executing_testcase.browser.current_url() + os.linesep)
+                #         executing_testcase.logger.error(testcase.browser.__dict__)
+                #         executing_testcase.logger.error(
+                #             "---------------- Error URL & Browser Info End --------------" + os.linesep)
+                #     except BaseException:
+                #         # todo: MacOS executing_testcase.browser.current_url() windows: ?
+                #         pass
 
                 executing_testcase.logger.error(traceback_info)
 
                 if executing_testcase.timeout_flag is True:
                     exception_info = "TestCaseTimeoutException"
                     traceback_info_str = "TestcaseTimeout"
                 else:
```

### Comparing `linktest-2.6.6/linktest/memory_usage.py` & `linktest-2.6.7/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/re_func.py` & `linktest-2.6.7/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/run.py` & `linktest-2.6.7/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/run_testcase_thread.py` & `linktest-2.6.7/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/scp_report_to_specified_path.py` & `linktest-2.6.7/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/selenium_helper.py` & `linktest-2.6.7/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/timeout_thread.py` & `linktest-2.6.7/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/ui_testcase.py` & `linktest-2.6.7/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/update_config.py` & `linktest-2.6.7/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/webdriver_wrapper.py` & `linktest-2.6.7/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/webdriver_wrapper_chrome.py` & `linktest-2.6.7/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/webdriver_wrapper_edge.py` & `linktest-2.6.7/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/webdriver_wrapper_firefox.py` & `linktest-2.6.7/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/webdriver_wrapper_ie.py` & `linktest-2.6.7/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/webdriver_wrapper_safari.py` & `linktest-2.6.7/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest/xml_report.py` & `linktest-2.6.7/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.6/linktest.egg-info/SOURCES.txt` & `linktest-2.6.7/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

