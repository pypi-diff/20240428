# Comparing `tmp/pc-perf-1.1.3.tar.gz` & `tmp/pc-perf-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pc-perf-1.1.3.tar", last modified: Tue Apr 23 22:42:58 2024, max compression
+gzip compressed data, was "pc-perf-1.1.4.tar", last modified: Sun Apr 28 13:41:29 2024, max compression
```

## Comparing `pc-perf-1.1.3.tar` & `pc-perf-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 22:42:58.734708 pc-perf-1.1.3/
--rw-rw-rw-   0        0        0    35823 2024-04-20 15:52:03.000000 pc-perf-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      943 2024-04-23 22:42:58.733709 pc-perf-1.1.3/PKG-INFO
--rwxrwxrwx   0        0        0   377856 2024-01-28 09:39:06.000000 pc-perf-1.1.3/PresentMon.exe
--rw-rw-rw-   0        0        0      341 2024-04-20 17:44:37.000000 pc-perf-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 22:42:58.706132 pc-perf-1.1.3/core/
--rw-rw-rw-   0        0        0     2447 2024-04-06 12:27:42.000000 pc-perf-1.1.3/core/monitor.py
--rw-rw-rw-   0        0        0     9574 2024-04-21 07:07:46.000000 pc-perf-1.1.3/core/pc_tools.py
--rw-rw-rw-   0        0        0     6709 2024-04-21 07:37:00.000000 pc-perf-1.1.3/dao.py
--rw-rw-rw-   0        0        0      664 2024-04-21 15:03:50.000000 pc-perf-1.1.3/log.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:42:58.732708 pc-perf-1.1.3/pc_perf.egg-info/
--rw-rw-rw-   0        0        0      943 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      240 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4156 2024-04-21 15:05:37.000000 pc-perf-1.1.3/pc_perf.py
--rw-rw-rw-   0        0        0       42 2024-04-23 22:42:58.734708 pc-perf-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2591 2024-04-23 22:42:38.000000 pc-perf-1.1.3/setup.py
--rw-rw-rw-   0        0        0     1545 2024-04-20 11:36:25.000000 pc-perf-1.1.3/task_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:42:58.706132 pc-perf-1.1.3/test_result/
--rw-rw-rw-   0        0        0    30322 2024-04-20 11:36:25.000000 pc-perf-1.1.3/test_result/index.html
--rw-rw-rw-   0        0        0     2879 2024-04-21 15:04:24.000000 pc-perf-1.1.3/util.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:41:29.126645 pc-perf-1.1.4/
+-rw-rw-rw-   0        0        0    35823 2024-04-20 15:52:03.000000 pc-perf-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      943 2024-04-28 13:41:29.111074 pc-perf-1.1.4/PKG-INFO
+-rwxrwxrwx   0        0        0   377856 2024-01-28 09:39:06.000000 pc-perf-1.1.4/PresentMon.exe
+-rw-rw-rw-   0        0        0     1143 2024-04-28 13:34:36.000000 pc-perf-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 13:41:29.048533 pc-perf-1.1.4/core/
+-rw-rw-rw-   0        0        0     2584 2024-04-28 13:34:36.000000 pc-perf-1.1.4/core/monitor.py
+-rw-rw-rw-   0        0        0    10132 2024-04-28 13:34:36.000000 pc-perf-1.1.4/core/pc_tools.py
+-rw-rw-rw-   0        0        0     6709 2024-04-21 07:37:00.000000 pc-perf-1.1.4/dao.py
+-rw-rw-rw-   0        0        0      664 2024-04-21 15:03:50.000000 pc-perf-1.1.4/log.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:41:29.111074 pc-perf-1.1.4/pc_perf.egg-info/
+-rw-rw-rw-   0        0        0      943 2024-04-28 13:41:28.000000 pc-perf-1.1.4/pc_perf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-28 13:41:28.000000 pc-perf-1.1.4/pc_perf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:41:28.000000 pc-perf-1.1.4/pc_perf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-28 13:41:28.000000 pc-perf-1.1.4/pc_perf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      240 2024-04-28 13:41:28.000000 pc-perf-1.1.4/pc_perf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-28 13:41:28.000000 pc-perf-1.1.4/pc_perf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4156 2024-04-21 15:05:37.000000 pc-perf-1.1.4/pc_perf.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 13:41:29.126645 pc-perf-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2591 2024-04-28 13:35:00.000000 pc-perf-1.1.4/setup.py
+-rw-rw-rw-   0        0        0     1545 2024-04-20 11:36:25.000000 pc-perf-1.1.4/task_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:41:29.095456 pc-perf-1.1.4/test_result/
+-rw-rw-rw-   0        0        0    30322 2024-04-20 11:36:25.000000 pc-perf-1.1.4/test_result/index.html
+-rw-rw-rw-   0        0        0     2879 2024-04-21 15:04:24.000000 pc-perf-1.1.4/util.py
```

### Comparing `pc-perf-1.1.3/LICENSE` & `pc-perf-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.3/PKG-INFO` & `pc-perf-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pc-perf
-Version: 1.1.3
+Version: 1.1.4
 Summary: pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
 Home-page: https://github.com/15525730080/pc_perf
 Author: 范博洲
 Author-email: 15525730080@163.com
 License: MIT
 Keywords: pc fps cpu memory gpu monitor
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pc-perf-1.1.3/PresentMon.exe` & `pc-perf-1.1.4/PresentMon.exe`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.3/core/monitor.py` & `pc-perf-1.1.4/core/monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import csv
 import inspect
 import json
 import time
+import traceback
 from pathlib import Path
 
 from log import log as logger
 
 
 def print_json(data, *args, **kwargs):
     data_json = json.dumps(data)
@@ -54,19 +55,22 @@
             self.key_value = [key.split("(")[0] for key in self.key_value]
 
     async def run(self):
         async for _ in MonitorIter(self.stop_event):
             before_func = time.time()
             param_names = inspect.signature(self.func).parameters.keys()
             params = {name: self.kwargs.get(name) for name in param_names}
-            print(params)
-            res = await self.func(**params)
-            if self.is_out and res:
-                with open(self.csv_path, "a+", encoding="utf-8", newline="") as f:
-                    csv_writer = csv.writer(f)
-                    csv_writer.writerow([res.get(key, "") for key in self.key_value])
-            end_func = time.time()
-            if interval_time := (int(end_func) - int(before_func)) <= 1:
-                await asyncio.sleep(interval_time)
+            try:
+                res = await self.func(**params)
+                if self.is_out and res:
+                    with open(self.csv_path, "a+", encoding="utf-8", newline="") as f:
+                        csv_writer = csv.writer(f)
+                        csv_writer.writerow([res.get(key, "") for key in self.key_value])
+            except:
+                logger.error(traceback.print_exc())
+            finally:
+                end_func = time.time()
+                if interval_time := (int(end_func) - int(before_func)) <= 1:
+                    await asyncio.sleep(interval_time)
 
     def stop(self):
         self.stop_event.clear()
```

### Comparing `pc-perf-1.1.3/core/pc_tools.py` & `pc-perf-1.1.4/core/pc_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 from io import BytesIO
 import psutil
 import pynvml
 from pathlib import Path
 from log import log
 from core.monitor import Monitor
 
+SUPPORT_GPU = True
 try:
     pynvml.nvmlInit()
 except:
     traceback.print_exc()
     log.info("本设备gpu获取不适配")
+    SUPPORT_GPU = False
 from PIL import ImageGrab
 
 
 def print_json(msg):
     log.info(json.dumps(msg))
 
 
@@ -182,51 +184,66 @@
         print_json(memory_info)
         return memory_info
 
     return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
 
 
 async def fps(pid):
+    if platform.system() != "Windows":
+        return {"type": "fps", "time": int(time.time())}
     frames = WinFps(pid).fps()
     if not frames:
         return frames
     res = {"type": "fps", "fps": len(frames), "frames": frames, "time": int(frames[0]) if frames else int(time.time())}
     print_json(res)
     return res
 
 
 async def gpu(pid):
     def real_func(pid):
         pid = int(pid)
         start_time = int(time.time())
-        device_count = pynvml.nvmlDeviceGetCount()
-        res = None
-        for i in range(device_count):
-            handle = pynvml.nvmlDeviceGetHandleByIndex(i)
-            processes = pynvml.nvmlDeviceGetComputeRunningProcesses(handle)
-            for process in processes:
-                print(process)
-                if process.pid == pid:
-                    gpu_Utilization = pynvml.nvmlDeviceGetUtilizationRates(handle)
-                    gpu_utilization_percentage = gpu_Utilization.gpu  # GPU的计算使用率
-                    res = {"gpu": gpu_utilization_percentage, "time": start_time}
-                    print_json(res)
-                    return res
-        return res
+        if SUPPORT_GPU:
+            device_count = pynvml.nvmlDeviceGetCount()
+            res = None
+            for i in range(device_count):
+                handle = pynvml.nvmlDeviceGetHandleByIndex(i)
+                processes = pynvml.nvmlDeviceGetComputeRunningProcesses(handle)
+                for process in processes:
+                    print(process)
+                    if process.pid == pid:
+                        gpu_Utilization = pynvml.nvmlDeviceGetUtilizationRates(handle)
+                        gpu_utilization_percentage = gpu_Utilization.gpu  # GPU的计算使用率
+                        res = {"gpu": gpu_utilization_percentage, "time": start_time}
+                        print_json(res)
+                        return res
+            return res
+        else:
+            return {"time": start_time}
 
     return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
 
 
 async def process_info(pid):
     def real_func(pid):
         start_time = int(time.time())
         process = psutil.Process(int(pid))
-        num_handles = process.num_handles()
-        num_threads = process.num_threads()
-        res = {"num_threads": num_threads, "num_handles": num_handles, "time": start_time}
+        num_handles = None
+        num_threads = None
+        try:
+            num_handles = process.num_handles()
+        except:
+            log.error(traceback.print_exc())
+        try:
+            num_threads = process.num_threads()
+        except:
+            log.error(traceback.print_exc())
+        res = {"time": start_time}
+        if num_handles: res["num_handles"] = num_handles
+        if num_threads: res["num_threads"] = num_threads
         print_json(res)
         return res
 
     return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
 
 
 async def perf(pid, save_dir):
```

### Comparing `pc-perf-1.1.3/dao.py` & `pc-perf-1.1.4/dao.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.3/log.py` & `pc-perf-1.1.4/log.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.3/pc_perf.egg-info/PKG-INFO` & `pc-perf-1.1.4/pc_perf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pc-perf
-Version: 1.1.3
+Version: 1.1.4
 Summary: pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
 Home-page: https://github.com/15525730080/pc_perf
 Author: 范博洲
 Author-email: 15525730080@163.com
 License: MIT
 Keywords: pc fps cpu memory gpu monitor
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pc-perf-1.1.3/pc_perf.py` & `pc-perf-1.1.4/pc_perf.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.3/setup.py` & `pc-perf-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 setup(
     # 包的名称，通常与包的目录名称相同
     name='pc-perf',
 
     # 版本号，遵循语义化版本控制规则
-    version='1.1.3',
+    version='1.1.4',
 
     # 项目简短描述
     description='pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示',
 
     # 项目的URL，通常是项目主页或源代码仓库
     url='https://github.com/15525730080/pc_perf',
```

### Comparing `pc-perf-1.1.3/task_handle.py` & `pc-perf-1.1.4/task_handle.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.3/test_result/index.html` & `pc-perf-1.1.4/test_result/index.html`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.3/util.py` & `pc-perf-1.1.4/util.py`

 * *Files identical despite different names*

