# Comparing `tmp/think_sql-0.7.4.tar.gz` & `tmp/think_sql-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "think_sql-0.7.4.tar", max compression
+gzip compressed data, was "think_sql-0.7.5.tar", max compression
```

## Comparing `think_sql-0.7.4.tar` & `think_sql-0.7.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1381 2024-04-26 06:29:53.818504 think_sql-0.7.4/pyproject.toml
--rw-r--r--   0        0        0    16301 2024-04-16 02:14:07.551128 think_sql-0.7.4/README.md
--rw-r--r--   0        0        0     1139 2024-04-19 08:37:22.016945 think_sql-0.7.4/think_sql/__init__.py
--rw-r--r--   0        0        0       70 2024-04-15 09:26:44.219328 think_sql-0.7.4/think_sql/dm/__init__.py
--rw-r--r--   0        0        0     4689 2024-04-18 06:56:42.003796 think_sql-0.7.4/think_sql/dm/db.py
--rw-r--r--   0        0        0    28937 2024-04-26 06:29:32.880410 think_sql-0.7.4/think_sql/dm/table.py
--rw-r--r--   0        0        0     5674 2024-04-19 07:27:25.515112 think_sql-0.7.4/think_sql/dm/util.py
--rw-r--r--   0        0        0       76 2024-04-15 05:46:17.205661 think_sql-0.7.4/think_sql/mysql/__init__.py
--rw-r--r--   0        0        0     4027 2024-04-16 02:15:08.168259 think_sql-0.7.4/think_sql/mysql/db.py
--rw-r--r--   0        0        0     2837 2024-01-19 04:32:29.868664 think_sql-0.7.4/think_sql/mysql/parse.py
--rw-r--r--   0        0        0    27967 2024-04-15 05:46:51.928111 think_sql-0.7.4/think_sql/mysql/sql_helper.py
--rw-r--r--   0        0        0    25609 2024-04-26 06:27:51.118394 think_sql-0.7.4/think_sql/mysql/table.py
--rw-r--r--   0        0        0     3475 2024-04-15 06:24:27.467941 think_sql-0.7.4/think_sql/mysql/util.py
--rw-r--r--   0        0        0        0 2024-04-11 01:32:11.713368 think_sql-0.7.4/think_sql/tool/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-16 00:57:11.045987 think_sql-0.7.4/think_sql/tool/base.py
--rw-r--r--   0        0        0     2360 2024-04-15 05:48:22.966562 think_sql-0.7.4/think_sql/tool/cache.py
--rw-r--r--   0        0        0     3713 2024-04-16 01:02:24.858779 think_sql-0.7.4/think_sql/tool/interface.py
--rw-r--r--   0        0        0     3379 2024-04-16 02:14:57.886205 think_sql-0.7.4/think_sql/tool/util.py
--rw-r--r--   0        0        0    17944 1970-01-01 00:00:00.000000 think_sql-0.7.4/setup.py
--rw-r--r--   0        0        0    17160 1970-01-01 00:00:00.000000 think_sql-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1381 2024-04-28 10:46:32.016058 think_sql-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0    16301 2024-04-16 02:14:07.551128 think_sql-0.7.5/README.md
+-rw-r--r--   0        0        0     1139 2024-04-19 08:37:22.016945 think_sql-0.7.5/think_sql/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-15 09:26:44.219328 think_sql-0.7.5/think_sql/dm/__init__.py
+-rw-r--r--   0        0        0     4689 2024-04-18 06:56:42.003796 think_sql-0.7.5/think_sql/dm/db.py
+-rw-r--r--   0        0        0    29061 2024-04-28 10:43:43.149865 think_sql-0.7.5/think_sql/dm/table.py
+-rw-r--r--   0        0        0     5674 2024-04-19 07:27:25.515112 think_sql-0.7.5/think_sql/dm/util.py
+-rw-r--r--   0        0        0       76 2024-04-15 05:46:17.205661 think_sql-0.7.5/think_sql/mysql/__init__.py
+-rw-r--r--   0        0        0     4027 2024-04-16 02:15:08.168259 think_sql-0.7.5/think_sql/mysql/db.py
+-rw-r--r--   0        0        0     2837 2024-01-19 04:32:29.868664 think_sql-0.7.5/think_sql/mysql/parse.py
+-rw-r--r--   0        0        0    27967 2024-04-15 05:46:51.928111 think_sql-0.7.5/think_sql/mysql/sql_helper.py
+-rw-r--r--   0        0        0    25609 2024-04-28 10:41:37.659474 think_sql-0.7.5/think_sql/mysql/table.py
+-rw-r--r--   0        0        0     3475 2024-04-15 06:24:27.467941 think_sql-0.7.5/think_sql/mysql/util.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:32:11.713368 think_sql-0.7.5/think_sql/tool/__init__.py
+-rw-r--r--   0        0        0     4092 2024-04-28 10:46:08.532102 think_sql-0.7.5/think_sql/tool/base.py
+-rw-r--r--   0        0        0     2360 2024-04-15 05:48:22.966562 think_sql-0.7.5/think_sql/tool/cache.py
+-rw-r--r--   0        0        0     3713 2024-04-16 01:02:24.858779 think_sql-0.7.5/think_sql/tool/interface.py
+-rw-r--r--   0        0        0     3379 2024-04-16 02:14:57.886205 think_sql-0.7.5/think_sql/tool/util.py
+-rw-r--r--   0        0        0    17944 1970-01-01 00:00:00.000000 think_sql-0.7.5/setup.py
+-rw-r--r--   0        0        0    17160 1970-01-01 00:00:00.000000 think_sql-0.7.5/PKG-INFO
```

### Comparing `think_sql-0.7.4/pyproject.toml` & `think_sql-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "think-sql"
-version = "0.7.4"
+version = "0.7.5"
 description = "ThinkSQL link think-orm(ThinkPHP)"
 authors = [ "hbh112233abc <hbh112233abc@163.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/hbh112233abc/think-sql"
 repository = "https://github.com/hbh112233abc/think-sql"
 documentation = "https://github.com/hbh112233abc/think-sql"
```

### Comparing `think_sql-0.7.4/README.md` & `think_sql-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/__init__.py` & `think_sql-0.7.5/think_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/dm/db.py` & `think_sql-0.7.5/think_sql/dm/db.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/dm/table.py` & `think_sql-0.7.5/think_sql/dm/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,17 +147,19 @@
                 self.pk = field
         return fields
 
     def get_last_sql(self) -> str:
         """获取最后执行的sql"""
         return self.db_cursor.statement
 
-    def get_lastid(self) -> str:
+    def get_lastid(self) -> int:
         """获取最后作用的id"""
-        return self.db_cursor.lastrowid
+        self.db_cursor.execute('SELECT SCOPE_IDENTITY() as last_id')
+        result = self.db_cursor.fetchone()
+        return result['last_id'] if result else 0
 
     def get_rowcount(self) -> int:
         """获取sql影响条数"""
         return self.db_cursor.rowcount
 
     def fetch_sql(self,flag:bool=True):
         """设置获取sql语句标识
```

### Comparing `think_sql-0.7.4/think_sql/dm/util.py` & `think_sql-0.7.5/think_sql/dm/util.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/mysql/db.py` & `think_sql-0.7.5/think_sql/mysql/db.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/mysql/parse.py` & `think_sql-0.7.5/think_sql/mysql/parse.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/mysql/sql_helper.py` & `think_sql-0.7.5/think_sql/mysql/sql_helper.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/mysql/table.py` & `think_sql-0.7.5/think_sql/mysql/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 self.pk = d
         return fields
 
     def get_last_sql(self) -> str:
         """获取最后执行的sql"""
         return self.db_cursor._executed
 
-    def get_lastid(self) -> str:
+    def get_lastid(self) -> int:
         """获取最后作用的id"""
         return self.db_cursor.lastrowid
 
     def get_rowcount(self) -> int:
         """获取sql影响条数"""
         return self.db_cursor.rowcount
```

### Comparing `think_sql-0.7.4/think_sql/mysql/util.py` & `think_sql-0.7.5/think_sql/mysql/util.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/tool/base.py` & `think_sql-0.7.5/think_sql/tool/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         Args:
             config: str|dict|DBConfig 数据库连接配置
             params: dict 数据库连接参数
             debug: bool 调试模式
         """
         self.config = db_config(config)
         self.params = params
-
         self.log = logger
         self.connector = None
         self.cursor = None
         self.auto_commit = True
         self._debug = debug
 
         self.connect()
@@ -43,14 +42,18 @@
 
         Args:
             flag (bool, optional): 调试标识. Defaults to True.
         """
         self._debug = flag
         return self
 
+    def set_logger(self,logger):
+        self.log = logger
+        return self
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, trace):
         """退出操作
         如果return True可以阻止异常传播
 
@@ -74,15 +77,15 @@
         self, db:Database, table_name: str
     ):
         self.db = db
         self.connector = db.connector
         self.db_cursor = db.cursor
         self.table_name = table_name
         self._debug = db._debug
-        self.log = logger
+        self.log = db.logger
         self._fetch_sql = False
         self.use_cache = False
         self.cache_key = None
         self.cache_expire = 3600
         self.cache_storage = cacheout.Cache()
 
     def debug(self, flag: bool = True):
@@ -93,14 +96,18 @@
 
         Returns:
             self: 支持链式调用
         """
         self._debug = flag
         return self
 
+    def set_logger(self,logger):
+        self.log = logger
+        return self
+
     def fetch_sql(self, flag: bool = True):
         """输出sql语句
 
         Args:
             flag (bool, optional): 是否输出sql. Defaults to True.
         """
         self._fetch_sql = flag
```

### Comparing `think_sql-0.7.4/think_sql/tool/cache.py` & `think_sql-0.7.5/think_sql/tool/cache.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/tool/interface.py` & `think_sql-0.7.5/think_sql/tool/interface.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/think_sql/tool/util.py` & `think_sql-0.7.5/think_sql/tool/util.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.7.4/setup.py` & `think_sql-0.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'mysql': ['pymysql>=1.1.0,<2.0.0',
            'sql-metadata>=2.10.0,<3.0.0',
            'tabulate>=0.9.0,<0.10.0',
            'sqlparse>=0.4.4,<0.5.0']}
 
 setup_kwargs = {
     'name': 'think-sql',
-    'version': '0.7.4',
+    'version': '0.7.5',
     'description': 'ThinkSQL link think-orm(ThinkPHP)',
     'long_description': '# ThinkSQL 类似 ThinkPHP 的数据库引擎\n\n## Drivers\n\n- [x] MySQL\n- [x] 达梦(DM8)\n\n## Install\n\n- use mysql\n\n```\npip install think-sql[mysql]\n```\n\n- use 达梦(DM8)\n\n```\npip install think-sql[dm]\n```\n\n## How to use\n\n### 1. simple demo\n\n> Database: `test` Table: `user`\n\n- example dict params\n\n```python\nfrom think_sql import DB\n\nconfig = {\n    \'driver\': \'mysql\',\n    \'host\': \'127.0.0.1\',\n    \'port\': 3306,\n    \'user\': \'root\',\n    \'password\': \'root\',\n    \'database\': \'test\',\n}\n\nwith DB(config) as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\n- example dsn str\n\n```python\nfrom think_sql import DB\n\nwith DB("root:\'root\'@127.0.0.1:3306/test") as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\n- example DBConfig\n\n```python\nfrom think_sql import DB\nfrom think_sql.tool.util import DBConfig\nconfig = DBConfig(\n  host=\'127.0.0.1\',\n  port=3306,\n  user=\'root\',\n  password=\'root\',\n  database=\'test\',\n)\nwith DB(config) as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\nresult\n\n```json\n{\n  "id": 1,\n  "username": "hbh112233abc",\n  "age": "36",\n  "address": "FUJIAN.XIAMEN"\n}\n```\n\n### 2. Introduction\n\n#### DB\n\n- **init**(config:Union[str,dict,DBConfig],params={})\n\n  init database, return DB instance\n\n  - config:Union[str,dict,DBConfig]\n    - str: `user:\'password\'@host:port/database`\n    - dict: `{\'host\':\'127.0.0.1\',\'port\':3306,\'user\':\'root\',\'password\':\'root\',\'database\':\'test\'}`\n    - DBConfig: `DBConfig(host=\'127.0.0.1\',port=3306,user=\'root\',password=\'root\',database=\'test\')`\n  - params:dict pymysql connect other params\n\n- connect()\n  connect database use **init** params\n\n- table(table_name):Table\n  return class Table <think_sql.table.Table>\n\n- check_connected():bool\n  check connected, try reconnect database\n\n- query(sql,params=())\n  query sql return cursor.fetchall List[dict]\n\n- execute(sql,params=())\n  execute sql write operate(ex:insert,update,delete,...)\n\n#### Table\n\n- **init**(connector: Connection,cursor: Cursor,table_name: str,debug: bool = True)\n\n- init()\n  initialize query condition\n\n- debug(flag=True)\n  set debug flag\n\n- set_cache_storage(storage: CacheStorage)\n  set cache storage ex: Redis\n\n- cache(key: str = None, expire: int = 3600)\n  use cache at query\n\n- cursor(sql: str, params: list = []) -> Cursor\n  return cursor object\n\n- get_last_sql() -> str\n  return last sql string\n\n- get_lastid() -> str\n  return last row id\n\n- get_rowcount() -> int\n  return affect rows count\n\n- fetch_sql(flag: bool = True)\n  set fetch sql flag,if flag = True then `query` and `execute` will only return sql\n\n- build_sql(operation: str, params: list = []) -> str\n  return build sql\n\n- query(sql: str, params: list = []) -> list\n  execute read operation sql and return cursor.fetchall()\n  when `fetch_sql`=True then return sql and not execute the sql\n\n- execute(sql: str, params: list = []) -> int\n  execute write operation sql and return affect rows count\n  when `fetch_sql`=True then return sql and not execute the sql\n\n- where(field: Union[str, list, tuple], symbol: str = \'\', value: Any = None)\n  set query conditions, support multipe use\n\n  > where(field,value)\n\n  ```sql\n  where field = value\n  ```\n\n  > where(field,symbol,value)\n\n  ```sql\n  where field symbol value\n  ```\n\n  ```python\n  where(\n      [\n          [field1,symbol1,value1],\n          [field2,symbol2,value2]\n      ]\n  )\n  ```\n\n  ```sql\n  where field1 symbol1 value1 and field2 symbol2 value2\n  ```\n\n  > where(field1,symbol1,value1).where(field2,symbol2,value2)\n\n  ```sql\n  where field1 symbol1 value1 and field2 symbol2 value2\n  ```\n\n  - symbol\n\n  | symbol     | another                  | demo                                                                                    |\n  | ---------- | ------------------------ | --------------------------------------------------------------------------------------- |\n  | `=`        | `eq`,`=`                 | where(\'id\',\'=\',1)                                                                       |\n  | `<>`       | `neq`, `!=`, `<>`        | where(\'id\',\'<>\',1)                                                                      |\n  | `>`        | `gt`,`>`                 | where(\'id\',\'>\',1)                                                                       |\n  | `>=`       | `egt`,`>=`               | where(\'id\',\'>=\',1)                                                                      |\n  | `<`        | `lt`, `<`                | where(\'id\',\'<\',1)                                                                       |\n  | `<=`       | `elt`,`<=`               | where(\'id\',\'<=\',1)                                                                      |\n  | `in`       | `in`,`not in`            | where(\'id\',\'in\',[1,2,3])                                                                |\n  | `between`  | `between`,`not between`  | where(\'id\',\'between\',[1,5]) where(\'id\',\'between\',\'1,5\') where(\'id\',\'between\',\'1 and 5\') |\n  | `like`     | `like`, `not like`       | where(\'name\',\'like\',\'%hbh%\')                                                            |\n  | `null`     | `is null`,`null`         | where(\'remark\',\'is null\')                                                               |\n  | `not null` | `is not null`,`not null` | where(\'remark\',\'is not null\')                                                           |\n  | `exists`   | `exists`, `not exists`   | where(\'remark\',\'exists\')                                                                |\n  | `exp`      | `exp`                    | where(\'id\',\'exp\',\'in (1,2,3)\')                                                          |\n\n- where_or(field: Union[str, list], symbol: str = \'\', value: Any = None)\n\n  > where(\'id\',1).where_or(\'id\',5)\n\n  ```\n  where id = 1 or id = 5\n  ```\n\n- limit(start: int, step: int = None)\n  LIMIT start,step\n\n- page(index: int = 1, size: int = 20)\n  LIMIT index\\*size-1,size\n\n- order(field: str, sort: str = \'asc\')\n  ORDER BY field sort\n\n- group(field:str)\n  GROUP BY field\n\n- distinct(field:str)\n  SELECT DISTINCT field\n\n- field(fields: Any, exclude: bool = False)\n  SELECT fields\n  if `exclude`=True then select the fields of table (exlude:`fields`)\n\n- select(build_sql: bool = False) -> list\n  return select query result\n  if `build_sql`=True then return sql\n\n- find()\n  return select ... limit 1\n\n- value(field: str)\n  return the field of first row\n\n- column(field: str,key: str = \'\')\n\n  > column(\'name\')\n\n  return [\'hbh\',\'mondy\']\n\n  > column(\'name,score\')\n\n  return [{\'hbh\':80},{\'mondy\':88}]\n\n  > column(\'score\',\'name\')\n\n  return {\'hbh\':80, \'mondy\':88}\n\n  > column(\'id,score\',\'name\')\n\n  return {\n  \'hbh\':{\'id\':1,\'score\':80},\n  \'mondy\':{\'id\':2,\'score\':88}\n  }\n\n- alias(short_name: str = \'\')\n  set alias table_name\n\n- join(table_name: str, as_name: str = \'\', on: str = \'\', join: str = \'inner\', and_str: str = \'\')\n  - `table_name` join table_name\n  - `as_name` alias short_table_name for `table_name`\n  - `on` join condition\n  - `join` join type in \'INNER\', \'LEFT\', \'RIGHT\', \'FULL OUTER\'\n  - `and_str` and condition\n    demo\n  ```python\n  db.table(\'table1\').alias(\'a\').join(\n    \'table2\',\'b\',\'a.id=b.a_id\',\'left\'\n  ).join(\n    \'table3\',\'c\',\'c.a_id=a.id\'\n  ).field(\n    \'a.id,a.name,b.id as b_id,b.score,c.id as c_id,c.remark\'\n  ).where(\n    \'a.id\',1\n  ).find()\n  ```\n  sql\n  ```sql\n  SELECT\n      a.id,\n      a.name,\n      b.id AS b_id,\n      b.score,\n      c.id AS c_id,\n      c.remark\n  FROM\n      table1 AS a\n      LEFT JOIN table2 AS b ON a.id = b.a_id\n      INNER JOIN table3 AS c ON c.a_id = a.id\n  WHERE\n      a.id = 1\n      LIMIT 1\n  ```\n- union(sql1: str, sql2: str, union_all: bool = False)\n  union sql1 and sql2\n\n  - union_all if union_all is True then `UNION ALL`\n\n  _demo_\n\n  ```python\n  sql1 = db.table(\'table1\').field(\'name,score\').where(\'status\',1).select(build_sql=True)\n  sql2 = db.table(\'table2\').field(\'name,score\').where(\'status\',1).select(build_sql=True)\n\n  result = db.table().union(sql1,sql2).where(\'score\',\'>\',60).select()\n  ```\n\n  _sql_\n\n  ```sql\n  SELECT\n  *\n  FROM\n      ( SELECT `name`, `score` FROM table1 WHERE `status` = 1 )\n      UNION\n      ( SELECT `name`, `score` FROM table2 WHERE `status` = 1 )\n  WHERE\n      score > 60\n  ```\n\n- insert(data: Union[dict, List[dict]], replace: bool = False) -> int\n  insert data to database\n\n  - `data` dict: insert one record; list: insert multiple records\n  - `replace` bool if `replace` is True then use `REPLACE INTO`\n\n  _demo_\n  insert one record\n\n  ```python\n  db.table(\'table1\').insert({\'name\':\'test\',\'score\':100})\n  ```\n\n  ```sql\n  INSERT INTO table1 (`name`, `score`) VALUES (\'test\', 100)\n  ```\n\n  insert multiple records\n\n  ```python\n  db.table(\'table1\').insert([{\'name\':\'test\',\'score\':100},{\'name\':\'test2\',\'score\':101}])\n  ```\n\n  ```sql\n  INSERT INTO table1 (`name`, `score`) VALUES (\'test\', 100), (\'test2\', 101)\n  ```\n\n  replace mode\n\n  ```python\n  db.table(\'table1\').insert({\'id\':1,\'name\':\'test\',\'score\':100},replace=True)\n  ```\n\n  ```sql\n  REPLACE INTO table1 (`id`, `name`, `score`) VALUES (1,\'test\', 100)\n  ```\n\n- update(data: dict, all_record: bool = False) -> int\n  update data\n\n  - `data` dict you want update data\n  - `all_record` bool if `all_record` is False then you must set update condition; if you want to update all records then you need set `all_record` = True\n\n- delete(all_record: bool = False) -> int\n  delete record\n\n  - `all_record` bool if `all_record` is False then you must set delete condition; if you want to delete all records then you need set `all_record` = True\n\n- inc(field: str, step: Union[str, int, float] = 1) -> int\n\n  increase `field` +`step`\n\n- dec(field: str, step: int = 1) -> int\n\n  decrease `field` -`step`\n\n- max(field: str) -> Union[int, float]\n\n  get the max value of `field`\n\n- sum(field: str) -> Union[int, float, Decimal]\n\n  get the sum value of `field`\n\n- avg(field: str) -> Union[int, float, Decimal]\n\n  get the avg value of `field`\n\n- count(field: str = \'\\*\') -> int\n\n  get the count of records\n\n- copy_to(new_table: str = None, create_blank_table: bool = False) -> int\n\n  copy data to `new_table`\n\n  - `new_table` if `new_table` is None then `new_table` will auto set like `{table_name}_copy`\n  - `create_blank_table` bool if `create_blank_table` is True then only create a blank table like current table.\n\n  _demo_\n\n  ```sql\n  db.table(\'user\').field(\n    \'name,score\'\n  ).where(\n    \'score\',\'>\',60\n  ).copy_to(\'good_boy\')\n  ```\n\n  _sql_\n\n  ```sql\n  SELECT\n    `name`,\n      `score`\n  INTO `good_boy`\n  FROM\n  `user`\n  WHERE\n      score > 60\n  ```\n\n- insert_to(new_table: str, fields: Union[str, list, tuple] = None) -> int\n\n  ```sql\n  INSERT INTO {new_table} SELECT {select_fields} FROM {table} {join} WHERE {where}{group}{order}{limit}\n  ```\n\n- exists(self) -> bool\n\n  check record exists with some query conditions, it use `SELECT 1 FROM {table} {join} WHERE {where} LIMIT 1`\n\n- batch_update(data:List[dict],key:str) -> int\n\n  batch update multiple records\n\n  _demo_\n\n  ```python\n  data = [\n      {\'id\':1,\'score\':66},\n      {\'id\':2,\'score\':59},\n      {\'id\':3,\'score\':86},\n      {\'id\':4,\'score\':90},\n  ]\n  db.table(\'user\').batch(data,key=\'id\')\n  ```\n\n  _sql_\n\n  ```sql\n  update `user` set score = 66 where id = 1;\n  update `user` set score = 59 where id = 2;\n  update `user` set score = 86 where id = 3;\n  update `user` set score = 90 where id = 4;\n  ```\n\n#### support transaction\n\n```python\nfrom think_sql import DB\ndb_dsn = "root:\'password\'@127.0.0.1:3306/database"\nwith DB(db_dsn) as db:\n    # result: insert two records into database\n    with db.start_trans():\n        db.table(\'user\').insert({\'name\':\'think_sql1\',\'score\':98})\n        db.table(\'user\').insert({\'name\':\'think_sql2\',\'score\':99})\n    # result: nothing inserted\n    with db.start_trans():\n        db.table(\'user\').insert({\'name\':\'think_sql1\',\'score\':98})\n        db.table(\'user\').insert({\'name\':\'think_sql2\',\'score\':99})\n        raise Exception(\'error\')\n\n    # The above operation does not affect subsequent operations.\n    db.table(\'user\').insert({\'name\':\'think_sql3\',\'score\':100})\n```\n\n#### sql_helper for mysql\n\n> [Ref:hcymysql/sql_helper](https://github.com/hcymysql/sql_helper)\n\n```python\nfrom think_sql import DB\nfrom think_sql.mysql.sql_helper import help\n\ndb_dsn = "root:\'password\'@127.0.0.1:3306/database"\nwith DB(db_dsn) as db:\n    sql = "slow query sql"\n    help(db, sql)\n```\n\n> result\n\n```shell\n1) 输入的SQL语句是：\n----------------------------------------------------------------------------------------------------\nSELECT *\nFROM hy_cabrecs\nWHERE finished_count > 0\n----------------------------------------------------------------------------------------------------\n2) EXPLAIN执行计划:\n+------+---------------+------------+--------------+--------+-----------------+-------+-----------+-------+--------+------------+-------------+\n| id   | select_type   | table      | partitions   | type   | possible_keys   | key   | key_len   | ref   | rows   | filtered   | Extra       |\n+======+===============+============+==============+========+=================+=======+===========+=======+========+============+=============+\n| 1    | SIMPLE        | hy_cabrecs | None         | ALL    | None            | None  | None      | None  | 14422  | 33.33      | Using where |\n+------+---------------+------------+--------------+--------+-----------------+-------+-----------+-------+--------+------------+-------------+\n3) 索引优化建议：\n----------------------------------------------------------------------------------------------------\n取出表 【hy_cabrecs】 where条件字段 【finished_count】 100000 条记录，重复的数据有：【16093】 条，没有必要为该字段创建索引。\n 【hy_cabrecs】 表，无需添加任何索引。\n```\n\n#### parse for mysql\n\n- parse alter sql\n\n  ```python\n  from think_sql.mysql import parse\n  sql = """\n    alter     table\n    slow_log_test\n    add\n    iii int not null default 0  comment   \'a\';\n  """\n\n  print(parse.alter_sql(sql))\n  ```\n\n  result:\n\n  ```json\n  {\n    "table": "slow_log_test",\n    "field": "iii",\n    "field_type": "int",\n    "is_null": "NOT NULL",\n    "default": "0",\n    "comment": "\'a\'",\n    "after": ""\n  }\n  ```\n\n## Development\n\n### poetry 包管理器\n\n[官网](https://python-poetry.org/)\n\n[Python 包管理之 poetry 的使用](https://blog.csdn.net/zhoubihui0000/article/details/104937285)\n\n[Python 包管理之 poetry 基本使用](https://zhuanlan.zhihu.com/p/110721747)\n\n```\n# 配置虚拟环境在项目目录下\npoetry config virtualenvs.path true\n# 安装依赖\npoetry install\n# 进入虚拟环境\npoetry shell\n```\n\n### poetry command\n\n| 名称    | 功能                                                       |\n| ------- | ---------------------------------------------------------- |\n| new     | 创建一个项目脚手架，包含基本结构、pyproject.toml 文件      |\n| init    | 基于已有的项目代码创建 pyproject.toml 文件，支持交互式填写 |\n| install | 安装依赖库                                                 |\n| update  | 更新依赖库                                                 |\n| add     | 添加依赖库                                                 |\n| remove  | 移除依赖库                                                 |\n| show    | 查看具体依赖库信息，支持显示树形依赖链                     |\n| build   | 构建 tar.gz 或 wheel 包                                    |\n| publish | 发布到 PyPI                                                |\n| run     | 运行脚本和代码                                             |\n\n## unit test\n\n```\npytest --cov --cov-report=html\n```\n\n## publish\n\n```\npoetry build\npoetry config pypi-token.pypi "your pypi.org api token"\npoetry publish -n\n```\n',
     'author': 'hbh112233abc',
     'author_email': 'hbh112233abc@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hbh112233abc/think-sql',
```

### Comparing `think_sql-0.7.4/PKG-INFO` & `think_sql-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: think-sql
-Version: 0.7.4
+Version: 0.7.5
 Summary: ThinkSQL link think-orm(ThinkPHP)
 Home-page: https://github.com/hbh112233abc/think-sql
 License: MIT
 Keywords: sql,think-sql,DB,Table,mysql,达梦
 Author: hbh112233abc
 Author-email: hbh112233abc@163.com
 Requires-Python: >=3.8,<4.0
```

