# Comparing `tmp/Fr1997v011-1.3.8.tar.gz` & `tmp/Fr1997v011-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.3.8.tar", last modified: Fri Apr 26 07:00:56 2024, max compression
+gzip compressed data, was "Fr1997v011-1.3.9.tar", last modified: Fri Apr 26 08:09:56 2024, max compression
```

## Comparing `Fr1997v011-1.3.8.tar` & `Fr1997v011-1.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 07:00:56.535258 Fr1997v011-1.3.8/
-drwxrwxrwx   0        0        0        0 2024-04-26 07:00:56.517219 Fr1997v011-1.3.8/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-26 07:00:56.000000 Fr1997v011-1.3.8/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-26 07:00:56.000000 Fr1997v011-1.3.8/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 07:00:56.000000 Fr1997v011-1.3.8/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-26 07:00:56.000000 Fr1997v011-1.3.8/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-26 07:00:56.000000 Fr1997v011-1.3.8/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.3.8/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-26 07:00:56.533256 Fr1997v011-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-26 06:48:47.000000 Fr1997v011-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 07:00:56.519740 Fr1997v011-1.3.8/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.3.8/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:00:56.526739 Fr1997v011-1.3.8/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.3.8/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   173516 2024-04-26 06:59:50.000000 Fr1997v011-1.3.8/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:00:56.530256 Fr1997v011-1.3.8/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.3.8/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-26 07:00:56.535258 Fr1997v011-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-26 06:48:37.000000 Fr1997v011-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.891466 Fr1997v011-1.3.9/
+drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.883180 Fr1997v011-1.3.9/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-26 08:09:56.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-26 08:09:56.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 08:09:56.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-26 07:13:28.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-26 08:09:56.000000 Fr1997v011-1.3.9/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-26 08:09:56.890466 Fr1997v011-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-26 07:13:26.000000 Fr1997v011-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.884178 Fr1997v011-1.3.9/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.3.9/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.887468 Fr1997v011-1.3.9/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.3.9/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   172355 2024-04-26 08:09:55.000000 Fr1997v011-1.3.9/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:09:56.889466 Fr1997v011-1.3.9/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.3.9/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-26 08:09:56.892466 Fr1997v011-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-26 07:13:26.000000 Fr1997v011-1.3.9/setup.py
```

### Comparing `Fr1997v011-1.3.8/LICENSE` & `Fr1997v011-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.3.8/README.md` & `Fr1997v011-1.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.3.8.tar.gz
+pip install dist/Fr1997v011-1.3.9.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.3.8/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.3.9/fr1997_mode/mode_func/all_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -3792,22 +3792,22 @@
             print('Fr包err cnd获取路径失败', E)
 
 
 # FastGpt
 class FastGptAuto:
 
     def __init__(self, **kwargs):
-        self.run_path = kwargs.get('run_path', 2)  # 2测试 01正式
+        self.run_path = int(kwargs.get('run_path', 2))  # 2测试 01正式
         self.avatar = "/icon/logo.svg"
 
         # 正式|测试
         if self.run_path == 2:
             self.conn_tp = 2
             self.base_url = 'http://101.35.29.36:3020/api'
-            self.authorization = 'fastgpt-xBfm0yXYOSTIRNl4JBGAKBKk5Ga6klbezPhWknV7gsTiUdsQOVVkvcVjtrYioRrp'
+            self.authorization = 'fastgpt-nE4z8uvJrrh5N1OvvdjDFG7Y055Rj9xVVXKeVSghM1cFAr1zXRUMdxm5v7a6pC'
         else:
             self.conn_tp = ModeFunc().path
             self.base_url = 'https://aitest.dso100.com/api'
             self.authorization = 'fastgpt-nE4z8uvJrrh5N1OvvdjDFG7Y055Rj9xVVXKeVSghM1cFAr1zXRUMdxm5v7a6pC'
 
         self.user_text_table = 'cd_douyin_user_video_text'
         self.es_user_text_table = 'douyin_user_video_text'
@@ -3855,43 +3855,24 @@
                 data_data = response.json()
                 code = data_data['code']
                 if code == 200:
                     return data_data
         return {'code': 500}
 
     # 应用 修改 【知识库】 【提示词】
-    def app_update(self, app_id, dataset_ids, cue_word):
-        sql = 'SELECT name,json_data FROM `cd_python_json` where `name` = "fastgpt_app_update_json"'
-        all_data = mode_pro.mysql_db(method="s", table="cd_python_json", sql=sql)
-        for at in all_data:
-            fastgpt_app_create_json = json.loads(at[1])
-            fastgpt_app_create_json['modules'][2]['inputs'][7]['value'] = cue_word
-            # dataset_ids = '662732843f901b42fce83f3c,6627514c3f901b42fce89e27'
-            dataset_ids_list = dataset_ids.split(',')
-            for dt_id in dataset_ids_list:
-                fastgpt_app_create_json['modules'][3]['inputs'][1]['value'].append({
-                    "datasetId": dt_id,
-                    "vectorModel": {
-                        "model": "text-embedding-ada-002",
-                        "name": "Embedding-2",
-                        "inputPrice": 0,
-                        "outputPrice": 0,
-                        "defaultToken": 700,
-                        "maxToken": 3000,
-                        "weight": 100,
-                        "defaultConfig": {}
-                    }
-                })
-            response = requests.post(f'{self.base_url}/core/app/update?appId={app_id}', headers=self.get_token_header(),
-                                     json=fastgpt_app_create_json)
-            if response.status_code == 200:
-                data_data = response.json()
-                code = data_data['code']
-                if code == 200:
-                    return data_data
+    def app_update(self, app_id, up_data):
+        response = requests.post(
+            f'{self.base_url}/core/app/update?appId={app_id}',
+            headers=self.get_token_header(),
+            json=up_data)
+        if response.status_code == 200:
+            data_data = response.json()
+            code = data_data['code']
+            if code == 200:
+                return data_data
         return {'code': 500}
 
     # 知识库 创建
     def dataset_create(self, dataset_name):
         data = {
             "parentId": None,
             "type": "dataset",
@@ -4352,8 +4333,7 @@
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 mode_fastgpt = FastGptAuto(run_path=1)  # fastgpt
 mode_fastgpt_test = FastGptAuto(run_path=2)  # fastgpt test
 
 mode_pro = ModeFunc()  # main
-
```

