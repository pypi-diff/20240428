# Comparing `tmp/pgqueuer-0.1.0.tar.gz` & `tmp/pgqueuer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.1.0.tar", last modified: Fri Apr 26 21:08:02 2024, max compression
+gzip compressed data, was "pgqueuer-0.2.0.tar", last modified: Sat Apr 27 16:18:09 2024, max compression
```

## Comparing `pgqueuer-0.1.0.tar` & `pgqueuer-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:02.275880 pgqueuer-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:02.271880 pgqueuer-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:02.271880 pgqueuer-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-26 21:08:02.275880 pgqueuer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:08:02.275880 pgqueuer-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:02.271880 pgqueuer-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:02.271880 pgqueuer-0.1.0/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:02.275880 pgqueuer-0.1.0/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-26 21:08:02.000000 pgqueuer-0.1.0/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-26 21:08:02.000000 pgqueuer-0.1.0/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:08:02.000000 pgqueuer-0.1.0/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-26 21:08:02.000000 pgqueuer-0.1.0/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 21:08:02.000000 pgqueuer-0.1.0/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 21:08:02.000000 pgqueuer-0.1.0/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:02.275880 pgqueuer-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:02.275880 pgqueuer-0.1.0/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-26 21:07:53.000000 pgqueuer-0.1.0/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:18:09.377997 pgqueuer-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:18:09.369997 pgqueuer-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:18:09.373997 pgqueuer-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-27 16:18:09.377997 pgqueuer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:18:09.377997 pgqueuer-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:18:09.373997 pgqueuer-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:18:09.373997 pgqueuer-0.2.0/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:18:09.377997 pgqueuer-0.2.0/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-27 16:18:09.000000 pgqueuer-0.2.0/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-27 16:18:09.000000 pgqueuer-0.2.0/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:18:09.000000 pgqueuer-0.2.0/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-27 16:18:09.000000 pgqueuer-0.2.0/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 16:18:09.000000 pgqueuer-0.2.0/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 16:18:09.000000 pgqueuer-0.2.0/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:18:09.377997 pgqueuer-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:18:09.377997 pgqueuer-0.2.0/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-27 16:17:59.000000 pgqueuer-0.2.0/test/test_tm.py
```

### Comparing `pgqueuer-0.1.0/.github/workflows/ci.yml` & `pgqueuer-0.2.0/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -32,7 +32,15 @@
       - name: Install PgQueuer
         run: |
           pip install pip -U
           pip install .[dev]
 
       - name: Full test
         run: pytest -v
+
+  check-all-ci-passed:
+    name: Check test matrix passed.
+    needs: ci
+    runs-on: ubuntu-latest
+    steps:
+      - name: Check status
+        run: echo "All tests passed; ready to merge."
```

### Comparing `pgqueuer-0.1.0/.github/workflows/linting.yml` & `pgqueuer-0.2.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.1.0/.github/workflows/release.yml` & `pgqueuer-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.1.0/.gitignore` & `pgqueuer-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.1.0/LICENSE` & `pgqueuer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.1.0/PKG-INFO` & `pgqueuer-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.1.0
+Version: 0.2.0
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
@@ -32,18 +32,14 @@
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: myst-parser; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 ## PgQueuer
 
 PgQueuer is a minimalist, high-performance job queue library for Python, leveraging the robustness of PostgreSQL. Designed for simplicity and efficiency, PgQueuer uses PostgreSQL's native features like transactions, row locking, and LISTEN/NOTIFY to manage job queues effortlessly.
 
 ### Features
 
@@ -96,45 +92,38 @@
 In this scenario, the system is designed to manage a queue of incoming data messages that need to be processed. Each message is encapsulated as a job, and these jobs are then processed by a designated function linked to an entrypoint. This is typical in systems where large volumes of data are collected continuously, such as telemetry data from IoT devices, logs from web servers, or transaction data in financial systems.
 
 #### Function Description:
 The `fetch` function, tied to the `fetch` entrypoint, is responsible for processing each message. It simulates a processing task by printing the content of each message. This function could be adapted to perform more complex operations such as parsing, analyzing, storing, or forwarding the data as required by the application.
 
 ```python
 import asyncio
-import time
 
 import asyncpg
-
-from PgQueuer import qm, queries
+from PgQueuer.models import Job
+from PgQueuer.qm import QueueManager
 
 
 async def main() -> None:
     # Set up a connection pool with a minimum of 2 connections.
     pool = await asyncpg.create_pool(min_size=2)
     # Initialize the QueueManager with the connection pool and query handler.
-    app = qm.QueueManager(
-        pool, 
-        queries.PgQueuerQueries(pool),
-        queries.PgQueuerLogQueries(pool),
-    )
+    qm = QueueManager(pool)
 
     # Number of messages to simulate.
     N = 10_000
 
     # Enqueue messages.
     for n in range(N):
-        await app.q.enqueue("fetch", f"this is from me: {n}".encode())
+        await qm.queries.enqueue("fetch", f"this is from me: {n}".encode())
 
     # Define a processing function for each message.
-    @c.entrypoint("fetch")
-    async def process_message(context: bytes) -> None:
-        # Simulate parsing the message.
-        message = context.decode()
+    @qm.entrypoint("fetch")
+    async def process_message(job: Job) -> None:
         # Print the message to simulate processing.
-        print(f"Processed message: {message}")
+        print(f"Processed message: {job}")
 
-    await app.run()
+    await qm.run()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `pgqueuer-0.1.0/README.md` & `pgqueuer-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,45 +53,38 @@
 In this scenario, the system is designed to manage a queue of incoming data messages that need to be processed. Each message is encapsulated as a job, and these jobs are then processed by a designated function linked to an entrypoint. This is typical in systems where large volumes of data are collected continuously, such as telemetry data from IoT devices, logs from web servers, or transaction data in financial systems.
 
 #### Function Description:
 The `fetch` function, tied to the `fetch` entrypoint, is responsible for processing each message. It simulates a processing task by printing the content of each message. This function could be adapted to perform more complex operations such as parsing, analyzing, storing, or forwarding the data as required by the application.
 
 ```python
 import asyncio
-import time
 
 import asyncpg
-
-from PgQueuer import qm, queries
+from PgQueuer.models import Job
+from PgQueuer.qm import QueueManager
 
 
 async def main() -> None:
     # Set up a connection pool with a minimum of 2 connections.
     pool = await asyncpg.create_pool(min_size=2)
     # Initialize the QueueManager with the connection pool and query handler.
-    app = qm.QueueManager(
-        pool, 
-        queries.PgQueuerQueries(pool),
-        queries.PgQueuerLogQueries(pool),
-    )
+    qm = QueueManager(pool)
 
     # Number of messages to simulate.
     N = 10_000
 
     # Enqueue messages.
     for n in range(N):
-        await app.q.enqueue("fetch", f"this is from me: {n}".encode())
+        await qm.queries.enqueue("fetch", f"this is from me: {n}".encode())
 
     # Define a processing function for each message.
-    @c.entrypoint("fetch")
-    async def process_message(context: bytes) -> None:
-        # Simulate parsing the message.
-        message = context.decode()
+    @qm.entrypoint("fetch")
+    async def process_message(job: Job) -> None:
         # Print the message to simulate processing.
-        print(f"Processed message: {message}")
+        print(f"Processed message: {job}")
 
-    await app.run()
+    await qm.run()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `pgqueuer-0.1.0/pyproject.toml` & `pgqueuer-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -46,19 +46,14 @@
     "asyncpg-stubs",
     "mypy-extensions",
     "mypy",
     "pytest-asyncio",
     "pytest",
     "ruff",
 ]
-docs = [
-    "myst-parser",
-    "sphinx",
-    "sphinx-rtd-theme",
-]
 
 [tool.setuptools_scm]
 write_to = "src/_version.py"
 
 [tool.ruff]
 line-length = 88
 [tool.ruff.lint]
@@ -76,15 +71,15 @@
     "C90",
 ]
 [tool.ruff.lint.isort]
 combine-as-imports = true
 
 [tool.mypy]
 disallow_untyped_defs = true
-exclude = "^(build|docs)"
+exclude = "^(build)"
 extra_checks = true
 ignore_missing_imports = true
 plugins = ["pydantic.mypy"]
 python_version = "3.10"
 strict_equality = true
 warn_redundant_casts = true
 warn_unused_configs = true
```

### Comparing `pgqueuer-0.1.0/src/PgQueuer/cli.py` & `pgqueuer-0.2.0/src/PgQueuer/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,15 +116,13 @@
     async with asyncpg.create_pool(
         parsed.pg_dsn,
         database=parsed.pg_database,
         password=parsed.pg_password,
         port=parsed.pg_port,
         user=parsed.pg_user,
         host=parsed.pg_host,
-        min_size=0,
-        max_size=1,
     ) as pool:
         match parsed.command:
             case "install":
-                await queries.InstallUninstallQueries(pool=pool).install()
+                await queries.Queries(pool=pool).install()
             case "uninstall":
-                await queries.InstallUninstallQueries(pool=pool).uninstall()
+                await queries.Queries(pool=pool).uninstall()
```

### Comparing `pgqueuer-0.1.0/src/PgQueuer/models.py` & `pgqueuer-0.2.0/src/PgQueuer/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal
 
-from pydantic import AwareDatetime, BaseModel, RootModel
+from pydantic import AwareDatetime, BaseModel
 
 STATUS = Literal[
     "queued",
     "picked",
 ]
 STATUS_LOG = Literal[
     "exception",
@@ -22,11 +22,26 @@
     priority: int
     created: AwareDatetime
     status: STATUS
     entrypoint: str
     payload: bytes | None
 
 
-class Jobs(RootModel[list[Job]]):
+class QueueSize(BaseModel):
     """
-    A collection model that encapsulates a list of Job instances.
+    Represents the number of jobs per entrypoint and priority in the queue.
     """
+
+    count: int
+    entrypoint: str
+    priority: int
+
+
+class LogSize(BaseModel):
+    """
+    Represents log details for jobs based on status, entrypoint, and priority.
+    """
+
+    count: int
+    entrypoint: str
+    priority: int
+    status: STATUS_LOG
```

### Comparing `pgqueuer-0.1.0/src/PgQueuer/qm.py` & `pgqueuer-0.2.0/src/PgQueuer/qm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from __future__ import annotations
 
 import asyncio
 import dataclasses
-from typing import Awaitable, Callable, TypeAlias, TypeVar
+from typing import TYPE_CHECKING, Awaitable, Callable, TypeAlias, TypeVar
 
 import asyncpg
 from pgcachewatch.listeners import PGEventQueue
 from pgcachewatch.models import PGChannel
 
 from .logconfig import logger
 from .models import Job
-from .queries import PgQueuerLogQueries, PgQueuerQueries
+from .queries import Queries
 from .tm import TaskManager
 
-EntrypointFn: TypeAlias = Callable[[bytes | None], Awaitable[None]]
-T = TypeVar("T", bound=EntrypointFn)
+if TYPE_CHECKING:
+    EntrypointFn: TypeAlias = Callable[[Job], Awaitable[None]]
+    T = TypeVar("T", bound=EntrypointFn)
 
 
 @dataclasses.dataclass
 class QueueManager:
     """
     Manages job queues and dispatches jobs to registered entry points,
     handling database connections and events.
     """
 
     pool: asyncpg.Pool
-    q: PgQueuerQueries = dataclasses.field(init=False)
-    ql: PgQueuerLogQueries = dataclasses.field(init=False)
+    queries: Queries = dataclasses.field(init=False)
 
     channel: PGChannel = dataclasses.field(
         default=PGChannel("ch_pgqueuer"),
         init=False,
     )
     alive: bool = dataclasses.field(
         init=False,
@@ -49,26 +49,26 @@
     def __post_init__(self) -> None:
         """
         Initializes database query handlers and validates pool size upon
         instance creation.
         """
         if self.pool.get_min_size() < 1:
             raise ValueError("... min size must be gt 1.")
-        self.q = PgQueuerQueries(self.pool)
-        self.ql = PgQueuerLogQueries(self.pool)
+        self.queries = Queries(self.pool)
 
     def entrypoint(self, name: str) -> Callable[[T], T]:
         """
         Decorator to register a function as an entrypoint for
         handling specific job types.
         """
 
+        if name in self.registry:
+            raise RuntimeError(f"{name} already in registry, name must be unique.")
+
         def register(func: T) -> T:
-            if name in self.registry:
-                raise RuntimeError(f"{name} already in registry, must be unique.")
             self.registry[name] = func
             return func
 
         return register
 
     async def run(self) -> None:
         """
@@ -76,17 +76,16 @@
         registered entry points until stopped.
         """
         async with self.pool.acquire() as conn:
             listener = PGEventQueue()
             await listener.connect(conn, self.channel)
 
             while self.alive:
-                while (jobs := await self.q.dequeue()).root:
-                    for job in jobs.root:
-                        self._dispatch(job)
+                while job := await self.queries.dequeue():
+                    self._dispatch(job)
                 await listener.get()
 
             await asyncio.gather(*self.tm.tasks)
 
     def _dispatch(self, job: Job) -> None:
         """
         Internal method to asynchronously handle job dispatch,
@@ -96,24 +95,24 @@
         async def runit() -> None:
             logger.debug(
                 "Dispatching entrypoint/id: %s/%s",
                 job.entrypoint,
                 job.id,
             )
             try:
-                await self.registry[job.entrypoint](job.payload)
+                await self.registry[job.entrypoint](job)
             except Exception:
                 logger.exception(
                     "Exception while processing entrypoint/id: %s/%s",
                     job.entrypoint,
                     job.id,
                 )
-                await self.ql.move_job_log(job, "exception")
+                await self.queries.log_job(job, "exception")
             else:
                 logger.debug(
                     "Dispatching entrypoint/id: %s/%s - successful",
                     job.entrypoint,
                     job.id,
                 )
-                await self.ql.move_job_log(job, "successful")
+                await self.queries.log_job(job, "successful")
 
         self.tm.add(asyncio.create_task(runit()))
```

### Comparing `pgqueuer-0.1.0/src/PgQueuer/queries.py` & `pgqueuer-0.2.0/src/PgQueuer/queries.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,232 +50,212 @@
     trigger: Final[str] = dataclasses.field(
         default_factory=lambda: add_prefix("tg_pgqueuer_changed"),
         kw_only=True,
     )
 
 
 @dataclasses.dataclass
-class InstallUninstallQueries:
+class Queries:
     """
-    Provides methods to install (create) and uninstall (drop)
-    database schemas and objects like tables, types, and triggers
-    related to the pgqueuer system.
+    Handles operations related to job queuing such as
+    enqueueing, dequeueing, and querying the size of the queue.
     """
 
     pool: asyncpg.Pool
     settings: DBSettings = dataclasses.field(default_factory=DBSettings)
 
     async def install(self) -> None:
         """
         Creates necessary database structures such as enums,
         tables, and triggers for job queuing and logging.
         """
-        await self.pool.execute(
-            f"""
-    CREATE TYPE {self.settings.queue_status_type} AS ENUM ('queued', 'picked');
-    CREATE TABLE {self.settings.queue_table} (
-        id SERIAL PRIMARY KEY,
-        priority INT NOT NULL,
-        created TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT CURRENT_TIMESTAMP,
-        status {self.settings.queue_status_type} NOT NULL,
-        entrypoint TEXT NOT NULL,
-        payload BYTEA
-    );
-    CREATE UNIQUE INDEX ON {self.settings.queue_table} (priority, id) WHERE status != 'picked';
-
-    CREATE TYPE {self.settings.log_table_status_type} AS ENUM ('exception', 'successful');
-    CREATE TABLE {self.settings.log_table} (
-        id SERIAL PRIMARY KEY,
-        priority INT NOT NULL,
-        created TIMESTAMP WITH TIME ZONE DEFAULT CURRENT_TIMESTAMP,
-        duration INTERVAL NOT NULL,
-        status {self.settings.log_table_status_type} NOT NULL,
-        entrypoint TEXT NOT NULL
-    );
-
-
-    CREATE FUNCTION {self.settings.function}() RETURNS TRIGGER AS $$
-    BEGIN
-        PERFORM pg_notify(
-        '{self.settings.channel}',
-        json_build_object(
-            'channel', '{self.settings.channel}',
-            'operation', lower(TG_OP),
-            'sent_at', NOW(),
-            'table', TG_TABLE_NAME
-        )::text);
-        RETURN NEW;
-    END;
-    $$ LANGUAGE plpgsql;
-
-    CREATE TRIGGER {self.settings.trigger}
-    AFTER INSERT OR UPDATE OR DELETE OR TRUNCATE ON {self.settings.queue_table}
-    EXECUTE FUNCTION {self.settings.function}();
-    """  # noqa: E501
-        )
+
+        query = f"""
+            CREATE TYPE {self.settings.queue_status_type} AS ENUM ('queued', 'picked');
+            CREATE TABLE {self.settings.queue_table} (
+                id SERIAL PRIMARY KEY,
+                priority INT NOT NULL,
+                created TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT CURRENT_TIMESTAMP,
+                status {self.settings.queue_status_type} NOT NULL,
+                entrypoint TEXT NOT NULL,
+                payload BYTEA
+            );
+            CREATE UNIQUE INDEX ON {self.settings.queue_table} (priority, id) WHERE status != 'picked';
+
+            CREATE TYPE {self.settings.log_table_status_type} AS ENUM ('exception', 'successful');
+            CREATE TABLE {self.settings.log_table} (
+                id SERIAL PRIMARY KEY,
+                priority INT NOT NULL,
+                created TIMESTAMP WITH TIME ZONE DEFAULT CURRENT_TIMESTAMP,
+                duration INTERVAL NOT NULL,
+                status {self.settings.log_table_status_type} NOT NULL,
+                entrypoint TEXT NOT NULL
+            );
+
+            CREATE FUNCTION {self.settings.function}() RETURNS TRIGGER AS $$
+            BEGIN
+                PERFORM pg_notify(
+                '{self.settings.channel}',
+                json_build_object(
+                    'channel', '{self.settings.channel}',
+                    'operation', lower(TG_OP),
+                    'sent_at', NOW(),
+                    'table', TG_TABLE_NAME
+                )::text);
+                RETURN NEW;
+            END;
+            $$ LANGUAGE plpgsql;
+
+            CREATE TRIGGER {self.settings.trigger}
+            AFTER INSERT OR UPDATE OR DELETE OR TRUNCATE ON {self.settings.queue_table}
+            EXECUTE FUNCTION {self.settings.function}();
+        """  # noqa: E501
+
+        await self.pool.execute(query)
 
     async def uninstall(self) -> None:
         """
         Drops all database structures related to job queuing
         and logging that were created by the install method.
         """
-        await self.pool.execute(
-            f"""
-    DROP TRIGGER {self.settings.trigger};
-    DROP FUNCTION {self.settings.function};
-    DROP TABLE {self.settings.queue_table};
-    DROP TABLE {self.settings.log_table};
-    DROP TYPE {self.settings.queue_status_type};
-    DROP TYPE {self.settings.log_table_status_type};
-    """
-        )
-
-
-@dataclasses.dataclass
-class PgQueuerQueries:
-    """
-    Handles operations related to job queuing such as
-    enqueueing, dequeueing, and querying the size of the queue.
-    """
-
-    pool: asyncpg.Pool
-    settings: DBSettings = dataclasses.field(default_factory=DBSettings)
+        query = f"""
+            DROP TRIGGER {self.settings.trigger};
+            DROP FUNCTION {self.settings.function};
+            DROP TABLE {self.settings.queue_table};
+            DROP TABLE {self.settings.log_table};
+            DROP TYPE {self.settings.queue_status_type};
+            DROP TYPE {self.settings.log_table_status_type};
+        """
+        await self.pool.execute(query)
 
-    async def dequeue(self) -> models.Jobs:
+    async def dequeue(self) -> models.Job | None:
         """
         Retrieves and updates the next 'queued' job to 'picked'
         status, ensuring no two jobs with the same entrypoint
         are picked simultaneously.
         """
         query = f"""
             WITH next_job AS (
                 SELECT p1.id
                 FROM {self.settings.queue_table} p1
                 WHERE p1.status = 'queued' AND NOT EXISTS (
                     SELECT FROM
                     {self.settings.queue_table} p2
-                    WHERE p1.entrypoint = p2.entrypoint AND p2.status = 'picked')
-                ORDER BY id
+                    WHERE p1.entrypoint = p2.entrypoint AND p2.status = 'picked'
+                )
+                ORDER BY priority, id
                 FOR UPDATE SKIP LOCKED
                 LIMIT 1
             )
             UPDATE {self.settings.queue_table}
             SET status = 'picked'
             WHERE id = ANY(SELECT id FROM next_job)
             RETURNING *;
         """
 
-        return models.Jobs.model_validate(map(dict, await self.pool.fetch(query)))
+        if row := await self.pool.fetchrow(query):
+            return models.Job.model_validate(dict(row))
+        return None
 
     async def enqueue(
         self,
         entrypoint: str,
         payload: bytes | None,
         priority: int = 0,
     ) -> None:
         """
         Inserts a new job into the queue with the specified
         entrypoint, payload, and priority, marking it as 'queued'.
         """
-        await self.pool.execute(
-            f"""
-    INSERT INTO {self.settings.queue_table} (priority, status, entrypoint, payload)
-    VALUES ($1, 'queued', $2, $3)""",
-            priority,
-            entrypoint,
-            payload,
-        )
+        query = f"""
+            INSERT INTO {self.settings.queue_table} (priority, status, entrypoint, payload)
+            VALUES ($1, 'queued', $2, $3)
+        """  # noqa: E501
+
+        await self.pool.execute(query, priority, entrypoint, payload)
 
-    async def clear(self, entrypoint: str | list[str] | None = None) -> None:
+    async def clear_queue(self, entrypoint: str | list[str] | None = None) -> None:
         """
         Clears jobs from the queue, optionally filtering by entrypoint if specified.
         """
         if entrypoint:
+            query = (
+                f"DELETE FROM {self.settings.queue_table} WHERE entrypoint = ANY($1)"
+            )
             await self.pool.execute(
-                f"DELETE FROM {self.settings.queue_table} WHERE entrypoint = ANY($1)",
+                query,
                 [entrypoint] if isinstance(entrypoint, str) else entrypoint,
             )
         else:
-            await self.pool.execute(f"TRUNCATE {self.settings.queue_table}")
+            query = f"TRUNCATE {self.settings.queue_table}"
+            await self.pool.execute(query)
 
-    async def qsize(self) -> dict[tuple[str, int], int]:
+    async def queue_size(self) -> list[models.QueueSize]:
         """
         Returns the number of jobs in the queue grouped by entrypoint and priority.
         """
-        return {
-            (row["entrypoint"], row["priority"]): row["cnt"]
-            for row in await self.pool.fetch(f"""
-        SELECT
-            count(*) AS cnt,
-            priority,
-            entrypoint
-        FROM
-            {self.settings.queue_table}
-        GROUP BY priority, entrypoint
-        """)
-        }
-
-
-@dataclasses.dataclass
-class PgQueuerLogQueries:
-    """
-    Manages operations related to job logging,
-    including moving jobs to a log table, clearing logs,
-    and querying the size of log entries.
-    """
-
-    pool: asyncpg.Pool
-    settings: DBSettings = dataclasses.field(default_factory=DBSettings)
+        query = f"""
+            SELECT
+                count(*) AS count,
+                priority,
+                entrypoint
+            FROM
+                {self.settings.queue_table}
+            GROUP BY priority, entrypoint
+        """
+        return [
+            models.QueueSize.model_validate(dict(x))
+            for x in await self.pool.fetch(query)
+        ]
 
-    async def move_job_log(self, job: models.Job, status: models.STATUS_LOG) -> None:
+    async def log_job(self, job: models.Job, status: models.STATUS_LOG) -> None:
         """
         Moves a completed or failed job from the queue table to the log
         table, recording its final status and duration.
         """
-        await self.pool.execute(
-            f"""
-    WITH moved_row AS (
-        DELETE FROM {self.settings.queue_table}
-        WHERE id = $1
-        RETURNING id, priority, created, entrypoint
-    )
+        query = f"""
+            WITH moved_row AS (
+                DELETE FROM {self.settings.queue_table}
+                WHERE id = $1
+                RETURNING id, priority, created, entrypoint
+            )
 
-    INSERT INTO {self.settings.log_table} (
-        id, priority, created, duration, status, entrypoint
-    )
-        SELECT id, priority, created, NOW() - created, $2, entrypoint
-        FROM moved_row;
-    """,
-            job.id,
-            status,
-        )
+            INSERT INTO {self.settings.log_table} (
+                id, priority, created, duration, status, entrypoint
+            )
+                SELECT id, priority, created, NOW() - created, $2, entrypoint
+                FROM moved_row;
+         """
+        await self.pool.execute(query, job.id, status)
 
-    async def clear(self, entrypoint: str | list[str] | None = None) -> None:
+    async def clear_log(self, entrypoint: str | list[str] | None = None) -> None:
         """
         Clears entries from the job log table, optionally filtering
         by entrypoint if specified.
         """
         if entrypoint:
+            query = f"DELETE FROM {self.settings.log_table} WHERE entrypoint = ANY($1)"
             await self.pool.execute(
-                f"DELETE FROM {self.settings.log_table} WHERE entrypoint = ANY($1)",
+                query,
                 [entrypoint] if isinstance(entrypoint, str) else entrypoint,
             )
         else:
-            await self.pool.execute(f"TRUNCATE {self.settings.log_table}")
+            query = f"TRUNCATE {self.settings.log_table}"
+            await self.pool.execute(query)
 
-    async def qsize(self) -> dict[tuple[str, str, int], int]:
+    async def log_size(self) -> list[models.LogSize]:
         """
         Returns the number of log entries grouped by status, entrypoint, and priority.
         """
-        return {
-            (row["status"], row["entrypoint"], row["priority"]): row["cnt"]
-            for row in await self.pool.fetch(f"""
-        SELECT
-            count(*) AS cnt,
-            status,
-            priority,
-            entrypoint
-        FROM
-            {self.settings.log_table}
-        GROUP BY status, priority, entrypoint
-        """)
-        }
+        query = f"""
+            SELECT
+                count(*) AS count,
+                status,
+                priority,
+                entrypoint
+            FROM
+                {self.settings.log_table}
+            GROUP BY status, priority, entrypoint
+        """
+        return [
+            models.LogSize.model_validate(dict(x)) for x in await self.pool.fetch(query)
+        ]
```

### Comparing `pgqueuer-0.1.0/src/PgQueuer/tm.py` & `pgqueuer-0.2.0/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.1.0/src/PgQueuer.egg-info/PKG-INFO` & `pgqueuer-0.2.0/src/PgQueuer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.1.0
+Version: 0.2.0
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
@@ -32,18 +32,14 @@
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: myst-parser; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 ## PgQueuer
 
 PgQueuer is a minimalist, high-performance job queue library for Python, leveraging the robustness of PostgreSQL. Designed for simplicity and efficiency, PgQueuer uses PostgreSQL's native features like transactions, row locking, and LISTEN/NOTIFY to manage job queues effortlessly.
 
 ### Features
 
@@ -96,45 +92,38 @@
 In this scenario, the system is designed to manage a queue of incoming data messages that need to be processed. Each message is encapsulated as a job, and these jobs are then processed by a designated function linked to an entrypoint. This is typical in systems where large volumes of data are collected continuously, such as telemetry data from IoT devices, logs from web servers, or transaction data in financial systems.
 
 #### Function Description:
 The `fetch` function, tied to the `fetch` entrypoint, is responsible for processing each message. It simulates a processing task by printing the content of each message. This function could be adapted to perform more complex operations such as parsing, analyzing, storing, or forwarding the data as required by the application.
 
 ```python
 import asyncio
-import time
 
 import asyncpg
-
-from PgQueuer import qm, queries
+from PgQueuer.models import Job
+from PgQueuer.qm import QueueManager
 
 
 async def main() -> None:
     # Set up a connection pool with a minimum of 2 connections.
     pool = await asyncpg.create_pool(min_size=2)
     # Initialize the QueueManager with the connection pool and query handler.
-    app = qm.QueueManager(
-        pool, 
-        queries.PgQueuerQueries(pool),
-        queries.PgQueuerLogQueries(pool),
-    )
+    qm = QueueManager(pool)
 
     # Number of messages to simulate.
     N = 10_000
 
     # Enqueue messages.
     for n in range(N):
-        await app.q.enqueue("fetch", f"this is from me: {n}".encode())
+        await qm.queries.enqueue("fetch", f"this is from me: {n}".encode())
 
     # Define a processing function for each message.
-    @c.entrypoint("fetch")
-    async def process_message(context: bytes) -> None:
-        # Simulate parsing the message.
-        message = context.decode()
+    @qm.entrypoint("fetch")
+    async def process_message(job: Job) -> None:
         # Print the message to simulate processing.
-        print(f"Processed message: {message}")
+        print(f"Processed message: {job}")
 
-    await app.run()
+    await qm.run()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `pgqueuer-0.1.0/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.2.0/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.1.0/test/conftest.py` & `pgqueuer-0.2.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.1.0/test/db/Dockerfile` & `pgqueuer-0.2.0/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.1.0/test/test_qm.py` & `pgqueuer-0.2.0/test/test_qm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 import asyncio
 
 import asyncpg
 import pytest
+from PgQueuer.models import Job
 from PgQueuer.qm import QueueManager
-from PgQueuer.queries import PgQueuerQueries
+from PgQueuer.queries import Queries
 
 
 @pytest.mark.parametrize("N", (1, 2, 32, 500))
 async def test_job_queing(
     pgpool: asyncpg.Pool,
     N: int,
 ) -> None:
     c = QueueManager(pgpool)
     seen = list[int]()
 
     @c.entrypoint("fetch")
-    async def fetch(context: bytes | None) -> None:
-        if context is None:
+    async def fetch(context: Job) -> None:
+        if context.payload is None:
             c.alive = False
             return
         assert context
-        seen.append(int(context))
+        seen.append(int(context.payload))
 
     for n in range(N):
-        await c.q.enqueue("fetch", f"{n}".encode())
+        await c.queries.enqueue("fetch", f"{n}".encode())
 
     # Stop flag
-    await c.q.enqueue("fetch", None)
+    await c.queries.enqueue("fetch", None)
 
     await asyncio.wait_for(c.run(), timeout=1)
     assert seen == list(range(N))
 
 
 @pytest.mark.parametrize("N", (1, 2, 32, 512))
 @pytest.mark.parametrize("concurrency", (1, 2, 3, 4))
 async def test_job_fetch(
     pgpool: asyncpg.Pool,
     N: int,
     concurrency: int,
 ) -> None:
-    q = PgQueuerQueries(pgpool)
+    q = Queries(pgpool)
     qmpool = [QueueManager(pgpool) for _ in range(concurrency)]
     seen = list[int]()
 
     for qm in qmpool:
 
         @qm.entrypoint("fetch")
-        async def fetch(context: bytes | None) -> None:
-            if context is None:
+        async def fetch(context: Job) -> None:
+            if context.payload is None:
                 for qm in qmpool:
                     qm.alive = False
                 return
             assert context
-            seen.append(int(context))
+            seen.append(int(context.payload))
 
     for n in range(N):
         await q.enqueue("fetch", f"{n}".encode())
 
     # Stop flag
     await q.enqueue("fetch", None)
```

### Comparing `pgqueuer-0.1.0/test/test_tm.py` & `pgqueuer-0.2.0/test/test_tm.py`

 * *Files identical despite different names*

