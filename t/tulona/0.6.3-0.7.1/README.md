# Comparing `tmp/tulona-0.6.3.tar.gz` & `tmp/tulona-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.6.3.tar", last modified: Fri Apr 26 15:59:52 2024, max compression
+gzip compressed data, was "tulona-0.7.1.tar", last modified: Sun Apr 28 12:16:12 2024, max compression
```

## Comparing `tulona-0.6.3.tar` & `tulona-0.7.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.600799 tulona-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:59:48.000000 tulona-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-26 15:59:52.600799 tulona-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-04-26 15:59:48.000000 tulona-0.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.592799 tulona-0.6.3/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.600799 tulona-0.6.3/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22856 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16443 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.600799 tulona-0.6.3/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.600799 tulona-0.6.3/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-26 15:59:48.000000 tulona-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:59:52.600799 tulona-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.756604 tulona-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-28 12:16:03.000000 tulona-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-04-28 12:16:12.756604 tulona-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13003 2024-04-28 12:16:03.000000 tulona-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.748604 tulona-0.7.1/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.748604 tulona-0.7.1/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.752604 tulona-0.7.1/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.752604 tulona-0.7.1/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.752604 tulona-0.7.1/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.752604 tulona-0.7.1/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.752604 tulona-0.7.1/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.756604 tulona-0.7.1/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-28 12:16:03.000000 tulona-0.7.1/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:16:12.756604 tulona-0.7.1/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-04-28 12:16:12.000000 tulona-0.7.1/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-28 12:16:12.000000 tulona-0.7.1/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:16:12.000000 tulona-0.7.1/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 12:16:12.000000 tulona-0.7.1/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-28 12:16:12.000000 tulona-0.7.1/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 12:16:12.000000 tulona-0.7.1/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-28 12:16:03.000000 tulona-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:16:12.756604 tulona-0.7.1/setup.cfg
```

### Comparing `tulona-0.6.3/LICENSE` & `tulona-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/PKG-INFO` & `tulona-0.7.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.6.3
+Version: 0.7.1
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -41,14 +41,18 @@
    * - Testing
      - |CI Test| |Deployment| |Coverage|
    * - Package
      - |PyPI Latest Release| |PyPI Downloads|
    * - Meta
      - |License Apache-2.0| |Codestyle Black|
 
+Functionality
+-------------
+The basic functionality of `tulona` is to compare datasets, write them into Excel files and highlight the mismatches.
+
 
 Connection Profiles
 -------------------
 Connection profiles is a `yaml` file that will store credentials and other details to connect to the databases/data sources.
 
 It must be setup in `profiles.yml` file and it must be placed under `$HOME/.tulona` dierctory.
 Create a directory named `.tulona` under your home directory and place `profiles.yml` under it.
@@ -101,51 +105,55 @@
 
   version: '2.0'
   name: integration_project
   config_version: 1
 
   outdir: output # the folder comparison result is written into
 
+  # Datasource names must be unique
   datasources:
     employee_postgres:
       connection_profile: pgdb
-      database: postgres
-      schema: public
+      database: postgresdb
+      schema: corporate
       table: employee
-      primary_key: employee_id
-      exclude_columns:  # optional
+      primary_key: Employee_ID
+      exclude_columns:
         - name
-      compare_column: Employee_ID  # conditional optional
+      compare_column: Employee_ID
     employee_mysql:
       connection_profile: mydb
-      database: db
-      schema: db
+      schema: corporate
       table: employee
-      primary_key: employee_id
-      exclude_columns:  # optional
+      primary_key: Employee_ID
+      exclude_columns:
         - phone_number
-      compare_column: Employee_ID  # conditional optional
+      compare_column: Employee_ID
     person_postgres:
       connection_profile: pgdb
-      database: postgres
-      schema: public
+      database: postgresdb
+      schema: corporate
       table: people_composite_key
       primary_key:
         - ID_1
         - ID_2
+      # exclude_columns:
+      #   - name
       compare_column:
         - ID_1
         - ID_2
     person_mysql:
       connection_profile: mydb
-      schema: db
+      schema: corporate
       table: people_composite_key
       primary_key:
         - ID_1
         - ID_2
+      # exclude_columns:
+      #   - phone_number
       compare_column:
         - ID_1
         - ID_2
     postgresdb_postgres:
       connection_profile: pgdb
       database: postgresdb
     none_mysql:
@@ -155,41 +163,124 @@
       database: postgresdb
       schema: corporate_copy
     none_mysql_schema:
       connection_profile: mydb
       schema: corporate
     employee_postgres_query:
       connection_profile: pgdb
+      database: postgresdb
+      schema: corporate
       query: select * from postgresdb.corporate.employee
       primary_key: Employee_ID
+      exclude_columns:
+        - name
       compare_column: Employee_ID
     employee_mysql_query:
       connection_profile: mydb
+      schema: corporate
       query: select * from corporate.employee
       primary_key: Employee_ID
+      exclude_columns:
+        - phone_number
       compare_column: Employee_ID
 
-  # List of lists
-  # The inner lists have datasources that need to be used for tasks like comparison
-  # For example employee_postgres vs employee_mysql. So a [employee_postgres, employee_mysql]
-  # Outer list is a list of those combinations.
-  # So like: [[employee_postgres, employee_mysql], [datasource3, datasource4]]
-  source_map:
-    - - employee_postgres
-      - employee_mysql
-    - - person_postgres
-      - person_mysql
-    - - employee_postgres_query
-      - employee_mysql_query
+  # List of task configs(Dict)
+  # Depending on the accepted params, task config can have different params
+  # The value for that `task` key is the name of the command you want to run
+  task_config:
+    - task: ping
+      datasources:
+        - person_postgres
+        - none_mysql
+        - employee_mysql_query
+
+    - task: profile
+      datasources:
+        - employee_postgres
+        - employee_mysql
+
+    - task: profile
+      datasources:
+        - person_postgres
+        - person_mysql
+      compare: true
+
+    - task: compare-row
+      datasources:
+        - employee_postgres
+        - employee_mysql
+      sample_count: 30
+
+    - task: compare-row
+      datasources:
+        - employee_postgres
+        - employee_mysql
+
+    - task: compare-row
+      datasources:
+        - employee_postgres_query
+        - employee_mysql_query
+
+    - task: compare-column
+      datasources:
+        - employee_postgres
+        - employee_mysql
+
+    - task: compare-column
+      datasources:
+        - person_postgres
+        - person_mysql
+      composite: false # If it's false, specifying it is optional
+
+    - task: compare-column
+      datasources:
+        - person_postgres
+        - person_mysql
+      composite: true
+
+    - task: compare
+      datasources:
+        - employee_postgres
+        - employee_mysql
+      composite: true
+
+    - task: compare
+      datasources:
+        - person_postgres
+        - person_mysql
+      composite: true
+      sample_count: 30
+
+    - task: scan
+      datasources:
+        - postgresdb_postgres_schema
+
+    - task: scan
+      datasources:
+        - postgresdb_postgres
+        - none_mysql
+      compare: false
+
+    - task: scan
+      datasources:
+        - postgresdb_postgres_schema
+        - none_mysql_schema
+      compare: true
+
+    - task: scan
+      datasources:
+        - postgresdb_postgres
+        - none_mysql
+      compare: true
 
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
-All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
+If you don't setup `task_config`, all commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
 Tulona has following commands available:
 
 * **ping**: To test connectivity to the databases for the datasources. Sample command:
 
   * To ping one data source pass the name to the `--datasources` parameter:
 
@@ -209,63 +300,82 @@
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
+  * Sample output will be something like this:
+
+    |profile|
+
 * **compare-row**: To compare sample data from two sources/tables/queries. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
     ``tulona compare-row --datasources employee_postgres,employee_mysql``
 
   * Command with `--sample-count` parameter:
 
     ``tulona compare-row --sample-count 50 --datasources employee_postgres,employee_mysql``
 
   * Compare queries instead of tables, useful when you want to compare resutls of two queries:
 
     ``tulona compare-row --datasources employee_postgres_query,employee_mysql_query``
 
+  * Sample output will be something like this:
+
+    |compare_row|
+
 * **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
   * Column[s] to compare is[are] specified in `tulona-project.yml` file as part of datasource configs, with `compare_column` property. Sample command:
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
 
   * Compare multiples columns as composite key (combination of column values will be compared) with additional `--composite` flag:
 
     ``tulona compare-column --composite --datasources employee_postgres,employee_mysql``
 
+  * Sample output will be something like this:
+
+    |compare_column|
+
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
 * **scan**: To scan and compare databases or schemas in terms of metadata and tables present if you want to compare all tables and don't want to set up datasource config for all of them. Sample commands:
 
   * Scan without comparing:
 
     ``tulona scan --datasources postgresdb_postgres_schema,none_mysql_schema``
 
   * Scan and compare:
 
     ``tulona scan --compare --datasources postgresdb_postgres_schema,none_mysql_schema``
 
+* **run**: To execute all the tasks defined in the `task_config` section. Sample command:
+
+    ``tulona run``
 
-From `tulona v0.4.0` a new project config property has been introduced: `source_map`. If this config is set, in the project config file (tulona-project.yml), then `--datasources` parameter can be skipped with commands.
-For example this command:
+If you setup `task_config`, there is no need to pass the `--datasources` parameter.
+In that case the following command (to compare some datasoruces):
 
 ``tulona compare --datasources employee_postgres,employee_mysql``
 
 will become this:
 
 ``tulona compare``
 
-Please look at the sample project config from above to understand how to use `source_map` property.
+and it will run all the `compare` tasks defined in the `task_config` section. From our example project config file above, it will run 2 `compare` tasks.
+
+Also setting up `task_config` can be greatly benificial as you can set up different instance of same/different tasks with different config to execute in one go with the `run` command.
+
+Please look at the sample project config from above to understand how to set up `task_config` property.
 
 For debug level log, add `-v` or `--verbose` flag along with any command. For example:
 
 ``tulona ping -v --datasources employee_postgres``
 
 To know more about any specific command, execute `tulona <command> -h`.
 
@@ -280,14 +390,22 @@
 * Execute `python -m build`.
 
 Install wheel executable file
 -----------------------------
 * Execute `pip install <wheel-file.whl>`
 
 
+.. |profile| image:: images/profile.png
+  :alt: Profile output
+.. |compare_row| image:: images/compare_row.png
+  :alt: Row comparison output
+.. |compare_column| image:: images/compare_column.png
+  :alt: Column comparison output
+
+
 .. |CI Test| image:: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml
 .. |Deployment| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml
 .. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/graph/badge.svg?token=UGNjjgRskE
    :target: https://codecov.io/gh/mrinalsardar/tulona
    :alt: Coverage status
```

### Comparing `tulona-0.6.3/README.rst` & `tulona-0.7.1/core/tulona.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,58 @@
+Metadata-Version: 2.1
+Name: tulona
+Version: 0.7.1
+Summary: A tool to compare data from different sources.
+Author: Mrinal Kanti Sardar
+Project-URL: Homepage, https://github.com/mrinalsardar/tulona
+Project-URL: Documentation, https://github.com/mrinalsardar/tulona
+Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
+Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
+Keywords: tulona,comparison,data comparison,database scan,database profile
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: click~=8.1
+Requires-Dist: ruamel.yaml~=0.18
+Requires-Dist: psycopg2-binary~=2.9
+Requires-Dist: pymysql~=1.1
+Requires-Dist: cryptography~=42.0
+Requires-Dist: snowflake-sqlalchemy~=1.5
+Requires-Dist: pyodbc~=5.1
+Requires-Dist: pandas~=1.5
+Requires-Dist: openpyxl~=3.1
+Requires-Dist: Jinja2~=3.1
+Requires-Dist: pydantic~=2.7
+
 Tulona
 ======
 A utility to compare tables, espacially useful to perform validations for migration projects.
 
 .. list-table::
    :widths: 50 200
 
    * - Testing
      - |CI Test| |Deployment| |Coverage|
    * - Package
      - |PyPI Latest Release| |PyPI Downloads|
    * - Meta
      - |License Apache-2.0| |Codestyle Black|
 
+Functionality
+-------------
+The basic functionality of `tulona` is to compare datasets, write them into Excel files and highlight the mismatches.
+
 
 Connection Profiles
 -------------------
 Connection profiles is a `yaml` file that will store credentials and other details to connect to the databases/data sources.
 
 It must be setup in `profiles.yml` file and it must be placed under `$HOME/.tulona` dierctory.
 Create a directory named `.tulona` under your home directory and place `profiles.yml` under it.
@@ -68,51 +105,55 @@
 
   version: '2.0'
   name: integration_project
   config_version: 1
 
   outdir: output # the folder comparison result is written into
 
+  # Datasource names must be unique
   datasources:
     employee_postgres:
       connection_profile: pgdb
-      database: postgres
-      schema: public
+      database: postgresdb
+      schema: corporate
       table: employee
-      primary_key: employee_id
-      exclude_columns:  # optional
+      primary_key: Employee_ID
+      exclude_columns:
         - name
-      compare_column: Employee_ID  # conditional optional
+      compare_column: Employee_ID
     employee_mysql:
       connection_profile: mydb
-      database: db
-      schema: db
+      schema: corporate
       table: employee
-      primary_key: employee_id
-      exclude_columns:  # optional
+      primary_key: Employee_ID
+      exclude_columns:
         - phone_number
-      compare_column: Employee_ID  # conditional optional
+      compare_column: Employee_ID
     person_postgres:
       connection_profile: pgdb
-      database: postgres
-      schema: public
+      database: postgresdb
+      schema: corporate
       table: people_composite_key
       primary_key:
         - ID_1
         - ID_2
+      # exclude_columns:
+      #   - name
       compare_column:
         - ID_1
         - ID_2
     person_mysql:
       connection_profile: mydb
-      schema: db
+      schema: corporate
       table: people_composite_key
       primary_key:
         - ID_1
         - ID_2
+      # exclude_columns:
+      #   - phone_number
       compare_column:
         - ID_1
         - ID_2
     postgresdb_postgres:
       connection_profile: pgdb
       database: postgresdb
     none_mysql:
@@ -122,41 +163,124 @@
       database: postgresdb
       schema: corporate_copy
     none_mysql_schema:
       connection_profile: mydb
       schema: corporate
     employee_postgres_query:
       connection_profile: pgdb
+      database: postgresdb
+      schema: corporate
       query: select * from postgresdb.corporate.employee
       primary_key: Employee_ID
+      exclude_columns:
+        - name
       compare_column: Employee_ID
     employee_mysql_query:
       connection_profile: mydb
+      schema: corporate
       query: select * from corporate.employee
       primary_key: Employee_ID
+      exclude_columns:
+        - phone_number
       compare_column: Employee_ID
 
-  # List of lists
-  # The inner lists have datasources that need to be used for tasks like comparison
-  # For example employee_postgres vs employee_mysql. So a [employee_postgres, employee_mysql]
-  # Outer list is a list of those combinations.
-  # So like: [[employee_postgres, employee_mysql], [datasource3, datasource4]]
-  source_map:
-    - - employee_postgres
-      - employee_mysql
-    - - person_postgres
-      - person_mysql
-    - - employee_postgres_query
-      - employee_mysql_query
+  # List of task configs(Dict)
+  # Depending on the accepted params, task config can have different params
+  # The value for that `task` key is the name of the command you want to run
+  task_config:
+    - task: ping
+      datasources:
+        - person_postgres
+        - none_mysql
+        - employee_mysql_query
+
+    - task: profile
+      datasources:
+        - employee_postgres
+        - employee_mysql
+
+    - task: profile
+      datasources:
+        - person_postgres
+        - person_mysql
+      compare: true
+
+    - task: compare-row
+      datasources:
+        - employee_postgres
+        - employee_mysql
+      sample_count: 30
+
+    - task: compare-row
+      datasources:
+        - employee_postgres
+        - employee_mysql
+
+    - task: compare-row
+      datasources:
+        - employee_postgres_query
+        - employee_mysql_query
+
+    - task: compare-column
+      datasources:
+        - employee_postgres
+        - employee_mysql
+
+    - task: compare-column
+      datasources:
+        - person_postgres
+        - person_mysql
+      composite: false # If it's false, specifying it is optional
+
+    - task: compare-column
+      datasources:
+        - person_postgres
+        - person_mysql
+      composite: true
+
+    - task: compare
+      datasources:
+        - employee_postgres
+        - employee_mysql
+      composite: true
+
+    - task: compare
+      datasources:
+        - person_postgres
+        - person_mysql
+      composite: true
+      sample_count: 30
+
+    - task: scan
+      datasources:
+        - postgresdb_postgres_schema
+
+    - task: scan
+      datasources:
+        - postgresdb_postgres
+        - none_mysql
+      compare: false
+
+    - task: scan
+      datasources:
+        - postgresdb_postgres_schema
+        - none_mysql_schema
+      compare: true
+
+    - task: scan
+      datasources:
+        - postgresdb_postgres
+        - none_mysql
+      compare: true
 
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
-All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
+If you don't setup `task_config`, all commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
 Tulona has following commands available:
 
 * **ping**: To test connectivity to the databases for the datasources. Sample command:
 
   * To ping one data source pass the name to the `--datasources` parameter:
 
@@ -176,63 +300,82 @@
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
+  * Sample output will be something like this:
+
+    |profile|
+
 * **compare-row**: To compare sample data from two sources/tables/queries. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
     ``tulona compare-row --datasources employee_postgres,employee_mysql``
 
   * Command with `--sample-count` parameter:
 
     ``tulona compare-row --sample-count 50 --datasources employee_postgres,employee_mysql``
 
   * Compare queries instead of tables, useful when you want to compare resutls of two queries:
 
     ``tulona compare-row --datasources employee_postgres_query,employee_mysql_query``
 
+  * Sample output will be something like this:
+
+    |compare_row|
+
 * **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
   * Column[s] to compare is[are] specified in `tulona-project.yml` file as part of datasource configs, with `compare_column` property. Sample command:
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
 
   * Compare multiples columns as composite key (combination of column values will be compared) with additional `--composite` flag:
 
     ``tulona compare-column --composite --datasources employee_postgres,employee_mysql``
 
+  * Sample output will be something like this:
+
+    |compare_column|
+
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
 * **scan**: To scan and compare databases or schemas in terms of metadata and tables present if you want to compare all tables and don't want to set up datasource config for all of them. Sample commands:
 
   * Scan without comparing:
 
     ``tulona scan --datasources postgresdb_postgres_schema,none_mysql_schema``
 
   * Scan and compare:
 
     ``tulona scan --compare --datasources postgresdb_postgres_schema,none_mysql_schema``
 
+* **run**: To execute all the tasks defined in the `task_config` section. Sample command:
 
-From `tulona v0.4.0` a new project config property has been introduced: `source_map`. If this config is set, in the project config file (tulona-project.yml), then `--datasources` parameter can be skipped with commands.
-For example this command:
+    ``tulona run``
+
+If you setup `task_config`, there is no need to pass the `--datasources` parameter.
+In that case the following command (to compare some datasoruces):
 
 ``tulona compare --datasources employee_postgres,employee_mysql``
 
 will become this:
 
 ``tulona compare``
 
-Please look at the sample project config from above to understand how to use `source_map` property.
+and it will run all the `compare` tasks defined in the `task_config` section. From our example project config file above, it will run 2 `compare` tasks.
+
+Also setting up `task_config` can be greatly benificial as you can set up different instance of same/different tasks with different config to execute in one go with the `run` command.
+
+Please look at the sample project config from above to understand how to set up `task_config` property.
 
 For debug level log, add `-v` or `--verbose` flag along with any command. For example:
 
 ``tulona ping -v --datasources employee_postgres``
 
 To know more about any specific command, execute `tulona <command> -h`.
 
@@ -247,22 +390,30 @@
 * Execute `python -m build`.
 
 Install wheel executable file
 -----------------------------
 * Execute `pip install <wheel-file.whl>`
 
 
+.. |profile| image:: images/profile.png
+  :alt: Profile output
+.. |compare_row| image:: images/compare_row.png
+  :alt: Row comparison output
+.. |compare_column| image:: images/compare_column.png
+  :alt: Column comparison output
+
+
 .. |CI Test| image:: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml
 .. |Deployment| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml
 .. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/graph/badge.svg?token=UGNjjgRskE
    :target: https://codecov.io/gh/mrinalsardar/tulona
    :alt: Coverage status
 .. |PyPI Latest Release| image:: https://img.shields.io/pypi/v/tulona.svg
    :target: https://pypi.python.org/pypi/tulona/
 .. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/tulona.svg?label=PyPI%20downloads
    :target: https://pypi.org/project/tulona/
 .. |License Apache-2.0| image:: https://img.shields.io/:license-Apache%202-brightgreen.svg
    :target: http://www.apache.org/licenses/LICENSE-2.0.txt
 .. |Codestyle Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
+   :target: https://github.com/psf/black
```

### Comparing `tulona-0.6.3/core/tulona/adapter/connection.py` & `tulona-0.7.1/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/adapter/mssql.py` & `tulona-0.7.1/core/tulona/adapter/mssql.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Dict
 
 from sqlalchemy import create_engine
 from sqlalchemy.engine import URL
 
-from tulona.exceptions import TulonaMissingPropertyError
-
 
 def get_mssql_engine(conn_profile: Dict):
     if "connection_string" in conn_profile:
         connection_string = conn_profile["connection_string"]
         url = URL.create("mssql+pyodbc", query={"odbc_connect": connection_string})
         engine = create_engine(url)
 
     # validate properties
     if "connection_string" not in conn_profile:
-        mandaory_properties = {"driver_version", "server", "database"}
-        if len(mandaory_properties.intersection(set(conn_profile.keys()))) != len(
-            mandaory_properties
-        ):
-            raise TulonaMissingPropertyError(
-                f"One or more of {mandaory_properties} connection propertie[s] is/are missing"
-            )
+        raise NotImplementedError(
+            "Please use 'connection_string' property to connect to Microsoft SQL Server"
+        )
+        # mandaory_properties = {"driver_version", "server", "database"}
+        # if len(mandaory_properties.intersection(set(conn_profile.keys()))) != len(
+        #     mandaory_properties
+        # ):
+        #     raise TulonaMissingPropertyError(
+        #         f"One or more of {mandaory_properties} connection propertie[s] is/are missing"
+        #     )
 
     return engine
```

### Comparing `tulona-0.6.3/core/tulona/adapter/mysql.py` & `tulona-0.7.1/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/adapter/postgres.py` & `tulona-0.7.1/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/adapter/snowflake.py` & `tulona-0.7.1/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/cli/params.py` & `tulona-0.7.1/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/config/profile.py` & `tulona-0.7.1/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/config/project.py` & `tulona-0.7.1/core/tulona/config/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,29 @@
 class ProjectModel(BaseModel):
     version: str
     name: str
     config_version: int = 1
     engine: str = "pandas"
     outdir: str = "output"
     datasources: Dict
-    source_map: List[List] = list()
+    task_config: List[Dict] = list()
 
 
 class Project:
     @property
     def get_project_root(self):
         return Path().absolute()
 
     @property
     def project_conf_path(self) -> str:
         return Path(self.get_project_root, PROJECT_FILE_NAME)
 
     def validate_project_config(self, project_dict_raw: Dict) -> bool:
+        log.debug(f'task_config: {project_dict_raw["task_config"]}')
+
         try:
             _ = ProjectModel(**project_dict_raw)
         except TulonaInvalidProjectConfigError as exc:
             raise TulonaInvalidProjectConfigError(exc)
 
     def load_project_config(self) -> None:
         project_file_uri = self.project_conf_path
```

### Comparing `tulona-0.6.3/core/tulona/exceptions.py` & `tulona-0.7.1/core/tulona/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,7 +62,14 @@
 
 
 class TulonaFundamentalError(Exception):
     def __init__(self, message: str):
         self.message = message
         self.formatted_message = f"ERROR: {self.message}"
         super().__init__(self.formatted_message)
+
+
+class TulonaUnSupportedTaskError(Exception):
+    def __init__(self, message: str):
+        self.message = message
+        self.formatted_message = f"ERROR: {self.message}"
+        super().__init__(self.formatted_message)
```

### Comparing `tulona-0.6.3/core/tulona/task/base.py` & `tulona-0.7.1/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/task/compare.py` & `tulona-0.7.1/core/tulona/task/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,14 @@
             if "query" in ds_config and "table" in ds_config:
                 raise AttributeError(
                     "Both 'query' and 'table' cannot be specified in datasource config"
                 )
 
             if "query" in ds_config:
                 econf_dict["queries"].append(ds_config["query"])
-                if "exclude_columns" in ds_config:
-                    log.warning(
-                        "Attribute 'exclude_columns' doesn't have any effect"
-                        " with attribute 'query'"
-                    )
-                econf_dict["exclude_columns_lol"].append([])
                 if "schema" in ds_config:
                     log.warning(
                         "Attribute 'schema' doesn't have any effect"
                         " with attribute 'query'"
                     )
                 if "table_fqns" in econf_dict:
                     if len(econf_dict["table_fqns"]) > 0:
@@ -120,21 +114,14 @@
 
                 table_fqn = get_table_fqn(
                     database,
                     schema,
                     table,
                 )
 
-                exclude_columns = (
-                    ds_config["exclude_columns"] if "exclude_columns" in ds_config else []
-                )
-                if isinstance(exclude_columns, str):
-                    exclude_columns = [exclude_columns]
-                econf_dict["exclude_columns_lol"].append(exclude_columns)
-
                 econf_dict["table_fqns"].append(table_fqn)
                 if "queries" in econf_dict:
                     if len(econf_dict["queries"]) > 0:
                         raise AttributeError(
                             "Same attribute from 'query' and 'table' has to be"
                             " specified in all candidate datasource confgis"
                         )
@@ -142,14 +129,21 @@
                         econf_dict.pop("queries")
             else:
                 raise TulonaMissingPropertyError(
                     "Either 'table' for 'query' must be specified"
                     "in datasource config for row comparison."
                 )
 
+            exclude_columns = (
+                ds_config["exclude_columns"] if "exclude_columns" in ds_config else []
+            )
+            if isinstance(exclude_columns, str):
+                exclude_columns = [exclude_columns]
+            econf_dict["exclude_columns_lol"].append(exclude_columns)
+
             log.debug(f"Acquiring connection to the database of: {ds_name}")
             connection_profile = get_connection_profile(self.profile, ds_config)
             conman = self.get_connection_manager(conn_profile=connection_profile)
             econf_dict["connection_managers"].append(conman)
 
             if "primary_key" in ds_config:
                 ds_pk = (
@@ -204,14 +198,15 @@
             raise ValueError("Data comparison needs two data sources.")
 
         # Config extraction
         econf_dict = self.extract_confs()
         dbtype1, dbtype2 = econf_dict["dbtypes"]
         if "table_fqns" in econf_dict:
             table_fqn1, table_fqn2 = econf_dict["table_fqns"]
+            log.debug(f"Sample count: {self.sample_count}")
         else:
             query1, query2 = econf_dict["queries"]
         exclude_columns1, exclude_columns2 = econf_dict["exclude_columns_lol"]
         conman1, conman2 = econf_dict["connection_managers"]
 
         # TODO: push column exclusion down to the database/query
         # TODO: We probably don't need to create pk tuple out of pk
@@ -225,55 +220,58 @@
         while i < num_try:
             log.debug(f"Extraction iteration: {i + 1}/{num_try}")
 
             if "table_fqns" in econf_dict:
                 query1 = get_table_data_query(
                     dbtype1, table_fqn1, self.sample_count, query_expr
                 )
-            if self.sample_count < 51:
-                sanitized_query1 = re.sub(r"\(.*\)", "(...)", query1)
-                log.debug(f"Executing query: {sanitized_query1}")
+
+            sanitized_query1 = re.sub(r"where(.*)\(.*\)", r"where\g<1>(...)", query1)
+            log.debug(f"Executing query: {sanitized_query1}")
             df1 = get_query_output_as_df(connection_manager=conman1, query_text=query1)
             if df1.shape[0] == 0:
                 raise ValueError(f"Table {table_fqn1} doesn't have any data")
 
             df1 = df1.rename(columns={c: c.lower() for c in df1.columns})
             for k in primary_key:
                 if k not in df1.columns.tolist():
                     raise ValueError(f"Primary key {k} not present in {table_fqn1}")
 
             # Exclude columns
             if len(exclude_columns1) > 0:
-                log.debug(f"Excluding columns from {table_fqn1}: {exclude_columns1}")
+                log.debug(
+                    f"Excluding columns from {econf_dict['ds_names'][0]}: {exclude_columns1}"
+                )
                 df1 = apply_column_exclusion(
-                    df1, primary_key, exclude_columns1, table_fqn1
+                    df1, primary_key, exclude_columns1, econf_dict["ds_names"][0]
                 )
             if "table_fqns" in econf_dict:
                 query2 = get_table_data_query(
                     dbtype2,
                     table_fqn2,
                     self.sample_count,
                     query_expr=build_filter_query_expression(df1, primary_key),
                 )
-            if self.sample_count < 51:
-                sanitized_query2 = re.sub(r"\(.*\)", "(...)", query2)
-                log.debug(f"Executing query: {sanitized_query2}")
+            sanitized_query2 = re.sub(r"where(.*)\(.*\)", r"where\g<1>(...)", query2)
+            log.debug(f"Executing query: {sanitized_query2}")
 
             df2 = get_query_output_as_df(connection_manager=conman2, query_text=query2)
             df2 = df2.rename(columns={c: c.lower() for c in df2.columns})
 
             for k in primary_key:
                 if k not in df2.columns.tolist():
                     raise ValueError(f"Primary key {k} not present in {table_fqn2}")
 
             # Exclude columns
             if len(exclude_columns2) > 0:
-                log.debug(f"Excluding columns from {table_fqn2}: {exclude_columns2}")
+                log.debug(
+                    f"Excluding columns from {econf_dict['ds_names'][1]}: {exclude_columns2}"
+                )
                 df2 = apply_column_exclusion(
-                    df2, primary_key, exclude_columns2, table_fqn2
+                    df2, primary_key, exclude_columns2, econf_dict["ds_names"][1]
                 )
 
             if df2.shape[0] > 0:
                 for k in primary_key:
                     df1 = df1[df1[k].isin(df2[k].tolist())]
                 row_data_list = [df1, df2]
                 break
```

### Comparing `tulona-0.6.3/core/tulona/task/helper.py` & `tulona-0.7.1/core/tulona/task/helper.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/task/ping.py` & `tulona-0.7.1/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/task/profile.py` & `tulona-0.7.1/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/task/scan.py` & `tulona-0.7.1/core/tulona/task/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from copy import deepcopy
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, List, Union
 
 from tulona.config.runtime import RunConfig
-from tulona.exceptions import TulonaMissingPropertyError
+from tulona.exceptions import TulonaMissingPropertyError, TulonaUnSupportedTaskError
 from tulona.task.base import BaseTask
 from tulona.task.compare import CompareTask
 from tulona.task.helper import perform_comparison
 from tulona.util.excel import dataframes_into_excel
 from tulona.util.filesystem import create_dir_if_not_exist
 from tulona.util.profiles import extract_profile_name, get_connection_profile
 from tulona.util.sql import get_query_output_as_df
@@ -37,29 +37,33 @@
     final_outdir: Union[Path, str]
     compare: bool = DEFAULT_VALUES["compare_scans"]
     sample_count: int = DEFAULT_VALUES["sample_count"]
     composite: bool = DEFAULT_VALUES["compare_column_composite"]
 
     def execute(self):
         log.info(f"Starting task: scan{' --compare' if self.compare else ''}")
-        log.debug(f"Datasource: {self.datasources}")
-        log.debug(f"Compare: {self.compare}")
         log.debug(f"Full output directory: {self.final_outdir}")
         start_time = time.time()
 
         scan_result = {}
         ds_name_compressed_list = []
         connection_profile_names = []
         primary_keys = []
         ds_config_list = []
         for ds_name in self.datasources:
             log.info(f"Processing datasource {ds_name}")
             ds_compressed = ds_name.replace("_", "")
             ds_name_compressed_list.append(ds_compressed)
             ds_config = self.project["datasources"][ds_name]
+            if "table" in ds_config or "query" in ds_config:
+                raise TulonaUnSupportedTaskError(
+                    "Scan doesn't work on table/query."
+                    " Please use one of the following tasks:"
+                    " profile, compare-row, compare-column, compare"
+                )
             ds_config_list.append(ds_config)
             scan_result[ds_name] = {}
             scan_result[ds_name]["database"] = {}
             scan_result[ds_name]["schema"] = {}
             if "primary_key" in ds_config:
                 primary_keys.append(ds_config["primary_key"])
```

### Comparing `tulona-0.6.3/core/tulona/util/database.py` & `tulona-0.7.1/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/util/dataframe.py` & `tulona-0.7.1/core/tulona/util/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 from tulona.exceptions import TulonaFundamentalError
 
 
 def apply_column_exclusion(
     df: pd.DataFrame,
     primary_key: Union[List, Tuple, str],
     exclude_columns: list,
-    table: str,
+    ds_name: str,
 ) -> Union[pd.DataFrame, None]:
     for k in primary_key:
         if k in exclude_columns:
             raise TulonaFundamentalError(
                 f"Cannot exclude primary key/join key {k} from comparison"
             )
 
     missing_cols = []
     for col in exclude_columns:
         if col not in df.columns.tolist():
             missing_cols.append(col)
 
     if len(missing_cols) > 0:
         raise ValueError(
-            f"Columns [{missing_cols}] to be excluded are not present in {table}"
+            f"Columns [{missing_cols}] to be excluded are not present in {ds_name}"
         )
 
     df = df.drop(columns=exclude_columns)
     return df
```

### Comparing `tulona-0.6.3/core/tulona/util/excel.py` & `tulona-0.7.1/core/tulona/util/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,13 +80,13 @@
                         row[col_idx + i].border = right_border
                     else:
                         row[col_idx + i].border = middle_border
 
     wb.save(excel_file)
 
 
-def dataframes_into_excel(
+def dataframes_into_excel(  # pargma: no cover
     sheet_df_map: Dict, outfile_fqn: Union[Path, str], mode: str
 ) -> None:
     with pd.ExcelWriter(outfile_fqn, mode=mode) as writer:
         for sheet, df in sheet_df_map.items():
             df.to_excel(writer, sheet_name=sheet, index=False)
```

### Comparing `tulona-0.6.3/core/tulona/util/profiles.py` & `tulona-0.7.1/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona/util/sql.py` & `tulona-0.7.1/core/tulona/util/sql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/core/tulona.egg-info/SOURCES.txt` & `tulona-0.7.1/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.6.3/pyproject.toml` & `tulona-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.6.3"
+version = "0.7.1"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -111,15 +111,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.6.3"
+current_version = "0.7.1"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
```

