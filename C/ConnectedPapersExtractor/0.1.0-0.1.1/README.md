# Comparing `tmp/connectedpapersextractor-0.1.0.tar.gz` & `tmp/connectedpapersextractor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectedpapersextractor-0.1.0.tar", last modified: Sat Apr 13 14:02:37 2024, max compression
+gzip compressed data, was "connectedpapersextractor-0.1.1.tar", max compression
```

## Comparing `connectedpapersextractor-0.1.0.tar` & `connectedpapersextractor-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-13 14:02:37.885158 connectedpapersextractor-0.1.0/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 19:44:41.000000 connectedpapersextractor-0.1.0/LICENSE
--rw-r--r--   0 tesla     (1000) tesla     (1000)      645 2024-04-13 14:02:37.885158 connectedpapersextractor-0.1.0/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       27 2024-04-13 12:36:50.000000 connectedpapersextractor-0.1.0/README.md
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      107 2024-04-12 22:23:59.000000 connectedpapersextractor-0.1.0/pyproject.toml
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      703 2024-04-13 14:02:37.885158 connectedpapersextractor-0.1.0/setup.cfg
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-13 14:02:37.881158 connectedpapersextractor-0.1.0/src/
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-13 14:02:37.885158 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      204 2024-04-13 13:08:29.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor/ArticleFilter.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      493 2024-04-13 12:57:20.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor/PdfSummary.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      177 2024-04-13 12:36:52.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor/__init__.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)     1760 2024-04-13 13:53:19.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor/_get_pdf_summaries.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      979 2024-04-13 13:08:29.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor/_get_urls.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      960 2024-04-13 13:08:29.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor/get_summaries.py
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-13 14:02:37.885158 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor.egg-info/
--rw-r--r--   0 tesla     (1000) tesla     (1000)      645 2024-04-13 14:02:37.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor.egg-info/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      570 2024-04-13 14:02:37.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor.egg-info/SOURCES.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-13 14:02:37.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor.egg-info/dependency_links.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       45 2024-04-13 14:02:37.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor.egg-info/requires.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       25 2024-04-13 14:02:37.000000 connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.1.1/LICENSE
+-rw-r--r--   0        0        0      644 2024-04-28 14:10:16.375106 connectedpapersextractor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-27 22:23:56.499918 connectedpapersextractor-0.1.1/src/connectedpapersextractor/ArticleFilter.py
+-rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.1.1/src/connectedpapersextractor/Config.py
+-rw-r--r--   0        0        0      374 2024-04-28 13:45:00.686988 connectedpapersextractor-0.1.1/src/connectedpapersextractor/MainPartsExtractor.py
+-rw-r--r--   0        0        0     2062 2024-04-28 13:45:00.742987 connectedpapersextractor-0.1.1/src/connectedpapersextractor/PdfSummary.py
+-rw-r--r--   0        0        0     2486 2024-04-28 13:45:00.750987 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_AIExtractor.py
+-rw-r--r--   0        0        0      344 2024-04-28 13:39:32.895971 connectedpapersextractor-0.1.1/src/connectedpapersextractor/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-28 13:43:53.635611 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_add_docs.py
+-rw-r--r--   0        0        0      872 2024-04-28 11:53:43.189003 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_combine_summaries.py
+-rw-r--r--   0        0        0     2526 2024-04-28 13:41:29.892333 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_get_pdf_summaries.py
+-rw-r--r--   0        0        0     2052 2024-04-28 13:39:32.907971 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_summarize_documents_piecemeal.py
+-rw-r--r--   0        0        0     1529 2024-04-28 13:39:32.871971 connectedpapersextractor-0.1.1/src/connectedpapersextractor/create_related_work.py
+-rw-r--r--   0        0        0     1450 2024-04-28 13:47:45.376986 connectedpapersextractor-0.1.1/src/connectedpapersextractor/get_summaries.py
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 connectedpapersextractor-0.1.1/PKG-INFO
```

### Comparing `connectedpapersextractor-0.1.0/LICENSE` & `connectedpapersextractor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.0/src/ConnectedPapersExtractor/_get_pdf_summaries.py` & `connectedpapersextractor-0.1.1/src/connectedpapersextractor/_get_pdf_summaries.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,79 @@
+import json
+from dataclasses import asdict
 from itertools import count
 from pathlib import Path
 from typing import Union
 
-import arxiv
+from download import download
 from enhanced_webdriver import EnhancedWebdriver
+from undetected_chromedriver import ChromeOptions
 
-from . import ArticleFilter
-from .PdfSummary import PdfSummary
+from . import PdfSummaries, PdfSummary
+from .Config import Config
 
 
 def _get_pdf_summaries(
     connected_papers_link: str,
-    article_filter: ArticleFilter,
     dir_path: Union[str, Path] = Path("./"),
-) -> list[PdfSummary]:
-    driver = EnhancedWebdriver.create()
+) -> PdfSummaries:
+    options = ChromeOptions()
+    options.headless = True
+    driver = EnhancedWebdriver.create(undetected=True, options=options)
     driver.get(connected_papers_link)
     summaries = list()
+    downloads = list()
     for index in count(1):
         if not driver.click(
             f'//*[@id="desktop-app"]/div[2]/div[4]/div[1]/div/div[2]/div/div[2]/div[{index}]'
         ):
             break
-        link = (
-            driver.get_attribute(
-                '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[5]/a[1]',
-                "href",
-            )
-            .split("/")[-1]
-            .rpartition(".")[0]
+        link = driver.get_attribute(
+            '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[5]/a[1]',
+            "href",
         )
-        if not link:
-            continue
-        try:
-            paper = next(arxiv.Client().results(arxiv.Search(id_list=[link])))
-        except StopIteration:
+        if (
+            driver.get_text_of_element(
+                '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[5]/a[1]/span'
+            )
+            != "PDF"
+        ):
             continue
-        summaries.append(
-            PdfSummary(
-                download_function=lambda: paper.download_pdf(dirpath=str(dir_path)),
-                year=int(
-                    driver.get_text_of_element(
-                        '//*[@id="desktop-app"]/div[2]/div[4]/div[1]/div/div[2]/div/div[2]/div[2]/div[2]/div[2]'
-                    )
-                ),
-                citations=int(
-                    driver.get_text_of_element(
-                        '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[4]/div[1]'
-                    ).split()[0]
-                ),
+        title = driver.get_text_of_element(
+            '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[1]/div/a'
+        )
+        file_path = dir_path.joinpath(link.rpartition("/")[-1]).with_suffix(".pdf")
+        summary = PdfSummary(
+            file_path=file_path,
+            year=int(
+                driver.get_text_of_element(
+                    '//*[@id="desktop-app"]/div[2]/div[4]/div[1]/div/div[2]/div/div[2]/div[2]/div[2]/div[2]'
+                )
+            ),
+            citations=int(
+                driver.get_text_of_element(
+                    '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[4]/div[1]'
+                ).split()[0]
+            ),
+            title=title,
+        )
+        summaries.append(summary)
+        downloads.append(
+            (
+                link,
+                str(file_path),
             )
         )
-    summaries = article_filter.filter(summaries)
-
+    driver.quit()
+    for link, file_path in downloads:
+        download(link, file_path)
+    summaries = list(filter(PdfSummary.is_valid, summaries))
+    dir_path.joinpath(Config.metadate_file_name).write_text(
+        json.dumps(
+            dict(
+                (str(summary_dict.pop("file_path")), summary_dict)
+                for summary_dict in map(asdict, summaries)
+            ),
+            indent=2,
+        )
+    )
     return summaries
```

