# Comparing `tmp/voice2text_deltabot-1.3.0-py3-none-any.whl.zip` & `tmp/voice2text_deltabot-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 17482 bytes, number of entries: 10
--rw-r--r--  2.0 unx      189 b- defN 24-Apr-28 00:58 voice2text_deltabot/__init__.py
--rw-r--r--  2.0 unx       90 b- defN 24-Apr-28 00:58 voice2text_deltabot/__main__.py
--rw-r--r--  2.0 unx      411 b- defN 24-Apr-28 00:59 voice2text_deltabot/_version.py
--rw-r--r--  2.0 unx     4650 b- defN 24-Apr-28 00:58 voice2text_deltabot/hooks.py
--rw-r--r--  2.0 unx    35141 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2047 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      903 b- defN 24-Apr-28 00:59 voice2text_deltabot-1.3.0.dist-info/RECORD
-10 files, 43603 bytes uncompressed, 15908 bytes compressed:  63.5%
+Zip file size: 17459 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      189 b- defN 24-Apr-28 14:21 voice2text_deltabot/__init__.py
+-rw-r--r--  2.0 unx       90 b- defN 24-Apr-28 14:21 voice2text_deltabot/__main__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-28 14:21 voice2text_deltabot/_version.py
+-rw-r--r--  2.0 unx     4555 b- defN 24-Apr-28 14:21 voice2text_deltabot/hooks.py
+-rw-r--r--  2.0 unx    35141 b- defN 24-Apr-28 14:21 voice2text_deltabot-1.3.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2047 b- defN 24-Apr-28 14:21 voice2text_deltabot-1.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 14:21 voice2text_deltabot-1.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 24-Apr-28 14:21 voice2text_deltabot-1.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-28 14:21 voice2text_deltabot-1.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      903 b- defN 24-Apr-28 14:21 voice2text_deltabot-1.3.1.dist-info/RECORD
+10 files, 43508 bytes uncompressed, 15885 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: voice2text_deltabot/_version.py
 Comment: 
 
 Filename: voice2text_deltabot/hooks.py
 Comment: 
 
-Filename: voice2text_deltabot-1.3.0.dist-info/LICENSE.txt
+Filename: voice2text_deltabot-1.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: voice2text_deltabot-1.3.0.dist-info/METADATA
+Filename: voice2text_deltabot-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: voice2text_deltabot-1.3.0.dist-info/WHEEL
+Filename: voice2text_deltabot-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: voice2text_deltabot-1.3.0.dist-info/entry_points.txt
+Filename: voice2text_deltabot-1.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: voice2text_deltabot-1.3.0.dist-info/top_level.txt
+Filename: voice2text_deltabot-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: voice2text_deltabot-1.3.0.dist-info/RECORD
+Filename: voice2text_deltabot-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## voice2text_deltabot/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '1.3.0'
-__version_tuple__ = version_tuple = (1, 3, 0)
+__version__ = version = '1.3.1'
+__version_tuple__ = version_tuple = (1, 3, 1)
```

## voice2text_deltabot/hooks.py

```diff
@@ -102,19 +102,15 @@
             return
 
     if msg.view_type in (MessageViewtype.VOICE, MessageViewtype.AUDIO):
         start = time.time()
         segments, info = MODEL.transcribe(msg.file)
         lines = []
         for seg in segments:
-            if (
-                seg.avg_logprob < -0.7
-                or seg.no_speech_prob > 0.5
-                or seg.compression_ratio < 0.9
-            ):
+            if seg.avg_logprob < -0.7 or seg.no_speech_prob > 0.5:
                 continue
             text = seg.text.strip()
             if text.strip("."):
                 lines.append(text)
         took = time.time() - start
         percent = int(info.language_probability * 100)
         bot.logger.info(
```

## Comparing `voice2text_deltabot-1.3.0.dist-info/LICENSE.txt` & `voice2text_deltabot-1.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `voice2text_deltabot-1.3.0.dist-info/METADATA` & `voice2text_deltabot-1.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voice2text-deltabot
-Version: 1.3.0
+Version: 1.3.1
 Summary: Delta Chat bot to extract text from voice messages
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/voice2text_deltabot
 Keywords: deltachat,bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

