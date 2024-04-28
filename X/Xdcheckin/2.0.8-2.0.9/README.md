# Comparing `tmp/xdcheckin-2.0.8.tar.gz` & `tmp/xdcheckin-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdcheckin-2.0.8.tar", last modified: Sun Apr 21 13:16:51 2024, max compression
+gzip compressed data, was "xdcheckin-2.0.9.tar", last modified: Sat Apr 27 01:02:54 2024, max compression
```

## Comparing `xdcheckin-2.0.8.tar` & `xdcheckin-2.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.119346 xdcheckin-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-21 13:16:51.119346 xdcheckin-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:16:51.119346 xdcheckin-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.111346 xdcheckin-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.119346 xdcheckin-2.0.8/src/Xdcheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 13:16:51.000000 xdcheckin-2.0.8/src/Xdcheckin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.111346 xdcheckin-2.0.8/src/xdcheckin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/core/chaoxing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/core/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/core/xidian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/activity.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/classroom.js
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/curriculum.js
--rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/g_classroom_urls.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/location.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/login.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/misc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/player.js
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/static/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:51.115346 xdcheckin-2.0.8/src/xdcheckin/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/util/chaoxing_captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-21 13:16:45.000000 xdcheckin-2.0.8/src/xdcheckin/util/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.827584 xdcheckin-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/src/Xdcheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 01:02:54.000000 xdcheckin-2.0.9/src/Xdcheckin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.831584 xdcheckin-2.0.9/src/xdcheckin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.831584 xdcheckin-2.0.9/src/xdcheckin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33622 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/core/chaoxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/core/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/core/xidian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.831584 xdcheckin-2.0.9/src/xdcheckin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/src/xdcheckin/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/activity.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/classroom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/curriculum.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/g_classroom_urls.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/location.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/misc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/player.js
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/static/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/src/xdcheckin/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:54.835584 xdcheckin-2.0.9/src/xdcheckin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/util/chaoxing_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-27 01:02:46.000000 xdcheckin-2.0.9/src/xdcheckin/util/encryption.py
```

### Comparing `xdcheckin-2.0.8/LICENSE` & `xdcheckin-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/PKG-INFO` & `xdcheckin-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.8
+Version: 2.0.9
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `xdcheckin-2.0.8/README.md` & `xdcheckin-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/pyproject.toml` & `xdcheckin-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Xdcheckin"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
 	{name = "Pairman", email = "pairmanxlr@gmail.com"}
 ]
 readme = "README.md"
 description = "Chaoxing Checkin Tool for XDU."
 license = {text = "GNU General Public License v3 (GPLv3)"}
 keywords = ["xdu", "xidian", "chaoxing", "livestream"]
```

### Comparing `xdcheckin-2.0.8/src/Xdcheckin.egg-info/PKG-INFO` & `xdcheckin-2.0.9/src/Xdcheckin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.8
+Version: 2.0.9
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `xdcheckin-2.0.8/src/Xdcheckin.egg-info/SOURCES.txt` & `xdcheckin-2.0.9/src/Xdcheckin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/core/chaoxing.py` & `xdcheckin-2.0.9/src/xdcheckin/core/chaoxing.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,15 @@
 		return [
 			{
 				"active_id": str(activity["id"]),
 				"type": activity["otherId"],
 				"name": activity["nameOne"],
 				"time_start": str(_datetime.fromtimestamp(activity["startTime"] // 1000)),
 				"time_end":
-					str(_datetime.fromtimestamp((activity["endTime"]) // 1000))
+					str(_datetime.fromtimestamp(activity["endTime"] // 1000))
 					if activity["endTime"] else "",
 				"time_left": activity["nameFour"]
 			} for activity in data if activity["status"] == 1 and activity.get("otherId") in ("2", "4")
 		]
 
 	def course_get_course_activities_ppt(
 		self, course: dict = {"course_id": "", "class_id": ""}
@@ -544,15 +544,17 @@
 				"time_left": activity["nameFour"]
 			}
 			details = self.checkin_get_details(activity = activity_new)
 			if not details["otherId"] in (2, 4):
 				continue
 			activity_new.update({
 				"type": str(details["otherId"]),
-				"time_end": str(_datetime.fromtimestamp(details["endTime"]["time"] // 1000))
+				"time_end":
+					str(_datetime.fromtimestamp(details["endTime"]["time"] // 1000))
+					if details["endTime"] else "",
 			})
 			activities.append(activity_new)
 		return activities
 
 	def course_get_activities(self):
 		"""Get activities of all courses.
 		:return: Dictionary of class IDs to ongoing activities.
```

### Comparing `xdcheckin-2.0.8/src/xdcheckin/core/locations.py` & `xdcheckin-2.0.9/src/xdcheckin/core/locations.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/core/xidian.py` & `xdcheckin-2.0.9/src/xdcheckin/core/xidian.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/server.py` & `xdcheckin-2.0.9/src/xdcheckin/server/server.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/activity.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/activity.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/classroom.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/classroom.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/curriculum.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/curriculum.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/g_classroom_urls.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/g_classroom_urls.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/location.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/location.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/login.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/login.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/misc.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/misc.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/player.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/player.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/style.css` & `xdcheckin-2.0.9/src/xdcheckin/server/static/style.css`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/static/util.js` & `xdcheckin-2.0.9/src/xdcheckin/server/static/util.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/server/templates/index.html` & `xdcheckin-2.0.9/src/xdcheckin/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/util/chaoxing_captcha.py` & `xdcheckin-2.0.9/src/xdcheckin/util/chaoxing_captcha.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.8/src/xdcheckin/util/encryption.py` & `xdcheckin-2.0.9/src/xdcheckin/util/encryption.py`

 * *Files identical despite different names*

