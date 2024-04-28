# Comparing `tmp/nonebot_plugin_orm-0.7.1.tar.gz` & `tmp/nonebot_plugin_orm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_orm-0.7.1.tar", last modified: Sun Feb 25 07:06:43 2024, max compression
+gzip compressed data, was "nonebot_plugin_orm-0.7.2.tar", last modified: Sun Apr 28 09:59:24 2024, max compression
```

## Comparing `nonebot_plugin_orm-0.7.1.tar` & `nonebot_plugin_orm-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1078 2024-02-25 07:06:18.005894 nonebot_plugin_orm-0.7.1/LICENSE
--rw-r--r--   0        0        0     7133 2024-02-25 07:06:18.005894 nonebot_plugin_orm-0.7.1/README.md
--rw-r--r--   0        0        0     7191 2024-02-25 07:06:18.005894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/__init__.py
--rw-r--r--   0        0        0     8161 2024-02-25 07:06:18.005894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/__main__.py
--rw-r--r--   0        0        0     1037 2024-02-25 07:06:18.005894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/config.py
--rw-r--r--   0        0        0      416 2024-02-25 07:06:18.005894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/env.py
--rw-r--r--   0        0        0    31802 2024-02-25 07:06:18.005894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/migrate.py
--rw-r--r--   0        0        0     3502 2024-02-25 07:06:18.005894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/model.py
--rw-r--r--   0        0        0     5148 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/param.py
--rw-r--r--   0        0        0        0 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/py.typed
--rw-r--r--   0        0        0       19 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/generic/README
--rw-r--r--   0        0        0        0 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/generic/__init__.py
--rw-r--r--   0        0        0     2476 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/generic/env.py
--rw-r--r--   0        0        0      667 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/generic/script.py.mako
--rw-r--r--   0        0        0        0 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/generic/versions/__init__.py
--rw-r--r--   0        0        0      654 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/multidb/README
--rw-r--r--   0        0        0        0 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/multidb/__init__.py
--rw-r--r--   0        0        0     4426 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/multidb/env.py
--rw-r--r--   0        0        0      957 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/multidb/script.py.mako
--rw-r--r--   0        0        0        0 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/multidb/versions/__init__.py
--rw-r--r--   0        0        0    12946 2024-02-25 07:06:18.009894 nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/utils.py
--rw-r--r--   0        0        0     2119 2024-02-25 07:06:43.749833 nonebot_plugin_orm-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     8801 1970-01-01 00:00:00.000000 nonebot_plugin_orm-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/LICENSE
+-rw-r--r--   0        0        0     7133 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/README.md
+-rw-r--r--   0        0        0     7361 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/__init__.py
+-rw-r--r--   0        0        0     8161 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/__main__.py
+-rw-r--r--   0        0        0     1037 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/config.py
+-rw-r--r--   0        0        0      416 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/env.py
+-rw-r--r--   0        0        0    31862 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/migrate.py
+-rw-r--r--   0        0        0     3502 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/model.py
+-rw-r--r--   0        0        0     5148 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/param.py
+-rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/py.typed
+-rw-r--r--   0        0        0       19 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/README
+-rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/__init__.py
+-rw-r--r--   0        0        0     2476 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/env.py
+-rw-r--r--   0        0        0      667 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/script.py.mako
+-rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/versions/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/README
+-rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/__init__.py
+-rw-r--r--   0        0        0     4426 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/env.py
+-rw-r--r--   0        0        0      957 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/script.py.mako
+-rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/versions/__init__.py
+-rw-r--r--   0        0        0    12946 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/utils.py
+-rw-r--r--   0        0        0     2119 2024-04-28 09:59:24.479448 nonebot_plugin_orm-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     8801 1970-01-01 00:00:00.000000 nonebot_plugin_orm-0.7.2/PKG-INFO
```

### Comparing `nonebot_plugin_orm-0.7.1/LICENSE` & `nonebot_plugin_orm-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/README.md` & `nonebot_plugin_orm-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/__init__.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,16 +79,18 @@
         stdout=StreamToLogger(), cmd_opts=cmd_opts
     ) as alembic_config:
         if plugin_config.alembic_startup_check:
             cmd_opts.cmd = (migrate.check, [], [])
             try:
                 await greenlet_spawn(migrate.check, alembic_config)
             except click.UsageError:
-                logger.error("启动检查失败")
-                raise
+                if not click.confirm("目标数据库未更新到最新迁移, 是否更新?"):
+                    raise
+                cmd_opts.cmd = (migrate.upgrade, [], [])
+                await greenlet_spawn(migrate.upgrade, alembic_config)
         else:
             logger.warning("跳过启动检查, 正在同步数据库模式...")
             cmd_opts.cmd = (migrate.sync, ["revision"], [])
             await greenlet_spawn(migrate.sync, alembic_config)
 
 
 def _init_orm():
@@ -106,25 +108,27 @@
         _session_factory,
         lambda: (id(current_event.get(None)), current_matcher.get(None)),
     )
 
     run_postprocessor(_scoped_sessions.remove)
 
 
-@wraps(lambda: None)  # NOTE: for dependency injection
 def get_session(**local_kw: Any) -> sa_async.AsyncSession:
     try:
         return _session_factory(**local_kw)
     except NameError:
         raise RuntimeError("nonebot-plugin-orm 未初始化") from None
 
 
 # NOTE: NoneBot DI will run sync function in thread pool executor,
 # which is poor performance for this simple function, so we wrap it as a coroutine function.
-AsyncSession = Annotated[sa_async.AsyncSession, Depends(coroutine(get_session))]
+AsyncSession = Annotated[
+    sa_async.AsyncSession,
+    Depends(coroutine(wraps(lambda: None)(get_session)), use_cache=False),
+]
 
 
 def get_scoped_session() -> sa_async.async_scoped_session[sa_async.AsyncSession]:
     try:
         return _scoped_sessions
     except NameError:
         raise RuntimeError("nonebot-plugin-orm 未初始化") from None
```

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/__main__.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/config.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/migrate.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/migrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import sqlalchemy
 from alembic.config import Config
 from sqlalchemy.util import asbool
 from nonebot import logger, get_plugin
 from sqlalchemy import MetaData, Connection
 from alembic.util.editor import open_in_editor
 from alembic.script import Script, ScriptDirectory
+from alembic.util import AutogenerateDiffsDetected
 from alembic.util.langhelpers import rev_id as _rev_id
 from alembic.operations.ops import UpgradeOps, DowngradeOps
 from alembic.migration import StampStep, RevisionStep, MigrationContext
 from alembic.runtime.environment import EnvironmentContext, ProcessRevisionDirectiveFn
 from alembic.autogenerate.api import (
     RevisionContext,
     produce_migrations,
@@ -538,15 +539,15 @@
         revision_context=revision_context,
     ):
         script.run_env()
 
     migration_script = revision_context.generated_revisions[-1]
     diffs = cast(UpgradeOps, migration_script.upgrade_ops).as_diffs()
     if diffs:
-        raise click.UsageError(f"检测到新的升级操作:\n{pformat(diffs)}")
+        raise AutogenerateDiffsDetected(f"检测到新的升级操作:\n{pformat(diffs)}")
     else:
         config.print_stdout("没有检测到新的升级操作")
 
 
 def merge(
     config: AlembicConfig,
     revisions: tuple[str, ...],
```

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/model.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/param.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/param.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/generic/env.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/env.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/generic/script.py.mako` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/script.py.mako`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/multidb/README` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/README`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/multidb/env.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/env.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/templates/multidb/script.py.mako` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/script.py.mako`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/nonebot_plugin_orm/utils.py` & `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.1/pyproject.toml` & `nonebot_plugin_orm-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-orm"
-version = "0.7.1"
+version = "0.7.2"
 description = "SQLAlchemy ORM support for nonebot"
 authors = [
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
     { name = "ProgramRipper", email = "programripper@foxmail.com" },
 ]
 dependencies = [
     "alembic~=1.13",
@@ -42,21 +42,21 @@
 asyncmy = [
     "sqlalchemy[asyncmy]",
 ]
 aiomysql = [
     "sqlalchemy[aiomysql]",
 ]
 postgresql = [
-    "sqlalchemy[postgresql_psycopgbinary]",
+    "sqlalchemy[postgresql-psycopgbinary]",
 ]
 psycopg = [
-    "sqlalchemy[postgresql_psycopgbinary]",
+    "sqlalchemy[postgresql-psycopgbinary]",
 ]
 asyncpg = [
-    "sqlalchemy[postgresql_asyncpg]",
+    "sqlalchemy[postgresql-asyncpg]",
 ]
 sqlite = [
     "sqlalchemy[aiosqlite]",
 ]
 aiosqlite = [
     "sqlalchemy[aiosqlite]",
 ]
```

### Comparing `nonebot_plugin_orm-0.7.1/PKG-INFO` & `nonebot_plugin_orm-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-orm
-Version: 0.7.1
+Version: 0.7.2
 Summary: SQLAlchemy ORM support for nonebot
-Keywords: nonebot orm sqlalchemy
+Keywords: nonebot,orm,sqlalchemy
 Home-page: https://github.com/nonebot/plugin-orm
 Author-Email: yanyongyu <yyy@nonebot.dev>, ProgramRipper <programripper@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonebot/plugin-orm
 Project-URL: Repository, https://github.com/nonebot/plugin-orm
 Project-URL: Documentation, https://github.com/nonebot/plugin-orm
 Requires-Python: <4.0,>=3.8
@@ -18,17 +18,17 @@
 Requires-Dist: nonebot2~=2.2
 Requires-Dist: sqlalchemy~=2.0
 Requires-Dist: typing-extensions~=4.9; python_version < "3.11"
 Requires-Dist: sqlalchemy[aiosqlite]; extra == "default"
 Requires-Dist: sqlalchemy[aiomysql]; extra == "mysql"
 Requires-Dist: sqlalchemy[asyncmy]; extra == "asyncmy"
 Requires-Dist: sqlalchemy[aiomysql]; extra == "aiomysql"
-Requires-Dist: sqlalchemy[postgresql_psycopgbinary]; extra == "postgresql"
-Requires-Dist: sqlalchemy[postgresql_psycopgbinary]; extra == "psycopg"
-Requires-Dist: sqlalchemy[postgresql_asyncpg]; extra == "asyncpg"
+Requires-Dist: sqlalchemy[postgresql-psycopgbinary]; extra == "postgresql"
+Requires-Dist: sqlalchemy[postgresql-psycopgbinary]; extra == "psycopg"
+Requires-Dist: sqlalchemy[postgresql-asyncpg]; extra == "asyncpg"
 Requires-Dist: sqlalchemy[aiosqlite]; extra == "sqlite"
 Requires-Dist: sqlalchemy[aiosqlite]; extra == "aiosqlite"
 Provides-Extra: default
 Provides-Extra: mysql
 Provides-Extra: asyncmy
 Provides-Extra: aiomysql
 Provides-Extra: postgresql
```

