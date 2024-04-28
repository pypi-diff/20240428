# Comparing `tmp/gppt-4.0.1.tar.gz` & `tmp/gppt-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gppt-4.0.1.tar", max compression
+gzip compressed data, was "gppt-4.1.0.tar", max compression
```

## Comparing `gppt-4.0.1.tar` & `gppt-4.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1046 2024-02-14 13:42:44.494561 gppt-4.0.1/LICENSE.txt
--rw-r--r--   0        0        0     5004 2024-02-14 13:42:44.494561 gppt-4.0.1/README.md
--rw-r--r--   0        0        0      543 2024-02-14 13:42:44.494561 gppt-4.0.1/gppt/__init__.py
--rw-r--r--   0        0        0     2442 2024-02-14 13:42:44.494561 gppt-4.0.1/gppt/auth.py
--rw-r--r--   0        0        0      508 2024-02-14 13:42:44.494561 gppt-4.0.1/gppt/consts.py
--rw-r--r--   0        0        0     6002 2024-02-14 13:42:44.494561 gppt-4.0.1/gppt/gppt.py
--rw-r--r--   0        0        0     4203 2024-02-14 13:42:44.494561 gppt-4.0.1/gppt/main.py
--rw-r--r--   0        0        0        0 2024-02-14 13:42:44.494561 gppt-4.0.1/gppt/py.typed
--rw-r--r--   0        0        0      829 2024-02-14 13:42:44.494561 gppt-4.0.1/gppt/types.py
--rw-r--r--   0        0        0     2358 2024-02-14 13:42:44.494561 gppt-4.0.1/gppt/utils.py
--rw-r--r--   0        0        0     1722 2024-02-14 13:42:44.494561 gppt-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 gppt-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1046 2024-04-28 20:00:57.856616 gppt-4.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     5004 2024-04-28 20:00:57.856616 gppt-4.1.0/README.md
+-rw-r--r--   0        0        0      543 2024-04-28 20:00:57.856616 gppt-4.1.0/gppt/__init__.py
+-rw-r--r--   0        0        0     2442 2024-04-28 20:00:57.856616 gppt-4.1.0/gppt/auth.py
+-rw-r--r--   0        0        0      508 2024-04-28 20:00:57.856616 gppt-4.1.0/gppt/consts.py
+-rw-r--r--   0        0        0     6030 2024-04-28 20:00:57.856616 gppt-4.1.0/gppt/gppt.py
+-rw-r--r--   0        0        0     4203 2024-04-28 20:00:57.856616 gppt-4.1.0/gppt/main.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:00:57.856616 gppt-4.1.0/gppt/py.typed
+-rw-r--r--   0        0        0      829 2024-04-28 20:00:57.856616 gppt-4.1.0/gppt/types.py
+-rw-r--r--   0        0        0     2358 2024-04-28 20:00:57.856616 gppt-4.1.0/gppt/utils.py
+-rw-r--r--   0        0        0     1723 2024-04-28 20:00:57.856616 gppt-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 gppt-4.1.0/PKG-INFO
```

### Comparing `gppt-4.0.1/LICENSE.txt` & `gppt-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gppt-4.0.1/README.md` & `gppt-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gppt-4.0.1/gppt/__init__.py` & `gppt-4.1.0/gppt/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     LoginInfo,
     LoginUserInfo,
     OAuthAPIResponse,
     PixivLoginFailed,
     ProfileURIs,
 )
 
-__version__ = "4.0.1"
+__version__ = "4.1.0"
 
 __all__ = [
     "PixivAuth",
     "PixivAuth",
     "LoginCred",
     "LoginInfo",
     "LoginUserInfo",
```

### Comparing `gppt-4.0.1/gppt/auth.py` & `gppt-4.1.0/gppt/auth.py`

 * *Files identical despite different names*

### Comparing `gppt-4.0.1/gppt/gppt.py` & `gppt-4.1.0/gppt/gppt.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,19 +133,19 @@
             proxies=PROXIES,
             timeout=TIMEOUT,
         )
         return cast(LoginInfo, response.json())
 
     def __fill_login_form(self) -> None:
         if self.username:
-            el = self.driver.find_element(By.XPATH, "//input[@autocomplete='username']")
+            el = self.driver.find_element(By.XPATH, "//input[starts-with(@autocomplete, 'username')]")
             _slow_type(el, self.username)
 
         if self.password:
-            el = self.driver.find_element(By.XPATH, "//input[@autocomplete='current-password']")
+            el = self.driver.find_element(By.XPATH, "//input[starts-with(@autocomplete, 'current-password')]")
             _slow_type(el, self.password)
 
     def __try_login(self) -> None:
         label_selectors = [f"contains(text(), '{label}')" for label in ["ログイン", "Log In", "登录", "로그인", "登入"]]
         el = self.driver.find_element(By.XPATH, f"//button[@type='submit'][{' or '.join(label_selectors)}]")
         el.send_keys(Keys.ENTER)
```

### Comparing `gppt-4.0.1/gppt/main.py` & `gppt-4.1.0/gppt/main.py`

 * *Files identical despite different names*

### Comparing `gppt-4.0.1/gppt/types.py` & `gppt-4.1.0/gppt/types.py`

 * *Files identical despite different names*

### Comparing `gppt-4.0.1/gppt/utils.py` & `gppt-4.1.0/gppt/utils.py`

 * *Files identical despite different names*

### Comparing `gppt-4.0.1/pyproject.toml` & `gppt-4.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 description = "Get your Pixiv token (for running upbit/pixivpy)"
 keywords = ["pixiv", "api", "token"]
 name = "gppt"
 packages = [{include = "gppt"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/get-pixivpy-token"
-version = "4.0.1"
+version = "4.1.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 pixivpy3 = "^3.7.3"
 pwinput = "^1.0.3"
 requests = "^2.31.0"
 selenium = "^4.14.0"
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.991,<1.9"
+mypy = ">=0.991,<1.10"
 pre-commit = ">=2.20,<4.0"
 taskipy = "^1.10.3"
 types-requests = "^2.28.11.15"
 pytest = ">=7.2.2,<9.0.0"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 
 [tool.poetry.scripts]
 gppt = "gppt.main:main"
 
 [tool.black]
 line-length = 120
 target-version = ['py39']
```

### Comparing `gppt-4.0.1/PKG-INFO` & `gppt-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gppt
-Version: 4.0.1
+Version: 4.1.0
 Summary: Get your Pixiv token (for running upbit/pixivpy)
 Home-page: https://github.com/eggplants/get-pixivpy-token
 License: MIT
 Keywords: pixiv,api,token
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.8,<4
```

