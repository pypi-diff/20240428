# Comparing `tmp/sessionless-0.0.3.tar.gz` & `tmp/sessionless-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessionless-0.0.3.tar", last modified: Sat Apr 13 19:16:45 2024, max compression
+gzip compressed data, was "sessionless-0.0.4.tar", last modified: Sun Apr 28 14:24:15 2024, max compression
```

## Comparing `sessionless-0.0.3.tar` & `sessionless-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-13 19:16:45.553071 sessionless-0.0.3/
--rw-r--r--   0 habsoomane   (501) staff       (20)     3581 2024-04-13 19:16:45.551816 sessionless-0.0.3/PKG-INFO
--rw-r--r--   0 habsoomane   (501) staff       (20)     2973 2024-04-12 23:12:13.000000 sessionless-0.0.3/README.md
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-13 19:16:45.544859 sessionless-0.0.3/sessionless/
--rw-r--r--   0 habsoomane   (501) staff       (20)       59 2024-04-12 22:02:34.000000 sessionless-0.0.3/sessionless/__init__.py
--rw-r--r--   0 habsoomane   (501) staff       (20)     2598 2024-04-12 23:14:33.000000 sessionless-0.0.3/sessionless/modelsecp256k1.py
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-13 19:16:45.550673 sessionless-0.0.3/sessionless.egg-info/
--rw-r--r--   0 habsoomane   (501) staff       (20)     3581 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/PKG-INFO
--rw-r--r--   0 habsoomane   (501) staff       (20)      294 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/SOURCES.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)        1 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/dependency_links.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       15 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/requires.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       18 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/top_level.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       38 2024-04-13 19:16:45.553370 sessionless-0.0.3/setup.cfg
--rw-r--r--   0 habsoomane   (501) staff       (20)     1126 2024-04-13 19:16:30.000000 sessionless-0.0.3/setup.py
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-13 19:16:45.549566 sessionless-0.0.3/tests/
--rw-r--r--   0 habsoomane   (501) staff       (20)       63 2024-04-12 22:08:56.000000 sessionless-0.0.3/tests/__init__.py
--rw-r--r--   0 habsoomane   (501) staff       (20)     2794 2024-04-12 23:11:57.000000 sessionless-0.0.3/tests/modelsecp256k1__test.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-28 14:24:15.848871 sessionless-0.0.4/
+-rw-r--r--   0 habsoomane   (501) staff       (20)     3882 2024-04-28 14:24:15.847945 sessionless-0.0.4/PKG-INFO
+-rw-r--r--   0 habsoomane   (501) staff       (20)     3274 2024-04-27 23:39:27.000000 sessionless-0.0.4/README.md
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-28 14:24:15.839877 sessionless-0.0.4/sessionless/
+-rw-r--r--   0 habsoomane   (501) staff       (20)       59 2024-04-27 23:29:22.000000 sessionless-0.0.4/sessionless/__init__.py
+-rw-r--r--   0 habsoomane   (501) staff       (20)     2273 2024-04-27 23:42:26.000000 sessionless-0.0.4/sessionless/modelsecp256k1.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-28 14:24:15.846876 sessionless-0.0.4/sessionless.egg-info/
+-rw-r--r--   0 habsoomane   (501) staff       (20)     3882 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/PKG-INFO
+-rw-r--r--   0 habsoomane   (501) staff       (20)      291 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/SOURCES.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)        1 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/dependency_links.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       15 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/requires.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       17 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/top_level.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       38 2024-04-28 14:24:15.849059 sessionless-0.0.4/setup.cfg
+-rw-r--r--   0 habsoomane   (501) staff       (20)     1126 2024-04-27 23:01:41.000000 sessionless-0.0.4/setup.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-28 14:24:15.845574 sessionless-0.0.4/test/
+-rw-r--r--   0 habsoomane   (501) staff       (20)       69 2024-04-27 23:23:43.000000 sessionless-0.0.4/test/__init__.py
+-rw-r--r--   0 habsoomane   (501) staff       (20)     2761 2024-04-27 23:43:45.000000 sessionless-0.0.4/test/test_modelsecp256k1.py
```

### Comparing `sessionless-0.0.3/PKG-INFO` & `sessionless-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessionless
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.
 Author: Sessionless Team
 Author-email: zach@planetnine.app
 Keywords: authentication,cryptography,authenticate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -32,50 +32,50 @@
 ## Development 
 
 ### Getting started
 To use this package, please call a new instance of the SessionlessSecp256k1 class. Users will need to provide a get key method. This method will be referenced later on to obtain key values.
 
 ```python
 # This will create an instance of the SessionlessSecp256k1 class 
-# Users must pass a method to retrieve keys.
-def get_key():
-    pass
-sessionless = SessionlessSecp256k1(get_key)
+
+sessionless = SessionlessSecp256k1()
 ```
 
 ### Generating private and public keys
-The generate keys method will generate a private key and a public key. To use the method, users must provide a method to save the keys. 
+The generate keys method will generate a unique private key and a public key. To use the method, users must provide a method to save the keys. This function to save the keys is left to the user's implementation.
 ```python
-def save_key():
-    pass
-private_key, public_key = sessionless.generate_keys(save_key) # This will return the encrypted private and public key
+# The defined function will be called upon to store the generated keys
+def saveKey(keyPair):
+    db.store(keyPair["privateKey"], keyPair["publicKey"])
+private_key, public_key = sessionless.generateKeys(saveKey) 
 ```
 
 ### Signing messages
-Users can easily sign messages by providing a message to the sign method. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed.
+Users can easily sign messages by providing a message to the sign method and a callable method that will return the private key. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed. The method to the get the key is left to the user's implementation.
 ```python
+# The defined method to get the keys will be called to retrieve the private key
 msg = {
 "message": "The weather is so nice today!"
 }
-signature = sessionless.sign(msg)
+signature = sessionless.sign(msg, getKey(privateKey={}))
 ```
 
 ### Verifying messages
 Users can verify messages and signatures to ensure data integrity, authenticity, and non-repudiation. Users will pass a signature, message, and an encrypted public key as parameters. If public key is not provided, a public key will be generated from the instance's private key.
 ```python
-res = sessionless.verify_signature(signature, msg, public_key) # Returns True
-res2 = sessionless.verify_signature(first_signature, first_msg, second_primary_key) # Returns False
+result = sessionless.verifySignature(signature, msg, public_key) # Returns True
+result2 = sessionless.verifySignature(first_signature, first_msg, second_primary_key) # Returns False
 ```
 
 ### Associating messages
 Users can verify that two messages can be associated using the associate method. 
 ```python
-res = sessionless.associate(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
+result = sessionless.associate(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
 
 ```
 
 ### Generating UUIDs [Universally Unique Identifiers]
 Users can generate unique identifiers as needed by calling the generate UUID method.
 ```python
-uuid = sessionless.generate_UUID() # Returns UUID
+uuid = sessionless.generateUUID() # Returns UUID
 
 ```
```

### Comparing `sessionless-0.0.3/README.md` & `sessionless-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,50 +16,50 @@
 ## Development 
 
 ### Getting started
 To use this package, please call a new instance of the SessionlessSecp256k1 class. Users will need to provide a get key method. This method will be referenced later on to obtain key values.
 
 ```python
 # This will create an instance of the SessionlessSecp256k1 class 
-# Users must pass a method to retrieve keys.
-def get_key():
-    pass
-sessionless = SessionlessSecp256k1(get_key)
+
+sessionless = SessionlessSecp256k1()
 ```
 
 ### Generating private and public keys
-The generate keys method will generate a private key and a public key. To use the method, users must provide a method to save the keys. 
+The generate keys method will generate a unique private key and a public key. To use the method, users must provide a method to save the keys. This function to save the keys is left to the user's implementation.
 ```python
-def save_key():
-    pass
-private_key, public_key = sessionless.generate_keys(save_key) # This will return the encrypted private and public key
+# The defined function will be called upon to store the generated keys
+def saveKey(keyPair):
+    db.store(keyPair["privateKey"], keyPair["publicKey"])
+private_key, public_key = sessionless.generateKeys(saveKey) 
 ```
 
 ### Signing messages
-Users can easily sign messages by providing a message to the sign method. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed.
+Users can easily sign messages by providing a message to the sign method and a callable method that will return the private key. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed. The method to the get the key is left to the user's implementation.
 ```python
+# The defined method to get the keys will be called to retrieve the private key
 msg = {
 "message": "The weather is so nice today!"
 }
-signature = sessionless.sign(msg)
+signature = sessionless.sign(msg, getKey(privateKey={}))
 ```
 
 ### Verifying messages
 Users can verify messages and signatures to ensure data integrity, authenticity, and non-repudiation. Users will pass a signature, message, and an encrypted public key as parameters. If public key is not provided, a public key will be generated from the instance's private key.
 ```python
-res = sessionless.verify_signature(signature, msg, public_key) # Returns True
-res2 = sessionless.verify_signature(first_signature, first_msg, second_primary_key) # Returns False
+result = sessionless.verifySignature(signature, msg, public_key) # Returns True
+result2 = sessionless.verifySignature(first_signature, first_msg, second_primary_key) # Returns False
 ```
 
 ### Associating messages
 Users can verify that two messages can be associated using the associate method. 
 ```python
-res = sessionless.associate(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
+result = sessionless.associate(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
 
 ```
 
 ### Generating UUIDs [Universally Unique Identifiers]
 Users can generate unique identifiers as needed by calling the generate UUID method.
 ```python
-uuid = sessionless.generate_UUID() # Returns UUID
+uuid = sessionless.generateUUID() # Returns UUID
 
 ```
```

### Comparing `sessionless-0.0.3/sessionless.egg-info/PKG-INFO` & `sessionless-0.0.4/sessionless.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessionless
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.
 Author: Sessionless Team
 Author-email: zach@planetnine.app
 Keywords: authentication,cryptography,authenticate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -32,50 +32,50 @@
 ## Development 
 
 ### Getting started
 To use this package, please call a new instance of the SessionlessSecp256k1 class. Users will need to provide a get key method. This method will be referenced later on to obtain key values.
 
 ```python
 # This will create an instance of the SessionlessSecp256k1 class 
-# Users must pass a method to retrieve keys.
-def get_key():
-    pass
-sessionless = SessionlessSecp256k1(get_key)
+
+sessionless = SessionlessSecp256k1()
 ```
 
 ### Generating private and public keys
-The generate keys method will generate a private key and a public key. To use the method, users must provide a method to save the keys. 
+The generate keys method will generate a unique private key and a public key. To use the method, users must provide a method to save the keys. This function to save the keys is left to the user's implementation.
 ```python
-def save_key():
-    pass
-private_key, public_key = sessionless.generate_keys(save_key) # This will return the encrypted private and public key
+# The defined function will be called upon to store the generated keys
+def saveKey(keyPair):
+    db.store(keyPair["privateKey"], keyPair["publicKey"])
+private_key, public_key = sessionless.generateKeys(saveKey) 
 ```
 
 ### Signing messages
-Users can easily sign messages by providing a message to the sign method. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed.
+Users can easily sign messages by providing a message to the sign method and a callable method that will return the private key. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed. The method to the get the key is left to the user's implementation.
 ```python
+# The defined method to get the keys will be called to retrieve the private key
 msg = {
 "message": "The weather is so nice today!"
 }
-signature = sessionless.sign(msg)
+signature = sessionless.sign(msg, getKey(privateKey={}))
 ```
 
 ### Verifying messages
 Users can verify messages and signatures to ensure data integrity, authenticity, and non-repudiation. Users will pass a signature, message, and an encrypted public key as parameters. If public key is not provided, a public key will be generated from the instance's private key.
 ```python
-res = sessionless.verify_signature(signature, msg, public_key) # Returns True
-res2 = sessionless.verify_signature(first_signature, first_msg, second_primary_key) # Returns False
+result = sessionless.verifySignature(signature, msg, public_key) # Returns True
+result2 = sessionless.verifySignature(first_signature, first_msg, second_primary_key) # Returns False
 ```
 
 ### Associating messages
 Users can verify that two messages can be associated using the associate method. 
 ```python
-res = sessionless.associate(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
+result = sessionless.associate(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
 
 ```
 
 ### Generating UUIDs [Universally Unique Identifiers]
 Users can generate unique identifiers as needed by calling the generate UUID method.
 ```python
-uuid = sessionless.generate_UUID() # Returns UUID
+uuid = sessionless.generateUUID() # Returns UUID
 
 ```
```

### Comparing `sessionless-0.0.3/setup.py` & `sessionless-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 def read_markdown_file(file_path):
     with open(file_path, 'r', encoding='utf-8') as file:
         markdown_content = file.read()
     return markdown_content
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.'
 LONG_DESCRIPTION = read_markdown_file("./README.md")
 
 # Setting up
 setup(
         name="sessionless", 
         version=VERSION,
```

