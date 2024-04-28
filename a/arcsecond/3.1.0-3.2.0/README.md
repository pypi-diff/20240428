# Comparing `tmp/arcsecond-3.1.0.tar.gz` & `tmp/arcsecond-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcsecond-3.1.0.tar", last modified: Fri Apr 12 06:14:13 2024, max compression
+gzip compressed data, was "arcsecond-3.2.0.tar", last modified: Sun Apr 28 20:25:30 2024, max compression
```

## Comparing `arcsecond-3.1.0.tar` & `arcsecond-3.2.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.617282 arcsecond-3.1.0/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1072 2018-07-30 07:31:57.000000 arcsecond-3.1.0/LICENSE
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-12 06:14:13.617219 arcsecond-3.1.0/PKG-INFO
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1029 2024-03-31 14:10:14.000000 arcsecond-3.1.0/README.md
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.611600 arcsecond-3.1.0/arcsecond/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      269 2024-04-12 06:13:35.000000 arcsecond-3.1.0/arcsecond/__init__.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.613875 arcsecond-3.1.0/arcsecond/api/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      203 2024-03-31 12:00:54.000000 arcsecond-3.1.0/arcsecond/api/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4643 2024-04-08 12:33:03.000000 arcsecond-3.1.0/arcsecond/api/config.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      304 2024-03-31 14:42:08.000000 arcsecond-3.1.0/arcsecond/api/constants.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4271 2024-04-12 06:06:33.000000 arcsecond-3.1.0/arcsecond/api/endpoint.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2443 2024-04-12 06:01:52.000000 arcsecond-3.1.0/arcsecond/api/main.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     6312 2024-03-31 14:44:54.000000 arcsecond-3.1.0/arcsecond/cli.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      190 2024-04-11 12:35:40.000000 arcsecond-3.1.0/arcsecond/errors.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2277 2024-03-31 14:34:46.000000 arcsecond-3.1.0/arcsecond/options.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.615688 arcsecond-3.1.0/arcsecond/uploader/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2024-03-21 21:27:31.000000 arcsecond-3.1.0/arcsecond/uploader/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1401 2024-04-11 12:56:04.000000 arcsecond-3.1.0/arcsecond/uploader/constants.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4060 2024-04-11 12:33:52.000000 arcsecond-3.1.0/arcsecond/uploader/context.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2508 2024-04-11 10:17:13.000000 arcsecond-3.1.0/arcsecond/uploader/errors.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1061 2024-04-12 06:11:19.000000 arcsecond-3.1.0/arcsecond/uploader/logger.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     5481 2024-04-12 06:04:34.000000 arcsecond-3.1.0/arcsecond/uploader/uploader.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2801 2024-03-31 07:23:32.000000 arcsecond-3.1.0/arcsecond/uploader/utils.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4079 2024-04-12 06:12:47.000000 arcsecond-3.1.0/arcsecond/uploader/walker.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.612774 arcsecond-3.1.0/arcsecond.egg-info/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/PKG-INFO
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      877 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/SOURCES.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/dependency_links.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       49 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/entry_points.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/not-zip-safe
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       55 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/requires.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       16 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/top_level.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       61 2024-04-12 06:14:13.617480 arcsecond-3.1.0/setup.cfg
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1621 2024-03-24 20:33:09.000000 arcsecond-3.1.0/setup.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.610148 arcsecond-3.1.0/tests/
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.616253 arcsecond-3.1.0/tests/cli/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.1.0/tests/cli/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1551 2024-03-31 12:07:38.000000 arcsecond-3.1.0/tests/cli/test_cli_options.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1383 2024-03-29 18:20:59.000000 arcsecond-3.1.0/tests/cli/test_config.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.616892 arcsecond-3.1.0/tests/module/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.1.0/tests/module/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1133 2024-03-29 09:03:34.000000 arcsecond-3.1.0/tests/module/test_arcsecond_root.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1092 2024-03-29 18:42:28.000000 arcsecond-3.1.0/tests/module/test_login.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-28 20:25:30.086972 arcsecond-3.2.0/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1072 2018-07-30 07:31:57.000000 arcsecond-3.2.0/LICENSE
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-28 20:25:30.086857 arcsecond-3.2.0/PKG-INFO
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1029 2024-03-31 14:10:14.000000 arcsecond-3.2.0/README.md
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-28 20:25:30.080358 arcsecond-3.2.0/arcsecond/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      412 2024-04-28 20:22:05.000000 arcsecond-3.2.0/arcsecond/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       22 2024-04-28 20:22:05.000000 arcsecond-3.2.0/arcsecond/__version__.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-28 20:25:30.082760 arcsecond-3.2.0/arcsecond/api/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      203 2024-03-31 12:00:54.000000 arcsecond-3.2.0/arcsecond/api/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4643 2024-04-08 12:33:03.000000 arcsecond-3.2.0/arcsecond/api/config.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      304 2024-03-31 14:42:08.000000 arcsecond-3.2.0/arcsecond/api/constants.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4271 2024-04-13 08:46:15.000000 arcsecond-3.2.0/arcsecond/api/endpoint.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2443 2024-04-13 08:46:15.000000 arcsecond-3.2.0/arcsecond/api/main.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     6613 2024-04-28 20:23:13.000000 arcsecond-3.2.0/arcsecond/cli.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      190 2024-04-11 12:35:40.000000 arcsecond-3.2.0/arcsecond/errors.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2277 2024-03-31 14:34:46.000000 arcsecond-3.2.0/arcsecond/options.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-28 20:25:30.084865 arcsecond-3.2.0/arcsecond/uploader/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      206 2024-04-28 20:22:10.000000 arcsecond-3.2.0/arcsecond/uploader/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1401 2024-04-11 12:56:04.000000 arcsecond-3.2.0/arcsecond/uploader/constants.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     6231 2024-04-28 20:06:47.000000 arcsecond-3.2.0/arcsecond/uploader/context.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     3392 2024-04-22 06:19:50.000000 arcsecond-3.2.0/arcsecond/uploader/errors.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1056 2024-04-22 06:03:32.000000 arcsecond-3.2.0/arcsecond/uploader/logger.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     6185 2024-04-28 20:22:21.000000 arcsecond-3.2.0/arcsecond/uploader/uploader.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     3281 2024-04-28 20:06:47.000000 arcsecond-3.2.0/arcsecond/uploader/utils.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     3881 2024-04-28 20:14:41.000000 arcsecond-3.2.0/arcsecond/uploader/walker.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-28 20:25:30.081509 arcsecond-3.2.0/arcsecond.egg-info/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-28 20:25:30.000000 arcsecond-3.2.0/arcsecond.egg-info/PKG-INFO
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      902 2024-04-28 20:25:30.000000 arcsecond-3.2.0/arcsecond.egg-info/SOURCES.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-28 20:25:30.000000 arcsecond-3.2.0/arcsecond.egg-info/dependency_links.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       49 2024-04-28 20:25:30.000000 arcsecond-3.2.0/arcsecond.egg-info/entry_points.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-28 20:25:30.000000 arcsecond-3.2.0/arcsecond.egg-info/not-zip-safe
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       55 2024-04-28 20:25:30.000000 arcsecond-3.2.0/arcsecond.egg-info/requires.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       16 2024-04-28 20:25:30.000000 arcsecond-3.2.0/arcsecond.egg-info/top_level.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       61 2024-04-28 20:25:30.087551 arcsecond-3.2.0/setup.cfg
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1624 2024-04-28 20:22:43.000000 arcsecond-3.2.0/setup.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-28 20:25:30.078217 arcsecond-3.2.0/tests/
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-28 20:25:30.085441 arcsecond-3.2.0/tests/cli/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.2.0/tests/cli/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1551 2024-03-31 12:07:38.000000 arcsecond-3.2.0/tests/cli/test_cli_options.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1383 2024-03-29 18:20:59.000000 arcsecond-3.2.0/tests/cli/test_config.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-28 20:25:30.086165 arcsecond-3.2.0/tests/module/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.2.0/tests/module/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1133 2024-03-29 09:03:34.000000 arcsecond-3.2.0/tests/module/test_arcsecond_root.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1092 2024-03-29 18:42:28.000000 arcsecond-3.2.0/tests/module/test_login.py
```

### Comparing `arcsecond-3.1.0/LICENSE` & `arcsecond-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/PKG-INFO` & `arcsecond-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcsecond
-Version: 3.1.0
+Version: 3.2.0
 Summary:  CLI for arcsecond.io
 Home-page: https://github.com/arcsecond-io/cli
 Author: Cedric Foellmi
 Author-email: cedric@arcsecond.io
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `arcsecond-3.1.0/README.md` & `arcsecond-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/arcsecond/api/config.py` & `arcsecond-3.2.0/arcsecond/api/config.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/arcsecond/api/endpoint.py` & `arcsecond-3.2.0/arcsecond/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/arcsecond/api/main.py` & `arcsecond-3.2.0/arcsecond/api/main.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/arcsecond/cli.py` & `arcsecond-3.2.0/arcsecond/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import json
 
 import click
 
 from . import __version__
 from .api import ArcsecondAPI, ArcsecondConfig
 from .options import State, basic_options
-from .uploader.context import Context
+from .uploader.context import UploadContext
 from .uploader.errors import ArcsecondError
 from .uploader.utils import display_command_summary
-from .uploader.walker import walk
+from .uploader.walker import walk_folder_and_upload
 
 pass_state = click.make_pass_decorator(State, ensure=True)
 
 VERSION_HELP_STRING = "Show the CLI version and exit."
 
 
 @click.group(invoke_without_command=True)
 @click.option('--version', is_flag=True, help=VERSION_HELP_STRING)
 @click.option('-V', is_flag=True, help=VERSION_HELP_STRING)
 @click.option('-h', is_flag=True, help="Show this message and exit.")
 @click.pass_context
 def main(ctx, version=False, v=False, h=False):
     if version or v:
-        click.echo(__version__)
+        click.echo(__version__.__version__)
     elif ctx.invoked_subcommand is None:
         click.echo(ctx.get_help())
 
 
 @main.command(help=VERSION_HELP_STRING)
 def version():
-    click.echo(__version__)
+    click.echo(__version__.__version__)
 
 
 @main.command(help='Login to your Arcsecond account.')
 @click.option('--username', required=True, nargs=1, prompt=True,
               help='Account username (without @). Primary email address is also allowed.')
 @click.option('--type', required=True, type=click.Choice(['access', 'upload'], case_sensitive=False), prompt=True,
               help='Your access key (a.k.a. API key). Visit your settings page to copy and paste it here. One of Access or Upload key must be provided.')
@@ -128,20 +128,23 @@
 
 
 @main.command(help='Upload the content of a folder.')
 @click.argument('folder', required=True, nargs=1)
 @click.option('-d', '--dataset',
               required=True, nargs=1, type=click.STRING,
               help="The UUID or name of the dataset to put data in. If new, it will be created.")
+@click.option('-t', '--telescope',
+              required=False, nargs=1, type=click.UUID,
+              help="The telescope UUID, to be attached to the dataset.")
 @click.option('-p', '--portal',
-              required=False, nargs=1,
+              required=False, nargs=1, type=click.STRING,
               help="The portal subdomain, if uploading for an Observatory Portal.")
 @basic_options
 @pass_state
-def upload(state, folder, dataset=None, portal=None):
+def upload(state, folder, dataset=None, telescope=None, portal=None):
     """
     Upload the content of a folder.
 
     You will be prompted for confirmation before the whole walking process actually
     start.
 
     Every DataFile must belong to a Dataset. If you provide a Dataset UUID, Oort will
@@ -152,14 +155,14 @@
     You can use `arcsecond datasets [OPTIONS]` to get a list of your existing datasets
     (with their UUID).
 
     Arcsecond will then start walking through the folder tree and uploads regular files
     (hidden and empty files will be skipped).
     """
     config = ArcsecondConfig(state)
-    context = Context(config, dataset_uuid_or_name=dataset, subdomain=portal)
+    context = UploadContext(config, dataset_uuid_or_name=dataset, telescope_uuid=telescope, org_subdomain=portal)
     context.validate()
 
     display_command_summary(context, [folder, ])
     ok = input('\n   ----> OK? (Press Enter) ')
     if ok.strip() == '':
-        walk(context, folder)
+        walk_folder_and_upload(context, folder)
```

### Comparing `arcsecond-3.1.0/arcsecond/options.py` & `arcsecond-3.2.0/arcsecond/options.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/arcsecond/uploader/constants.py` & `arcsecond-3.2.0/arcsecond/uploader/constants.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/arcsecond/uploader/errors.py` & `arcsecond-3.2.0/arcsecond/uploader/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,13 +67,35 @@
     def __init__(self, dataset_uuid, error_string=''):
         msg = f'Invalid / unknown dataset with UUID {dataset_uuid}.'
         if error_string:
             msg += f'\n{error_string}'
         super().__init__(msg)
 
 
+class InvalidTelescopeError(ArcsecondError):
+    def __init__(self, telescope_uuid, error_string=''):
+        msg = f'Invalid / unknown telescope with UUID {telescope_uuid}.'
+        if error_string:
+            msg += f'\n{error_string}'
+        super().__init__(msg)
+
+
+class InvalidTelescopeInDatasetError(ArcsecondError):
+    def __init__(self, telescope_uuid, dataset_telescope_uuid, dataset_uuid):
+        msg = f'Telescope {telescope_uuid} does not match with existing {dataset_telescope_uuid} in Dataset {dataset_uuid}.'
+        super().__init__(msg)
+
+
 class InvalidOrganisationDatasetError(ArcsecondError):
     def __init__(self, dataset_uuid, org_subdomain, error_string=''):
         msg = f'Dataset with UUID {dataset_uuid} unknown within organisation {org_subdomain}.'
         if error_string:
             msg += f'\n{error_string}'
         super().__init__(msg)
+
+
+class InvalidOrganisationTelescopeError(ArcsecondError):
+    def __init__(self, telescope_uuid, org_subdomain, error_string=''):
+        msg = f'Telescope with UUID {telescope_uuid} unknown within organisation {org_subdomain}.'
+        if error_string:
+            msg += f'\n{error_string}'
+        super().__init__(msg)
```

### Comparing `arcsecond-3.1.0/arcsecond/uploader/logger.py` & `arcsecond-3.2.0/arcsecond/uploader/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from datetime import datetime
 from logging import DEBUG, FileHandler, Formatter, INFO, Logger, StreamHandler, getLogger
 from pathlib import Path
 
 
-def get_oort_logger(debug=False) -> Logger:
+def get_logger(debug=False) -> Logger:
     suffix = ' (test)' if os.environ.get('OORT_TESTS') == '1' else ''
     logger = getLogger('arcsecond' + suffix)
     logger.setLevel(DEBUG if debug else INFO)
 
     if len(logger.handlers) == 0:
         formatter = Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
```

### Comparing `arcsecond-3.1.0/arcsecond/uploader/uploader.py` & `arcsecond-3.2.0/arcsecond/uploader/uploader.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import socket
 from datetime import datetime
 from pathlib import Path
 
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
 from arcsecond import ArcsecondAPI
-from arcsecond import __version__
+from arcsecond.__version__ import __version__
 from .constants import Status, Substatus
-from .context import Context
+from .context import UploadContext
 from .errors import UploadRemoteDatasetCheckError, UploadRemoteFileError, UploadRemoteFileTagsError
-from .logger import get_oort_logger
+from .logger import get_logger
 
 
 class FileUploader(object):
-    def __init__(self, context: Context, root_path: Path, file_path: Path, display_progress: bool = False):
+    def __init__(self, context: UploadContext, root_path: Path, file_path: Path, display_progress: bool = False):
         self._context = context
         self._root_path = root_path
         self._file_path = file_path
         self._display_progress = display_progress
 
-        self._logger = get_oort_logger(debug=True)
+        self._logger = get_logger(debug=True)
         self._started = None
         self._progress = 0
         self._is_test_context = bool(os.environ.get('OORT_TESTS') == '1')
         self._status = [Status.NEW, Substatus.PENDING, None]
 
         self._api = ArcsecondAPI(self._context.config, self._context.organisation_subdomain)
 
@@ -37,26 +37,37 @@
         return self._file_path.stat().st_size
 
     def _prepare_dataset(self):
         self._logger.info(f'{self.log_prefix} Preparing Dataset...')
         self._status = [Status.PREPARING, Substatus.CHECKING, None]
 
         if self._context.dataset_uuid:
-            response, error = self._api.datasets.read(self._context.dataset_uuid)
+            # Valid Dataset UUID. Dataset exists remotely. -> Read or update with Telescope.
+            if self._context._should_update_dataset_with_telescope:
+                payload = {'telescope': self._context.telescope_uuid}
+                response, error = self._api.datasets.update(self._context.dataset_uuid, payload)
+            else:
+                response, error = self._api.datasets.read(self._context.dataset_uuid)
+
             if error:
                 raise UploadRemoteDatasetCheckError(str(error))
+
             self._context.update_dataset(response)
             self._logger.info(f'{self.log_prefix} Dataset preparation done.')
 
         elif self._context.dataset_name:
-            # Dataset UUID is empty, and CLI validators have already checked this dataset doesn't exist.
-            # Simply create dataset.
-            response, error = self._api.datasets.create({'name': self._context.dataset_name})
+            # No valid Dataset UUID, only a name. Dataset does not exist remotely. Create it (possibly with Telescope).
+            payload = {'name': self._context.dataset_name}
+            if self._context._should_update_dataset_with_telescope:
+                payload.update(telescope=self._context.telescope_uuid)
+
+            response, error = self._api.datasets.create(payload)
             if error:
                 raise UploadRemoteDatasetCheckError(str(error))
+
             self._context.update_dataset(response)
             self._logger.info(f'{self.log_prefix} Dataset preparation done.')
 
         else:
             raise UploadRemoteDatasetCheckError('No dataset specified.')
 
     def __get_upload_data(self):
@@ -97,22 +108,26 @@
             self._status = [Status.ERROR, Substatus.ERROR, None]
             raise UploadRemoteFileError(f"{str(error.status)} - {str(error)}")
 
     def _update_tags(self):
         self._logger.info(f'{self.log_prefix} Updating file tags....')
         self._status = [Status.FINISHING, Substatus.TAGGING, None]
 
-        tag_root = f'oort|root|{str(self._root_path)}'
-        tag_origin = f'oort|origin|{socket.gethostname()}'
-        tag_uploader = f'oort|uploader|{self._context.config.username}'
-        tag_oort = f'oort|version|{__version__}'
+        tag_root = f'arcsecond|root|{str(self._root_path)}'
+        tag_origin = f'arcsecond|origin|{socket.gethostname()}'
+        tag_uploader = f'arcsecond|uploader|{self._context.config.username}'
+        tag_version = f'arcsecond|version|{__version__}'
+        tags = [tag_root, tag_origin, tag_uploader, tag_version]
+
+        if self._context.telescope_uuid:
+            tag_telescope = f'arcsecond|telescope|{self._context.telescope_uuid}'
+            tags.append(tag_telescope)
 
         # Tags being a list, they cannot be part of the MultipartEncoder.fields because they will
         # be interpreted as a file field tuple/list.
-        tags = [tag_root, tag_origin, tag_uploader, tag_oort]
         response, error = self._api.datafiles.update(self._datafile.get('pk'), json={'tags': tags})
         if error:
             self._status = [Status.ERROR, Substatus.ERROR, None]
             raise UploadRemoteFileTagsError(str(error))
         else:
             self._status = [Status.OK, Substatus.DONE, None]
```

### Comparing `arcsecond-3.1.0/arcsecond/uploader/utils.py` & `arcsecond-3.2.0/arcsecond/uploader/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import pathlib
 
 import click
 
-from .context import Context
+from .context import UploadContext
 
 
 def is_file_hidden(path):
     return any([part for part in path.parts if len(part) > 0 and part[0] == '.'])
 
 
 def __get_formatted_time(seconds):
@@ -34,33 +34,42 @@
         return '0 Bytes'
     k = 1024
     units = ['Bytes', 'kB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB']
     i = math.floor(math.log10(1.0 * size) / math.log10(k))
     return f"{(size / math.pow(k, i)):.2f} {units[i]}"
 
 
-def display_command_summary(context: Context, folders: list):
+def display_command_summary(context: UploadContext, folders: list):
     click.echo("\n --- Upload summary --- ")
     click.echo(f" • Arcsecond username: @{context.config.username} (Upload key: {context.config.upload_key[:4]}••••)")
     if context.organisation_subdomain:
         role = context.config.read_key(context.organisation_subdomain)
-        msg = f" • Uploading to Observatory Portal '{context.organisation_subdomain}' (as {role})."
+        msg = f" • Uploading to Observatory Portal '{context.organisation_subdomain}'."
     else:
         msg = " • Uploading to your *personal* account."
     click.echo(msg)
 
     if context.dataset_uuid and context.dataset_name:
         msg = f" • Data will be appended to existing dataset '{context.dataset_name}' ({context.dataset_uuid})."
     elif not context.dataset_uuid and context.dataset_name:
         msg = f" • Data will be inserted into a new dataset named '{context.dataset_name}'."
     else:
+        # This is not supposed to happen anymore.
         msg = " • Using folder names for dataset names (one folder = one dataset)."
     click.echo(msg)
 
-    click.echo(f" • Using API server: {context.config.api_name}")
+    if context.telescope:
+        msg = f" • Dataset will be attached to the telescope named '{context.telescope.get('name')}' ({context.telescope.get('uuid')})."
+        click.echo(msg)
+    else:
+        if not context.dataset_uuid and context.dataset_name:
+            msg = " • Dataset will not be attached to any telescope. It can be changed later in the web."
+            click.echo(msg)
+
+    click.echo(f" • Using API server: '{context.config.api_name}' ({context.config.api_server})")
     click.echo(f" • Folder{'s' if len(folders) > 1 else ''}:")
     for folder in folders:
         folder_path = pathlib.Path(folder).expanduser().resolve()
         click.echo(f"   > Path: {str(folder_path.parent if folder_path.is_file() else folder_path)}")
 
         if folder_path == pathlib.Path.home():
             click.echo("   >>> Warning: This folder is your HOME folder. <<<")
```

### Comparing `arcsecond-3.1.0/arcsecond/uploader/walker.py` & `arcsecond-3.2.0/arcsecond/uploader/walker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-import time
 from collections import Counter
 from pathlib import Path
 
 import click
 
 from .constants import Status
-from .context import Context
-from .logger import get_oort_logger
+from .context import UploadContext
+from .logger import get_logger
 from .uploader import FileUploader
 from .utils import is_file_hidden
 
 
 def __get_duplicates(values):
     dups = Counter(values) - Counter(set(values))
     return list(dups.keys())
 
 
-def __walk_first_pass(context: Context, root_path: Path):
-    logger = get_oort_logger()
+def __walk_first_pass(context: UploadContext, root_path: Path):
+    logger = get_logger()
     log_prefix = '[Walker - 1/2]'
     logger.info(f"{log_prefix} Making a first pass to collect info on files...")
-    if context.config.api_name != 'dev':
-        # For user experience, and let him/her read the above message.
-        time.sleep(3)
 
     total_file_count = sum(1 for f in root_path.glob('**/*') if f.is_file() and not is_file_hidden(f))
 
     index = 0
     file_paths = []
     for file_path in root_path.glob('**/*'):
         # Skipping both hidden files and hidden directories.
@@ -39,28 +35,26 @@
         click.echo(msg)
         file_paths.append(file_path)
 
     logger.info(f"{log_prefix} Finished collecting file info inside folder {str(root_path)}.")
     return file_paths
 
 
-def __walk_second_pass(context: Context, root_path: Path, file_paths: list):
-    logger = get_oort_logger()
+def __walk_second_pass(context: UploadContext, root_path: Path, file_paths: list):
+    logger = get_logger()
     log_prefix = '[Walker - 2/2]'
     logger.info(f"{log_prefix} Starting second pass to upload files...")
-    if context.config.api_name != 'dev':
-        time.sleep(3)
 
     uploads = {'succeeded': [], 'skipped': [], 'failed': []}
     total_file_count = len(file_paths)
 
     index = 0
     for file_path in file_paths:
         index += 1
-        click.echo(f"\n{log_prefix} File {index} / {total_file_count} ({index / total_file_count * 100:.2f}%)\n")
+        click.echo(f"{log_prefix} File {index} / {total_file_count} ({index / total_file_count * 100:.2f}%)")
 
         uploader = FileUploader(context, root_path, file_path, display_progress=True)
         status, substatus, error = uploader.upload_file()
         if status == Status.OK:
             uploads['succeeded'].append(str(file_path))
         elif status == Status.SKIPPED:
             uploads['skipped'].append((str(file_path), substatus, error))
@@ -69,16 +63,16 @@
 
     msg = f"{log_prefix}\n\nFinished upload walk inside folder {root_path} "
     logger.info(msg)
 
     return uploads
 
 
-def walk(context: Context, folder_string: str):
-    logger = get_oort_logger()
+def walk_folder_and_upload(context: UploadContext, folder_string: str):
+    logger = get_logger()
     log_prefix = '[Walker]'
     root_path = Path(folder_string).resolve()
     if root_path.is_file():  # Just in case we pass a file...
         root_path = root_path.parent
 
     logger.info(f"{log_prefix} Starting to walk through {root_path} and its subfolders...")
 
@@ -95,15 +89,15 @@
         msg += f"{', '.join(duplicates)}"
         logger.error(msg)
         logger.error(f"Exiting.")
         return
 
     uploads = __walk_second_pass(context, root_path, file_paths)
     msg = f"{log_prefix} uploads succeeded: {len(uploads['succeeded'])}, "
-    msg += f"skipped: {len(uploads['skipped'])}, failed:{len(uploads['failed'])} failed.\n"
+    msg += f"skipped: {len(uploads['skipped'])}, failed: {len(uploads['failed'])}\n"
     logger.info(msg)
 
     if len(uploads['skipped']) > 0:
         logger.error(f'{log_prefix} Here are the skipped uploads:')
         for path, substatus, error in uploads['skipped']:
             logger.warning(f'{path} ({substatus})')
```

### Comparing `arcsecond-3.1.0/arcsecond.egg-info/PKG-INFO` & `arcsecond-3.2.0/arcsecond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcsecond
-Version: 3.1.0
+Version: 3.2.0
 Summary:  CLI for arcsecond.io
 Home-page: https://github.com/arcsecond-io/cli
 Author: Cedric Foellmi
 Author-email: cedric@arcsecond.io
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `arcsecond-3.1.0/arcsecond.egg-info/SOURCES.txt` & `arcsecond-3.2.0/arcsecond.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 arcsecond/__init__.py
+arcsecond/__version__.py
 arcsecond/cli.py
 arcsecond/errors.py
 arcsecond/options.py
 arcsecond.egg-info/PKG-INFO
 arcsecond.egg-info/SOURCES.txt
 arcsecond.egg-info/dependency_links.txt
 arcsecond.egg-info/entry_points.txt
```

### Comparing `arcsecond-3.1.0/setup.py` & `arcsecond-3.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import ast
 import os
 import re
 
 from setuptools import find_packages, setup
 
 _version_re = re.compile(r'__version__\s+=\s+(.*)')
-with open('arcsecond/__init__.py', 'rb') as f:
+with open('arcsecond/__version__.py', 'rb') as f:
     __version__ = str(ast.literal_eval(_version_re.search(f.read().decode('utf-8')).group(1)))
 
 _directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
```

### Comparing `arcsecond-3.1.0/tests/cli/test_cli_options.py` & `arcsecond-3.2.0/tests/cli/test_cli_options.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/tests/cli/test_config.py` & `arcsecond-3.2.0/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/tests/module/test_arcsecond_root.py` & `arcsecond-3.2.0/tests/module/test_arcsecond_root.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.1.0/tests/module/test_login.py` & `arcsecond-3.2.0/tests/module/test_login.py`

 * *Files identical despite different names*

