# Comparing `tmp/PFlowC-1.3.0.tar.gz` & `tmp/PFlowC-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-1.3.0.tar", last modified: Sun Apr 28 08:38:21 2024, max compression
+gzip compressed data, was "PFlowC-1.4.0.tar", last modified: Sun Apr 28 09:25:23 2024, max compression
```

## Comparing `PFlowC-1.3.0.tar` & `PFlowC-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.881882 PFlowC-1.3.0/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.879972 PFlowC-1.3.0/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      325 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       71 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        6 2024-04-28 08:38:21.000000 PFlowC-1.3.0/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 08:38:21.881671 PFlowC-1.3.0/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      223 2024-04-28 08:38:02.000000 PFlowC-1.3.0/README.rst
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.880290 PFlowC-1.3.0/pflow/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      111 2024-04-28 08:36:00.000000 PFlowC-1.3.0/pflow/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1523 2024-04-28 08:35:55.000000 PFlowC-1.3.0/pflow/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      725 2024-04-28 08:11:00.000000 PFlowC-1.3.0/pflow/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.880773 PFlowC-1.3.0/pflow/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.3.0/pflow/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3785 2024-04-28 06:00:02.000000 PFlowC-1.3.0/pflow/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 08:38:21.881217 PFlowC-1.3.0/pflow/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.3.0/pflow/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1890 2022-12-03 21:50:12.000000 PFlowC-1.3.0/pflow/utils/logger.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 08:38:21.881924 PFlowC-1.3.0/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2335 2024-04-28 08:36:46.000000 PFlowC-1.3.0/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.884977 PFlowC-1.4.0/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.882795 PFlowC-1.4.0/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 08:53:56.000000 PFlowC-1.4.0/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1888 2024-04-28 09:25:09.000000 PFlowC-1.4.0/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      725 2024-04-28 08:11:00.000000 PFlowC-1.4.0/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.883851 PFlowC-1.4.0/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.0/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     4612 2024-04-28 09:23:45.000000 PFlowC-1.4.0/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.884272 PFlowC-1.4.0/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.0/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.0/PFlowC/utils/logger.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.883517 PFlowC-1.4.0/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      332 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 09:25:23.884748 PFlowC-1.4.0/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      223 2024-04-28 08:38:02.000000 PFlowC-1.4.0/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:25:23.885018 PFlowC-1.4.0/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2344 2024-04-28 08:47:29.000000 PFlowC-1.4.0/setup.py
```

### Comparing `PFlowC-1.3.0/PFlowC.egg-info/PKG-INFO` & `PFlowC-1.4.0/PFlowC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.3.0
+Version: 1.4.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PFlowC-1.3.0/PKG-INFO` & `PFlowC-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.3.0
+Version: 1.4.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PFlowC-1.3.0/pflow/main.py` & `PFlowC-1.4.0/PFlowC/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,29 +7,41 @@
 @disc:
 ======================================="""
 import json
 import logging
 import os
 
 import click
-from pflow import get_version
 
-from pflow.proxy_helper.macosx import set_web_proxy, set_cmd_proxy
-from pflow.utils import logger
+from PFlowC import get_version
+from PFlowC.proxy_helper.macosx import set_web_proxy, set_cmd_proxy, stop_web_proxy
+from PFlowC.utils import logger
+
+home_dir = os.path.expanduser("~/.PFlowC")
+config_fp = os.path.join(home_dir, "config.json")
+log_dir = os.path.join(home_dir, "logs")
+logger.init("PFlowC", console_level=logging.INFO, log_dir=log_dir)
 
-print(get_version())
 
+@click.group(
+    help="Command line interface for Proxy Flow Controller with basic auto configurations.\nVersion: {}".format(
+        get_version()))
+def main():
+    pass
 
 
+@main.command(help="Version")
+def version():
+    print(get_version())
 
-@click.command(help="Command line interface for FlowPilot")
-def main():
-    config_fp = os.path.expanduser("~/.flowPilot/config.json")
+
+@main.command(help="Run proxy flow controller.")
+def on():
     if not os.path.isfile(config_fp):
-        click.echo("upstream config file: {} does not exist.".format(config_fp))
+        logging.warning("upstream config file: {} does not exist.".format(config_fp))
         host = click.prompt("Input the proxy upstream host")
         port = click.prompt("Input the proxy upstream port")
         config = {"host": host, "port": port, "bypass_domains": [
             "127.0.0.1",
             "192.168.0.0/16",
             "172.16.0.0/16",
             "10.0.0.0/8"
@@ -43,10 +55,14 @@
     port = config["port"]
     ignores_list = config["bypass_domains"]
     bypass_domains = list(set(ignores_list))
     set_web_proxy(host, port, bypass_domains)
     set_cmd_proxy(host, port, bypass_domains)
 
 
+@main.command()
+def off():
+    stop_web_proxy()
+
+
 if __name__ == '__main__':
-    logger.init("FlowPilot", console_level=logging.INFO)
     main()
```

### Comparing `PFlowC-1.3.0/pflow/proxy.py` & `PFlowC-1.4.0/PFlowC/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.3.0/pflow/proxy_helper/macosx.py` & `PFlowC-1.4.0/PFlowC/proxy_helper/macosx.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,29 +68,49 @@
                 res.append(service)
         return res
     except subprocess.CalledProcessError as e:
         print(f"Error: {e}")
         return []
 
 
-def set_web_proxy(host, port: int, bypass_domains: list[str]):
+def set_web_proxy(host, port, bypass_domains: list[str]):
     """
     Apply the settings using 'networksetup'
     :param host:
     :param port:
     :param bypass_domains:
     :return:
     """
     # 利用 networksetup的 -listallnetworkservices 参数来获取并自动遍历出 networservices.
     network_services = get_network_services()
     logging.info(f"network services:{network_services}")
     for service in network_services:
         for proxy_type in ["webproxy", "securewebproxy", "socksfirewallproxy"]:
+
+            cmd = ["/usr/sbin/networksetup", "-set" + proxy_type + "state", service, "on"]
+            resp = subprocess.run(cmd, check=True)
+            if resp.returncode != 0:
+                logging.error(f"执行{cmd}时发生异常!")
+
             cmd = ["/usr/sbin/networksetup", "-set" + proxy_type, service, host, str(port)]
             resp = subprocess.run(cmd, check=True)
             if resp.returncode != 0:
                 logging.error(f"执行{cmd}时发生异常!")
         cmd = ["/usr/sbin/networksetup", "-setproxybypassdomains", service, *bypass_domains]
         resp = subprocess.run(cmd)
         if resp.returncode != 0:
             logging.error(f"执行{cmd}时发生异常!")
         logging.info(f"网络[{service}]配置代理成功!")
+
+
+def stop_web_proxy():
+    network_services = get_network_services()
+    logging.info(f"network services:{network_services}")
+    for service in network_services:
+        for proxy_type in ["webproxy", "securewebproxy", "socksfirewallproxy"]:
+
+            cmd = ["/usr/sbin/networksetup", "-set" + proxy_type + "state", service, "off"]
+            resp = subprocess.run(cmd, check=True)
+            if resp.returncode != 0:
+                logging.error(f"执行{cmd}时发生异常!")
+            else:
+                logging.info(f"网络[{service}]代理[{proxy_type}]关闭成功!")
```

### Comparing `PFlowC-1.3.0/pflow/utils/logger.py` & `PFlowC-1.4.0/PFlowC/utils/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import datetime
 import logging
 import os
 
 import colorlog
 
 
-def init(filename, file_level=logging.DEBUG, console_level=logging.INFO):
+def init(filename, file_level=logging.DEBUG, console_level=logging.INFO, log_dir=os.path.join("~", "logs")):
     # 控制台输出不同级别日志颜色设置
     color_config = {
         'DEBUG': 'cyan',
         'INFO': 'green',
         'WARNING': 'yellow',
         'ERROR': 'red',
         'CRITICAL': 'purple',
@@ -32,21 +32,20 @@
     console_handler.setFormatter(colorlog.ColoredFormatter(
         fmt='{log_color:s}[{asctime:s}][{levelname:^7s}][{threadName:s}-{filename:s}:{lineno:d}]: {message:s}',
         log_colors=color_config, style='{'))
     # 指定最低日志级别：（critical > error > warning > info > debug）
     console_handler.setLevel(console_level)
 
     # 输出到文件
-    LOG_DIR = os.path.join(".", "logs")
-    if not os.path.exists(LOG_DIR):
-        os.makedirs(LOG_DIR)
+    if not os.path.exists(log_dir):
+        os.makedirs(log_dir)
     n = datetime.datetime.now()
-    logFilePath = os.path.join(LOG_DIR, f"{filename}-{n.strftime('%Y%m%d%H%M')}.log")
+    logFilePath = os.path.join(log_dir, f"{filename}-{n.strftime('%Y%m%d%H%M')}.log")
     file_handler = logging.FileHandler(filename=logFilePath, mode='a', encoding='utf-8')
     file_handler.setFormatter(
         logging.Formatter(fmt='[{asctime:s}][{levelname:^7s}][{threadName:s}-{filename:s}:{lineno:d}]: {message:s}',
                           style='{', datefmt='%m/%d/%Y %H:%M:%S'))
     # 指定最低日志级别：（critical > error > warning > info > debug）
     file_handler.setLevel(file_level)
 
     logging.basicConfig(level=min(file_level, console_level), handlers=[file_handler, console_handler])
-    logging.debug("日志输出文件：" + logFilePath)
+    logging.debug("日志输出文件：" + logFilePath)
```

### Comparing `PFlowC-1.3.0/setup.py` & `PFlowC-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,21 +34,21 @@
     logging.warning('Fail load requirements file, so using default ones.')
     install_reqs = []
 
 long_description = open('README.rst').read()
 
 setup(
     name='PFlowC',
-    version='1.3.0',
+    version='1.4.0',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
-    packages=["pflow", "pflow.utils", "pflow.proxy_helper"],
+    packages=["PFlowC", "PFlowC.utils", "PFlowC.proxy_helper"],
     install_requires=install_reqs,
     include_package_data=True,
     python_requires='>=3.7',
     long_description=long_description,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
@@ -63,12 +63,12 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     keywords="proxy flow control",
     entry_points={
         'console_scripts': [
-            'pflow-cli=pfc.main:main',
-            'proxy-cli=pfc.proxy:main',
+            'pflow-cli=PFlowC.main:main',
+            'proxy-cli=PFlowC.proxy:main',
         ],
     },
 )
```

