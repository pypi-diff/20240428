# Comparing `tmp/package_auto_assembler-0.0.8.tar.gz` & `tmp/package_auto_assembler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_auto_assembler-0.0.8.tar", last modified: Thu Apr 25 00:58:49 2024, max compression
+gzip compressed data, was "package_auto_assembler-0.0.9.tar", last modified: Sat Apr 27 02:30:07 2024, max compression
```

## Comparing `package_auto_assembler-0.0.8.tar` & `package_auto_assembler-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:58:49.660907 package_auto_assembler-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-25 00:55:40.000000 package_auto_assembler-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25016 2024-04-25 00:58:49.660907 package_auto_assembler-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-25 00:55:40.000000 package_auto_assembler-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:58:49.656907 package_auto_assembler-0.0.8/package_auto_assembler/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:58:44.000000 package_auto_assembler-0.0.8/package_auto_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56391 2024-04-25 00:58:44.000000 package_auto_assembler-0.0.8/package_auto_assembler/package_auto_assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:58:49.660907 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25016 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:58:49.660907 package_auto_assembler-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:30:07.334751 package_auto_assembler-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 02:25:43.000000 package_auto_assembler-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25416 2024-04-27 02:30:07.334751 package_auto_assembler-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-27 02:25:43.000000 package_auto_assembler-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:30:07.334751 package_auto_assembler-0.0.9/package_auto_assembler/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 02:30:02.000000 package_auto_assembler-0.0.9/package_auto_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60610 2024-04-27 02:30:02.000000 package_auto_assembler-0.0.9/package_auto_assembler/package_auto_assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-27 02:30:06.000000 package_auto_assembler-0.0.9/package_auto_assembler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:30:07.334751 package_auto_assembler-0.0.9/package_auto_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25416 2024-04-27 02:30:07.000000 package_auto_assembler-0.0.9/package_auto_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-27 02:30:07.000000 package_auto_assembler-0.0.9/package_auto_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 02:30:07.000000 package_auto_assembler-0.0.9/package_auto_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-27 02:30:07.000000 package_auto_assembler-0.0.9/package_auto_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 02:30:07.000000 package_auto_assembler-0.0.9/package_auto_assembler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 02:30:07.334751 package_auto_assembler-0.0.9/setup.cfg
```

### Comparing `package_auto_assembler-0.0.8/LICENSE` & `package_auto_assembler-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.0.8/PKG-INFO` & `package_auto_assembler-0.0.9/package_auto_assembler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: package_auto_assembler
-Version: 0.0.8
+Name: package-auto-assembler
+Version: 0.0.9
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -165,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-04-25 00:58:46</td>
+      <td>2024-04-27 02:30:03</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-04-25 00:58:46</td>
+      <td>2024-04-27 02:30:03</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-04-25 00:58:46</td>
+      <td>2024-04-27 02:30:03</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -839,29 +839,44 @@
     # name of label in commit message [example_module] for filter
     label_name = 'example_module',
     # new version to be used in release notes
     version = '0.0.2'
 )
 ```
 
+    No relevant commit messages found!
+
+
+    ..trying depth 2 !
+
+
+    No relevant commit messages found!
+
+
     No messages to clean were provided
 
 
 ##### - overwritting commit messages fro example
 
 
 ```python
 # commit messages from last merge
 rnh.commit_messages
 ```
 
 
 
 
-    ['Update README', 'Update requirements']
+    ['Update README',
+     'Update requirements',
+     '[package_auto_assembler] fetching more of commit history for ReleaseNotesHandler',
+     'Update requirements',
+     '[package_auto_assember] minor fixes to ReleaseNotesHandler; initial changes to allow for test install capability',
+     'Update README',
+     'Update requirements']
 
 
 
 
 ```python
 example_commit_messages = [
     '[example_module] usage example for initial release notes; bugfixes for RNH',
```

### Comparing `package_auto_assembler-0.0.8/README.md` & `package_auto_assembler-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.0.8/package_auto_assembler/package_auto_assembler.py` & `package_auto_assembler-0.0.9/package_auto_assembler/package_auto_assembler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1205,16 +1205,18 @@
 @attr.s
 class ReleaseNotesHandler:
 
     # inputs
     filepath = attr.ib(default='release_notes.md', type=str)
     label_name = attr.ib(default=None, type=list)
     version = attr.ib(default='0.0.1', type=str)
+    max_search_depth = attr.ib(default=2, type=int)
 
     # processed
+    n_last_messages = attr.ib(default=1, type=int)
     existing_contents = attr.ib(default=None, type=list)
     commit_messages = attr.ib(default=None, type=list)
     filtered_messages = attr.ib(default=None, type=list)
     processed_messages = attr.ib(default=None, type=list)
     processed_note_entries  = attr.ib(default=None, type=list)
 
 
@@ -1247,23 +1249,23 @@
         if self.logger is None:
             logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
             logger = logging.getLogger(self.logger_name)
             logger.setLevel(self.loggerLvl)
 
             self.logger = logger
 
-    def _get_commits_since_last_merge(self):
+    def _get_commits_since_last_merge(self, n_last_messages : int = 1):
 
         # First, find the last merge commit
-        find_merge_command = ["git", "log", "--merges", "--format=%H", "-n", "1"]
+        find_merge_command = ["git", "log", "--merges", "--format=%H", "-n", str(n_last_messages)]
         merge_result = subprocess.run(find_merge_command, capture_output=True, text=True)
         if merge_result.returncode != 0:
             raise Exception("Failed to find last merge commit")
 
-        last_merge_commit_hash = merge_result.stdout.strip()
+        last_merge_commit_hash = merge_result.stdout.strip().split("\n")[n_last_messages-1]
         if not last_merge_commit_hash:
             raise Exception("No merge commits found")
 
         # Now, get all commits after the last merge commit
         log_command = ["git", "log", f"{last_merge_commit_hash}..HEAD", "--no-merges", "--format=%s"]
         log_result = subprocess.run(log_command, capture_output=True, text=True)
         if log_result.returncode != 0:
@@ -1287,14 +1289,24 @@
         # This pattern will match messages that start with optional spaces, followed by [<package_name>],
         # possibly surrounded by spaces, and then any text. It is case-sensitive.
         pattern = re.compile(rf'\s*\[\s*{re.escape(label_name)}\s*\].*')
 
         # Filter messages that match the pattern
         filtered_messages = [msg for msg in commit_messages if pattern.search(msg)]
 
+        if filtered_messages == []:
+            self.n_last_messages += 1
+            self.logger.warning(f"No relevant commit messages found!")
+            if self.n_last_messages <= self.max_search_depth:
+                self.logger.warning(f"..trying depth {self.n_last_messages} !")
+                self._get_commits_since_last_merge(n_last_messages = self.n_last_messages)
+                self._filter_commit_messages_by_package(
+                    label_name = label_name)
+                filtered_messages = self.filtered_messages
+
         self.filtered_messages = filtered_messages
 
 
     def _clean_and_split_commit_messages(self,
                                          commit_messages : list = None):
 
         if commit_messages is None:
@@ -1322,15 +1334,17 @@
 
     def _create_release_note_entry(self,
                                   existing_contents : str = None,
                                   version : str = None,
                                   new_messages : list = None):
 
         if existing_contents is None:
-            existing_contents = self.existing_contents.copy()
+            if self.existing_contents is not None:
+                existing_contents = self.existing_contents.copy()
+
 
         if version is None:
             version = self.version
 
         if new_messages is None:
             new_messages = self.processed_messages
 
@@ -1373,33 +1387,32 @@
                 content = file.readlines()
         else:
             # No existing file, start with empty contents
             content = None
 
         return content
 
-
     def save_release_notes(self,
                            filepath : str = None,
                            note_entries : str = None):
 
         """
         Save updated release notes content.
         """
 
         if filepath is None:
             filepath = self.filepath
 
         if note_entries is None:
             note_entries = self.processed_note_entries
 
-
-        # Write the updated or new contents back to the file
-        with open(filepath, 'w') as file:
-            file.writelines(note_entries)
+        if self.processed_messages != []:
+            # Write the updated or new contents back to the file
+            with open(filepath, 'w') as file:
+                file.writelines(note_entries)
 
 @attr.s
 class PackageAutoAssembler:
     # pylint: disable=too-many-instance-attributes
 
     ## inputs
     module_name = attr.ib(type=str)
@@ -1426,35 +1439,45 @@
     requirements_list = attr.ib(default=[])
     execute_readme_notebook = attr.ib(default=True, type = bool)
     python_version = attr.ib(default="3.8")
     version_increment_type = attr.ib(default="patch", type = str)
     default_version = attr.ib(default="0.0.1", type = str)
     kernel_name = attr.ib(default = 'python', type = str)
 
+    ## handler classes
+    setup_dir_h_class = attr.ib(default=SetupDirHandler)
+    version_h_class = attr.ib(default=VersionHandler)
+    import_mapping_h_class = attr.ib(default=ImportMappingHandler)
+    local_dependacies_h_class = attr.ib(default=LocalDependaciesHandler)
+    requirements_h_class = attr.ib(default=RequirementsHandler)
+    metadata_h_class = attr.ib(default=MetadataHandler)
+    long_doc_h_class = attr.ib(default=LongDocHandler)
+
     ## handlers
-    setup_dir_h = attr.ib(default=SetupDirHandler)
-    version_h = attr.ib(default=VersionHandler)
-    import_mapping_h = attr.ib(default=ImportMappingHandler)
-    local_dependacies_h = attr.ib(default=LocalDependaciesHandler)
-    requirements_h = attr.ib(default=RequirementsHandler)
-    metadata_h = attr.ib(default=MetadataHandler)
-    long_doc_h = attr.ib(default=LongDocHandler)
+    setup_dir_h = attr.ib(default = None, type = SetupDirHandler)
+    version_h = attr.ib(default = None, type = VersionHandler)
+    import_mapping_h = attr.ib(default = None, type=ImportMappingHandler)
+    local_dependacies_h = attr.ib(default = None, type=LocalDependaciesHandler)
+    requirements_h = attr.ib(default = None, type=RequirementsHandler)
+    metadata_h = attr.ib(default = None, type=MetadataHandler)
+    long_doc_h = attr.ib(default = None, type=LongDocHandler)
 
     ## output
     package_result = attr.ib(init=False)
     metadata = attr.ib(init=False)
 
     logger = attr.ib(default=None)
     logger_name = attr.ib(default='Package Auto Assembler')
     loggerLvl = attr.ib(default=logging.INFO)
     logger_format = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         self._initialize_logger()
-        self._initialize_handlers()
+        #self._initialize_handlers()
+        self._initialize_import_mapping_handler()
 
 
     def _initialize_logger(self):
 
         """
         Initialize a logger for the class instance based on the specified logging level and logger name.
         """
@@ -1462,14 +1485,87 @@
         if self.logger is None:
             logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
             logger = logging.getLogger(self.logger_name)
             logger.setLevel(self.loggerLvl)
 
             self.logger = logger
 
+    def _initialize_metadata_handler(self):
+
+        """
+        Initialize metadata handler with available parameters.
+        """
+
+        self.metadata_h = self.metadata_h_class(
+            module_filepath = self.module_filepath)
+
+    def _initialize_version_handler(self):
+
+        """
+        Initialize version handler with available parameters.
+        """
+
+        self.version_h = self.version_h_class(
+            versions_filepath = self.versions_filepath,
+            log_filepath = self.log_filepath,
+            default_version = self.default_version)
+
+    def _initialize_requirements_handler(self):
+
+        """
+        Initialize requirements handler with available parameters.
+        """
+
+        self.requirements_h = self.requirements_h_class(
+            module_filepath = self.module_filepath,
+            custom_modules_filepath = self.dependencies_dir,
+            python_version = self.python_version)
+
+    def _initialize_import_mapping_handler(self):
+
+        """
+        Initialize import mapping handler with available parameters.
+        """
+
+        self.import_mapping_h = self.import_mapping_h_class(
+            mapping_filepath = self.mapping_filepath)
+
+    def _initialize_local_dependacies_handler(self):
+
+        """
+        Initialize local dependanies handler with available parameters.
+        """
+
+        self.local_dependacies_h = self.local_dependacies_h_class(
+            main_module_filepath = self.module_filepath,
+            dependencies_dir = self.dependencies_dir)
+
+    def _initialize_long_doc_handler(self):
+
+        """
+        Initialize long doc handler with available parameters.
+        """
+
+        self.long_doc_h = self.long_doc_h_class(
+            notebook_path = self.example_notebook_path,
+            kernel_name = self.kernel_name)
+
+    def _initialize_setup_dir_handler(self):
+
+        """
+        Initialize setup dir handler with available parameters.
+        """
+
+        self.setup_dir_h = self.setup_dir_h_class(
+            module_name = self.module_name,
+            module_filepath = self.module_filepath,
+            setup_directory = self.setup_directory,
+            logger = self.logger)
+
+
     def _initialize_handlers(self):
 
         """
         Initialize handlers with available parameters.
         """
 
         self.metadata_h = self.metadata_h(module_filepath = self.module_filepath)
@@ -1499,14 +1595,17 @@
 
     def add_metadata_from_module(self, module_filepath : str = None):
 
         """
         Add metadata extracted from the module.
         """
 
+        if self.metadata_h is None:
+            self._initialize_metadata_handler()
+
         if module_filepath is None:
             module_filepath = self.module_filepath
 
         # extracting package metadata
         self.metadata = self.metadata_h.get_package_metadata(module_filepath = module_filepath)
 
 
@@ -1517,14 +1616,17 @@
                               versions_filepath : str = None,
                               log_filepath : str = None):
 
         """
         Increment version and creates entry in version logs.
         """
 
+        if self.version_h is None:
+            self._initialize_version_handler()
+
         if module_name is None:
             module_name = self.module_name
 
         if version_increment_type is None:
             version_increment_type = self.version_increment_type
 
         if version is None:
@@ -1544,14 +1646,17 @@
 
     def prep_setup_dir(self):
 
         """
         Prepare setup directory.
         """
 
+        if self.setup_dir_h is None:
+            self._initialize_setup_dir_handler()
+
         # create empty dir for setup
         self.setup_dir_h.flush_n_make_setup_dir()
         # copy module to dir
         self.setup_dir_h.copy_module_to_setup_dir()
         # create init file for new package
         self.setup_dir_h.create_init_file()
 
@@ -1561,14 +1666,17 @@
                                 dependencies_dir : str = None,
                                 save_filepath : str = None):
 
         """
         Combine local dependacies and main module into one file.
         """
 
+        if self.local_dependacies_h is None:
+            self._initialize_local_dependacies_handler()
+
         if main_module_filepath is None:
             main_module_filepath = self.module_filepath
 
         if dependencies_dir is None:
             dependencies_dir = self.dependencies_dir
 
         if save_filepath is None:
@@ -1588,14 +1696,17 @@
                                      module_filepath : str = None,
                                      import_mappings : str = None):
 
         """
         Extract and add requirements from the module.
         """
 
+        if self.requirements_h is None:
+            self._initialize_requirements_handler()
+
         if module_filepath is None:
             module_filepath = self.module_filepath
 
         if import_mappings is None:
 
             if self.mapping_filepath is None:
                 import_mappings = {}
@@ -1616,14 +1727,17 @@
                     output_path : str = None,
                     execute_notebook : bool = None):
 
         """
         Make README file based on usage example.
         """
 
+        if self.long_doc_h is None:
+            self._initialize_long_doc_handler()
+
         if example_notebook_path is None:
             example_notebook_path = self.example_notebook_path
 
         if output_path is None:
             output_path = os.path.join(self.setup_directory,
                                        "README.md")
 
@@ -1647,14 +1761,17 @@
                        requirements : str = None,
                        classifiers : list = None):
 
         """
         Assemble setup.py file.
         """
 
+        if self.setup_dir_h is None:
+            self._initialize_setup_dir_handler()
+
         if metadata is None:
             metadata = self.metadata
 
         if requirements is None:
             requirements = self.requirements_list
 
         if classifiers is None:
```

### Comparing `package_auto_assembler-0.0.8/package_auto_assembler/setup.py` & `package_auto_assembler-0.0.9/package_auto_assembler/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="package_auto_assembler",
     packages=["package_auto_assembler"],
-    install_requires=['### package_auto_assembler.py', 'attrs>=22.2.0', 'pandas', 'pyyaml', 'stdlib-list', 'nbconvert', 'nbformat'],
+    install_requires=['### package_auto_assembler.py', 'stdlib-list', 'nbconvert', 'attrs>=22.2.0', 'pandas', 'pyyaml', 'nbformat'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.0.8"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.0.9"
 )
```

### Comparing `package_auto_assembler-0.0.8/package_auto_assembler.egg-info/PKG-INFO` & `package_auto_assembler-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: package-auto-assembler
-Version: 0.0.8
+Name: package_auto_assembler
+Version: 0.0.9
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -165,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-04-25 00:58:46</td>
+      <td>2024-04-27 02:30:03</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-04-25 00:58:46</td>
+      <td>2024-04-27 02:30:03</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-04-25 00:58:46</td>
+      <td>2024-04-27 02:30:03</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -839,29 +839,44 @@
     # name of label in commit message [example_module] for filter
     label_name = 'example_module',
     # new version to be used in release notes
     version = '0.0.2'
 )
 ```
 
+    No relevant commit messages found!
+
+
+    ..trying depth 2 !
+
+
+    No relevant commit messages found!
+
+
     No messages to clean were provided
 
 
 ##### - overwritting commit messages fro example
 
 
 ```python
 # commit messages from last merge
 rnh.commit_messages
 ```
 
 
 
 
-    ['Update README', 'Update requirements']
+    ['Update README',
+     'Update requirements',
+     '[package_auto_assembler] fetching more of commit history for ReleaseNotesHandler',
+     'Update requirements',
+     '[package_auto_assember] minor fixes to ReleaseNotesHandler; initial changes to allow for test install capability',
+     'Update README',
+     'Update requirements']
 
 
 
 
 ```python
 example_commit_messages = [
     '[example_module] usage example for initial release notes; bugfixes for RNH',
```

