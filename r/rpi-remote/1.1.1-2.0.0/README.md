# Comparing `tmp/rpi-remote-1.1.1.tar.gz` & `tmp/rpi_remote-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi-remote-1.1.1.tar", last modified: Sun Jan  7 14:55:23 2024, max compression
+gzip compressed data, was "rpi_remote-2.0.0.tar", last modified: Sun Apr 28 15:31:47 2024, max compression
```

## Comparing `rpi-remote-1.1.1.tar` & `rpi_remote-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 14:55:23.627213 rpi-remote-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-07 14:54:56.000000 rpi-remote-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-01-07 14:55:23.627213 rpi-remote-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-07 14:54:56.000000 rpi-remote-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-07 14:54:56.000000 rpi-remote-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 14:55:23.623213 rpi-remote-1.1.1/rpi_remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 14:54:56.000000 rpi-remote-1.1.1/rpi_remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-01-07 14:54:56.000000 rpi-remote-1.1.1/rpi_remote/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-01-07 14:54:56.000000 rpi-remote-1.1.1/rpi_remote/rpi_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 14:55:23.627213 rpi-remote-1.1.1/rpi_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-01-07 14:55:23.000000 rpi-remote-1.1.1/rpi_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-07 14:55:23.000000 rpi-remote-1.1.1/rpi_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 14:55:23.000000 rpi-remote-1.1.1/rpi_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-07 14:55:23.000000 rpi-remote-1.1.1/rpi_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-07 14:55:23.000000 rpi-remote-1.1.1/rpi_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-07 14:55:23.000000 rpi-remote-1.1.1/rpi_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 14:55:23.627213 rpi-remote-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:31:47.232153 rpi_remote-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 15:31:24.000000 rpi_remote-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-28 15:31:47.232153 rpi_remote-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-28 15:31:24.000000 rpi_remote-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-28 15:31:24.000000 rpi_remote-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:31:47.232153 rpi_remote-2.0.0/rpi_remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:31:24.000000 rpi_remote-2.0.0/rpi_remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-28 15:31:24.000000 rpi_remote-2.0.0/rpi_remote/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-28 15:31:24.000000 rpi_remote-2.0.0/rpi_remote/rpi_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:31:47.232153 rpi_remote-2.0.0/rpi_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-28 15:31:47.000000 rpi_remote-2.0.0/rpi_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-28 15:31:47.000000 rpi_remote-2.0.0/rpi_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:31:47.000000 rpi_remote-2.0.0/rpi_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-28 15:31:47.000000 rpi_remote-2.0.0/rpi_remote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-28 15:31:47.000000 rpi_remote-2.0.0/rpi_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 15:31:47.000000 rpi_remote-2.0.0/rpi_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:31:47.232153 rpi_remote-2.0.0/setup.cfg
```

### Comparing `rpi-remote-1.1.1/LICENSE` & `rpi_remote-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi-remote-1.1.1/PKG-INFO` & `rpi_remote-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 Metadata-Version: 2.1
 Name: rpi-remote
-Version: 1.1.1
+Version: 2.0.0
 Summary: Rpi remote client
 Author-email: Aron Radics <radics.aron.jozsef@gmail.com>
 Project-URL: Homepage, https://github.com/radaron/rpi_remote_client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: paramiko>=2.12.0
 Requires-Dist: requests>=2.28.1
 Requires-Dist: psutil>=5.8.0
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 ![PyPI - Version](https://img.shields.io/pypi/v/rpi-remote?style=for-the-badge&logo=python&logoColor=yellow&link=https%3A%2F%2Fpypi.org%2Fproject%2Frpi-remote%2F)
 
 # Rpi Remote client
 
 ## Installation
 
-### Prerequisites
-```
-sudo apt install build-essential libffi-dev gcc pkg-config python3-dev python3-pip libssl-dev cargo openssl
-```
-Install rust: https://www.rust-lang.org/tools/install
-
-### Install package
-```
+### Install/Upgrade package
+``` shell
 python3 -m pip install --upgrade rpi-remote --user
 ```
 
 ### Create service
-```
+``` shell
 echo "[Unit]
 Description=rpi_remote service
 After=multi-user.target
 Conflicts=getty@tty1.service
 [Service]
 User=${USER}
 Type=simple
@@ -48,20 +41,32 @@
 Environment="LANG=C.UTF-8"
 ExecStart=${HOME}/.local/bin/rpi-remote
 Restart=on-failure
 RestartSec=3
 [Install]
 WantedBy=multi-user.target" | sudo tee /etc/systemd/system/rpi-remote.service
 ```
-```
+``` shell
 sudo systemctl daemon-reload
 sudo systemctl enable rpi-remote.service
 sudo systemctl start rpi-remote.service
 ```
 
-## Edit config
+## Configuartion
 Config file path: ```~/.config/rpi_remote/config.ini```
 
-## Check logs
+This file automatically generated when the service starts. See the example below.
+``` ini
+[connection]
+server_host = localhost
+server_port = 80 # 443 in case of https
+ssl = true # true/false
+local_port = 22
+period_time_sec = 30
+client_name = test_client
+disk_path = /media/HDD
 ```
+
+## Check logs
+``` shell
 journalctl -fu rpi-remote
 ```
```

### Comparing `rpi-remote-1.1.1/README.md` & `rpi_remote-2.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/rpi-remote?style=for-the-badge&logo=python&logoColor=yellow&link=https%3A%2F%2Fpypi.org%2Fproject%2Frpi-remote%2F)
 
 # Rpi Remote client
 
 ## Installation
 
-### Prerequisites
-```
-sudo apt install build-essential libffi-dev gcc pkg-config python3-dev python3-pip libssl-dev cargo openssl
-```
-Install rust: https://www.rust-lang.org/tools/install
-
-### Install package
-```
+### Install/Upgrade package
+``` shell
 python3 -m pip install --upgrade rpi-remote --user
 ```
 
 ### Create service
-```
+``` shell
 echo "[Unit]
 Description=rpi_remote service
 After=multi-user.target
 Conflicts=getty@tty1.service
 [Service]
 User=${USER}
 Type=simple
@@ -28,20 +22,32 @@
 Environment="LANG=C.UTF-8"
 ExecStart=${HOME}/.local/bin/rpi-remote
 Restart=on-failure
 RestartSec=3
 [Install]
 WantedBy=multi-user.target" | sudo tee /etc/systemd/system/rpi-remote.service
 ```
-```
+``` shell
 sudo systemctl daemon-reload
 sudo systemctl enable rpi-remote.service
 sudo systemctl start rpi-remote.service
 ```
 
-## Edit config
+## Configuartion
 Config file path: ```~/.config/rpi_remote/config.ini```
 
-## Check logs
+This file automatically generated when the service starts. See the example below.
+``` ini
+[connection]
+server_host = localhost
+server_port = 80 # 443 in case of https
+ssl = true # true/false
+local_port = 22
+period_time_sec = 30
+client_name = test_client
+disk_path = /media/HDD
 ```
+
+## Check logs
+``` shell
 journalctl -fu rpi-remote
 ```
```

### Comparing `rpi-remote-1.1.1/rpi_remote/rpi_remote.py` & `rpi_remote-2.0.0/rpi_remote/rpi_remote.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 import os
 import json
 import configparser
 import statistics
 import logging.handlers
 import requests
 import psutil
-from requests.exceptions import ConnectionError # pylint: disable=redefined-builtin
+from requests.exceptions import ConnectionError  # pylint: disable=redefined-builtin
 from .forward import ClientForwarder
 
 
-class RpiRemoteClient: # pylint: disable=too-few-public-methods
+class RpiRemoteClient:  # pylint: disable=too-few-public-methods
 
     CONFIG_FOLDER_PATH = os.path.join(os.path.expanduser('~'), ".config", "rpi_remote")
     CONFIG_PATH = os.path.join(CONFIG_FOLDER_PATH, "config.ini")
     DEFAULT_CONFIG = {
         "connection": {
-            "host_address": "http://localhost:8080",
+            "server_host": "localhost",
+            "server_port": "443",
+            "ssl": "true",
+            "local_port": "22",
             "period_time_sec": "30",
             "client_name": "test_client",
             "disk_path": "/media/HDD",
         }
     }
 
     def __init__(self):
@@ -49,42 +52,53 @@
             config[section] = {}
             for config_key, config_value in configs.items():
                 config[section][config_key] = config_value
         with open(self.CONFIG_PATH, 'w', encoding='utf-8') as f:
             config.write(f)
         return config
 
+    @property
+    def _schema(self):
+        return "https://" if self._config['connection']['ssl'] == 'true' else "http://"
+
+    @property
+    def _server_host(self):
+        return self._config['connection']['server_host']
+
+    @property
+    def _server_port(self):
+        return self._config['connection']['server_port']
+
     def _get_order(self):
-        url = f"{self._config['connection']['host_address']}/rpi/api/order"
+        url = f"{self._schema}{self._server_host}:{self._server_port}/rpi/api/order"
         client_name = self._config['connection']['client_name']
         request = requests.get(url, headers={'name': client_name}, timeout=5)
         return request.json()
 
     def _send_metrics(self):
         metrics = self._collect_metrics()
-        url = f"{self._config['connection']['host_address']}/rpi/api/metric"
+        url = f"{self._schema}{self._server_host}:{self._server_port}/rpi/api/metric"
         client_name = self._config['connection']['client_name']
         data = {
             'name': client_name,
             'uptime': metrics['uptime_hous'],
             'cpu_usage': metrics['cpu_percent'],
             'memory_usage': metrics['mem_percent'],
             'disk_usage': metrics['disk_usage'],
             'temperature': metrics['temperature'],
         }
         headers = {'Content-type': 'application/json'}
-        resp = requests.put(url, data=json.dumps(data), headers=headers, timeout=5)
-        print(resp.status_code, resp.content)
+        requests.put(url, data=json.dumps(data), headers=headers, timeout=5)
 
     def _collect_metrics(self):
         uptime_sec = time.time() - psutil.boot_time()
         disk_path = self._config['connection']['disk_path'] if \
             os.path.exists(self._config['connection']['disk_path']) else '/'
         return {
-            'uptime_hous': int(uptime_sec/3600),
+            'uptime_hous': int(uptime_sec / 3600),
             'mem_percent': int(psutil.virtual_memory().percent),
             'cpu_percent': self._get_cpu_avarage_load(),
             'disk_usage': int(psutil.disk_usage(disk_path).percent),
             'temperature': self._get_cpu_temperature(),
         }
 
     @staticmethod
@@ -105,20 +119,23 @@
             return -1
 
     def run(self):
         self._logger.info("Starting rpi-remote client...")
         while True:
             try:
                 if data := self._get_order():
-                    forwarder = ClientForwarder(**data, logger=self._logger)
+                    forwarder = ClientForwarder(host=self._server_host, port=data['port'],
+                                                local_port=self._config['connection']['local_port'])
                     forwarder.start()
+                    self._get_order()
                 self._send_metrics()
             except ConnectionError as e:
                 self._logger.warning("Cannot connect to host: '%s'", e.request.url)
-            except Exception as e: # pylint: disable=broad-except
-                self._logger.error(e)
+            except Exception:  # pylint: disable=broad-except
+                self._logger.exception("Error occurred")
             finally:
                 time.sleep(int(self._config['connection']['period_time_sec']))
 
+
 def main():
     client = RpiRemoteClient()
     client.run()
```

### Comparing `rpi-remote-1.1.1/rpi_remote.egg-info/PKG-INFO` & `rpi_remote-2.0.0/rpi_remote.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 Metadata-Version: 2.1
 Name: rpi-remote
-Version: 1.1.1
+Version: 2.0.0
 Summary: Rpi remote client
 Author-email: Aron Radics <radics.aron.jozsef@gmail.com>
 Project-URL: Homepage, https://github.com/radaron/rpi_remote_client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: paramiko>=2.12.0
 Requires-Dist: requests>=2.28.1
 Requires-Dist: psutil>=5.8.0
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 ![PyPI - Version](https://img.shields.io/pypi/v/rpi-remote?style=for-the-badge&logo=python&logoColor=yellow&link=https%3A%2F%2Fpypi.org%2Fproject%2Frpi-remote%2F)
 
 # Rpi Remote client
 
 ## Installation
 
-### Prerequisites
-```
-sudo apt install build-essential libffi-dev gcc pkg-config python3-dev python3-pip libssl-dev cargo openssl
-```
-Install rust: https://www.rust-lang.org/tools/install
-
-### Install package
-```
+### Install/Upgrade package
+``` shell
 python3 -m pip install --upgrade rpi-remote --user
 ```
 
 ### Create service
-```
+``` shell
 echo "[Unit]
 Description=rpi_remote service
 After=multi-user.target
 Conflicts=getty@tty1.service
 [Service]
 User=${USER}
 Type=simple
@@ -48,20 +41,32 @@
 Environment="LANG=C.UTF-8"
 ExecStart=${HOME}/.local/bin/rpi-remote
 Restart=on-failure
 RestartSec=3
 [Install]
 WantedBy=multi-user.target" | sudo tee /etc/systemd/system/rpi-remote.service
 ```
-```
+``` shell
 sudo systemctl daemon-reload
 sudo systemctl enable rpi-remote.service
 sudo systemctl start rpi-remote.service
 ```
 
-## Edit config
+## Configuartion
 Config file path: ```~/.config/rpi_remote/config.ini```
 
-## Check logs
+This file automatically generated when the service starts. See the example below.
+``` ini
+[connection]
+server_host = localhost
+server_port = 80 # 443 in case of https
+ssl = true # true/false
+local_port = 22
+period_time_sec = 30
+client_name = test_client
+disk_path = /media/HDD
 ```
+
+## Check logs
+``` shell
 journalctl -fu rpi-remote
 ```
```

