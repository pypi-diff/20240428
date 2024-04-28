# Comparing `tmp/tweety_ns-1.1.4b0.tar.gz` & `tmp/tweety_ns-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety_ns-1.1.4b0.tar", last modified: Sat Apr 27 10:33:45 2024, max compression
+gzip compressed data, was "tweety_ns-1.1.5.tar", last modified: Sun Apr 28 18:06:24 2024, max compression
```

## Comparing `tweety_ns-1.1.4b0.tar` & `tweety_ns-1.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 10:33:45.788365 tweety_ns-1.1.4b0/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1893 2024-04-27 10:33:45.788365 tweety_ns-1.1.4b0/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety_ns-1.1.4b0/README.md
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety_ns-1.1.4b0/pyproject.toml
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      673 2024-04-27 10:33:45.788365 tweety_ns-1.1.4b0/setup.cfg
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      787 2024-04-27 10:30:57.000000 tweety_ns-1.1.4b0/setup.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 10:33:45.780365 tweety_ns-1.1.4b0/src/
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 10:33:45.784365 tweety_ns-1.1.4b0/src/tweety/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      278 2024-04-27 10:32:00.000000 tweety_ns-1.1.4b0/src/tweety/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7526 2024-04-27 08:15:36.000000 tweety_ns-1.1.4b0/src/tweety/auth.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31976 2024-04-27 09:34:06.000000 tweety_ns-1.1.4b0/src/tweety/bot.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    98004 2024-04-27 09:42:49.000000 tweety_ns-1.1.4b0/src/tweety/builder.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 10:33:45.784365 tweety_ns-1.1.4b0/src/tweety/events/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety_ns-1.1.4b0/src/tweety/events/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2083 2024-04-27 09:38:42.000000 tweety_ns-1.1.4b0/src/tweety/events/newmessage.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    22029 2024-04-14 08:52:30.000000 tweety_ns-1.1.4b0/src/tweety/exceptions_.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2343 2024-04-23 07:03:34.000000 tweety_ns-1.1.4b0/src/tweety/filters.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20593 2024-04-27 09:09:11.000000 tweety_ns-1.1.4b0/src/tweety/http.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2362 2024-04-10 16:34:41.000000 tweety_ns-1.1.4b0/src/tweety/session.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 10:33:45.788365 tweety_ns-1.1.4b0/src/tweety/types/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety_ns-1.1.4b0/src/tweety/types/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3094 2024-04-27 09:46:41.000000 tweety_ns-1.1.4b0/src/tweety/types/base.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety_ns-1.1.4b0/src/tweety/types/bookmarks.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety_ns-1.1.4b0/src/tweety/types/community.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety_ns-1.1.4b0/src/tweety/types/follow.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety_ns-1.1.4b0/src/tweety/types/gifs.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20705 2024-04-27 10:29:57.000000 tweety_ns-1.1.4b0/src/tweety/types/inbox.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety_ns-1.1.4b0/src/tweety/types/likes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety_ns-1.1.4b0/src/tweety/types/lists.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety_ns-1.1.4b0/src/tweety/types/mentions.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9022 2024-04-10 16:29:13.000000 tweety_ns-1.1.4b0/src/tweety/types/n_types.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety_ns-1.1.4b0/src/tweety/types/notification.py
--rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety_ns-1.1.4b0/src/tweety/types/places.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety_ns-1.1.4b0/src/tweety/types/retweets.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety_ns-1.1.4b0/src/tweety/types/search.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety_ns-1.1.4b0/src/tweety/types/topic.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58815 2024-04-14 08:56:44.000000 tweety_ns-1.1.4b0/src/tweety/types/twDataTypes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-04-12 07:15:06.000000 tweety_ns-1.1.4b0/src/tweety/types/usertweet.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety_ns-1.1.4b0/src/tweety/updates.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36810 2024-04-27 09:40:36.000000 tweety_ns-1.1.4b0/src/tweety/user.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6586 2024-04-25 11:56:51.000000 tweety_ns-1.1.4b0/src/tweety/utils.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-27 10:33:45.788365 tweety_ns-1.1.4b0/src/tweety_ns.egg-info/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1893 2024-04-27 10:33:45.000000 tweety_ns-1.1.4b0/src/tweety_ns.egg-info/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-27 10:33:45.000000 tweety_ns-1.1.4b0/src/tweety_ns.egg-info/SOURCES.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-27 10:33:45.000000 tweety_ns-1.1.4b0/src/tweety_ns.egg-info/dependency_links.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-27 10:33:45.000000 tweety_ns-1.1.4b0/src/tweety_ns.egg-info/requires.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-27 10:33:45.000000 tweety_ns-1.1.4b0/src/tweety_ns.egg-info/top_level.txt
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety_ns-1.1.5/README.md
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety_ns-1.1.5/pyproject.toml
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/setup.cfg
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      785 2024-04-28 18:03:59.000000 tweety_ns-1.1.5/setup.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.239461 tweety_ns-1.1.5/src/
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.243461 tweety_ns-1.1.5/src/tweety/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      276 2024-04-28 18:03:47.000000 tweety_ns-1.1.5/src/tweety/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7526 2024-04-27 08:15:36.000000 tweety_ns-1.1.5/src/tweety/auth.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31976 2024-04-27 09:34:06.000000 tweety_ns-1.1.5/src/tweety/bot.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    99908 2024-04-28 16:22:34.000000 tweety_ns-1.1.5/src/tweety/builder.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.243461 tweety_ns-1.1.5/src/tweety/events/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety_ns-1.1.5/src/tweety/events/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2083 2024-04-27 09:38:42.000000 tweety_ns-1.1.5/src/tweety/events/newmessage.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    22029 2024-04-14 08:52:30.000000 tweety_ns-1.1.5/src/tweety/exceptions_.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2343 2024-04-23 07:03:34.000000 tweety_ns-1.1.5/src/tweety/filters.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    21533 2024-04-28 17:21:24.000000 tweety_ns-1.1.5/src/tweety/http.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2362 2024-04-10 16:34:41.000000 tweety_ns-1.1.5/src/tweety/session.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/src/tweety/types/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1363 2024-04-28 17:55:38.000000 tweety_ns-1.1.5/src/tweety/types/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3094 2024-04-28 09:58:11.000000 tweety_ns-1.1.5/src/tweety/types/base.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety_ns-1.1.5/src/tweety/types/bookmarks.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety_ns-1.1.5/src/tweety/types/community.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety_ns-1.1.5/src/tweety/types/follow.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety_ns-1.1.5/src/tweety/types/gifs.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    23118 2024-04-28 17:55:38.000000 tweety_ns-1.1.5/src/tweety/types/inbox.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety_ns-1.1.5/src/tweety/types/likes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety_ns-1.1.5/src/tweety/types/lists.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety_ns-1.1.5/src/tweety/types/mentions.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9173 2024-04-28 17:48:11.000000 tweety_ns-1.1.5/src/tweety/types/n_types.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety_ns-1.1.5/src/tweety/types/notification.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety_ns-1.1.5/src/tweety/types/places.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety_ns-1.1.5/src/tweety/types/retweets.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety_ns-1.1.5/src/tweety/types/search.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety_ns-1.1.5/src/tweety/types/topic.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58815 2024-04-14 08:56:44.000000 tweety_ns-1.1.5/src/tweety/types/twDataTypes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-04-12 07:15:06.000000 tweety_ns-1.1.5/src/tweety/types/usertweet.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety_ns-1.1.5/src/tweety/updates.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    39586 2024-04-28 18:03:47.000000 tweety_ns-1.1.5/src/tweety/user.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6771 2024-04-28 18:03:47.000000 tweety_ns-1.1.5/src/tweety/utils.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/src/tweety_ns.egg-info/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/requires.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety_ns-1.1.4b0/PKG-INFO` & `tweety_ns-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.4b0
+Version: 1.1.5
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety_ns-1.1.4b0/README.md` & `tweety_ns-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/setup.cfg` & `tweety_ns-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tweety-ns
-version = 1.1.4b0
+version = 1.1.5
 author = Tayyab Kharl
 author_email = tayyabmahr@gmail.com
 description = An easy Twitter Scraper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mahrtayyab/tweety
 project_urls =
```

### Comparing `tweety_ns-1.1.4b0/src/tweety/auth.py` & `tweety_ns-1.1.5/src/tweety/auth.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/bot.py` & `tweety_ns-1.1.5/src/tweety/bot.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/builder.py` & `tweety_ns-1.1.5/src/tweety/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,17 @@
     URL_TWEET_ANALYTICS = "https://twitter.com/i/api/graphql/vnwexpl0q33_Bky-SROVww/TweetActivityQuery"
     URL_TWEET_TRANSLATE = "https://twitter.com/i/api/1.1/strato/column/None/tweetId={},destinationLanguage={},translationSource=Some(Google),feature=None,timeout=None,onlyCached=None/translation/service/translateTweet"
     URL_TWEET_DETAILS_AS_GUEST = "https://api.twitter.com/graphql/5GOHgZe-8U2j5sVHQzEm9A/TweetResultByRestId"
     URL_TWEET_HISTORY = "https://twitter.com/i/api/graphql/MYJ08HcXJuxtXMXWMP-63w/TweetEditHistory"
     URL_AUSER_INITIAL_INBOX = "https://twitter.com/i/api/1.1/dm/inbox_initial_state.json"  # noqa
     URL_AUSER_INBOX_UPDATES = "https://twitter.com/i/api/1.1/dm/user_updates.json"  # noqa
     URL_AUSER_TRUSTED_INBOX = "https://twitter.com/i/api/1.1/dm/inbox_timeline/trusted.json"  # noqa
+    URL_AUSER_UNTRUSTED_INBOX = "https://twitter.com/i/api/1.1/dm/inbox_timeline/untrusted.json"  # noqa
+    URL_AUSER_UPDATE_GROUP_NAME = "https://twitter.com/i/api/1.1/dm/conversation/{}/update_name.json"  # noqa
+    URL_AUSER_UPDATE_GROUP_AVATAR = "https://twitter.com/i/api/1.1/dm/conversation/{}/update_avatar.json"  # noqa
     URL_AUSER_NOTIFICATION_MENTIONS = "https://twitter.com/i/api/2/notifications/mentions.json"  # noqa
     URL_AUSER_SETTINGS = "https://api.twitter.com/1.1/account/settings.json"  # noqa
     URL_AUSER_ADD_GROUP_MEMBER = "https://twitter.com/i/api/graphql/oBwyQ0_xVbAQ8FAyG0pCRA/AddParticipantsMutation"  # noqa
     URL_AUSER_SEND_MESSAGE = "https://twitter.com/i/api/1.1/dm/new2.json"  # noqa
     URL_AUSER_CONVERSATION = "https://twitter.com/i/api/1.1/dm/conversation/{}.json"  # noqa
     URL_AUSER_CREATE_TWEET = "https://twitter.com/i/api/graphql/tTsjMKyhajZvK4q76mpIBg/CreateTweet"  # noqa
     URL_AUSER_DELETE_TWEET = "https://twitter.com/i/api/graphql/VaenaVgh5q5ih7kvyVjgtg/DeleteTweet"  # noqa
@@ -717,14 +720,15 @@
             'krs_registration_enabled': True,
             'cards_platform': 'Web-12',
             'include_cards': '1',
             'include_ext_alt_text': True,
             'include_ext_limited_action_results': True,
             'include_quote_count': True,
             'include_reply_count': '1',
+            'count': 100,
             'tweet_mode': 'extended',
             'include_ext_views': True,
             'dm_users': True,
             'include_groups': True,
             'include_inbox_timelines': True,
             'include_ext_media_color': True,
             'supports_reactions': True,
@@ -771,15 +775,15 @@
             'include_inbox_timelines': True,
             'include_ext_media_color': True,
             'supports_reactions': True,
             'include_ext_edit_control': True,
             'ext': 'mediaColor,altText,mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl',
         }
 
-        return "GET", self._build(self.URL_AUSER_TRUSTED_INBOX, urlencode(params))
+        return "GET", self._build(self.URL_AUSER_UNTRUSTED_INBOX, urlencode(params))
 
     @return_with_headers
     def get_conversation_with_messages(self, conversation_id, max_id=None):
         params = {
             'context': 'FETCH_DM_CONVERSATION',
             'include_profile_interstitial_type': '1',
             'include_blocking': '1',
@@ -856,14 +860,53 @@
 
         params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features)),
                   'fieldToggles': str(json.dumps(fieldToggles))}
 
         return "GET", self._build(self.URL_AUSER_BOOKMARK, urlencode(params))
 
     @return_with_headers
+    def create_group(self, participants, first_message):
+        params = {
+            'ext': 'mediaColor,altText,mediaStats,highlightedLabel,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl,article',
+            'include_ext_alt_text': 'true',
+            'include_ext_limited_action_results': 'true',
+            'include_reply_count': '1',
+            'tweet_mode': 'extended',
+            'include_ext_views': 'true',
+            'include_groups': 'true',
+            'include_inbox_timelines': 'true',
+            'include_ext_media_color': 'true',
+            'supports_reactions': 'true',
+        }
+
+        json_data = {
+            'recipient_ids': participants,
+            'request_id': utils.create_request_id(),
+            'text': first_message,
+            'cards_platform': 'Web-12',
+            'include_cards': 1,
+            'include_quote_count': True,
+            'dm_users': False,
+        }
+
+        return "POST", self._build(self.URL_AUSER_SEND_MESSAGE, urlencode(params)), json_data
+
+    @return_with_headers
+    def update_conversation_group_name(self, conversation_id, name):
+        data = {'name': name}
+        url = self.URL_AUSER_UPDATE_GROUP_NAME.format(conversation_id)
+        return "POST", url, None, data
+
+    @return_with_headers
+    def update_conversation_group_avatar(self, conversation_id, avatar_id):
+        data = {'avatar_id': avatar_id}
+        url = self.URL_AUSER_UPDATE_GROUP_AVATAR.format(conversation_id)
+        return "POST", url, None, data
+
+    @return_with_headers
     def send_message(self, conversation_id, text, media_id=None):
         params = {
             'ext': 'mediaColor,altText,mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl',
             'include_ext_alt_text': True,
             'include_ext_limited_action_results': True,
             'include_reply_count': '1',
             'tweet_mode': 'extended',
```

### Comparing `tweety_ns-1.1.4b0/src/tweety/events/newmessage.py` & `tweety_ns-1.1.5/src/tweety/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/exceptions_.py` & `tweety_ns-1.1.5/src/tweety/exceptions_.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/filters.py` & `tweety_ns-1.1.5/src/tweety/filters.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/http.py` & `tweety_ns-1.1.5/src/tweety/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,31 @@
         response = self.__get_response__(**self.__builder.get_untrusted_inbox(max_id, low_quality))
         return response
 
     def get_conversation(self, conversation_id, max_id=None):
         response = self.__get_response__(**self.__builder.get_conversation_with_messages(conversation_id, max_id))
         return response
 
+    def create_conversation_group(self, participants, first_message):
+        request_data = self.__builder.create_group(participants, first_message)
+        response = self.__get_response__(**request_data)
+        return response
+
+    def update_conversation_name(self, conversation_id, name):
+        request_data = self.__builder.update_conversation_group_name(conversation_id, name)
+        request_data['headers']['Content-Type'] = f"application/x-www-form-urlencoded"
+        response = self.__get_response__(ignore_none_data=True, **request_data)
+        return response
+
+    def update_conversation_avatar(self, conversation_id, avatar_id):
+        request_data = self.__builder.update_conversation_group_avatar(conversation_id, avatar_id)
+        request_data['headers']['Content-Type'] = f"application/x-www-form-urlencoded"
+        response = self.__get_response__(ignore_none_data=True, **request_data)
+        return response
+
     def send_message(self, conversation_id, text, media_id):
         request_data = self.__builder.send_message(conversation_id, text, media_id)
         response = self.__get_response__(**request_data)
         return response
 
     def create_pool(self, pool):
         request_data = self.__builder.create_pool(pool)
```

### Comparing `tweety_ns-1.1.4b0/src/tweety/session.py` & `tweety_ns-1.1.5/src/tweety/session.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/__init__.py` & `tweety_ns-1.1.5/src/tweety/types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,26 @@
     AudioSpace,
     Gif,
     Topic,
     TweetTranslate,
     TweetAnalytics,
     Place
 )
-from .n_types import UploadedMedia, Proxy, PROXY_TYPE_SOCKS4, PROXY_TYPE_SOCKS5, PROXY_TYPE_HTTP, HOME_TIMELINE_TYPE_FOLLOWING, HOME_TIMELINE_TYPE_FOR_YOU
+from .n_types import (
+    UploadedMedia,
+    Proxy,
+    PROXY_TYPE_SOCKS4,
+    PROXY_TYPE_SOCKS5,
+    PROXY_TYPE_HTTP,
+    HOME_TIMELINE_TYPE_FOLLOWING,
+    HOME_TIMELINE_TYPE_FOR_YOU,
+    INBOX_PAGE_TYPES,
+    INBOX_PAGE_TYPE_TRUSTED,
+    INBOX_PAGE_TYPE_UNTRUSTED
+)
 from .search import Search, TypeHeadSearch
 from .usertweet import UserTweets, SelfTimeline, TweetComments, TweetHistory, UserMedia, UserHighlights, UserLikes
 from .mentions import Mention
 from .inbox import Inbox, SendMessage, Media, Conversation
 from .bookmarks import Bookmarks
 from .likes import TweetLikes
 from .retweets import TweetRetweets
```

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/base.py` & `tweety_ns-1.1.5/src/tweety/types/base.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/bookmarks.py` & `tweety_ns-1.1.5/src/tweety/types/bookmarks.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/community.py` & `tweety_ns-1.1.5/src/tweety/types/community.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/follow.py` & `tweety_ns-1.1.5/src/tweety/types/follow.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/gifs.py` & `tweety_ns-1.1.5/src/tweety/types/gifs.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/inbox.py` & `tweety_ns-1.1.5/src/tweety/types/inbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import re
 import threading
 import time
-import traceback
-from . import User, Media, URL, Hashtag, ShortUser, Symbol
-from ..utils import parse_time, parse_wait_time
+import warnings
+from . import User, Media, URL, Hashtag, ShortUser, Symbol, INBOX_PAGE_TYPES, INBOX_PAGE_TYPE_UNTRUSTED, INBOX_PAGE_TYPE_TRUSTED
+from ..utils import parse_time, parse_wait_time, get_next_index
+from ..exceptions_ import TwitterError
 
 
 class Inbox(dict):
     HAS_MORE_STATUS = "HAS_MORE"
     AT_END_STATUS = "AT_END"
 
-    def __init__(self, user_id, client, pages, wait_time=2):
+    def __init__(self, user_id, client, pages, wait_time=2, page_types=INBOX_PAGE_TYPES):
+        _page_types = [page_types] if not isinstance(page_types, list) else page_types
         super().__init__()
         self._client = client
         self._got_initial = False
         self._inbox_timelines = {}
+        self._retries = 2
+        self._types = [i for i in _page_types if i in INBOX_PAGE_TYPES]
         self.pages = pages
         self.wait_time = wait_time
         self.conversations = []
         self.messages = []
         self.cursor = None
         self.last_seen_event_id = None
         self.trusted_last_seen_event_id = None
@@ -45,15 +49,15 @@
                 self.conversations.insert(to_edit, _conversation)
             else:
                 self.conversations.append(_conversation)
 
         self._parse_messages(this_page)
         return this_page, _initial_inbox
 
-    def get_page(self, min_entry_id=None, page_type="trusted"):
+    def get_page(self, min_entry_id=None, page_type=INBOX_PAGE_TYPE_TRUSTED):
         if not self._got_initial:
             if not self.cursor:
                 response = self._client.http.get_initial_inbox()
             else:
                 response = self._client.http.get_inbox_updates(cursor=self.cursor)
 
             page, inbox = self._parse_response(response)
@@ -64,26 +68,35 @@
 
             if inbox.get("inbox_timelines"):
                 self._inbox_timelines = inbox.get("inbox_timelines", {})
 
             self._got_initial = True
             return page, self.cursor, None
         else:
-            if page_type not in ("trusted", "untrusted"):
-                page_type = "trusted"
+            if page_type not in INBOX_PAGE_TYPES:
+                page_type = INBOX_PAGE_TYPE_TRUSTED
 
             if not min_entry_id:
                 raise ValueError("'min_entry_id' is required after initial request.")
 
-            if page_type == "untrusted":
-                response = self._client.http.get_untrusted_inbox(min_entry_id)
-            else:
-                response = self._client.http.get_trusted_inbox(min_entry_id)
+            response = None
 
-            page, inbox = self._parse_response(response)
+            for _ in range(self._retries):
+                try:
+                    if page_type == INBOX_PAGE_TYPE_UNTRUSTED:
+                        response = self._client.http.get_untrusted_inbox(min_entry_id)
+                    else:
+                        response = self._client.http.get_trusted_inbox(min_entry_id)
+                except TwitterError as inbox_fetch_error:
+                    pass
+
+            if response:
+                page, inbox = self._parse_response(response)
+            else:
+                page, inbox = [], {}
 
             return page, inbox.get('min_entry_id', 0), inbox.get('status', self.AT_END_STATUS)
 
     def get_new_messages(self, cursor=None):
         if not cursor:
             cursor = self.cursor
 
@@ -95,48 +108,58 @@
         self.untrusted_last_seen_event_id = self['untrusted_last_seen_event_id'] = inbox.get('untrusted_last_seen_event_id')
 
         if inbox.get("inbox_timelines"):
             self._inbox_timelines = inbox.get("inbox_timelines", {})
 
         return page
 
-    def get_next_page(self):
+    def get_next_page(self, page_type=None):
         if not self._got_initial:
             page, cursor, _ = self.get_page()
             self.cursor = self['cursor'] = cursor
             return page
         else:
-            page_type = "trusted"
+            if not page_type or page_type not in INBOX_PAGE_TYPES:
+                page_type = INBOX_PAGE_TYPE_TRUSTED
 
             if self._inbox_timelines[page_type]['status'] == self.AT_END_STATUS:
-                page_type = "untrusted"
+                page_type = INBOX_PAGE_TYPE_UNTRUSTED
 
             page_attrs = self._inbox_timelines.get(page_type, {})
+
             min_entry_id = page_attrs.get('min_entry_id', 0)
             status = page_attrs.get('status', self.AT_END_STATUS)
 
             if status == self.AT_END_STATUS:
                 return []
 
             page, new_min_entry_id, new_status = self.get_page(min_entry_id=min_entry_id, page_type=page_type)
             self._inbox_timelines[page_type]["min_entry_id"] = new_min_entry_id
             self._inbox_timelines[page_type]["status"] = new_status
             return page
 
     def generator(self):
         this_page = 0
+        page_type_index = 0
+        page_type = self._types[page_type_index]
+
         while this_page != int(self.pages):
-            results = self.get_next_page()
+            results = self.get_next_page(page_type)
 
             if len(results) == 0:
-                break
+                page_type_index = get_next_index(self._types, page_type_index)
 
-            yield self, results
+                if not page_type_index:
+                    break
 
+                page_type = self._types[page_type_index]
+
+            yield self, results
             this_page += 1
+
             if this_page != self.pages:
                 time.sleep(parse_wait_time(self.wait_time))
 
         return self
 
     def _parse_messages(self, conversations):
         for conv in conversations:
@@ -186,14 +209,17 @@
         self.last_read_event_id = self['last_read_event_id'] = self._get_key("last_read_event_id")
         self.low_quality = self['low_quality'] = self._get_key("low_quality")
         self.max_entry_id = self['max_entry_id'] = self._get_key("max_entry_id")
         self.min_entry_id = self['min_entry_id'] = self._get_key("min_entry_id")
         self.muted = self['muted'] = self._get_key("muted")
         self.notifications_disabled = self['notifications_disabled'] = self._get_key("notifications_disabled")
         self.nsfw = self['nsfw'] = self._get_key("nsfw")
+        self.avatar_url = self['avatar_image_https'] = self._get_key("avatar_image_https")  # only for Group
+        self.created_at = self['create_time'] = parse_time(self._get_key("create_time"))  # only for Group
+        self.created_by_user_id = self['created_by_user_id'] = self._get_key("created_by_user_id")  # only for Group
         self.read_only = self['read_only'] = self._get_key("read_only")
         self.trusted = self['trusted'] = self._get_key("trusted")
         self.type = self['type'] = self._get_key("type")
         self.participants = self['participants'] = self.get_participants()
         self.name = self['name'] = self._get_key("name", self._get_one_to_one_name())
         self.messages = self['messages'] = self.parse_messages()
         self.is_group = self.type == self.TYPE_GROUP_DM
@@ -258,14 +284,16 @@
                 self._inbox,
                 self._client
             )
         elif entry.get('conversation_name_update') and str(entry['conversation_name_update']['conversation_id']) == str(self.id):
             return MessageNameUpdate(entry['conversation_name_update'], self._inbox, self._client)
         elif entry.get('conversation_create') and str(entry['conversation_create']['conversation_id']) == str(self.id):
             return MessageConversationCreated(entry['conversation_create'], self._inbox, self._client)
+        elif entry.get('conversation_avatar_update') and str(entry['conversation_avatar_update']['conversation_id']) == str(self.id):
+            return MessageConversationAvatarUpdate(entry["conversation_avatar_update"], self._inbox, self._client)
 
         return None
 
     def parse_messages(self):
         messages = []
         if not self._get_all_messages:
             for entry in self._inbox.get('entries', []):
@@ -428,14 +456,32 @@
 
     def __repr__(self):
         return "MessageConversationCreated(id={}, time={})".format(
             self.id, self.time
         )
 
 
+class MessageConversationAvatarUpdate(dict):
+    def __init__(self, update, _inbox, client):
+        super().__init__()
+        self._raw = update
+        self._inbox = _inbox
+        self._client = client
+        self.by_user_id = self["by_user_id"] = self._raw.get("by_user_id")
+        self.id = self['id'] = self._raw['id']
+        self.time = self['time'] = parse_time(self._raw.get('time'))
+        self.conversation_id = self["conversation_id"] = self._raw.get("conversation_id")
+        self.avatar_url = self["avatar_url"] = self._raw.get("conversation_avatar_image_https")
+
+    def __repr__(self):
+        return "MessageConversationAvatarUpdate(id={}, by_user_id={})".format(
+            self.id, self.by_user_id
+        )
+
+
 class Message(dict):
     def __init__(self, message, _inbox, client):
         super().__init__()
         self._raw = message
         self._inbox = _inbox
         self._client = client
         self._entities = self._get_message_data('entities', {})
```

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/likes.py` & `tweety_ns-1.1.5/src/tweety/types/likes.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/lists.py` & `tweety_ns-1.1.5/src/tweety/types/lists.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/mentions.py` & `tweety_ns-1.1.5/src/tweety/types/mentions.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/n_types.py` & `tweety_ns-1.1.5/src/tweety/types/n_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from ..exceptions_ import *
 
 PROXY_TYPE_SOCKS4 = SOCKS4 = 1
 PROXY_TYPE_SOCKS5 = SOCKS5 = 2
 PROXY_TYPE_HTTP = HTTP = 3
 HOME_TIMELINE_TYPE_FOR_YOU = "HomeTimeline"
 HOME_TIMELINE_TYPE_FOLLOWING = "HomeLatestTimeline"
+INBOX_PAGE_TYPE_TRUSTED = "trusted"
+INBOX_PAGE_TYPE_UNTRUSTED = "untrusted"
+INBOX_PAGE_TYPES = (INBOX_PAGE_TYPE_TRUSTED, INBOX_PAGE_TYPE_UNTRUSTED)
 
 
 class Proxy:
     def __init__(self, host: str, port: int, proxy_type: int, username: str = None, password: str = None):
         self.host = host
         self.password = password
         self.proxy_type = proxy_type
```

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/notification.py` & `tweety_ns-1.1.5/src/tweety/types/notification.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/places.py` & `tweety_ns-1.1.5/src/tweety/types/places.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/retweets.py` & `tweety_ns-1.1.5/src/tweety/types/retweets.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/search.py` & `tweety_ns-1.1.5/src/tweety/types/search.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/topic.py` & `tweety_ns-1.1.5/src/tweety/types/topic.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/twDataTypes.py` & `tweety_ns-1.1.5/src/tweety/types/twDataTypes.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/types/usertweet.py` & `tweety_ns-1.1.5/src/tweety/types/usertweet.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.4b0/src/tweety/user.py` & `tweety_ns-1.1.5/src/tweety/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union, Tuple, List
 from .exceptions_ import ListNotFound
 from .types.inbox import Message, Conversation
 from .utils import create_conversation_id, AuthRequired, find_objects, get_tweet_id
 from .types import (User, Mention, Inbox, UploadedMedia, SendMessage, Tweet, Bookmarks, SelfTimeline, TweetLikes,
                     TweetRetweets, Poll, Choice, TweetNotifications, Lists, List as TwList, ListMembers, ListTweets,
                     Topic, TopicTweets, MutualFollowers, HOME_TIMELINE_TYPE_FOR_YOU, TweetAnalytics, BlockedUsers,
-                    ShortUser, Place)
+                    ShortUser, Place, INBOX_PAGE_TYPE_TRUSTED)
 from .filters import SearchFilters
 
 
 @AuthRequired
 class UserMethods:
 
     @property
@@ -331,40 +331,44 @@
         return notifications.generator()
 
     def get_inbox(
             self,
             user_id: Union[int, str, User] = None,
             pages: int = 1,
             wait_time: Union[int, list, tuple] = 2,
+            page_types: Union[str, List[str]] = INBOX_PAGE_TYPE_TRUSTED
     ) -> Inbox:
         """
         :param user_id : (`str`, `int`, `User`) Not Implemented
         :param pages: (`int`) The number of pages to get
         :param wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param page_types: list[`str`] Which Type of Conversation to Get | INBOX_PAGE_TYPE_TRUSTED, INBOX_PAGE_TYPE_UNTRUSTED
         :return:
         """
 
-        inbox = Inbox(self.user.id, self, pages, wait_time)
+        inbox = Inbox(self.user.id, self, pages, wait_time, page_types)
         list(inbox.generator())
         return inbox
 
     def iter_inbox(
             self,
             user_id: Union[int, str, User] = None,
             pages: int = 1,
             wait_time: Union[int, list, tuple] = 2,
+            page_types: Union[str, List[str]] = INBOX_PAGE_TYPE_TRUSTED
     ) -> Inbox:
         """
         :param user_id : (`str`, `int`, `User`) Not Implemented
         :param pages: (`int`) The number of pages to get
         :param wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param page_types: list[`str`] Which Type of Conversation to Get | INBOX_PAGE_TYPE_TRUSTED, INBOX_PAGE_TYPE_UNTRUSTED
         :return:
         """
 
-        inbox = Inbox(self.user.id, self, pages, wait_time)
+        inbox = Inbox(self.user.id, self, pages, wait_time, page_types)
         return inbox.generator()
 
     def add_member_to_group(
             self,
             members: Union[str, int, list],
             group_id: Union[str, int, Conversation]
     ):
@@ -377,14 +381,88 @@
             else:
                 member_ids.append(member)
 
         group_id = group_id.id if isinstance(group_id, Conversation) else group_id
 
         return self.request.add_group_member(member_ids, group_id)
 
+    def create_conversation_group(
+            self,
+            participants: List[Union[str, int, User, ShortUser]],
+            first_message: str,
+            name: str = None
+    ):
+        """
+        Create a Conversation Group
+
+        :param participants: IDs of all the participants you want to add
+        :param first_message: First message you want to in the group (Yes it is Required)
+        :param name: Name of the group you want to set
+        :return: .types.inbox.Conversation
+        """
+
+        participants_id = []
+        for participant in participants:
+            try:
+                user_id = self._get_user_id(participant)
+                participants_id.append(str(user_id))
+            except:
+                pass
+
+        participants_id = ",".join(participants_id)
+        response = self.request.create_conversation_group(participants_id, first_message)
+        new_conversation = list(response["conversations"].values())[0]
+        conversation = Conversation(new_conversation, response, self)
+
+        if name:
+            self.update_conversation_group_name(conversation, name)
+            conversation.name = name
+
+        return conversation
+
+    def update_conversation_group_name(
+            self,
+            conversation_id: Union[str, int, Conversation],
+            name: str
+    ):
+        """
+        Update the name of Conversation Group
+
+        :param conversation_id: ID of the Group
+        :param name: New Name of the Group
+        :return:
+        """
+
+        if isinstance(conversation_id, Conversation):
+            conversation_id = conversation_id.id
+
+        self.request.update_conversation_name(conversation_id, name)
+        return True
+
+    def update_conversation_group_avatar(
+            self,
+            conversation_id: Union[str, int, Conversation],
+            file: Union[str, UploadedMedia]
+    ):
+        """
+        Update the Avatar/Profile Image of Conversation Group
+
+        :param conversation_id: ID of the Group
+        :param file: New Name of the Group
+        :return:
+        """
+
+        if isinstance(conversation_id, Conversation):
+            conversation_id = conversation_id.id
+
+        file = self._upload_media(file)[0].media_id
+
+        self.request.update_conversation_avatar(conversation_id, file)
+        return True
+
     def send_message(
             self,
             username: Union[str, int, User],
             text: str,
             file: Union[str, UploadedMedia] = None,
             in_group: bool = False  # TODO : Find better way
     ) -> Message:
@@ -424,15 +502,15 @@
             pool: dict = None,
             place: Union[str, Place] = None
     ) -> Tweet:
 
         """
         Create a Tweet
 
-        :param pool: Pool you want to include in the tweet
+        :param pool: (`dict`) Pool you want to include in the tweet
         :param text: (`str`) Text content of Tweet
         :param files: (`list[Union[str, UploadedMedia, tuple[str, str]]]`) Files to be sent with Tweet (max 4)
         :param filter_: (`str`) Filter to applied for Tweet audience
         :param reply_to: (`str` | `int` | `Tweet`) ID of tweet to reply to
         :param quote: (`str` | `int` | `Tweet`) ID / URL of tweet to be quoted
         :param place: (`str` `Place`) ID of location you want to add
         :return: Tweet
```

### Comparing `tweety_ns-1.1.4b0/src/tweety/utils.py` & `tweety_ns-1.1.5/src/tweety/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import inspect
 import json
 import os.path
 import random
 import re
 import string
 import sys
-import traceback
 import uuid
 from dateutil import parser as date_parser
 from urllib.parse import urlparse
 from .exceptions_ import AuthenticationRequired
 from .filters import Language
 
 GUEST_TOKEN_REGEX = re.compile("gt=(.*?);")
@@ -73,14 +72,21 @@
 
     if isinstance(wait_time, (tuple, list)):
         return random.randint(*wait_time)
 
     return int(wait_time)
 
 
+def get_next_index(iterable, current_index, __default__=None):
+    try:
+        _ = iterable[current_index + 1]
+        return current_index + 1
+    except IndexError:
+        return __default__
+
 def custom_json(self, **kwargs):
     try:
         return json.loads(self.content, **kwargs)
     except:
         return None
```

### Comparing `tweety_ns-1.1.4b0/src/tweety_ns.egg-info/PKG-INFO` & `tweety_ns-1.1.5/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.4b0
+Version: 1.1.5
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety_ns-1.1.4b0/src/tweety_ns.egg-info/SOURCES.txt` & `tweety_ns-1.1.5/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

