# Comparing `tmp/mini_toolbox-1.0.2.tar.gz` & `tmp/mini_toolbox-1.0.3.tar.gz`

## Comparing `mini_toolbox-1.0.2.tar` & `mini_toolbox-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/.gitignore
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/LICENSE
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/README.md
--rwxr-xr-x   0        0        0     2064 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/build.sh
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/docs/.readthedocs.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/docs/Makefile
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/docs/source/conf.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/docs/source/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/docs/source/_static/favicon.png
--rw-r--r--   0        0        0    23723 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/docs/source/_static/logo.png
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/__init__.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/api_json.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/archive.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/config.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/crypt.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/dingtalk.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/extra.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/ftp.py
--rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/git.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/hash.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/jenkins.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/jfrog.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/logger.py
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/mail.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/mysql.py
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/path.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/pip_list.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/recoding.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/ssh.py
--rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/svn.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/utils.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/xlsx.py
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/xml.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/alpha/__init__.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/alpha/mini_server.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/mini_toolbox/useless/__init__.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/tests/test_haha.py
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 mini_toolbox-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/LICENSE
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/README.md
+-rwxr-xr-x   0        0        0     2064 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/build.sh
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/docs/Makefile
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/docs/source/conf.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/docs/source/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/docs/source/_static/favicon.png
+-rw-r--r--   0        0        0    23723 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/docs/source/_static/logo.png
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/__init__.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/api_json.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/archive.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/config.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/crypt.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/dingtalk.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/extra.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/ftp.py
+-rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/git.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/hash.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/jenkins.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/jfrog.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/logger.py
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/mail.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/mysql.py
+-rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/path.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/pip_list.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/recoding.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/ssh.py
+-rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/svn.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/utils.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/xlsx.py
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/xml.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/alpha/__init__.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/alpha/mini_server.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/mini_toolbox/useless/__init__.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/tests/test_haha.py
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 mini_toolbox-1.0.3/PKG-INFO
```

### Comparing `mini_toolbox-1.0.2/.gitignore` & `mini_toolbox-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/CHANGELOG.md` & `mini_toolbox-1.0.3/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 ## v1.1.0 (2024-04-xx) (ing)
 ```shell
 # Deprecated
     - None
 # Changed
     - 调整update_obj方法为update_json
     - 调整_Dict2Obj对象为_Dict2Object
+    - 调整文本编码解析工具, 更换chardet为charamel
 # Added
     - 新增_Dict2Object类__str__方法, 用于格式化打印数据对象
     - 新增_Dict2Object类obj2dict方法, 用于将对象转化数据字典
     - 新增update_obj方法, 用于更新_Dict2Object数据对象
     - 新增update_json方法, 用于增/改/查json数据文件, 返回_Dict2Object数据对象
 # Fixed
     - 修复rtd-docs部分模块生成失败问题
     - 调整可选依赖相关组件及安装说明
+    - 修复jenkins日志编码解析不准确问题
 ```
 
 ## v1.0.0 (2024-03-29) (推荐)
 ```shell
 # Deprecated
     - None
 # Changed
```

### Comparing `mini_toolbox-1.0.2/LICENSE` & `mini_toolbox-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/README.md` & `mini_toolbox-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/build.sh` & `mini_toolbox-1.0.3/build.sh`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/pyproject.toml` & `mini_toolbox-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'mini_toolbox'
-version = '1.0.2'
+version = '1.0.3'
 authors = [{ name = 'gnzhoutian', email = 'gnzhoutian@qq.com' }]
 description = 'Python迷你工具箱，包含简化的常用工具，旨在帮助脚本快速开发。'
 keywords = ['tools', 'toolbox', 'mini-tools', 'mini-toolbox']
 readme = 'README.md'
 requires-python = '>=3.6'
 classifiers = [
     'Development Status :: 4 - Beta',
@@ -31,15 +31,15 @@
     'pip >= 19.0.0',           # base
     'setuptools >= 39.0.0',    # base
     'wheel',                   # base
     'requests >= 2.20.0',      # for api_json and dingtalk
     'pymysql',                 # for mysql
     'pyartifactory >= 1.11.0', # for jfrog
     'jenkinsapi',              # for jenkins
-    'chardet == 3.0.4',        # for jenkins
+    'charamel',                # for jenkins
     'python-gitlab',           # for git
     'paramiko',                # for ssh
     'openpyxl',                # for xlsx
     'xlrd == 1.2.0',           # for xlsx
     'rsa >= 4.5',              # for crypt
     'pydes',                   # for crypt
     'lxml',                    # for xml
```

### Comparing `mini_toolbox-1.0.2/.vscode/settings.json` & `mini_toolbox-1.0.3/.vscode/settings.json`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         ".pytest_cache": true,
         ".coverage": true,
         // less edit
         "LICENSE": true,
         ".gitignore": true,
         "build.sh": true,
         "docs": true,
-        "pyproject.toml": true,
+        // "pyproject.toml": true,
         // "README.md": true,
         // final
         // "mini_toolbox/alpha": true,
         // "mini_toolbox/useless": true,
         // "mini_toolbox/__init__.py": true,
         // "mini_toolbox/xml.py": true,
         // "mini_toolbox/xlsx.py": true,
```

### Comparing `mini_toolbox-1.0.2/docs/Makefile` & `mini_toolbox-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/docs/source/conf.py` & `mini_toolbox-1.0.3/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 sys.path.insert(0, os.path.abspath("../.."))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 # The full version, including alpha/beta/rc tags.
-release = '1.0.2'
+release = '1.0.3'
 
 project = 'Python迷你工具箱'
 author = 'gnzhoutian'
 copyright = '2024, {}, 文档版本 {}, Python 3.6+'.format(author, release)
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
```

### Comparing `mini_toolbox-1.0.2/docs/source/_static/logo.png` & `mini_toolbox-1.0.3/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/api_json.py` & `mini_toolbox-1.0.3/mini_toolbox/api_json.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/archive.py` & `mini_toolbox-1.0.3/mini_toolbox/archive.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/config.py` & `mini_toolbox-1.0.3/mini_toolbox/config.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/crypt.py` & `mini_toolbox-1.0.3/mini_toolbox/crypt.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/dingtalk.py` & `mini_toolbox-1.0.3/mini_toolbox/dingtalk.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/extra.py` & `mini_toolbox-1.0.3/mini_toolbox/extra.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/ftp.py` & `mini_toolbox-1.0.3/mini_toolbox/ftp.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/git.py` & `mini_toolbox-1.0.3/mini_toolbox/git.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/hash.py` & `mini_toolbox-1.0.3/mini_toolbox/hash.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/jenkins.py` & `mini_toolbox-1.0.3/mini_toolbox/jenkins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # """ 用于jenkins相关操作 """
 
 __all__ = ['JenkinsTools']
 
 import time
-import chardet
+import charamel
 from jenkinsapi.jenkins import Jenkins
 from typing import Optional
 from .logger import logger
 
 
 class JenkinsTools():
     """ 用于jenkins相关操作, 支持token
@@ -18,14 +18,15 @@
         user (str): 用户名
         token (str): 用户密码, 建议使用token
         server (str): jenkins服务器地址
     """
 
     def __init__(self, user: str, token: str, server: str):
         self.jenkins = Jenkins(baseurl=server, username=user, password=token, timeout=10)
+        self.chardet = None
 
     def build_job(self, job_name: str, params: Optional[dict] = None, poll: int = 20, bg=False, ccu=True) -> tuple:
         """ 调用执行job, 返回任务执行的状态信息
         
         Args: 
             job_name (str): jenkins的job名称
             params (Optional[dict]): 用于参数化构建, 键值与job变量取交集生效
@@ -98,20 +99,21 @@
 
         build_status = build_task.get_status()
         build_url = build_task.get_build_url() + 'console'
         build_log = None
 
         if build_status is not None:
             build_log = build_task.get_console().encode('ISO-8859-1', errors=errors)
+            if not self.chardet:
+                self.chardet = charamel.Detector()
             if not encoding:
-                encoding = chardet.detect(build_log)['encoding'] or 'utf-8'  # 自动解码失败时默认使用utf-8解码
+                encoding = self.chardet.detect(build_log)
             build_log = build_log.decode(encoding, errors=errors)
-
             logger.debug('任务执行状态: {} 任务地址: {}'.format(build_status, build_url))
-            logger.debug('任务执行日志: {}'.format(build_log))
+            logger.debug('任务日志编码: {} 详细日志: {}'.format(encoding, build_log))
 
         return (build_status, build_url, build_log)
 
     def has_job(self, job_name: str) -> bool:
         """ 返回任务执行的状态信息
         
         Args:
```

### Comparing `mini_toolbox-1.0.2/mini_toolbox/jfrog.py` & `mini_toolbox-1.0.3/mini_toolbox/jfrog.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/logger.py` & `mini_toolbox-1.0.3/mini_toolbox/logger.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/mail.py` & `mini_toolbox-1.0.3/mini_toolbox/mail.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/mysql.py` & `mini_toolbox-1.0.3/mini_toolbox/mysql.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/path.py` & `mini_toolbox-1.0.3/mini_toolbox/path.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/pip_list.py` & `mini_toolbox-1.0.3/mini_toolbox/pip_list.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/recoding.py` & `mini_toolbox-1.0.3/mini_toolbox/recoding.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/ssh.py` & `mini_toolbox-1.0.3/mini_toolbox/ssh.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/svn.py` & `mini_toolbox-1.0.3/mini_toolbox/svn.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/utils.py` & `mini_toolbox-1.0.3/mini_toolbox/utils.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/xlsx.py` & `mini_toolbox-1.0.3/mini_toolbox/xlsx.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/xml.py` & `mini_toolbox-1.0.3/mini_toolbox/xml.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/mini_toolbox/alpha/mini_server.py` & `mini_toolbox-1.0.3/mini_toolbox/alpha/mini_server.py`

 * *Files identical despite different names*

### Comparing `mini_toolbox-1.0.2/PKG-INFO` & `mini_toolbox-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-toolbox
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python迷你工具箱，包含简化的常用工具，旨在帮助脚本快速开发。
 Project-URL: Changelog, https://mini-toolbox.readthedocs.io/zh/latest//CHANGELOG.html
 Project-URL: Documentation, https://mini-toolbox.readthedocs.io/zh/latest/
 Project-URL: Homepage, https://pypi.org/project/mini-toolbox
 Project-URL: Issues, https://github.com/gnzhoutian/mini_toolbox/issues
 Project-URL: Repository, https://github.com/gnzhoutian/mini_toolbox.git
 Author-email: gnzhoutian <gnzhoutian@qq.com>
@@ -27,15 +27,15 @@
 Provides-Extra: docs
 Requires-Dist: myst-parser==0.16.1; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme==1.1.1; extra == 'docs'
 Requires-Dist: sphinx==4.5.0; extra == 'docs'
 Provides-Extra: full
 Requires-Dist: apscheduler; extra == 'full'
 Requires-Dist: beautifulsoup4; extra == 'full'
-Requires-Dist: chardet==3.0.4; extra == 'full'
+Requires-Dist: charamel; extra == 'full'
 Requires-Dist: colorlog; extra == 'full'
 Requires-Dist: jenkinsapi; extra == 'full'
 Requires-Dist: lxml; extra == 'full'
 Requires-Dist: openpyxl; extra == 'full'
 Requires-Dist: paramiko; extra == 'full'
 Requires-Dist: pip>=19.0.0; extra == 'full'
 Requires-Dist: pyartifactory>=1.11.0; extra == 'full'
```

