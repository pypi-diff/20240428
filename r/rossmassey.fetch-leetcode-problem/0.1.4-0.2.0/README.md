# Comparing `tmp/rossmassey_fetch_leetcode_problem-0.1.4.tar.gz` & `tmp/rossmassey_fetch_leetcode_problem-0.2.0.tar.gz`

## Comparing `rossmassey_fetch_leetcode_problem-0.1.4.tar` & `rossmassey_fetch_leetcode_problem-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/requirements.txt
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/.vscode/launch.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/make.bat
--rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/.$diagram.drawio.dtmp
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/conf.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/cookies.rst
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/database.rst
--rw-r--r--   0        0        0     7465 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/diagram.drawio
--rw-r--r--   0        0        0    48066 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/diagram.png
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/index.rst
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/private.rst
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/public.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/docs/source/_static/css/custom.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_cookies.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_func_parsing.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_leetcode_api.py
--rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_parsing.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_problem_index.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_util.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/main.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/problem_info.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/schema.sql
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/LICENSE
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/README.md
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/.vscode/launch.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/.$diagram.drawio.dtmp
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/cookies.rst
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/database.rst
+-rw-r--r--   0        0        0     7465 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/diagram.drawio
+-rw-r--r--   0        0        0    48066 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/diagram.png
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/private.rst
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/public.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/docs/source/_static/css/custom.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_cookies.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_func_parsing.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_leetcode_api.py
+-rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_parsing.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_problem_index.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_util.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/main.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/problem_info.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/schema.sql
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/README.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 rossmassey_fetch_leetcode_problem-0.2.0/PKG-INFO
```

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/.github/workflows/gh-pages.yml` & `rossmassey_fetch_leetcode_problem-0.2.0/.github/workflows/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/.github/workflows/python-publish.yml` & `rossmassey_fetch_leetcode_problem-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/Makefile` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/make.bat` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/.$diagram.drawio.dtmp` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/.$diagram.drawio.dtmp`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/conf.py` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/cookies.rst` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/cookies.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 cookies.txt
 -----------
 ``cookies.txt`` is needed for synced user code.
 
-Export a Netscape HTTP Cookie File for ``leetcode.com`` (refer to browser extensions).
-
-Alternatively, create a file with the text ``LEETCODE_SESSION``, a tab (``\t``),
-and your session token. This can be found in the Network tab in developer tools,
-under Request Cookies, for requests to ``leetcode.com``.
+Export a Netscape HTTP Cookie File for ``leetcode.com`` (see browser extensions like ``cookies.txt``).
 
 Save as ``cookies.txt`` in the ``src/fetch_leetcode_problem/`` directory, or supply
 the ``load_cookie`` function with its relative location.
 
 .. code-block:: python
 
       import fetch_leetcode_problem as lc
@@ -26,8 +22,8 @@
 
 .. code-block:: bash
 
     package_location=$(pip show rossmassey.fetch-leetcode-problem | grep Location)
     package_path=$(echo $package_location | cut -d ' ' -f2)
     cp cookies.txt $package_path/fetch_leetcode_problem/
 
-It takes a while to expire
+It takes a while to expire
```

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/database.rst` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/database.rst`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/diagram.drawio` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/diagram.drawio`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/diagram.png` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/diagram.png`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/index.rst` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/private.rst` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/private.rst`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/docs/source/public.rst` & `rossmassey_fetch_leetcode_problem-0.2.0/docs/source/public.rst`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_func_parsing.py` & `rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_func_parsing.py`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_leetcode_api.py` & `rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_leetcode_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Functions to fetch data from LeetCode API
 """
 import requests
 
-from ._cookies import get_leetcode_session_cookie
+from ._cookies import get_cookies
 
 PROBLEM_API = 'https://leetcode.com/api/problems/all/'
 GRAPHQL_API = 'https://leetcode.com/graphql'
 
 COOKIE = None
 
 
 def fetch_problems() -> list:
     """
     Fetch all problems from LeetCode API
 
     Returns:
         list: tuples with num, title, slug, and question id for each problem
     """
-    response = requests.get(PROBLEM_API)
+    response = requests.get(PROBLEM_API, cookies=COOKIE)
     data = response.json()
 
     problems = []
     for item in data['stat_status_pairs']:
         stat = item['stat']
 
         num = stat['frontend_question_id']
@@ -111,8 +111,8 @@
     }
 
     return _fetch_graphql(payload)['data']['question']
 
 
 def set_cookie(cookie_path: str):
     global COOKIE
-    COOKIE = get_leetcode_session_cookie(cookie_path)
+    COOKIE = get_cookies(cookie_path)
```

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_parsing.py` & `rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_parsing.py`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/_problem_index.py` & `rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/_problem_index.py`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/main.py` & `rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/main.py`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/src/rossmassey/fetch_leetcode_problem/problem_info.py` & `rossmassey_fetch_leetcode_problem-0.2.0/src/rossmassey/fetch_leetcode_problem/problem_info.py`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/.gitignore` & `rossmassey_fetch_leetcode_problem-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/LICENSE` & `rossmassey_fetch_leetcode_problem-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/README.md` & `rossmassey_fetch_leetcode_problem-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/pyproject.toml` & `rossmassey_fetch_leetcode_problem-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/rossmassey/fetch_leetcode_problem"]
 
 [project]
 name = "rossmassey.fetch_leetcode_problem"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
   { name="Ross Massey", email="massey0ross@gmail.com" },
 ]
 description = "A package for getting information about a leetcode problem"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `rossmassey_fetch_leetcode_problem-0.1.4/PKG-INFO` & `rossmassey_fetch_leetcode_problem-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rossmassey.fetch_leetcode_problem
-Version: 0.1.4
+Version: 0.2.0
 Summary: A package for getting information about a leetcode problem
 Project-URL: Homepage, https://github.com/rossmassey/fetch-leetcode-problem
 Project-URL: Documentation, https://rossmassey.github.io/fetch-leetcode-problem/
 Project-URL: Issues, https://github.com/rossmassey/fetch-leetcode-problem/issues
 Author-email: Ross Massey <massey0ross@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

