# Comparing `tmp/srcsrv-1.2.10.tar.gz` & `tmp/srcsrv-1.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srcsrv-1.2.10.tar", last modified: Sat Mar  2 16:36:23 2024, max compression
+gzip compressed data, was "srcsrv-1.2.13.tar", last modified: Sun Apr 28 00:43:33 2024, max compression
```

## Comparing `srcsrv-1.2.10.tar` & `srcsrv-1.2.13.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-02 16:36:23.491752 srcsrv-1.2.10/
--rw-rw-rw-   0        0        0     1069 2022-08-20 22:38:23.000000 srcsrv-1.2.10/LICENSE
--rw-rw-rw-   0        0        0    14377 2024-03-02 16:36:23.489949 srcsrv-1.2.10/PKG-INFO
--rw-rw-rw-   0        0        0    13855 2024-03-02 16:33:45.000000 srcsrv-1.2.10/README.md
--rw-rw-rw-   0        0        0       42 2024-03-02 16:36:23.491752 srcsrv-1.2.10/setup.cfg
--rw-rw-rw-   0        0        0     2582 2024-03-01 07:11:59.000000 srcsrv-1.2.10/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:36:23.379439 srcsrv-1.2.10/srcsrv/
--rw-rw-rw-   0        0        0     1275 2023-09-14 12:28:57.000000 srcsrv-1.2.10/srcsrv/__init__.py
--rw-rw-rw-   0        0        0    14634 2024-03-01 07:11:59.000000 srcsrv-1.2.10/srcsrv/__main__.py
--rw-rw-rw-   0        0        0     6391 2024-03-01 07:11:59.000000 srcsrv-1.2.10/srcsrv/indexer.py
--rw-rw-rw-   0        0        0     7540 2023-09-14 12:28:57.000000 srcsrv-1.2.10/srcsrv/pdb.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:36:23.409982 srcsrv-1.2.10/srcsrv/plugins/
--rw-rw-rw-   0        0        0     1349 2023-09-14 12:28:57.000000 srcsrv-1.2.10/srcsrv/plugins/__init__.py
--rw-rw-rw-   0        0        0    10631 2024-03-01 07:11:59.000000 srcsrv-1.2.10/srcsrv/plugins/bitbucket.py
--rw-rw-rw-   0        0        0     8788 2024-03-01 07:11:59.000000 srcsrv-1.2.10/srcsrv/plugins/codebase.py
--rw-rw-rw-   0        0        0     8250 2024-03-01 07:11:59.000000 srcsrv-1.2.10/srcsrv/plugins/github.py
--rw-rw-rw-   0        0        0    10106 2024-03-01 07:11:59.000000 srcsrv-1.2.10/srcsrv/plugins/gitlab.py
--rw-rw-rw-   0        0        0     6801 2023-09-14 12:28:57.000000 srcsrv-1.2.10/srcsrv/plugins/plugin.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:36:23.433830 srcsrv-1.2.10/srcsrv/tools/
--rw-rw-rw-   0        0        0     1156 2023-09-14 12:28:57.000000 srcsrv-1.2.10/srcsrv/tools/__init__.py
--rw-rw-rw-   0        0        0     3681 2023-09-14 12:28:57.000000 srcsrv-1.2.10/srcsrv/tools/api.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:36:23.436612 srcsrv-1.2.10/srcsrv/utils/
--rw-rw-rw-   0        0        0     4484 2024-03-01 07:11:59.000000 srcsrv-1.2.10/srcsrv/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-02 16:36:23.476424 srcsrv-1.2.10/srcsrv.egg-info/
--rw-rw-rw-   0        0        0    14377 2024-03-02 16:36:23.000000 srcsrv-1.2.10/srcsrv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-03-02 16:36:23.000000 srcsrv-1.2.10/srcsrv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-02 16:36:23.000000 srcsrv-1.2.10/srcsrv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-03-02 16:36:23.000000 srcsrv-1.2.10/srcsrv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-02 16:36:23.000000 srcsrv-1.2.10/srcsrv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.835469 srcsrv-1.2.13/
+-rw-rw-rw-   0        0        0     1069 2022-08-20 22:38:23.000000 srcsrv-1.2.13/LICENSE
+-rw-rw-rw-   0        0        0    14500 2024-04-28 00:43:33.831522 srcsrv-1.2.13/PKG-INFO
+-rw-rw-rw-   0        0        0    13978 2024-04-26 16:19:46.000000 srcsrv-1.2.13/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 00:43:33.838240 srcsrv-1.2.13/setup.cfg
+-rw-rw-rw-   0        0        0     2582 2024-04-28 00:38:01.000000 srcsrv-1.2.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.742861 srcsrv-1.2.13/srcsrv/
+-rw-rw-rw-   0        0        0     1275 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/__init__.py
+-rw-rw-rw-   0        0        0    14634 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/__main__.py
+-rw-rw-rw-   0        0        0     6391 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/indexer.py
+-rw-rw-rw-   0        0        0     7683 2024-04-28 00:38:01.000000 srcsrv-1.2.13/srcsrv/pdb.py
+drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.775724 srcsrv-1.2.13/srcsrv/plugins/
+-rw-rw-rw-   0        0        0     1349 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/plugins/__init__.py
+-rw-rw-rw-   0        0        0    10631 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/plugins/bitbucket.py
+-rw-rw-rw-   0        0        0     8788 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/plugins/codebase.py
+-rw-rw-rw-   0        0        0     8250 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/plugins/github.py
+-rw-rw-rw-   0        0        0    10106 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/plugins/gitlab.py
+-rw-rw-rw-   0        0        0     6801 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/plugins/plugin.py
+drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.783131 srcsrv-1.2.13/srcsrv/tools/
+-rw-rw-rw-   0        0        0     1156 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/tools/__init__.py
+-rw-rw-rw-   0        0        0     3681 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/tools/api.py
+drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.790975 srcsrv-1.2.13/srcsrv/utils/
+-rw-rw-rw-   0        0        0     4484 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.817676 srcsrv-1.2.13/srcsrv.egg-info/
+-rw-rw-rw-   0        0        0    14500 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/top_level.txt
```

### Comparing `srcsrv-1.2.10/LICENSE` & `srcsrv-1.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/PKG-INFO` & `srcsrv-1.2.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srcsrv
-Version: 1.2.10
+Version: 1.2.13
 Summary: Source indexing package
 Home-page: https://github.com/urielmann/srcsrv-public
 Author: Uri Mann
 Author-email: abba.mann@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -186,9 +186,10 @@
 # External Links
 
 [Srcsrv.doc](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&ved=2ahUKEwjO_sL72NHlAhVYnp4KHcdmCdgQFjACegQIAxAC&url=https%3A%2F%2Fcrashopensource.files.wordpress.com%2F2007%2F10%2Fsrcsrv.doc&usg=AOvVaw0ONZV3AtYTB1S8sgPqhTsU)  
 [The SrcTool Utility](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/the-srctool-utility)  
 [Source Indexing is Underused Awesomeness](https://randomascii.wordpress.com/2011/11/11/source-indexing-is-underused-awesomeness/)  
 [Debugging with source indexed **.PDB**](docs/SETUP.md)  
 [Advance topics **.PDB**](docs/ADVANCE.md)  
+[Introduction to SRCSRV Package](https://drive.google.com/drive/folders/1j785kRtb1VvbeqtbieNoWMpL2L2obcpn?usp=drive_link)
```

### Comparing `srcsrv-1.2.10/README.md` & `srcsrv-1.2.13/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -169,7 +169,8 @@
 # External Links
 
 [Srcsrv.doc](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&ved=2ahUKEwjO_sL72NHlAhVYnp4KHcdmCdgQFjACegQIAxAC&url=https%3A%2F%2Fcrashopensource.files.wordpress.com%2F2007%2F10%2Fsrcsrv.doc&usg=AOvVaw0ONZV3AtYTB1S8sgPqhTsU)  
 [The SrcTool Utility](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/the-srctool-utility)  
 [Source Indexing is Underused Awesomeness](https://randomascii.wordpress.com/2011/11/11/source-indexing-is-underused-awesomeness/)  
 [Debugging with source indexed **.PDB**](docs/SETUP.md)  
 [Advance topics **.PDB**](docs/ADVANCE.md)  
+[Introduction to SRCSRV Package](https://drive.google.com/drive/folders/1j785kRtb1VvbeqtbieNoWMpL2L2obcpn?usp=drive_link)
```

### Comparing `srcsrv-1.2.10/setup.py` & `srcsrv-1.2.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='srcsrv',
-    version='1.2.10',
+    version='1.2.13',
     author='Uri Mann',
     author_email='abba.mann@gmail.com',
     description='Source indexing package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Additional assets for README.md
     package_data={'': [
```

### Comparing `srcsrv-1.2.10/srcsrv/__init__.py` & `srcsrv-1.2.13/srcsrv/__init__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/__main__.py` & `srcsrv-1.2.13/srcsrv/__main__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/indexer.py` & `srcsrv-1.2.13/srcsrv/indexer.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/pdb.py` & `srcsrv-1.2.13/srcsrv/pdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,25 +46,28 @@
         '''
         Property containing a list of source files in the current source tree
         :return List of source files
         '''
         # Send the output to a file. On large .PDBs with many entries
         # using OS buffering consumes too much time and memory.
         with open(self._srcs_path, 'w+') as srcs:
+            cmd = [
+                self.si.srctool,
+                f'-l:{srcs_match}*',
+                '-r', '-z', '-h',
+                self._pdb_path
+            ]
+
             try:
-                cp = subprocess.run([self.si.srctool,
-                                     f'-l:{srcs_match}*',
-                                     '-r', '-z', '-h',
-                                     self._pdb_path],
-                                     stdout=srcs, check=True)
+                cp = subprocess.run(cmd, stdout=srcs, check=True)
                 srcs.seek(0)
                 yield from srcs
             except subprocess.CalledProcessError as ex:
                 if ex.stderr:
-                    logging.error(f'{self.si.srctool} returned an error processing {ex.stderr}')
+                    logging.error(f'{cmd=} returned error 0x{ex.returncode:08x}! stdout: "{ex.stdout}", stderr: "{ex.stderr}"')
 
     def process(self):
         '''
         Process a single .PDB file
         '''
         start = time.time()
         summary = {
@@ -143,18 +146,26 @@
 '''SRCSRV: end ------------------------------------------------
 '''
             )
 
         logging.info(f'{self._pdb_path} contains: {self._sources_count} source files')
         # Write the the output file onto the .PDB
         if not self.si.args.dry_run:
+            cmd = [
+                self.si.pdbstr,
+                '-w',
+                f'-p:{self._pdb_path}',
+                '-s:srcsrv',
+                f'-i:{stream.name}'
+            ]
+
             try:
-                cp = subprocess.run([self.si.pdbstr, '-w', f'-p:{self._pdb_path}', f'-s:srcsrv', f'-i:{stream.name}'], check=True)
+                cp = subprocess.run(cmd, check=True)
             except subprocess.CalledProcessError as ex:
-                logging.error(f'{self.si.pdbstr} returned an error processing {ex.stderr}')
+                logging.error(f'{cmd=} returned error 0x{ex.returncode:08x}! stdout: "{ex.stdout}", stderr: "{ex.stderr}"')
 
         if not self.si.args.keep:
             # Remove the output files
             os.remove(self._ini_path)
             os.remove(self._srcs_path)
 
         if self.si.args.summary:
```

### Comparing `srcsrv-1.2.10/srcsrv/plugins/__init__.py` & `srcsrv-1.2.13/srcsrv/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/plugins/bitbucket.py` & `srcsrv-1.2.13/srcsrv/plugins/bitbucket.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/plugins/codebase.py` & `srcsrv-1.2.13/srcsrv/plugins/codebase.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/plugins/github.py` & `srcsrv-1.2.13/srcsrv/plugins/github.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/plugins/gitlab.py` & `srcsrv-1.2.13/srcsrv/plugins/gitlab.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/plugins/plugin.py` & `srcsrv-1.2.13/srcsrv/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/tools/__init__.py` & `srcsrv-1.2.13/srcsrv/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/tools/api.py` & `srcsrv-1.2.13/srcsrv/tools/api.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv/utils/__init__.py` & `srcsrv-1.2.13/srcsrv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.10/srcsrv.egg-info/PKG-INFO` & `srcsrv-1.2.13/srcsrv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srcsrv
-Version: 1.2.10
+Version: 1.2.13
 Summary: Source indexing package
 Home-page: https://github.com/urielmann/srcsrv-public
 Author: Uri Mann
 Author-email: abba.mann@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -186,9 +186,10 @@
 # External Links
 
 [Srcsrv.doc](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&ved=2ahUKEwjO_sL72NHlAhVYnp4KHcdmCdgQFjACegQIAxAC&url=https%3A%2F%2Fcrashopensource.files.wordpress.com%2F2007%2F10%2Fsrcsrv.doc&usg=AOvVaw0ONZV3AtYTB1S8sgPqhTsU)  
 [The SrcTool Utility](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/the-srctool-utility)  
 [Source Indexing is Underused Awesomeness](https://randomascii.wordpress.com/2011/11/11/source-indexing-is-underused-awesomeness/)  
 [Debugging with source indexed **.PDB**](docs/SETUP.md)  
 [Advance topics **.PDB**](docs/ADVANCE.md)  
+[Introduction to SRCSRV Package](https://drive.google.com/drive/folders/1j785kRtb1VvbeqtbieNoWMpL2L2obcpn?usp=drive_link)
```

