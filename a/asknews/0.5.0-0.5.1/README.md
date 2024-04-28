# Comparing `tmp/asknews-0.5.0-py3-none-any.whl.zip` & `tmp/asknews-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 22019 bytes, number of entries: 24
+Zip file size: 22032 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 asknews_sdk/__init__.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 asknews_sdk/api/__init__.py
 -rw-r--r--  2.0 unx     4442 b- defN 80-Jan-01 00:00 asknews_sdk/api/analytics.py
 -rw-r--r--  2.0 unx      170 b- defN 80-Jan-01 00:00 asknews_sdk/api/base.py
 -rw-r--r--  2.0 unx     7443 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
 -rw-r--r--  2.0 unx    11705 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
 -rw-r--r--  2.0 unx    10375 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
 -rw-r--r--  2.0 unx    15904 b- defN 80-Jan-01 00:00 asknews_sdk/client.py
 -rw-r--r--  2.0 unx      740 b- defN 80-Jan-01 00:00 asknews_sdk/dto/__init__.py
 -rw-r--r--  2.0 unx     2424 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
 -rw-r--r--  2.0 unx     3381 b- defN 80-Jan-01 00:00 asknews_sdk/dto/chat.py
 -rw-r--r--  2.0 unx      606 b- defN 80-Jan-01 00:00 asknews_sdk/dto/error.py
 -rw-r--r--  2.0 unx     1284 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
 -rw-r--r--  2.0 unx      552 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
--rw-r--r--  2.0 unx     4166 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
+-rw-r--r--  2.0 unx     4194 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1414 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
 -rw-r--r--  2.0 unx     6302 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5248 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1583 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3185 b- defN 80-Jan-01 00:00 asknews-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.5.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.5.0.dist-info/RECORD
-24 files, 84686 bytes uncompressed, 18985 bytes compressed:  77.6%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3185 b- defN 80-Jan-01 00:00 asknews-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.5.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.5.1.dist-info/RECORD
+24 files, 84714 bytes uncompressed, 18998 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.5.0.dist-info/LICENSE
+Filename: asknews-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.5.0.dist-info/METADATA
+Filename: asknews-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.5.0.dist-info/WHEEL
+Filename: asknews-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.5.0.dist-info/RECORD
+Filename: asknews-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asknews_sdk/dto/stories.py

```diff
@@ -80,14 +80,15 @@
     languages: dict[str, int]
     keywords: list[str]
     intra_cluster_statistics: IntraClusterStatistics
     silhouette_score: dict
     article_ids: list[UUID]
     countries: dict[str, int]
     markdown_citations: list[str]
+    confidence: float = 0.0
 
 class StoryResponse(BaseSchema):
     uuid: Annotated[UUID, Field(title='UUID')]
     categories: Annotated[list[str], Field(title='Categories')]
     countries: Annotated[dict[str, int], Field(title='Countries')]
     countries_pct: Annotated[dict[str, float], Field(title='Countries percentage')]
     current_update_uuid: Annotated[str, Field(title='Current update UUID')]
```

## Comparing `asknews-0.5.0.dist-info/LICENSE` & `asknews-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.5.0.dist-info/METADATA` & `asknews-0.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asknews
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python SDK for AskNews
 Home-page: https://gitlab.com/emergentmethods/asknews/python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `asknews-0.5.0.dist-info/RECORD` & `asknews-0.5.1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 asknews_sdk/client.py,sha256=Lj7akBppXJI7XUNDgkbQhEbcGDP58P5noEA_ncXjeYM,15904
 asknews_sdk/dto/__init__.py,sha256=tNRL7YBHo76LAeTADE9qIj5xR0eQywJHpuer7QSuJXY,740
 asknews_sdk/dto/base.py,sha256=B5FJzeaKDNg9GE14cI7TdE_6vTQ1_HUhzY0RToVh-bw,2424
 asknews_sdk/dto/chat.py,sha256=AvRpnpGGaW3wCItqn77L-YtIg9OMCc-isuaeJyFEm80,3381
 asknews_sdk/dto/error.py,sha256=XhOo_lgl9vVHbhUVQiFIUXVaXAexUULjr7Hph5b6Ovc,606
 asknews_sdk/dto/news.py,sha256=vI3CC3rljq9I7T5ivp97KZpbvSeJJzel7b5N3qFEqyo,1284
 asknews_sdk/dto/sentiment.py,sha256=m6d-5mQ0dd4vewj7wF3-IZGLknXHkaKRmdYbyUaYI50,552
-asknews_sdk/dto/stories.py,sha256=91vsZukWukCrBR3GM4LkgT5Pn0NydU8Ec8hUb37uPRc,4166
+asknews_sdk/dto/stories.py,sha256=qE_X43yuEA3Bi8OQHr3MndQ6TKdGGHz-a1FIkixWNgY,4194
 asknews_sdk/errors.py,sha256=F7VncOcrCxM1mYGCqV2NUGDnDnqQWgxhhmXd__-5bK8,1414
 asknews_sdk/sdk.py,sha256=etSaKeGiUIQ2qd1Ek_m86eKTEe7FbAYacUq1UdY1Nd4,6302
 asknews_sdk/security.py,sha256=C3_-lQMwHNx9E-4GC4LedXofJ2ybZLGQGxIh55nVvks,5248
 asknews_sdk/utils.py,sha256=YAk-0ANXWu7J9PlKCyptXZnlvle4cLXuQWXxjxxWojQ,1583
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.5.0.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.5.0.dist-info/METADATA,sha256=t57msDyGwFhD8qQqSWR4OpHI-ulGmV_6dB86Tzw4cJg,3185
-asknews-0.5.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.5.0.dist-info/RECORD,,
+asknews-0.5.1.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.5.1.dist-info/METADATA,sha256=JsR7yZp5QOd8ih29RM_9kG0J6tGzKMTFmtR3YogbTs8,3185
+asknews-0.5.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.5.1.dist-info/RECORD,,
```

