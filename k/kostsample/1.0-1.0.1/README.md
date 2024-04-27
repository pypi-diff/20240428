# Comparing `tmp/kostsample-1.0.tar.gz` & `tmp/kostsample-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kostsample-1.0.tar", last modified: Sat Apr 27 11:18:24 2024, max compression
+gzip compressed data, was "kostsample-1.0.1.tar", last modified: Sat Apr 27 22:39:05 2024, max compression
```

## Comparing `kostsample-1.0.tar` & `kostsample-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 vkostyre   (501) staff       (20)        0 2024-04-27 11:18:24.889982 kostsample-1.0/
--rw-r--r--   0 vkostyre   (501) staff       (20)     1099 2024-04-27 10:48:36.000000 kostsample-1.0/LICENSE.md
--rw-r--r--   0 vkostyre   (501) staff       (20)     4213 2024-04-27 11:18:24.889262 kostsample-1.0/PKG-INFO
--rw-r--r--   0 vkostyre   (501) staff       (20)     3866 2024-04-27 11:11:57.000000 kostsample-1.0/README.md
-drwxr-xr-x   0 vkostyre   (501) staff       (20)        0 2024-04-27 11:18:24.885291 kostsample-1.0/kostsample/
--rw-r--r--   0 vkostyre   (501) staff       (20)        0 2024-04-27 10:48:36.000000 kostsample-1.0/kostsample/__init__.py
--rw-r--r--   0 vkostyre   (501) staff       (20)       38 2024-04-27 10:48:36.000000 kostsample-1.0/kostsample/main.py
-drwxr-xr-x   0 vkostyre   (501) staff       (20)        0 2024-04-27 11:18:24.888321 kostsample-1.0/kostsample.egg-info/
--rw-r--r--   0 vkostyre   (501) staff       (20)     4213 2024-04-27 11:18:24.000000 kostsample-1.0/kostsample.egg-info/PKG-INFO
--rw-r--r--   0 vkostyre   (501) staff       (20)      244 2024-04-27 11:18:24.000000 kostsample-1.0/kostsample.egg-info/SOURCES.txt
--rw-r--r--   0 vkostyre   (501) staff       (20)        1 2024-04-27 11:18:24.000000 kostsample-1.0/kostsample.egg-info/dependency_links.txt
--rw-r--r--   0 vkostyre   (501) staff       (20)       48 2024-04-27 11:18:24.000000 kostsample-1.0/kostsample.egg-info/entry_points.txt
--rw-r--r--   0 vkostyre   (501) staff       (20)       11 2024-04-27 11:18:24.000000 kostsample-1.0/kostsample.egg-info/top_level.txt
--rw-r--r--   0 vkostyre   (501) staff       (20)       38 2024-04-27 11:18:24.890228 kostsample-1.0/setup.cfg
--rw-r--r--   0 vkostyre   (501) staff       (20)      773 2024-04-27 11:18:20.000000 kostsample-1.0/setup.py
+drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-27 22:39:05.469819 kostsample-1.0.1/
+-rw-r--r--   0 jenkins    (117) jenkins    (123)     5189 2024-04-27 22:39:05.469819 kostsample-1.0.1/PKG-INFO
+-rw-r--r--   0 jenkins    (117) jenkins    (123)     3866 2024-04-27 19:40:14.000000 kostsample-1.0.1/README.md
+drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-27 22:39:05.469819 kostsample-1.0.1/kostsample/
+-rw-r--r--   0 jenkins    (117) jenkins    (123)        0 2024-04-27 19:40:14.000000 kostsample-1.0.1/kostsample/__init__.py
+-rw-r--r--   0 jenkins    (117) jenkins    (123)       38 2024-04-27 19:40:14.000000 kostsample-1.0.1/kostsample/main.py
+drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-27 22:39:05.469819 kostsample-1.0.1/kostsample.egg-info/
+-rw-r--r--   0 jenkins    (117) jenkins    (123)     5189 2024-04-27 22:39:05.000000 kostsample-1.0.1/kostsample.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (117) jenkins    (123)      233 2024-04-27 22:39:05.000000 kostsample-1.0.1/kostsample.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (117) jenkins    (123)        1 2024-04-27 22:39:05.000000 kostsample-1.0.1/kostsample.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (117) jenkins    (123)       49 2024-04-27 22:39:05.000000 kostsample-1.0.1/kostsample.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (117) jenkins    (123)       11 2024-04-27 22:39:05.000000 kostsample-1.0.1/kostsample.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (117) jenkins    (123)       38 2024-04-27 22:39:05.469819 kostsample-1.0.1/setup.cfg
+-rw-r--r--   0 jenkins    (117) jenkins    (123)      775 2024-04-27 20:57:41.000000 kostsample-1.0.1/setup.py
```

### Comparing `kostsample-1.0/PKG-INFO` & `kostsample-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: kostsample
-Version: 1.0
-Summary: python-sample-app is a starter template for new python applications
-Home-page: https://github.com/becosta/python-sample-app
-Author: Benjamin Costa & Vitalii Kostyreva
-Author-email: kostyreva-09876@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Python Sample App
 
 [Python Sample App](https://github.com/becosta/python-sample-app) is a starter template for new python applications.
 You can clone it, edit some basic stuff and get started on your new app.
 
 ## Installing
```

### Comparing `kostsample-1.0/kostsample.egg-info/PKG-INFO` & `kostsample-1.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,132 +1,132 @@
 Metadata-Version: 2.1
 Name: kostsample
-Version: 1.0
+Version: 1.0.1
 Summary: python-sample-app is a starter template for new python applications
 Home-page: https://github.com/becosta/python-sample-app
 Author: Benjamin Costa & Vitalii Kostyreva
 Author-email: kostyreva-09876@gmail.com
 License: MIT
+Description: # Python Sample App
+        
+        [Python Sample App](https://github.com/becosta/python-sample-app) is a starter template for new python applications.
+        You can clone it, edit some basic stuff and get started on your new app.
+        
+        ## Installing
+        
+        First set some variables:
+        ```sh
+        your_project_name=<project_name>
+        your_main_package_name=<main_package_name>
+        ```
+        
+        Then clone or download this repository:
+        ```sh
+        $ git clone https://github.com/becosta/python-sample-app.git
+        $ rm -rf python-sample-app/.git/
+        ```
+        Or:
+        ```sh
+        $ curl -LkSs https://api.github.com/repos/becosta/python-sample-app/tarball | tar -xvzp -C . ; mv becosta-python-sample-app-* python-sample-app
+        ```
+        
+        Next thing to do is to rename the project directory (python-sample-app) to your project's name.
+        ```sh
+        $ mv python-sample-app ${your_project_name} && cd ${your_project_name}
+        ```
+        
+        Then you can move on to renaming the main package directory (python_sample_app).
+        ```sh
+        $ mv kostsample ${your_main_package_name}
+        ```
+        
+        ## Application layout
+        
+        Your new application layout is as following:
+        ```
+        python-sample-app
+        ├── apidoc/
+        |   └── .gitkeep
+        ├── dist/
+        |   └── .gitkeep
+        ├── doc/
+        |   └── .gitkeep
+        ├── python_sample_app/
+        |   ├── test/
+        |   |   └── __init__.py
+        |   ├── __init__.py
+        |   └── main.py
+        ├── scripts/
+        |   └── .gitkeep
+        ├── .gitignore
+        ├── LICENSE.md
+        ├── README.md
+        └── setup.py
+        ```
+        
+        ## Editing to match your project needs
+        
+        After this you need to edit setup.py: ```$ editor setup.py```
+        ```python
+        name='<your_project>',
+        version='<your_project_version>',
+        description='<your_project_description>',
+        author='<your_name>',
+        author_email='<you@example.com>',
+        license="<your_project_license>",
+        url="<your_project_url>",
+        packages=['<your_project_main_package>'],
+        entry_points={
+                'console_scripts': [
+                    '<your_command>=<your_project_main_package>.main:main',
+                ],
+        },
+        ```
+        Note that ```<your_command>``` is the name of the entry script that will be generated by ```$ pip install -e .```. In other words this is the name of the command you'll use to call your application from the console later on. Also, note that you can have more than one entry point [see the setuptools documentation](https://setuptools.readthedocs.io/en/latest/setuptools.html#dynamic-discovery-of-services-and-plugins) for more information.
+        
+        Once done, edit ```LICENSE.md```, ```README.md``` and ```.gitignore``` according to your needs. If you don't need any of the ```apidoc```, ```dist```, ```doc``` and ```scripts``` directories you should remove them now.
+        
+        Finally you can create your git repository, install your project locally and run it:
+        ```sh
+        $ git init && git add .
+        $ git commit -m "Iniatial commit"
+        $ pip install -e .
+        $ <your_command>
+        Hello World!
+        $
+        ```
+        
+        ## Start coding
+        
+        To get started, create a module in ```${your_project_name}/${your_main_package_name}``` and call it in ```${your_project_name}/${your_main_package_name}/main.py```.
+        
+        A simple example would be :
+        ```python
+        ## ${your_project_name}/${your_main_package_name}/application.py
+        def class Application:
+            def run(self):
+                print("Hello World! From module application.")
+        
+        
+        # ${your_project_name}/${your_main_package_name}/main.py
+        import <your_main_package_name>.application
+        def main():
+            <your_main_package_name>.application.Application().run()
+        ```
+        
+        You can then add more modules, either as simple as a flat file like application.py or more complex with a full directory tree.
+        
+        ## Distributing your project
+        
+        You can easily distribute your project to [PyPi](https://pypi.python.org/pypi)
+        
+        Once you have created an account on PyPi, a pretty basic example would be:
+        ```sh
+        pip install twine
+        python setup.py sdist
+        twine upload dist/*
+        ```
+        
+        See the [PyPi tutorial](https://wiki.python.org/moin/CheeseShopTutorial#Submitting_Packages_to_the_Package_Index) for more information
+        
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Python Sample App
-
-[Python Sample App](https://github.com/becosta/python-sample-app) is a starter template for new python applications.
-You can clone it, edit some basic stuff and get started on your new app.
-
-## Installing
-
-First set some variables:
-```sh
-your_project_name=<project_name>
-your_main_package_name=<main_package_name>
-```
-
-Then clone or download this repository:
-```sh
-$ git clone https://github.com/becosta/python-sample-app.git
-$ rm -rf python-sample-app/.git/
-```
-Or:
-```sh
-$ curl -LkSs https://api.github.com/repos/becosta/python-sample-app/tarball | tar -xvzp -C . ; mv becosta-python-sample-app-* python-sample-app
-```
-
-Next thing to do is to rename the project directory (python-sample-app) to your project's name.
-```sh
-$ mv python-sample-app ${your_project_name} && cd ${your_project_name}
-```
-
-Then you can move on to renaming the main package directory (python_sample_app).
-```sh
-$ mv kostsample ${your_main_package_name}
-```
-
-## Application layout
-
-Your new application layout is as following:
-```
-python-sample-app
-├── apidoc/
-|   └── .gitkeep
-├── dist/
-|   └── .gitkeep
-├── doc/
-|   └── .gitkeep
-├── python_sample_app/
-|   ├── test/
-|   |   └── __init__.py
-|   ├── __init__.py
-|   └── main.py
-├── scripts/
-|   └── .gitkeep
-├── .gitignore
-├── LICENSE.md
-├── README.md
-└── setup.py
-```
-
-## Editing to match your project needs
-
-After this you need to edit setup.py: ```$ editor setup.py```
-```python
-name='<your_project>',
-version='<your_project_version>',
-description='<your_project_description>',
-author='<your_name>',
-author_email='<you@example.com>',
-license="<your_project_license>",
-url="<your_project_url>",
-packages=['<your_project_main_package>'],
-entry_points={
-        'console_scripts': [
-            '<your_command>=<your_project_main_package>.main:main',
-        ],
-},
-```
-Note that ```<your_command>``` is the name of the entry script that will be generated by ```$ pip install -e .```. In other words this is the name of the command you'll use to call your application from the console later on. Also, note that you can have more than one entry point [see the setuptools documentation](https://setuptools.readthedocs.io/en/latest/setuptools.html#dynamic-discovery-of-services-and-plugins) for more information.
-
-Once done, edit ```LICENSE.md```, ```README.md``` and ```.gitignore``` according to your needs. If you don't need any of the ```apidoc```, ```dist```, ```doc``` and ```scripts``` directories you should remove them now.
-
-Finally you can create your git repository, install your project locally and run it:
-```sh
-$ git init && git add .
-$ git commit -m "Iniatial commit"
-$ pip install -e .
-$ <your_command>
-Hello World!
-$
-```
-
-## Start coding
-
-To get started, create a module in ```${your_project_name}/${your_main_package_name}``` and call it in ```${your_project_name}/${your_main_package_name}/main.py```.
-
-A simple example would be :
-```python
-## ${your_project_name}/${your_main_package_name}/application.py
-def class Application:
-    def run(self):
-        print("Hello World! From module application.")
-
-
-# ${your_project_name}/${your_main_package_name}/main.py
-import <your_main_package_name>.application
-def main():
-    <your_main_package_name>.application.Application().run()
-```
-
-You can then add more modules, either as simple as a flat file like application.py or more complex with a full directory tree.
-
-## Distributing your project
-
-You can easily distribute your project to [PyPi](https://pypi.python.org/pypi)
-
-Once you have created an account on PyPi, a pretty basic example would be:
-```sh
-pip install twine
-python setup.py sdist
-twine upload dist/*
-```
-
-See the [PyPi tutorial](https://wiki.python.org/moin/CheeseShopTutorial#Submitting_Packages_to_the_Package_Index) for more information
```

### Comparing `kostsample-1.0/setup.py` & `kostsample-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Used in pypi.org as the README description of your package
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setup(
         name='kostsample',
-        version='1.0',
+        version='1.0.1',
         description='python-sample-app is a starter template for new python applications',
         author='Benjamin Costa & Vitalii Kostyreva',
         author_email='kostyreva-09876@gmail.com',
         license="MIT",
         url="https://github.com/becosta/python-sample-app",
         packages=['kostsample'],
         entry_points={
```

