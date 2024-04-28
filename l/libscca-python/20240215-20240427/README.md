# Comparing `tmp/libscca-python-20240215.tar.gz` & `tmp/libscca-python-20240427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libscca-python-20240215.tar", last modified: Thu Feb 15 13:41:40 2024, max compression
+gzip compressed data, was "libscca-python-20240427.tar", last modified: Sun Apr 28 04:54:22 2024, max compression
```

## Comparing `libscca-python-20240215.tar` & `libscca-python-20240427.tar`

### file list

```diff
@@ -1,873 +1,873 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libscca/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2008 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14105 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3475 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_filename_strings.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2446 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2426 2024-02-15 05:32:50.000000 libscca-20240215/libscca/scca_file_metrics_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_file_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2855 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_compressed_blocks_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12716 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_compressed_blocks_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4358 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6517 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2511 2023-12-03 09:33:31.000000 libscca-20240215/libscca/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11436 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_compressed_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3316 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_volume_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9466 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1084 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7614 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21838 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_filename_strings.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12126 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_volume_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4670 2024-02-15 05:32:50.000000 libscca-20240215/libscca/scca_volume_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2371 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_filename_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9158 2024-02-15 05:32:50.000000 libscca-20240215/libscca/scca_file_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21724 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_file_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7987 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_filename_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2444 2024-02-15 11:41:30.000000 libscca-20240215/libscca/libscca_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17948 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_file_metrics.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_file_metrics.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49498 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57955 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2024-02-15 05:32:50.000000 libscca-20240215/libscca/scca_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2820 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2293 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_compressed_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35582 2024-02-15 11:41:21.000000 libscca-20240215/libscca/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1082 2024-02-15 11:41:30.000000 libscca-20240215/libscca/libscca.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1824 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2038 2024-02-15 05:32:50.000000 libscca-20240215/libscca/scca_trace_chain_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-02-15 05:32:50.000000 libscca-20240215/libscca/libscca_notify.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32764 2024-02-15 11:41:21.000000 libscca-20240215/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-02-15 11:41:03.000000 libscca-20240215/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-15 05:32:49.000000 libscca-20240215/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-15 11:41:21.000000 libscca-20240215/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 05:32:49.000000 libscca-20240215/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/pyscca/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2353 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_volumes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13994 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_volume_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4358 2024-02-15 05:33:54.000000 libscca-20240215/pyscca/pyscca_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2574 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_volume_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44433 2024-02-15 05:33:54.000000 libscca-20240215/pyscca/pyscca_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1391 2023-12-03 09:33:31.000000 libscca-20240215/pyscca/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2401 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_filenames.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10568 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_file_metrics_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10162 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_file_metrics.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2701 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_file_metrics_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16043 2024-02-15 05:33:54.000000 libscca-20240215/pyscca/pyscca.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8868 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_libscca.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9197 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_volumes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49562 2024-02-15 11:41:21.000000 libscca-20240215/pyscca/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2085 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_file_metrics.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9196 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_filenames.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-02-15 05:32:50.000000 libscca-20240215/pyscca/pyscca_file_object_io_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-15 11:41:21.000000 libscca-20240215/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2023-12-03 09:33:31.000000 libscca-20240215/m4/libfwnt.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:33:31.000000 libscca-20240215/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:33:31.000000 libscca-20240215/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:33:31.000000 libscca-20240215/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:33:31.000000 libscca-20240215/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:34:07.000000 libscca-20240215/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:34:07.000000 libscca-20240215/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:33:31.000000 libscca-20240215/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:34:07.000000 libscca-20240215/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:34:07.000000 libscca-20240215/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:33:31.000000 libscca-20240215/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:33:31.000000 libscca-20240215/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:33:31.000000 libscca-20240215/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:33:31.000000 libscca-20240215/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:33:31.000000 libscca-20240215/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-15 11:41:15.000000 libscca-20240215/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-15 11:41:15.000000 libscca-20240215/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:33:31.000000 libscca-20240215/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:34:07.000000 libscca-20240215/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-15 11:41:15.000000 libscca-20240215/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:34:07.000000 libscca-20240215/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:33:31.000000 libscca-20240215/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:33:31.000000 libscca-20240215/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:33:31.000000 libscca-20240215/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:34:07.000000 libscca-20240215/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-15 11:41:15.000000 libscca-20240215/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:34:07.000000 libscca-20240215/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:34:07.000000 libscca-20240215/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-15 11:41:15.000000 libscca-20240215/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:34:07.000000 libscca-20240215/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:33:31.000000 libscca-20240215/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:33:31.000000 libscca-20240215/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:33:31.000000 libscca-20240215/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:33:31.000000 libscca-20240215/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:33:31.000000 libscca-20240215/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/include/libscca/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1802 2024-02-15 05:32:49.000000 libscca-20240215/include/libscca/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1800 2024-02-15 11:41:30.000000 libscca-20240215/include/libscca/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5021 2024-02-15 05:32:49.000000 libscca-20240215/include/libscca/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4890 2024-02-15 11:41:30.000000 libscca-20240215/include/libscca/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-02-15 05:32:49.000000 libscca-20240215/include/libscca/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-02-15 05:32:49.000000 libscca-20240215/include/libscca/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-15 05:32:49.000000 libscca-20240215/include/libscca/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-02-15 11:41:30.000000 libscca-20240215/include/libscca/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-02-15 05:32:49.000000 libscca-20240215/include/libscca/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17788 2024-02-15 05:32:49.000000 libscca-20240215/include/libscca.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      459 2024-02-15 05:32:49.000000 libscca-20240215/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17788 2024-02-15 11:41:30.000000 libscca-20240215/include/libscca.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27506 2024-02-15 11:41:21.000000 libscca-20240215/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-15 05:32:49.000000 libscca-20240215/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-15 05:32:49.000000 libscca-20240215/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-15 05:32:49.000000 libscca-20240215/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-15 05:32:49.000000 libscca-20240215/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-15 05:32:49.000000 libscca-20240215/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-15 05:32:49.000000 libscca-20240215/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-15 05:32:49.000000 libscca-20240215/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-15 05:32:49.000000 libscca-20240215/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-15 05:32:49.000000 libscca-20240215/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-02-15 11:41:30.000000 libscca-20240215/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16225 2024-02-15 11:41:20.000000 libscca-20240215/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17185 2024-02-15 11:41:30.000000 libscca-20240215/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-15 05:32:49.000000 libscca-20240215/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-15 05:32:49.000000 libscca-20240215/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-15 05:32:49.000000 libscca-20240215/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24532 2024-02-15 11:41:21.000000 libscca-20240215/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29535 2024-02-15 11:41:21.000000 libscca-20240215/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-15 11:40:55.000000 libscca-20240215/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30008 2024-02-15 11:41:21.000000 libscca-20240215/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-15 11:41:01.000000 libscca-20240215/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2342 2023-12-03 09:33:31.000000 libscca-20240215/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32994 2024-02-15 11:41:21.000000 libscca-20240215/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-15 11:40:50.000000 libscca-20240215/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:34:07.000000 libscca-20240215/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-15 11:41:21.000000 libscca-20240215/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-02-15 05:32:50.000000 libscca-20240215/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2071 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/libscca.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/libscca-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-02-15 11:41:30.000000 libscca-20240215/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/libscca-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-15 05:32:49.000000 libscca-20240215/dpkg/libscca-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-02-15 11:41:30.000000 libscca-20240215/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-15 05:32:49.000000 libscca-20240215/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1987809 2024-02-15 11:41:19.000000 libscca-20240215/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-15 11:41:21.000000 libscca-20240215/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-15 11:41:21.000000 libscca-20240215/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libscca/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9494 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libscca/libscca.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_error/scca_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_compressed_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5916 2024-02-15 05:33:33.000000 libscca-20240215/msvscpp/scca_test_compressed_block/scca_test_compressed_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_tools_path_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5918 2024-02-15 05:33:33.000000 libscca-20240215/msvscpp/scca_test_tools_path_string/scca_test_tools_path_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/pyscca/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7286 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/pyscca/pyscca.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_notify/scca_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-02-15 05:33:33.000000 libscca-20240215/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_filename_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5913 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_filename_string/scca_test_filename_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5895 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_io_handle/scca_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/sccainfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6763 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/sccainfo/sccainfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_file_information/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5916 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_file_information/scca_test_file_information.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_file_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5901 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_file_header/scca_test_file_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_filename_strings/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5916 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_filename_strings/scca_test_filename_strings.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6535 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_file/scca_test_file.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29950 2024-02-15 05:33:33.000000 libscca-20240215/msvscpp/libscca.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5831 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_tools_signal/scca_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libfwnt/libfwnt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23058 2024-02-15 11:41:21.000000 libscca-20240215/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8006 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_volume_information/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5922 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_volume_information/scca_test_volume_information.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6544 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_support/scca_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_file_metrics/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5904 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_file_metrics/scca_test_file_metrics.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5831 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/scca_test_tools_output/scca_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-15 05:33:11.000000 libscca-20240215/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/msvscpp/scca_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6308 2024-02-15 05:33:33.000000 libscca-20240215/msvscpp/scca_test_tools_info_handle/scca_test_tools_info_handle.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-15 05:32:49.000000 libscca-20240215/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30299 2024-02-15 11:41:21.000000 libscca-20240215/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-15 11:40:54.000000 libscca-20240215/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      341 2024-02-15 05:32:49.000000 libscca-20240215/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-15 11:41:21.000000 libscca-20240215/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31983 2024-02-15 11:41:21.000000 libscca-20240215/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-15 11:40:52.000000 libscca-20240215/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-15 05:32:49.000000 libscca-20240215/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-02-15 05:32:49.000000 libscca-20240215/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-15 11:41:21.000000 libscca-20240215/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-15 05:32:49.000000 libscca-20240215/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1197 2024-02-15 05:32:49.000000 libscca-20240215/acinclude.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/sccatools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8827 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccainput.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2521 2024-02-15 05:33:54.000000 libscca-20240215/sccatools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5782 2024-02-15 05:33:54.000000 libscca-20240215/sccatools/sccainfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1284 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/path_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_libscca.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2023-12-03 09:33:31.000000 libscca-20240215/sccatools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24657 2024-02-15 05:33:54.000000 libscca-20240215/sccatools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccainput.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3818 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31352 2024-02-15 11:41:21.000000 libscca-20240215/sccatools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/sccatools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8702 2024-02-15 05:32:50.000000 libscca-20240215/sccatools/path_string.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:34:07.000000 libscca-20240215/config.rpath
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      739 2024-02-15 05:32:49.000000 libscca-20240215/libscca.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32389 2024-02-15 11:41:21.000000 libscca-20240215/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-15 11:41:00.000000 libscca-20240215/libcthreads/libcthreads_queue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2342 2024-02-15 11:41:30.000000 libscca-20240215/libscca.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-15 11:41:21.000000 libscca-20240215/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29577 2024-02-15 11:41:21.000000 libscca-20240215/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-15 11:40:58.000000 libscca-20240215/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2023-12-03 09:33:31.000000 libscca-20240215/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1383 2024-02-15 05:32:50.000000 libscca-20240215/manuals/sccainfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      154 2023-12-03 09:33:31.000000 libscca-20240215/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8009 2024-02-15 05:32:50.000000 libscca-20240215/manuals/libscca.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26498 2024-02-15 11:41:21.000000 libscca-20240215/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53211 2024-02-15 05:33:33.000000 libscca-20240215/tests/scca_test_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3424 2024-02-15 05:33:54.000000 libscca-20240215/tests/pyscca_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8908 2024-02-15 05:33:33.000000 libscca-20240215/tests/scca_test_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5590 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7438 2024-02-15 05:33:54.000000 libscca-20240215/tests/pyscca_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_macros.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-02-15 05:33:54.000000 libscca-20240215/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1367 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23285 2024-02-15 05:33:33.000000 libscca-20240215/tests/scca_test_volume_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28897 2024-02-15 05:33:33.000000 libscca-20240215/tests/scca_test_file_metrics.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8515 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_libscca.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5941 2024-02-15 05:33:33.000000 libscca-20240215/tests/scca_test_file_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6649 2024-02-15 05:33:33.000000 libscca-20240215/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2024-02-15 05:33:33.000000 libscca-20240215/tests/scca_test_compressed_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_libuna.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-15 05:32:50.000000 libscca-20240215/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4073 2024-02-15 05:32:50.000000 libscca-20240215/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13247 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-15 05:32:50.000000 libscca-20240215/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14219 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63670 2024-02-15 11:41:21.000000 libscca-20240215/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6119 2024-02-15 05:33:33.000000 libscca-20240215/tests/scca_test_filename_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9111 2024-02-15 05:33:33.000000 libscca-20240215/tests/scca_test_filename_strings.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3313 2024-02-15 05:32:50.000000 libscca-20240215/tests/test_sccainfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7237 2024-02-15 05:32:50.000000 libscca-20240215/tests/scca_test_tools_path_string.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4183 2024-02-15 05:33:54.000000 libscca-20240215/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:40.000000 libscca-20240215/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-02-15 05:32:50.000000 libscca-20240215/ossfuzz/ossfuzz_libscca.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      889 2023-12-03 09:33:31.000000 libscca-20240215/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-15 05:32:50.000000 libscca-20240215/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2199 2024-02-15 05:32:50.000000 libscca-20240215/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31731 2024-02-15 11:41:21.000000 libscca-20240215/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-15 11:41:15.000000 libscca-20240215/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_locale_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_locale_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33204 2024-02-15 11:41:21.000000 libscca-20240215/libfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-02-15 11:41:07.000000 libscca-20240215/libfwnt/libfwnt_access_control_entry.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30357 2024-02-15 11:41:21.000000 libscca-20240215/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-15 11:40:59.000000 libscca-20240215/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:34:08.000000 libscca-20240215/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:33:31.000000 libscca-20240215/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:34:07.000000 libscca-20240215/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:34:08.000000 libscca-20240215/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:34:08.000000 libscca-20240215/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:34:08.000000 libscca-20240215/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:34:08.000000 libscca-20240215/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:34:08.000000 libscca-20240215/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:33:31.000000 libscca-20240215/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-02-15 11:41:30.000000 libscca-20240215/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:33:31.000000 libscca-20240215/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:34:08.000000 libscca-20240215/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-15 11:41:11.000000 libscca-20240215/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53101 2024-02-15 11:41:21.000000 libscca-20240215/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-15 11:41:11.000000 libscca-20240215/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40626 2024-02-15 11:41:21.000000 libscca-20240215/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1683 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34813 2024-02-15 11:41:21.000000 libscca-20240215/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-15 11:41:06.000000 libscca-20240215/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29411 2024-02-15 11:41:21.000000 libscca-20240215/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-15 11:40:56.000000 libscca-20240215/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:38.000000 libscca-20240215/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-15 11:40:53.000000 libscca-20240215/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28924 2024-02-15 11:41:21.000000 libscca-20240215/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-15 13:41:39.000000 libscca-20240215/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32150 2024-02-15 11:41:21.000000 libscca-20240215/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-15 11:41:04.000000 libscca-20240215/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56827 2024-02-15 11:41:18.000000 libscca-20240215/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3285 2024-02-15 05:32:49.000000 libscca-20240215/libscca.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7649 2024-02-15 05:32:49.000000 libscca-20240215/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-02-15 13:41:40.714164 libscca-20240215/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libscca/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2008 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14105 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3475 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_filename_strings.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2446 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2426 2024-04-27 14:42:01.000000 libscca-20240427/libscca/scca_file_metrics_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_file_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2855 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_compressed_blocks_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12716 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_compressed_blocks_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4358 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6517 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2497 2024-04-28 04:16:07.000000 libscca-20240427/libscca/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11436 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_compressed_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3316 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_volume_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9466 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1084 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7614 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21838 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_filename_strings.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12126 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_volume_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4670 2024-04-27 14:42:01.000000 libscca-20240427/libscca/scca_volume_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2371 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_filename_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9158 2024-04-27 14:42:01.000000 libscca-20240427/libscca/scca_file_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21724 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_file_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7987 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_filename_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2444 2024-04-28 04:35:11.000000 libscca-20240427/libscca/libscca_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17948 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_file_metrics.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_file_metrics.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49498 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57955 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2024-04-27 14:42:01.000000 libscca-20240427/libscca/scca_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2820 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2293 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_compressed_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36256 2024-04-28 04:34:58.000000 libscca-20240427/libscca/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1082 2024-04-28 04:35:11.000000 libscca-20240427/libscca/libscca.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1824 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2038 2024-04-27 14:42:01.000000 libscca-20240427/libscca/scca_trace_chain_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-27 14:42:01.000000 libscca-20240427/libscca/libscca_notify.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33328 2024-04-28 04:34:58.000000 libscca-20240427/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-04-28 04:34:39.000000 libscca-20240427/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-27 14:41:58.000000 libscca-20240427/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-28 04:34:58.000000 libscca-20240427/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 14:41:58.000000 libscca-20240427/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/pyscca/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2353 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_volumes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13994 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_volume_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4358 2024-04-28 04:13:37.000000 libscca-20240427/pyscca/pyscca_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2574 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_volume_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44433 2024-04-28 04:13:37.000000 libscca-20240427/pyscca/pyscca_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2024-04-28 04:16:20.000000 libscca-20240427/pyscca/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2401 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_filenames.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10568 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_file_metrics_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10162 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_file_metrics.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2701 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_file_metrics_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16043 2024-04-28 04:13:37.000000 libscca-20240427/pyscca/pyscca.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8868 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_libscca.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9197 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_volumes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50208 2024-04-28 04:34:58.000000 libscca-20240427/pyscca/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2085 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_file_metrics.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9196 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_filenames.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-04-27 14:42:02.000000 libscca-20240427/pyscca/pyscca_file_object_io_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-28 04:34:58.000000 libscca-20240427/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:18.000000 libscca-20240427/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9040 2024-04-27 14:42:03.000000 libscca-20240427/m4/libfwnt.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-27 14:42:03.000000 libscca-20240427/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-27 14:42:03.000000 libscca-20240427/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:33:31.000000 libscca-20240427/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-27 14:42:03.000000 libscca-20240427/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:34:07.000000 libscca-20240427/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:34:07.000000 libscca-20240427/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-27 14:42:03.000000 libscca-20240427/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:34:07.000000 libscca-20240427/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:34:07.000000 libscca-20240427/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-27 14:42:03.000000 libscca-20240427/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-27 14:42:03.000000 libscca-20240427/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-27 14:42:03.000000 libscca-20240427/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-27 14:42:03.000000 libscca-20240427/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-27 14:42:03.000000 libscca-20240427/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-28 04:34:52.000000 libscca-20240427/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-28 04:34:52.000000 libscca-20240427/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-04-27 14:42:03.000000 libscca-20240427/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:34:07.000000 libscca-20240427/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-28 04:34:51.000000 libscca-20240427/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:34:07.000000 libscca-20240427/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-27 14:42:03.000000 libscca-20240427/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-27 14:42:03.000000 libscca-20240427/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-27 14:42:03.000000 libscca-20240427/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:34:07.000000 libscca-20240427/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-28 04:34:52.000000 libscca-20240427/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:34:07.000000 libscca-20240427/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:34:07.000000 libscca-20240427/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-28 04:34:52.000000 libscca-20240427/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:34:07.000000 libscca-20240427/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-27 14:42:03.000000 libscca-20240427/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-27 14:42:03.000000 libscca-20240427/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:33:31.000000 libscca-20240427/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-04-27 14:42:03.000000 libscca-20240427/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-27 14:42:03.000000 libscca-20240427/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/include/libscca/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1802 2024-04-27 14:42:01.000000 libscca-20240427/include/libscca/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1800 2024-04-28 04:35:11.000000 libscca-20240427/include/libscca/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5021 2024-04-27 14:42:01.000000 libscca-20240427/include/libscca/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4890 2024-04-28 04:35:11.000000 libscca-20240427/include/libscca/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-04-27 14:42:01.000000 libscca-20240427/include/libscca/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-27 14:42:01.000000 libscca-20240427/include/libscca/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-27 14:42:01.000000 libscca-20240427/include/libscca/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-04-28 04:35:11.000000 libscca-20240427/include/libscca/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-04-27 14:42:01.000000 libscca-20240427/include/libscca/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17788 2024-04-27 14:42:01.000000 libscca-20240427/include/libscca.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-04-28 04:14:46.000000 libscca-20240427/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17788 2024-04-28 04:35:11.000000 libscca-20240427/include/libscca.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27486 2024-04-28 04:34:58.000000 libscca-20240427/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-27 14:42:00.000000 libscca-20240427/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-27 14:42:00.000000 libscca-20240427/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-27 14:42:00.000000 libscca-20240427/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-27 14:42:00.000000 libscca-20240427/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-27 14:42:00.000000 libscca-20240427/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-27 14:42:00.000000 libscca-20240427/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-27 14:42:00.000000 libscca-20240427/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-28 04:14:46.000000 libscca-20240427/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-27 14:42:00.000000 libscca-20240427/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-28 04:35:11.000000 libscca-20240427/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16225 2024-04-28 04:34:57.000000 libscca-20240427/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17185 2024-04-28 04:35:11.000000 libscca-20240427/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-27 14:42:00.000000 libscca-20240427/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-27 14:42:00.000000 libscca-20240427/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-27 14:42:00.000000 libscca-20240427/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24539 2024-04-28 04:34:58.000000 libscca-20240427/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29737 2024-04-28 04:34:58.000000 libscca-20240427/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-28 04:34:31.000000 libscca-20240427/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30246 2024-04-28 04:34:58.000000 libscca-20240427/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-04-28 04:34:37.000000 libscca-20240427/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2150 2024-04-28 04:17:15.000000 libscca-20240427/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33589 2024-04-28 04:34:58.000000 libscca-20240427/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-28 04:34:25.000000 libscca-20240427/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:34:07.000000 libscca-20240427/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-28 04:34:58.000000 libscca-20240427/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-27 14:42:03.000000 libscca-20240427/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2071 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/libscca.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/libscca-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-28 04:35:11.000000 libscca-20240427/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/libscca-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-27 14:41:58.000000 libscca-20240427/dpkg/libscca-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-04-28 04:35:11.000000 libscca-20240427/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-27 14:41:58.000000 libscca-20240427/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1990389 2024-04-28 04:34:56.000000 libscca-20240427/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-28 04:34:58.000000 libscca-20240427/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-28 04:34:58.000000 libscca-20240427/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libscca/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9494 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libscca/libscca.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_error/scca_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_compressed_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5916 2024-04-28 04:13:18.000000 libscca-20240427/msvscpp/scca_test_compressed_block/scca_test_compressed_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_tools_path_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5918 2024-04-28 04:13:18.000000 libscca-20240427/msvscpp/scca_test_tools_path_string/scca_test_tools_path_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/pyscca/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7286 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/pyscca/pyscca.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_notify/scca_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1529 2024-04-28 04:15:51.000000 libscca-20240427/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_filename_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5913 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_filename_string/scca_test_filename_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5895 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_io_handle/scca_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/sccainfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6763 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/sccainfo/sccainfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_file_information/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5916 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_file_information/scca_test_file_information.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_file_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5901 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_file_header/scca_test_file_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_filename_strings/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5916 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_filename_strings/scca_test_filename_strings.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6535 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_file/scca_test_file.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29950 2024-04-28 04:13:18.000000 libscca-20240427/msvscpp/libscca.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5831 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_tools_signal/scca_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libfwnt/libfwnt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23058 2024-04-28 04:34:58.000000 libscca-20240427/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8006 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_volume_information/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5922 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_volume_information/scca_test_volume_information.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6544 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_support/scca_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_file_metrics/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5904 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_file_metrics/scca_test_file_metrics.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5831 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/scca_test_tools_output/scca_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-27 14:42:27.000000 libscca-20240427/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/msvscpp/scca_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6308 2024-04-28 04:13:18.000000 libscca-20240427/msvscpp/scca_test_tools_info_handle/scca_test_tools_info_handle.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-27 14:42:00.000000 libscca-20240427/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30570 2024-04-28 04:34:58.000000 libscca-20240427/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-28 04:34:29.000000 libscca-20240427/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      341 2024-04-27 14:41:58.000000 libscca-20240427/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-28 04:34:58.000000 libscca-20240427/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32483 2024-04-28 04:34:58.000000 libscca-20240427/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-28 04:34:26.000000 libscca-20240427/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-27 14:41:58.000000 libscca-20240427/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-04-27 14:41:58.000000 libscca-20240427/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-28 04:34:58.000000 libscca-20240427/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-27 14:41:58.000000 libscca-20240427/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1197 2024-04-27 14:41:58.000000 libscca-20240427/acinclude.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/sccatools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8827 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccainput.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2521 2024-04-28 04:13:37.000000 libscca-20240427/sccatools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5782 2024-04-28 04:13:37.000000 libscca-20240427/sccatools/sccainfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1284 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/path_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_libscca.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1242 2024-04-28 04:15:41.000000 libscca-20240427/sccatools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24657 2024-04-28 04:13:37.000000 libscca-20240427/sccatools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccainput.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3818 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31633 2024-04-28 04:34:58.000000 libscca-20240427/sccatools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/sccatools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8702 2024-04-27 14:42:02.000000 libscca-20240427/sccatools/path_string.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:34:07.000000 libscca-20240427/config.rpath
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      739 2024-04-27 14:41:58.000000 libscca-20240427/libscca.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32922 2024-04-28 04:34:58.000000 libscca-20240427/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-28 04:34:36.000000 libscca-20240427/libcthreads/libcthreads_queue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2342 2024-04-28 04:35:11.000000 libscca-20240427/libscca.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-28 04:34:58.000000 libscca-20240427/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29768 2024-04-28 04:34:58.000000 libscca-20240427/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-28 04:34:33.000000 libscca-20240427/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2023-12-03 09:33:31.000000 libscca-20240427/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1383 2024-04-27 14:42:03.000000 libscca-20240427/manuals/sccainfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      125 2024-04-28 04:15:33.000000 libscca-20240427/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8009 2024-04-27 14:42:03.000000 libscca-20240427/manuals/libscca.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26498 2024-04-28 04:34:58.000000 libscca-20240427/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53211 2024-04-28 04:13:18.000000 libscca-20240427/tests/scca_test_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3424 2024-04-28 04:13:37.000000 libscca-20240427/tests/pyscca_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8908 2024-04-28 04:13:18.000000 libscca-20240427/tests/scca_test_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5590 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7438 2024-04-28 04:13:37.000000 libscca-20240427/tests/pyscca_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_macros.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4046 2024-04-28 04:14:28.000000 libscca-20240427/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1367 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23285 2024-04-28 04:13:18.000000 libscca-20240427/tests/scca_test_volume_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28897 2024-04-28 04:13:18.000000 libscca-20240427/tests/scca_test_file_metrics.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8515 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_libscca.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5941 2024-04-28 04:13:18.000000 libscca-20240427/tests/scca_test_file_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6666 2024-04-28 04:17:32.000000 libscca-20240427/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2024-04-28 04:13:18.000000 libscca-20240427/tests/scca_test_compressed_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_libuna.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-27 14:42:03.000000 libscca-20240427/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4403 2024-04-27 14:42:03.000000 libscca-20240427/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13247 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-27 14:42:03.000000 libscca-20240427/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14219 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64815 2024-04-28 04:34:58.000000 libscca-20240427/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6119 2024-04-28 04:13:18.000000 libscca-20240427/tests/scca_test_filename_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9111 2024-04-28 04:13:18.000000 libscca-20240427/tests/scca_test_filename_strings.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3282 2024-04-27 14:42:03.000000 libscca-20240427/tests/test_sccainfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7237 2024-04-27 14:42:03.000000 libscca-20240427/tests/scca_test_tools_path_string.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4152 2024-04-28 04:14:09.000000 libscca-20240427/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-27 14:42:01.000000 libscca-20240427/ossfuzz/ossfuzz_libscca.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      885 2024-04-28 04:15:11.000000 libscca-20240427/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-27 14:42:01.000000 libscca-20240427/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2199 2024-04-27 14:42:01.000000 libscca-20240427/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31792 2024-04-28 04:34:58.000000 libscca-20240427/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-28 04:34:51.000000 libscca-20240427/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_locale_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2024-04-28 04:34:44.000000 libscca-20240427/libfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-04-28 04:34:44.000000 libscca-20240427/libfwnt/libfwnt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_locale_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33847 2024-04-28 04:34:58.000000 libscca-20240427/libfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-04-28 04:34:43.000000 libscca-20240427/libfwnt/libfwnt_access_control_entry.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30665 2024-04-28 04:34:58.000000 libscca-20240427/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-28 04:34:35.000000 libscca-20240427/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:21.000000 libscca-20240427/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:34:08.000000 libscca-20240427/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:33:31.000000 libscca-20240427/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:34:07.000000 libscca-20240427/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:34:08.000000 libscca-20240427/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:34:08.000000 libscca-20240427/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:34:08.000000 libscca-20240427/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:34:08.000000 libscca-20240427/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:34:08.000000 libscca-20240427/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:33:31.000000 libscca-20240427/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-28 04:35:10.000000 libscca-20240427/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:33:31.000000 libscca-20240427/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:34:08.000000 libscca-20240427/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-28 04:34:47.000000 libscca-20240427/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56249 2024-04-28 04:34:58.000000 libscca-20240427/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-28 04:34:47.000000 libscca-20240427/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-28 04:34:46.000000 libscca-20240427/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40508 2024-04-28 04:34:58.000000 libscca-20240427/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35557 2024-04-28 04:34:58.000000 libscca-20240427/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-28 04:34:42.000000 libscca-20240427/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29606 2024-04-28 04:34:58.000000 libscca-20240427/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-28 04:34:32.000000 libscca-20240427/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:19.000000 libscca-20240427/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-28 04:34:28.000000 libscca-20240427/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29073 2024-04-28 04:34:58.000000 libscca-20240427/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-28 04:54:20.000000 libscca-20240427/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32657 2024-04-28 04:34:58.000000 libscca-20240427/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-28 04:34:40.000000 libscca-20240427/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56827 2024-04-28 04:34:54.000000 libscca-20240427/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3285 2024-04-27 14:41:58.000000 libscca-20240427/libscca.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7649 2024-04-27 14:41:58.000000 libscca-20240427/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-04-28 04:54:22.209318 libscca-20240427/PKG-INFO
```

### Comparing `libscca-20240215/libscca/libscca_support.h` & `libscca-20240427/libscca/libscca_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_file_header.c` & `libscca-20240427/libscca/libscca_file_header.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_filename_strings.h` & `libscca-20240427/libscca/libscca_filename_strings.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libfdata.h` & `libscca-20240427/libscca/libscca_libfdata.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_definitions.h.in` & `libscca-20240427/libscca/libscca_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_error.h` & `libscca-20240427/libscca/libscca_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_debug.h` & `libscca-20240427/libscca/libscca_debug.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/scca_file_metrics_array.h` & `libscca-20240427/libscca/scca_file_metrics_array.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_file_information.h` & `libscca-20240427/libscca/libscca_file_information.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libfdatetime.h` & `libscca-20240427/libscca/libscca_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libfwnt.h` & `libscca-20240427/libscca/libscca_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_compressed_blocks_stream.h` & `libscca-20240427/libscca/libscca_compressed_blocks_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_extern.h` & `libscca-20240427/libscca/libscca_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_compressed_blocks_stream.c` & `libscca-20240427/libscca/libscca_compressed_blocks_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libfvalue.h` & `libscca-20240427/libscca/libscca_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_io_handle.h` & `libscca-20240427/libscca/libscca_io_handle.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_file.h` & `libscca-20240427/libscca/libscca_file.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libbfio.h` & `libscca-20240427/libscca/libscca_libbfio.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/Makefile.am` & `libscca-20240427/libscca/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -80,21 +80,19 @@
 libscca_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libscca_definitions.h.in \
 	libscca.rc \
 	libscca.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libscca_definitions.h \
+	libscca.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libscca_definitions.h
-	-rm -f libscca.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libscca ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libscca_la_SOURCES)
```

### Comparing `libscca-20240215/libscca/libscca_compressed_block.c` & `libscca-20240427/libscca/libscca_compressed_block.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_volume_information.h` & `libscca-20240427/libscca/libscca_volume_information.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_support.c` & `libscca-20240427/libscca/libscca_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca.rc.in` & `libscca-20240427/libscca/libscca.rc.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_debug.c` & `libscca-20240427/libscca/libscca_debug.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_filename_strings.c` & `libscca-20240427/libscca/libscca_filename_strings.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_volume_information.c` & `libscca-20240427/libscca/libscca_volume_information.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/scca_volume_information.h` & `libscca-20240427/libscca/scca_volume_information.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libcnotify.h` & `libscca-20240427/libscca/libscca_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libclocale.h` & `libscca-20240427/libscca/libscca_libclocale.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_filename_string.h` & `libscca-20240427/libscca/libscca_filename_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/scca_file_information.h` & `libscca-20240427/libscca/scca_file_information.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_codepage.h` & `libscca-20240427/libscca/libscca_codepage.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_types.h` & `libscca-20240427/libscca/libscca_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_file_information.c` & `libscca-20240427/libscca/libscca_file_information.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_notify.c` & `libscca-20240427/libscca/libscca_notify.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_error.c` & `libscca-20240427/libscca/libscca_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_filename_string.c` & `libscca-20240427/libscca/libscca_filename_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_definitions.h` & `libscca-20240427/libscca/libscca_definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBSCCA )
 #include <libscca/definitions.h>
 
 /* The definitions in <libscca/definitions.h> are copied here
  * for local use of libscca
  */
 #else
-#define LIBSCCA_VERSION						20240215
+#define LIBSCCA_VERSION						20240427
 
 /* The version string
  */
-#define LIBSCCA_VERSION_STRING					"20240215"
+#define LIBSCCA_VERSION_STRING					"20240427"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBSCCA_ACCESS_FLAGS
```

### Comparing `libscca-20240215/libscca/libscca_file_metrics.c` & `libscca-20240427/libscca/libscca_file_metrics.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libuna.h` & `libscca-20240427/libscca/libscca_libuna.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_file_metrics.h` & `libscca-20240427/libscca/libscca_file_metrics.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libcerror.h` & `libscca-20240427/libscca/libscca_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_io_handle.c` & `libscca-20240427/libscca/libscca_io_handle.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_file.c` & `libscca-20240427/libscca/libscca_file.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/scca_file_header.h` & `libscca-20240427/libscca/scca_file_header.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_file_header.h` & `libscca-20240427/libscca/libscca_file_header.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_compressed_block.h` & `libscca-20240427/libscca/libscca_compressed_block.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/Makefile.in` & `libscca-20240427/libscca/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -550,16 +550,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -633,15 +633,18 @@
 
 libscca_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libscca_definitions.h.in \
 	libscca.rc \
 	libscca.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libscca_definitions.h \
+	libscca.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -886,24 +889,41 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libscca.Plo
+	-rm -f ./$(DEPDIR)/libscca_compressed_block.Plo
+	-rm -f ./$(DEPDIR)/libscca_compressed_blocks_stream.Plo
+	-rm -f ./$(DEPDIR)/libscca_debug.Plo
+	-rm -f ./$(DEPDIR)/libscca_error.Plo
+	-rm -f ./$(DEPDIR)/libscca_file.Plo
+	-rm -f ./$(DEPDIR)/libscca_file_header.Plo
+	-rm -f ./$(DEPDIR)/libscca_file_information.Plo
+	-rm -f ./$(DEPDIR)/libscca_file_metrics.Plo
+	-rm -f ./$(DEPDIR)/libscca_filename_string.Plo
+	-rm -f ./$(DEPDIR)/libscca_filename_strings.Plo
+	-rm -f ./$(DEPDIR)/libscca_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libscca_notify.Plo
+	-rm -f ./$(DEPDIR)/libscca_support.Plo
+	-rm -f ./$(DEPDIR)/libscca_volume_information.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1001,19 +1021,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libscca_definitions.h
-	-rm -f libscca.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libscca ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libscca_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libscca/libscca.rc` & `libscca-20240427/libscca/libscca.rc`

 * *Files 20% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Prefetch File (PF) format\0"
-      VALUE "FileVersion",		"20240215" "\0"
+      VALUE "FileVersion",		"20240427" "\0"
       VALUE "InternalName",		"libscca.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libscca.dll\0"
       VALUE "ProductName",		"libscca\0"
-      VALUE "ProductVersion",		"20240215" "\0"
+      VALUE "ProductVersion",		"20240427" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libscca/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libscca-20240215/libscca/libscca_libcdata.h` & `libscca-20240427/libscca/libscca_libcdata.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca.c` & `libscca-20240427/libscca/libscca.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_libfcache.h` & `libscca-20240427/libscca/libscca_libfcache.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_unused.h` & `libscca-20240427/libscca/libscca_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/scca_trace_chain_array.h` & `libscca-20240427/libscca/scca_trace_chain_array.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca/libscca_notify.h` & `libscca-20240427/libscca/libscca_notify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_error.h` & `libscca-20240427/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_area.c` & `libscca-20240427/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_stream.h` & `libscca-20240427/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_cache.h` & `libscca-20240427/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_range_list.c` & `libscca-20240427/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_mapped_range.c` & `libscca-20240427/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_libcerror.h` & `libscca-20240427/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_definitions.h` & `libscca-20240427/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libscca-20240215/libfdata/libfdata_list.c` & `libscca-20240427/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_libcdata.h` & `libscca-20240427/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_list.h` & `libscca-20240427/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_list_element.h` & `libscca-20240427/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/Makefile.am` & `libscca-20240427/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libscca-20240215/libfdata/libfdata_libcnotify.h` & `libscca-20240427/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_extern.h` & `libscca-20240427/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_notify.c` & `libscca-20240427/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_cache.c` & `libscca-20240427/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_stream.c` & `libscca-20240427/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_unused.h` & `libscca-20240427/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_range.h` & `libscca-20240427/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_area.h` & `libscca-20240427/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_error.c` & `libscca-20240427/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_support.h` & `libscca-20240427/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_range.c` & `libscca-20240427/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_mapped_range.h` & `libscca-20240427/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_support.c` & `libscca-20240427/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_list_element.c` & `libscca-20240427/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_segments_array.c` & `libscca-20240427/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_types.h` & `libscca-20240427/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_notify.h` & `libscca-20240427/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_range_list.h` & `libscca-20240427/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_segments_array.h` & `libscca-20240427/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/Makefile.in` & `libscca-20240427/libfdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -534,16 +534,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -567,15 +567,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -787,24 +788,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -900,17 +916,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libfdata/libfdata_vector.c` & `libscca-20240427/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_libfcache.h` & `libscca-20240427/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdata/libfdata_vector.h` & `libscca-20240427/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/COPYING` & `libscca-20240427/COPYING`

 * *Files identical despite different names*

### Comparing `libscca-20240215/install-sh` & `libscca-20240427/install-sh`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_volumes.h` & `libscca-20240427/pyscca/pyscca_volumes.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_volume_information.c` & `libscca-20240427/pyscca/pyscca_volume_information.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_file.h` & `libscca-20240427/pyscca/pyscca_file.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_libclocale.h` & `libscca-20240427/pyscca/pyscca_libclocale.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_volume_information.h` & `libscca-20240427/pyscca/pyscca_volume_information.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_file.c` & `libscca-20240427/pyscca/pyscca_file.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_python.h` & `libscca-20240427/pyscca/pyscca_python.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/Makefile.am` & `libscca-20240427/pyscca/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -47,13 +47,11 @@
 	@LIBBFIO_LIBADD@
 
 pyscca_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyscca_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libscca-20240215/pyscca/pyscca_libuna.h` & `libscca-20240427/pyscca/pyscca_libuna.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_datetime.c` & `libscca-20240427/pyscca/pyscca_datetime.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_string.h` & `libscca-20240427/pyscca/pyscca_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_integer.h` & `libscca-20240427/pyscca/pyscca_integer.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_integer.c` & `libscca-20240427/pyscca/pyscca_integer.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_error.c` & `libscca-20240427/pyscca/pyscca_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_error.h` & `libscca-20240427/pyscca/pyscca_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_filenames.h` & `libscca-20240427/pyscca/pyscca_filenames.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_file_metrics_entries.c` & `libscca-20240427/pyscca/pyscca_file_metrics_entries.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_unused.h` & `libscca-20240427/pyscca/pyscca_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_file_metrics.c` & `libscca-20240427/pyscca/pyscca_file_metrics.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_libbfio.h` & `libscca-20240427/pyscca/pyscca_libbfio.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_file_metrics_entries.h` & `libscca-20240427/pyscca/pyscca_file_metrics_entries.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca.c` & `libscca-20240427/pyscca/pyscca.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_string.c` & `libscca-20240427/pyscca/pyscca_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_libscca.h` & `libscca-20240427/pyscca/pyscca_libscca.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_datetime.h` & `libscca-20240427/pyscca/pyscca_datetime.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_file_object_io_handle.h` & `libscca-20240427/pyscca/pyscca_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_libcerror.h` & `libscca-20240427/pyscca/pyscca_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_volumes.c` & `libscca-20240427/pyscca/pyscca_volumes.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/Makefile.in` & `libscca-20240427/pyscca/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -565,16 +565,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -612,15 +612,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyscca_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyscca_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -942,24 +943,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyscca_la-pyscca.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_error.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_file.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_file_metrics.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_file_metrics_entries.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_filenames.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_integer.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_string.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_volume_information.Plo
+	-rm -f ./$(DEPDIR)/pyscca_la-pyscca_volumes.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1055,13 +1070,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/pyscca/pyscca_file_metrics.h` & `libscca-20240427/pyscca/pyscca_file_metrics.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca.h` & `libscca-20240427/pyscca/pyscca.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_filenames.c` & `libscca-20240427/pyscca/pyscca_filenames.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/pyscca/pyscca_file_object_io_handle.c` & `libscca-20240427/pyscca/pyscca_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/depcomp` & `libscca-20240427/depcomp`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/libfwnt.m4` & `libscca-20240427/m4/libfwnt.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfwnt required headers and functions
 dnl
-dnl Version: 20191217
+dnl Version: 20240413
 
 dnl Function to detect if libfwnt is available
 dnl ac_libfwnt_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWNT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno],
     [ac_cv_libfwnt=no],
     [ac_cv_libfwnt=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfwnt which returns "yes" and --with-libfwnt= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect],
+      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfwnt"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfwnt],
           [1])
@@ -214,16 +216,17 @@
           fwnt,
           libfwnt_lzxpress_huffman_decompress,
           [ac_cv_libfwnt_dummy=yes],
           [ac_cv_libfwnt=no])
 
         ac_cv_libfwnt_LIBADD="-lfwnt"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes],
+      [test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfwnt in directory: $ac_cv_with_libfwnt],
         [1])
       ])
     ])
 
   AS_IF(
@@ -245,15 +248,15 @@
     ])
   ])
 
 dnl Function to detect if libfwnt dependencies are available
 AC_DEFUN([AX_LIBFWNT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
   ])
 
 dnl Function to detect how to enable libfwnt
 AC_DEFUN([AX_LIBFWNT_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/libcfile.m4` & `libscca-20240427/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/libfdatetime.m4` & `libscca-20240427/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/tests.m4` & `libscca-20240427/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/libcpath.m4` & `libscca-20240427/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/lib-prefix.m4` & `libscca-20240427/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/progtest.m4` & `libscca-20240427/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/libuna.m4` & `libscca-20240427/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/gettext.m4` & `libscca-20240427/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/lib-ld.m4` & `libscca-20240427/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/libclocale.m4` & `libscca-20240427/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/libcdata.m4` & `libscca-20240427/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/libcsplit.m4` & `libscca-20240427/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/common.m4` & `libscca-20240427/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libscca-20240215/m4/libcthreads.m4` & `libscca-20240427/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libscca-20240215/m4/ltversion.m4` & `libscca-20240427/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/ltsugar.m4` & `libscca-20240427/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/libfdata.m4` & `libscca-20240427/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/host-cpu-c-abi.m4` & `libscca-20240427/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/libtool.m4` & `libscca-20240427/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/po.m4` & `libscca-20240427/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/libcerror.m4` & `libscca-20240427/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/libcnotify.m4` & `libscca-20240427/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/libbfio.m4` & `libscca-20240427/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/intlmacosx.m4` & `libscca-20240427/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/lt~obsolete.m4` & `libscca-20240427/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/lib-link.m4` & `libscca-20240427/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/iconv.m4` & `libscca-20240427/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/ltoptions.m4` & `libscca-20240427/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/nls.m4` & `libscca-20240427/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/python.m4` & `libscca-20240427/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libscca-20240215/m4/libfvalue.m4` & `libscca-20240427/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/types.m4` & `libscca-20240427/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/m4/libfcache.m4` & `libscca-20240427/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libscca-20240215/m4/pthread.m4` & `libscca-20240427/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libscca-20240215/include/libscca/definitions.h.in` & `libscca-20240427/include/libscca/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca/definitions.h` & `libscca-20240427/include/libscca/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBSCCA_DEFINITIONS_H )
 #define _LIBSCCA_DEFINITIONS_H
 
 #include <libscca/types.h>
 
-#define LIBSCCA_VERSION				20240215
+#define LIBSCCA_VERSION				20240427
 
 /* The version string
  */
-#define LIBSCCA_VERSION_STRING			"20240215"
+#define LIBSCCA_VERSION_STRING			"20240427"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBSCCA_ACCESS_FLAGS
```

### Comparing `libscca-20240215/include/libscca/types.h.in` & `libscca-20240427/include/libscca/types.h.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca/types.h` & `libscca-20240427/include/libscca/types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca/features.h.in` & `libscca-20240427/include/libscca/features.h.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca/error.h` & `libscca-20240427/include/libscca/error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca/extern.h` & `libscca-20240427/include/libscca/extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca/features.h` & `libscca-20240427/include/libscca/features.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca/codepage.h` & `libscca-20240427/include/libscca/codepage.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca.h.in` & `libscca-20240427/include/libscca.h.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/libscca.h` & `libscca-20240427/include/libscca.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/include/Makefile.in` & `libscca-20240427/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -516,15 +516,20 @@
 
 EXTRA_DIST = \
 	libscca.h.in \
 	libscca/definitions.h.in \
 	libscca/features.h.in \
 	libscca/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libscca.h \
+	libscca/definitions.h \
+	libscca/features.h \
+	libscca/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -721,23 +726,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -819,17 +826,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libscca.h
-	-rm -f libscca/definitions.h
-	-rm -f libscca/features.h
-	-rm -f libscca/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/common/config_borlandc.h` & `libscca-20240427/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/file_stream.h` & `libscca-20240427/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/memory.h` & `libscca-20240427/common/memory.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/byte_stream.h` & `libscca-20240427/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/common.h` & `libscca-20240427/common/common.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/config_winapi.h` & `libscca-20240427/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/system_string.h` & `libscca-20240427/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/types.h.in` & `libscca-20240427/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/types.h` & `libscca-20240427/common/types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/config.h.in` & `libscca-20240427/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/config.h` & `libscca-20240427/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -532,24 +532,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libscca"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libscca 20240215"
+#define PACKAGE_STRING "libscca 20240427"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libscca"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240215"
+#define PACKAGE_VERSION "20240427"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -570,15 +570,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240215"
+#define VERSION "20240427"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libscca-20240215/common/wide_string.h` & `libscca-20240427/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/narrow_string.h` & `libscca-20240427/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/config_msc.h` & `libscca-20240427/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/common/Makefile.in` & `libscca-20240427/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -469,15 +469,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -485,15 +487,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -661,23 +666,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -757,15 +764,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/libclocale/libclocale_wide_string.c` & `libscca-20240427/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/libclocale_support.h` & `libscca-20240427/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/Makefile.am` & `libscca-20240427/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libscca-20240215/libclocale/libclocale_definitions.h` & `libscca-20240427/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libscca-20240215/libclocale/libclocale_unused.h` & `libscca-20240427/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/libclocale_libcerror.h` & `libscca-20240427/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/libclocale_locale.h` & `libscca-20240427/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/libclocale_support.c` & `libscca-20240427/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/libclocale_codepage.c` & `libscca-20240427/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/libclocale_locale.c` & `libscca-20240427/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/Makefile.in` & `libscca-20240427/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -515,30 +515,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -741,24 +742,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -845,17 +852,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libclocale/libclocale_extern.h` & `libscca-20240427/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/libclocale_wide_string.h` & `libscca-20240427/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libclocale/libclocale_codepage.h` & `libscca-20240427/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_libcdata.h` & `libscca-20240427/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_types.h` & `libscca-20240427/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_cache_value.c` & `libscca-20240427/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_unused.h` & `libscca-20240427/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/Makefile.am` & `libscca-20240427/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libscca-20240215/libfcache/libfcache_support.h` & `libscca-20240427/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_error.h` & `libscca-20240427/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_support.c` & `libscca-20240427/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_cache.h` & `libscca-20240427/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_error.c` & `libscca-20240427/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_libcerror.h` & `libscca-20240427/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_date_time.c` & `libscca-20240427/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_extern.h` & `libscca-20240427/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_cache_value.h` & `libscca-20240427/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/Makefile.in` & `libscca-20240427/libfcache/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -517,16 +517,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -538,15 +538,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -750,24 +751,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -855,17 +863,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libfcache/libfcache_date_time.h` & `libscca-20240427/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfcache/libfcache_definitions.h` & `libscca-20240427/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libscca-20240215/libfcache/libfcache_cache.c` & `libscca-20240427/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/Makefile.am` & `libscca-20240427/Makefile.am`

 * *Files 11% similar despite different names*

```diff
@@ -60,16 +60,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libscca.pc \
+	libscca.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libscca.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -93,19 +100,7 @@
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libscca && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libscca.pc
-	-rm -f libscca.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libscca-20240215/libbfio/libbfio_file_range.h` & `libscca-20240427/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file_range_io_handle.c` & `libscca-20240427/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_support.c` & `libscca-20240427/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_libcpath.h` & `libscca-20240427/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_error.h` & `libscca-20240427/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_libclocale.h` & `libscca-20240427/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_error.c` & `libscca-20240427/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_libuna.h` & `libscca-20240427/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file_io_handle.h` & `libscca-20240427/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file_pool.h` & `libscca-20240427/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file_range.c` & `libscca-20240427/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_types.h` & `libscca-20240427/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_unused.h` & `libscca-20240427/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_libcdata.h` & `libscca-20240427/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file.h` & `libscca-20240427/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/Makefile.am` & `libscca-20240427/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libscca-20240215/libbfio/libbfio_libcfile.h` & `libscca-20240427/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_definitions.h` & `libscca-20240427/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libscca-20240215/libbfio/libbfio_codepage.h` & `libscca-20240427/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file_io_handle.c` & `libscca-20240427/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_support.h` & `libscca-20240427/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_memory_range.h` & `libscca-20240427/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file_pool.c` & `libscca-20240427/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file_range_io_handle.h` & `libscca-20240427/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_libcthreads.h` & `libscca-20240427/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_system_string.h` & `libscca-20240427/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_memory_range_io_handle.c` & `libscca-20240427/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_handle.c` & `libscca-20240427/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_file.c` & `libscca-20240427/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_handle.h` & `libscca-20240427/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_memory_range.c` & `libscca-20240427/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_pool.c` & `libscca-20240427/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_libcerror.h` & `libscca-20240427/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/Makefile.in` & `libscca-20240427/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -535,16 +535,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -575,15 +575,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -794,24 +795,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -880,14 +895,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -898,23 +915,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/libbfio/libbfio_system_string.c` & `libscca-20240427/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_memory_range_io_handle.h` & `libscca-20240427/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_extern.h` & `libscca-20240427/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/libbfio/libbfio_pool.h` & `libscca-20240427/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libscca-20240215/config.guess` & `libscca-20240427/config.guess`

 * *Files identical despite different names*

### Comparing `libscca-20240215/dpkg/copyright` & `libscca-20240427/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libscca-20240215/dpkg/control` & `libscca-20240427/dpkg/control`

 * *Files identical despite different names*

### Comparing `libscca-20240215/dpkg/rules` & `libscca-20240427/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libscca-20240215/COPYING.LESSER` & `libscca-20240427/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libscca-20240215/configure` & `libscca-20240427/configure`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libscca 20240215.
+# Generated by GNU Autoconf 2.71 for libscca 20240427.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libscca'
 PACKAGE_TARNAME='libscca'
-PACKAGE_VERSION='20240215'
-PACKAGE_STRING='libscca 20240215'
+PACKAGE_VERSION='20240427'
+PACKAGE_STRING='libscca 20240427'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libscca.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1653,15 +1653,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libscca 20240215 to adapt to many kinds of systems.
+\`configure' configures libscca 20240427 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1724,15 +1724,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libscca 20240215:";;
+     short | recursive ) echo "Configuration of libscca 20240427:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1976,15 +1976,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libscca configure 20240215
+libscca configure 20240427
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2697,15 +2697,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libscca $as_me 20240215, which was
+It was created by libscca $as_me 20240427, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4186,15 +4186,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libscca'
- VERSION='20240215'
+ VERSION='20240427'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23781,15 +23781,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24280,15 +24280,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24430,15 +24431,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24532,15 +24533,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26172,15 +26173,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26234,47 +26235,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26308,15 +26314,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26350,15 +26356,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26393,15 +26399,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26435,15 +26441,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26477,15 +26483,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26519,15 +26525,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26561,15 +26567,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26604,15 +26610,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26646,15 +26652,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26688,15 +26694,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26730,15 +26736,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26772,15 +26778,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26815,15 +26821,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26857,15 +26863,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26899,15 +26905,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26941,15 +26947,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26983,15 +26989,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27026,67 +27032,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27174,15 +27189,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30953,15 +30968,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30986,15 +31002,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31064,15 +31080,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31619,15 +31635,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31783,15 +31800,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31861,15 +31878,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32319,15 +32336,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32382,15 +32400,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32460,15 +32478,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33183,15 +33201,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33216,15 +33235,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33294,15 +33313,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40504,15 +40523,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40537,15 +40557,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40615,15 +40635,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41804,15 +41824,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42126,15 +42147,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42204,15 +42225,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43009,15 +43030,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43207,15 +43229,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43285,15 +43307,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45403,15 +45425,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45436,15 +45459,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45514,15 +45537,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46434,15 +46457,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46535,15 +46559,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46613,15 +46637,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49901,15 +49925,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49934,15 +49959,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50012,15 +50037,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -53456,15 +53481,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -53489,15 +53515,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53567,15 +53593,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -57881,15 +57907,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -57914,15 +57941,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -57992,15 +58019,15 @@
 printf "%s\n" "$ac_cv_with_libfwnt" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno
 then :
   ac_cv_libfwnt=no
 else $as_nop
   ac_cv_libfwnt=check
-        if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect
+                if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   if test -d "$ac_cv_with_libfwnt"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -59382,15 +59409,16 @@
 fi
 
 
         ac_cv_libfwnt_LIBADD="-lfwnt"
 fi
 
 fi
-    if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes
+
+    if test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfwnt in directory: $ac_cv_with_libfwnt
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -59415,15 +59443,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwnt" != xyes
 then :
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWNT 1" >>confdefs.h
@@ -59734,16 +59762,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -60760,15 +60792,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libscca $as_me 20240215, which was
+This file was extended by libscca $as_me 20240427, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -60828,15 +60860,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libscca config.status 20240215
+libscca config.status 20240427
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libscca-20240215/compile` & `libscca-20240427/compile`

 * *Files identical despite different names*

### Comparing `libscca-20240215/missing` & `libscca-20240427/missing`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libscca/libscca.vcproj` & `libscca-20240427/msvscpp/libscca/libscca.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libfdata/libfdata.vcproj` & `libscca-20240427/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_error/scca_test_error.vcproj` & `libscca-20240427/msvscpp/scca_test_error/scca_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_compressed_block/scca_test_compressed_block.vcproj` & `libscca-20240427/msvscpp/scca_test_compressed_block/scca_test_compressed_block.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_tools_path_string/scca_test_tools_path_string.vcproj` & `libscca-20240427/msvscpp/scca_test_tools_path_string/scca_test_tools_path_string.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/pyscca/pyscca.vcproj` & `libscca-20240427/msvscpp/pyscca/pyscca.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_notify/scca_test_notify.vcproj` & `libscca-20240427/msvscpp/scca_test_notify/scca_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libclocale/libclocale.vcproj` & `libscca-20240427/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libfcache/libfcache.vcproj` & `libscca-20240427/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/Makefile.am` & `libscca-20240427/msvscpp/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -34,13 +34,11 @@
 	scca_test_volume_information/scca_test_volume_information.vcproj \
 	sccainfo/sccainfo.vcproj \
 	libscca.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libscca-20240215/msvscpp/libbfio/libbfio.vcproj` & `libscca-20240427/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libcfile/libcfile.vcproj` & `libscca-20240427/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_filename_string/scca_test_filename_string.vcproj` & `libscca-20240427/msvscpp/scca_test_filename_string/scca_test_filename_string.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libcdata/libcdata.vcproj` & `libscca-20240427/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_io_handle/scca_test_io_handle.vcproj` & `libscca-20240427/msvscpp/scca_test_io_handle/scca_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/sccainfo/sccainfo.vcproj` & `libscca-20240427/msvscpp/sccainfo/sccainfo.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_file_information/scca_test_file_information.vcproj` & `libscca-20240427/msvscpp/scca_test_file_information/scca_test_file_information.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libcthreads/libcthreads.vcproj` & `libscca-20240427/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_file_header/scca_test_file_header.vcproj` & `libscca-20240427/msvscpp/scca_test_file_header/scca_test_file_header.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_filename_strings/scca_test_filename_strings.vcproj` & `libscca-20240427/msvscpp/scca_test_filename_strings/scca_test_filename_strings.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_file/scca_test_file.vcproj` & `libscca-20240427/msvscpp/scca_test_file/scca_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libscca.sln` & `libscca-20240427/msvscpp/libscca.sln`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_tools_signal/scca_test_tools_signal.vcproj` & `libscca-20240427/msvscpp/scca_test_tools_signal/scca_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libcpath/libcpath.vcproj` & `libscca-20240427/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libfwnt/libfwnt.vcproj` & `libscca-20240427/msvscpp/libfwnt/libfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libcsplit/libcsplit.vcproj` & `libscca-20240427/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libuna/libuna.vcproj` & `libscca-20240427/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/Makefile.in` & `libscca-20240427/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -491,15 +491,16 @@
 	scca_test_volume_information/scca_test_volume_information.vcproj \
 	sccainfo/sccainfo.vcproj \
 	libscca.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -603,23 +604,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -698,13 +701,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/msvscpp/libfvalue/libfvalue.vcproj` & `libscca-20240427/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_volume_information/scca_test_volume_information.vcproj` & `libscca-20240427/msvscpp/scca_test_volume_information/scca_test_volume_information.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_support/scca_test_support.vcproj` & `libscca-20240427/msvscpp/scca_test_support/scca_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_file_metrics/scca_test_file_metrics.vcproj` & `libscca-20240427/msvscpp/scca_test_file_metrics/scca_test_file_metrics.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libcnotify/libcnotify.vcproj` & `libscca-20240427/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libcerror/libcerror.vcproj` & `libscca-20240427/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_tools_output/scca_test_tools_output.vcproj` & `libscca-20240427/msvscpp/scca_test_tools_output/scca_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/libfdatetime/libfdatetime.vcproj` & `libscca-20240427/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/msvscpp/scca_test_tools_info_handle/scca_test_tools_info_handle.vcproj` & `libscca-20240427/msvscpp/scca_test_tools_info_handle/scca_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_extern.h` & `libscca-20240427/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_support.h` & `libscca-20240427/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_unused.h` & `libscca-20240427/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_notify.h` & `libscca-20240427/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_support.c` & `libscca-20240427/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_types.h` & `libscca-20240427/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/Makefile.am` & `libscca-20240427/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libscca-20240215/libcfile/libcfile_notify.c` & `libscca-20240427/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_system_string.h` & `libscca-20240427/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_file.h` & `libscca-20240427/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_libcnotify.h` & `libscca-20240427/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_system_string.c` & `libscca-20240427/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_error.h` & `libscca-20240427/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_libcerror.h` & `libscca-20240427/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_file.c` & `libscca-20240427/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_libclocale.h` & `libscca-20240427/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_winapi.h` & `libscca-20240427/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/Makefile.in` & `libscca-20240427/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -517,16 +517,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -541,15 +541,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -754,24 +755,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -860,17 +869,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libcfile/libcfile_error.c` & `libscca-20240427/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_libuna.h` & `libscca-20240427/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_winapi.c` & `libscca-20240427/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcfile/libcfile_definitions.h` & `libscca-20240427/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libscca-20240215/INSTALL` & `libscca-20240427/INSTALL`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_list_element.h` & `libscca-20240427/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_array.h` & `libscca-20240427/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_definitions.h` & `libscca-20240427/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libscca-20240215/libcdata/libcdata_libcerror.h` & `libscca-20240427/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_unused.h` & `libscca-20240427/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_btree.h` & `libscca-20240427/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_btree.c` & `libscca-20240427/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_support.c` & `libscca-20240427/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_list.c` & `libscca-20240427/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_extern.h` & `libscca-20240427/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_list.h` & `libscca-20240427/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_btree_values_list.h` & `libscca-20240427/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/Makefile.am` & `libscca-20240427/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libscca-20240215/libcdata/libcdata_btree_node.h` & `libscca-20240427/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_range_list_value.h` & `libscca-20240427/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_range_list.h` & `libscca-20240427/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_range_list.c` & `libscca-20240427/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_array.c` & `libscca-20240427/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_list_element.c` & `libscca-20240427/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_libcthreads.h` & `libscca-20240427/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_tree_node.h` & `libscca-20240427/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_error.h` & `libscca-20240427/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_types.h` & `libscca-20240427/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_btree_node.c` & `libscca-20240427/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_tree_node.c` & `libscca-20240427/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_support.h` & `libscca-20240427/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/Makefile.in` & `libscca-20240427/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -531,16 +531,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -557,15 +557,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -775,24 +776,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -886,17 +900,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libcdata/libcdata_range_list_value.c` & `libscca-20240427/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_btree_values_list.c` & `libscca-20240427/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcdata/libcdata_error.c` & `libscca-20240427/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/config.sub` & `libscca-20240427/config.sub`

 * *Files identical despite different names*

### Comparing `libscca-20240215/setup.py` & `libscca-20240427/setup.py`

 * *Files identical despite different names*

### Comparing `libscca-20240215/acinclude.m4` & `libscca-20240427/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccainput.c` & `libscca-20240427/sccatools/sccainput.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_libclocale.h` & `libscca-20240427/sccatools/sccatools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_libfdatetime.h` & `libscca-20240427/sccatools/sccatools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_signal.h` & `libscca-20240427/sccatools/sccatools_signal.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/info_handle.h` & `libscca-20240427/sccatools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_getopt.h` & `libscca-20240427/sccatools/sccatools_getopt.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccainfo.c` & `libscca-20240427/sccatools/sccainfo.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/path_string.h` & `libscca-20240427/sccatools/path_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_libcerror.h` & `libscca-20240427/sccatools/sccatools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_libscca.h` & `libscca-20240427/sccatools/sccatools_libscca.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/Makefile.am` & `libscca-20240427/sccatools/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -41,17 +41,15 @@
 	@LIBFDATETIME_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libscca/libscca.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on sccainfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(sccainfo_SOURCES)
```

### Comparing `libscca-20240215/sccatools/info_handle.c` & `libscca-20240427/sccatools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccainput.h` & `libscca-20240427/sccatools/sccainput.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_output.c` & `libscca-20240427/sccatools/sccatools_output.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_unused.h` & `libscca-20240427/sccatools/sccatools_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_i18n.h` & `libscca-20240427/sccatools/sccatools_i18n.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_libbfio.h` & `libscca-20240427/sccatools/sccatools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_getopt.c` & `libscca-20240427/sccatools/sccatools_getopt.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_libcnotify.h` & `libscca-20240427/sccatools/sccatools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_libuna.h` & `libscca-20240427/sccatools/sccatools_libuna.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/Makefile.in` & `libscca-20240427/sccatools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -509,16 +509,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -551,15 +551,16 @@
 	@LIBFDATETIME_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libscca/libscca.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -807,23 +808,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/path_string.Po
+	-rm -f ./$(DEPDIR)/sccainfo.Po
+	-rm -f ./$(DEPDIR)/sccainput.Po
+	-rm -f ./$(DEPDIR)/sccatools_getopt.Po
+	-rm -f ./$(DEPDIR)/sccatools_output.Po
+	-rm -f ./$(DEPDIR)/sccatools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -913,17 +923,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on sccainfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(sccainfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/sccatools/sccatools_output.h` & `libscca-20240427/sccatools/sccatools_output.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/sccatools_signal.c` & `libscca-20240427/sccatools/sccatools_signal.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/sccatools/path_string.c` & `libscca-20240427/sccatools/path_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/config.rpath` & `libscca-20240427/config.rpath`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca.pc.in` & `libscca-20240427/libscca.pc.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_thread.h` & `libscca-20240427/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_read_write_lock.h` & `libscca-20240427/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_thread.c` & `libscca-20240427/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_thread_pool.h` & `libscca-20240427/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_support.h` & `libscca-20240427/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_lock.h` & `libscca-20240427/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_unused.h` & `libscca-20240427/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_lock.c` & `libscca-20240427/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_condition.h` & `libscca-20240427/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_repeating_thread.h` & `libscca-20240427/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/Makefile.am` & `libscca-20240427/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libscca-20240215/libcthreads/libcthreads_support.c` & `libscca-20240427/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_mutex.c` & `libscca-20240427/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_queue.c` & `libscca-20240427/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_mutex.h` & `libscca-20240427/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_types.h` & `libscca-20240427/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_thread_attributes.h` & `libscca-20240427/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_condition.c` & `libscca-20240427/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_error.c` & `libscca-20240427/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_read_write_lock.c` & `libscca-20240427/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_libcerror.h` & `libscca-20240427/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_definitions.h` & `libscca-20240427/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libscca-20240215/libcthreads/libcthreads_thread_pool.c` & `libscca-20240427/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_error.h` & `libscca-20240427/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_thread_attributes.c` & `libscca-20240427/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_extern.h` & `libscca-20240427/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/libcthreads_repeating_thread.c` & `libscca-20240427/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcthreads/Makefile.in` & `libscca-20240427/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -535,16 +535,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -559,15 +559,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -777,24 +778,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -888,17 +902,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libcthreads/libcthreads_queue.h` & `libscca-20240427/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca.spec` & `libscca-20240427/libscca.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libscca
-Version: 20240215
+Version: 20240427
 Release: 1
 Summary: Library to access the Windows Prefetch File (PF) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libscca
                
@@ -90,10 +90,10 @@
 %files -n libscca-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Thu Feb 15 2024 Joachim Metz <joachim.metz@gmail.com> 20240215-1
+* Sun Apr 28 2024 Joachim Metz <joachim.metz@gmail.com> 20240427-1
 - Auto-generated
```

### Comparing `libscca-20240215/test-driver` & `libscca-20240427/test-driver`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_support.c` & `libscca-20240427/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_libcerror.h` & `libscca-20240427/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_definitions.h` & `libscca-20240427/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libscca-20240215/libcpath/Makefile.am` & `libscca-20240427/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libscca-20240215/libcpath/libcpath_error.c` & `libscca-20240427/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_extern.h` & `libscca-20240427/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_system_string.h` & `libscca-20240427/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_support.h` & `libscca-20240427/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_libcsplit.h` & `libscca-20240427/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_system_string.c` & `libscca-20240427/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_libclocale.h` & `libscca-20240427/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_error.h` & `libscca-20240427/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/Makefile.in` & `libscca-20240427/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -511,16 +511,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -532,15 +532,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -743,24 +744,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -847,17 +854,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libcpath/libcpath_libuna.h` & `libscca-20240427/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_unused.h` & `libscca-20240427/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_path.c` & `libscca-20240427/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcpath/libcpath_path.h` & `libscca-20240427/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/ChangeLog` & `libscca-20240427/ChangeLog`

 * *Files identical despite different names*

### Comparing `libscca-20240215/manuals/sccainfo.1` & `libscca-20240427/manuals/sccainfo.1`

 * *Files identical despite different names*

### Comparing `libscca-20240215/manuals/libscca.3` & `libscca-20240427/manuals/libscca.3`

 * *Files identical despite different names*

### Comparing `libscca-20240215/manuals/Makefile.in` & `libscca-20240427/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -491,15 +491,16 @@
 	sccainfo.1 \
 	libscca.3
 
 EXTRA_DIST = \
 	sccainfo.1 \
 	libscca.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -692,23 +693,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -790,13 +793,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/tests/scca_test_file.c` & `libscca-20240427/tests/scca_test_file.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_libcerror.h` & `libscca-20240427/tests/scca_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/pyscca_test_support.py` & `libscca-20240427/tests/pyscca_test_support.py`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_file_header.c` & `libscca-20240427/tests/scca_test_file_header.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_tools_info_handle.c` & `libscca-20240427/tests/scca_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/pyscca_test_file.py` & `libscca-20240427/tests/pyscca_test_file.py`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_error.c` & `libscca-20240427/tests/scca_test_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_macros.h` & `libscca-20240427/tests/scca_test_macros.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/test_tools.sh` & `libscca-20240427/tests/test_tools.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output path_string signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libscca-20240215/tests/scca_test_libcpath.h` & `libscca-20240427/tests/scca_test_libcpath.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_tools_signal.c` & `libscca-20240427/tests/scca_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_volume_information.c` & `libscca-20240427/tests/scca_test_volume_information.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_file_metrics.c` & `libscca-20240427/tests/scca_test_file_metrics.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_io_handle.c` & `libscca-20240427/tests/scca_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_libscca.h` & `libscca-20240427/tests/scca_test_libscca.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_libbfio.h` & `libscca-20240427/tests/scca_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_file_information.c` & `libscca-20240427/tests/scca_test_file_information.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/Makefile.am` & `libscca-20240427/tests/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -281,13 +281,12 @@
 	scca_test_unused.h \
 	scca_test_volume_information.c
 
 scca_test_volume_information_LDADD = \
 	../libscca/libscca.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libscca-20240215/tests/scca_test_compressed_block.c` & `libscca-20240427/tests/scca_test_compressed_block.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_functions.h` & `libscca-20240427/tests/scca_test_functions.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_libuna.h` & `libscca-20240427/tests/scca_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/test_python_module.sh` & `libscca-20240427/tests/test_python_module.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="file";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libscca";
+PYTHON_MODULE="pyscca";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyscca_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyscca_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyscca");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libscca-20240215/tests/scca_test_functions.c` & `libscca-20240427/tests/scca_test_functions.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_getopt.h` & `libscca-20240427/tests/scca_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_notify.c` & `libscca-20240427/tests/scca_test_notify.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_libclocale.h` & `libscca-20240427/tests/scca_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/test_runner.sh` & `libscca-20240427/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_libcnotify.h` & `libscca-20240427/tests/scca_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_memory.h` & `libscca-20240427/tests/scca_test_memory.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_support.c` & `libscca-20240427/tests/scca_test_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_getopt.c` & `libscca-20240427/tests/scca_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_unused.h` & `libscca-20240427/tests/scca_test_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_memory.c` & `libscca-20240427/tests/scca_test_memory.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_tools_output.c` & `libscca-20240427/tests/scca_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/Makefile.in` & `libscca-20240427/tests/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -845,16 +845,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1109,16 +1109,18 @@
 	scca_test_unused.h \
 	scca_test_volume_information.c
 
 scca_test_volume_information_LDADD = \
 	../libscca/libscca.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1610,24 +1612,50 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../sccatools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../sccatools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../sccatools/$(DEPDIR)/info_handle.Po
+	-rm -f ../sccatools/$(DEPDIR)/path_string.Po
+	-rm -f ../sccatools/$(DEPDIR)/sccainput.Po
+	-rm -f ../sccatools/$(DEPDIR)/sccatools_output.Po
+	-rm -f ../sccatools/$(DEPDIR)/sccatools_signal.Po
+	-rm -f ./$(DEPDIR)/scca_test_compressed_block.Po
+	-rm -f ./$(DEPDIR)/scca_test_error.Po
+	-rm -f ./$(DEPDIR)/scca_test_file.Po
+	-rm -f ./$(DEPDIR)/scca_test_file_header.Po
+	-rm -f ./$(DEPDIR)/scca_test_file_information.Po
+	-rm -f ./$(DEPDIR)/scca_test_file_metrics.Po
+	-rm -f ./$(DEPDIR)/scca_test_filename_string.Po
+	-rm -f ./$(DEPDIR)/scca_test_filename_strings.Po
+	-rm -f ./$(DEPDIR)/scca_test_functions.Po
+	-rm -f ./$(DEPDIR)/scca_test_getopt.Po
+	-rm -f ./$(DEPDIR)/scca_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/scca_test_memory.Po
+	-rm -f ./$(DEPDIR)/scca_test_notify.Po
+	-rm -f ./$(DEPDIR)/scca_test_support.Po
+	-rm -f ./$(DEPDIR)/scca_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/scca_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/scca_test_tools_path_string.Po
+	-rm -f ./$(DEPDIR)/scca_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/scca_test_volume_information.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1734,13 +1762,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/tests/scca_test_filename_string.c` & `libscca-20240427/tests/scca_test_filename_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/scca_test_filename_strings.c` & `libscca-20240427/tests/scca_test_filename_strings.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/test_sccainfo.sh` & `libscca-20240427/tests/test_sccainfo.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("sccainfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libscca-20240215/tests/scca_test_tools_path_string.c` & `libscca-20240427/tests/scca_test_tools_path_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/tests/test_library.sh` & `libscca-20240427/tests/test_library.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="compressed_block error file_header file_information file_metrics filename_string filename_strings io_handle notify volume_information";
 LIBRARY_TESTS_WITH_INPUT="file support";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libscca-20240215/ossfuzz/ossfuzz_libscca.h` & `libscca-20240427/ossfuzz/ossfuzz_libscca.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/ossfuzz/Makefile.am` & `libscca-20240427/ossfuzz/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libscca/libscca.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
```

### Comparing `libscca-20240215/ossfuzz/ossfuzz_libbfio.h` & `libscca-20240427/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/ossfuzz/file_fuzzer.cc` & `libscca-20240427/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libscca-20240215/ossfuzz/Makefile.in` & `libscca-20240427/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -524,16 +524,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -553,15 +553,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libscca/libscca.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -803,23 +804,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -903,17 +907,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/ltmain.sh` & `libscca-20240427/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_locale_identifier.h` & `libscca-20240427/libfwnt/libfwnt_locale_identifier.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_lzxpress.c` & `libscca-20240427/libfwnt/libfwnt_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_extern.h` & `libscca-20240427/libfwnt/libfwnt_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_security_identifier.c` & `libscca-20240427/libfwnt/libfwnt_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_libcerror.h` & `libscca-20240427/libfwnt/libfwnt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_bit_stream.c` & `libscca-20240427/libfwnt/libfwnt_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_error.h` & `libscca-20240427/libfwnt/libfwnt_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_lznt1.h` & `libscca-20240427/libfwnt/libfwnt_lznt1.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_notify.c` & `libscca-20240427/libfwnt/libfwnt_notify.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/Makefile.am` & `libscca-20240427/libfwnt/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFWNT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfwnt.la
@@ -30,19 +30,17 @@
 	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 	libfwnt_support.c libfwnt_support.h \
 	libfwnt_types.h \
 	libfwnt_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
```

### Comparing `libscca-20240215/libfwnt/libfwnt_security_identifier.h` & `libscca-20240427/libfwnt/libfwnt_security_identifier.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_support.h` & `libscca-20240427/libfwnt/libfwnt_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_huffman_tree.h` & `libscca-20240427/libfwnt/libfwnt_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_error.c` & `libscca-20240427/libfwnt/libfwnt_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_access_control_list.h` & `libscca-20240427/libfwnt/libfwnt_access_control_list.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_security_descriptor.c` & `libscca-20240427/libfwnt/libfwnt_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_access_control_list.c` & `libscca-20240427/libfwnt/libfwnt_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_definitions.h` & `libscca-20240427/libfwnt/libfwnt_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwnt/definitions.h> are copied here
  * for local use of libfwnt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWNT_VERSION					20240126
+#define LIBFWNT_VERSION					20240415
 
 /* The version string
  */
-#define LIBFWNT_VERSION_STRING				"20240126"
+#define LIBFWNT_VERSION_STRING				"20240415"
 
 
 /* The endian definitions
  */
 #define LIBFWNT_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWNT_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
```

### Comparing `libscca-20240215/libfwnt/libfwnt_huffman_tree.c` & `libscca-20240427/libfwnt/libfwnt_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_debug.c` & `libscca-20240427/libfwnt/libfwnt_debug.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_lznt1.c` & `libscca-20240427/libfwnt/libfwnt_lznt1.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_notify.h` & `libscca-20240427/libfwnt/libfwnt_notify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_locale_identifier.c` & `libscca-20240427/libfwnt/libfwnt_locale_identifier.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_debug.h` & `libscca-20240427/libfwnt/libfwnt_debug.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_libcdata.h` & `libscca-20240427/libfwnt/libfwnt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_lzx.h` & `libscca-20240427/libfwnt/libfwnt_lzx.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_unused.h` & `libscca-20240427/libfwnt/libfwnt_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_libcnotify.h` & `libscca-20240427/libfwnt/libfwnt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_access_control_entry.c` & `libscca-20240427/libfwnt/libfwnt_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_lzxpress.h` & `libscca-20240427/libfwnt/libfwnt_lzxpress.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_security_descriptor.h` & `libscca-20240427/libfwnt/libfwnt_security_descriptor.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_lzx.c` & `libscca-20240427/libfwnt/libfwnt_lzx.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/Makefile.in` & `libscca-20240427/libfwnt/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -537,16 +537,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFWNT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFWNT_TRUE@noinst_LTLIBRARIES = libfwnt.la
@@ -569,15 +569,16 @@
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_notify.c libfwnt_notify.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_support.c libfwnt_support.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_types.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -790,24 +791,40 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfwnt_access_control_entry.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_access_control_list.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_error.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_locale_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lznt1.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzx.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzxpress.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -904,17 +921,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libfwnt/libfwnt_bit_stream.h` & `libscca-20240427/libfwnt/libfwnt_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_types.h` & `libscca-20240427/libfwnt/libfwnt_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_support.c` & `libscca-20240427/libfwnt/libfwnt_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfwnt/libfwnt_access_control_entry.h` & `libscca-20240427/libfwnt/libfwnt_access_control_entry.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_narrow_string.c` & `libscca-20240427/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_definitions.h` & `libscca-20240427/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libscca-20240215/libcsplit/libcsplit_types.h` & `libscca-20240427/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_wide_split_string.c` & `libscca-20240427/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_support.h` & `libscca-20240427/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/Makefile.am` & `libscca-20240427/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libscca-20240215/libcsplit/libcsplit_libcerror.h` & `libscca-20240427/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_wide_string.c` & `libscca-20240427/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_unused.h` & `libscca-20240427/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_wide_split_string.h` & `libscca-20240427/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_error.c` & `libscca-20240427/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_narrow_split_string.c` & `libscca-20240427/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_extern.h` & `libscca-20240427/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_error.h` & `libscca-20240427/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_support.c` & `libscca-20240427/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_wide_string.h` & `libscca-20240427/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/Makefile.in` & `libscca-20240427/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -521,16 +521,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -539,15 +539,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -752,24 +753,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -858,17 +867,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libcsplit/libcsplit_narrow_split_string.h` & `libscca-20240427/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcsplit/libcsplit_narrow_string.h` & `libscca-20240427/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/po/remove-potcdate.sin` & `libscca-20240427/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libscca-20240215/po/Makefile.in.in` & `libscca-20240427/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/po/en@quot.header` & `libscca-20240427/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libscca-20240215/po/en@boldquot.header` & `libscca-20240427/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libscca-20240215/po/insert-header.sin` & `libscca-20240427/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libscca-20240215/po/Makevars` & `libscca-20240427/po/Makevars`

 * *Files identical despite different names*

### Comparing `libscca-20240215/po/Makevars.in` & `libscca-20240427/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/po/Rules-quot` & `libscca-20240427/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1251.c` & `libscca-20240427/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf16_string.c` & `libscca-20240427/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_base16_stream.c` & `libscca-20240427/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf8_stream.h` & `libscca-20240427/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_2.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_932.c` & `libscca-20240427/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_dingbats.h` & `libscca-20240427/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf8_string.c` & `libscca-20240427/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_base64_stream.c` & `libscca-20240427/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_error.h` & `libscca-20240427/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_turkish.h` & `libscca-20240427/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_unicode_character.c` & `libscca-20240427/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_gaelic.c` & `libscca-20240427/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_arabic.h` & `libscca-20240427/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_thai.c` & `libscca-20240427/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_874.h` & `libscca-20240427/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_15.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf8_string.h` & `libscca-20240427/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_16.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1255.c` & `libscca-20240427/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf7_stream.c` & `libscca-20240427/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_byte_stream.h` & `libscca-20240427/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_koi8_u.c` & `libscca-20240427/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_unused.h` & `libscca-20240427/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_6.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_14.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_base64_stream.h` & `libscca-20240427/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_error.c` & `libscca-20240427/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_centraleurroman.h` & `libscca-20240427/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_romanian.c` & `libscca-20240427/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_6.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_9.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_russian.h` & `libscca-20240427/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_dingbats.c` & `libscca-20240427/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_15.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_936.c` & `libscca-20240427/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_croatian.h` & `libscca-20240427/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_scsu.h` & `libscca-20240427/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/Makefile.am` & `libscca-20240427/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libscca-20240215/libuna/libuna_utf32_stream.c` & `libscca-20240427/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_936.h` & `libscca-20240427/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_10.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_roman.c` & `libscca-20240427/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf7_stream.h` & `libscca-20240427/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_3.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_thai.h` & `libscca-20240427/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_farsi.h` & `libscca-20240427/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_ukrainian.c` & `libscca-20240427/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_inuit.c` & `libscca-20240427/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_932.h` & `libscca-20240427/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_874.c` & `libscca-20240427/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_5.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_10.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_definitions.h` & `libscca-20240427/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libscca-20240215/libuna/libuna_url_stream.h` & `libscca-20240427/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_icelandic.h` & `libscca-20240427/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_koi8_u.h` & `libscca-20240427/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf16_stream.c` & `libscca-20240427/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1253.c` & `libscca-20240427/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_4.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_greek.c` & `libscca-20240427/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_libcerror.h` & `libscca-20240427/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_centraleurroman.c` & `libscca-20240427/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1254.c` & `libscca-20240427/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_13.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_7.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1255.h` & `libscca-20240427/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_unicode_character.h` & `libscca-20240427/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_8.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_13.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_949.h` & `libscca-20240427/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_cyrillic.c` & `libscca-20240427/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_celtic.c` & `libscca-20240427/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_support.h` & `libscca-20240427/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_4.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_949.c` & `libscca-20240427/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf16_stream.h` & `libscca-20240427/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_symbol.c` & `libscca-20240427/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_roman.h` & `libscca-20240427/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1257.c` & `libscca-20240427/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1254.h` & `libscca-20240427/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_950.c` & `libscca-20240427/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_extern.h` & `libscca-20240427/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1256.c` & `libscca-20240427/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_types.h` & `libscca-20240427/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_base32_stream.h` & `libscca-20240427/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1253.h` & `libscca-20240427/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_16.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf8_stream.c` & `libscca-20240427/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1250.h` & `libscca-20240427/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_2.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_support.c` & `libscca-20240427/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_koi8_r.c` & `libscca-20240427/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_5.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf16_string.h` & `libscca-20240427/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf32_string.c` & `libscca-20240427/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_icelandic.c` & `libscca-20240427/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1256.h` & `libscca-20240427/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf32_string.h` & `libscca-20240427/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_romanian.h` & `libscca-20240427/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_8.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_koi8_r.h` & `libscca-20240427/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_cyrillic.h` & `libscca-20240427/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_arabic.c` & `libscca-20240427/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_croatian.c` & `libscca-20240427/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_9.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_greek.h` & `libscca-20240427/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1258.h` & `libscca-20240427/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_7.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/Makefile.in` & `libscca-20240427/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -689,16 +689,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -764,15 +764,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1034,24 +1035,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1197,17 +1263,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_3.c` & `libscca-20240427/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1250.c` & `libscca-20240427/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_scsu.c` & `libscca-20240427/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1252.c` & `libscca-20240427/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_turkish.c` & `libscca-20240427/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_ukrainian.h` & `libscca-20240427/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_russian.c` & `libscca-20240427/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1258.c` & `libscca-20240427/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_celtic.h` & `libscca-20240427/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_byte_stream.c` & `libscca-20240427/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_gaelic.h` & `libscca-20240427/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_utf32_stream.h` & `libscca-20240427/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_symbol.h` & `libscca-20240427/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1257.h` & `libscca-20240427/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_inuit.h` & `libscca-20240427/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_mac_farsi.c` & `libscca-20240427/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_950.h` & `libscca-20240427/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_url_stream.c` & `libscca-20240427/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1251.h` & `libscca-20240427/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_windows_1252.h` & `libscca-20240427/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_codepage_iso_8859_14.h` & `libscca-20240427/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_base16_stream.h` & `libscca-20240427/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libuna/libuna_base32_stream.c` & `libscca-20240427/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/Makefile.in` & `libscca-20240427/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -635,16 +635,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libscca.pc \
+	libscca.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libscca.pc
 
 all: all-recursive
 
@@ -1061,23 +1068,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1189,22 +1199,10 @@
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libscca && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libscca.pc
-	-rm -f libscca.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libscca-20240215/libfvalue/libfvalue_filetime.c` & `libscca-20240427/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_utf16_string.c` & `libscca-20240427/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_libfwnt.h` & `libscca-20240427/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_value.c` & `libscca-20240427/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_value.h` & `libscca-20240427/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_definitions.h` & `libscca-20240427/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libscca-20240215/libfvalue/libfvalue_codepage.h` & `libscca-20240427/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_split_utf16_string.c` & `libscca-20240427/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_error.c` & `libscca-20240427/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_utf8_string.c` & `libscca-20240427/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_unused.h` & `libscca-20240427/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_split_utf16_string.h` & `libscca-20240427/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_filetime.h` & `libscca-20240427/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_support.c` & `libscca-20240427/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_extern.h` & `libscca-20240427/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/Makefile.am` & `libscca-20240427/libfvalue/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFWNT_CPPFLAGS@ \
@@ -40,19 +40,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libscca-20240215/libfvalue/libfvalue_value_type.h` & `libscca-20240427/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_libcerror.h` & `libscca-20240427/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_split_utf8_string.c` & `libscca-20240427/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_data_handle.h` & `libscca-20240427/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_libcnotify.h` & `libscca-20240427/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_data_handle.c` & `libscca-20240427/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_integer.c` & `libscca-20240427/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_value_type.c` & `libscca-20240427/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_integer.h` & `libscca-20240427/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_binary_data.h` & `libscca-20240427/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_value_entry.h` & `libscca-20240427/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_utf16_string.h` & `libscca-20240427/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_error.h` & `libscca-20240427/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_table.h` & `libscca-20240427/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_libfguid.h` & `libscca-20240427/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_split_utf8_string.h` & `libscca-20240427/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_floating_point.h` & `libscca-20240427/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_libfdatetime.h` & `libscca-20240427/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_string.h` & `libscca-20240427/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_binary_data.c` & `libscca-20240427/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_value_entry.c` & `libscca-20240427/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_libcdata.h` & `libscca-20240427/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_support.h` & `libscca-20240427/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_table.c` & `libscca-20240427/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/Makefile.in` & `libscca-20240427/libfvalue/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -552,16 +552,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFWNT_CPPFLAGS@ \
@@ -594,15 +594,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -817,24 +818,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -933,17 +952,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libfvalue/libfvalue_utf8_string.h` & `libscca-20240427/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_floating_point.c` & `libscca-20240427/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_types.h` & `libscca-20240427/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_string.c` & `libscca-20240427/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfvalue/libfvalue_libuna.h` & `libscca-20240427/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_definitions.h` & `libscca-20240427/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libscca-20240215/libcnotify/libcnotify_extern.h` & `libscca-20240427/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_support.c` & `libscca-20240427/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_stream.h` & `libscca-20240427/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/Makefile.am` & `libscca-20240427/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libscca-20240215/libcnotify/libcnotify_unused.h` & `libscca-20240427/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_verbose.h` & `libscca-20240427/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_print.h` & `libscca-20240427/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_stream.c` & `libscca-20240427/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_support.h` & `libscca-20240427/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_verbose.c` & `libscca-20240427/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/Makefile.in` & `libscca-20240427/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -513,30 +513,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -739,24 +740,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -843,17 +850,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libcnotify/libcnotify_libcerror.h` & `libscca-20240427/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcnotify/libcnotify_print.c` & `libscca-20240427/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/libcerror_system.c` & `libscca-20240427/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/libcerror_error.c` & `libscca-20240427/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/libcerror_extern.h` & `libscca-20240427/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/Makefile.am` & `libscca-20240427/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libscca-20240215/libcerror/libcerror_types.h` & `libscca-20240427/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/libcerror_support.h` & `libscca-20240427/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/libcerror_error.h` & `libscca-20240427/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/libcerror_system.h` & `libscca-20240427/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/libcerror_definitions.h` & `libscca-20240427/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libscca-20240215/libcerror/libcerror_support.c` & `libscca-20240427/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/libcerror_unused.h` & `libscca-20240427/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libcerror/Makefile.in` & `libscca-20240427/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -510,28 +510,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -733,24 +734,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -836,17 +842,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libfdatetime/libfdatetime_floatingtime.h` & `libscca-20240427/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_nsf_timedate.c` & `libscca-20240427/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_error.h` & `libscca-20240427/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_floatingtime.c` & `libscca-20240427/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_support.h` & `libscca-20240427/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_hfs_time.h` & `libscca-20240427/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_definitions.h` & `libscca-20240427/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libscca-20240215/libfdatetime/libfdatetime_hfs_time.c` & `libscca-20240427/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/Makefile.am` & `libscca-20240427/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libscca-20240215/libfdatetime/libfdatetime_filetime.c` & `libscca-20240427/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_systemtime.h` & `libscca-20240427/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_extern.h` & `libscca-20240427/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_posix_time.c` & `libscca-20240427/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_unused.h` & `libscca-20240427/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_fat_date_time.h` & `libscca-20240427/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_systemtime.c` & `libscca-20240427/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_nsf_timedate.h` & `libscca-20240427/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_libcerror.h` & `libscca-20240427/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_support.c` & `libscca-20240427/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_error.c` & `libscca-20240427/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_posix_time.h` & `libscca-20240427/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_date_time_values.h` & `libscca-20240427/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_filetime.h` & `libscca-20240427/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_date_time_values.c` & `libscca-20240427/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/libfdatetime_types.h` & `libscca-20240427/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libfdatetime/Makefile.in` & `libscca-20240427/libfdatetime/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -532,16 +532,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -554,15 +554,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -771,24 +772,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -881,17 +894,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libscca-20240215/libfdatetime/libfdatetime_fat_date_time.c` & `libscca-20240427/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libscca-20240215/aclocal.m4` & `libscca-20240427/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libscca-20240215/libscca.spec.in` & `libscca-20240427/libscca.spec.in`

 * *Files identical despite different names*

### Comparing `libscca-20240215/configure.ac` & `libscca-20240427/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libscca],
- [20240215],
+ [20240427],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libscca.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

