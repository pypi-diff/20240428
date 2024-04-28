# Comparing `tmp/clovers_groupmate_waifu-0.1.1.tar.gz` & `tmp/clovers_groupmate_waifu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_groupmate_waifu-0.1.1.tar", max compression
+gzip compressed data, was "clovers_groupmate_waifu-0.1.2.tar", max compression
```

## Comparing `clovers_groupmate_waifu-0.1.1.tar` & `clovers_groupmate_waifu-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    14844 2024-04-27 15:12:59.041886 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-27 15:12:59.041886 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/clovers.py
--rw-r--r--   0        0        0     2642 2024-04-27 15:28:58.471177 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/config.py
--rw-r--r--   0        0        0     1763 2024-04-27 15:12:59.042386 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/data.py
--rw-r--r--   0        0        0      627 2024-04-27 15:12:59.042886 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/utils.py
--rw-r--r--   0        0        0     1086 2024-04-27 15:12:59.040886 clovers_groupmate_waifu-0.1.1/LICENSE
--rw-r--r--   0        0        0      389 2024-04-27 15:43:54.534832 clovers_groupmate_waifu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4830 2024-04-27 15:51:02.765042 clovers_groupmate_waifu-0.1.1/README.md
--rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 clovers_groupmate_waifu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    14844 2024-04-27 15:12:59.041886 clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-27 15:12:59.041886 clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/clovers.py
+-rw-r--r--   0        0        0     2642 2024-04-27 15:28:58.471177 clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/config.py
+-rw-r--r--   0        0        0     1819 2024-04-28 04:24:06.056867 clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/data.py
+-rw-r--r--   0        0        0      627 2024-04-27 15:12:59.042886 clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/utils.py
+-rw-r--r--   0        0        0     1086 2024-04-27 15:12:59.040886 clovers_groupmate_waifu-0.1.2/LICENSE
+-rw-r--r--   0        0        0      389 2024-04-28 04:04:45.170238 clovers_groupmate_waifu-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4818 2024-04-27 15:59:04.794098 clovers_groupmate_waifu-0.1.2/README.md
+-rw-r--r--   0        0        0     5019 1970-01-01 00:00:00.000000 clovers_groupmate_waifu-0.1.2/PKG-INFO
```

### Comparing `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/__init__.py` & `clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/clovers.py` & `clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/config.py` & `clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/config.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/data.py` & `clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     record_yinpa0: Counter[str] = Counter()
     """银趴被动记录"""
 
 
 class User(BaseModel):
     user_id: str
     nickname: str
-    card: str
+    card: str | None
     avatar: str
     last_sent_time: int = 0
     group_nickname_dict: dict[str, str] = {}
 
     def group_nickname(self, group_id: str):
         return self.group_nickname_dict.get(group_id) or self.nickname
 
@@ -34,18 +34,19 @@
     record: dict[str, GroupData] = {}
     protect_uids: set[str] = set()
     "保护名单"
     user_data: dict[str, User] = {}
 
     def update_nickname(self, user_list: list[User], group_id: str):
         for user in user_list:
-            if user.user_id in self.user_data:
+            if user.user_id in self.user_data and user.card:
                 self.user_data[user.user_id].group_nickname_dict[group_id] = user.card
             else:
-                user.group_nickname_dict[group_id] = user.card
+                if user.card:
+                    user.group_nickname_dict[group_id] = user.card
                 self.user_data[user.user_id] = user
 
     @classmethod
     def load(cls, path: str | Path):
         file = Path(path)
         if file.exists():
             with open(file, "r", encoding="utf8") as f:
```

### Comparing `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/utils.py` & `clovers_groupmate_waifu-0.1.2/clovers_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.1/LICENSE` & `clovers_groupmate_waifu-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.1/README.md` & `clovers_groupmate_waifu-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 <div align="center">
 
 # clovers-groupmate-waifu
 
 _✨ 娶群友 ✨_
 
 <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="python">
-<a href="./LICENSE">
-<img src="https://img.shields.io/github/license/KarisAya/clovers-groupmate-waifu.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/clovers-groupmate-waifu">
-<img src="https://img.shields.io/pypi/v/clovers-groupmate-waifu.svg" alt="pypi">
-</a>
-<a href="https://pypi.python.org/pypi/clovers-groupmate-waifu">
-<img src="https://img.shields.io/pypi/dm/clovers-groupmate-waifu" alt="pypi download">
-</a>
+<a href="./LICENSE"><img src="https://img.shields.io/github/license/KarisAya/clovers_groupmate_waifu.svg" alt="license"></a>
+<a href="https://pypi.python.org/pypi/clovers_groupmate_waifu"><img src="https://img.shields.io/pypi/v/clovers_groupmate_waifu.svg" alt="pypi"></a>
+<a href="https://pypi.python.org/pypi/clovers_groupmate_waifu"><img src="https://img.shields.io/pypi/dm/clovers_groupmate_waifu" alt="pypi download"></a>
 
 </div>
 
 ## 💿 安装
 
 ```bash
 pip install clovers_groupmate_waifu
```

### Comparing `clovers_groupmate_waifu-0.1.1/PKG-INFO` & `clovers_groupmate_waifu-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clovers-groupmate-waifu
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0)
 Requires-Dist: clovers[linecard,tools] (>=0.1.8,<0.2.0)
@@ -13,23 +13,17 @@
 <div align="center">
 
 # clovers-groupmate-waifu
 
 _✨ 娶群友 ✨_
 
 <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="python">
-<a href="./LICENSE">
-<img src="https://img.shields.io/github/license/KarisAya/clovers-groupmate-waifu.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/clovers-groupmate-waifu">
-<img src="https://img.shields.io/pypi/v/clovers-groupmate-waifu.svg" alt="pypi">
-</a>
-<a href="https://pypi.python.org/pypi/clovers-groupmate-waifu">
-<img src="https://img.shields.io/pypi/dm/clovers-groupmate-waifu" alt="pypi download">
-</a>
+<a href="./LICENSE"><img src="https://img.shields.io/github/license/KarisAya/clovers_groupmate_waifu.svg" alt="license"></a>
+<a href="https://pypi.python.org/pypi/clovers_groupmate_waifu"><img src="https://img.shields.io/pypi/v/clovers_groupmate_waifu.svg" alt="pypi"></a>
+<a href="https://pypi.python.org/pypi/clovers_groupmate_waifu"><img src="https://img.shields.io/pypi/dm/clovers_groupmate_waifu" alt="pypi download"></a>
 
 </div>
 
 ## 💿 安装
 
 ```bash
 pip install clovers_groupmate_waifu
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clovers-groupmate-waifu Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: clovers-groupmate-waifu Version: 0.1.2 Summary:
 Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3 Requires-Dist: clovers-
 apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers[linecard,tools]
 (>=0.1.8,<0.2.0) Description-Content-Type: text/markdown
    # clovers-groupmate-waifu _â¨ å¨¶ç¾¤å â¨_[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i
                                    _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ```bash pip install clovers_groupmate_waifu ``` ## âï¸ éç½®
```

