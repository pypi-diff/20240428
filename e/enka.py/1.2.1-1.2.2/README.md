# Comparing `tmp/enka.py-1.2.1.tar.gz` & `tmp/enka.py-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enka.py-1.2.1.tar", last modified: Mon Jan  1 06:13:19 2024, max compression
+gzip compressed data, was "enka.py-1.2.2.tar", last modified: Sun Apr 28 12:39:47 2024, max compression
```

## Comparing `enka.py-1.2.1.tar` & `enka.py-1.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-01-01 06:13:19.812317 enka.py-1.2.1/
--rw-rw-rw-   0        0        0     1047 2023-12-06 10:08:31.000000 enka.py-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     4920 2024-01-01 06:13:19.811320 enka.py-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4267 2023-12-06 10:08:31.000000 enka.py-1.2.1/README.md
--rw-rw-rw-   0        0        0     4153 2023-12-06 10:08:31.000000 enka.py-1.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-01 06:13:19.808330 enka.py-1.2.1/enka.py.egg-info/
--rw-rw-rw-   0        0        0     4920 2024-01-01 06:13:19.000000 enka.py-1.2.1/enka.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-01-01 06:13:19.000000 enka.py-1.2.1/enka.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-01 06:13:19.000000 enka.py-1.2.1/enka.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-09 07:42:49.000000 enka.py-1.2.1/enka.py.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-01-01 06:13:19.000000 enka.py-1.2.1/enka.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-01 06:13:19.000000 enka.py-1.2.1/enka.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-01 06:13:19.809327 enka.py-1.2.1/enkapy/
--rw-rw-rw-   0        0        0      114 2023-12-06 10:08:31.000000 enka.py-1.2.1/enkapy/__init__.py
--rw-rw-rw-   0        0        0    12797 2024-01-01 05:44:45.000000 enka.py-1.2.1/enkapy/client.py
--rw-rw-rw-   0        0        0      352 2023-12-06 10:08:31.000000 enka.py-1.2.1/enkapy/exception.py
-drwxrwxrwx   0        0        0        0 2024-01-01 06:13:19.811320 enka.py-1.2.1/enkapy/model/
--rw-rw-rw-   0        0        0      432 2023-12-18 02:48:04.000000 enka.py-1.2.1/enkapy/model/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-12-18 03:15:43.000000 enka.py-1.2.1/enkapy/model/artifact.py
--rw-rw-rw-   0        0        0     4141 2024-01-01 06:09:05.000000 enka.py-1.2.1/enkapy/model/character.py
--rw-rw-rw-   0        0        0     6074 2023-12-06 10:08:31.000000 enka.py-1.2.1/enkapy/model/combats.py
--rw-rw-rw-   0        0        0     1227 2024-01-01 05:54:37.000000 enka.py-1.2.1/enkapy/model/players.py
--rw-rw-rw-   0        0        0     1381 2024-01-01 06:11:08.000000 enka.py-1.2.1/enkapy/model/weapon.py
--rw-rw-rw-   0        0        0       42 2024-01-01 06:13:19.812317 enka.py-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      835 2024-01-01 06:13:19.000000 enka.py-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 12:39:47.915228 enka.py-1.2.2/
+-rw-rw-rw-   0        0        0     1047 2023-12-06 10:08:31.000000 enka.py-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4920 2024-04-28 12:39:47.915228 enka.py-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4267 2023-12-06 10:08:31.000000 enka.py-1.2.2/README.md
+-rw-rw-rw-   0        0        0     4153 2023-12-06 10:08:31.000000 enka.py-1.2.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-28 12:39:47.910244 enka.py-1.2.2/enka.py.egg-info/
+-rw-rw-rw-   0        0        0     4920 2024-04-28 12:39:47.000000 enka.py-1.2.2/enka.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-04-28 12:39:47.000000 enka.py-1.2.2/enka.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 12:39:47.000000 enka.py-1.2.2/enka.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-09 07:42:49.000000 enka.py-1.2.2/enka.py.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-04-28 12:39:47.000000 enka.py-1.2.2/enka.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 12:39:47.000000 enka.py-1.2.2/enka.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 12:39:47.911242 enka.py-1.2.2/enkapy/
+-rw-rw-rw-   0        0        0      114 2023-12-06 10:08:31.000000 enka.py-1.2.2/enkapy/__init__.py
+-rw-rw-rw-   0        0        0    12799 2024-04-28 12:39:16.000000 enka.py-1.2.2/enkapy/client.py
+-rw-rw-rw-   0        0        0      352 2023-12-06 10:08:31.000000 enka.py-1.2.2/enkapy/exception.py
+drwxrwxrwx   0        0        0        0 2024-04-28 12:39:47.915228 enka.py-1.2.2/enkapy/model/
+-rw-rw-rw-   0        0        0      432 2023-12-18 02:48:04.000000 enka.py-1.2.2/enkapy/model/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-12-18 03:15:43.000000 enka.py-1.2.2/enkapy/model/artifact.py
+-rw-rw-rw-   0        0        0     4141 2024-01-01 06:09:05.000000 enka.py-1.2.2/enkapy/model/character.py
+-rw-rw-rw-   0        0        0     6074 2023-12-06 10:08:31.000000 enka.py-1.2.2/enkapy/model/combats.py
+-rw-rw-rw-   0        0        0     1227 2024-01-01 05:54:37.000000 enka.py-1.2.2/enkapy/model/players.py
+-rw-rw-rw-   0        0        0     1381 2024-01-01 06:11:08.000000 enka.py-1.2.2/enkapy/model/weapon.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 12:39:47.915228 enka.py-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      835 2024-04-28 12:39:37.000000 enka.py-1.2.2/setup.py
```

### Comparing `enka.py-1.2.1/LICENSE` & `enka.py-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enka.py-1.2.1/PKG-INFO` & `enka.py-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enka.py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/pwnless/enka.py
 Author: pwnless
 Author-email: mystream@riseup.net
 Keywords: enkapy.py,enkapy,enka.network,genshinapi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enka.py-1.2.1/README.md` & `enka.py-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `enka.py-1.2.1/README.rst` & `enka.py-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `enka.py-1.2.1/enka.py.egg-info/PKG-INFO` & `enka.py-1.2.2/enka.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enka.py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/pwnless/enka.py
 Author: pwnless
 Author-email: mystream@riseup.net
 Keywords: enkapy.py,enkapy,enka.network,genshinapi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enka.py-1.2.1/enkapy/client.py` & `enka.py-1.2.2/enkapy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         user = await client.fetch_user(104267816)
         print(f"Nickname: {user.player.nickname}")
 
     """
     _URL = "https://enka.network/api/uid/{uid}"
     # https://github.com/theBowja/GenshinData-1
     # https://raw.githubusercontent.com/GrownNed/Homework/master
-    _REPO_BASE = 'https://gitlab.com/Dimbreath/AnimeGameData/-/raw/main'
+    _REPO_BASE = 'https://gitlab.com/Dimbreath/AnimeGameData/-/raw/master'
     _LANG_URL = _REPO_BASE + '/TextMap/TextMap{lang}.json?inline=false'
     _AVATAR_URL = _REPO_BASE + '/ExcelBinOutput/AvatarExcelConfigData.json?inline=false'
     _TALENT_URL = _REPO_BASE + '/ExcelBinOutput/AvatarTalentExcelConfigData.json?inline=false'
     _SKILL_DEPOT_URL = _REPO_BASE + '/ExcelBinOutput/AvatarSkillDepotExcelConfigData.json?inline=false'
     _SKILL_URL = _REPO_BASE + '/ExcelBinOutput/AvatarSkillExcelConfigData.json?inline=false'
     USER_AGENT = "Mozilla/5.0"
     timeout = 30
```

### Comparing `enka.py-1.2.1/enkapy/model/artifact.py` & `enka.py-1.2.2/enkapy/model/artifact.py`

 * *Files identical despite different names*

### Comparing `enka.py-1.2.1/enkapy/model/character.py` & `enka.py-1.2.2/enkapy/model/character.py`

 * *Files identical despite different names*

### Comparing `enka.py-1.2.1/enkapy/model/combats.py` & `enka.py-1.2.2/enkapy/model/combats.py`

 * *Files identical despite different names*

### Comparing `enka.py-1.2.1/enkapy/model/players.py` & `enka.py-1.2.2/enkapy/model/players.py`

 * *Files identical despite different names*

### Comparing `enka.py-1.2.1/enkapy/model/weapon.py` & `enka.py-1.2.2/enkapy/model/weapon.py`

 * *Files identical despite different names*

### Comparing `enka.py-1.2.1/setup.py` & `enka.py-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="enka.py",
-    version="1.2.1",
+    version="1.2.2",
     author="pwnless",
     author_email="mystream@riseup.net",
     description="Library for fetching JSON data from site https://enka.network/",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/pwnless/enka.py",
     keywords=['enkapy.py', 'enkapy', 'enka.network', 'genshinapi'],
```

