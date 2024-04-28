# Comparing `tmp/fastapi_simple_rate_limiter-0.0.2.tar.gz` & `tmp/fastapi_simple_rate_limiter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_simple_rate_limiter-0.0.2.tar", max compression
+gzip compressed data, was "fastapi_simple_rate_limiter-0.0.3.tar", max compression
```

## Comparing `fastapi_simple_rate_limiter-0.0.2.tar` & `fastapi_simple_rate_limiter-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-10-03 15:11:02.729119 fastapi_simple_rate_limiter-0.0.2/LICENSE
--rw-r--r--   0        0        0     5291 2023-10-03 15:21:31.191598 fastapi_simple_rate_limiter-0.0.2/README.md
--rw-r--r--   0        0        0      164 2023-10-06 15:09:15.646781 fastapi_simple_rate_limiter-0.0.2/fastapi_simple_rate_limiter/__init__.py
--rw-r--r--   0        0        0      851 2023-10-03 13:36:37.763137 fastapi_simple_rate_limiter-0.0.2/fastapi_simple_rate_limiter/database.py
--rw-r--r--   0        0        0      320 2023-10-03 13:36:37.766349 fastapi_simple_rate_limiter-0.0.2/fastapi_simple_rate_limiter/exception.py
--rw-r--r--   0        0        0     4575 2023-10-06 15:09:15.641317 fastapi_simple_rate_limiter-0.0.2/fastapi_simple_rate_limiter/limiter.py
--rw-r--r--   0        0        0      431 2023-10-06 15:09:15.651778 fastapi_simple_rate_limiter-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 fastapi_simple_rate_limiter-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-10-03 15:11:02.729119 fastapi_simple_rate_limiter-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6445 2024-04-28 13:26:03.153666 fastapi_simple_rate_limiter-0.0.3/README.md
+-rw-r--r--   0        0        0      200 2024-04-28 12:56:16.315196 fastapi_simple_rate_limiter-0.0.3/fastapi_simple_rate_limiter/__init__.py
+-rw-r--r--   0        0        0      851 2023-10-03 13:36:37.763137 fastapi_simple_rate_limiter-0.0.3/fastapi_simple_rate_limiter/database.py
+-rw-r--r--   0        0        0      320 2023-10-03 13:36:37.766349 fastapi_simple_rate_limiter-0.0.3/fastapi_simple_rate_limiter/exception.py
+-rw-r--r--   0        0        0    10208 2024-04-28 13:12:17.821001 fastapi_simple_rate_limiter-0.0.3/fastapi_simple_rate_limiter/limiter.py
+-rw-r--r--   0        0        0      431 2024-04-28 13:29:05.228134 fastapi_simple_rate_limiter-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6901 1970-01-01 00:00:00.000000 fastapi_simple_rate_limiter-0.0.3/PKG-INFO
```

### Comparing `fastapi_simple_rate_limiter-0.0.2/LICENSE` & `fastapi_simple_rate_limiter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_simple_rate_limiter-0.0.2/README.md` & `fastapi_simple_rate_limiter-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fastapi-simple-rate-limiter
+Version: 0.0.3
+Summary: Rate limiter to limit the number of API requests in FastAPI
+Author: jintaekimmm
+Author-email: jintae.kimmm@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: redis (>=5.0.1,<6.0.0)
+Description-Content-Type: text/markdown
+
 # FastAPI Simple RateLimiter
 
 This package contains the API Rate limit decorator for use in FastAPI.
 
 It is easy to use, can only be specified in a specific API URL Path, and can be used without special storage (in memory).
 
 Additionally, you can use redis to properly share and control the API rate limit value even in multi-instance situations.
@@ -147,14 +160,48 @@
 ```
 
 You can return results as a JSONResponse in the desired format via a custom exception.
 
 However, when creating a custom exception, there is a limitation that only `status_code` and `message` can be used. Since the limits of the structure are not checked within `message`, it seems that it can have a free form.
 
 
+## New Feature: FailedLimiter
+
+This limiter has the ability to restrict access after a certain number of failures.
+
+For example, you might want to limit indiscriminate access to an authentication function like login (e.g., you might want to block a user for 30 minutes after 5 incorrect password entries).
+
+```python
+from fastapi import FastAPI
+from fastapi.requests import Request
+
+from fastapi_simple_rate_limiter import FailedLimiter
+
+failed_limiter = FailedLimiter(limit=3, seconds=300, redis=r)
+
+
+@app.get("/login")
+@failed_limiter
+async def test_login_api(request: Request):
+    if auth_ok:
+        # After successful login, reset the failure count
+        await failed_limiter.reset(request)
+    else:
+        # If login fails, increment the number of failures
+        await failed_limiter.fail_up(request)
+```
+This API route restricts access for 300 seconds after three failures
+
+The decorator requires limit and seconds to be set, and allows you to enter the number of failures to limit and the time to limit access
+
+Otherwise, the available options can be set the same as for rate_limiter
+
+Both custom exception and redis storage can be used
+
+
 ## Get client real IP Address
 
 When checking the API rate limit, use a key combining the client's IP address and API url path.
 
 If all client IP addresses are the same, the rate limit will be shared by all users rather than individual users.
 
 Here we introduce a method to check the actual IP address of the client when using uvicorn and gunicorn.
@@ -177,8 +224,8 @@
 
 ```shell
 gunicorn app.main:app --bind 0.0.0.0:8000 -k uvicorn.workers.UvicornWorker --forwarded-allow-ips "*"
 ```
 
 ## License
 
-This project is licensed under the terms of the MIT license.
+This project is licensed under the terms of the MIT license.
```

### Comparing `fastapi_simple_rate_limiter-0.0.2/fastapi_simple_rate_limiter/database.py` & `fastapi_simple_rate_limiter-0.0.3/fastapi_simple_rate_limiter/database.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_rate_limiter-0.0.2/PKG-INFO` & `fastapi_simple_rate_limiter-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fastapi-simple-rate-limiter
-Version: 0.0.2
-Summary: Rate limiter to limit the number of API requests in FastAPI
-Author: jintaekimmm
-Author-email: jintae.kimmm@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: redis (>=5.0.1,<6.0.0)
-Description-Content-Type: text/markdown
-
 # FastAPI Simple RateLimiter
 
 This package contains the API Rate limit decorator for use in FastAPI.
 
 It is easy to use, can only be specified in a specific API URL Path, and can be used without special storage (in memory).
 
 Additionally, you can use redis to properly share and control the API rate limit value even in multi-instance situations.
@@ -160,14 +147,48 @@
 ```
 
 You can return results as a JSONResponse in the desired format via a custom exception.
 
 However, when creating a custom exception, there is a limitation that only `status_code` and `message` can be used. Since the limits of the structure are not checked within `message`, it seems that it can have a free form.
 
 
+## New Feature: FailedLimiter
+
+This limiter has the ability to restrict access after a certain number of failures.
+
+For example, you might want to limit indiscriminate access to an authentication function like login (e.g., you might want to block a user for 30 minutes after 5 incorrect password entries).
+
+```python
+from fastapi import FastAPI
+from fastapi.requests import Request
+
+from fastapi_simple_rate_limiter import FailedLimiter
+
+failed_limiter = FailedLimiter(limit=3, seconds=300, redis=r)
+
+
+@app.get("/login")
+@failed_limiter
+async def test_login_api(request: Request):
+    if auth_ok:
+        # After successful login, reset the failure count
+        await failed_limiter.reset(request)
+    else:
+        # If login fails, increment the number of failures
+        await failed_limiter.fail_up(request)
+```
+This API route restricts access for 300 seconds after three failures
+
+The decorator requires limit and seconds to be set, and allows you to enter the number of failures to limit and the time to limit access
+
+Otherwise, the available options can be set the same as for rate_limiter
+
+Both custom exception and redis storage can be used
+
+
 ## Get client real IP Address
 
 When checking the API rate limit, use a key combining the client's IP address and API url path.
 
 If all client IP addresses are the same, the rate limit will be shared by all users rather than individual users.
 
 Here we introduce a method to check the actual IP address of the client when using uvicorn and gunicorn.
@@ -190,8 +211,8 @@
 
 ```shell
 gunicorn app.main:app --bind 0.0.0.0:8000 -k uvicorn.workers.UvicornWorker --forwarded-allow-ips "*"
 ```
 
 ## License
 
-This project is licensed under the terms of the MIT license.
+This project is licensed under the terms of the MIT license.
```

