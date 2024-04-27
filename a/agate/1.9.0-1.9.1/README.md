# Comparing `tmp/agate-1.9.0.tar.gz` & `tmp/agate-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agate-1.9.0.tar", last modified: Wed Oct 18 03:54:22 2023, max compression
+gzip compressed data, was "agate-1.9.1.tar", last modified: Thu Dec 21 20:05:08 2023, max compression
```

## Comparing `agate-1.9.0.tar` & `agate-1.9.1.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.026629 agate-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-10-18 03:54:10.000000 agate-1.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38646 2023-10-18 03:54:10.000000 agate-1.9.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-10-18 03:54:10.000000 agate-1.9.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-18 03:54:10.000000 agate-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2023-10-18 03:54:22.026629 agate-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-10-18 03:54:10.000000 agate-1.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:21.982628 agate-1.9.0/agate/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-10-18 03:54:10.000000 agate-1.9.0/agate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:21.986628 agate-1.9.0/agate/aggregations/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/all.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/any.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/deciles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/first.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/has_nulls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/iqr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/mad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/max_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/max_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/median.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/min.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/quartiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/quintiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/stdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-10-18 03:54:10.000000 agate-1.9.0/agate/aggregations/variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2023-10-18 03:54:10.000000 agate-1.9.0/agate/columns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:21.986628 agate-1.9.0/agate/computations/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/change.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/percent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/percent_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/percentile_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-10-18 03:54:10.000000 agate-1.9.0/agate/computations/slug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2023-10-18 03:54:10.000000 agate-1.9.0/agate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2023-10-18 03:54:10.000000 agate-1.9.0/agate/csv_py3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:21.990628 agate-1.9.0/agate/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-10-18 03:54:10.000000 agate-1.9.0/agate/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-10-18 03:54:10.000000 agate-1.9.0/agate/data_types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-10-18 03:54:10.000000 agate-1.9.0/agate/data_types/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2023-10-18 03:54:10.000000 agate-1.9.0/agate/data_types/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2023-10-18 03:54:10.000000 agate-1.9.0/agate/data_types/date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2023-10-18 03:54:10.000000 agate-1.9.0/agate/data_types/number.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-10-18 03:54:10.000000 agate-1.9.0/agate/data_types/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-10-18 03:54:10.000000 agate-1.9.0/agate/data_types/time_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-10-18 03:54:10.000000 agate-1.9.0/agate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-10-18 03:54:10.000000 agate-1.9.0/agate/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-10-18 03:54:10.000000 agate-1.9.0/agate/mapped_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-10-18 03:54:10.000000 agate-1.9.0/agate/rows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:21.994629 agate-1.9.0/agate/table/
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/bins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/column_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/denormalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/distinct.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/find.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/from_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/from_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/group_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/homogenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/join.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/print_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/print_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/print_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/print_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/to_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-10-18 03:54:10.000000 agate-1.9.0/agate/table/where.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:21.998628 agate-1.9.0/agate/tableset/
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/column_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/having.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/print_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/proxy_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-18 03:54:10.000000 agate-1.9.0/agate/tableset/to_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-10-18 03:54:10.000000 agate-1.9.0/agate/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2023-10-18 03:54:10.000000 agate-1.9.0/agate/type_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2023-10-18 03:54:10.000000 agate-1.9.0/agate/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-10-18 03:54:10.000000 agate-1.9.0/agate/warns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:21.982628 agate-1.9.0/agate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2023-10-18 03:54:21.000000 agate-1.9.0/agate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2023-10-18 03:54:21.000000 agate-1.9.0/agate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 03:54:21.000000 agate-1.9.0/agate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-10-18 03:54:21.000000 agate-1.9.0/agate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-18 03:54:21.000000 agate-1.9.0/agate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:21.998628 agate-1.9.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:10.000000 agate-1.9.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-10-18 03:54:10.000000 agate-1.9.0/benchmarks/test_joins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      994 2023-10-18 03:54:10.000000 agate-1.9.0/charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.002628 agate-1.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-10-18 03:54:10.000000 agate-1.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-10-18 03:54:10.000000 agate-1.9.0/docs/about.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.006628 agate-1.9.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/aggregations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/columns_and_rows.rst
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/computations.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/csv.rst
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/data_types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/fixed.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/table.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/tableset.rst
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/testcase.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/type_tester.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api/warns.rst
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-18 03:54:10.000000 agate-1.9.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-18 03:54:10.000000 agate-1.9.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-10-18 03:54:10.000000 agate-1.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2023-10-18 03:54:10.000000 agate-1.9.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.010629 agate-1.9.0/docs/cookbook/
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/charting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/columns.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/compute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/create.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/excel.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/filter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/homogenize.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/locale.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/lookup.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/r.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/rank.rst
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/remove.rst
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/save.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/search.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/sort.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/sql.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/standardize.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/statistics.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/transform.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook/underscore.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-10-18 03:54:10.000000 agate-1.9.0/docs/cookbook.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-10-18 03:54:10.000000 agate-1.9.0/docs/extensions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.010629 agate-1.9.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2023-10-18 03:54:10.000000 agate-1.9.0/docs/images/bar_chart.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2023-10-18 03:54:10.000000 agate-1.9.0/docs/images/column_chart.svg
--rw-r--r--   0 runner    (1001) docker     (127)    93360 2023-10-18 03:54:10.000000 agate-1.9.0/docs/images/dots_chart.svg
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2023-10-18 03:54:10.000000 agate-1.9.0/docs/images/lattice.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-10-18 03:54:10.000000 agate-1.9.0/docs/images/line_chart.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-10-18 03:54:10.000000 agate-1.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-10-18 03:54:10.000000 agate-1.9.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-18 03:54:10.000000 agate-1.9.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-18 03:54:10.000000 agate-1.9.0/docs/release_process.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-18 03:54:10.000000 agate-1.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-18 03:54:10.000000 agate-1.9.0/docs/tutorial.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1473 2023-10-18 03:54:10.000000 agate-1.9.0/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2023-10-18 03:54:10.000000 agate-1.9.0/example.py.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.014629 agate-1.9.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.014629 agate-1.9.0/examples/realdata/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-10-18 03:54:10.000000 agate-1.9.0/examples/realdata/Datagov_FY10_EDU_recp_by_State.csv
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-18 03:54:10.000000 agate-1.9.0/examples/realdata/README.csv
--rw-r--r--   0 runner    (1001) docker     (127)   126910 2023-10-18 03:54:10.000000 agate-1.9.0/examples/realdata/exonerations-20150828.csv
--rw-r--r--   0 runner    (1001) docker     (127)   212083 2023-10-18 03:54:10.000000 agate-1.9.0/examples/realdata/ks_1033_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.018628 agate-1.9.0/examples/tableset/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-18 03:54:10.000000 agate-1.9.0/examples/tableset/table1.csv
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-18 03:54:10.000000 agate-1.9.0/examples/tableset/table1.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-18 03:54:10.000000 agate-1.9.0/examples/tableset/table2.csv
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-18 03:54:10.000000 agate-1.9.0/examples/tableset/table2.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-18 03:54:10.000000 agate-1.9.0/examples/tableset/table3.csv
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-18 03:54:10.000000 agate-1.9.0/examples/tableset/table3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.018628 agate-1.9.0/examples/tableset/type_error/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-18 03:54:10.000000 agate-1.9.0/examples/tableset/type_error/table1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-18 03:54:10.000000 agate-1.9.0/examples/tableset/type_error/table2.csv
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test.json
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_cr.csv
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_crlf.csv
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_csv_sniff.csv
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_from_json_ambiguous.json
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_key.json
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_keyed.json
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_latin1.csv
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_mixed.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_nested.json
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_newline.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_no_header.csv
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_non_string_keyed.json
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_tableset.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_utf16_big.csv
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-18 03:54:10.000000 agate-1.9.0/examples/test_utf16_little.csv
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-18 03:54:10.000000 agate-1.9.0/examples/testfixed
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-18 03:54:10.000000 agate-1.9.0/examples/testfixed_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-18 03:54:10.000000 agate-1.9.0/examples/testfixed_schema.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     2674 2023-10-18 03:54:10.000000 agate-1.9.0/exonerations.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-18 03:54:22.026629 agate-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-10-18 03:54:10.000000 agate-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.018628 agate-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-18 03:54:10.000000 agate-1.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_agate.py
--rw-r--r--   0 runner    (1001) docker     (127)    27223 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    18075 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_computations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21440 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_mapped_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_py3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.022628 agate-1.9.0/tests/test_table/
--rw-r--r--   0 runner    (1001) docker     (127)    21907 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_bins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_charting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_denormalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_from_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_group_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_homogenize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_order_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_print_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_print_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_print_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_print_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_table/test_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 03:54:22.026629 agate-1.9.0/tests/test_tableset/
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_tableset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_tableset/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_tableset/test_charting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_tableset/test_having.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_tableset/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_type_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2023-10-18 03:54:10.000000 agate-1.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   125652 2023-10-18 03:54:10.000000 agate-1.9.0/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.491449 agate-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-12-21 20:05:00.000000 agate-1.9.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38726 2023-12-21 20:05:00.000000 agate-1.9.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-21 20:05:00.000000 agate-1.9.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2023-12-21 20:05:00.000000 agate-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2023-12-21 20:05:08.491449 agate-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-12-21 20:05:00.000000 agate-1.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.451449 agate-1.9.1/agate/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2023-12-21 20:05:00.000000 agate-1.9.1/agate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.459449 agate-1.9.1/agate/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/deciles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/has_nulls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/iqr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/mad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/max_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/max_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/quartiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/quintiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/stdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-12-21 20:05:00.000000 agate-1.9.1/agate/aggregations/variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2023-12-21 20:05:00.000000 agate-1.9.1/agate/columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.459449 agate-1.9.1/agate/computations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/percent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/percent_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/percentile_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-12-21 20:05:00.000000 agate-1.9.1/agate/computations/slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2023-12-21 20:05:00.000000 agate-1.9.1/agate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2023-12-21 20:05:00.000000 agate-1.9.1/agate/csv_py3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.459449 agate-1.9.1/agate/data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-21 20:05:00.000000 agate-1.9.1/agate/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-12-21 20:05:00.000000 agate-1.9.1/agate/data_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-12-21 20:05:00.000000 agate-1.9.1/agate/data_types/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2023-12-21 20:05:00.000000 agate-1.9.1/agate/data_types/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2023-12-21 20:05:00.000000 agate-1.9.1/agate/data_types/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2023-12-21 20:05:00.000000 agate-1.9.1/agate/data_types/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-21 20:05:00.000000 agate-1.9.1/agate/data_types/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-21 20:05:00.000000 agate-1.9.1/agate/data_types/time_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-12-21 20:05:00.000000 agate-1.9.1/agate/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-12-21 20:05:00.000000 agate-1.9.1/agate/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-12-21 20:05:00.000000 agate-1.9.1/agate/mapped_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-21 20:05:00.000000 agate-1.9.1/agate/rows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.467449 agate-1.9.1/agate/table/
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/column_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/denormalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/distinct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/from_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/from_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/homogenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/print_bars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/print_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/print_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-21 20:05:00.000000 agate-1.9.1/agate/table/where.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.467449 agate-1.9.1/agate/tableset/
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/column_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/having.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/print_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/proxy_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-12-21 20:05:00.000000 agate-1.9.1/agate/tableset/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-12-21 20:05:00.000000 agate-1.9.1/agate/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2023-12-21 20:05:00.000000 agate-1.9.1/agate/type_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2023-12-21 20:05:00.000000 agate-1.9.1/agate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-12-21 20:05:00.000000 agate-1.9.1/agate/warns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.491449 agate-1.9.1/agate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2023-12-21 20:05:08.000000 agate-1.9.1/agate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2023-12-21 20:05:08.000000 agate-1.9.1/agate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 20:05:08.000000 agate-1.9.1/agate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-21 20:05:08.000000 agate-1.9.1/agate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-21 20:05:08.000000 agate-1.9.1/agate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.467449 agate-1.9.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:00.000000 agate-1.9.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2023-12-21 20:05:00.000000 agate-1.9.1/benchmarks/test_joins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      994 2023-12-21 20:05:00.000000 agate-1.9.1/charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.471449 agate-1.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-12-21 20:05:00.000000 agate-1.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-12-21 20:05:00.000000 agate-1.9.1/docs/about.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.475449 agate-1.9.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/aggregations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/columns_and_rows.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/computations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/data_types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/fixed.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/table.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/tableset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/testcase.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/type_tester.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api/warns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-21 20:05:00.000000 agate-1.9.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-21 20:05:00.000000 agate-1.9.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-12-21 20:05:00.000000 agate-1.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2023-12-21 20:05:00.000000 agate-1.9.1/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.479449 agate-1.9.1/docs/cookbook/
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/charting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/columns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/compute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/excel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/filter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/homogenize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/locale.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/lookup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/r.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/rank.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/remove.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/save.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/search.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/sort.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/sql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/standardize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/transform.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook/underscore.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-12-21 20:05:00.000000 agate-1.9.1/docs/cookbook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-12-21 20:05:00.000000 agate-1.9.1/docs/extensions.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.479449 agate-1.9.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2023-12-21 20:05:00.000000 agate-1.9.1/docs/images/bar_chart.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2023-12-21 20:05:00.000000 agate-1.9.1/docs/images/column_chart.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    93360 2023-12-21 20:05:00.000000 agate-1.9.1/docs/images/dots_chart.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2023-12-21 20:05:00.000000 agate-1.9.1/docs/images/lattice.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-12-21 20:05:00.000000 agate-1.9.1/docs/images/line_chart.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-12-21 20:05:00.000000 agate-1.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-21 20:05:00.000000 agate-1.9.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-21 20:05:00.000000 agate-1.9.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2023-12-21 20:05:00.000000 agate-1.9.1/docs/release_process.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-21 20:05:00.000000 agate-1.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-21 20:05:00.000000 agate-1.9.1/docs/tutorial.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1473 2023-12-21 20:05:00.000000 agate-1.9.1/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2023-12-21 20:05:00.000000 agate-1.9.1/example.py.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.483449 agate-1.9.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.483449 agate-1.9.1/examples/realdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-21 20:05:00.000000 agate-1.9.1/examples/realdata/Datagov_FY10_EDU_recp_by_State.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-21 20:05:00.000000 agate-1.9.1/examples/realdata/README.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   126910 2023-12-21 20:05:00.000000 agate-1.9.1/examples/realdata/exonerations-20150828.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   212083 2023-12-21 20:05:00.000000 agate-1.9.1/examples/realdata/ks_1033_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.483449 agate-1.9.1/examples/tableset/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-21 20:05:00.000000 agate-1.9.1/examples/tableset/table1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-21 20:05:00.000000 agate-1.9.1/examples/tableset/table1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-21 20:05:00.000000 agate-1.9.1/examples/tableset/table2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-21 20:05:00.000000 agate-1.9.1/examples/tableset/table2.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-21 20:05:00.000000 agate-1.9.1/examples/tableset/table3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-21 20:05:00.000000 agate-1.9.1/examples/tableset/table3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.483449 agate-1.9.1/examples/tableset/type_error/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-21 20:05:00.000000 agate-1.9.1/examples/tableset/type_error/table1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-21 20:05:00.000000 agate-1.9.1/examples/tableset/type_error/table2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_cr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_crlf.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_csv_sniff.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_from_json_ambiguous.json
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_key.json
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_keyed.json
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_latin1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_mixed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_nested.json
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_newline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_no_header.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_non_string_keyed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_tableset.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_utf16_big.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-21 20:05:00.000000 agate-1.9.1/examples/test_utf16_little.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-21 20:05:00.000000 agate-1.9.1/examples/testfixed
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-21 20:05:00.000000 agate-1.9.1/examples/testfixed_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-21 20:05:00.000000 agate-1.9.1/examples/testfixed_schema.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2674 2023-12-21 20:05:00.000000 agate-1.9.1/exonerations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-21 20:05:08.491449 agate-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-12-21 20:05:00.000000 agate-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.487449 agate-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-21 20:05:00.000000 agate-1.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_agate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27223 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18075 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_computations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21440 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_mapped_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_py3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.491449 agate-1.9.1/tests/test_table/
+-rw-r--r--   0 runner    (1001) docker     (127)    21907 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_charting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_denormalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_from_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_homogenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_order_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_print_bars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_print_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_print_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_print_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_table/test_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 20:05:08.491449 agate-1.9.1/tests/test_tableset/
+-rw-r--r--   0 runner    (1001) docker     (127)    11417 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_tableset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_tableset/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_tableset/test_charting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_tableset/test_having.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_tableset/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_type_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2023-12-21 20:05:00.000000 agate-1.9.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125652 2023-12-21 20:05:00.000000 agate-1.9.1/tutorial.ipynb
```

### Comparing `agate-1.9.0/AUTHORS.rst` & `agate-1.9.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/CHANGELOG.rst` & `agate-1.9.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.9.1 - December 21, 2023
+-------------------------
+
+* Add Babel 2.14 support.
+
 1.9.0 - October 17, 2023
 ------------------------
 
 * feat: Add a ``text_truncation_chars`` configuration for values that exceed ``max_column_width`` in :meth:`.Table.print_table` and :meth:`.Table.print_html`.
 * feat: Add a ``number_truncation_chars`` configuration for values that exceed ``max_precision`` in :meth:`.Table.print_table` and :meth:`.Table.print_html`.
 
 1.8.0 - October 10, 2023
```

### Comparing `agate-1.9.0/COPYING` & `agate-1.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/PKG-INFO` & `agate-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agate
-Version: 1.9.0
+Version: 1.9.1
 Summary: A data analysis library that is optimized for humans instead of machines.
 Home-page: https://agate.readthedocs.org/
 Author: Christopher Groskopf
 Author-email: chrisgroskopf@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/wireservice/agate
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `agate-1.9.0/README.rst` & `agate-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/__init__.py` & `agate-1.9.1/agate/__init__.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/__init__.py` & `agate-1.9.1/agate/aggregations/__init__.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/all.py` & `agate-1.9.1/agate/aggregations/all.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/any.py` & `agate-1.9.1/agate/aggregations/any.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/base.py` & `agate-1.9.1/agate/aggregations/base.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/count.py` & `agate-1.9.1/agate/aggregations/count.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/deciles.py` & `agate-1.9.1/agate/aggregations/deciles.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/first.py` & `agate-1.9.1/agate/aggregations/first.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/iqr.py` & `agate-1.9.1/agate/aggregations/iqr.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/mad.py` & `agate-1.9.1/agate/aggregations/mad.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/max.py` & `agate-1.9.1/agate/aggregations/max.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/max_length.py` & `agate-1.9.1/agate/aggregations/max_length.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/max_precision.py` & `agate-1.9.1/agate/aggregations/max_precision.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/mean.py` & `agate-1.9.1/agate/aggregations/mean.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/median.py` & `agate-1.9.1/agate/aggregations/median.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/min.py` & `agate-1.9.1/agate/aggregations/min.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/mode.py` & `agate-1.9.1/agate/aggregations/mode.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/percentiles.py` & `agate-1.9.1/agate/aggregations/percentiles.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/quartiles.py` & `agate-1.9.1/agate/aggregations/quartiles.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/quintiles.py` & `agate-1.9.1/agate/aggregations/quintiles.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/stdev.py` & `agate-1.9.1/agate/aggregations/stdev.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/sum.py` & `agate-1.9.1/agate/aggregations/sum.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/summary.py` & `agate-1.9.1/agate/aggregations/summary.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/aggregations/variance.py` & `agate-1.9.1/agate/aggregations/variance.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/columns.py` & `agate-1.9.1/agate/columns.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/__init__.py` & `agate-1.9.1/agate/computations/__init__.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/base.py` & `agate-1.9.1/agate/computations/base.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/change.py` & `agate-1.9.1/agate/computations/change.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/formula.py` & `agate-1.9.1/agate/computations/formula.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/percent.py` & `agate-1.9.1/agate/computations/percent.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/percent_change.py` & `agate-1.9.1/agate/computations/percent_change.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/percentile_rank.py` & `agate-1.9.1/agate/computations/percentile_rank.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/rank.py` & `agate-1.9.1/agate/computations/rank.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/computations/slug.py` & `agate-1.9.1/agate/computations/slug.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/config.py` & `agate-1.9.1/agate/config.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/csv_py3.py` & `agate-1.9.1/agate/csv_py3.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/data_types/__init__.py` & `agate-1.9.1/agate/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/data_types/base.py` & `agate-1.9.1/agate/data_types/base.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/data_types/boolean.py` & `agate-1.9.1/agate/data_types/boolean.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/data_types/date.py` & `agate-1.9.1/agate/data_types/date.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/data_types/date_time.py` & `agate-1.9.1/agate/data_types/date_time.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/data_types/number.py` & `agate-1.9.1/agate/data_types/number.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,16 +39,19 @@
         self.currency_symbols = currency_symbols
 
         # Suppress Babel warning on Python 3.6
         # See #665
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
 
-            self.group_symbol = group_symbol or self.locale.number_symbols.get('group', ',')
-            self.decimal_symbol = decimal_symbol or self.locale.number_symbols.get('decimal', '.')
+            # Babel 2.14 support.
+            # https://babel.pocoo.org/en/latest/changelog.html#possibly-backwards-incompatible-changes
+            number_symbols = self.locale.number_symbols.get('latn', self.locale.number_symbols)
+            self.group_symbol = group_symbol or number_symbols.get('group', ',')
+            self.decimal_symbol = decimal_symbol or number_symbols.get('decimal', '.')
 
     def cast(self, d):
         """
         Cast a single value to a :class:`decimal.Decimal`.
 
         :returns:
             :class:`decimal.Decimal` or :code:`None`.
```

### Comparing `agate-1.9.0/agate/data_types/text.py` & `agate-1.9.1/agate/data_types/text.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/data_types/time_delta.py` & `agate-1.9.1/agate/data_types/time_delta.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/exceptions.py` & `agate-1.9.1/agate/exceptions.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/fixed.py` & `agate-1.9.1/agate/fixed.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/mapped_sequence.py` & `agate-1.9.1/agate/mapped_sequence.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/rows.py` & `agate-1.9.1/agate/rows.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/__init__.py` & `agate-1.9.1/agate/table/__init__.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/aggregate.py` & `agate-1.9.1/agate/table/aggregate.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/bar_chart.py` & `agate-1.9.1/agate/table/bar_chart.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/bins.py` & `agate-1.9.1/agate/table/bins.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/column_chart.py` & `agate-1.9.1/agate/table/column_chart.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/compute.py` & `agate-1.9.1/agate/table/compute.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/denormalize.py` & `agate-1.9.1/agate/table/denormalize.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/distinct.py` & `agate-1.9.1/agate/table/distinct.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/from_csv.py` & `agate-1.9.1/agate/table/from_csv.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/from_fixed.py` & `agate-1.9.1/agate/table/from_fixed.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/from_json.py` & `agate-1.9.1/agate/table/from_json.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/from_object.py` & `agate-1.9.1/agate/table/from_object.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/group_by.py` & `agate-1.9.1/agate/table/group_by.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/homogenize.py` & `agate-1.9.1/agate/table/homogenize.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/join.py` & `agate-1.9.1/agate/table/join.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/limit.py` & `agate-1.9.1/agate/table/limit.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/line_chart.py` & `agate-1.9.1/agate/table/line_chart.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/merge.py` & `agate-1.9.1/agate/table/merge.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/normalize.py` & `agate-1.9.1/agate/table/normalize.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/order_by.py` & `agate-1.9.1/agate/table/order_by.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/pivot.py` & `agate-1.9.1/agate/table/pivot.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/print_bars.py` & `agate-1.9.1/agate/table/print_bars.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/print_html.py` & `agate-1.9.1/agate/table/print_html.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/print_structure.py` & `agate-1.9.1/agate/table/print_structure.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/print_table.py` & `agate-1.9.1/agate/table/print_table.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/rename.py` & `agate-1.9.1/agate/table/rename.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/scatterplot.py` & `agate-1.9.1/agate/table/scatterplot.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/select.py` & `agate-1.9.1/agate/table/select.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/to_csv.py` & `agate-1.9.1/agate/table/to_csv.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/to_json.py` & `agate-1.9.1/agate/table/to_json.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/table/where.py` & `agate-1.9.1/agate/table/where.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/__init__.py` & `agate-1.9.1/agate/tableset/__init__.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/aggregate.py` & `agate-1.9.1/agate/tableset/aggregate.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/bar_chart.py` & `agate-1.9.1/agate/tableset/bar_chart.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/column_chart.py` & `agate-1.9.1/agate/tableset/column_chart.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/from_csv.py` & `agate-1.9.1/agate/tableset/from_csv.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/from_json.py` & `agate-1.9.1/agate/tableset/from_json.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/having.py` & `agate-1.9.1/agate/tableset/having.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/line_chart.py` & `agate-1.9.1/agate/tableset/line_chart.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/merge.py` & `agate-1.9.1/agate/tableset/merge.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/print_structure.py` & `agate-1.9.1/agate/tableset/print_structure.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/proxy_methods.py` & `agate-1.9.1/agate/tableset/proxy_methods.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/scatterplot.py` & `agate-1.9.1/agate/tableset/scatterplot.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/tableset/to_json.py` & `agate-1.9.1/agate/tableset/to_json.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/testcase.py` & `agate-1.9.1/agate/testcase.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/type_tester.py` & `agate-1.9.1/agate/type_tester.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/utils.py` & `agate-1.9.1/agate/utils.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate/warns.py` & `agate-1.9.1/agate/warns.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/agate.egg-info/PKG-INFO` & `agate-1.9.1/agate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agate
-Version: 1.9.0
+Version: 1.9.1
 Summary: A data analysis library that is optimized for humans instead of machines.
 Home-page: https://agate.readthedocs.org/
 Author: Christopher Groskopf
 Author-email: chrisgroskopf@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/wireservice/agate
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `agate-1.9.0/agate.egg-info/SOURCES.txt` & `agate-1.9.1/agate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/benchmarks/test_joins.py` & `agate-1.9.1/benchmarks/test_joins.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/charts.py` & `agate-1.9.1/charts.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/Makefile` & `agate-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/about.rst` & `agate-1.9.1/docs/about.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/api/aggregations.rst` & `agate-1.9.1/docs/api/aggregations.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/api/computations.rst` & `agate-1.9.1/docs/api/computations.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/api/csv.rst` & `agate-1.9.1/docs/api/csv.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/api/data_types.rst` & `agate-1.9.1/docs/api/data_types.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/api/fixed.rst` & `agate-1.9.1/docs/api/fixed.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/api/table.rst` & `agate-1.9.1/docs/api/table.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/api/tableset.rst` & `agate-1.9.1/docs/api/tableset.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/conf.py` & `agate-1.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 sys.path.insert(0, os.path.abspath('..'))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'agate'
 copyright = '2017, Christopher Groskopf'
-version = '1.9.0'
+version = '1.9.1'
 release = version
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autosummary',
```

### Comparing `agate-1.9.0/docs/contributing.rst` & `agate-1.9.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/charting.rst` & `agate-1.9.1/docs/cookbook/charting.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/columns.rst` & `agate-1.9.1/docs/cookbook/columns.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/compute.rst` & `agate-1.9.1/docs/cookbook/compute.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/create.rst` & `agate-1.9.1/docs/cookbook/create.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/datetime.rst` & `agate-1.9.1/docs/cookbook/datetime.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/excel.rst` & `agate-1.9.1/docs/cookbook/excel.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/filter.rst` & `agate-1.9.1/docs/cookbook/filter.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/homogenize.rst` & `agate-1.9.1/docs/cookbook/homogenize.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/locale.rst` & `agate-1.9.1/docs/cookbook/locale.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/lookup.rst` & `agate-1.9.1/docs/cookbook/lookup.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/r.rst` & `agate-1.9.1/docs/cookbook/r.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/rank.rst` & `agate-1.9.1/docs/cookbook/rank.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/remove.rst` & `agate-1.9.1/docs/cookbook/remove.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/save.rst` & `agate-1.9.1/docs/cookbook/save.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/search.rst` & `agate-1.9.1/docs/cookbook/search.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/sort.rst` & `agate-1.9.1/docs/cookbook/sort.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/sql.rst` & `agate-1.9.1/docs/cookbook/sql.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/standardize.rst` & `agate-1.9.1/docs/cookbook/standardize.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/statistics.rst` & `agate-1.9.1/docs/cookbook/statistics.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/transform.rst` & `agate-1.9.1/docs/cookbook/transform.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook/underscore.rst` & `agate-1.9.1/docs/cookbook/underscore.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/cookbook.rst` & `agate-1.9.1/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/extensions.rst` & `agate-1.9.1/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/images/bar_chart.svg` & `agate-1.9.1/docs/images/bar_chart.svg`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/images/column_chart.svg` & `agate-1.9.1/docs/images/column_chart.svg`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/images/dots_chart.svg` & `agate-1.9.1/docs/images/dots_chart.svg`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/images/lattice.svg` & `agate-1.9.1/docs/images/lattice.svg`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/images/line_chart.svg` & `agate-1.9.1/docs/images/line_chart.svg`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/index.rst` & `agate-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/install.rst` & `agate-1.9.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/docs/release_process.rst` & `agate-1.9.1/docs/release_process.rst`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/example.py` & `agate-1.9.1/example.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/example.py.ipynb` & `agate-1.9.1/example.py.ipynb`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/examples/realdata/Datagov_FY10_EDU_recp_by_State.csv` & `agate-1.9.1/examples/realdata/Datagov_FY10_EDU_recp_by_State.csv`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/examples/realdata/exonerations-20150828.csv` & `agate-1.9.1/examples/realdata/exonerations-20150828.csv`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/examples/realdata/ks_1033_data.csv` & `agate-1.9.1/examples/realdata/ks_1033_data.csv`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/examples/test.json` & `agate-1.9.1/examples/test.json`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/examples/test_key.json` & `agate-1.9.1/examples/test_key.json`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/examples/test_keyed.json` & `agate-1.9.1/examples/test_keyed.json`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/examples/test_non_string_keyed.json` & `agate-1.9.1/examples/test_non_string_keyed.json`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/examples/test_tableset.json` & `agate-1.9.1/examples/test_tableset.json`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/exonerations.py` & `agate-1.9.1/exonerations.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/setup.py` & `agate-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='agate',
-    version='1.9.0',
+    version='1.9.1',
     description='A data analysis library that is optimized for humans instead of machines.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Christopher Groskopf',
     author_email='chrisgroskopf@gmail.com',
     url='https://agate.readthedocs.org/',
     project_urls={
```

### Comparing `agate-1.9.0/tests/test_aggregations.py` & `agate-1.9.1/tests/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_columns.py` & `agate-1.9.1/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_computations.py` & `agate-1.9.1/tests/test_computations.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_data_types.py` & `agate-1.9.1/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_fixed.py` & `agate-1.9.1/tests/test_fixed.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_from_json.py` & `agate-1.9.1/tests/test_from_json.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_mapped_sequence.py` & `agate-1.9.1/tests/test_mapped_sequence.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_py3.py` & `agate-1.9.1/tests/test_py3.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/__init__.py` & `agate-1.9.1/tests/test_table/__init__.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_aggregate.py` & `agate-1.9.1/tests/test_table/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_bins.py` & `agate-1.9.1/tests/test_table/test_bins.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_charting.py` & `agate-1.9.1/tests/test_table/test_charting.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_compute.py` & `agate-1.9.1/tests/test_table/test_compute.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_denormalize.py` & `agate-1.9.1/tests/test_table/test_denormalize.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_from_csv.py` & `agate-1.9.1/tests/test_table/test_from_csv.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_group_by.py` & `agate-1.9.1/tests/test_table/test_group_by.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_homogenize.py` & `agate-1.9.1/tests/test_table/test_homogenize.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_join.py` & `agate-1.9.1/tests/test_table/test_join.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_merge.py` & `agate-1.9.1/tests/test_table/test_merge.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_normalize.py` & `agate-1.9.1/tests/test_table/test_normalize.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_order_py.py` & `agate-1.9.1/tests/test_table/test_order_py.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_pivot.py` & `agate-1.9.1/tests/test_table/test_pivot.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_print_bars.py` & `agate-1.9.1/tests/test_table/test_print_bars.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_print_html.py` & `agate-1.9.1/tests/test_table/test_print_html.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_print_structure.py` & `agate-1.9.1/tests/test_table/test_print_structure.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_print_table.py` & `agate-1.9.1/tests/test_table/test_print_table.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_rename.py` & `agate-1.9.1/tests/test_table/test_rename.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_to_csv.py` & `agate-1.9.1/tests/test_table/test_to_csv.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_table/test_to_json.py` & `agate-1.9.1/tests/test_table/test_to_json.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_tableset/__init__.py` & `agate-1.9.1/tests/test_tableset/__init__.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_tableset/test_aggregate.py` & `agate-1.9.1/tests/test_tableset/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_tableset/test_charting.py` & `agate-1.9.1/tests/test_tableset/test_charting.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_tableset/test_having.py` & `agate-1.9.1/tests/test_tableset/test_having.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_tableset/test_merge.py` & `agate-1.9.1/tests/test_tableset/test_merge.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_type_tester.py` & `agate-1.9.1/tests/test_type_tester.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tests/test_utils.py` & `agate-1.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `agate-1.9.0/tutorial.ipynb` & `agate-1.9.1/tutorial.ipynb`

 * *Files identical despite different names*

