# Comparing `tmp/tebbytools-0.2.4.tar.gz` & `tmp/tebbytools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tebbytools-0.2.4.tar", last modified: Thu Apr 18 15:27:36 2024, max compression
+gzip compressed data, was "tebbytools-0.3.1.tar", last modified: Sat Apr 27 22:31:16 2024, max compression
```

## Comparing `tebbytools-0.2.4.tar` & `tebbytools-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.768087 tebbytools-0.2.4/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-18 15:27:36.767719 tebbytools-0.2.4/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)     1921 2024-04-17 03:26:55.000000 tebbytools-0.2.4/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-18 15:27:36.768144 tebbytools-0.2.4/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-04-18 15:27:30.000000 tebbytools-0.2.4/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.765371 tebbytools-0.2.4/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.766540 tebbytools-0.2.4/src/tebbytools/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       66 2024-04-17 03:25:44.000000 tebbytools-0.2.4/src/tebbytools/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.2.4/src/tebbytools/reviewlist.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     5194 2024-04-18 15:25:49.000000 tebbytools-0.2.4/src/tebbytools/wordbank.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.767487 tebbytools-0.2.4/src/tebbytools.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-18 15:27:36.000000 tebbytools-0.2.4/src/tebbytools.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      267 2024-04-18 15:27:36.000000 tebbytools-0.2.4/src/tebbytools.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-18 15:27:36.000000 tebbytools-0.2.4/src/tebbytools.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-04-18 15:27:36.000000 tebbytools-0.2.4/src/tebbytools.egg-info/top_level.txt
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.767205 tebbytools-0.2.4/tests/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      906 2024-04-17 03:25:59.000000 tebbytools-0.2.4/tests/test.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.323503 tebbytools-0.3.1/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-27 22:31:16.323280 tebbytools-0.3.1/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2783 2024-04-27 22:29:15.000000 tebbytools-0.3.1/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-27 22:31:16.323576 tebbytools-0.3.1/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-04-27 22:31:11.000000 tebbytools-0.3.1/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.320954 tebbytools-0.3.1/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.321678 tebbytools-0.3.1/src/tebbytools/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       99 2024-04-27 22:29:15.000000 tebbytools-0.3.1/src/tebbytools/__init__.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.322835 tebbytools-0.3.1/src/tebbytools/quickquiz/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       33 2024-04-27 22:29:15.000000 tebbytools-0.3.1/src/tebbytools/quickquiz/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2319 2024-04-27 22:29:15.000000 tebbytools-0.3.1/src/tebbytools/quickquiz/quickquiz.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     1912 2024-04-27 22:29:15.000000 tebbytools-0.3.1/src/tebbytools/quickquiz/quiz.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.3.1/src/tebbytools/reviewlist.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     5194 2024-04-18 15:25:49.000000 tebbytools-0.3.1/src/tebbytools/wordbank.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.323024 tebbytools-0.3.1/src/tebbytools.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-27 22:31:16.000000 tebbytools-0.3.1/src/tebbytools.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      361 2024-04-27 22:31:16.000000 tebbytools-0.3.1/src/tebbytools.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-27 22:31:16.000000 tebbytools-0.3.1/src/tebbytools.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-04-27 22:31:16.000000 tebbytools-0.3.1/src/tebbytools.egg-info/top_level.txt
```

### Comparing `tebbytools-0.2.4/README.md` & `tebbytools-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```python
 from tebbytools import WordBank
 
 # Initialize a WordBank instance
 wb = WordBank(file_path="path/to/your/word_bank.json")
 
 # Set a new file path
-wb.set_file_path("~/new_path/word_bank.json")
+wb.set_file_path("new/path/to/your/word_bank.json")
 
 # Add a word to the bank with optional tags
 wb.add_word("hello", tags=["greeting", "basic"])
 
 # Get all words in the bank
 words = wb.get_all_words()
 
@@ -59,21 +59,43 @@
 ```python
 from tebbytools import ReviewList
 
 # Initialize a ReviewList instance
 rl = ReviewList(file_path="path/to/your/review_list.txt", size=5)
 
 # Set a new file path
-rl.set_file_path("~/new_path/review_list.txt")
+rl.set_file_path("new/path/to/your/review_list.txt")
 
 # Add a new word
 rl.add_word("hello")
 
 # Check if the review list is full
 is_full = rl.is_full()
 
 # Get the review list
 review_list = rl.get_list()
 
 # Clear the review list
 rl.clear_list()
 ```
+
+### Quick Quiz
+
+A `QuickQuiz` is a simple quiz application that runs a local web server.
+You can input your terms in a text box after starting the quiz, or include a list of terms as an argument to the `start()` method.
+By default, the server will run on port 5000, but you can modify this behavior by setting the port argument in the `start()` method.\
+
+The `QuickQuiz` is designed to be used with the `ReviewList`. Once the review list is full, quickly quiz yourself on its contents.
+
+```python
+from tebbytools import ReviewList, QuickQuiz
+
+# Initialize a ReviewList instance
+rl = ReviewList(file_path="path/to/your/review_list.txt", size=5)
+
+# Check if the review list is full
+if rl.is_full():
+    # Initialize a QuickQuiz instance
+    qq = QuickQuiz()
+    # Start the server with a list of terms
+    qq.start(terms=rl.get_list(), port=1234)
+```
```

### Comparing `tebbytools-0.2.4/src/tebbytools/reviewlist.py` & `tebbytools-0.3.1/src/tebbytools/reviewlist.py`

 * *Files identical despite different names*

### Comparing `tebbytools-0.2.4/src/tebbytools/wordbank.py` & `tebbytools-0.3.1/src/tebbytools/wordbank.py`

 * *Files identical despite different names*

