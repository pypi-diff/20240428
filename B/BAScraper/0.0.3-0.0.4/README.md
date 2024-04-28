# Comparing `tmp/BAScraper-0.0.3.tar.gz` & `tmp/BAScraper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BAScraper-0.0.3.tar", last modified: Thu Feb  1 16:15:47 2024, max compression
+gzip compressed data, was "BAScraper-0.0.4.tar", last modified: Sat Mar 23 16:39:46 2024, max compression
```

## Comparing `BAScraper-0.0.3.tar` & `BAScraper-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 maxjo     (1000) maxjo     (1000)        0 2024-02-01 16:15:47.950199 BAScraper-0.0.3/
-drwxr-xr-x   0 maxjo     (1000) maxjo     (1000)        0 2024-02-01 16:15:47.950199 BAScraper-0.0.3/BAScraper/
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)    25411 2024-02-01 16:14:52.000000 BAScraper-0.0.3/BAScraper/BAScraper.py
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)       32 2024-01-29 13:29:14.000000 BAScraper-0.0.3/BAScraper/__init__.py
-drwxr-xr-x   0 maxjo     (1000) maxjo     (1000)        0 2024-02-01 16:15:47.950199 BAScraper-0.0.3/BAScraper.egg-info/
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)     1038 2024-02-01 16:15:47.000000 BAScraper-0.0.3/BAScraper.egg-info/PKG-INFO
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)      235 2024-02-01 16:15:47.000000 BAScraper-0.0.3/BAScraper.egg-info/SOURCES.txt
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)        1 2024-02-01 16:15:47.000000 BAScraper-0.0.3/BAScraper.egg-info/dependency_links.txt
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)        9 2024-02-01 16:15:47.000000 BAScraper-0.0.3/BAScraper.egg-info/requires.txt
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)       10 2024-02-01 16:15:47.000000 BAScraper-0.0.3/BAScraper.egg-info/top_level.txt
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)     1062 2024-01-19 05:12:00.000000 BAScraper-0.0.3/LICENSE
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)     1038 2024-02-01 16:15:47.950199 BAScraper-0.0.3/PKG-INFO
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)    14214 2024-01-31 01:43:39.000000 BAScraper-0.0.3/README.md
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)       38 2024-02-01 16:15:47.950199 BAScraper-0.0.3/setup.cfg
--rw-r--r--   0 maxjo     (1000) maxjo     (1000)     1454 2024-02-01 12:34:50.000000 BAScraper-0.0.3/setup.py
+drwxr-xr-x   0 maxjo     (1000) maxjo     (1000)        0 2024-03-23 16:39:46.715975 BAScraper-0.0.4/
+drwxr-xr-x   0 maxjo     (1000) maxjo     (1000)        0 2024-03-23 16:39:46.715975 BAScraper-0.0.4/BAScraper/
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)    28306 2024-03-23 16:34:35.000000 BAScraper-0.0.4/BAScraper/BAScraper.py
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)       32 2024-01-29 13:29:14.000000 BAScraper-0.0.4/BAScraper/__init__.py
+drwxr-xr-x   0 maxjo     (1000) maxjo     (1000)        0 2024-03-23 16:39:46.715975 BAScraper-0.0.4/BAScraper.egg-info/
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)     1038 2024-03-23 16:39:46.000000 BAScraper-0.0.4/BAScraper.egg-info/PKG-INFO
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)      235 2024-03-23 16:39:46.000000 BAScraper-0.0.4/BAScraper.egg-info/SOURCES.txt
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)        1 2024-03-23 16:39:46.000000 BAScraper-0.0.4/BAScraper.egg-info/dependency_links.txt
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)        9 2024-03-23 16:39:46.000000 BAScraper-0.0.4/BAScraper.egg-info/requires.txt
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)       10 2024-03-23 16:39:46.000000 BAScraper-0.0.4/BAScraper.egg-info/top_level.txt
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)     1062 2024-01-19 05:12:00.000000 BAScraper-0.0.4/LICENSE
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)     1038 2024-03-23 16:39:46.715975 BAScraper-0.0.4/PKG-INFO
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)    14214 2024-01-31 01:43:39.000000 BAScraper-0.0.4/README.md
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)       38 2024-03-23 16:39:46.715975 BAScraper-0.0.4/setup.cfg
+-rw-r--r--   0 maxjo     (1000) maxjo     (1000)     1521 2024-03-23 16:39:23.000000 BAScraper-0.0.4/setup.py
```

### Comparing `BAScraper-0.0.3/BAScraper/BAScraper.py` & `BAScraper-0.0.4/BAScraper/BAScraper.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import List
 from datetime import datetime
 
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from queue import Queue
 
 import os
-from threading import Lock
+from threading import Lock, RLock
 import pprint
 pretty = pprint.PrettyPrinter(indent=4).pprint
 
 # imports no longer used
 # from dotenv import load_dotenv
 
 
@@ -34,40 +34,60 @@
                  backoffsec=3,
                  max_retries=5,
                  timeout=10,
                  threads=4,
                  comment_t=None,
                  batch_size=0,
                  log_level='INFO',
-                 cwd=os.getcwd()):
+                 cwd=os.getcwd(),
+                 pace_mode='auto-hard'):
 
         """
         might add these params from pmaw
         mem_safe (boolean, optional): If True, stores responses in cache during operation, defaults to False
         safe_exit (boolean, optional): If True, will safely exit if interrupted by storing current responses
         and requests in the cache. Will also load previous requests / responses if found in cache, defaults to False
+
+        ! new ratelimit -> 30 requests per 60 seconds = 3 requests per second ->
+        soft limit starting from 15 requests per second (1.5 requests per second)
+        hard limit starting from 30 requests per second (3 requests per second)
+        hard limit starting from 1k requests per hour (1 request every 4 second)
         """
 
+        # variables for managing rate limits
+        # rate limit as of feb 9th 2023
+        assert pace_mode in ['auto-soft', 'auto-hard', 'manual']
+        self.max_pool_amount_soft = 15
+        self.max_pool_amount_hard = 30
+        self.refill_second = 60
+        self.last_refilled = time.time()
+        self.pace_mode = pace_mode  # auto by default
+        if pace_mode == 'auto-soft':
+            self.max_pool_amount = self.max_pool_amount_soft
+        elif pace_mode == 'auto-hard':
+            self.max_pool_amount = self.max_pool_amount_hard
+        self.pool_amount = self.max_pool_amount
+        self.throttling = False  # needed this since the threads can't get out of throttled state
+        # (needs shared throttled/not-throttled state)
+        self.pool_lock = RLock()
+        self.throttle_lock = RLock()
+
         self.sleepsec = sleepsec  # cooldown per request
         self.backoffsec = backoffsec  # backoff amount after error happens in request
         self.threads = threads  # no. of threads if multithreading is used
         self.max_retries = max_retries  # maximum retry times
         self.timeout = timeout  # time until it's considered as timout err
         self.comment_t = comment_t if comment_t else threads  # no. of threads used for comment fetching, defaults to 'threads'
         self.batch_size = batch_size  # not implemented yet, for RAM offload to disk
 
         self.submission_url = 'https://api.pullpush.io/reddit/search/submission/'
         self.comment_url = 'https://api.pullpush.io/reddit/search/comment/'
 
         self.cwd = cwd
 
-        # Rlocks are no longer used for now
-        # self.print_lock = RLock()
-        self.file_lock = Lock()
-
         # google custom search engine creds
         try:
             self.cse_id = creds.CSE_ID
             self.cse_api = creds.CSE_API_KEY
             print('CSE credentials detected.')
 
         except (NameError, AttributeError):
@@ -86,14 +106,55 @@
 
         # create console handler and set level
         ch = logging.StreamHandler()
         ch.setLevel(log_level)  # CHANGE HERE TO CONTROL DISPLAYED LOG MESSAGE LEVEL
         ch.setFormatter(logging.Formatter('%(levelname)s - %(message)s'))
         self.logger.addHandler(ch)
 
+    def request_sleep(self, thread_no=None, sleepsec=None):
+        sleepsec = self.sleepsec if sleepsec is None else sleepsec
+
+        match self.pace_mode:
+            case 'auto-soft' | 'auto-hard':
+                self.pool_lock.acquire()
+                if time.time() - self.last_refilled > self.refill_second:
+                    self.pool_amount = self.max_pool_amount
+                    self.last_refilled = time.time()
+                    self.logger.info(f't-{thread_no}: pool refilled!')
+
+                if self.pool_amount > 0:
+                    time.sleep(sleepsec)
+                    self.pool_amount -= 1
+                    self.pool_lock.release()
+                    return
+
+                else:
+                    self.pool_lock.release()
+                    with self.throttle_lock:
+                        self.throttling = True
+                        s = self.refill_second - (time.time() - self.last_refilled)
+                        self.logger.info(f't-{thread_no}: soft/hard limit reached! throttling for {s}...')
+                        self.logger.info(f'sleeping for {s}sec')
+                        time.sleep(s)
+                        '''
+                        while True:
+                            if (time.time() - self.last_refilled > self.refill_second) or not self.throttling:
+                                self.throttling = False
+                                break
+                            time.sleep(1)
+                        '''
+                    self.request_sleep(thread_no)
+
+            case 'manual':
+                time.sleep(sleepsec)
+                return
+
+            case _:
+                raise Exception(f'{thread_no}: Wrong variable for `mode`!')
+
     # TODO: make it so that when `ids` field is used,
     #  try to use `_make_request_from_queued_id` function for large batches
     def get_submissions(self,
                         after: datetime = None,
                         before: datetime = None,
                         get_comments: bool = False,
                         duplicate_action: str = 'newest',
@@ -272,38 +333,40 @@
         retries = 0
         while retries < self.max_retries:
             try:
                 if 'after' in params:
                     params['after'] = params['after']-1
 
                 response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
-
                 result = response.json()['data']
 
                 if response.ok:
-                    self.logger.info(
-                        f"t-{thread_id}: {response.status_code} - {len(result)} - {response.elapsed}")
+                    with self.pool_lock:
+                        self.logger.info(
+                            f"t-{thread_id}: pool: {self.pool_amount} | len: {len(result)} | time: {response.elapsed}")
                 else:
                     self.logger.error(f"t-{thread_id}: {response.status_code} - {response.elapsed}"
                                       f"\n{response.text}\n")
 
-                time.sleep(self.sleepsec)
+                self.request_sleep(thread_id)
                 return result
 
-            except (requests.exceptions.Timeout, requests.exceptions.ConnectionError) as err:
+            except (requests.exceptions.Timeout,
+                    requests.exceptions.ConnectionError,
+                    requests.exceptions.HTTPError) as err:
                 retries += 1
                 self.logger.warning(
                     f"t-{thread_id}: {err}\nRetrying... Attempt {retries}/{self.max_retries}")
-                time.sleep(self.backoffsec * retries)  # backoff
+                self.request_sleep(thread_id, self.backoffsec * retries)  # backoff
 
             except json.decoder.JSONDecodeError:
                 retries += 1
                 self.logger.warning(
                     f"t-{thread_id}: JSONDecodeError: Retrying... Attempt {retries}/{self.max_retries}")
-                time.sleep(self.backoffsec * retries)  # backoff
+                self.request_sleep(thread_id, self.backoffsec * retries)  # backoff
 
             except Exception as err:
                 raise Exception(f't-{thread_id}: unexpected error: {err}')
 
         self.logger.error(f't-{thread_id}: failed request attempt. skipping...')
         return list()
 
@@ -402,22 +465,18 @@
                         if self.is_deleted(post):
                             indexed[link_id] = post  # default keeping the newest deleted version for no
                 case _:
                     raise Exception(f'invalid parameter for `duplicate_action`: '
                                     f"should be one of ['newest', 'oldest', 'remove', 'keep_original', 'keep_removed']")
 
         # delete all the submission/comment that has placeholders remaining
-        del_list = list()
-        for k, v in indexed.items():
-            if v == 'dupe':
-                del_list.append(k)
-        for k in del_list:
-            if k in del_list:
-                self.logger.warning(f'failed `is_deleted` detection. deleting {k} from results!')
-                del indexed[k]
+        def alert_dupe(k):
+            self.logger.warning(f'failed `is_deleted` detection. deleting {k} from results!')
+            return k
+        indexed = {alert_dupe(k): v for k, v in indexed.items() if v != 'dupe'}
 
         """
         so the is_deleted function sometimes return all the dupes as either all False or True. 
         (False positives/ False negatives and so on)
         Which will prevent the 'dupe' placeholder from getting replaced, later causing errors.
         
         for now I made it so that it'll just delete the submission/comment that has placeholders remaining
```

### Comparing `BAScraper-0.0.3/BAScraper.egg-info/PKG-INFO` & `BAScraper-0.0.4/BAScraper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BAScraper
-Version: 0.0.3
+Version: 0.0.4
 Summary: API wrapper for PullPush.io - the 3rd party replacement API for Reddit.
 Author: maxjo
 Author-email: jo@yeongmin.net
 Project-URL: Github, https://github.com/maxjo020418/BAScraper
 Keywords: reddit scraper,reddit,scraper,pullpush,wrapper
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `BAScraper-0.0.3/LICENSE` & `BAScraper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BAScraper-0.0.3/PKG-INFO` & `BAScraper-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BAScraper
-Version: 0.0.3
+Version: 0.0.4
 Summary: API wrapper for PullPush.io - the 3rd party replacement API for Reddit.
 Author: maxjo
 Author-email: jo@yeongmin.net
 Project-URL: Github, https://github.com/maxjo020418/BAScraper
 Keywords: reddit scraper,reddit,scraper,pullpush,wrapper
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `BAScraper-0.0.3/README.md` & `BAScraper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `BAScraper-0.0.3/setup.py` & `BAScraper-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # run `python -m build` to build
+# `twine check dist/*` to verify
+# `twine upload dist/*` to upload
 # check https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html#summary for details
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'API wrapper for PullPush.io - the 3rd party replacement API for Reddit.'
 LONG_DESCRIPTION = '''currently it can:
 - get submissions/comments from a certain subreddit in supported order/sorting methods specified in the PullPush.io API docs
 - get comments under the retrieved submissions
 - can get all the submissions based on the number of submissions or in a certain timeframe you specify
 - can recover(if possible) deleted/removed submission/comments from the returned result
 check the [documentation on the github](https://github.com/maxjo020418/BAScraper) for detailed info
```

