# Comparing `tmp/compose-pydantic-0.2.0.tar.gz` & `tmp/compose_pydantic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose-pydantic-0.2.0.tar", last modified: Sat Apr  2 13:15:06 2022, max compression
+gzip compressed data, was "compose_pydantic-0.2.1.tar", last modified: Sun Apr 28 15:27:09 2024, max compression
```

## Comparing `compose-pydantic-0.2.0.tar` & `compose_pydantic-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-04-02 13:15:06.086355 compose-pydantic-0.2.0/
--rw-r--r--   0 alex       (501) staff       (20)     1114 2022-03-31 11:21:04.000000 compose-pydantic-0.2.0/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     5598 2022-04-02 13:15:06.086795 compose-pydantic-0.2.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     4855 2022-04-02 13:13:21.000000 compose-pydantic-0.2.0/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-04-02 13:15:06.076135 compose-pydantic-0.2.0/compose_pydantic/
--rw-r--r--   0 alex       (501) staff       (20)     1866 2022-03-31 09:20:48.000000 compose-pydantic-0.2.0/compose_pydantic/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2610 2022-04-02 13:14:45.000000 compose-pydantic-0.2.0/compose_pydantic/lib.py
--rw-r--r--   0 alex       (501) staff       (20)    14897 2022-03-29 14:22:15.000000 compose-pydantic-0.2.0/compose_pydantic/models.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-04-02 13:15:06.085917 compose-pydantic-0.2.0/compose_pydantic.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     5598 2022-04-02 13:15:05.000000 compose-pydantic-0.2.0/compose_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      321 2022-04-02 13:15:06.000000 compose-pydantic-0.2.0/compose_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2022-04-02 13:15:05.000000 compose-pydantic-0.2.0/compose_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       45 2022-04-02 13:15:05.000000 compose-pydantic-0.2.0/compose_pydantic.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       17 2022-04-02 13:15:05.000000 compose-pydantic-0.2.0/compose_pydantic.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       80 2022-03-30 15:24:47.000000 compose-pydantic-0.2.0/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)      816 2022-04-02 13:15:06.087882 compose-pydantic-0.2.0/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-28 15:27:09.374096 compose_pydantic-0.2.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1114 2024-04-28 14:17:52.000000 compose_pydantic-0.2.1/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     6127 2024-04-28 15:27:09.374096 compose_pydantic-0.2.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4972 2024-04-28 14:46:48.000000 compose_pydantic-0.2.1/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)       80 2024-04-28 14:17:52.000000 compose_pydantic-0.2.1/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1059 2024-04-28 15:27:09.378096 compose_pydantic-0.2.1/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-28 15:27:09.366096 compose_pydantic-0.2.1/src/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-28 15:27:09.370096 compose_pydantic-0.2.1/src/compose_pydantic/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1866 2024-04-28 14:46:48.000000 compose_pydantic-0.2.1/src/compose_pydantic/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2610 2024-04-28 14:46:48.000000 compose_pydantic-0.2.1/src/compose_pydantic/lib.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14897 2024-04-28 14:46:48.000000 compose_pydantic-0.2.1/src/compose_pydantic/models.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-28 15:27:09.370096 compose_pydantic-0.2.1/src/compose_pydantic.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6127 2024-04-28 15:27:09.000000 compose_pydantic-0.2.1/src/compose_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      414 2024-04-28 15:27:09.000000 compose_pydantic-0.2.1/src/compose_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-04-28 15:27:09.000000 compose_pydantic-0.2.1/src/compose_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-04-28 15:26:40.000000 compose_pydantic-0.2.1/src/compose_pydantic.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1000) alex      (1000)      120 2024-04-28 15:27:09.000000 compose_pydantic-0.2.1/src/compose_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2024-04-28 15:27:09.000000 compose_pydantic-0.2.1/src/compose_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-28 15:27:09.370096 compose_pydantic-0.2.1/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1071 2024-04-28 15:24:43.000000 compose_pydantic-0.2.1/tests/test_lib.py
```

### Comparing `compose-pydantic-0.2.0/LICENSE` & `compose_pydantic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compose-pydantic-0.2.0/PKG-INFO` & `compose_pydantic-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 Metadata-Version: 2.1
 Name: compose-pydantic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parse Compose Specification data using Pydantic
 Home-page: https://github.com/alexmon/compose-pydantic
 Author: Alexandros Monastiriotis
 Author-email: alexmondev@gmail.com
 License: MIT
 Keywords: Compose,Pydantic
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic==1.9.0
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: mergedeep>=1.3.4
+Provides-Extra: dev
+Requires-Dist: IPython; extra == "dev"
+Provides-Extra: testing
+Requires-Dist: IPython; extra == "testing"
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: mock; extra == "testing"
+Requires-Dist: flake8==5.0.4; extra == "testing"
 
 # compose-pydantic
 
 Parse `Compose Specification` YAML using `Pydantic` and `PyYAML`.
 
 ## Description
 
@@ -34,15 +45,15 @@
     --output compose_pydantic/models.py
 ```
 
 ## Getting Started
 
 ### Dependencies
 
-* pydantic>=1.9.0
+* pydantic==1.9.0
 * PyYAML>=6.0
 * mergedeep>=1.3.4
 
 ### Installation
 
 ```bash
 pip install compose-pydantic
@@ -61,14 +72,22 @@
 ```
 
 Result:
 ```python
 {'version': '3.9', 'name': None, 'services': {'db': Service(deploy=None, build=None, blkio_config=None, cap_add=None, cap_drop=None, cgroup_parent=None, command=None, configs=None, container_name=None, cpu_count=None, cpu_percent=None, cpu_shares=None, cpu_quota=None, cpu_period=None, cpu_rt_period=None, cpu_rt_runtime=None, cpus=None, cpuset=None, credential_spec=None, depends_on=None, device_cgroup_rules=None, devices=None, dns=None, dns_opt=None, dns_search=None, domainname=None, entrypoint=None, env_file=None, environment=ListOrDict(__root__=['POSTGRES_NAME=devpostgres', 'POSTGRES_USER=devpostgres', 'POSTGRES_PASSWORD=devpostgres']), expose=None, extends=None, external_links=None, extra_hosts=None, group_add=None, healthcheck=None, hostname=None, image='postgres', init=None, ipc=None, isolation=None, labels=None, links=None, logging=None, mac_address=None, mem_limit=None, mem_reservation=None, mem_swappiness=None, memswap_limit=None, network_mode=None, networks=None, oom_kill_disable=None, oom_score_adj=None, pid=None, pids_limit=None, platform=None, ports=None, privileged=None, profiles=None, pull_policy=None, read_only=None, restart=None, runtime=None, scale=None, security_opt=None, shm_size=None, secrets=None, sysctls=None, stdin_open=None, stop_grace_period=None, stop_signal=None, storage_opt=None, tmpfs=None, tty=None, ulimits=None, user=None, userns_mode=None, volumes=['./data/db:/var/lib/postgresql/data'], volumes_from=None, working_dir=None), 'web': Service(deploy=None, build='.', blkio_config=None, cap_add=None, cap_drop=None, cgroup_parent=None, command='python manage.py runserver 0.0.0.0:8000', configs=None, container_name=None, cpu_count=None, cpu_percent=None, cpu_shares=None, cpu_quota=None, cpu_period=None, cpu_rt_period=None, cpu_rt_runtime=None, cpus=None, cpuset=None, credential_spec=None, depends_on=ListOfStrings(__root__=['db']), device_cgroup_rules=None, devices=None, dns=None, dns_opt=None, dns_search=None, domainname=None, entrypoint=None, env_file=None, environment=ListOrDict(__root__=['POSTGRES_NAME=devpostgres', 'POSTGRES_USER=devpostgres', 'POSTGRES_PASSWORD=devpostgres']), expose=None, extends=None, external_links=None, extra_hosts=None, group_add=None, healthcheck=None, hostname=None, image=None, init=None, ipc=None, isolation=None, labels=None, links=None, logging=None, mac_address=None, mem_limit=None, mem_reservation=None, mem_swappiness=None, memswap_limit=None, network_mode=None, networks=None, oom_kill_disable=None, oom_score_adj=None, pid=None, pids_limit=None, platform=None, ports=['8000:8000'], privileged=None, profiles=None, pull_policy=None, read_only=None, restart=None, runtime=None, scale=None, security_opt=None, shm_size=None, secrets=None, sysctls=None, stdin_open=None, stop_grace_period=None, stop_signal=None, storage_opt=None, tmpfs=None, tty=None, ulimits=None, user=None, userns_mode=None, volumes=['.:/code'], volumes_from=None, working_dir=None)}, 'networks': None, 'volumes': None, 'secrets': None, 'configs': None}
 ```
 
+## Tests
+
+If you're working with a clone of this repository, you can run tests like this:
+
+```bash
+$ make init test
+```
+
 See also `tests/test_lib.py` for the different ways you may use the factory class to access compose spec data.
 
 ## Authors
 
 Alexandros Monastiriotis alexmondev@gmail.com
 
 ## Version History
@@ -89,13 +108,7 @@
 Inspiration, libraries, etc.
 * [pydantic](https://github.com/samuelcolvin/pydantic/)
 * [datamodel-code-generator](https://github.com/koxudaxi/datamodel-code-generator/)
 * [Compose Specification](https://github.com/compose-spec/compose-spec)
 * [PyYAML](https://github.com/yaml/pyyaml)
 * [mergedeep](https://github.com/clarketm/mergedeep)
 * [Understanding multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files)
-
-
-
-
-
-
```

### Comparing `compose-pydantic-0.2.0/README.md` & `compose_pydantic-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     --output compose_pydantic/models.py
 ```
 
 ## Getting Started
 
 ### Dependencies
 
-* pydantic>=1.9.0
+* pydantic==1.9.0
 * PyYAML>=6.0
 * mergedeep>=1.3.4
 
 ### Installation
 
 ```bash
 pip install compose-pydantic
@@ -40,14 +40,22 @@
 ```
 
 Result:
 ```python
 {'version': '3.9', 'name': None, 'services': {'db': Service(deploy=None, build=None, blkio_config=None, cap_add=None, cap_drop=None, cgroup_parent=None, command=None, configs=None, container_name=None, cpu_count=None, cpu_percent=None, cpu_shares=None, cpu_quota=None, cpu_period=None, cpu_rt_period=None, cpu_rt_runtime=None, cpus=None, cpuset=None, credential_spec=None, depends_on=None, device_cgroup_rules=None, devices=None, dns=None, dns_opt=None, dns_search=None, domainname=None, entrypoint=None, env_file=None, environment=ListOrDict(__root__=['POSTGRES_NAME=devpostgres', 'POSTGRES_USER=devpostgres', 'POSTGRES_PASSWORD=devpostgres']), expose=None, extends=None, external_links=None, extra_hosts=None, group_add=None, healthcheck=None, hostname=None, image='postgres', init=None, ipc=None, isolation=None, labels=None, links=None, logging=None, mac_address=None, mem_limit=None, mem_reservation=None, mem_swappiness=None, memswap_limit=None, network_mode=None, networks=None, oom_kill_disable=None, oom_score_adj=None, pid=None, pids_limit=None, platform=None, ports=None, privileged=None, profiles=None, pull_policy=None, read_only=None, restart=None, runtime=None, scale=None, security_opt=None, shm_size=None, secrets=None, sysctls=None, stdin_open=None, stop_grace_period=None, stop_signal=None, storage_opt=None, tmpfs=None, tty=None, ulimits=None, user=None, userns_mode=None, volumes=['./data/db:/var/lib/postgresql/data'], volumes_from=None, working_dir=None), 'web': Service(deploy=None, build='.', blkio_config=None, cap_add=None, cap_drop=None, cgroup_parent=None, command='python manage.py runserver 0.0.0.0:8000', configs=None, container_name=None, cpu_count=None, cpu_percent=None, cpu_shares=None, cpu_quota=None, cpu_period=None, cpu_rt_period=None, cpu_rt_runtime=None, cpus=None, cpuset=None, credential_spec=None, depends_on=ListOfStrings(__root__=['db']), device_cgroup_rules=None, devices=None, dns=None, dns_opt=None, dns_search=None, domainname=None, entrypoint=None, env_file=None, environment=ListOrDict(__root__=['POSTGRES_NAME=devpostgres', 'POSTGRES_USER=devpostgres', 'POSTGRES_PASSWORD=devpostgres']), expose=None, extends=None, external_links=None, extra_hosts=None, group_add=None, healthcheck=None, hostname=None, image=None, init=None, ipc=None, isolation=None, labels=None, links=None, logging=None, mac_address=None, mem_limit=None, mem_reservation=None, mem_swappiness=None, memswap_limit=None, network_mode=None, networks=None, oom_kill_disable=None, oom_score_adj=None, pid=None, pids_limit=None, platform=None, ports=['8000:8000'], privileged=None, profiles=None, pull_policy=None, read_only=None, restart=None, runtime=None, scale=None, security_opt=None, shm_size=None, secrets=None, sysctls=None, stdin_open=None, stop_grace_period=None, stop_signal=None, storage_opt=None, tmpfs=None, tty=None, ulimits=None, user=None, userns_mode=None, volumes=['.:/code'], volumes_from=None, working_dir=None)}, 'networks': None, 'volumes': None, 'secrets': None, 'configs': None}
 ```
 
+## Tests
+
+If you're working with a clone of this repository, you can run tests like this:
+
+```bash
+$ make init test
+```
+
 See also `tests/test_lib.py` for the different ways you may use the factory class to access compose spec data.
 
 ## Authors
 
 Alexandros Monastiriotis alexmondev@gmail.com
 
 ## Version History
@@ -68,11 +76,7 @@
 Inspiration, libraries, etc.
 * [pydantic](https://github.com/samuelcolvin/pydantic/)
 * [datamodel-code-generator](https://github.com/koxudaxi/datamodel-code-generator/)
 * [Compose Specification](https://github.com/compose-spec/compose-spec)
 * [PyYAML](https://github.com/yaml/pyyaml)
 * [mergedeep](https://github.com/clarketm/mergedeep)
 * [Understanding multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files)
-
-
-
-
```

### Comparing `compose-pydantic-0.2.0/compose_pydantic/__init__.py` & `compose_pydantic-0.2.1/src/compose_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `compose-pydantic-0.2.0/compose_pydantic/lib.py` & `compose_pydantic-0.2.1/src/compose_pydantic/lib.py`

 * *Files identical despite different names*

### Comparing `compose-pydantic-0.2.0/compose_pydantic/models.py` & `compose_pydantic-0.2.1/src/compose_pydantic/models.py`

 * *Files identical despite different names*

### Comparing `compose-pydantic-0.2.0/compose_pydantic.egg-info/PKG-INFO` & `compose_pydantic-0.2.1/src/compose_pydantic.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 Metadata-Version: 2.1
 Name: compose-pydantic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parse Compose Specification data using Pydantic
 Home-page: https://github.com/alexmon/compose-pydantic
 Author: Alexandros Monastiriotis
 Author-email: alexmondev@gmail.com
 License: MIT
 Keywords: Compose,Pydantic
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic==1.9.0
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: mergedeep>=1.3.4
+Provides-Extra: dev
+Requires-Dist: IPython; extra == "dev"
+Provides-Extra: testing
+Requires-Dist: IPython; extra == "testing"
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: mock; extra == "testing"
+Requires-Dist: flake8==5.0.4; extra == "testing"
 
 # compose-pydantic
 
 Parse `Compose Specification` YAML using `Pydantic` and `PyYAML`.
 
 ## Description
 
@@ -34,15 +45,15 @@
     --output compose_pydantic/models.py
 ```
 
 ## Getting Started
 
 ### Dependencies
 
-* pydantic>=1.9.0
+* pydantic==1.9.0
 * PyYAML>=6.0
 * mergedeep>=1.3.4
 
 ### Installation
 
 ```bash
 pip install compose-pydantic
@@ -61,14 +72,22 @@
 ```
 
 Result:
 ```python
 {'version': '3.9', 'name': None, 'services': {'db': Service(deploy=None, build=None, blkio_config=None, cap_add=None, cap_drop=None, cgroup_parent=None, command=None, configs=None, container_name=None, cpu_count=None, cpu_percent=None, cpu_shares=None, cpu_quota=None, cpu_period=None, cpu_rt_period=None, cpu_rt_runtime=None, cpus=None, cpuset=None, credential_spec=None, depends_on=None, device_cgroup_rules=None, devices=None, dns=None, dns_opt=None, dns_search=None, domainname=None, entrypoint=None, env_file=None, environment=ListOrDict(__root__=['POSTGRES_NAME=devpostgres', 'POSTGRES_USER=devpostgres', 'POSTGRES_PASSWORD=devpostgres']), expose=None, extends=None, external_links=None, extra_hosts=None, group_add=None, healthcheck=None, hostname=None, image='postgres', init=None, ipc=None, isolation=None, labels=None, links=None, logging=None, mac_address=None, mem_limit=None, mem_reservation=None, mem_swappiness=None, memswap_limit=None, network_mode=None, networks=None, oom_kill_disable=None, oom_score_adj=None, pid=None, pids_limit=None, platform=None, ports=None, privileged=None, profiles=None, pull_policy=None, read_only=None, restart=None, runtime=None, scale=None, security_opt=None, shm_size=None, secrets=None, sysctls=None, stdin_open=None, stop_grace_period=None, stop_signal=None, storage_opt=None, tmpfs=None, tty=None, ulimits=None, user=None, userns_mode=None, volumes=['./data/db:/var/lib/postgresql/data'], volumes_from=None, working_dir=None), 'web': Service(deploy=None, build='.', blkio_config=None, cap_add=None, cap_drop=None, cgroup_parent=None, command='python manage.py runserver 0.0.0.0:8000', configs=None, container_name=None, cpu_count=None, cpu_percent=None, cpu_shares=None, cpu_quota=None, cpu_period=None, cpu_rt_period=None, cpu_rt_runtime=None, cpus=None, cpuset=None, credential_spec=None, depends_on=ListOfStrings(__root__=['db']), device_cgroup_rules=None, devices=None, dns=None, dns_opt=None, dns_search=None, domainname=None, entrypoint=None, env_file=None, environment=ListOrDict(__root__=['POSTGRES_NAME=devpostgres', 'POSTGRES_USER=devpostgres', 'POSTGRES_PASSWORD=devpostgres']), expose=None, extends=None, external_links=None, extra_hosts=None, group_add=None, healthcheck=None, hostname=None, image=None, init=None, ipc=None, isolation=None, labels=None, links=None, logging=None, mac_address=None, mem_limit=None, mem_reservation=None, mem_swappiness=None, memswap_limit=None, network_mode=None, networks=None, oom_kill_disable=None, oom_score_adj=None, pid=None, pids_limit=None, platform=None, ports=['8000:8000'], privileged=None, profiles=None, pull_policy=None, read_only=None, restart=None, runtime=None, scale=None, security_opt=None, shm_size=None, secrets=None, sysctls=None, stdin_open=None, stop_grace_period=None, stop_signal=None, storage_opt=None, tmpfs=None, tty=None, ulimits=None, user=None, userns_mode=None, volumes=['.:/code'], volumes_from=None, working_dir=None)}, 'networks': None, 'volumes': None, 'secrets': None, 'configs': None}
 ```
 
+## Tests
+
+If you're working with a clone of this repository, you can run tests like this:
+
+```bash
+$ make init test
+```
+
 See also `tests/test_lib.py` for the different ways you may use the factory class to access compose spec data.
 
 ## Authors
 
 Alexandros Monastiriotis alexmondev@gmail.com
 
 ## Version History
@@ -89,13 +108,7 @@
 Inspiration, libraries, etc.
 * [pydantic](https://github.com/samuelcolvin/pydantic/)
 * [datamodel-code-generator](https://github.com/koxudaxi/datamodel-code-generator/)
 * [Compose Specification](https://github.com/compose-spec/compose-spec)
 * [PyYAML](https://github.com/yaml/pyyaml)
 * [mergedeep](https://github.com/clarketm/mergedeep)
 * [Understanding multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files)
-
-
-
-
-
-
```

