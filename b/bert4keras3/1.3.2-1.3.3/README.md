# Comparing `tmp/bert4keras3-1.3.2-py3-none-any.whl.zip` & `tmp/bert4keras3-1.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 43962 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      150 b- defN 24-Apr-26 10:58 bert4keras3/__init__.py
+Zip file size: 43978 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      214 b- defN 24-Apr-28 15:54 bert4keras3/__init__.py
 -rw-rw-rw-  2.0 fat    23146 b- defN 24-Apr-26 10:58 bert4keras3/backend.py
 -rw-rw-rw-  2.0 fat    11419 b- defN 24-Apr-26 10:58 bert4keras3/layers.py
 -rw-rw-rw-  2.0 fat     5211 b- defN 24-Apr-26 10:58 bert4keras3/models.py
 -rw-rw-rw-  2.0 fat    30152 b- defN 24-Apr-26 10:58 bert4keras3/ops.py
 -rw-rw-rw-  2.0 fat    27955 b- defN 24-Apr-26 10:58 bert4keras3/snippets.py
 -rw-rw-rw-  2.0 fat    15509 b- defN 24-Apr-26 10:58 bert4keras3/tokenizers.py
 -rw-rw-rw-  2.0 fat    28576 b- defN 24-Apr-26 10:58 bert4keras3/transformers.py
--rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-26 11:03 bert4keras3-1.3.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      188 b- defN 24-Apr-26 11:03 bert4keras3-1.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 11:03 bert4keras3-1.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-26 11:03 bert4keras3-1.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1047 b- defN 24-Apr-26 11:03 bert4keras3-1.3.2.dist-info/RECORD
-13 files, 154815 bytes uncompressed, 42234 bytes compressed:  72.7%
+-rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-28 15:58 bert4keras3-1.3.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      188 b- defN 24-Apr-28 15:58 bert4keras3-1.3.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 15:58 bert4keras3-1.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-28 15:58 bert4keras3-1.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1047 b- defN 24-Apr-28 15:58 bert4keras3-1.3.3.dist-info/RECORD
+13 files, 154879 bytes uncompressed, 42250 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: bert4keras3/tokenizers.py
 Comment: 
 
 Filename: bert4keras3/transformers.py
 Comment: 
 
-Filename: bert4keras3-1.3.2.dist-info/LICENSE
+Filename: bert4keras3-1.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: bert4keras3-1.3.2.dist-info/METADATA
+Filename: bert4keras3-1.3.3.dist-info/METADATA
 Comment: 
 
-Filename: bert4keras3-1.3.2.dist-info/WHEEL
+Filename: bert4keras3-1.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: bert4keras3-1.3.2.dist-info/top_level.txt
+Filename: bert4keras3-1.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bert4keras3-1.3.2.dist-info/RECORD
+Filename: bert4keras3-1.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bert4keras3/__init__.py

```diff
@@ -1,6 +1,8 @@
 #! -*- coding: utf-8 -*-
 
-__version__ = '1.1.2'
+__version__ = '1.3'
 
 from bert4keras3 import backend,layers,models,snippets,tokenizers
+from bert4keras3 import Models
+from bert4keras3 import Layers_add
 from bert4keras3.backend import ops
```

## Comparing `bert4keras3-1.3.2.dist-info/LICENSE` & `bert4keras3-1.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bert4keras3-1.3.2.dist-info/RECORD` & `bert4keras3-1.3.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-bert4keras3/__init__.py,sha256=CMb8S8X82Zw-9GhxgUom0I8qs7veKePBxPqa7nStNpk,150
+bert4keras3/__init__.py,sha256=cGygEKNWzw6mGicNGuB_KCwEEAT3qcybGRHuqLEPe-4,214
 bert4keras3/backend.py,sha256=D-9WqJu_Xu37hoHecwQyZmhMgIWrli38_ny8SyW9ZXE,23146
 bert4keras3/layers.py,sha256=IbVd3zYbsXhjeVOjcA0TSpuIbfa3eAJQ6f9N_eXnYO4,11419
 bert4keras3/models.py,sha256=o7DHSr3Dvj7IIa5oVBqyO92fIm2oLU-pPoo5YsSlNaU,5211
 bert4keras3/ops.py,sha256=H1sbMv6WOJ5iGAB0rosPz9LoqdT0jS8knLRW_6XkFRU,30152
 bert4keras3/snippets.py,sha256=YwdYRvrewhM6g8ax9_Ath0HsJATzuyZksL5Dow9l65A,27955
 bert4keras3/tokenizers.py,sha256=PCxtC4L9tF2w-GUDujdPK8Z5WlnbaL8mYhRfHn1S_Qg,15509
 bert4keras3/transformers.py,sha256=g0-dYhls5_Og9bWCBkIgGpofK-sScFnqZO0kqAKmbkE,28576
-bert4keras3-1.3.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-bert4keras3-1.3.2.dist-info/METADATA,sha256=N49Bzh0uR0eBp6zu8C2T7yHJkWzjpFfVMeQ-Bhjz96Q,188
-bert4keras3-1.3.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-bert4keras3-1.3.2.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
-bert4keras3-1.3.2.dist-info/RECORD,,
+bert4keras3-1.3.3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+bert4keras3-1.3.3.dist-info/METADATA,sha256=mILKrE16fAn-2bPeoyDlQCKy0lPTk0rn2WHRZ9lEXZ8,188
+bert4keras3-1.3.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+bert4keras3-1.3.3.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
+bert4keras3-1.3.3.dist-info/RECORD,,
```

