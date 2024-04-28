# Comparing `tmp/PFlowC-1.4.0.tar.gz` & `tmp/PFlowC-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-1.4.0.tar", last modified: Sun Apr 28 09:25:23 2024, max compression
+gzip compressed data, was "PFlowC-1.4.1.tar", last modified: Sun Apr 28 09:33:45 2024, max compression
```

## Comparing `PFlowC-1.4.0.tar` & `PFlowC-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.884977 PFlowC-1.4.0/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.882795 PFlowC-1.4.0/PFlowC/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 08:53:56.000000 PFlowC-1.4.0/PFlowC/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1888 2024-04-28 09:25:09.000000 PFlowC-1.4.0/PFlowC/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      725 2024-04-28 08:11:00.000000 PFlowC-1.4.0/PFlowC/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.883851 PFlowC-1.4.0/PFlowC/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.0/PFlowC/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     4612 2024-04-28 09:23:45.000000 PFlowC-1.4.0/PFlowC/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.884272 PFlowC-1.4.0/PFlowC/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.0/PFlowC/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.0/PFlowC/utils/logger.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:25:23.883517 PFlowC-1.4.0/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      332 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 09:25:23.000000 PFlowC-1.4.0/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 09:25:23.884748 PFlowC-1.4.0/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      223 2024-04-28 08:38:02.000000 PFlowC-1.4.0/README.rst
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:25:23.885018 PFlowC-1.4.0/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2344 2024-04-28 08:47:29.000000 PFlowC-1.4.0/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.971889 PFlowC-1.4.1/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.969759 PFlowC-1.4.1/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:33:42.000000 PFlowC-1.4.1/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1927 2024-04-28 09:29:46.000000 PFlowC-1.4.1/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-1.4.1/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.970883 PFlowC-1.4.1/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.1/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     5857 2024-04-28 09:32:36.000000 PFlowC-1.4.1/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.971328 PFlowC-1.4.1/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.1/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.1/PFlowC/utils/logger.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 09:33:45.970522 PFlowC-1.4.1/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      332 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 09:33:45.000000 PFlowC-1.4.1/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     1138 2024-04-28 09:33:45.971703 PFlowC-1.4.1/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      223 2024-04-28 08:38:02.000000 PFlowC-1.4.1/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 09:33:45.971924 PFlowC-1.4.1/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2344 2024-04-28 09:33:35.000000 PFlowC-1.4.1/setup.py
```

### Comparing `PFlowC-1.4.0/PFlowC/main.py` & `PFlowC-1.4.1/PFlowC/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 import logging
 import os
 
 import click
 
 from PFlowC import get_version
-from PFlowC.proxy_helper.macosx import set_web_proxy, set_cmd_proxy, stop_web_proxy
+from PFlowC.proxy_helper.macosx import set_web_proxy, set_cmd_proxy, stop_web_proxy, clear_cmd_proxy
 from PFlowC.utils import logger
 
 home_dir = os.path.expanduser("~/.PFlowC")
 config_fp = os.path.join(home_dir, "config.json")
 log_dir = os.path.join(home_dir, "logs")
 logger.init("PFlowC", console_level=logging.INFO, log_dir=log_dir)
 
@@ -58,11 +58,12 @@
     set_web_proxy(host, port, bypass_domains)
     set_cmd_proxy(host, port, bypass_domains)
 
 
 @main.command()
 def off():
     stop_web_proxy()
+    clear_cmd_proxy()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `PFlowC-1.4.0/PFlowC/proxy.py` & `PFlowC-1.4.1/PFlowC/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 
-from pfc.utils.proxy_helper.macosx import set_web_proxy, set_cmd_proxy
+from PFlowC.proxy_helper.macosx import set_web_proxy, set_cmd_proxy
 
 
 @click.command
 @click.option("--host", "-h", default="127.0.0.1", help="The host address of the proxy")
 @click.option("--port", "-p", default=8080, help="The port of the proxy")
 @click.option("--socks_port", "-s", default=8090, help="The port of the socks server")
 @click.option("--bypass-domains", type=list, default=['127.0.0.1', "192.168.0.0/16"],
```

### Comparing `PFlowC-1.4.0/PFlowC/proxy_helper/macosx.py` & `PFlowC-1.4.1/PFlowC/proxy_helper/macosx.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 @Software: PyCharm
 @disc:
 ======================================="""
 import logging
 import subprocess
 import os
 
+env_rc_files: list[str] = [".zshrc", ".bashrc"]
 
-def set_cmd_proxy(host, port, bypass_domains: list[str], env_rc_files: list[str] = [".zshrc", ".bashrc"]):
+
+def set_cmd_proxy(host, port, bypass_domains: list[str]):
     # 新的代理服务器设置
     http_proxy_url = "http://{}:{}".format(host, port)
     https_proxy_url = "http://{}:{}".format(host, port)
     no_proxy_domains = ",".join(bypass_domains)
     for env_rc_file in env_rc_files:
         # 要编辑的文件路径
         env_rc_fp = os.path.expanduser(f"~/{env_rc_file}")
@@ -34,27 +36,61 @@
                             ("http_proxy=" in line)
                             or ("https_proxy=" in line)
                             or ("no_proxy=" in line)
                     ):
                         updated_lines.append(line)
 
                 # 添加新的代理设置
-                updated_lines.append("\n# 更新代理设置\n")
                 updated_lines.append(f"export http_proxy=\"{http_proxy_url}\"\n")
                 updated_lines.append(f"export https_proxy=\"{https_proxy_url}\"\n")
                 updated_lines.append(f"export no_proxy=\"{no_proxy_domains}\"\n")
 
                 # 将更新后的行重写回文件
                 zshrc_file.seek(0)
                 zshrc_file.truncate()
                 zshrc_file.writelines(updated_lines)
 
             logging.info(f"代理设置已在{env_rc_file}文件中更新，请运行 'source ~/{env_rc_file}' 以应用新的环境变量设置。")
 
 
+def clear_cmd_proxy():
+    for env_rc_file in env_rc_files:
+        # 要编辑的文件路径
+        env_rc_fp = os.path.expanduser(f"~/{env_rc_file}")
+
+        # 检查并读取文件内容
+        if not os.path.isfile(env_rc_fp):
+            pass
+        else:
+            with open(env_rc_fp, "r+") as zshrc_file:
+                lines = zshrc_file.readlines()
+                updated_lines = []
+
+                # 查找并移除旧的代理设置
+                for line in lines:
+                    if not (
+                            ("http_proxy=" in line)
+                            or ("https_proxy=" in line)
+                            or ("no_proxy=" in line)
+                    ):
+                        updated_lines.append(line)
+
+                # 添加新的代理设置
+                updated_lines.append("export http_proxy=\"\"\n")
+                updated_lines.append("export https_proxy=\"\"\n")
+                updated_lines.append("export no_proxy=\"\"\n")
+
+                # 将更新后的行重写回文件
+                zshrc_file.seek(0)
+                zshrc_file.truncate()
+                zshrc_file.writelines(updated_lines)
+
+            logging.info(f"已清理在{env_rc_file}文件中的代理配置，请运行 'source ~/{env_rc_file}' 使其改变生效.")
+
+
 def get_network_services():
     """
     利用 networksetup的 -listallnetworkservices 参数来获取并自动遍历出 networservices.
     """
 
     try:
         # 调用networksetup命令并使用-listallnetworkservices选项来列出所有网络服务
```

### Comparing `PFlowC-1.4.0/PFlowC/utils/logger.py` & `PFlowC-1.4.1/PFlowC/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.0/PFlowC.egg-info/PKG-INFO` & `PFlowC-1.4.1/PFlowC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.4.0
+Version: 1.4.1
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PFlowC-1.4.0/PKG-INFO` & `PFlowC-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 1.4.0
+Version: 1.4.1
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PFlowC-1.4.0/setup.py` & `PFlowC-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     logging.warning('Fail load requirements file, so using default ones.')
     install_reqs = []
 
 long_description = open('README.rst').read()
 
 setup(
     name='PFlowC',
-    version='1.4.0',
+    version='1.4.1',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
     packages=["PFlowC", "PFlowC.utils", "PFlowC.proxy_helper"],
     install_requires=install_reqs,
```

