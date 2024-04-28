# Comparing `tmp/medium_to_markdown_py-1.0.0.tar.gz` & `tmp/medium_to_markdown_py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_to_markdown_py-1.0.0.tar", last modified: Sun Apr 28 04:36:12 2024, max compression
+gzip compressed data, was "medium_to_markdown_py-1.0.1.tar", last modified: Sun Apr 28 14:21:29 2024, max compression
```

## Comparing `medium_to_markdown_py-1.0.0.tar` & `medium_to_markdown_py-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 04:36:12.377130 medium_to_markdown_py-1.0.0/
--rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.0/LICENSE
--rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 04:36:12.377066 medium_to_markdown_py-1.0.0/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      592 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.0/README.md
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 04:36:12.375774 medium_to_markdown_py-1.0.0/medium-to-markdown-py/
--rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.0/medium-to-markdown-py/__init__.py
--rw-r--r--   0 shin       (501) staff       (20)     6716 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.0/medium-to-markdown-py/medium_to_markdown.py
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 04:36:12.376853 medium_to_markdown_py-1.0.0/medium_to_markdown_py.egg-info/
--rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.0/medium_to_markdown_py.egg-info/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      382 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.0/medium_to_markdown_py.egg-info/SOURCES.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.0/medium_to_markdown_py.egg-info/dependency_links.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.0/medium_to_markdown_py.egg-info/not-zip-safe
--rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.0/medium_to_markdown_py.egg-info/requires.txt
--rw-r--r--   0 shin       (501) staff       (20)       22 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.0/medium_to_markdown_py.egg-info/top_level.txt
--rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 04:36:12.377329 medium_to_markdown_py-1.0.0/setup.cfg
--rw-r--r--   0 shin       (501) staff       (20)      599 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.0/setup.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:21:29.438583 medium_to_markdown_py-1.0.1/
+-rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.1/LICENSE
+-rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 14:21:29.438520 medium_to_markdown_py-1.0.1/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      633 2024-04-28 14:20:07.000000 medium_to_markdown_py-1.0.1/README.md
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:21:29.437206 medium_to_markdown_py-1.0.1/medium-to-markdown-py/
+-rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 14:21:11.000000 medium_to_markdown_py-1.0.1/medium-to-markdown-py/__init__.py
+-rw-r--r--   0 shin       (501) staff       (20)     7313 2024-04-28 14:19:31.000000 medium_to_markdown_py-1.0.1/medium-to-markdown-py/medium_to_markdown.py
+-rw-r--r--   0 shin       (501) staff       (20)      320 2024-04-28 13:54:29.000000 medium_to_markdown_py-1.0.1/medium-to-markdown-py/tester.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:21:29.438323 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/
+-rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      414 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/not-zip-safe
+-rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/requires.txt
+-rw-r--r--   0 shin       (501) staff       (20)       22 2024-04-28 14:21:29.000000 medium_to_markdown_py-1.0.1/medium_to_markdown_py.egg-info/top_level.txt
+-rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 14:21:29.438777 medium_to_markdown_py-1.0.1/setup.cfg
+-rw-r--r--   0 shin       (501) staff       (20)      599 2024-04-28 14:21:17.000000 medium_to_markdown_py-1.0.1/setup.py
```

### Comparing `medium_to_markdown_py-1.0.0/LICENSE` & `medium_to_markdown_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.0.0/medium-to-markdown-py/medium_to_markdown.py` & `medium_to_markdown_py-1.0.1/medium-to-markdown-py/medium_to_markdown.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,92 @@
 from datetime import datetime
 from bs4 import BeautifulSoup, Tag, NavigableString
 
 import requests
 import shutil
 import os
-import argparse
-
+import re
 class MediumParser:
     
     IMAGE_SEQUENCE = 0
     OUTPUT_DIR = "medium/origin_md"
     
-    def __init__(self, url, output_filename, is_image_download=False,ssl_verify=False):
+    def __init__(self, url, output_filename="", is_image_download=False,ssl_verify=False,headers={'User-Agent': 'Mozilla/5.0'}):
+        """
+            Initialize a MediumParser object.
+
+            Parameters:
+            - url (str): The URL of the Medium article to convert to Markdown.
+            - output_filename (str): The desired filename for the output Markdown file. If not provided, a default filename will be used.
+            - is_image_download (bool): Flag indicating whether to download images referenced in the article. Default is False.
+            - ssl_verify (bool): Flag indicating whether to verify SSL certificates when making requests. Default is False.
+            - headers (dict): Custom headers to include in the HTTP requests. Default is {'User-Agent': 'Mozilla/5.0'}.
+        """
         self.url = url
-        self.output_filename = output_filename
         self.is_image_download = is_image_download
         self.ssl_verify = ssl_verify
+        self.headers = headers
         self.current_date = datetime.now().strftime("%Y-%m-%d")
         self.title=""
         self.author=""
+        self.output_filename=output_filename
         
-        if self.output_filename.endswith(".md"):
-            self.output_filename = self.output_filename[:-3]
-            
-        self.output_filename = f"{self.current_date}-{self.output_filename[:-3]}"
-        
+        if self.output_filename != "":
+            if self.output_filename.endswith(".md"):
+                self.output_filename = self.output_filename[:-3]
+                
+            self.output_filename = f"{self.current_date}-{self.output_filename}"
+
 
     def parse_and_savefile(self):
+        """
+        Parses the Medium post, saves it as a Markdown file, and returns True if successful, False otherwise.
+        """
         try:
             dom = self.get_dom(self.url)
+            self.get_meta(dom)
+            
+            if self.output_filename == "":
+                self.output_filename = re.sub(r'[<>:"/\\|?*]', '', self.title).replace(" ", "_")
+                output_filename = f"{self.OUTPUT_DIR}/{self.current_date}-{self.output_filename}.md"
+            else:
+                output_filename = f"{self.OUTPUT_DIR}/{self.output_filename}.md"
+                
             parsed_post = self.parse_medium_post(dom)
-            output_filename = f"{self.OUTPUT_DIR}/{self.output_filename}.md"
             
             if not os.path.exists(os.path.dirname(output_filename)):
                 os.makedirs(os.path.dirname(output_filename))
             
-            with open(output_filename, "w",encoding='utf-8') as f:
+            with open(output_filename, "w", encoding='utf-8') as f:
                 f.write(parsed_post)
                 
             return True
         except Exception as e:
             print(f"An error occurred: {e}")
             return False
 
     def get_dom(self,url):
-        response = requests.get(url, verify=self.ssl_verify)
+        response = requests.get(url, verify=self.ssl_verify,headers=self.headers)
         response.raise_for_status()
         return BeautifulSoup(response.text, 'html.parser')
-
+    
+    def get_meta(self,dom):
+        try:
+            title_tag = dom.find('meta', {'name': 'title'})
+            author_tag = dom.find('meta', {'name': 'author'})
+            self.title = title_tag['content'] if title_tag else ''
+            self.author = author_tag['content'] if author_tag else ''
+            return True
+        except Exception as e:
+            print(f"An error occurred: {e}")
+            return False
+        
     def parse_medium_post(self,dom):
         parsed_post = []
-        title_tag = dom.find('meta', {'name': 'title'})
-        author_tag = dom.find('meta', {'name': 'author'})
-        self.title = title_tag['content'] if title_tag else ''
-        self.author = author_tag['content'] if author_tag else ''
+        
         for node in dom.children:
             content = self.parse_dom(node)
             if content:
                 parsed_post.append(content)
       
         parsed_post.insert(0, f"---\ntitle: {self.title}\nauthor: {self.author}\ndate: {self.current_date}\nurl: {self.url}\n---\n")
         return '\n'.join(parsed_post)
@@ -88,27 +117,27 @@
                 if links_str:
                     links = links_str.split(" ")
                     link = next((link for link in links if 'webp' in link), None)
                     if link:
                         if self.is_image_download==False:
                             parsed_content.append(f"![Medium-Image]({link.strip()})\n")
                         else:
-                            response = requests.get(link.strip(), stream=True,verify=self.ssl_verify)
+                            response = requests.get(link.strip(), stream=True,verify=self.ssl_verify,headers=self.headers)
                             if response.status_code == 200:
 
                                 filename = f"{self.output_filename}_{self.IMAGE_SEQUENCE}.png"
                                 local_image_path = f"{self.OUTPUT_DIR}/image/{filename}"
                                 if not os.path.exists(os.path.dirname(local_image_path)):
                                     os.makedirs(os.path.dirname(local_image_path))
                                 with open(local_image_path, 'wb') as out_file:
                                     shutil.copyfileobj(response.raw, out_file)
                                     
                                 del response
 
-                                parsed_content.append(f"![Medium-Image]({local_image_path})\n")
+                                parsed_content.append(f"![Medium-Image](image/{filename})\n")
                                 self.IMAGE_SEQUENCE += 1
             else:
                 for child in node.children:
                     child_content = self.parse_dom(child)
                     if child_content:
                         parsed_content.append(child_content)
         
@@ -140,26 +169,8 @@
 
     def parse_formatting_text(self,element):
         result = []
         for child in element.children:
             text = self.extract_inline(child)
             if text:
                 result.append(text)
-        return ''.join(result)
-
-if __name__ == "__main__":
-    print("Medium to Markdown Parser")
-    print("Start parsing...")
-    
-    arg_parser = argparse.ArgumentParser(description="Medium to Markdown Parser")
-    arg_parser.add_argument("--url", help="Medium post URL",required=True)
-    arg_parser.add_argument("--filename", help="Output filename",required=True)
-    arg_parser.add_argument("--is_image_download", help="Image download option(Y or N)", default="N",required=False)
-    arg_parser.add_argument("--ssl_verify", help="SSL Verify option(Y or N)", default="N",required=False)
-    args = arg_parser.parse_args()
-    
-    parser = MediumParser(args.url, args.filename, 
-                            False if args.is_image_download.upper() == "N" else True, 
-                            False if args.ssl_verify.upper() == "N" else True)
-    
-    if parser.parse_and_savefile():
-        print("Parsing is done.")
+        return ''.join(result)
```

### Comparing `medium_to_markdown_py-1.0.0/setup.py` & `medium_to_markdown_py-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medium-to-markdown-py',
-    version='1.0.0',
+    version='1.0.1',
     description='medium-to-markdown-py is a Python package that converts Medium articles to Markdown format.',
     author='knowslog',
     author_email='scshin88@gmail.com',
     url='https://github.com/tourbut/medium-to-markdown_python',
     install_requires=['beautifulsoup4', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['medium', 'knowslog', 'markdown', 'medium to markdown'],
```

