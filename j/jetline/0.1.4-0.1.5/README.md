# Comparing `tmp/jetline-0.1.4.tar.gz` & `tmp/jetline-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetline-0.1.4.tar", last modified: Sat Apr 27 08:54:06 2024, max compression
+gzip compressed data, was "jetline-0.1.5.tar", last modified: Sun Apr 28 16:04:44 2024, max compression
```

## Comparing `jetline-0.1.4.tar` & `jetline-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-27 08:54:06.449047 jetline-0.1.4/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-27 08:54:06.448847 jetline-0.1.4/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.4/README.md
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-27 08:54:06.443811 jetline-0.1.4/jetline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/__init__.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-27 08:54:06.446287 jetline-0.1.4/jetline/commands/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/commands/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1998 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/commands/_helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10737 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/commands/analyze_project.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.4/jetline/commands/create_pipe.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/commands/info.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2866 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/commands/installer.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.4/jetline/commands/run_pipeline.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.4/jetline/commands/to_exe.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-27 08:54:06.446805 jetline-0.1.4/jetline/data/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/data/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/data/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.4/jetline/data/helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.4/jetline/logging.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-27 08:54:06.447308 jetline-0.1.4/jetline/pipeline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/pipeline/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1684 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/pipeline/node.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.4/jetline/pipeline/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-27 08:54:06.448304 jetline-0.1.4/jetline/templates/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.4/jetline/templates/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      226 2024-04-27 08:20:29.000000 jetline-0.1.4/jetline/templates/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.4/jetline/templates/main.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.4/jetline/templates/nodes.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      406 2024-04-27 08:20:10.000000 jetline-0.1.4/jetline/templates/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-27 08:54:06.448622 jetline-0.1.4/jetline.egg-info/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-27 08:54:06.000000 jetline-0.1.4/jetline.egg-info/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      776 2024-04-27 08:54:06.000000 jetline-0.1.4/jetline.egg-info/SOURCES.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-27 08:54:06.000000 jetline-0.1.4/jetline.egg-info/dependency_links.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-27 08:54:06.000000 jetline-0.1.4/jetline.egg-info/entry_points.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-27 08:54:06.000000 jetline-0.1.4/jetline.egg-info/requires.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-27 08:54:06.000000 jetline-0.1.4/jetline.egg-info/top_level.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-27 08:54:06.449094 jetline-0.1.4/setup.cfg
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1639 2024-04-27 08:54:05.000000 jetline-0.1.4/setup.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.184131 jetline-0.1.5/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:04:44.183932 jetline-0.1.5/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.5/README.md
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.178314 jetline-0.1.5/jetline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.181001 jetline-0.1.5/jetline/commands/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/commands/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1997 2024-04-28 08:26:04.000000 jetline-0.1.5/jetline/commands/_helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     4122 2024-04-26 06:00:11.000000 jetline-0.1.5/jetline/commands/create_pipe.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     9821 2024-04-28 15:55:37.000000 jetline-0.1.5/jetline/commands/create_viz.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/commands/info.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2912 2024-04-28 15:45:14.000000 jetline-0.1.5/jetline/commands/installer.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1485 2024-04-27 07:23:16.000000 jetline-0.1.5/jetline/commands/run_pipeline.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10251 2024-04-27 08:48:48.000000 jetline-0.1.5/jetline/commands/to_exe.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.181672 jetline-0.1.5/jetline/data/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/data/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     5190 2024-04-28 16:03:38.000000 jetline-0.1.5/jetline/data/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      362 2024-04-27 08:37:20.000000 jetline-0.1.5/jetline/data/helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.5/jetline/logging.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.182289 jetline-0.1.5/jetline/pipeline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/pipeline/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1717 2024-04-28 11:42:42.000000 jetline-0.1.5/jetline/pipeline/node.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-26 05:59:24.000000 jetline-0.1.5/jetline/pipeline/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.183356 jetline-0.1.5/jetline/templates/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.5/jetline/templates/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      226 2024-04-27 08:20:29.000000 jetline-0.1.5/jetline/templates/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      504 2024-04-27 07:36:36.000000 jetline-0.1.5/jetline/templates/main.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      292 2024-04-27 08:19:53.000000 jetline-0.1.5/jetline/templates/nodes.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      406 2024-04-27 08:20:10.000000 jetline-0.1.5/jetline/templates/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-28 16:04:44.183688 jetline-0.1.5/jetline.egg-info/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      771 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/SOURCES.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/dependency_links.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/entry_points.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/requires.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-28 16:04:44.000000 jetline-0.1.5/jetline.egg-info/top_level.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-28 16:04:44.184181 jetline-0.1.5/setup.cfg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1639 2024-04-28 16:04:33.000000 jetline-0.1.5/setup.py
```

### Comparing `jetline-0.1.4/PKG-INFO` & `jetline-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.4
+Version: 0.1.5
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.4/README.md` & `jetline-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jetline-0.1.4/jetline/commands/_helper.py` & `jetline-0.1.5/jetline/commands/_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 return None, None
             place_path = os.path.join(current_dir, place)
             return project_name, place_path, current_dir
     except Exception:
         raise ValueError("Project name or place is missing in the TOML file.")
 
 
-def _extract_pipeline_order(current_directory):
+def extract_pipeline_order(current_directory):
     """
     Extracts the PIPELINE_ORDER list from the content of the main file.
 
     :param current_directory: The directory of the main file.
     :return: The extracted PIPELINE_ORDER list or None if not found.
     """
     main_path = os.path.join(current_directory, 'main.py')
```

### Comparing `jetline-0.1.4/jetline/commands/create_pipe.py` & `jetline-0.1.5/jetline/commands/create_pipe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.4/jetline/commands/info.py` & `jetline-0.1.5/jetline/commands/info.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.4/jetline/commands/installer.py` & `jetline-0.1.5/jetline/commands/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import click
 import os
 import shutil
 import toml
 from pathlib import Path
 from colorama import Fore, Style
 from jetline.commands._helper import echo_jetline
+
+
 @click.command()
-@click.option('--project-name', prompt=f'{Fore.CYAN}? Project name:{Style.RESET_ALL}', default="project", help='Name of the project')
-@click.option('--pipeline-name', prompt=f'{Fore.CYAN}? Pipeline folder name:{Style.RESET_ALL}', default='pipelines', help='Name of the pipeline Folder')
+@click.option('--project-name', prompt=f'{Fore.CYAN}? Project name:{Style.RESET_ALL}', default="project",
+              help='Name of the project')
+@click.option('--pipeline-name', prompt=f'{Fore.CYAN}? Pipeline folder name:{Style.RESET_ALL}', default='pipelines',
+              help='Name of the pipeline Folder')
 def installer(project_name, pipeline_name):
     project_folder = os.path.abspath(project_name)
     os.makedirs(project_folder, exist_ok=True)
 
     click.echo(click.style("\n🚀 Setting up your project...", fg='cyan', bold=True))
 
     project_toml = {
@@ -22,58 +26,59 @@
         'locations': {
             'pipeline_folder': os.path.join(project_folder, pipeline_name),
             'main_file': os.path.join(project_folder, 'main.py'),
             'data_file': os.path.join(project_folder, 'data.py')
         }
     }
 
-
     with open(os.path.join(project_folder, 'project.toml'), 'w') as f:
         toml.dump(project_toml, f)
 
-
     init_file = os.path.join(project_folder, "__init__.py")
     Path(init_file).touch()
 
-
     templates_folder = os.path.join(os.path.dirname(__file__), '..', 'templates')
 
-
     shutil.copy(os.path.join(templates_folder, 'main.py'), project_folder)
 
     pipeline_folder = os.path.join(project_folder, pipeline_name)
     os.makedirs(pipeline_folder, exist_ok=True)
 
     shutil.copy(os.path.join(templates_folder, 'data.py'), project_folder)
 
     example_pipeline_folder = os.path.join(pipeline_folder, 'example_pipeline')
     os.makedirs(example_pipeline_folder, exist_ok=True)
 
     init_file_example = os.path.join(example_pipeline_folder, "__init__.py")
     Path(init_file_example).touch()
 
     shutil.copy(os.path.join(templates_folder, 'pipeline.py'), example_pipeline_folder)
+
     def replace_text_in_file(file_path, old_text, new_text):
         with open(file_path, 'r') as file:
             file_content = file.read()
-        
+
         file_content = file_content.replace(old_text, new_text)
-        
+
         with open(file_path, 'w') as file:
             file.write(file_content)
 
     replace_text_in_file(os.path.join(example_pipeline_folder, 'pipeline.py'), '__PIPE__', 'example_pipeline')
 
     shutil.copy(os.path.join(templates_folder, 'nodes.py'), example_pipeline_folder)
-    
 
-    click.echo(click.style("✅ Project setup complete at ", fg='green', bold=True) + click.style(project_folder, fg='white'))
+    click.echo(
+        click.style("✅ Project setup complete at ", fg='green', bold=True) + click.style(project_folder, fg='white'))
+
+    click.echo(
+        click.style(f"\nRun {Fore.YELLOW}cd {project_name}{Style.RESET_ALL} to navigate to the project directory.",
+                    fg='cyan'))
 
-    click.echo(click.style(f"\nRun {Fore.YELLOW}cd {project_name}{Style.RESET_ALL} to navigate to the project directory.", fg='cyan'))
 
 def main():
     echo_jetline()
     click.echo(f"\033[90;4mInstallation Guide:\033[0m")
     installer()
+
+
 if __name__ == '__main__':
     main()
-
```

### Comparing `jetline-0.1.4/jetline/commands/run_pipeline.py` & `jetline-0.1.5/jetline/commands/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.4/jetline/commands/to_exe.py` & `jetline-0.1.5/jetline/commands/to_exe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.4/jetline/data/data.py` & `jetline-0.1.5/jetline/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     """
     A class representing data.
 
     Attributes:
         name (str): The name of the data.
         data (Any): The actual data stored.
     """
-    def __init__(self, name, data):
-        self.name = name
+    def __init__(self, data):
         self.data = data
    
 class DataManager:
     """
     The DataManager class is responsible for managing data objects. It ensures that only a single instance of the class is created.
```

### Comparing `jetline-0.1.4/jetline/pipeline/node.py` & `jetline-0.1.5/jetline/pipeline/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,20 @@
         outputs (list or None): A list of output names for the function. If None, the node does not have outputs.
 
     Methods:
         execute(data_manager):
         Executes the function of the node using input data from the data manager. If outputs are specified, updates the data manager with the results.
 
     """
-    def __init__(self, name, function, inputs, outputs=None):
+    def __init__(self, name, function, inputs, outputs=None, viz=None):
         self.name = name
         self.function = function
         self.inputs = inputs
         self.outputs = outputs
+        self.viz = viz
 
     def execute(self, data_manager):
         """
 
         Executes the given function with the provided input data and updates the output data if specified.
 
         Parameters:
```

### Comparing `jetline-0.1.4/jetline/pipeline/pipeline.py` & `jetline-0.1.5/jetline/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.1.4/jetline.egg-info/PKG-INFO` & `jetline-0.1.5/jetline.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.1.4
+Version: 0.1.5
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jetline-0.1.4/jetline.egg-info/SOURCES.txt` & `jetline-0.1.5/jetline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 jetline.egg-info/SOURCES.txt
 jetline.egg-info/dependency_links.txt
 jetline.egg-info/entry_points.txt
 jetline.egg-info/requires.txt
 jetline.egg-info/top_level.txt
 jetline/commands/__init__.py
 jetline/commands/_helper.py
-jetline/commands/analyze_project.py
 jetline/commands/create_pipe.py
+jetline/commands/create_viz.py
 jetline/commands/info.py
 jetline/commands/installer.py
 jetline/commands/run_pipeline.py
 jetline/commands/to_exe.py
 jetline/data/__init__.py
 jetline/data/data.py
 jetline/data/helper.py
```

### Comparing `jetline-0.1.4/setup.py` & `jetline-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'vulture'
     
 
 ]
 
 setup(
     name='jetline',
-    version='0.1.4',
+    version='0.1.5',
     description='Automated Pipeline Builder',
     url='https://github.com/your_username/jetline',
     author='Johannes Kanthak',
     author_email='johannes.kanthak@kdc-solutions.de',
     license='MIT',
     classifiers=classifiers,
     keywords='pipeline automation',
```

