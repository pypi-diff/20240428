# Comparing `tmp/zz-pix-0.0.7.tar.gz` & `tmp/zz-pix-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zz-pix-0.0.7.tar", last modified: Tue Apr  2 13:17:38 2024, max compression
+gzip compressed data, was "zz-pix-0.0.8.tar", last modified: Sun Apr 28 09:43:51 2024, max compression
```

## Comparing `zz-pix-0.0.7.tar` & `zz-pix-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 13:17:38.189724 zz-pix-0.0.7/
--rw-rw-rw-   0        0        0    11541 2024-03-29 15:51:16.000000 zz-pix-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     8041 2024-04-02 13:17:38.189724 zz-pix-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 13:17:38.179209 zz-pix-0.0.7/pix/
--rw-rw-rw-   0        0        0        0 2024-03-29 15:51:16.000000 zz-pix-0.0.7/pix/__init__.py
--rw-rw-rw-   0        0        0     4614 2024-04-02 13:16:09.000000 zz-pix-0.0.7/pix/caption.py
--rw-rw-rw-   0        0        0     4497 2024-04-02 13:16:09.000000 zz-pix-0.0.7/pix/cli_parser.py
--rw-rw-rw-   0        0        0     2856 2024-03-29 15:51:16.000000 zz-pix-0.0.7/pix/converter.py
--rw-rw-rw-   0        0        0     3852 2024-03-29 15:51:16.000000 zz-pix-0.0.7/pix/croper.py
--rw-rw-rw-   0        0        0     4456 2024-04-02 13:16:09.000000 zz-pix-0.0.7/pix/main.py
--rw-rw-rw-   0        0        0      182 2024-04-02 13:16:09.000000 zz-pix-0.0.7/pix/manifest.json
--rw-rw-rw-   0        0        0      588 2024-03-30 18:15:25.000000 zz-pix-0.0.7/pix/prune.py
--rw-rw-rw-   0        0        0     1580 2024-03-29 15:51:16.000000 zz-pix-0.0.7/pix/resizer.py
--rw-rw-rw-   0        0        0      706 2024-03-29 18:51:50.000000 zz-pix-0.0.7/pix/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-02 13:17:38.189724 zz-pix-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1824 2024-04-02 13:17:34.000000 zz-pix-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:17:38.188722 zz-pix-0.0.7/zz_pix.egg-info/
--rw-rw-rw-   0        0        0     8041 2024-04-02 13:17:38.000000 zz-pix-0.0.7/zz_pix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-02 13:17:38.000000 zz-pix-0.0.7/zz_pix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 13:17:38.000000 zz-pix-0.0.7/zz_pix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-02 13:17:38.000000 zz-pix-0.0.7/zz_pix.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2024-04-02 13:17:38.000000 zz-pix-0.0.7/zz_pix.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 13:17:38.000000 zz-pix-0.0.7/zz_pix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 09:43:51.315734 zz-pix-0.0.8/
+-rw-rw-rw-   0        0        0    11541 2024-03-29 15:51:16.000000 zz-pix-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     6391 2024-04-28 09:43:51.314231 zz-pix-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 09:43:51.299612 zz-pix-0.0.8/pix/
+-rw-rw-rw-   0        0        0        0 2024-03-29 15:51:16.000000 zz-pix-0.0.8/pix/__init__.py
+-rw-rw-rw-   0        0        0     3343 2024-04-28 07:49:22.000000 zz-pix-0.0.8/pix/cli_parser.py
+-rw-rw-rw-   0        0        0     2856 2024-03-29 15:51:16.000000 zz-pix-0.0.8/pix/converter.py
+-rw-rw-rw-   0        0        0     3852 2024-03-29 15:51:16.000000 zz-pix-0.0.8/pix/croper.py
+-rw-rw-rw-   0        0        0     3464 2024-04-28 07:50:00.000000 zz-pix-0.0.8/pix/main.py
+-rw-rw-rw-   0        0        0      182 2024-04-28 07:48:49.000000 zz-pix-0.0.8/pix/manifest.json
+-rw-rw-rw-   0        0        0      588 2024-03-30 18:15:25.000000 zz-pix-0.0.8/pix/prune.py
+-rw-rw-rw-   0        0        0     1580 2024-03-29 15:51:16.000000 zz-pix-0.0.8/pix/resizer.py
+-rw-rw-rw-   0        0        0      706 2024-03-29 18:51:50.000000 zz-pix-0.0.8/pix/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 09:43:51.315734 zz-pix-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2024-04-28 07:49:09.000000 zz-pix-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:43:51.314231 zz-pix-0.0.8/zz_pix.egg-info/
+-rw-rw-rw-   0        0        0     6391 2024-04-28 09:43:51.000000 zz-pix-0.0.8/zz_pix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-04-28 09:43:51.000000 zz-pix-0.0.8/zz_pix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:43:51.000000 zz-pix-0.0.8/zz_pix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-28 09:43:51.000000 zz-pix-0.0.8/zz_pix.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2024-04-28 09:43:51.000000 zz-pix-0.0.8/zz_pix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-28 09:43:51.000000 zz-pix-0.0.8/zz_pix.egg-info/top_level.txt
```

### Comparing `zz-pix-0.0.7/LICENSE` & `zz-pix-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.7/PKG-INFO` & `zz-pix-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zz-pix
-Version: 0.0.7
+Version: 0.0.8
 Summary: CLI tool for image manipulation
 Home-page: https://github.com/sean1832/pix
 Author: Zeke Zhang
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,18 +21,15 @@
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Raster-Based
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow
 Requires-Dist: pillow-avif-plugin
 Requires-Dist: pillow-heif
-Requires-Dist: transformers>=4.39.2
-Requires-Dist: torch>=2.2.2
 Requires-Dist: termcolor
-Requires-Dist: pyexiv2
 Requires-Dist: tqdm
 
 # PIX
 [![PyPI - Version](https://img.shields.io/pypi/v/zz-pix)](https://pypi.org/project/zz-pix)
 [![PyPI - License](https://img.shields.io/pypi/l/zz-pix)](LICENSE)
 [![Downloads](https://static.pepy.tech/badge/zz-pix)](https://pepy.tech/project/zz-pix)
 
@@ -151,34 +148,16 @@
 
 | Option         | Input Type | Description                                       | Default |
 |----------------|------------|---------------------------------------------------|---------|
 | input          | String     | Input image or directory                          | N/A     |
 | `-r`, `--resolution` | String   | Minimum resolution (WxH)                         | N/A     |
 | `--dry-run`      | Flag       | List files to be removed without deleting them    | N/A     |
 
-#### Caption
-Create text description to images or directories of images using machine learning models. Currently supports [BLIP](https://huggingface.co/Salesforce/blip-image-captioning-base) and [BLIP2](https://huggingface.co/Salesforce/blip2-opt-2.7b) models. 
->The `BLIP2` model is more accurate but slower than the `BLIP` model. The `BLIP2` model is recommended for better results.
-
-```sh
-pix caption [OPTIONS]
-```
-
-| Option          | Input Type | Description                                | Default |
-|-----------------|------------|--------------------------------------------|---------|
-| `input`           | String     | Input image or directory                   | N/A     |
-| `-t`, `--token`     | Integer    | Max token length for captioning            | 32      |
-| `-b`, `--batch`     | Integer    | Batch size for captioning (increase speed but also increase memory usage. CPU mode is capped to `2`.)                  | 1       |
-| `-p`, `--prompt`    | String     | Prompt for captioning                      | N/A     |
-| `--temperature`   | Float      | Temperature for captioning                 | 1.0     |
-| `--seed`          | Integer    | Seed for reproducibility                   | N/A     |
-| `--large`         | Flag       | Use the large model                        | N/A     |
-| `--cpu`           | Flag       | Use CPU instead of GPU                     | N/A     |
-| `--metadata`      | Flag       | Write caption as metadata for the image    | N/A     |
-| `--blip2`         | Flag       | Use Blip2 model for captioning (slower but results better)| N/A|
-| `--verbose`       | Flag       | Print verbose output                       | N/A     |
+#### ~~Caption~~ 
+(Removed this feature, implemented in a separate tool [zz-img-caption](https://github.com/sean1832/zz-img-caption))
+
 
 
 
 ## License
 [Apache-2.0](LICENSE)
```

### Comparing `zz-pix-0.0.7/pix/cli_parser.py` & `zz-pix-0.0.8/pix/cli_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,23 +43,9 @@
 
     # prune command
     prune_parser = subparser.add_parser("prune", help="Remove images smaller than specified resolution")
     prune_parser.add_argument("input", type=str, help="Input image or directory")
     prune_parser.add_argument("-r", "--resolution", type=str, help="Minimum resolution as WxH. Images smaller than this will be removed.")
     prune_parser.add_argument("--dry-run", action="store_true", help="Perform a dry run without deleting files.")
 
-    # blip command
-    blip_parser = subparser.add_parser("caption", help="Caption on images")
-    blip_parser.add_argument("input", type=str, help="Input image or directory")
-    blip_parser.add_argument("-t", "--token", type=int, help="Max token length for captioning", default=32)
-    blip_parser.add_argument("-b", "--batch", type=int, help="Batch size for captioning", default=1)
-    blip_parser.add_argument("-p", "--prompt", type=str, help="Prompt for captioning")
-    blip_parser.add_argument("--temperature", type=float, help="Temperature for captioning", default=1.0)
-    blip_parser.add_argument("--seed", type=int, help="Seed for reproducibility")
-    blip_parser.add_argument("--large", action="store_true", help="Use the large model")
-    blip_parser.add_argument("--cpu", action="store_true", help="Use CPU instead of GPU")
-    blip_parser.add_argument("--metadata", action="store_true", help="Write caption as metadata for image")
-    blip_parser.add_argument("--blip2", action="store_true", help="Use Blip2 model for captioning")
-    blip_parser.add_argument("--verbose", action="store_true", help="Print verbose output")
-
     return parser
 # fmt: on
```

### Comparing `zz-pix-0.0.7/pix/converter.py` & `zz-pix-0.0.8/pix/converter.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.7/pix/croper.py` & `zz-pix-0.0.8/pix/croper.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.7/pix/main.py` & `zz-pix-0.0.8/pix/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import glob
 import pathlib
 import traceback
 
-import pyexiv2
-
-from pix import cli_parser, converter, croper, prune, resizer, utils
+from pix import cli_parser, converter, croper, prune, resizer
 
 
 def get_io_paths(args):
     file_input = pathlib.Path(args.input)
     file_output = pathlib.Path(args.output)
     return file_input, file_output
 
@@ -88,37 +85,14 @@
         prune.prune_image(file_input, args.resolution, args.dry_run)
     elif file_input.is_dir():
         prune.prune_images(file_input, args.resolution, args.dry_run)
     else:
         raise FileNotFoundError(f"`{args.input}` not found.")
 
 
-def caption_cmd(args):
-    from pix.caption import Blip
-
-    file_input = pathlib.Path(args.input).absolute()
-    if file_input.is_dir():
-        file_input = file_input.joinpath("*.*")
-    inputs = glob.glob(str(file_input))  # wildcard
-    # filter out non-image files
-    inputs = [i for i in inputs if utils.is_file_supported(i)]
-
-    blip = Blip(args.large, args.cpu, args.blip2)
-
-    caption_dicts = blip.caption_image(
-        inputs, args.token, args.seed, args.temperature, args.batch, args.prompt
-    )
-    for image, caption_dict in zip(inputs, caption_dicts):
-        caption = caption_dict[0]["generated_text"]
-        if args.metadata:
-            with pyexiv2.Image(image) as img:
-                img.modify_exif({"Exif.Image.XPComment": caption})
-        if args.verbose:
-            print(f"\n{image} - {caption}")
-
 
 def main():
     try:
         parser = cli_parser.get_parser()
         args = parser.parse_args()
         if args.command is None:
             parser.print_help()
@@ -136,18 +110,14 @@
         elif args.command == "crop":
             crop_cmd(args)
 
         # Prune command
         elif args.command == "prune":
             prune_cmd(args)
 
-        # Blip command
-        elif args.command == "caption":
-            caption_cmd(args)
-
         print("Done!")
     except FileNotFoundError as e:
         print("File not found:", e)
         exit(1)
     except FileExistsError as e:
         print(e)
         exit(1)
```

### Comparing `zz-pix-0.0.7/pix/prune.py` & `zz-pix-0.0.8/pix/prune.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.7/pix/resizer.py` & `zz-pix-0.0.8/pix/resizer.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.7/pix/utils.py` & `zz-pix-0.0.8/pix/utils.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.7/setup.py` & `zz-pix-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,15 @@
             "manifest.json",
         ]
     },
     install_requires=[
         "pillow",
         "pillow-avif-plugin",
         "pillow-heif",
-        "transformers>=4.39.2",
-        "torch>=2.2.2",
         "termcolor",
-        "pyexiv2",
         "tqdm",
     ],
     entry_points={
         "console_scripts": [
             "pix = pix.main:main",
         ],
     },
```

### Comparing `zz-pix-0.0.7/zz_pix.egg-info/PKG-INFO` & `zz-pix-0.0.8/zz_pix.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zz-pix
-Version: 0.0.7
+Version: 0.0.8
 Summary: CLI tool for image manipulation
 Home-page: https://github.com/sean1832/pix
 Author: Zeke Zhang
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,18 +21,15 @@
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Raster-Based
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow
 Requires-Dist: pillow-avif-plugin
 Requires-Dist: pillow-heif
-Requires-Dist: transformers>=4.39.2
-Requires-Dist: torch>=2.2.2
 Requires-Dist: termcolor
-Requires-Dist: pyexiv2
 Requires-Dist: tqdm
 
 # PIX
 [![PyPI - Version](https://img.shields.io/pypi/v/zz-pix)](https://pypi.org/project/zz-pix)
 [![PyPI - License](https://img.shields.io/pypi/l/zz-pix)](LICENSE)
 [![Downloads](https://static.pepy.tech/badge/zz-pix)](https://pepy.tech/project/zz-pix)
 
@@ -151,34 +148,16 @@
 
 | Option         | Input Type | Description                                       | Default |
 |----------------|------------|---------------------------------------------------|---------|
 | input          | String     | Input image or directory                          | N/A     |
 | `-r`, `--resolution` | String   | Minimum resolution (WxH)                         | N/A     |
 | `--dry-run`      | Flag       | List files to be removed without deleting them    | N/A     |
 
-#### Caption
-Create text description to images or directories of images using machine learning models. Currently supports [BLIP](https://huggingface.co/Salesforce/blip-image-captioning-base) and [BLIP2](https://huggingface.co/Salesforce/blip2-opt-2.7b) models. 
->The `BLIP2` model is more accurate but slower than the `BLIP` model. The `BLIP2` model is recommended for better results.
-
-```sh
-pix caption [OPTIONS]
-```
-
-| Option          | Input Type | Description                                | Default |
-|-----------------|------------|--------------------------------------------|---------|
-| `input`           | String     | Input image or directory                   | N/A     |
-| `-t`, `--token`     | Integer    | Max token length for captioning            | 32      |
-| `-b`, `--batch`     | Integer    | Batch size for captioning (increase speed but also increase memory usage. CPU mode is capped to `2`.)                  | 1       |
-| `-p`, `--prompt`    | String     | Prompt for captioning                      | N/A     |
-| `--temperature`   | Float      | Temperature for captioning                 | 1.0     |
-| `--seed`          | Integer    | Seed for reproducibility                   | N/A     |
-| `--large`         | Flag       | Use the large model                        | N/A     |
-| `--cpu`           | Flag       | Use CPU instead of GPU                     | N/A     |
-| `--metadata`      | Flag       | Write caption as metadata for the image    | N/A     |
-| `--blip2`         | Flag       | Use Blip2 model for captioning (slower but results better)| N/A|
-| `--verbose`       | Flag       | Print verbose output                       | N/A     |
+#### ~~Caption~~ 
+(Removed this feature, implemented in a separate tool [zz-img-caption](https://github.com/sean1832/zz-img-caption))
+
 
 
 
 ## License
 [Apache-2.0](LICENSE)
```

