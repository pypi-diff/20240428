# Comparing `tmp/clovers_groupmate_waifu-0.1.0.post3.tar.gz` & `tmp/clovers_groupmate_waifu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_groupmate_waifu-0.1.0.post3.tar", max compression
+gzip compressed data, was "clovers_groupmate_waifu-0.1.1.tar", max compression
```

## Comparing `clovers_groupmate_waifu-0.1.0.post3.tar` & `clovers_groupmate_waifu-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    14844 2024-04-23 13:29:58.828804 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-23 16:19:41.580219 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/clovers.py
--rw-r--r--   0        0        0     2696 2024-04-23 10:14:52.156708 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/config.py
--rw-r--r--   0        0        0     1763 2024-04-23 04:39:50.328249 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/data.py
--rw-r--r--   0        0        0      627 2024-04-19 18:04:26.925322 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/utils.py
--rw-r--r--   0        0        0     1086 2023-11-06 04:36:06.280670 clovers_groupmate_waifu-0.1.0.post3/LICENSE
--rw-r--r--   0        0        0      391 2024-04-23 16:43:50.889424 clovers_groupmate_waifu-0.1.0.post3/pyproject.toml
--rw-r--r--   0        0        0     3209 2023-11-06 04:36:06.281170 clovers_groupmate_waifu-0.1.0.post3/README.md
--rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 clovers_groupmate_waifu-0.1.0.post3/PKG-INFO
+-rw-r--r--   0        0        0    14844 2024-04-27 15:12:59.041886 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-27 15:12:59.041886 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/clovers.py
+-rw-r--r--   0        0        0     2642 2024-04-27 15:28:58.471177 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/config.py
+-rw-r--r--   0        0        0     1763 2024-04-27 15:12:59.042386 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/data.py
+-rw-r--r--   0        0        0      627 2024-04-27 15:12:59.042886 clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/utils.py
+-rw-r--r--   0        0        0     1086 2024-04-27 15:12:59.040886 clovers_groupmate_waifu-0.1.1/LICENSE
+-rw-r--r--   0        0        0      389 2024-04-27 15:43:54.534832 clovers_groupmate_waifu-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4830 2024-04-27 15:51:02.765042 clovers_groupmate_waifu-0.1.1/README.md
+-rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 clovers_groupmate_waifu-0.1.1/PKG-INFO
```

### Comparing `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/__init__.py` & `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/clovers.py` & `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/config.py` & `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,14 @@
         "Noto Color Emoji",
     ]
 
     waifu_path: str = str(Path("./data/waifu/").absolute())
     """文件记录存档路径"""
     waifu_reset: bool = True
     """是否每日重置cp记录"""
-    waifu_cd_bye: int = 3600
-    """分手冷却"""
     waifu_he: int = 40
     """指定成功概率"""
     waifu_be: int = 20
     """指定失败概率"""
     waifu_ntr: int = 50
     """NTR概率"""
     happy_end_tips: list[str] = [
```

### Comparing `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/data.py` & `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/data.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/utils.py` & `clovers_groupmate_waifu-0.1.1/clovers_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post3/LICENSE` & `clovers_groupmate_waifu-0.1.1/LICENSE`

 * *Files identical despite different names*

