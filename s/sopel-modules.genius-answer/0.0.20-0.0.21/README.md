# Comparing `tmp/sopel_modules_genius_answer-0.0.20.tar.gz` & `tmp/sopel_modules_genius_answer-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules_genius_answer-0.0.20.tar", last modified: Sat Apr 27 15:13:34 2024, max compression
+gzip compressed data, was "sopel_modules_genius_answer-0.0.21.tar", last modified: Sun Apr 28 16:47:14 2024, max compression
```

## Comparing `sopel_modules_genius_answer-0.0.20.tar` & `sopel_modules_genius_answer-0.0.21.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-27 15:13:34.831294 sopel_modules_genius_answer-0.0.20/
--rw-rw-r--   0 user      (1000) user      (1000)      702 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.20/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      135 2024-04-26 17:11:45.000000 sopel_modules_genius_answer-0.0.20/NOTE.md
--rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-27 15:13:34.830294 sopel_modules_genius_answer-0.0.20/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      736 2024-04-26 16:54:45.000000 sopel_modules_genius_answer-0.0.20/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      674 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.20/TODO
--rw-rw-r--   0 user      (1000) user      (1000)      642 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.20/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-27 15:13:34.831294 sopel_modules_genius_answer-0.0.20/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-27 15:13:34.829294 sopel_modules_genius_answer-0.0.20/sopel_modules/
--rw-rw-r--   0 user      (1000) user      (1000)       56 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.20/sopel_modules/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-27 15:13:34.830294 sopel_modules_genius_answer-0.0.20/sopel_modules/genius-answer/
--rw-rw-r--   0 user      (1000) user      (1000)     5137 2024-04-27 15:13:07.000000 sopel_modules_genius_answer-0.0.20/sopel_modules/genius-answer/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-27 15:13:34.830294 sopel_modules_genius_answer-0.0.20/sopel_modules.genius_answer.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-27 15:13:34.000000 sopel_modules_genius_answer-0.0.20/sopel_modules.genius_answer.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      368 2024-04-27 15:13:34.000000 sopel_modules_genius_answer-0.0.20/sopel_modules.genius_answer.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-27 15:13:34.000000 sopel_modules_genius_answer-0.0.20/sopel_modules.genius_answer.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-27 15:13:34.000000 sopel_modules_genius_answer-0.0.20/sopel_modules.genius_answer.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-27 15:13:34.000000 sopel_modules_genius_answer-0.0.20/sopel_modules.genius_answer.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 16:47:14.771087 sopel_modules_genius_answer-0.0.21/
+-rw-rw-r--   0 user      (1000) user      (1000)      702 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.21/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      135 2024-04-26 17:11:45.000000 sopel_modules_genius_answer-0.0.21/NOTE.md
+-rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-28 16:47:14.771087 sopel_modules_genius_answer-0.0.21/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      736 2024-04-26 16:54:45.000000 sopel_modules_genius_answer-0.0.21/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      674 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.21/TODO
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.21/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-28 16:47:14.771087 sopel_modules_genius_answer-0.0.21/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 16:47:14.770087 sopel_modules_genius_answer-0.0.21/sopel_modules/
+-rw-rw-r--   0 user      (1000) user      (1000)       56 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.21/sopel_modules/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 16:47:14.770087 sopel_modules_genius_answer-0.0.21/sopel_modules/genius-answer/
+-rw-rw-r--   0 user      (1000) user      (1000)     5102 2024-04-28 16:45:34.000000 sopel_modules_genius_answer-0.0.21/sopel_modules/genius-answer/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 16:47:14.770087 sopel_modules_genius_answer-0.0.21/sopel_modules.genius_answer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1144 2024-04-28 16:47:14.000000 sopel_modules_genius_answer-0.0.21/sopel_modules.genius_answer.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      368 2024-04-28 16:47:14.000000 sopel_modules_genius_answer-0.0.21/sopel_modules.genius_answer.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 16:47:14.000000 sopel_modules_genius_answer-0.0.21/sopel_modules.genius_answer.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-28 16:47:14.000000 sopel_modules_genius_answer-0.0.21/sopel_modules.genius_answer.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-28 16:47:14.000000 sopel_modules_genius_answer-0.0.21/sopel_modules.genius_answer.egg-info/top_level.txt
```

### Comparing `sopel_modules_genius_answer-0.0.20/.gitignore` & `sopel_modules_genius_answer-0.0.21/.gitignore`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.20/PKG-INFO` & `sopel_modules_genius_answer-0.0.21/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.genius-answer
-Version: 0.0.20
+Version: 0.0.21
 Summary: A sopel plugin (irc-bot) to answer with a quote from rapgenius.com 
 Author-email: eoli3n <eoli3n@runbox.com>
 License: WTFPL
 Project-URL: Source code, https://github.com/eoli3n/sopel-genius-answer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sopel<8,>=7.1
```

### Comparing `sopel_modules_genius_answer-0.0.20/README.md` & `sopel_modules_genius_answer-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.20/TODO` & `sopel_modules_genius_answer-0.0.21/TODO`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.20/pyproject.toml` & `sopel_modules_genius_answer-0.0.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sopel_modules_genius_answer-0.0.20/sopel_modules/genius-answer/__init__.py` & `sopel_modules_genius_answer-0.0.21/sopel_modules/genius-answer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             answer = search_line_by_song(result['song_id'])
 
         return answer
 
     except:
         return False
 
-@plugin.rule(r'(.*\b)($nickname)[ :,](.*)')
+@plugin.rule(r'$nick (.*)')
 
 def sentence_responder(bot, trigger):
 
     # configure fallback
     global fallback
     if bot.config.fallback.default:
         fallback = bot.config.fallback.default
@@ -139,15 +139,15 @@
             bot.memory["last_nick_count"] += 1
 
         if getattr(bot.config.limitation, trigger.nick):
             if bot.memory["last_nick_count"] > int(getattr(bot.config.limitation, trigger.nick)):
                 LOGGER.info(trigger.nick + " is now blocked")
                 return
 
-    message = trigger.group(1) + trigger.group(3)
+    message = trigger.group(1)
     response = genius_bot_answer(message)
 
     if not trigger.sender.is_nick():
         channel = bot.channels[trigger.sender].name.replace('#','')
         if getattr(bot.config.fallback, channel):
             fallback = getattr(bot.config.fallback, channel)
     # answer
```

### Comparing `sopel_modules_genius_answer-0.0.20/sopel_modules.genius_answer.egg-info/PKG-INFO` & `sopel_modules_genius_answer-0.0.21/sopel_modules.genius_answer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.genius-answer
-Version: 0.0.20
+Version: 0.0.21
 Summary: A sopel plugin (irc-bot) to answer with a quote from rapgenius.com 
 Author-email: eoli3n <eoli3n@runbox.com>
 License: WTFPL
 Project-URL: Source code, https://github.com/eoli3n/sopel-genius-answer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sopel<8,>=7.1
```

