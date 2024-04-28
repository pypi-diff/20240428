# Comparing `tmp/Fr1997v011-1.3.9.tar.gz` & `tmp/Fr1997v011-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.3.9.tar", last modified: Fri Apr 26 08:09:56 2024, max compression
+gzip compressed data, was "Fr1997v011-1.4.0.tar", last modified: Sun Apr 28 08:18:45 2024, max compression
```

## Comparing `Fr1997v011-1.3.9.tar` & `Fr1997v011-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.891466 Fr1997v011-1.3.9/
-drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.883180 Fr1997v011-1.3.9/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-26 08:09:56.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-26 08:09:56.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 08:09:56.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-26 07:13:28.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-26 08:09:56.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.3.9/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-26 08:09:56.890466 Fr1997v011-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-26 07:13:26.000000 Fr1997v011-1.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.884178 Fr1997v011-1.3.9/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.3.9/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.887468 Fr1997v011-1.3.9/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.3.9/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   172355 2024-04-26 08:09:55.000000 Fr1997v011-1.3.9/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.889466 Fr1997v011-1.3.9/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.3.9/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-26 08:09:56.892466 Fr1997v011-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-26 07:13:26.000000 Fr1997v011-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.136817 Fr1997v011-1.4.0/
+drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.121280 Fr1997v011-1.4.0/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-28 08:18:44.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-28 08:18:44.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 08:18:44.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-28 07:52:40.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-28 08:18:44.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-28 08:18:45.134817 Fr1997v011-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-28 07:52:43.000000 Fr1997v011-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.123796 Fr1997v011-1.4.0/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.0/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.129797 Fr1997v011-1.4.0/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.0/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   172508 2024-04-28 08:18:42.000000 Fr1997v011-1.4.0/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.132800 Fr1997v011-1.4.0/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.0/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 08:18:45.136817 Fr1997v011-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-28 07:52:38.000000 Fr1997v011-1.4.0/setup.py
```

### Comparing `Fr1997v011-1.3.9/LICENSE` & `Fr1997v011-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.3.9/README.md` & `Fr1997v011-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.3.9.tar.gz
+pip install dist/Fr1997v011-1.4.0.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.3.9/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.4.0/fr1997_mode/mode_func/all_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -2296,14 +2296,21 @@
         code = kwargs.get('code')
         status_codes = self.django_config()['status_codes']
         return {
             sc: status_codes[code][sc],
             msg: status_codes[code][msg],
         }
 
+    # 获取请求的ip 【1=正式】 【2=测试】
+    def user_ip(self, request):
+        if request.META.get('REMOTE_ADDR', None) == '1.14.10.13':
+            return 1
+        else:
+            return 2
+
 
 # mode
 class ModeFunc:
     def __init__(self):
         self.path = mode_pros.run_machine()['platform']
 
     # >>>>----------------       数据库 redis数据库        ----------------<<<<<
@@ -3876,15 +3883,15 @@
         data = {
             "parentId": None,
             "type": "dataset",
             "name": dataset_name,
             "intro": '',
             "avatar": self.avatar,
             "vectorModel": "text-embedding-ada-002",
-            "agentModel": "gpt-3.5-turbo"
+            "agentModel": 'gpt-3.5-turbo-1106'
         }
         response = requests.post(f'{self.base_url}/core/dataset/create', headers=self.get_header(), json=data)
         if response.status_code == 200:
             data_data = response.json()
             code = data_data['code']
             if code == 200:
                 return data_data['data']
@@ -4168,55 +4175,61 @@
                 'create_time': int(time.time()),
                 'dataset_name': dataset_name,
                 'dataset_id': dataset_id,
                 'collection_id': collection_id,
             }])
 
     # 计划任务 达人文案库 -> 知识库
-    def user_text_to_dataset(self):
-        sql = (f'SELECT id,user_id,sec_uid,nickname,create_time,time_frame,time_frame_video_count'
-               f' FROM {self.user_text_table} WHERE to_dataset = 0 and `state` = 1 limit 1')  # to_dataset=0|1
+    def user_text_to_dataset(self, h_id):
+        sql = f"""SELECT id,user_id,sec_uid,nickname,create_time,time_frame,time_frame_video_count,`state`,to_dataset
+         FROM {self.user_text_table} 
+         WHERE id = {h_id}"""  # to_dataset=0|1
         all_data = mode_pro.mysql_db(method='s', table=self.user_text_table, sql=sql, conn_tp=self.conn_tp)
-        for i in all_data:
-            print(i)
-            id_id = i[0]
-            user_id = i[1]
-            sec_uid = i[2]
-            nickname = i[3]
-            create_time = i[4]
-            time_frame = i[5]
-            time_frame_video_count = i[6]
-
-            tf_stamp = self.time_frame_stamp(time_frame, create_time)
-            # 时间范围 视频
-            query = {
-                "bool": {
-                    "must": [
-                        {"match": {"sec_uid": sec_uid}},
-                        {"match": {"aweme_type": 0}},
-                        {"range": {"create_time": {"gte": tf_stamp}}},
-                        {"range": {"create_time": {"lte": create_time}}},
-                    ]
-                }
+        if not all_data:
+            return {'code': -1, 'msg': '数据不存在'}
+
+        i = all_data[0]
+        sec_uid = i[2]
+        nickname = i[3]
+        create_time = i[4]
+        time_frame = i[5]
+        if i[7] != 1:
+            return {'code': -1, 'msg': '数据转译中'}
+
+        if i[8] == 1:
+            return {'code': -1, 'msg': '知识库已添加'}
+
+        tf_stamp = self.time_frame_stamp(time_frame, create_time)
+        # 时间范围 视频
+        query = {
+            "bool": {
+                "must": [
+                    {"match": {"sec_uid": sec_uid}},
+                    {"match": {"aweme_type": 0}},
+                    {"range": {"create_time": {"gte": tf_stamp}}},
+                    {"range": {"create_time": {"lte": create_time}}},
+                ]
             }
-            source = ['video_text']
-            data_data = mode_pro.es_search_new_20231215(table=self.es_user_text_table, query=query, _source=source,
-                                                        size=3000)
-
-            push_data = []  # 要添加知识库的文案
-            for v in data_data:
-                print(v)
-                data_info = v['_source']
-                push_data.append({
-                    "q": data_info.get('video_text', ''),
-                    "a": ""
-                })
+        }
+        source = ['video_text']
+        data_data = mode_pro.es_search_new_20231215(table=self.es_user_text_table, query=query, _source=source,
+                                                    size=3000)
+
+        push_data = []  # 要添加知识库的文案
+        for v in data_data:
+            data_info = v['_source']
+            push_data.append({
+                "q": data_info.get('video_text', ''),
+                "a": ""
+            })
 
-            # 创建知识库
-            self.func_create_dataset(dataset_name=nickname, push_data=push_data, save_info=i)
+        # 创建知识库
+        self.func_create_dataset(dataset_name=nickname, push_data=push_data, save_info=i)
+
+        return {'code': 1, 'msg': 'ok'}
 
     # 计划任务 判断知识库文案装填成功
     def dataset_is_upload(self):
         save_data = []
         sql = f'SELECT id,dataset_id,collection_id FROM {self.all_dataset_table} where is_upload = 0'
         all_data = mode_pro.mysql_db(method='s', table=self.all_dataset_table, sql=sql, conn_tp=self.conn_tp)
         for i in all_data:
@@ -4329,11 +4342,11 @@
 mode_spider = SpiderJike()  # 数据请求
 mode_django = DjangoJike()  # django配置
 mode_douyin = DouyinJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
-mode_fastgpt = FastGptAuto(run_path=1)  # fastgpt
-mode_fastgpt_test = FastGptAuto(run_path=2)  # fastgpt test
 
 mode_pro = ModeFunc()  # main
+
+
```

