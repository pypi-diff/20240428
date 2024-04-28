# Comparing `tmp/th-influx-sdk-1.0.5.tar.gz` & `tmp/th-influx-sdk-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th-influx-sdk-1.0.5.tar", last modified: Wed Apr 24 07:06:40 2024, max compression
+gzip compressed data, was "th-influx-sdk-1.0.6.tar", last modified: Sun Apr 28 09:51:23 2024, max compression
```

## Comparing `th-influx-sdk-1.0.5.tar` & `th-influx-sdk-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 07:06:40.884897 th-influx-sdk-1.0.5/
--rw-rw-rw-   0        0        0      300 2024-04-24 07:06:40.883901 th-influx-sdk-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 07:06:40.873926 th-influx-sdk-1.0.5/ThInfluxSDK/
--rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.5/ThInfluxSDK/__init__.py
--rw-rw-rw-   0        0        0    17810 2024-04-24 07:05:50.000000 th-influx-sdk-1.0.5/ThInfluxSDK/influxSDK.py
--rw-rw-rw-   0        0        0       42 2024-04-24 07:06:40.885894 th-influx-sdk-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-24 07:06:35.000000 th-influx-sdk-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:06:40.881906 th-influx-sdk-1.0.5/th_influx_sdk.egg-info/
--rw-rw-rw-   0        0        0      300 2024-04-24 07:06:40.000000 th-influx-sdk-1.0.5/th_influx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-24 07:06:40.000000 th-influx-sdk-1.0.5/th_influx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 07:06:40.000000 th-influx-sdk-1.0.5/th_influx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-24 07:06:40.000000 th-influx-sdk-1.0.5/th_influx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-24 07:06:40.000000 th-influx-sdk-1.0.5/th_influx_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 09:51:23.285783 th-influx-sdk-1.0.6/
+-rw-rw-rw-   0        0        0      300 2024-04-28 09:51:23.282786 th-influx-sdk-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 09:51:23.273827 th-influx-sdk-1.0.6/ThInfluxSDK/
+-rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.6/ThInfluxSDK/__init__.py
+-rw-rw-rw-   0        0        0    18490 2024-04-28 09:48:49.000000 th-influx-sdk-1.0.6/ThInfluxSDK/influxSDK.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 09:51:23.285783 th-influx-sdk-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-04-28 09:49:53.000000 th-influx-sdk-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:51:23.282786 th-influx-sdk-1.0.6/th_influx_sdk.egg-info/
+-rw-rw-rw-   0        0        0      300 2024-04-28 09:51:23.000000 th-influx-sdk-1.0.6/th_influx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-28 09:51:23.000000 th-influx-sdk-1.0.6/th_influx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:51:23.000000 th-influx-sdk-1.0.6/th_influx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-28 09:51:23.000000 th-influx-sdk-1.0.6/th_influx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-28 09:51:23.000000 th-influx-sdk-1.0.6/th_influx_sdk.egg-info/top_level.txt
```

### Comparing `th-influx-sdk-1.0.5/ThInfluxSDK/influxSDK.py` & `th-influx-sdk-1.0.6/ThInfluxSDK/influxSDK.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,34 +234,36 @@
         Dict: 字典，包含查询结果的键值对。
 
     """
     # 将点号列表连接成一个字符串，使用'|'作为分隔符
     point_str = '|'.join(pointList)
 
     # 构建SQL查询语句
-    sql_query = f"SELECT LAST(value), uuid FROM {tableName} WHERE uuid =~ /^{point_str}$/"
+    sql_query = f"SELECT LAST(VALUE), UUID FROM {tableName} WHERE UUID =~ /^{point_str}$/"
 
     # 如果查询时间不为空，则添加时间条件和分组
     if queryTime:
-        sql_query += f" AND time <= '{queryTime}' GROUP BY uuid"
+        sql_query += f" AND time <= '{queryTime}' GROUP BY UUID"
 
-        # 执行查询
+    print(sql_query)
+
+    # 执行查询
     result = influxDB.query(sql_query, database=database)
 
     # 初始化一个有序字典来存储结果
     data_map = OrderedDict()
 
     # 遍历查询结果
     if result.error:
         print("查询出错: ", result.error)
     else:
         series = result.get_points()
         if series:
             for point in series:
-                uuid = point['uuid']
+                uuid = point['UUID']
                 value_obj = point['last']
                 data_map[uuid] = value_obj
 
     return data_map
 
 
 def get_his_set_data_by_complete(database: str, tableName: str, startTime: str, endTime: str, pointList: List[str],
@@ -317,16 +319,36 @@
             uuid_to_add = value
         else:
             uuid_to_add = map_data[uuid]
 
             # 构建结果列表
         result_list.append([time, uuid_to_add, uuid])
 
-        # 转换为JSON字符串
-    to_json_string = json.dumps(result_list)
+    # print(result_list)
+    # 初始化最外层的字典
+    map_all = OrderedDict()
+    if result_list:
+        for item_list in result_list:
+            # 转换UTC时间为北京时间
+            time_beijing = convert_utc_to_beijing_time(item_list[0])
+
+            # 获取或创建当前时间对应的字典
+            map2 = map_all.get(time_beijing)
+            if map2 is None:
+                map2 = OrderedDict()
+                map2["time"] = time_beijing
+                map_all[time_beijing] = map2
+
+            map2[item_list[2]] = item_list[1]
+
+    values_set = []
+    for d in map_all.values():
+        values_set.append(d)
+    # 转换为JSON字符串
+    to_json_string = json.dumps(values_set)
 
     return to_json_string
 
 
 def get_his_set_data(database: str, tableName: str, startTime: str, endTime: str,
                      pointList: List[str], influxDB: InfluxDBClient) -> str:
     """
```

### Comparing `th-influx-sdk-1.0.5/setup.py` & `th-influx-sdk-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name='th-influx-sdk',
-    version='1.0.5',
+    version='1.0.6',
     description='A SDK for influxDb',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='xiongyi',
     author_email='15679191752@163.com',
     packages=find_packages(),
     install_requires=[
```

