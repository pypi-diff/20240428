# Comparing `tmp/blurry_cli-0.7.1.tar.gz` & `tmp/blurry_cli-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blurry_cli-0.7.1.tar", max compression
+gzip compressed data, was "blurry_cli-0.7.2.tar", max compression
```

## Comparing `blurry_cli-0.7.1.tar` & `blurry_cli-0.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1068 2024-04-13 20:11:15.540569 blurry_cli-0.7.1/LICENSE
--rw-r--r--   0        0        0     1782 2024-04-13 20:11:15.540569 blurry_cli-0.7.1/README.md
--rw-r--r--   0        0        0     9905 2024-04-13 20:11:15.540569 blurry_cli-0.7.1/blurry/__init__.py
--rw-r--r--   0        0        0       32 2024-04-13 20:11:15.540569 blurry_cli-0.7.1/blurry/__main__.py
--rw-r--r--   0        0        0      526 2024-04-13 20:11:15.540569 blurry_cli-0.7.1/blurry/async_typer.py
--rw-r--r--   0        0        0      872 2024-04-13 20:11:15.540569 blurry_cli-0.7.1/blurry/cli.py
--rw-r--r--   0        0        0      111 2024-04-13 20:11:15.540569 blurry_cli-0.7.1/blurry/constants.py
--rw-r--r--   0        0        0     3537 2024-04-13 20:11:15.540569 blurry_cli-0.7.1/blurry/images.py
--rw-r--r--   0        0        0     7427 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/markdown/__init__.py
--rw-r--r--   0        0        0     1778 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/markdown/front_matter.py
--rw-r--r--   0        0        0        0 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/markdown/renderer_functions/__init__.py
--rw-r--r--   0        0        0      787 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/markdown/renderer_functions/render_video.py
--rw-r--r--   0        0        0     1995 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/open_graph.py
--rw-r--r--   0        0        0      273 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/plugins/html_plugins/__init__.py
--rw-r--r--   0        0        0     1124 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/plugins/html_plugins/minify_html_plugin.py
--rw-r--r--   0        0        0        0 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/plugins/markdown_plugins/__init__.py
--rw-r--r--   0        0        0     1119 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/plugins/markdown_plugins/container_plugin.py
--rw-r--r--   0        0        0      683 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/plugins/markdown_plugins/punctuation_plugin.py
--rw-r--r--   0        0        0     1509 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/plugins/markdown_plugins/python_code_plugin.py
--rw-r--r--   0        0        0        0 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/py.typed
--rw-r--r--   0        0        0     1817 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/schema_validation.py
--rw-r--r--   0        0        0     2347 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/settings.py
--rw-r--r--   0        0        0     1752 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/sitemap.py
--rw-r--r--   0        0        0      777 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/types.py
--rw-r--r--   0        0        0     4376 2024-04-13 20:11:15.544569 blurry_cli-0.7.1/blurry/utils.py
--rw-r--r--   0        0        0     2195 2024-04-13 20:11:15.548569 blurry_cli-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 blurry_cli-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1782 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/README.md
+-rw-r--r--   0        0        0     9864 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/__main__.py
+-rw-r--r--   0        0        0      526 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/async_typer.py
+-rw-r--r--   0        0        0      872 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/cli.py
+-rw-r--r--   0        0        0      111 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/constants.py
+-rw-r--r--   0        0        0     3537 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/images.py
+-rw-r--r--   0        0        0     7897 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/markdown/__init__.py
+-rw-r--r--   0        0        0     1778 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/markdown/front_matter.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/markdown/renderer_functions/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/markdown/renderer_functions/render_video.py
+-rw-r--r--   0        0        0     1993 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/open_graph.py
+-rw-r--r--   0        0        0      273 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/html_plugins/__init__.py
+-rw-r--r--   0        0        0     1124 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/html_plugins/minify_html_plugin.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/markdown_plugins/__init__.py
+-rw-r--r--   0        0        0     1119 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/markdown_plugins/container_plugin.py
+-rw-r--r--   0        0        0      683 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/markdown_plugins/punctuation_plugin.py
+-rw-r--r--   0        0        0     1509 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/plugins/markdown_plugins/python_code_plugin.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/py.typed
+-rw-r--r--   0        0        0     1817 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/schema_validation.py
+-rw-r--r--   0        0        0     2347 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/settings.py
+-rw-r--r--   0        0        0     1752 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/sitemap.py
+-rw-r--r--   0        0        0      777 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/types.py
+-rw-r--r--   0        0        0     4376 2024-04-27 15:14:26.940594 blurry_cli-0.7.2/blurry/utils.py
+-rw-r--r--   0        0        0     2195 2024-04-27 15:14:26.944594 blurry_cli-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 blurry_cli-0.7.2/PKG-INFO
```

### Comparing `blurry_cli-0.7.1/LICENSE` & `blurry_cli-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/README.md` & `blurry_cli-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/__init__.py` & `blurry_cli-0.7.2/blurry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     # Copy file to build directory
     shutil.copyfile(filepath, build_filepath)
 
     # Create srcset images
     if mimetype in [
         mimetypes.types_map[".jpg"],
         mimetypes.types_map[".png"],
-        mimetypes.common_types[".webp"],
     ]:
         await generate_images_for_srcset(filepath)
 
 
 async def write_html_file(
     file_data: MarkdownFileData,
     file_data_list: list[MarkdownFileData],
```

### Comparing `blurry_cli-0.7.1/blurry/async_typer.py` & `blurry_cli-0.7.2/blurry/async_typer.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/cli.py` & `blurry_cli-0.7.2/blurry/cli.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/images.py` & `blurry_cli-0.7.2/blurry/images.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/markdown/__init__.py` & `blurry_cli-0.7.2/blurry/markdown/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,23 +65,32 @@
             # Convert relative path to URL pathname
             absolute_path = resolve_relative_path_in_markdown(src, self.filepath)
             extension = absolute_path.suffix.removeprefix(".")
             src = path_to_url_pathname(absolute_path)
             attributes["src"] = src
 
             if extension.lower() in SETTINGS.get("VIDEO_EXTENSIONS"):
-                return render_video(src, absolute_path, extension, title=text)
+                return render_video(src, absolute_path, extension, title=title)
 
             # Tailor srcset and sizes to image width
             with Image(filename=str(absolute_path)) as img:
                 image_width = img.width
                 image_height = img.height
+                # The .animated property doesn't always detect animated .webp images
+                # and .webp is optimized enough not to benefit much from .avif
+                image_is_animated = img.animation or extension.lower() == "webp"
                 attributes["width"] = image_width
                 attributes["height"] = image_height
 
+            if image_is_animated:
+                attributes_str = " ".join(
+                    f'{name}="{value}"' for name, value in attributes.items()
+                )
+                return f"<img {attributes_str} >"
+
             image_widths = get_widths_for_image_width(image_width)
 
             attributes["sizes"] = generate_sizes_string(image_widths)
             attributes["srcset"] = generate_srcset_string(src, image_widths)
             avif_srcset = generate_srcset_string(
                 src.replace(extension, "avif"), image_widths
             )
```

### Comparing `blurry_cli-0.7.1/blurry/markdown/front_matter.py` & `blurry_cli-0.7.2/blurry/markdown/front_matter.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/markdown/renderer_functions/render_video.py` & `blurry_cli-0.7.2/blurry/markdown/renderer_functions/render_video.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/open_graph.py` & `blurry_cli-0.7.2/blurry/open_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 from typing import Literal
 
 from blurry.types import SchemaType
 
 
-META_TAG_TEMPLATE = '<meta property="og:{property}" content="{content}" />'
+META_TAG_TEMPLATE = '<meta property="og:{property}" content="{content}">'
 
 OpenGraphType = Literal["article", "book", "profile", "website"]
 
 
 schema_type_to_open_graph_type: dict[SchemaType, OpenGraphType] = {
     SchemaType.ARTICLE: "article",
     SchemaType.BLOG_POSTING: "article",
```

### Comparing `blurry_cli-0.7.1/blurry/plugins/html_plugins/minify_html_plugin.py` & `blurry_cli-0.7.2/blurry/plugins/html_plugins/minify_html_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/plugins/markdown_plugins/container_plugin.py` & `blurry_cli-0.7.2/blurry/plugins/markdown_plugins/container_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/plugins/markdown_plugins/punctuation_plugin.py` & `blurry_cli-0.7.2/blurry/plugins/markdown_plugins/punctuation_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/plugins/markdown_plugins/python_code_plugin.py` & `blurry_cli-0.7.2/blurry/plugins/markdown_plugins/python_code_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/schema_validation.py` & `blurry_cli-0.7.2/blurry/schema_validation.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/settings.py` & `blurry_cli-0.7.2/blurry/settings.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/sitemap.py` & `blurry_cli-0.7.2/blurry/sitemap.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/types.py` & `blurry_cli-0.7.2/blurry/types.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/blurry/utils.py` & `blurry_cli-0.7.2/blurry/utils.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.7.1/pyproject.toml` & `blurry_cli-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blurry-cli"
-version = "0.7.1"
+version = "0.7.2"
 description = "A Mistune-based static site generator for Python"
 authors = ["John Franey <franey@duck.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/blurry-dev/blurry"
 keywords = ["static-site-generator", "seo", "pagespeed"]
 classifiers = [
```

### Comparing `blurry_cli-0.7.1/PKG-INFO` & `blurry_cli-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blurry-cli
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Mistune-based static site generator for Python
 Home-page: https://github.com/blurry-dev/blurry
 License: MIT
 Keywords: static-site-generator,seo,pagespeed
 Author: John Franey
 Author-email: franey@duck.com
 Requires-Python: >=3.10,<4.0
```

