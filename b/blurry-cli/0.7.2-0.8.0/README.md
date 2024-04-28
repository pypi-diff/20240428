# Comparing `tmp/blurry_cli-0.7.2.tar.gz` & `tmp/blurry_cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blurry_cli-0.7.2.tar", max compression
+gzip compressed data, was "blurry_cli-0.8.0.tar", max compression
```

## Comparing `blurry_cli-0.7.2.tar` & `blurry_cli-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1068 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/LICENSE
--rw-r--r--   0        0        0     1782 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/README.md
--rw-r--r--   0        0        0     9864 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/__init__.py
--rw-r--r--   0        0        0       32 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/__main__.py
--rw-r--r--   0        0        0      526 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/async_typer.py
--rw-r--r--   0        0        0      872 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/cli.py
--rw-r--r--   0        0        0      111 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/constants.py
--rw-r--r--   0        0        0     3537 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/images.py
--rw-r--r--   0        0        0     7897 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/markdown/__init__.py
--rw-r--r--   0        0        0     1778 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/markdown/front_matter.py
--rw-r--r--   0        0        0        0 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/markdown/renderer_functions/__init__.py
--rw-r--r--   0        0        0      787 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/markdown/renderer_functions/render_video.py
--rw-r--r--   0        0        0     1993 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/open_graph.py
--rw-r--r--   0        0        0      273 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/html_plugins/__init__.py
--rw-r--r--   0        0        0     1124 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/html_plugins/minify_html_plugin.py
--rw-r--r--   0        0        0        0 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/markdown_plugins/__init__.py
--rw-r--r--   0        0        0     1119 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/markdown_plugins/container_plugin.py
--rw-r--r--   0        0        0      683 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/markdown_plugins/punctuation_plugin.py
--rw-r--r--   0        0        0     1509 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/markdown_plugins/python_code_plugin.py
--rw-r--r--   0        0        0        0 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/py.typed
--rw-r--r--   0        0        0     1817 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/schema_validation.py
--rw-r--r--   0        0        0     2347 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/settings.py
--rw-r--r--   0        0        0     1752 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/sitemap.py
--rw-r--r--   0        0        0      777 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/types.py
--rw-r--r--   0        0        0     4376 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/utils.py
--rw-r--r--   0        0        0     2195 2024-04-27 15:14:26.944594 blurry_cli-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 blurry_cli-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1782 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/README.md
+-rw-r--r--   0        0        0    10037 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/__main__.py
+-rw-r--r--   0        0        0      526 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/async_typer.py
+-rw-r--r--   0        0        0     1009 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/cli.py
+-rw-r--r--   0        0        0      111 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/constants.py
+-rw-r--r--   0        0        0     3537 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/images.py
+-rw-r--r--   0        0        0     7897 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/markdown/__init__.py
+-rw-r--r--   0        0        0     1778 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/markdown/front_matter.py
+-rw-r--r--   0        0        0        0 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/markdown/renderer_functions/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/markdown/renderer_functions/render_video.py
+-rw-r--r--   0        0        0     1993 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/open_graph.py
+-rw-r--r--   0        0        0      349 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/html_plugins/__init__.py
+-rw-r--r--   0        0        0     1124 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/html_plugins/minify_html_plugin.py
+-rw-r--r--   0        0        0        0 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/jinja_plugins/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/jinja_plugins/blurry_image_extension.py
+-rw-r--r--   0        0        0        0 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/markdown_plugins/__init__.py
+-rw-r--r--   0        0        0     1119 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/markdown_plugins/container_plugin.py
+-rw-r--r--   0        0        0      683 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/markdown_plugins/punctuation_plugin.py
+-rw-r--r--   0        0        0     1509 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/plugins/markdown_plugins/python_code_plugin.py
+-rw-r--r--   0        0        0        0 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/py.typed
+-rw-r--r--   0        0        0     1817 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/schema_validation.py
+-rw-r--r--   0        0        0     2347 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/settings.py
+-rw-r--r--   0        0        0     1752 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/sitemap.py
+-rw-r--r--   0        0        0      777 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/types.py
+-rw-r--r--   0        0        0     4376 2024-04-28 14:23:32.103224 blurry_cli-0.8.0/blurry/utils.py
+-rw-r--r--   0        0        0     2355 2024-04-28 14:23:32.107224 blurry_cli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 blurry_cli-0.8.0/PKG-INFO
```

### Comparing `blurry_cli-0.7.2/LICENSE` & `blurry_cli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/README.md` & `blurry_cli-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/__init__.py` & `blurry_cli-0.8.0/blurry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from blurry.cli import print_blurry_name
 from blurry.cli import print_plugin_table
 from blurry.constants import ENV_VAR_PREFIX
 from blurry.images import generate_images_for_srcset
 from blurry.markdown import convert_markdown_file_to_html
 from blurry.open_graph import open_graph_meta_tags
 from blurry.plugins import discovered_html_plugins
+from blurry.plugins import discovered_jinja_extensions
 from blurry.plugins import discovered_jinja_filter_plugins
 from blurry.schema_validation import validate_front_matter_as_schema
 from blurry.settings import get_build_directory
 from blurry.settings import get_content_directory
 from blurry.settings import get_templates_directory
 from blurry.settings import SETTINGS
 from blurry.settings import update_settings
@@ -65,14 +66,17 @@
                 {
                     SETTINGS["MARKDOWN_FILE_JINJA_TEMPLATE_EXTENSION"].lstrip("."),
                     "html",
                     "xml",
                 }
             )
         ),
+        extensions=[
+            jinja_extension.load() for jinja_extension in discovered_jinja_extensions
+        ],
     )
     for filter_plugin in discovered_jinja_filter_plugins:
         try:
             jinja_env.filters[filter_plugin.name] = filter_plugin.load()
         except AttributeError:
             print(
                 f"Could not load Jinja filter plugin: {filter_plugin.name}. "
```

### Comparing `blurry_cli-0.7.2/blurry/async_typer.py` & `blurry_cli-0.8.0/blurry/async_typer.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/cli.py` & `blurry_cli-0.8.0/blurry/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from rich.console import Console
 from rich.table import Table
 
 from blurry.plugins import discovered_html_plugins
+from blurry.plugins import discovered_jinja_extensions
 from blurry.plugins import discovered_jinja_filter_plugins
 from blurry.plugins import discovered_markdown_plugins
 
 console = Console()
 
 
 def print_blurry_name():
@@ -23,11 +24,14 @@
     plugin_table = Table(show_header=True)
     plugin_table.add_column("Markdown Plugins")
     plugin_table.add_column("HTML Plugins")
     plugin_table.add_column("Jinja Plugins")
     plugin_table.add_row(
         "\n".join([p.name for p in discovered_markdown_plugins]),
         "\n".join([p.name for p in discovered_html_plugins]),
-        "\n".join([p.name for p in discovered_jinja_filter_plugins]),
+        "\n".join(
+            [p.name for p in discovered_jinja_filter_plugins]
+            + [p.name for p in discovered_jinja_extensions]
+        ),
     )
 
     console.print(plugin_table)
```

### Comparing `blurry_cli-0.7.2/blurry/images.py` & `blurry_cli-0.8.0/blurry/images.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/markdown/__init__.py` & `blurry_cli-0.8.0/blurry/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/markdown/front_matter.py` & `blurry_cli-0.8.0/blurry/markdown/front_matter.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/markdown/renderer_functions/render_video.py` & `blurry_cli-0.8.0/blurry/markdown/renderer_functions/render_video.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/open_graph.py` & `blurry_cli-0.8.0/blurry/open_graph.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/plugins/html_plugins/minify_html_plugin.py` & `blurry_cli-0.8.0/blurry/plugins/html_plugins/minify_html_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/plugins/markdown_plugins/container_plugin.py` & `blurry_cli-0.8.0/blurry/plugins/markdown_plugins/container_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/plugins/markdown_plugins/punctuation_plugin.py` & `blurry_cli-0.8.0/blurry/plugins/markdown_plugins/punctuation_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/plugins/markdown_plugins/python_code_plugin.py` & `blurry_cli-0.8.0/blurry/plugins/markdown_plugins/python_code_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/schema_validation.py` & `blurry_cli-0.8.0/blurry/schema_validation.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/settings.py` & `blurry_cli-0.8.0/blurry/settings.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/sitemap.py` & `blurry_cli-0.8.0/blurry/sitemap.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/types.py` & `blurry_cli-0.8.0/blurry/types.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/blurry/utils.py` & `blurry_cli-0.8.0/blurry/utils.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.2/pyproject.toml` & `blurry_cli-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blurry-cli"
-version = "0.7.2"
+version = "0.8.0"
 description = "A Mistune-based static site generator for Python"
 authors = ["John Franey <franey@duck.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/blurry-dev/blurry"
 keywords = ["static-site-generator", "seo", "pagespeed"]
 classifiers = [
@@ -33,14 +33,15 @@
 rich = "^13.3.3"
 selectolax = "^0.3.6"
 toml = "^0.10.2"
 typer = "^0.6.1"
 htmlmin2 = "^0.1.13"
 pydantic2-schemaorg = "^0.1.1"
 dpath = "^2.1.6"
+jinja2-simple-tags = "^0.6.1"
 
 [tool.poetry.scripts]
 blurry = 'blurry:main'
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 nox = "^2024.03.02"
@@ -66,7 +67,10 @@
 minify_html = 'blurry.plugins.html_plugins.minify_html_plugin:minify_html'
 
 [tool.poetry.plugins."blurry.markdown_plugins"]
 python_code = 'blurry.plugins.markdown_plugins.python_code_plugin:python_code'
 python_code_in_list = 'blurry.plugins.markdown_plugins.python_code_plugin:python_code_in_list'
 punctuation = 'blurry.plugins.markdown_plugins.punctuation_plugin:punctuation'
 container = 'blurry.plugins.markdown_plugins.container_plugin:container'
+
+[tool.poetry.plugins."blurry.jinja_extensions"]
+blurry_image = "blurry.plugins.jinja_plugins.blurry_image_extension:BlurryImage"
```

### Comparing `blurry_cli-0.7.2/PKG-INFO` & `blurry_cli-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blurry-cli
-Version: 0.7.2
+Version: 0.8.0
 Summary: A Mistune-based static site generator for Python
 Home-page: https://github.com/blurry-dev/blurry
 License: MIT
 Keywords: static-site-generator,seo,pagespeed
 Author: John Franey
 Author-email: franey@duck.com
 Requires-Python: >=3.10,<4.0
@@ -22,14 +22,15 @@
 Classifier: Topic :: Text Processing :: Markup :: Markdown 
 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: PyLD (>=2.0.3,<3.0.0)
 Requires-Dist: Wand (>=0.6.6,<0.7.0)
 Requires-Dist: dpath (>=2.1.6,<3.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: htmlmin2 (>=0.1.13,<0.2.0)
+Requires-Dist: jinja2-simple-tags (>=0.6.1,<0.7.0)
 Requires-Dist: livereload (>=2.6.3,<3.0.0)
 Requires-Dist: mistune (>=3.0.0rc5,<4.0.0)
 Requires-Dist: pydantic2-schemaorg (>=0.1.1,<0.2.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: selectolax (>=0.3.6,<0.4.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
```

