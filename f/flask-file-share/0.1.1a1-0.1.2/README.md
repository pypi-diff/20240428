# Comparing `tmp/flask_file_share-0.1.1a1.tar.gz` & `tmp/flask_file_share-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_file_share-0.1.1a1.tar", max compression
+gzip compressed data, was "flask_file_share-0.1.2.tar", max compression
```

## Comparing `flask_file_share-0.1.1a1.tar` & `flask_file_share-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     7677 2024-04-21 12:43:06.110087 flask_file_share-0.1.1a1/README.md
--rw-r--r--   0        0        0     1658 2024-04-21 16:41:02.270329 flask_file_share-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0      192 2024-04-21 12:43:06.114087 flask_file_share-0.1.1a1/src/flask_file_share/__init__.py
--rw-r--r--   0        0        0      388 2024-04-21 12:43:06.114087 flask_file_share-0.1.1a1/src/flask_file_share/app.py
--rw-r--r--   0        0        0     8111 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/cli.py
--rw-r--r--   0        0        0     8013 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/client.py
--rw-r--r--   0        0        0     2218 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/main.py
--rw-r--r--   0        0        0     4301 2024-04-21 16:36:33.686754 flask_file_share-0.1.1a1/src/flask_file_share/settings.py
--rw-r--r--   0        0        0     2166 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/static/app.js
--rwxr-xr-x   0        0        0     4059 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-144-144.png
--rwxr-xr-x   0        0        0     5411 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-192-192.png
--rwxr-xr-x   0        0        0     1338 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-48-48.png
--rwxr-xr-x   0        0        0    15486 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-512-512.png
--rwxr-xr-x   0        0        0     2002 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-72-72.png
--rwxr-xr-x   0        0        0     2580 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-96-96.png
--rw-r--r--   0        0        0  1086445 2024-03-09 11:52:04.333929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/harprit-bola-239056.png
--rw-r--r--   0        0        0    39216 2024-03-09 11:52:04.333929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/harprit-bola-239056.webp
--rw-r--r--   0        0        0  1802675 2024-03-09 11:52:04.345929 flask_file_share-0.1.1a1/src/flask_file_share/static/images/kevin-bhagat-461952.jpg
--rw-r--r--   0        0        0   298842 2024-03-09 11:52:04.349930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/kevin-bhagat-461952.webp
--rw-r--r--   0        0        0   853105 2024-03-09 11:52:04.353930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/luca-bravo-272609.png
--rw-r--r--   0        0        0    43480 2024-03-09 11:52:04.353930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/luca-bravo-272609.webp
--rw-r--r--   0        0        0   769849 2024-03-09 11:52:04.357930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/marta-de-la-concepcion-97951.jpg
--rw-r--r--   0        0        0    88434 2024-03-09 11:52:04.357930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/pwa-dark.png
--rw-r--r--   0        0        0   228416 2024-03-09 11:52:04.361930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/pwa-dark@2x.png
--rw-r--r--   0        0        0    83375 2024-03-09 11:52:04.361930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/pwa-light.png
--rw-r--r--   0        0        0   217423 2024-03-09 11:52:04.361930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/pwa-light@2x.png
--rw-r--r--   0        0        0  2761711 2024-03-09 11:52:04.373930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/william-iven-8514.jpg
--rw-r--r--   0        0        0   982142 2024-03-09 11:52:04.373930 flask_file_share-0.1.1a1/src/flask_file_share/static/images/william-iven-8514.webp
--rw-r--r--   0        0        0      969 2024-03-09 11:52:04.373930 flask_file_share-0.1.1a1/src/flask_file_share/static/manifest.json
--rw-r--r--   0        0        0      882 2024-03-09 11:52:04.373930 flask_file_share-0.1.1a1/src/flask_file_share/static/offline.html
--rw-r--r--   0        0        0     4163 2023-11-24 12:38:03.787366 flask_file_share-0.1.1a1/src/flask_file_share/static/progress-bar/index-download.js
--rw-r--r--   0        0        0      645 2023-11-23 16:49:10.764578 flask_file_share-0.1.1a1/src/flask_file_share/static/progress-bar/index.css
--rw-r--r--   0        0        0     3947 2024-03-09 11:52:04.373930 flask_file_share-0.1.1a1/src/flask_file_share/static/service-worker.js
--rw-r--r--   0        0        0     1561 2023-11-23 14:35:17.557411 flask_file_share-0.1.1a1/src/flask_file_share/static/sortable-js/sortable.min.css
--rw-r--r--   0        0        0     1187 2023-11-23 14:35:17.557411 flask_file_share-0.1.1a1/src/flask_file_share/static/sortable-js/sortable.min.js
--rw-r--r--   0        0        0     3822 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/templates/index.html
--rw-r--r--   0        0        0     1937 2024-03-09 11:52:04.329929 flask_file_share-0.1.1a1/src/flask_file_share/templates/login.html
--rw-r--r--   0        0        0      172 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/utils/__init__.py
--rw-r--r--   0        0        0      599 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/utils/mimetype.py
--rw-r--r--   0        0        0      680 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/utils/slugify.py
--rw-r--r--   0        0        0      914 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/utils/zip.py
--rw-r--r--   0        0        0      390 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/web/__init__.py
--rw-r--r--   0        0        0     3451 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/web/auth.py
--rw-r--r--   0        0        0     1030 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/web/config.py
--rw-r--r--   0        0        0     8844 2024-04-21 16:37:45.119704 flask_file_share-0.1.1a1/src/flask_file_share/web/routes.py
--rw-r--r--   0        0        0     4702 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/web/utils.py
--rw-r--r--   0        0        0      944 2024-04-21 12:43:06.118087 flask_file_share-0.1.1a1/src/flask_file_share/web/views.py
--rw-r--r--   0        0        0     9090 1970-01-01 00:00:00.000000 flask_file_share-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0     7677 2024-04-21 12:43:06.110087 flask_file_share-0.1.2/README.md
+-rw-r--r--   0        0        0     1583 2024-04-28 16:49:17.960560 flask_file_share-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      192 2024-04-21 12:43:06.114087 flask_file_share-0.1.2/src/flask_file_share/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-21 21:15:49.028322 flask_file_share-0.1.2/src/flask_file_share/app.py
+-rw-r--r--   0        0        0     8267 2024-04-21 21:15:49.024322 flask_file_share-0.1.2/src/flask_file_share/cli.py
+-rw-r--r--   0        0        0     8013 2024-04-21 12:43:06.118087 flask_file_share-0.1.2/src/flask_file_share/client.py
+-rw-r--r--   0        0        0     2377 2024-04-21 21:15:49.028322 flask_file_share-0.1.2/src/flask_file_share/main.py
+-rw-r--r--   0        0        0     4336 2024-04-21 21:18:17.096066 flask_file_share-0.1.2/src/flask_file_share/settings.py
+-rw-r--r--   0        0        0     2166 2024-03-09 11:52:04.329929 flask_file_share-0.1.2/src/flask_file_share/static/app.js
+-rwxr-xr-x   0        0        0     4059 2024-03-09 11:52:04.329929 flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-144-144.png
+-rwxr-xr-x   0        0        0     5411 2024-03-09 11:52:04.329929 flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-192-192.png
+-rwxr-xr-x   0        0        0     1338 2024-03-09 11:52:04.329929 flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-48-48.png
+-rwxr-xr-x   0        0        0    15486 2024-03-09 11:52:04.329929 flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-512-512.png
+-rwxr-xr-x   0        0        0     2002 2024-03-09 11:52:04.329929 flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-72-72.png
+-rwxr-xr-x   0        0        0     2580 2024-03-09 11:52:04.329929 flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-96-96.png
+-rw-r--r--   0        0        0  1086445 2024-03-09 11:52:04.333929 flask_file_share-0.1.2/src/flask_file_share/static/images/harprit-bola-239056.png
+-rw-r--r--   0        0        0    39216 2024-03-09 11:52:04.333929 flask_file_share-0.1.2/src/flask_file_share/static/images/harprit-bola-239056.webp
+-rw-r--r--   0        0        0  1802675 2024-03-09 11:52:04.345929 flask_file_share-0.1.2/src/flask_file_share/static/images/kevin-bhagat-461952.jpg
+-rw-r--r--   0        0        0   298842 2024-03-09 11:52:04.349930 flask_file_share-0.1.2/src/flask_file_share/static/images/kevin-bhagat-461952.webp
+-rw-r--r--   0        0        0   853105 2024-03-09 11:52:04.353930 flask_file_share-0.1.2/src/flask_file_share/static/images/luca-bravo-272609.png
+-rw-r--r--   0        0        0    43480 2024-03-09 11:52:04.353930 flask_file_share-0.1.2/src/flask_file_share/static/images/luca-bravo-272609.webp
+-rw-r--r--   0        0        0   769849 2024-03-09 11:52:04.357930 flask_file_share-0.1.2/src/flask_file_share/static/images/marta-de-la-concepcion-97951.jpg
+-rw-r--r--   0        0        0    88434 2024-03-09 11:52:04.357930 flask_file_share-0.1.2/src/flask_file_share/static/images/pwa-dark.png
+-rw-r--r--   0        0        0   228416 2024-03-09 11:52:04.361930 flask_file_share-0.1.2/src/flask_file_share/static/images/pwa-dark@2x.png
+-rw-r--r--   0        0        0    83375 2024-03-09 11:52:04.361930 flask_file_share-0.1.2/src/flask_file_share/static/images/pwa-light.png
+-rw-r--r--   0        0        0   217423 2024-03-09 11:52:04.361930 flask_file_share-0.1.2/src/flask_file_share/static/images/pwa-light@2x.png
+-rw-r--r--   0        0        0  2761711 2024-03-09 11:52:04.373930 flask_file_share-0.1.2/src/flask_file_share/static/images/william-iven-8514.jpg
+-rw-r--r--   0        0        0   982142 2024-03-09 11:52:04.373930 flask_file_share-0.1.2/src/flask_file_share/static/images/william-iven-8514.webp
+-rw-r--r--   0        0        0      969 2024-03-09 11:52:04.373930 flask_file_share-0.1.2/src/flask_file_share/static/manifest.json
+-rw-r--r--   0        0        0      882 2024-03-09 11:52:04.373930 flask_file_share-0.1.2/src/flask_file_share/static/offline.html
+-rw-r--r--   0        0        0     4163 2023-11-24 12:38:03.787366 flask_file_share-0.1.2/src/flask_file_share/static/progress-bar/index-download.js
+-rw-r--r--   0        0        0      645 2023-11-23 16:49:10.764578 flask_file_share-0.1.2/src/flask_file_share/static/progress-bar/index.css
+-rw-r--r--   0        0        0     3947 2024-03-09 11:52:04.373930 flask_file_share-0.1.2/src/flask_file_share/static/service-worker.js
+-rw-r--r--   0        0        0     1561 2023-11-23 14:35:17.557411 flask_file_share-0.1.2/src/flask_file_share/static/sortable-js/sortable.min.css
+-rw-r--r--   0        0        0     1187 2023-11-23 14:35:17.557411 flask_file_share-0.1.2/src/flask_file_share/static/sortable-js/sortable.min.js
+-rw-r--r--   0        0        0     3796 2024-04-21 21:15:49.008322 flask_file_share-0.1.2/src/flask_file_share/templates/index.html
+-rw-r--r--   0        0        0     1937 2024-03-09 11:52:04.329929 flask_file_share-0.1.2/src/flask_file_share/templates/login.html
+-rw-r--r--   0        0        0      172 2024-04-21 12:43:06.118087 flask_file_share-0.1.2/src/flask_file_share/utils/__init__.py
+-rw-r--r--   0        0        0      599 2024-04-21 12:43:06.118087 flask_file_share-0.1.2/src/flask_file_share/utils/mimetype.py
+-rw-r--r--   0        0        0      823 2024-04-28 10:33:48.174944 flask_file_share-0.1.2/src/flask_file_share/utils/slugify.py
+-rw-r--r--   0        0        0      914 2024-04-21 12:43:06.118087 flask_file_share-0.1.2/src/flask_file_share/utils/zip.py
+-rw-r--r--   0        0        0      390 2024-04-21 12:43:06.118087 flask_file_share-0.1.2/src/flask_file_share/web/__init__.py
+-rw-r--r--   0        0        0     3451 2024-04-21 20:53:41.832834 flask_file_share-0.1.2/src/flask_file_share/web/auth.py
+-rw-r--r--   0        0        0     1030 2024-04-21 12:43:06.118087 flask_file_share-0.1.2/src/flask_file_share/web/config.py
+-rw-r--r--   0        0        0     8844 2024-04-21 21:16:18.711788 flask_file_share-0.1.2/src/flask_file_share/web/routes.py
+-rw-r--r--   0        0        0     4702 2024-04-21 12:43:06.118087 flask_file_share-0.1.2/src/flask_file_share/web/utils.py
+-rw-r--r--   0        0        0      944 2024-04-21 12:43:06.118087 flask_file_share-0.1.2/src/flask_file_share/web/views.py
+-rw-r--r--   0        0        0     8964 1970-01-01 00:00:00.000000 flask_file_share-0.1.2/PKG-INFO
```

### Comparing `flask_file_share-0.1.1a1/README.md` & `flask_file_share-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/pyproject.toml` & `flask_file_share-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "flask-file-share"
-version = "0.1.1a1"
+version = "0.1.2"
 description = "Flask-based file sharing with web interface, API, and CLI app"
 authors = ["hermann-web <hermannagossou6@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {from = "src", include = "flask_file_share"}
 ]
 maintainers = [
     "Hermann Agossou <agossouhermann7@gmail.com>"
 ]
-homepage = "https://hermann-web.github.io/blog/blog/2023/11/14/flask-based-file-hosting-web-app--api--python-module--cli-app"
+homepage = "https://flask-file-share.readthedocs.io"
 repository = "https://github.com/Hermann-web/simple-file-hosting-with-flask"
 documentation = "https://flask-file-share.readthedocs.io"
 keywords = ["flask", "file sharing", "web interface", "API", "CLI"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/cli.py` & `flask_file_share-0.1.2/src/flask_file_share/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,22 +79,22 @@
     try:
         yield client
     finally:
         # logout even if exception occurs in the block
         client.logout()
 
 
-def handle_login(*args, **kwargs):  # pylint: disable=W0613
+def handle_login(args, file_sharing_client: FileSharingClient):  # pylint: disable=W0613
     """
     Handle login command.
     """
     return
 
 
-def handle_logout(*args, **kwargs):  # pylint: disable=W0613
+def handle_logout(args, file_sharing_client: FileSharingClient):  # pylint: disable=W0613
     """
     Handle logout command.
     """
     return
 
 
 def handle_list(args, file_sharing_client: FileSharingClient):
@@ -192,15 +192,15 @@
     else:
         print("Invalid output path")
         return
 
     file_sharing_client.download_last_n_files(nb_files, folder, filename)
 
 
-def build_cli_parser(parser):
+def build_cli_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     """
     Build CLI parser.
 
     Parameters
     ----------
     parser : argparse.ArgumentParser
         The ArgumentParser object.
@@ -232,15 +232,15 @@
         "--order",
         choices=["asc", "desc"],
         help="Order of files to list or download",
     )
     return parser
 
 
-def parse_args():
+def parse_args() -> argparse.Namespace:
     """
     Parse CLI arguments.
 
     Returns
     -------
     argparse.Namespace
         The parsed command-line arguments.
@@ -248,15 +248,15 @@
     """
     parser = argparse.ArgumentParser(description="File sharing CLI")
     parser = build_cli_parser(parser)
     args = parser.parse_args()
     return args
 
 
-def main(args):
+def main(args: argparse.Namespace):
     """
     Main function to execute CLI commands.
 
     Parameters
     ----------
     args : argparse.Namespace
         The parsed command-line arguments.
@@ -279,15 +279,15 @@
             "download": handle_download,
             "downloadl": handle_downloadl,
         }
 
         handler = command_handlers.get(args.cli_command)
 
         if not handler:
-            raise ValueError(f"Invalid command {args.command}")
+            raise ValueError(f"Invalid command {args.cli_command}")
 
         handler(args, file_sharing_client)
 
 
 if __name__ == "__main__":
     parsed_args = parse_args()
     main(args=parsed_args)
```

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/client.py` & `flask_file_share-0.1.2/src/flask_file_share/client.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/main.py` & `flask_file_share-0.1.2/src/flask_file_share/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 Example:
     python main.py server
     python main.py cli list -u myusername -p mypassword -n 5
 """
 
 import argparse
 
+from flask_file_share.app import build_web_app_parser
 from flask_file_share.app import main as web_main
 from flask_file_share.cli import build_cli_parser
 from flask_file_share.cli import main as cli_main
 
 
 def create_parser() -> argparse.ArgumentParser:
     """
@@ -46,15 +47,18 @@
     argparse.ArgumentParser:
         The ArgumentParser object for the CLI.
     """
     parser = argparse.ArgumentParser(description="FlaskFileShare Application")
     subparsers = parser.add_subparsers(dest="command", help="Select the component to run")
 
     # Subparser for the web server
-    _ = subparsers.add_parser('server', help='Run the web server')
+    web_app_parser = subparsers.add_parser('server', help='Run the web server')
+
+    # Web-specific arguments
+    web_app_parser = build_web_app_parser(web_app_parser)
 
     # Subparser for the CLI
     cli_parser = subparsers.add_parser('cli', help='Run the CLI tool')
 
     # CLI-specific arguments
     cli_parser = build_cli_parser(cli_parser)
 
@@ -66,15 +70,15 @@
     Main function to execute the CLI.
 
     """
     parser = create_parser()
     args = parser.parse_args()
 
     if args.command == 'server':
-        web_main()
+        web_main(args)
     elif args.command == 'cli':
         # Here, you re-invoke the CLI main with the processed arguments
         cli_main(args)
     else:
         parser.print_help()
```

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/settings.py` & `flask_file_share-0.1.2/src/flask_file_share/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     load_dotenv(_DOTENV_PATH)
 else:
     logging.warning(".env file not found")
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = os.getenv("DEBUG", "True").lower() == "true"
 
-USERNAME_STR = "FM_USERNAME"
-PASSWORD_STR = "FM_PASSWORD"
-SECRET_KEY_STR = "FM_SECRET_KEY"
+USERNAME_STR = "FFS_USERNAME"
+PASSWORD_STR = "FFS_PASSWORD"
+SECRET_KEY_STR = "FFS_SECRET_KEY"
 
 # Set values for username, password, and secret key
 if not DEBUG:
     _cdt1 = USERNAME_STR in os.environ
     _cdt2 = PASSWORD_STR in os.environ
     _cdt3 = SECRET_KEY_STR in os.environ
     # Raise error if DEBUG is False and username, password, or secret key is not provided
@@ -75,15 +75,15 @@
     logging.debug("USERNAME: %s", USERNAME)
     logging.debug("PASSWORD: %s", PASSWORD)
     logging.debug("SECRET_KEY: %s", SECRET_KEY)
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent
 
-UPLOADS_DATA_DIR = Path(os.getcwd()).resolve() / "uploads"
+UPLOADS_DATA_DIR = Path(os.getenv("UPLOADS_DATA_DIR", os.getcwd() + "/uploads")).resolve()
 UPLOADS_DATA_DIR.mkdir(exist_ok=True)
 
 UPLOAD_FOLDER = Path(os.getenv("UPLOAD_FOLDER", UPLOADS_DATA_DIR / "files")).resolve()
 UPLOAD_FOLDER.mkdir(exist_ok=True)
 
 DATA_FILE = Path(os.getenv("DATA_FILE", UPLOADS_DATA_DIR / "data.json")).resolve()
 assert DATA_FILE.parent.exists()
```

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/app.js` & `flask_file_share-0.1.2/src/flask_file_share/static/app.js`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-144-144.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-144-144.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-192-192.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-192-192.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-48-48.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-48-48.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-512-512.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-512-512.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-72-72.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-72-72.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/android-launchericon-96-96.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/android-launchericon-96-96.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/harprit-bola-239056.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/harprit-bola-239056.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/harprit-bola-239056.webp` & `flask_file_share-0.1.2/src/flask_file_share/static/images/harprit-bola-239056.webp`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/kevin-bhagat-461952.jpg` & `flask_file_share-0.1.2/src/flask_file_share/static/images/kevin-bhagat-461952.jpg`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/kevin-bhagat-461952.webp` & `flask_file_share-0.1.2/src/flask_file_share/static/images/kevin-bhagat-461952.webp`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/luca-bravo-272609.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/luca-bravo-272609.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/luca-bravo-272609.webp` & `flask_file_share-0.1.2/src/flask_file_share/static/images/luca-bravo-272609.webp`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/marta-de-la-concepcion-97951.jpg` & `flask_file_share-0.1.2/src/flask_file_share/static/images/marta-de-la-concepcion-97951.jpg`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/pwa-dark.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/pwa-dark.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/pwa-dark@2x.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/pwa-dark@2x.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/pwa-light.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/pwa-light.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/pwa-light@2x.png` & `flask_file_share-0.1.2/src/flask_file_share/static/images/pwa-light@2x.png`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/william-iven-8514.jpg` & `flask_file_share-0.1.2/src/flask_file_share/static/images/william-iven-8514.jpg`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/images/william-iven-8514.webp` & `flask_file_share-0.1.2/src/flask_file_share/static/images/william-iven-8514.webp`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/manifest.json` & `flask_file_share-0.1.2/src/flask_file_share/static/manifest.json`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/offline.html` & `flask_file_share-0.1.2/src/flask_file_share/static/offline.html`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/progress-bar/index-download.js` & `flask_file_share-0.1.2/src/flask_file_share/static/progress-bar/index-download.js`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/progress-bar/index.css` & `flask_file_share-0.1.2/src/flask_file_share/static/progress-bar/index.css`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/service-worker.js` & `flask_file_share-0.1.2/src/flask_file_share/static/service-worker.js`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/sortable-js/sortable.min.css` & `flask_file_share-0.1.2/src/flask_file_share/static/sortable-js/sortable.min.css`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/static/sortable-js/sortable.min.js` & `flask_file_share-0.1.2/src/flask_file_share/static/sortable-js/sortable.min.js`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/templates/index.html` & `flask_file_share-0.1.2/src/flask_file_share/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
       href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
     />
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
 
     <!-- https://www.cssscript.com/fast-html-table-sorting/ -->
     <link
       rel="stylesheet"
-      href="{{ url_for('static', filename='progress-bar/sortable-js/sortable.min.css') }}"
+      href="{{ url_for('static', filename='sortable-js/sortable.min.css') }}"
     />
-    <script src="{{ url_for('static', filename='progress-bar/sortable-js/sortable.min.js') }}"></script>
+    <script src="{{ url_for('static', filename='sortable-js/sortable.min.js') }}"></script>
     <link
       rel="stylesheet"
       href="{{ url_for('static', filename='progress-bar/index.css') }}"
     />
     <script src="{{ url_for('static', filename='progress-bar/index-download.js') }}"></script>
     <script src="{{ url_for('static', filename='progress-bar/index-upload.js') }}"></script>
     <style>
```

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/templates/login.html` & `flask_file_share-0.1.2/src/flask_file_share/templates/login.html`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/utils/mimetype.py` & `flask_file_share-0.1.2/src/flask_file_share/utils/mimetype.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/utils/slugify.py` & `flask_file_share-0.1.2/src/flask_file_share/utils/slugify.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """
 File: slugify.py
 ----------------
 
 A utility module for slugifying filenames.
 """
 
+from pathlib import Path
+from typing import Union
 from slugify import slugify  # pylint: disable=E0401
 
 
-def slugify_filename(filename: str) -> str:
+def slugify_filepath(filename: Union[str, Path]) -> Path:
     """
     Slugify the filename.
 
     Parameters
     ----------
     filename : str
         The original filename.
 
     Returns
     -------
     str
         The slugified filename.
     """
-    # Split the filename and extension
-    _ = filename.rsplit(".", 1)
-    assert len(_) == 2
-    base, extension = _
+    filename = Path(filename)
     # Slugify the base part
-    slug_base = slugify(base)
+    slug_base = slugify(filename.stem)
+    extension = filename.suffix.lower()
     # Join the slugified base with the original extension
-    slug_filename = f"{slug_base}.{extension}"
-    return slug_filename
+    slug_filename = f"{slug_base}{extension}"
+    return filename.parent / slug_filename
+
+def slugify_filename(filename: Union[str, Path]) -> str:
+    return str(slugify_filepath(filename))
```

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/utils/zip.py` & `flask_file_share-0.1.2/src/flask_file_share/utils/zip.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/web/auth.py` & `flask_file_share-0.1.2/src/flask_file_share/web/auth.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/web/config.py` & `flask_file_share-0.1.2/src/flask_file_share/web/config.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/web/routes.py` & `flask_file_share-0.1.2/src/flask_file_share/web/routes.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/web/utils.py` & `flask_file_share-0.1.2/src/flask_file_share/web/utils.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/src/flask_file_share/web/views.py` & `flask_file_share-0.1.2/src/flask_file_share/web/views.py`

 * *Files identical despite different names*

### Comparing `flask_file_share-0.1.1a1/PKG-INFO` & `flask_file_share-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: flask-file-share
-Version: 0.1.1a1
+Version: 0.1.2
 Summary: Flask-based file sharing with web interface, API, and CLI app
-Home-page: https://hermann-web.github.io/blog/blog/2023/11/14/flask-based-file-hosting-web-app--api--python-module--cli-app
+Home-page: https://flask-file-share.readthedocs.io
 License: MIT
 Keywords: flask,file sharing,web interface,API,CLI
 Author: hermann-web
 Author-email: hermannagossou6@gmail.com
 Maintainer: Hermann Agossou
 Maintainer-email: agossouhermann7@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -14,15 +14,14 @@
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Flask (>=3.0.3,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.4,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://flask-file-share.readthedocs.io
```

