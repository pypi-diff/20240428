# Comparing `tmp/dds-cloudapi-sdk-0.1.1.tar.gz` & `tmp/dds-cloudapi-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dds-cloudapi-sdk-0.1.1.tar", last modified: Fri Mar 22 03:43:28 2024, max compression
+gzip compressed data, was "dds-cloudapi-sdk-0.2.0.tar", last modified: Sun Apr 28 06:44:32 2024, max compression
```

## Comparing `dds-cloudapi-sdk-0.1.1.tar` & `dds-cloudapi-sdk-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2024-03-22 03:43:28.034999 dds-cloudapi-sdk-0.1.1/
--rw-r--r--   0 johnhu     (501) staff       (20)    11310 2023-06-16 10:36:53.000000 dds-cloudapi-sdk-0.1.1/LICENSE
--rw-r--r--   0 johnhu     (501) staff       (20)     5835 2024-03-22 03:43:28.034861 dds-cloudapi-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 johnhu     (501) staff       (20)     3982 2024-03-22 03:38:22.000000 dds-cloudapi-sdk-0.1.1/README.md
-drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2024-03-22 03:43:28.032151 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/
--rw-r--r--   0 johnhu     (501) staff       (20)      123 2024-03-14 08:06:40.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/__init__.py
--rw-r--r--   0 johnhu     (501) staff       (20)     3377 2024-03-21 06:37:38.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/client.py
--rw-r--r--   0 johnhu     (501) staff       (20)     1161 2024-03-22 03:38:22.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/config.py
-drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2024-03-22 03:43:28.034613 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/
--rw-r--r--   0 johnhu     (501) staff       (20)     1479 2024-03-22 03:43:21.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/__init__.py
--rw-r--r--   0 johnhu     (501) staff       (20)     3816 2024-03-21 02:33:16.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/base.py
--rw-r--r--   0 johnhu     (501) staff       (20)     7462 2024-03-21 08:01:14.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/gsam.py
--rw-r--r--   0 johnhu     (501) staff       (20)     7524 2024-03-19 11:03:43.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/ivp.py
--rw-r--r--   0 johnhu     (501) staff       (20)     4285 2024-03-20 11:02:15.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/prompt.py
--rw-r--r--   0 johnhu     (501) staff       (20)     3276 2024-03-20 11:02:15.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/trex_embd_customize.py
--rw-r--r--   0 johnhu     (501) staff       (20)     4253 2024-03-20 11:02:15.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/trex_embd_infer.py
--rw-r--r--   0 johnhu     (501) staff       (20)     3856 2024-03-20 08:54:25.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/trex_generic.py
--rw-r--r--   0 johnhu     (501) staff       (20)     4168 2024-03-20 11:02:15.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/trex_interactive.py
-drwxr-xr-x   0 johnhu     (501) staff       (20)        0 2024-03-22 03:43:28.032794 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk.egg-info/
--rw-r--r--   0 johnhu     (501) staff       (20)     5835 2024-03-22 03:43:27.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk.egg-info/PKG-INFO
--rw-r--r--   0 johnhu     (501) staff       (20)      638 2024-03-22 03:43:28.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 johnhu     (501) staff       (20)        1 2024-03-22 03:43:27.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 johnhu     (501) staff       (20)       62 2024-03-22 03:43:27.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk.egg-info/requires.txt
--rw-r--r--   0 johnhu     (501) staff       (20)       40 2024-03-22 03:43:27.000000 dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk.egg-info/top_level.txt
--rw-r--r--   0 johnhu     (501) staff       (20)       38 2024-03-22 03:43:28.035053 dds-cloudapi-sdk-0.1.1/setup.cfg
--rw-r--r--   0 johnhu     (501) staff       (20)     1733 2024-03-22 03:43:21.000000 dds-cloudapi-sdk-0.1.1/setup.py
+drwxr-xr-x   0 lizhiqiang   (501) staff       (20)        0 2024-04-28 06:44:32.963684 dds-cloudapi-sdk-0.2.0/
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)    11310 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/LICENSE
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     4947 2024-04-28 06:44:32.963147 dds-cloudapi-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     3982 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/README.md
+drwxr-xr-x   0 lizhiqiang   (501) staff       (20)        0 2024-04-28 06:44:32.956120 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)      142 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/__init__.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     3377 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/client.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     1170 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/config.py
+drwxr-xr-x   0 lizhiqiang   (501) staff       (20)        0 2024-04-28 06:44:32.962110 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     1725 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/__init__.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     3829 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/base.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     8772 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/detection.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     7452 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/gsam.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     7650 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/ivp.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     4559 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/prompt.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     3297 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/trex_embd_customize.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     4274 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/trex_embd_infer.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     3898 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/trex_generic.py
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     4189 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/trex_interactive.py
+drwxr-xr-x   0 lizhiqiang   (501) staff       (20)        0 2024-04-28 06:44:32.957978 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk.egg-info/
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     4947 2024-04-28 06:44:32.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)      674 2024-04-28 06:44:32.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)        1 2024-04-28 06:44:32.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)       62 2024-04-28 06:44:32.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk.egg-info/requires.txt
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)       40 2024-04-28 06:44:32.000000 dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk.egg-info/top_level.txt
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)       38 2024-04-28 06:44:32.963836 dds-cloudapi-sdk-0.2.0/setup.cfg
+-rw-r--r--   0 lizhiqiang   (501) staff       (20)     1752 2024-04-28 06:41:02.000000 dds-cloudapi-sdk-0.2.0/setup.py
```

### Comparing `dds-cloudapi-sdk-0.1.1/LICENSE` & `dds-cloudapi-sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dds-cloudapi-sdk-0.1.1/PKG-INFO` & `dds-cloudapi-sdk-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,144 +1,147 @@
 Metadata-Version: 2.1
 Name: dds-cloudapi-sdk
-Version: 0.1.1
+Version: 0.2.0
 Summary: The SDK for calling deepdataspace cloud API.
 Home-page: https://github.com/deepdataspace/dds-cloudapi-sdk
 Author: cvr@idea
-License: UNKNOWN
-Description: # dds-cloudapi-sdk
-        
-        ---
-        
-        <div align="center">
-        <p align="center">
-        
-        <!-- prettier-ignore -->
-        **The Python SDK for the DDS Cloud API.**
-        ---
-        
-        <!-- prettier-ignore -->
-        
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
-        [![PyPI python](https://img.shields.io/pypi/pyversions/dds-cloudapi-sdk)](https://pypi.org/project/dds-cloudapi-sdk)
-        [![PyPI version](https://img.shields.io/pypi/v/dds-cloudapi-sdk)](https://pypi.org/project/dds-cloudapi-sdk)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/dds-cloudapi-sdk)
-        
-        </p>
-        </div>
-        
-        ---
-        
-        The dds-cloudapi-sdk is a Python package designed to simplify interactions with the DDS Cloud API. It features:
-        
-        - **Straightforward** APIs
-        - **Unified** interfaces
-        - **Handy** utilities
-        
-        ## Installation
-        
-        You can get the SDK library directly from PyPi:
-        
-        ```shell
-        pip install dds-cloudapi-sdk
-        ```
-        
-        ## Quick Start
-        
-        Below is a straightforward example for the popular IVP algorithm:
-        
-        ```python
-        # 1. Initialize the client with your API token.
-        from dds_cloudapi_sdk import Config
-        from dds_cloudapi_sdk import Client
-        
-        token = "Your API Token Here"
-        config = Config(token)
-        client = Client(config)
-        
-        # 2. Upload local image to the server and get the URL.
-        infer_image_url = "https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg"
-        # infer_image_url = client.upload_file("path/to/infer/image.jpg")  # you can also upload local file for processing
-        prompt_image_url = infer_image_url  # use the same image for prompt
-        
-        # 3. Create a task with proper parameters.
-        from dds_cloudapi_sdk.tasks import IVPTask
-        from dds_cloudapi_sdk.tasks import RectPrompt
-        from dds_cloudapi_sdk.tasks import LabelTypes
-        
-        task = IVPTask(
-            prompt_image_url=prompt_image_url,
-            prompts=[RectPrompt(rect=[475.18, 550.20, 548.10, 599.92], is_positive=True)],
-            infer_image_url=infer_image_url,
-            infer_label_types=[LabelTypes.BBox, LabelTypes.Mask],  # infer both bbox and mask
-        )
-        
-        # 4. Run the task and get the result.
-        client.run_task(task)
-        
-        # 5. Parse the result.
-        from dds_cloudapi_sdk.tasks.ivp import TaskResult
-        
-        result: TaskResult = task.result
-        
-        mask_url = result.mask_url  # the image url with all masks drawn on
-        objects = result.objects  # the list of detected objects
-        for idx, obj in enumerate(objects):
-            # get the detection score
-            print(obj.score)  # 0.42
-        
-            # get the detection bbox
-            print(obj.bbox)  # [635.0, 458.0, 704.0, 508.0]
-        
-            # get the detection mask, it's of RLE format
-            print(obj.mask.counts)  # ]o`f08fa14M3L2O2M2O1O1O1O1N2O1N2O1N2N3M2O3L3M3N2M2N3N1N2O...
-        
-            # convert the RLE format to RGBA image
-            mask_image = task.rle2rgba(obj.mask)
-            print(mask_image.size)  # (1600, 1170)
-        
-            # save the image to file
-            mask_image.save(f"data/mask_{idx}.png")
-        
-        ```
-        
-        For more details on using the SDK, please refer to the [DDS CloudAPI SDK Reference](https://cloudapi-sdk.deepdataspace.com)
-        
-        ## 3. Apply for an API Token
-        Our API is in private beta. Contact us at [deepdataspace_dm@idea.edu.cn](mailto:deepdataspace_dm@idea.edu.cn) to apply for a free API token.  
-        Please include a brief introduction to your research or project and how you plan to use the API in your application.  
-        We're dedicated to supporting academic research and education and welcome any questions or suggestions.
-        
-        ## 4. License
-        
-        This project is released under
-        the [Apache 2.0 License](https://github.com/deepdataspace/dds-cloudapi-sdk/blob/main/LICENSE).
-        
-        ```text
-        Copyright 2023-present, IDEA
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy==1.24.4
+Requires-Dist: pillow==10.2.0
+Requires-Dist: pydantic==2.6.3
+Requires-Dist: requests==2.31.0
+
+# dds-cloudapi-sdk
+
+---
+
+<div align="center">
+<p align="center">
+
+<!-- prettier-ignore -->
+**The Python SDK for the DDS Cloud API.**
+---
+
+<!-- prettier-ignore -->
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
+[![PyPI python](https://img.shields.io/pypi/pyversions/dds-cloudapi-sdk)](https://pypi.org/project/dds-cloudapi-sdk)
+[![PyPI version](https://img.shields.io/pypi/v/dds-cloudapi-sdk)](https://pypi.org/project/dds-cloudapi-sdk)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/dds-cloudapi-sdk)
+
+</p>
+</div>
+
+---
+
+The dds-cloudapi-sdk is a Python package designed to simplify interactions with the DDS Cloud API. It features:
+
+- **Straightforward** APIs
+- **Unified** interfaces
+- **Handy** utilities
+
+## Installation
+
+You can get the SDK library directly from PyPi:
+
+```shell
+pip install dds-cloudapi-sdk
+```
+
+## Quick Start
+
+Below is a straightforward example for the popular IVP algorithm:
+
+```python
+# 1. Initialize the client with your API token.
+from dds_cloudapi_sdk import Config
+from dds_cloudapi_sdk import Client
+
+token = "Your API Token Here"
+config = Config(token)
+client = Client(config)
+
+# 2. Upload local image to the server and get the URL.
+infer_image_url = "https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg"
+# infer_image_url = client.upload_file("path/to/infer/image.jpg")  # you can also upload local file for processing
+prompt_image_url = infer_image_url  # use the same image for prompt
+
+# 3. Create a task with proper parameters.
+from dds_cloudapi_sdk.tasks import IVPTask
+from dds_cloudapi_sdk.tasks import RectPrompt
+from dds_cloudapi_sdk.tasks import LabelTypes
+
+task = IVPTask(
+    prompt_image_url=prompt_image_url,
+    prompts=[RectPrompt(rect=[475.18, 550.20, 548.10, 599.92], is_positive=True)],
+    infer_image_url=infer_image_url,
+    infer_label_types=[LabelTypes.BBox, LabelTypes.Mask],  # infer both bbox and mask
+)
+
+# 4. Run the task and get the result.
+client.run_task(task)
+
+# 5. Parse the result.
+from dds_cloudapi_sdk.tasks.ivp import TaskResult
+
+result: TaskResult = task.result
+
+mask_url = result.mask_url  # the image url with all masks drawn on
+objects = result.objects  # the list of detected objects
+for idx, obj in enumerate(objects):
+    # get the detection score
+    print(obj.score)  # 0.42
+
+    # get the detection bbox
+    print(obj.bbox)  # [635.0, 458.0, 704.0, 508.0]
+
+    # get the detection mask, it's of RLE format
+    print(obj.mask.counts)  # ]o`f08fa14M3L2O2M2O1O1O1O1N2O1N2O1N2N3M2O3L3M3N2M2N3N1N2O...
+
+    # convert the RLE format to RGBA image
+    mask_image = task.rle2rgba(obj.mask)
+    print(mask_image.size)  # (1600, 1170)
+
+    # save the image to file
+    mask_image.save(f"data/mask_{idx}.png")
+
+```
+
+For more details on using the SDK, please refer to the [DDS CloudAPI SDK Reference](https://cloudapi-sdk.deepdataspace.com)
+
+## 3. Apply for an API Token
+Our API is in private beta. Contact us at [deepdataspace_dm@idea.edu.cn](mailto:deepdataspace_dm@idea.edu.cn) to apply for a free API token.  
+Please include a brief introduction to your research or project and how you plan to use the API in your application.  
+We're dedicated to supporting academic research and education and welcome any questions or suggestions.
+
+## 4. License
+
+This project is released under
+the [Apache 2.0 License](https://github.com/deepdataspace/dds-cloudapi-sdk/blob/main/LICENSE).
+
+```text
+Copyright 2023-present, IDEA
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+```
```

### Comparing `dds-cloudapi-sdk-0.1.1/README.md` & `dds-cloudapi-sdk-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/client.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/client.py`

 * *Files identical despite different names*

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/config.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     return endpoint
 
 
 class Config:
     """
     The configuration representation for the SDK client.
 
-    :param token: The API token of your DDS account. Currently, you can apply for an API token by sending email to deepdataspace_dm@idea.edu.cn.
+    :param token: The API token of your DDS account. Currently, you can apply for an API token with `this form <https://deepdataspace.com/request_api>`_.
 
     """
 
     def __init__(self, token: str):
         """
         Initialize a configuration with API token.
         """
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/__init__.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
     print(task.result)
 
 """
 
 from dds_cloudapi_sdk.tasks.base import LabelTypes
 from dds_cloudapi_sdk.tasks.base import TaskStatus
+from dds_cloudapi_sdk.tasks.detection import DetectionModel
+from dds_cloudapi_sdk.tasks.detection import DetectionTarget
+from dds_cloudapi_sdk.tasks.detection import DetectionTask
 from dds_cloudapi_sdk.tasks.gsam import BaseGSAMTask
 from dds_cloudapi_sdk.tasks.gsam import TinyGSAMTask
 from dds_cloudapi_sdk.tasks.ivp import IVPTask
 from dds_cloudapi_sdk.tasks.prompt import *
 from dds_cloudapi_sdk.tasks.trex_embd_customize import TRexEmbdCustomize
 from dds_cloudapi_sdk.tasks.trex_embd_infer import TRexEmbdInfer
 from dds_cloudapi_sdk.tasks.trex_generic import TRexGenericInfer
@@ -43,9 +46,12 @@
     "BatchEmbdInfer",
     "IVPTask",
     "TinyGSAMTask",
     "BaseGSAMTask",
     "TRexGenericInfer",
     "TRexInteractiveInfer",
     "TRexEmbdCustomize",
-    "TRexEmbdInfer"
+    "TRexEmbdInfer",
+    "DetectionTask",
+    "DetectionModel",
+    "DetectionTarget"
 ]
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/gsam.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/gsam.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,23 +195,23 @@
     from dds_cloudapi_sdk import Config
     from dds_cloudapi_sdk import Client
     from dds_cloudapi_sdk import TextPrompt
 
     config = Config(test_token)
     client = Client(config)
     task = TinyGSAMTask(
-        "https://dds-frontend.oss-cn-shenzhen.aliyuncs.com/static_files/playground/grounded_sam/05.jpg",
+        "https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/grounded_sam/iron_man.jpg",
         [TextPrompt(text="iron man")]
     )
 
     client.run_task(task)
     print(task.result)
 
     task = BaseGSAMTask(
-        "https://dds-frontend.oss-cn-shenzhen.aliyuncs.com/static_files/playground/grounded_sam/05.jpg",
+        "https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/grounded_sam/iron_man.jpg",
         [TextPrompt(text="iron man")]
     )
 
     client.run_task(task)
     print(task.result)
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/ivp.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/ivp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Interactive Visual Prompting (iVP) is an interactive object detection and counting system based on the T-Rex model independently developed by the IDEA CVR team.
+Interactive Visual Prompting (IVP) is an interactive object detection and counting system based on the T-Rex model independently developed by the IDEA CVR team.
 
 It enables object detection and counting through visual prompts without any training, truly realizing a single visual model applicable to multiple scenarios.
 
 It particularly excels in counting objects in dense or overlapping scenes.
 
 This algorithm is available in DDS CloudAPI SDK through IVPTask.
 """
@@ -189,37 +189,37 @@
 
     from dds_cloudapi_sdk import Config
     from dds_cloudapi_sdk import Client
 
     config = Config(test_token)
     client = Client(config)
     task = IVPTask(
-        prompt_image_url="https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg",
+        prompt_image_url="https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg",
         prompts=[RectPrompt(rect=[475.18413597733706, 550.1983002832861, 548.1019830028329, 599.915014164306])],
-        infer_image_url="https://dev.deepdataspace.com/static/04_b.ae28c1d6.jpg",
+        infer_image_url="https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg",
         infer_label_types=[LabelTypes.BBox],
     )
 
     client.run_task(task)
     print(task.result)
 
     task = IVPTask(
-        prompt_image_url="https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg",
+        prompt_image_url="https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg",
         prompts=[RectPrompt(rect=[475.18413597733706, 550.1983002832861, 548.1019830028329, 599.915014164306])],
-        infer_image_url="https://dev.deepdataspace.com/static/04_b.ae28c1d6.jpg",
+        infer_image_url="https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg",
         infer_label_types=[LabelTypes.Mask],
     )
 
     client.run_task(task)
     print(task.result)
 
     task = IVPTask(
-        prompt_image_url="https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg",
+        prompt_image_url="https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg",
         prompts=[RectPrompt(rect=[475.18413597733706, 550.1983002832861, 548.1019830028329, 599.915014164306])],
-        infer_image_url="https://dev.deepdataspace.com/static/04_b.ae28c1d6.jpg",
+        infer_image_url="https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg",
         infer_label_types=[LabelTypes.Mask, LabelTypes.BBox],
     )
 
     client.run_task(task)
     print(task.result)
     for obj in task.result.objects:
         if obj.mask is not None:
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/prompt.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,71 +69,71 @@
     :param image: the image url the point prompts are acting on, if not provided, the infer image url in context will be used
     :param category_id: the category id of the points
     """
 
     points: List[List[float]]  #: a list of point locations in [[x1, y1], [x2, y2]]
 
     image: str = None  #: the image url the point prompts are acting on
-    category_id: int = None  #: the category id of the rects
+    category_id: int = None  #: the category id of the points, only required for :class:`TRexInteractiveInfer <dds_cloudapi_sdk.tasks.trex_interactive.TRexInteractiveInfer>` task.
 
 
 class BatchRectPrompt(pydantic.BaseModel):
     """
     A batch of rectangle prompts.
 
     :param rects: a list of rect locations in [[[upper_left_x, upper_left_y, lower_right_x, lower_right_y], ...]
     :param image: the image url the rectangle prompts are acting on
     :param category_id: the category id of the rects
     """
 
     rects: List[List[float]]  #: a list of rect locations in [[[upper_left_x, upper_left_y, lower_right_x, lower_right_y], ...]
 
     image: str = None  #: the image url the rectangle prompts are acting on, if not provided, the infer image url in context will be used
-    category_id: int = None  #: the category id of the rects
+    category_id: int = None  #: the category id of the rects, only required for :class:`TRexInteractiveInfer <dds_cloudapi_sdk.tasks.trex_interactive.TRexInteractiveInfer>` task.
 
 
 class BatchEmbdPrompt(pydantic.BaseModel):
     """
     A batch of embd prompts.
 
     :param embd: the embedding file url
     :param category_id: the category id of the rects
     """
 
     embd: str = None  #: the embedding file url
-    category_id: int  #: the category id of the rects
+    category_id: int  #: the category id of the objects inferred by this embedding file
 
 
 class BatchPointInfer(pydantic.BaseModel):
     """
     An infer image with batch point prompts.
 
     :param image: the image url to be inferred on
     :param prompts: a list of :class:`BatchPointPrompt <dds_cloudapi_sdk.tasks.prompt.BatchPointPrompt>`
     """
 
     image: str  #: the image url to be inferred on
-    prompts: List[BatchPointPrompt]  # a list of :class:`BatchPointPrompt <dds_cloudapi_sdk.tasks.prompt.BatchPointPrompt>`
+    prompts: List[BatchPointPrompt]  #: a list of :class:`BatchPointPrompt <dds_cloudapi_sdk.tasks.prompt.BatchPointPrompt>`
 
 
 class BatchRectInfer(pydantic.BaseModel):
     """
     An infer image with batch rect prompts.
 
     :param image: the image url to be inferred on
     :param prompts: a list of :class:`BatchRectPrompt <dds_cloudapi_sdk.tasks.prompt.BatchRectPrompt>`
     """
 
     image: str  #: the image url to be inferred on
-    prompts: List[BatchRectPrompt]  # a list of :class:`BatchRectPrompt <dds_cloudapi_sdk.tasks.prompt.BatchRectPrompt>`
+    prompts: List[BatchRectPrompt]  #: a list of :class:`BatchRectPrompt <dds_cloudapi_sdk.tasks.prompt.BatchRectPrompt>`
 
 
 class BatchEmbdInfer(pydantic.BaseModel):
     """
     An infer image with batch embd prompts.
 
     :param image: the image url to be inferred on
     :param prompts: a list of :class:`BatchEmbdPrompt <dds_cloudapi_sdk.tasks.prompt.BatchEmbdPrompt>`
     """
 
     image: str  #: the image url to be inferred on
-    prompts: List[BatchEmbdPrompt]  # a list of :class:`BatchEmbdPrompt <dds_cloudapi_sdk.tasks.prompt.BatchEmbdPrompt>`
+    prompts: List[BatchEmbdPrompt]  #: a list of :class:`BatchEmbdPrompt <dds_cloudapi_sdk.tasks.prompt.BatchEmbdPrompt>`
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/trex_embd_customize.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/trex_embd_customize.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     from dds_cloudapi_sdk import Config
     from dds_cloudapi_sdk import Client
 
     config = Config(test_token)
     client = Client(config)
 
-    image_url = "https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg"
+    image_url = "https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg"
 
     batch_prompts = [
         BatchRectPrompt(
             image=image_url,
             rects=[[475.18413597733706, 550.1983002832861, 548.1019830028329, 599.915014164306]]
         )
     ]
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/trex_embd_infer.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/trex_embd_infer.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     from dds_cloudapi_sdk import Config
     from dds_cloudapi_sdk import Client
 
     config = Config(test_token)
     client = Client(config)
 
-    image_url = "https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg"
+    image_url = "https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg"
 
     batch_prompts = [
         BatchRectPrompt(
             image=image_url,
             rects=[[475.18413597733706, 550.1983002832861, 548.1019830028329, 599.915014164306]]
         )
     ]
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/trex_generic.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/trex_generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,20 +105,20 @@
     from dds_cloudapi_sdk import Client
 
     config = Config(test_token)
     client = Client(config)
 
     batch_prompts = [
         BatchRectPrompt(
-            image="https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg",
+            image="https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg",
             rects=[[475.18413597733706, 550.1983002832861, 548.1019830028329, 599.915014164306]]
         )
     ]
     task = TRexGenericInfer(
-        image_url="https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg",
+        image_url="https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg",
         batch_prompts=batch_prompts
     )
 
     client.run_task(task)
     for obj in task.result.objects:
         print(obj)
         break
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk/tasks/trex_interactive.py` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk/tasks/trex_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     from dds_cloudapi_sdk import Config
     from dds_cloudapi_sdk import Client
 
     config = Config(test_token)
     client = Client(config)
 
-    infer_image = "https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg"
+    infer_image = "https://algosplt.oss-cn-shenzhen.aliyuncs.com/test_files/tasks/ivp/04_b.jpg"
 
     infer_1 = BatchRectInfer(
         image=infer_image,
         prompts=[
             BatchRectPrompt(category_id=1, rects=[[475.18413597733706, 550.1983002832861, 548.1019830028329, 599.915014164306]])
         ]
     )
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk.egg-info/PKG-INFO` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,144 +1,147 @@
 Metadata-Version: 2.1
 Name: dds-cloudapi-sdk
-Version: 0.1.1
+Version: 0.2.0
 Summary: The SDK for calling deepdataspace cloud API.
 Home-page: https://github.com/deepdataspace/dds-cloudapi-sdk
 Author: cvr@idea
-License: UNKNOWN
-Description: # dds-cloudapi-sdk
-        
-        ---
-        
-        <div align="center">
-        <p align="center">
-        
-        <!-- prettier-ignore -->
-        **The Python SDK for the DDS Cloud API.**
-        ---
-        
-        <!-- prettier-ignore -->
-        
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
-        [![PyPI python](https://img.shields.io/pypi/pyversions/dds-cloudapi-sdk)](https://pypi.org/project/dds-cloudapi-sdk)
-        [![PyPI version](https://img.shields.io/pypi/v/dds-cloudapi-sdk)](https://pypi.org/project/dds-cloudapi-sdk)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/dds-cloudapi-sdk)
-        
-        </p>
-        </div>
-        
-        ---
-        
-        The dds-cloudapi-sdk is a Python package designed to simplify interactions with the DDS Cloud API. It features:
-        
-        - **Straightforward** APIs
-        - **Unified** interfaces
-        - **Handy** utilities
-        
-        ## Installation
-        
-        You can get the SDK library directly from PyPi:
-        
-        ```shell
-        pip install dds-cloudapi-sdk
-        ```
-        
-        ## Quick Start
-        
-        Below is a straightforward example for the popular IVP algorithm:
-        
-        ```python
-        # 1. Initialize the client with your API token.
-        from dds_cloudapi_sdk import Config
-        from dds_cloudapi_sdk import Client
-        
-        token = "Your API Token Here"
-        config = Config(token)
-        client = Client(config)
-        
-        # 2. Upload local image to the server and get the URL.
-        infer_image_url = "https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg"
-        # infer_image_url = client.upload_file("path/to/infer/image.jpg")  # you can also upload local file for processing
-        prompt_image_url = infer_image_url  # use the same image for prompt
-        
-        # 3. Create a task with proper parameters.
-        from dds_cloudapi_sdk.tasks import IVPTask
-        from dds_cloudapi_sdk.tasks import RectPrompt
-        from dds_cloudapi_sdk.tasks import LabelTypes
-        
-        task = IVPTask(
-            prompt_image_url=prompt_image_url,
-            prompts=[RectPrompt(rect=[475.18, 550.20, 548.10, 599.92], is_positive=True)],
-            infer_image_url=infer_image_url,
-            infer_label_types=[LabelTypes.BBox, LabelTypes.Mask],  # infer both bbox and mask
-        )
-        
-        # 4. Run the task and get the result.
-        client.run_task(task)
-        
-        # 5. Parse the result.
-        from dds_cloudapi_sdk.tasks.ivp import TaskResult
-        
-        result: TaskResult = task.result
-        
-        mask_url = result.mask_url  # the image url with all masks drawn on
-        objects = result.objects  # the list of detected objects
-        for idx, obj in enumerate(objects):
-            # get the detection score
-            print(obj.score)  # 0.42
-        
-            # get the detection bbox
-            print(obj.bbox)  # [635.0, 458.0, 704.0, 508.0]
-        
-            # get the detection mask, it's of RLE format
-            print(obj.mask.counts)  # ]o`f08fa14M3L2O2M2O1O1O1O1N2O1N2O1N2N3M2O3L3M3N2M2N3N1N2O...
-        
-            # convert the RLE format to RGBA image
-            mask_image = task.rle2rgba(obj.mask)
-            print(mask_image.size)  # (1600, 1170)
-        
-            # save the image to file
-            mask_image.save(f"data/mask_{idx}.png")
-        
-        ```
-        
-        For more details on using the SDK, please refer to the [DDS CloudAPI SDK Reference](https://cloudapi-sdk.deepdataspace.com)
-        
-        ## 3. Apply for an API Token
-        Our API is in private beta. Contact us at [deepdataspace_dm@idea.edu.cn](mailto:deepdataspace_dm@idea.edu.cn) to apply for a free API token.  
-        Please include a brief introduction to your research or project and how you plan to use the API in your application.  
-        We're dedicated to supporting academic research and education and welcome any questions or suggestions.
-        
-        ## 4. License
-        
-        This project is released under
-        the [Apache 2.0 License](https://github.com/deepdataspace/dds-cloudapi-sdk/blob/main/LICENSE).
-        
-        ```text
-        Copyright 2023-present, IDEA
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy==1.24.4
+Requires-Dist: pillow==10.2.0
+Requires-Dist: pydantic==2.6.3
+Requires-Dist: requests==2.31.0
+
+# dds-cloudapi-sdk
+
+---
+
+<div align="center">
+<p align="center">
+
+<!-- prettier-ignore -->
+**The Python SDK for the DDS Cloud API.**
+---
+
+<!-- prettier-ignore -->
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
+[![PyPI python](https://img.shields.io/pypi/pyversions/dds-cloudapi-sdk)](https://pypi.org/project/dds-cloudapi-sdk)
+[![PyPI version](https://img.shields.io/pypi/v/dds-cloudapi-sdk)](https://pypi.org/project/dds-cloudapi-sdk)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/dds-cloudapi-sdk)
+
+</p>
+</div>
+
+---
+
+The dds-cloudapi-sdk is a Python package designed to simplify interactions with the DDS Cloud API. It features:
+
+- **Straightforward** APIs
+- **Unified** interfaces
+- **Handy** utilities
+
+## Installation
+
+You can get the SDK library directly from PyPi:
+
+```shell
+pip install dds-cloudapi-sdk
+```
+
+## Quick Start
+
+Below is a straightforward example for the popular IVP algorithm:
+
+```python
+# 1. Initialize the client with your API token.
+from dds_cloudapi_sdk import Config
+from dds_cloudapi_sdk import Client
+
+token = "Your API Token Here"
+config = Config(token)
+client = Client(config)
+
+# 2. Upload local image to the server and get the URL.
+infer_image_url = "https://dev.deepdataspace.com/static/04_a.ae28c1d6.jpg"
+# infer_image_url = client.upload_file("path/to/infer/image.jpg")  # you can also upload local file for processing
+prompt_image_url = infer_image_url  # use the same image for prompt
+
+# 3. Create a task with proper parameters.
+from dds_cloudapi_sdk.tasks import IVPTask
+from dds_cloudapi_sdk.tasks import RectPrompt
+from dds_cloudapi_sdk.tasks import LabelTypes
+
+task = IVPTask(
+    prompt_image_url=prompt_image_url,
+    prompts=[RectPrompt(rect=[475.18, 550.20, 548.10, 599.92], is_positive=True)],
+    infer_image_url=infer_image_url,
+    infer_label_types=[LabelTypes.BBox, LabelTypes.Mask],  # infer both bbox and mask
+)
+
+# 4. Run the task and get the result.
+client.run_task(task)
+
+# 5. Parse the result.
+from dds_cloudapi_sdk.tasks.ivp import TaskResult
+
+result: TaskResult = task.result
+
+mask_url = result.mask_url  # the image url with all masks drawn on
+objects = result.objects  # the list of detected objects
+for idx, obj in enumerate(objects):
+    # get the detection score
+    print(obj.score)  # 0.42
+
+    # get the detection bbox
+    print(obj.bbox)  # [635.0, 458.0, 704.0, 508.0]
+
+    # get the detection mask, it's of RLE format
+    print(obj.mask.counts)  # ]o`f08fa14M3L2O2M2O1O1O1O1N2O1N2O1N2N3M2O3L3M3N2M2N3N1N2O...
+
+    # convert the RLE format to RGBA image
+    mask_image = task.rle2rgba(obj.mask)
+    print(mask_image.size)  # (1600, 1170)
+
+    # save the image to file
+    mask_image.save(f"data/mask_{idx}.png")
+
+```
+
+For more details on using the SDK, please refer to the [DDS CloudAPI SDK Reference](https://cloudapi-sdk.deepdataspace.com)
+
+## 3. Apply for an API Token
+Our API is in private beta. Contact us at [deepdataspace_dm@idea.edu.cn](mailto:deepdataspace_dm@idea.edu.cn) to apply for a free API token.  
+Please include a brief introduction to your research or project and how you plan to use the API in your application.  
+We're dedicated to supporting academic research and education and welcome any questions or suggestions.
+
+## 4. License
+
+This project is released under
+the [Apache 2.0 License](https://github.com/deepdataspace/dds-cloudapi-sdk/blob/main/LICENSE).
+
+```text
+Copyright 2023-present, IDEA
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+```
```

### Comparing `dds-cloudapi-sdk-0.1.1/dds_cloudapi_sdk.egg-info/SOURCES.txt` & `dds-cloudapi-sdk-0.2.0/dds_cloudapi_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dds_cloudapi_sdk.egg-info/PKG-INFO
 dds_cloudapi_sdk.egg-info/SOURCES.txt
 dds_cloudapi_sdk.egg-info/dependency_links.txt
 dds_cloudapi_sdk.egg-info/requires.txt
 dds_cloudapi_sdk.egg-info/top_level.txt
 dds_cloudapi_sdk/tasks/__init__.py
 dds_cloudapi_sdk/tasks/base.py
+dds_cloudapi_sdk/tasks/detection.py
 dds_cloudapi_sdk/tasks/gsam.py
 dds_cloudapi_sdk/tasks/ivp.py
 dds_cloudapi_sdk/tasks/prompt.py
 dds_cloudapi_sdk/tasks/trex_embd_customize.py
 dds_cloudapi_sdk/tasks/trex_embd_infer.py
 dds_cloudapi_sdk/tasks/trex_generic.py
 dds_cloudapi_sdk/tasks/trex_interactive.py
```

### Comparing `dds-cloudapi-sdk-0.1.1/setup.py` & `dds-cloudapi-sdk-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-version = "0.1.1"
+from dds_cloudapi_sdk import version
 
 description = "The SDK for calling deepdataspace cloud API."
 with open("README.md", "r", encoding="utf8") as fp:
     long_description = fp.read()
 
 url = "https://github.com/deepdataspace/dds-cloudapi-sdk"
 author = "cvr@idea"
```

