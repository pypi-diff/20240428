# Comparing `tmp/python_gemini_api-2.4.7.tar.gz` & `tmp/python_gemini_api-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_gemini_api-2.4.7.tar", last modified: Sat Apr 27 13:17:03 2024, max compression
+gzip compressed data, was "python_gemini_api-2.4.8.tar", last modified: Sun Apr 28 14:01:14 2024, max compression
```

## Comparing `python_gemini_api-2.4.7.tar` & `python_gemini_api-2.4.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.538878 python_gemini_api-2.4.7/
--rw-rw-rw-   0        0        0     1097 2024-04-24 10:59:38.000000 python_gemini_api-2.4.7/LICENSE
--rw-rw-rw-   0        0        0    36504 2024-04-27 13:17:03.537298 python_gemini_api-2.4.7/PKG-INFO
--rw-rw-rw-   0        0        0    35177 2024-04-27 13:15:58.000000 python_gemini_api-2.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.475836 python_gemini_api-2.4.7/gemini/
--rw-rw-rw-   0        0        0     1511 2024-04-27 13:15:12.000000 python_gemini_api-2.4.7/gemini/__init__.py
--rw-rw-rw-   0        0        0    15192 2024-03-18 04:20:24.000000 python_gemini_api-2.4.7/gemini/async_client.py
--rw-rw-rw-   0        0        0    19096 2024-04-17 13:21:33.000000 python_gemini_api-2.4.7/gemini/client.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.477836 python_gemini_api-2.4.7/gemini/src/
--rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.7/gemini/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.482330 python_gemini_api-2.4.7/gemini/src/extensions/
--rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.7/gemini/src/extensions/__init__.py
--rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.7/gemini/src/extensions/replit.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.491676 python_gemini_api-2.4.7/gemini/src/misc/
--rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.7/gemini/src/misc/__init__.py
--rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.7/gemini/src/misc/constants.py
--rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.7/gemini/src/misc/decorator.py
--rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.7/gemini/src/misc/exceptions.py
--rw-rw-rw-   0        0        0     4487 2024-04-17 09:46:59.000000 python_gemini_api-2.4.7/gemini/src/misc/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.496863 python_gemini_api-2.4.7/gemini/src/model/
--rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.7/gemini/src/model/__init__.py
--rw-rw-rw-   0        0        0     8611 2024-03-18 04:29:31.000000 python_gemini_api-2.4.7/gemini/src/model/image.py
--rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python_gemini_api-2.4.7/gemini/src/model/output.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.503762 python_gemini_api-2.4.7/gemini/src/model/parser/
--rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.7/gemini/src/model/parser/__init__.py
--rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.7/gemini/src/model/parser/base.py
--rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.7/gemini/src/model/parser/custom_parser.py
--rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.7/gemini/src/model/parser/response_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.506158 python_gemini_api-2.4.7/gemini/src/modules/
--rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.7/gemini/src/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.513313 python_gemini_api-2.4.7/gemini/src/modules/openrouter/
--rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.7/gemini/src/modules/openrouter/__init__.py
--rw-rw-rw-   0        0        0     3048 2024-04-27 13:13:20.000000 python_gemini_api-2.4.7/gemini/src/modules/openrouter/async_client.py
--rw-rw-rw-   0        0        0     4753 2024-04-24 12:56:08.000000 python_gemini_api-2.4.7/gemini/src/modules/openrouter/client.py
--rw-rw-rw-   0        0        0      505 2024-04-24 13:06:12.000000 python_gemini_api-2.4.7/gemini/src/modules/openrouter/const.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.518672 python_gemini_api-2.4.7/gemini/src/modules/voice/
--rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.7/gemini/src/modules/voice/__init__.py
--rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.7/gemini/src/modules/voice/google.py
--rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.7/gemini/src/modules/voice/openai.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:17:03.534679 python_gemini_api-2.4.7/python_gemini_api.egg-info/
--rw-rw-rw-   0        0        0    36504 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-27 13:17:03.000000 python_gemini_api-2.4.7/python_gemini_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 13:17:03.538878 python_gemini_api-2.4.7/setup.cfg
--rw-rw-rw-   0        0        0     2204 2024-04-27 13:14:03.000000 python_gemini_api-2.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.342026 python_gemini_api-2.4.8/
+-rw-rw-rw-   0        0        0     1097 2024-04-24 10:59:38.000000 python_gemini_api-2.4.8/LICENSE
+-rw-rw-rw-   0        0        0    37858 2024-04-28 14:01:14.340018 python_gemini_api-2.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0    36531 2024-04-28 14:00:17.000000 python_gemini_api-2.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.288352 python_gemini_api-2.4.8/gemini/
+-rw-rw-rw-   0        0        0     1511 2024-04-28 14:00:46.000000 python_gemini_api-2.4.8/gemini/__init__.py
+-rw-rw-rw-   0        0        0    15168 2024-04-28 13:24:37.000000 python_gemini_api-2.4.8/gemini/async_client.py
+-rw-rw-rw-   0        0        0    19528 2024-04-28 13:24:49.000000 python_gemini_api-2.4.8/gemini/client.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.289357 python_gemini_api-2.4.8/gemini/src/
+-rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.8/gemini/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.293360 python_gemini_api-2.4.8/gemini/src/extensions/
+-rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.8/gemini/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.8/gemini/src/extensions/replit.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.301358 python_gemini_api-2.4.8/gemini/src/misc/
+-rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.8/gemini/src/misc/__init__.py
+-rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.8/gemini/src/misc/constants.py
+-rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.8/gemini/src/misc/decorator.py
+-rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.8/gemini/src/misc/exceptions.py
+-rw-rw-rw-   0        0        0     4487 2024-04-17 09:46:59.000000 python_gemini_api-2.4.8/gemini/src/misc/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.307601 python_gemini_api-2.4.8/gemini/src/model/
+-rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.8/gemini/src/model/__init__.py
+-rw-rw-rw-   0        0        0     9159 2024-04-28 13:59:51.000000 python_gemini_api-2.4.8/gemini/src/model/image.py
+-rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python_gemini_api-2.4.8/gemini/src/model/output.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.314139 python_gemini_api-2.4.8/gemini/src/model/parser/
+-rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.8/gemini/src/model/parser/__init__.py
+-rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.8/gemini/src/model/parser/base.py
+-rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.8/gemini/src/model/parser/custom_parser.py
+-rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.8/gemini/src/model/parser/response_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.316139 python_gemini_api-2.4.8/gemini/src/modules/
+-rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.8/gemini/src/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.322616 python_gemini_api-2.4.8/gemini/src/modules/openrouter/
+-rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.8/gemini/src/modules/openrouter/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-04-27 13:13:20.000000 python_gemini_api-2.4.8/gemini/src/modules/openrouter/async_client.py
+-rw-rw-rw-   0        0        0     4753 2024-04-24 12:56:08.000000 python_gemini_api-2.4.8/gemini/src/modules/openrouter/client.py
+-rw-rw-rw-   0        0        0      505 2024-04-24 13:06:12.000000 python_gemini_api-2.4.8/gemini/src/modules/openrouter/const.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.326744 python_gemini_api-2.4.8/gemini/src/modules/voice/
+-rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.8/gemini/src/modules/voice/__init__.py
+-rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.8/gemini/src/modules/voice/google.py
+-rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.8/gemini/src/modules/voice/openai.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.337736 python_gemini_api-2.4.8/python_gemini_api.egg-info/
+-rw-rw-rw-   0        0        0    37858 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 14:01:14.342026 python_gemini_api-2.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     2204 2024-04-27 13:14:03.000000 python_gemini_api-2.4.8/setup.py
```

### Comparing `python_gemini_api-2.4.7/LICENSE` & `python_gemini_api-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/PKG-INFO` & `python_gemini_api-2.4.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: python-gemini-api
-Version: 2.4.7
-Summary: The python package that returns Response of Google Gemini through API.
-Home-page: https://github.com/dsdanielpark/Gemini-API
-Author: Daniel Park
-Author-email: parkminwoo1991@gmail.com
-Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx[http2]>=0.20.0
-Requires-Dist: requests
-Requires-Dist: browser_cookie3
-Requires-Dist: loguru
-Requires-Dist: pydantic
-Requires-Dist: aiohttp
-Provides-Extra: voice
-Requires-Dist: gTTS; extra == "voice"
-Requires-Dist: SpeechRecognition; extra == "voice"
-Requires-Dist: openai; extra == "voice"
-Requires-Dist: anthropic; extra == "voice"
-
 
 # <img src="https://www.gstatic.com/lamda/images/favicon_v1_150160cddff7f294ce30.svg" width="35px" alt="Gemini Icon" /> Gemini API  <a href="https://pypi.org/project/python-gemini-api/"> <img alt="PyPI" src="https://img.shields.io/pypi/v/python-gemini-api?color=black"></a>
 
 
 <p align="right">
     <a href="https://github.com/dsdanielpark/Gemini-API"><img alt="pip download" src="https://img.shields.io/badge/pip_install-python_gemini_api-black"></a> 
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
@@ -179,26 +146,26 @@
 
 ## Quick Start
 
 **Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
-cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"<key>" : "<value>"} # Cookies may vary by account or region. Consider sending the entire cookie file.
 client = Gemini(cookies=cookies) # You can use various args
 
 response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
 **Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
-cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"<key>" : "<value>"}
 client = Gemini(cookies=cookies) # You can use various args
 
 response = client.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
@@ -254,14 +221,19 @@
 <br>
 
 ### # 02. Generate content
 Returns Gemini's response, but the first one might be empty. 
 
 
 ```python
+from gemini import Gemini
+
+cookies = {}
+client = Gemini(cookies=cookies)
+
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = client.generate_content(prompt)
 print(response.payload)
 ```
 
 
 > [!IMPORTANT]
@@ -285,107 +257,136 @@
 
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-client = Gemini(cookies=cookies) # You can use various args
+cookies = {} 
+client = Gemini(cookies=cookies) 
 
 response_text, response_status = client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
 You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
+from gemini import Gemini
+
+cookies = {}
+client = Gemini(cookies=cookies)
+
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = client.generate_content(prompt)
 print(response.text)
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
 
 *Async downloader*
 
 ```python
+from gemini import Gemini, GeminiImage
+
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 generated_images = response.generated_images # Check generated images [Dict]
 
-await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
+await image_client.save(generated_images, "save_dir", cookies=cookies)
+# image_data_dict = await image_client.fetch_images_dict(generated_images, cookies=cookies)
+# await image_client.save_images(image_data_dict, "save_dir")
 ```
 
 
 <details><summary>Further</summary>
 
 *Display images in IPython*
   You can display the image or transmit it to another application in byte format.
   
   ```python
-  bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
-  from IPython.display import display, Image
   import io
+  from gemini import Gemini, GeminiImage
+  from IPython.display import display, Image
+  
+  cookies = {}
+  client = Gemini(cookies=cookies)
+  image_client = GeminiImage(cookies=cookies)
+
+  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies) # Save default folder is `cached`
 
 # You can use byte type image dict for printing images as follow:
-# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
 ```
 
 *Async downloader wrapper*
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
+    await image_client.save(generated_imagse, save_path=save_path, cookies=cookies)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  
     asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
 ```
 
 `GeminiImage.save` method logic
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    image_data_dict = await GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
-    await GeminiImage.save_images(image_data_dict, save_path=save_path)  
+    image_data_dict = await image_client.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
+    await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  # Check response images [Dict]
     asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
 ```
@@ -399,64 +400,82 @@
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
 
 *Async downloader*
 ```python
+from gemini import Gemini, GeminiImage
+
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
-await GeminiImage.save(response_images, "save_dir")
-# image_data_dict = await GeminiImage.fetch_images_dict(response_images)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
+await image_client.save(response_images, "save_dir")
+# image_data_dict = await image_client.fetch_images_dict(response_images)
+# await image_client.save_images(image_data_dict, "save_dir")
 ```
 
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
 GeminiImage.save_sync(response_images, save_path="save_dir")
 
 # You can use byte type image dict as follow:
-# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+# bytes_images_dict = image_client.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
 ```
 
 *Async downloader wrapper*
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
-async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    await GeminiImage.save(response_images, save_path=save_path, cookies=cookies)
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
+async def save_response_web_imagse(response_images, save_path="save_dir"):
+    await image_client.save(response_images, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     response_images = response.web_images  
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
 ```
 
 `GeminiImage.save` method logic
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    image_data_dict = await GeminiImage.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
-    await GeminiImage.save_images(image_data_dict, save_path=save_path)  
+    image_data_dict = await image_client.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
+    await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     response_images = response.web_images  # Check response images [Dict]
     asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
 ```
 
@@ -467,14 +486,15 @@
 ### # 07. Generate content from images
 Takes an image as input and returns a response.
 
 ```python
 image = 'folder/image.jpg'
 # image = open('folder/image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported.
 
+# Image file path or Byte-formatted image array
 response = client.generate_content("What does the text in this image say?", image=image)
 response.response_dict
 ```
 
 <br>
 
 ### # 08. Generate content using Google Services
@@ -570,25 +590,28 @@
 https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
 ### Use rotating proxies via [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api)
 
-If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
+If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks. The argument at the [Secure Sockets Layer (SSL)](https://en.wikipedia.org/wiki/Transport_Layer_Security) level may need to be added to the header. Use it in conjunction with `verify=False`.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
 
-client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client = Gemini(cookies=cookies, proxies=proxies, timeout=30, verify=False)
+client.session.header["crawlbaseAPI-Parameters"] = "country=US"
 client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
+
+
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
 import requests
 from gemini import Gemini, Headers
 
 cookies = {} 
@@ -693,17 +716,28 @@
 
 
 
 
 
 <br>
 
-## Sponsor, [Crawlbase](https://crawlbase.com/)
+## Sponsor
+
+<p align="left">
+  <img src="assets/crawlbase.png" width="240">
+</p>
+
 Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
 
+
+
+
+
+
+
 <br>
 
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md)
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
```

#### html2text {}

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.7 Summary: The
-python package that returns Response of Google Gemini through API. Home-page:
-https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
-parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
-Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
-Natural Language :: English Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
-Approved :: MIT License Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.9 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: httpx[http2]>=0.20.0 Requires-
-Dist: requests Requires-Dist: browser_cookie3 Requires-Dist: loguru Requires-
-Dist: pydantic Requires-Dist: aiohttp Provides-Extra: voice Requires-Dist:
-gTTS; extra == "voice" Requires-Dist: SpeechRecognition; extra == "voice"
-Requires-Dist: openai; extra == "voice" Requires-Dist: anthropic; extra ==
-"voice" # [Gemini Icon]Gemini API_[_P_y_P_I_]
+# [Gemini Icon]Gemini API_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
 ba79-d9f89b637324 An **unofficial* Python wrapper, [python-gemini-api](https://
 pypi.org/project/python-gemini-api/), is available for users facing frequent
@@ -126,26 +109,24 @@
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
 reference. > [!IMPORTANT] > Experiment with different Google accounts and
 browser settings to find a working cookie. Success may vary by IP and account
 status. Once connected, a cookie typically remains effective over a month. Keep
 testing until successful.
 ## Quick Start **Generate content:** returns parsed response. ```python from
-gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
-or region. Consider sending the entire cookie file. client = Gemini
+gemini import Gemini cookies = {"" : ""} # Cookies may vary by account or
+region. Consider sending the entire cookie file. client = Gemini
 (cookies=cookies) # You can use various args response = client.generate_content
 ("Hello, Gemini. What's the weather like in Seoul today?") response.payload ```
 **Generate content from image:** you can use image as input. ```python from
-gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
-or region. Consider sending the entire cookie file. client = Gemini
-(cookies=cookies) # You can use various args response = client.generate_content
-("What does the text in this image say?", image='folder/image.jpg')
-response.payload ``` > [!NOTE] > If the generate_content method returns an
-empty payload, try executing it again without reinitializing the Gemini object.
-
+gemini import Gemini cookies = {"" : ""} client = Gemini(cookies=cookies) # You
+can use various args response = client.generate_content("What does the text in
+this image say?", image='folder/image.jpg') response.payload ``` > [!NOTE] > If
+the generate_content method returns an empty payload, try executing it again
+without reinitializing the Gemini object.
 
 ## Usage *Setting language and Gemini version using environment variables:
 * Setting Gemini response language (Optional): Check supported languages [here]
 (https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
 Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
 Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
 Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
@@ -161,111 +142,123 @@
 (cookies=cookies) # client = Gemini(cookie_fp="folder/cookie_file.json") #
 (*.json, *.txt) are supported. # client = Gemini(auto_cookies=True) # Or use
 auto_cookies paprameter ``` ##### Auto Cookie Update For `auto_cookie` to be
 set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the
 browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3)
 enables automatic cookie collection, though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
-be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
+be empty. ```python from gemini import Gemini cookies = {} client = Gemini
+(cookies=cookies) prompt = "Hello, Gemini. What's the weather like in Seoul
 today?" response = client.generate_content(prompt) print(response.payload) ```
 > [!IMPORTANT] > DO NOT send same prompt repeatly. **If the session connects
 successfully and `generate_content` runs well, CLOSE Gemini website.** If
 Gemini web stays open in the browser, cookies may expire faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
 following structure: - *rcid*: returns the response candidate id of the chosen
 candidate. - *text*: returns the text of the chosen candidate. - *code*:
 returns the codes of the chosen candidate. - *web_images*: returns a list of
 web images from the chosen candidate. - *generated_images*: returns a list of
 generated images from the chosen candidate. - *payload*: returns the response
 dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
 fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
-cookies = {} # Cookies may vary by account or region. Consider sending the
-entire cookie file. client = Gemini(cookies=cookies) # You can use various args
-response_text, response_status = client.send_request("Hello, Gemini. What's the
-weather like in Seoul today?") print(response_text) ``` You can track the total
-number of requests made by accessing the `request_count` property within the
-`Gemini` class.
-### # 04. Text generation Returns text generated by Gemini. ```python prompt =
+cookies = {} client = Gemini(cookies=cookies) response_text, response_status =
+client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
+print(response_text) ``` You can track the total number of requests made by
+accessing the `request_count` property within the `Gemini` class.
+### # 04. Text generation Returns text generated by Gemini. ```python from
+gemini import Gemini cookies = {} client = Gemini(cookies=cookies) prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
-downloader* ```python response = client.generate_content("Create illustrations
-of Seoul, South Korea.") generated_images = response.generated_images # Check
-generated images [Dict] await GeminiImage.save(generated_images, "save_dir",
-cookies=cookies) # image_data_dict = await GeminiImage.fetch_images_dict
-(generated_images, cookies=cookies) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Further *Display images in IPython* You can
-display the image or transmit it to another application in byte format.
-```python bytes_images_dict = GeminiImage.fetch_images_dict_sync
-(generated_images, cookies) # Get bytes images dict from IPython.display import
-display, Image import io for image_name, image_bytes in bytes_images_dict.items
-(): print(image_name) image = Image(data=image_bytes) display(image) ``` *Sync
-downloader* ```python from gemini import Gemini, GeminiImage response =
-client.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# You can use byte type image dict for printing images as follow: #
-bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
-cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ``` *Async
-downloader wrapper* ```python import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): await GeminiImage.save
-(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
-function if __name__ == "__main__": cookies = {"key" : "value"}
-generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
-(generated_imagse, save_path="save_dir", cookies=cookies)) ```
-`GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): image_data_dict = await
-GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
-images dict asynchronously await GeminiImage.save_images(image_data_dict,
-save_path=save_path) # Run the async function if __name__ == "__main__":
-cookies = {"key" : "value"} generated_imagse = response.generated_imagse #
-Check response images [Dict] asyncio.run(save_generated_imagse
-(generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
-GeminiImage for image processing. `web_images` works without cookies, but for
-images like `generated_image` from Gemini, pass cookies. Cookies are needed to
-download images from Google's storage. Check the response or use existing
-cookies variable.
+downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+response = client.generate_content("Create illustrations of Seoul, South
+Korea.") generated_images = response.generated_images # Check generated images
+[Dict] await image_client.save(generated_images, "save_dir", cookies=cookies) #
+image_data_dict = await image_client.fetch_images_dict(generated_images,
+cookies=cookies) # await image_client.save_images(image_data_dict, "save_dir")
+``` Further *Display images in IPython* You can display the image or transmit
+it to another application in byte format. ```python import io from gemini
+import Gemini, GeminiImage from IPython.display import display, Image cookies =
+{} client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+bytes_images_dict = image_client.fetch_images_dict_sync(generated_images,
+cookies) # Get bytes images dict for image_name, image_bytes in
+bytes_images_dict.items(): print(image_name) image = Image(data=image_bytes)
+display(image) ``` *Sync downloader* ```python from gemini import Gemini,
+GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client =
+GeminiImage(cookies=cookies) response = client.generate_content("Create
+illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict]
+image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+# Save default folder is `cached` # You can use byte type image dict for
+printing images as follow: # bytes_images_dict =
+image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
+bytes images dict # image_client.save_images_sync(bytes_images_dict,
+path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
+```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies): await image_client.save(generated_imagse,
+save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+"__main__": cookies = {"key" : "value"} generated_imagse =
+response.generated_imagse asyncio.run(save_generated_imagse(generated_imagse,
+save_path="save_dir", cookies=cookies)) ``` `GeminiImage.save` method logic
+```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies): image_data_dict = await image_client.fetch_images_dict
+(generated_imagse, cookies=cookies) # Get bytes images dict asynchronously
+await image_client.save_images(image_data_dict, save_path=save_path) # Run the
+async function if __name__ == "__main__": cookies = {"key" : "value"}
+generated_imagse = response.generated_imagse # Check response images [Dict]
+asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies)) ``` > [!NOTE] > Use GeminiImage for image processing.
+`web_images` works without cookies, but for images like `generated_image` from
+Gemini, pass cookies. Cookies are needed to download images from Google's
+storage. Check the response or use existing cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Async downloader* ```python response = client.generate_content("Create
-illustrations of Seoul, South Korea.") response_images = response.web_images #
-Check generated images [Dict] await GeminiImage.save(response_images,
-"save_dir") # image_data_dict = await GeminiImage.fetch_images_dict
-(response_images) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Further *Sync downloader* ```python from gemini import Gemini, GeminiImage
+Gemini. *Async downloader* ```python from gemini import Gemini, GeminiImage
+cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
+(cookies=cookies) response = client.generate_content("Create illustrations of
+Seoul, South Korea.") response_images = response.web_images # Check generated
+images [Dict] await image_client.save(response_images, "save_dir") #
+image_data_dict = await image_client.fetch_images_dict(response_images) # await
+image_client.save_images(image_data_dict, "save_dir") ``` Further *Sync
+downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Please recommend a travel itinerary for
 Seoul.") response_images = response.web_images # Check response images [Dict]
 GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
-type image dict as follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync
+type image dict as follow: # bytes_images_dict = image_client.fetch_bytes_sync
 (response_images, cookies) # Get bytes images dict #
-GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
-``` *Async downloader wrapper* ```python import asyncio from gemini import
-Gemini, GeminiImage async def save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies): await GeminiImage.save(response_images,
-save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to
+path ``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_response_web_imagse
+(response_images, save_path="save_dir"): await image_client.save
+(response_images, save_path=save_path) # Run the async function if __name__ ==
 "__main__": cookies = {"key" : "value"} response_images = response.web_images
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
-gemini import Gemini, GeminiImage async def save_response_web_imagse
+asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
+``` `GeminiImage.save` method logic ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_response_web_imagse
 (response_images, save_path="save_dir", cookies=cookies): image_data_dict =
-await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
-bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
-save_path=save_path) # Run the async function if __name__ == "__main__":
-response_images = response.web_images # Check response images [Dict]
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies)) ```
+await image_client.fetch_images_dict(response_images, cookies=cookies) # Get
+bytes images dict asynchronously await image_client.save_images
+(image_data_dict, save_path=save_path) # Run the async function if __name__ ==
+"__main__": response_images = response.web_images # Check response images
+[Dict] asyncio.run(save_response_web_imagse(response_images,
+save_path="save_dir", cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
-image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
-client.generate_content("What does the text in this image say?", image=image)
-response.response_dict ```
+image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. # Image file
+path or Byte-formatted image array response = client.generate_content("What
+does the text in this image say?", image=image) response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
 gemini.google.com/extensions). Please refer to the [official notice](https://
 support.google.com/gemini/answer/13695044) and review the [privacy policies]
 (https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-
 1578971242&p=privacy_help&rd=1) for more details. *extention flags* ``` @Gmail,
 @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels,
@@ -319,18 +312,22 @@
 crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
 **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
 //crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
 your connection requests to a **randomly rotating IP address** in a pool of
 proxies before reaching the target website. The combination of AI and ML make
-it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
-at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
-xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
-proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+it more effective to avoid CAPTCHAs and blocks. The argument at the [Secure
+Sockets Layer (SSL)](https://en.wikipedia.org/wiki/Transport_Layer_Security)
+level may need to be added to the header. Use it in conjunction with
+`verify=False`. ```python # Get your proxy url at crawlbase https://
+crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://xxxxx:
+@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
+proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30,
+verify=False) client.session.header["crawlbaseAPI-Parameters"] = "country=US"
 client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's
 scenery.") ``` ### Reusable session object For standard cases, use Gemini
 class; for exceptions, use session objects. When creating a new bot Gemini
 server, adjust Headers.MAIN. ```python import requests from gemini import
 Gemini, Headers cookies = {} session = requests.Session() session.headers =
 Headers.MAIN for key, value in cookies.items(): session.cookies.update({key:
 value}) client = Gemini(session=session) # You can use various args response =
@@ -396,18 +393,20 @@
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
 huggingface.co/jondurbin/cinematika-7b-v0.1) - `undi95/toppy-m-7b:free` -
 [Undi95/Toppy-M-7B](https://huggingface.co/Undi95/Toppy-M-7B?not-for-all-
 audiences=true) - `gryphe/mythomist-7b:free` - [Gryphe/MythoMist-7b](https://
 huggingface.co/Gryphe/MythoMist-7b) - `nousresearch/nous-capybara-7b:free` -
 [NousResearch/Nous-Capybara-7B-V1](https://huggingface.co/NousResearch/Nous-
 Capybara-7B-V1) from Nous Research
-## Sponsor, [Crawlbase](https://crawlbase.com/) Use [Crawlbase](https://
-crawlbase.com/) API for efficient data scraping to train AI models, boasting a
-98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant,
-supports massive data extraction, and is trusted by 70k+ developers.
+## Sponsor
+[assets/crawlbase.png]
+Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to
+train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to
+start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by
+70k+ developers.
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) First review [HanaokaYuzu/Gemini-API](https://github.com/
 HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://
 aistudio.google.com/) before using this package. You can find most help on the
 [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues)
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
```

### Comparing `python_gemini_api-2.4.7/README.md` & `python_gemini_api-2.4.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: python-gemini-api
+Version: 2.4.8
+Summary: The python package that returns Response of Google Gemini through API.
+Home-page: https://github.com/dsdanielpark/Gemini-API
+Author: Daniel Park
+Author-email: parkminwoo1991@gmail.com
+Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx[http2]>=0.20.0
+Requires-Dist: requests
+Requires-Dist: browser_cookie3
+Requires-Dist: loguru
+Requires-Dist: pydantic
+Requires-Dist: aiohttp
+Provides-Extra: voice
+Requires-Dist: gTTS; extra == "voice"
+Requires-Dist: SpeechRecognition; extra == "voice"
+Requires-Dist: openai; extra == "voice"
+Requires-Dist: anthropic; extra == "voice"
+
 
 # <img src="https://www.gstatic.com/lamda/images/favicon_v1_150160cddff7f294ce30.svg" width="35px" alt="Gemini Icon" /> Gemini API  <a href="https://pypi.org/project/python-gemini-api/"> <img alt="PyPI" src="https://img.shields.io/pypi/v/python-gemini-api?color=black"></a>
 
 
 <p align="right">
     <a href="https://github.com/dsdanielpark/Gemini-API"><img alt="pip download" src="https://img.shields.io/badge/pip_install-python_gemini_api-black"></a> 
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
@@ -146,26 +179,26 @@
 
 ## Quick Start
 
 **Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
-cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"<key>" : "<value>"} # Cookies may vary by account or region. Consider sending the entire cookie file.
 client = Gemini(cookies=cookies) # You can use various args
 
 response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
 **Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
-cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"<key>" : "<value>"}
 client = Gemini(cookies=cookies) # You can use various args
 
 response = client.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
@@ -221,14 +254,19 @@
 <br>
 
 ### # 02. Generate content
 Returns Gemini's response, but the first one might be empty. 
 
 
 ```python
+from gemini import Gemini
+
+cookies = {}
+client = Gemini(cookies=cookies)
+
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = client.generate_content(prompt)
 print(response.payload)
 ```
 
 
 > [!IMPORTANT]
@@ -252,107 +290,136 @@
 
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-client = Gemini(cookies=cookies) # You can use various args
+cookies = {} 
+client = Gemini(cookies=cookies) 
 
 response_text, response_status = client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
 You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
+from gemini import Gemini
+
+cookies = {}
+client = Gemini(cookies=cookies)
+
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = client.generate_content(prompt)
 print(response.text)
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
 
 *Async downloader*
 
 ```python
+from gemini import Gemini, GeminiImage
+
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 generated_images = response.generated_images # Check generated images [Dict]
 
-await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
+await image_client.save(generated_images, "save_dir", cookies=cookies)
+# image_data_dict = await image_client.fetch_images_dict(generated_images, cookies=cookies)
+# await image_client.save_images(image_data_dict, "save_dir")
 ```
 
 
 <details><summary>Further</summary>
 
 *Display images in IPython*
   You can display the image or transmit it to another application in byte format.
   
   ```python
-  bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
-  from IPython.display import display, Image
   import io
+  from gemini import Gemini, GeminiImage
+  from IPython.display import display, Image
+  
+  cookies = {}
+  client = Gemini(cookies=cookies)
+  image_client = GeminiImage(cookies=cookies)
+
+  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies) # Save default folder is `cached`
 
 # You can use byte type image dict for printing images as follow:
-# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
 ```
 
 *Async downloader wrapper*
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
+    await image_client.save(generated_imagse, save_path=save_path, cookies=cookies)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  
     asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
 ```
 
 `GeminiImage.save` method logic
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    image_data_dict = await GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
-    await GeminiImage.save_images(image_data_dict, save_path=save_path)  
+    image_data_dict = await image_client.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
+    await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  # Check response images [Dict]
     asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
 ```
@@ -366,64 +433,82 @@
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
 
 *Async downloader*
 ```python
+from gemini import Gemini, GeminiImage
+
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
-await GeminiImage.save(response_images, "save_dir")
-# image_data_dict = await GeminiImage.fetch_images_dict(response_images)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
+await image_client.save(response_images, "save_dir")
+# image_data_dict = await image_client.fetch_images_dict(response_images)
+# await image_client.save_images(image_data_dict, "save_dir")
 ```
 
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
 GeminiImage.save_sync(response_images, save_path="save_dir")
 
 # You can use byte type image dict as follow:
-# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+# bytes_images_dict = image_client.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
 ```
 
 *Async downloader wrapper*
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
-async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    await GeminiImage.save(response_images, save_path=save_path, cookies=cookies)
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
+async def save_response_web_imagse(response_images, save_path="save_dir"):
+    await image_client.save(response_images, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     response_images = response.web_images  
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
 ```
 
 `GeminiImage.save` method logic
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    image_data_dict = await GeminiImage.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
-    await GeminiImage.save_images(image_data_dict, save_path=save_path)  
+    image_data_dict = await image_client.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
+    await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     response_images = response.web_images  # Check response images [Dict]
     asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
 ```
 
@@ -434,14 +519,15 @@
 ### # 07. Generate content from images
 Takes an image as input and returns a response.
 
 ```python
 image = 'folder/image.jpg'
 # image = open('folder/image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported.
 
+# Image file path or Byte-formatted image array
 response = client.generate_content("What does the text in this image say?", image=image)
 response.response_dict
 ```
 
 <br>
 
 ### # 08. Generate content using Google Services
@@ -537,25 +623,28 @@
 https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
 ### Use rotating proxies via [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api)
 
-If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
+If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks. The argument at the [Secure Sockets Layer (SSL)](https://en.wikipedia.org/wiki/Transport_Layer_Security) level may need to be added to the header. Use it in conjunction with `verify=False`.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
 
-client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client = Gemini(cookies=cookies, proxies=proxies, timeout=30, verify=False)
+client.session.header["crawlbaseAPI-Parameters"] = "country=US"
 client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
+
+
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
 import requests
 from gemini import Gemini, Headers
 
 cookies = {} 
@@ -660,17 +749,28 @@
 
 
 
 
 
 <br>
 
-## Sponsor, [Crawlbase](https://crawlbase.com/)
+## Sponsor
+
+<p align="left">
+  <img src="assets/crawlbase.png" width="240">
+</p>
+
 Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
 
+
+
+
+
+
+
 <br>
 
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md)
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
```

#### html2text {}

```diff
@@ -1,8 +1,25 @@
-# [Gemini Icon]Gemini API_[_P_y_P_I_]
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.8 Summary: The
+python package that returns Response of Google Gemini through API. Home-page:
+https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
+parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
+Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
+2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
+Natural Language :: English Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: httpx[http2]>=0.20.0 Requires-
+Dist: requests Requires-Dist: browser_cookie3 Requires-Dist: loguru Requires-
+Dist: pydantic Requires-Dist: aiohttp Provides-Extra: voice Requires-Dist:
+gTTS; extra == "voice" Requires-Dist: SpeechRecognition; extra == "voice"
+Requires-Dist: openai; extra == "voice" Requires-Dist: anthropic; extra ==
+"voice" # [Gemini Icon]Gemini API_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
 ba79-d9f89b637324 An **unofficial* Python wrapper, [python-gemini-api](https://
 pypi.org/project/python-gemini-api/), is available for users facing frequent
@@ -109,26 +126,24 @@
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
 reference. > [!IMPORTANT] > Experiment with different Google accounts and
 browser settings to find a working cookie. Success may vary by IP and account
 status. Once connected, a cookie typically remains effective over a month. Keep
 testing until successful.
 ## Quick Start **Generate content:** returns parsed response. ```python from
-gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
-or region. Consider sending the entire cookie file. client = Gemini
+gemini import Gemini cookies = {"" : ""} # Cookies may vary by account or
+region. Consider sending the entire cookie file. client = Gemini
 (cookies=cookies) # You can use various args response = client.generate_content
 ("Hello, Gemini. What's the weather like in Seoul today?") response.payload ```
 **Generate content from image:** you can use image as input. ```python from
-gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
-or region. Consider sending the entire cookie file. client = Gemini
-(cookies=cookies) # You can use various args response = client.generate_content
-("What does the text in this image say?", image='folder/image.jpg')
-response.payload ``` > [!NOTE] > If the generate_content method returns an
-empty payload, try executing it again without reinitializing the Gemini object.
-
+gemini import Gemini cookies = {"" : ""} client = Gemini(cookies=cookies) # You
+can use various args response = client.generate_content("What does the text in
+this image say?", image='folder/image.jpg') response.payload ``` > [!NOTE] > If
+the generate_content method returns an empty payload, try executing it again
+without reinitializing the Gemini object.
 
 ## Usage *Setting language and Gemini version using environment variables:
 * Setting Gemini response language (Optional): Check supported languages [here]
 (https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
 Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
 Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
 Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
@@ -144,111 +159,123 @@
 (cookies=cookies) # client = Gemini(cookie_fp="folder/cookie_file.json") #
 (*.json, *.txt) are supported. # client = Gemini(auto_cookies=True) # Or use
 auto_cookies paprameter ``` ##### Auto Cookie Update For `auto_cookie` to be
 set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the
 browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3)
 enables automatic cookie collection, though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
-be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
+be empty. ```python from gemini import Gemini cookies = {} client = Gemini
+(cookies=cookies) prompt = "Hello, Gemini. What's the weather like in Seoul
 today?" response = client.generate_content(prompt) print(response.payload) ```
 > [!IMPORTANT] > DO NOT send same prompt repeatly. **If the session connects
 successfully and `generate_content` runs well, CLOSE Gemini website.** If
 Gemini web stays open in the browser, cookies may expire faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
 following structure: - *rcid*: returns the response candidate id of the chosen
 candidate. - *text*: returns the text of the chosen candidate. - *code*:
 returns the codes of the chosen candidate. - *web_images*: returns a list of
 web images from the chosen candidate. - *generated_images*: returns a list of
 generated images from the chosen candidate. - *payload*: returns the response
 dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
 fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
-cookies = {} # Cookies may vary by account or region. Consider sending the
-entire cookie file. client = Gemini(cookies=cookies) # You can use various args
-response_text, response_status = client.send_request("Hello, Gemini. What's the
-weather like in Seoul today?") print(response_text) ``` You can track the total
-number of requests made by accessing the `request_count` property within the
-`Gemini` class.
-### # 04. Text generation Returns text generated by Gemini. ```python prompt =
+cookies = {} client = Gemini(cookies=cookies) response_text, response_status =
+client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
+print(response_text) ``` You can track the total number of requests made by
+accessing the `request_count` property within the `Gemini` class.
+### # 04. Text generation Returns text generated by Gemini. ```python from
+gemini import Gemini cookies = {} client = Gemini(cookies=cookies) prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
-downloader* ```python response = client.generate_content("Create illustrations
-of Seoul, South Korea.") generated_images = response.generated_images # Check
-generated images [Dict] await GeminiImage.save(generated_images, "save_dir",
-cookies=cookies) # image_data_dict = await GeminiImage.fetch_images_dict
-(generated_images, cookies=cookies) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Further *Display images in IPython* You can
-display the image or transmit it to another application in byte format.
-```python bytes_images_dict = GeminiImage.fetch_images_dict_sync
-(generated_images, cookies) # Get bytes images dict from IPython.display import
-display, Image import io for image_name, image_bytes in bytes_images_dict.items
-(): print(image_name) image = Image(data=image_bytes) display(image) ``` *Sync
-downloader* ```python from gemini import Gemini, GeminiImage response =
-client.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# You can use byte type image dict for printing images as follow: #
-bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
-cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ``` *Async
-downloader wrapper* ```python import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): await GeminiImage.save
-(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
-function if __name__ == "__main__": cookies = {"key" : "value"}
-generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
-(generated_imagse, save_path="save_dir", cookies=cookies)) ```
-`GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): image_data_dict = await
-GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
-images dict asynchronously await GeminiImage.save_images(image_data_dict,
-save_path=save_path) # Run the async function if __name__ == "__main__":
-cookies = {"key" : "value"} generated_imagse = response.generated_imagse #
-Check response images [Dict] asyncio.run(save_generated_imagse
-(generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
-GeminiImage for image processing. `web_images` works without cookies, but for
-images like `generated_image` from Gemini, pass cookies. Cookies are needed to
-download images from Google's storage. Check the response or use existing
-cookies variable.
+downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+response = client.generate_content("Create illustrations of Seoul, South
+Korea.") generated_images = response.generated_images # Check generated images
+[Dict] await image_client.save(generated_images, "save_dir", cookies=cookies) #
+image_data_dict = await image_client.fetch_images_dict(generated_images,
+cookies=cookies) # await image_client.save_images(image_data_dict, "save_dir")
+``` Further *Display images in IPython* You can display the image or transmit
+it to another application in byte format. ```python import io from gemini
+import Gemini, GeminiImage from IPython.display import display, Image cookies =
+{} client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+bytes_images_dict = image_client.fetch_images_dict_sync(generated_images,
+cookies) # Get bytes images dict for image_name, image_bytes in
+bytes_images_dict.items(): print(image_name) image = Image(data=image_bytes)
+display(image) ``` *Sync downloader* ```python from gemini import Gemini,
+GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client =
+GeminiImage(cookies=cookies) response = client.generate_content("Create
+illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict]
+image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+# Save default folder is `cached` # You can use byte type image dict for
+printing images as follow: # bytes_images_dict =
+image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
+bytes images dict # image_client.save_images_sync(bytes_images_dict,
+path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
+```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies): await image_client.save(generated_imagse,
+save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+"__main__": cookies = {"key" : "value"} generated_imagse =
+response.generated_imagse asyncio.run(save_generated_imagse(generated_imagse,
+save_path="save_dir", cookies=cookies)) ``` `GeminiImage.save` method logic
+```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies): image_data_dict = await image_client.fetch_images_dict
+(generated_imagse, cookies=cookies) # Get bytes images dict asynchronously
+await image_client.save_images(image_data_dict, save_path=save_path) # Run the
+async function if __name__ == "__main__": cookies = {"key" : "value"}
+generated_imagse = response.generated_imagse # Check response images [Dict]
+asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies)) ``` > [!NOTE] > Use GeminiImage for image processing.
+`web_images` works without cookies, but for images like `generated_image` from
+Gemini, pass cookies. Cookies are needed to download images from Google's
+storage. Check the response or use existing cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Async downloader* ```python response = client.generate_content("Create
-illustrations of Seoul, South Korea.") response_images = response.web_images #
-Check generated images [Dict] await GeminiImage.save(response_images,
-"save_dir") # image_data_dict = await GeminiImage.fetch_images_dict
-(response_images) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Further *Sync downloader* ```python from gemini import Gemini, GeminiImage
+Gemini. *Async downloader* ```python from gemini import Gemini, GeminiImage
+cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
+(cookies=cookies) response = client.generate_content("Create illustrations of
+Seoul, South Korea.") response_images = response.web_images # Check generated
+images [Dict] await image_client.save(response_images, "save_dir") #
+image_data_dict = await image_client.fetch_images_dict(response_images) # await
+image_client.save_images(image_data_dict, "save_dir") ``` Further *Sync
+downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Please recommend a travel itinerary for
 Seoul.") response_images = response.web_images # Check response images [Dict]
 GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
-type image dict as follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync
+type image dict as follow: # bytes_images_dict = image_client.fetch_bytes_sync
 (response_images, cookies) # Get bytes images dict #
-GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
-``` *Async downloader wrapper* ```python import asyncio from gemini import
-Gemini, GeminiImage async def save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies): await GeminiImage.save(response_images,
-save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to
+path ``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_response_web_imagse
+(response_images, save_path="save_dir"): await image_client.save
+(response_images, save_path=save_path) # Run the async function if __name__ ==
 "__main__": cookies = {"key" : "value"} response_images = response.web_images
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
-gemini import Gemini, GeminiImage async def save_response_web_imagse
+asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
+``` `GeminiImage.save` method logic ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_response_web_imagse
 (response_images, save_path="save_dir", cookies=cookies): image_data_dict =
-await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
-bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
-save_path=save_path) # Run the async function if __name__ == "__main__":
-response_images = response.web_images # Check response images [Dict]
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies)) ```
+await image_client.fetch_images_dict(response_images, cookies=cookies) # Get
+bytes images dict asynchronously await image_client.save_images
+(image_data_dict, save_path=save_path) # Run the async function if __name__ ==
+"__main__": response_images = response.web_images # Check response images
+[Dict] asyncio.run(save_response_web_imagse(response_images,
+save_path="save_dir", cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
-image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
-client.generate_content("What does the text in this image say?", image=image)
-response.response_dict ```
+image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. # Image file
+path or Byte-formatted image array response = client.generate_content("What
+does the text in this image say?", image=image) response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
 gemini.google.com/extensions). Please refer to the [official notice](https://
 support.google.com/gemini/answer/13695044) and review the [privacy policies]
 (https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-
 1578971242&p=privacy_help&rd=1) for more details. *extention flags* ``` @Gmail,
 @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels,
@@ -302,18 +329,22 @@
 crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
 **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
 //crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
 your connection requests to a **randomly rotating IP address** in a pool of
 proxies before reaching the target website. The combination of AI and ML make
-it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
-at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
-xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
-proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+it more effective to avoid CAPTCHAs and blocks. The argument at the [Secure
+Sockets Layer (SSL)](https://en.wikipedia.org/wiki/Transport_Layer_Security)
+level may need to be added to the header. Use it in conjunction with
+`verify=False`. ```python # Get your proxy url at crawlbase https://
+crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://xxxxx:
+@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
+proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30,
+verify=False) client.session.header["crawlbaseAPI-Parameters"] = "country=US"
 client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's
 scenery.") ``` ### Reusable session object For standard cases, use Gemini
 class; for exceptions, use session objects. When creating a new bot Gemini
 server, adjust Headers.MAIN. ```python import requests from gemini import
 Gemini, Headers cookies = {} session = requests.Session() session.headers =
 Headers.MAIN for key, value in cookies.items(): session.cookies.update({key:
 value}) client = Gemini(session=session) # You can use various args response =
@@ -379,18 +410,20 @@
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
 huggingface.co/jondurbin/cinematika-7b-v0.1) - `undi95/toppy-m-7b:free` -
 [Undi95/Toppy-M-7B](https://huggingface.co/Undi95/Toppy-M-7B?not-for-all-
 audiences=true) - `gryphe/mythomist-7b:free` - [Gryphe/MythoMist-7b](https://
 huggingface.co/Gryphe/MythoMist-7b) - `nousresearch/nous-capybara-7b:free` -
 [NousResearch/Nous-Capybara-7B-V1](https://huggingface.co/NousResearch/Nous-
 Capybara-7B-V1) from Nous Research
-## Sponsor, [Crawlbase](https://crawlbase.com/) Use [Crawlbase](https://
-crawlbase.com/) API for efficient data scraping to train AI models, boasting a
-98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant,
-supports massive data extraction, and is trusted by 70k+ developers.
+## Sponsor
+[assets/crawlbase.png]
+Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to
+train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to
+start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by
+70k+ developers.
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) First review [HanaokaYuzu/Gemini-API](https://github.com/
 HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://
 aistudio.google.com/) before using this package. You can find most help on the
 [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues)
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
```

### Comparing `python_gemini_api-2.4.7/gemini/__init__.py` & `python_gemini_api-2.4.8/gemini/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     from .src.modules.voice.google import google_tts, google_stt
     from .src.modules.voice.openai import openai_tts, openai_stt
 except ImportError as e:
     pass
 
 gemini_api_key = environ.get("GEMINI_COOKIES")
 
-__version__ = "2.4.7"
+__version__ = "2.4.8"
 __author__ = (
     "daniel park <parkminwoo1991@gmail.com>, antonio cheang <teapotv8@proton.me>, "
     "HanaokaYuzu, CBoYXD, veonua, thewh1teagle, jjkoh95, yihong0618, nishantchauhan949, MeemeeLab, kota113, "
     "sachnun, amit9021, zeelsheladiya, ayansengupta17, thecodekitchen, SalimLouDev, Qewertyy, "
     "senseibence, mirusu400, szv99, sudoAlireza"
 )
```

### Comparing `python_gemini_api-2.4.7/gemini/async_client.py` & `python_gemini_api-2.4.8/gemini/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # To-Do: Current logic contains traces of development attempts, so need to add asynchronous processing based on core.py and document it.
 import os
 import re
 import json
-import time
 import httpx
 import random
 import string
 import urllib
 import asyncio
 import requests
-from typing import Optional, Any, List
+from typing import Optional
 
 from gemini.src.misc.constants import (
     URLs,
     Headers,
     SUPPORTED_BROWSERS,
 )
```

### Comparing `python_gemini_api-2.4.7/gemini/client.py` & `python_gemini_api-2.4.8/gemini/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,56 +9,69 @@
 from requests.exceptions import ConnectionError
 from typing import Optional, Tuple, Dict, Union, List
 
 from .src.misc.utils import upload_image, load_cookies
 from .src.model.parser.response_parser import ResponseParser
 from .src.model.output import GeminiCandidate, GeminiModelOutput
 from .src.model.parser.custom_parser import ParseMethod1, ParseMethod2
-from .src.misc.exceptions import GeminiAPIError
+from .src.misc.exceptions import (
+    GeminiAPIError,
+    PackageError,
+    TimeoutError,
+    RateLimitException,
+    ContentGenerationException,
+)
 
 from .src.misc.constants import (
     URLs,
     Headers,
     TARGET_COOKIES,
     WHOLE_COOKIES,
     SUPPORTED_BROWSERS,
 )
 
 
 class Gemini:
     """
-    A class to manage interactions with a web service, handling sessions, cookies, and proxies.
+    This class facilitates interactions with a web service by managing sessions, cookies, and proxy configurations.
 
     Attributes:
-        auto_cookies (bool): Whether to automatically manage cookies.
-        cookies (Dict[str, str]): A dictionary of cookies.
-        proxies (dict): A dictionary of proxy settings.
-        timeout (int): The timeout for requests.
-        session (requests.Session): The session for making requests.
-        base_url (str): The base URL for the web service.
+        auto_cookies (bool): If set to True, cookies are managed automatically.
+        cookies (dict[str, str]): Stores the cookies used in HTTP requests.
+        proxies (dict[str, str]): Proxy settings for the HTTP requests.
+        timeout (int): Timeout in seconds for HTTP requests.
+        session (requests.Session): The session used for HTTP requests.
+        base_url (str): The base URL of the web service.
+        target_cookies (list): Specific cookies targeted for operations if auto_cookies is enabled.
+        verify (bool): If True, the SSL certificate is verified. Defaults to True.
 
     Parameters:
-        session (Optional[requests.Session]): An existing requests session, if any.
-        cookies (Optional[Dict[str, str]]): Initial cookies to use, if any.
-        cookie_fp (str): File path to load cookies from, if `auto_cookies` is True.
-        auto_cookies (bool): Automatically manage cookies if True.
-        timeout (int): Timeout for requests, defaults to 30 seconds.
-        proxies (Optional[dict]): Proxy configuration for requests, if any.
-        rcid (str): Response candidate ID.
+        session (Optional[requests.Session]): An existing session, if any.
+        cookies (Optional[dict[str, str]]): Initial cookies, if any.
+        cookie_fp (str): File path to load cookies from if `auto_cookies` is set.
+        auto_cookies (bool): Enables automatic cookie management when True.
+        target_cookies (list): List of cookie names to manage if `auto_cookies` is set.
+        timeout (int): Request timeout; defaults to 30 seconds.
+        proxies (Optional[dict[str, str]]): Proxy settings, if any.
+
+    Raises:
+        ConnectionError: If there is a problem with the network connection.
+        TimeoutError: If the request times out.
     """
 
     def __init__(
         self,
         session: Optional[requests.Session] = None,
         cookies: Optional[Dict[str, str]] = None,
         cookie_fp: str = None,
         auto_cookies: bool = False,
         target_cookies: List = None,
         timeout: int = 30,
         proxies: Optional[dict] = None,
+        verify: bool = True,
     ) -> None:
         """
         Initializes the Gemini object with session, cookies, and other configurations.
         """
         self._request_count = 0
         self._nonce = None  # SNlM0e nonce value
         self._sid = None  # session id
@@ -71,14 +84,15 @@
         self.cookie_fp = cookie_fp
         self.cookies = cookies
         self.proxies = proxies or {}
         self.timeout = timeout
         self.session = session or self._initialize_session()
         self.base_url: str = URLs.BASE_URL.value
         self.parser = ResponseParser(cookies=self.cookies)
+        self.verify = True  # Default is True
 
     @property
     def request_count(self) -> int:
         return self._request_count
 
     @property
     def nonce(self) -> Optional[str]:
@@ -97,19 +111,15 @@
     def rcid(self, value: Optional[str]) -> None:
         self._rcid = value
 
     def _initialize_session(
         self,
     ) -> requests.Session:
         """
-        Initializes a new session with headers, cookies, and optionally loads cookies from a file.
-
-        Parameters:
-            cookies (Optional[Dict[str, str]]): Cookies to add to the session.
-            cookie_fp (Optional[str]): Path to a file from which to load cookies.
+        Initializes a sync session.
 
         Returns:
             requests.Session: The initialized session.
         """
         session = requests.Session()
         session.headers.update(Headers.MAIN)
         if self.cookies:
@@ -136,15 +146,15 @@
         """
         Retrieves the session ID (SID) and a SNlM0e nonce value from the application page.
         """
         try:
             response = requests.get(f"{URLs.BASE_URL.value}/app", cookies=self.cookies)
             if response.status_code != 200:
                 raise GeminiAPIError(
-                    f"Gemini API Error: Response code {response.status_code}\nExcessive connections may have temporarily blocked your account/IP, but web UI should remain accessible."
+                    f"Gemini API Error: Response code {response.status_code}\nDetails:\n{response}\n\nExcessive connections may have temporarily blocked your account/IP, but web UI should remain accessible."
                 )
 
             response.raise_for_status()
 
             sid_match = re.search(r'"FdrFJe":"([\d-]+)"', response.text)
             nonce_match = re.search(r'"SNlM0e":"(.*?)"', response.text)
 
@@ -236,14 +246,15 @@
         data = self._construct_payload(prompt, image, self._nonce)
         response = self.session.post(
             URLs.POST_ENDPOINT.value,
             params=params,
             data=data,
             timeout=self.timeout,
             proxies=self.proxies,
+            verify=self.verify,
         )
         self._reqid += 100000
         response.raise_for_status()
 
         return response.text, response.status_code
 
     def generate_content(
@@ -287,15 +298,15 @@
         return GeminiModelOutput(
             metadata=metadata,
             candidates=candidates,
             response_dict=parsed_response,
         )
 
     @staticmethod
-    def collect_candidates(data):
+    def collect_candidates(data: dict) -> list:
         """
         Collects candidate data from parsed response.
 
         Args:
             data: The parsed response data.
 
         Returns:
```

### Comparing `python_gemini_api-2.4.7/gemini/src/extensions/replit.py` & `python_gemini_api-2.4.8/gemini/src/extensions/replit.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/misc/constants.py` & `python_gemini_api-2.4.8/gemini/src/misc/constants.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/misc/decorator.py` & `python_gemini_api-2.4.8/gemini/src/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/misc/exceptions.py` & `python_gemini_api-2.4.8/gemini/src/misc/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/misc/utils.py` & `python_gemini_api-2.4.8/gemini/src/misc/utils.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/model/image.py` & `python_gemini_api-2.4.8/gemini/src/model/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,93 @@
+# Will be refactored.
 import os
-import random
 import httpx
+import random
 import asyncio
 import datetime
 from pathlib import Path
 from loguru import logger
-from typing import List, Optional, Dict
 from pydantic import BaseModel, HttpUrl
+from typing import List, Optional, Dict
 
 
 class GeminiImage(BaseModel):
     """
     Represents an image with URL, title, and alt text.
 
     Attributes:
         url (HttpUrl): The URL of the image.
         title (str): The title of the image. Defaults to "[Image]".
         alt (str): The alt text of the image. Defaults to "".
+        cookies (Optional[Dict[str, str]]): Optional cookies to be used for fetching the image.
+            This parameter is required if you want to fetch generated images.
 
     Methods:
-        validate_images(cls, images): Validates the input images list.
-        save(cls, images: List["GeminiImage"], save_path: str = "cached", cookies: Optional[dict] = None) -> Optional[Path]:
+        validate_images(images: List["GeminiImage"]) -> bool:
+            Validates the input images list.
+        save(images: List["GeminiImage"], save_path: str = "cached", cookies: Optional[dict] = None) -> Optional[Path]:
             Downloads and saves images asynchronously.
         fetch_bytes(url: HttpUrl, cookies: Optional[dict] = None) -> Optional[bytes]:
             Fetches bytes of an image asynchronously.
-        fetch_images_dict(cls, images: List["GeminiImage"], cookies: Optional[dict] = None) -> Dict[str, bytes]:
+        fetch_images_dict(images: List["GeminiImage"], cookies: Optional[dict] = None) -> Dict[str, bytes]:
             Fetches images asynchronously and returns a dictionary of image data.
-        save_images(cls, image_data: Dict[str, bytes], save_path: str = "cached"):
+        save_images(image_data: Dict[str, bytes], save_path: str = "cached"):
             Saves images locally.
     """
 
     url: HttpUrl
     title: str = "[Image]"
     alt: str = ""
+    cookies: Optional[Dict[str, str]] = None
+
+    def __init__(self, cookies: Optional[Dict[str, str]] = None):
+        """
+        Initialize GeminiImage with optional cookies.
 
-    @classmethod
-    def validate_images(cls, images):
+        Args:
+            cookies (Optional[Dict[str, str]]): Optional cookies to be used for fetching the image.
+                *This parameter is required if you want to fetch `generated images`.
+        """
+        self.cookies = cookies
+
+    def validate_images(self, images):
         """
         Validates the input images list.
 
         Args:
             images: The list of GeminiImage objects.
 
         Raises:
             ValueError: If the input images list is empty.
         """
         if not images:
             raise ValueError(
-                "Input is empty. Please provide images infomation to proceed."
+                "Input is empty. Please provide GeminiOutput formatted images list to proceed."
             )
 
     # Async downloader
-    @classmethod
     async def save(
-        cls,
+        self,
         images: List["GeminiImage"],
         save_path: str = "cached",
-        cookies: Optional[dict] = None,
     ) -> Optional[Path]:
         """
         Downloads and saves images asynchronously.
 
         Args:
             images (List["GeminiImage"]): The list of GeminiImage objects to download.
             save_path (str): The directory path to save the images. Defaults to "cached".
             cookies (Optional[dict]): Cookies to be used for downloading images. Defaults to None.
 
         Returns:
             Optional[Path]: The path to the directory where the images are saved, or None if saving fails.
         """
-        cls.validate_images(images)
-        image_data = await cls.fetch_images_dict(images, cookies)
-        await cls.save_images(image_data, save_path)
+        self.validate_images(images)
+        image_data = await self.fetch_images_dict(images, self.cookies)
+        await self.save_images(image_data, save_path)
 
     @staticmethod
     async def fetch_bytes(
         url: HttpUrl, cookies: Optional[dict] = None
     ) -> Optional[bytes]:
         """
         Fetches bytes of an image asynchronously.
@@ -92,30 +104,29 @@
                 response = await client.get(str(url), cookies=cookies)
                 response.raise_for_status()
                 return response.content
         except Exception as e:
             print(f"Failed to download {url}: {str(e)}")
             return None
 
-    @classmethod
     async def fetch_images_dict(
-        cls, images: List["GeminiImage"], cookies: Optional[dict] = None
+        self, images: List["GeminiImage"], cookies: Optional[dict] = None
     ) -> Dict[str, bytes]:
         """
         Fetches images asynchronously and returns a dictionary of image data.
 
         Args:
             images (List["GeminiImage"]): The list of GeminiImage objects to fetch.
             cookies (Optional[dict]): Cookies to be used for fetching the images. Defaults to None.
 
         Returns:
             Dict[str, bytes]: A dictionary containing image titles as keys and image bytes as values.
         """
-        cls.validate_images(images)
-        tasks = [cls.fetch_bytes(image.url, cookies=cookies) for image in images]
+        self.validate_images(images)
+        tasks = [self.fetch_bytes(image.url, cookies=cookies) for image in images]
         results = await asyncio.gather(*tasks)
         return {image.title: result for image, result in zip(images, results) if result}
 
     @staticmethod
     async def save_images(image_data: Dict[str, bytes], save_path: str = "cached"):
         """
         Saves images locally.
@@ -133,32 +144,31 @@
                 with open(filepath, "wb") as f:
                     f.write(data)
                 print(f"Saved {title} to {filepath}")
             except Exception as e:
                 print(f"Error saving {title}: {str(e)}")
 
     # Sync downloader
-    @staticmethod
     def save_sync(
+        self,
         images: List["GeminiImage"],
-        cookies: Optional[dict] = None,
         save_path: str = "cached",
     ) -> Optional[Path]:
         """Synchronously saves the image to the specified path.
 
         Args:
             path (str): The directory where the image will be saved.
             filename (str, optional): The filename for the saved image. If not provided,
                 a filename is generated based on the image title.
             cookies (dict, optional): Cookies to be used for downloading the image.
 
         Returns:
             Optional[Path]: The path where the image is saved, or None if saving fails.
         """
-        image_data = GeminiImage.fetch_images_dict_sync(images, cookies)
+        image_data = GeminiImage.fetch_images_dict_sync(images, self.cookies)
         GeminiImage.validate_images(image_data)
         GeminiImage.save_images_sync(image_data, save_path)
 
     @staticmethod
     def fetch_bytes_sync(
         url: HttpUrl, cookies: Optional[dict] = None
     ) -> Optional[bytes]:
```

### Comparing `python_gemini_api-2.4.7/gemini/src/model/output.py` & `python_gemini_api-2.4.8/gemini/src/model/output.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/model/parser/base.py` & `python_gemini_api-2.4.8/gemini/src/model/parser/base.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/model/parser/custom_parser.py` & `python_gemini_api-2.4.8/gemini/src/model/parser/custom_parser.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/model/parser/response_parser.py` & `python_gemini_api-2.4.8/gemini/src/model/parser/response_parser.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/modules/openrouter/async_client.py` & `python_gemini_api-2.4.8/gemini/src/modules/openrouter/async_client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/modules/openrouter/client.py` & `python_gemini_api-2.4.8/gemini/src/modules/openrouter/client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/modules/voice/google.py` & `python_gemini_api-2.4.8/gemini/src/modules/voice/google.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/gemini/src/modules/voice/openai.py` & `python_gemini_api-2.4.8/gemini/src/modules/voice/openai.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/python_gemini_api.egg-info/PKG-INFO` & `python_gemini_api-2.4.8/python_gemini_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gemini-api
-Version: 2.4.7
+Version: 2.4.8
 Summary: The python package that returns Response of Google Gemini through API.
 Home-page: https://github.com/dsdanielpark/Gemini-API
 Author: Daniel Park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -179,26 +179,26 @@
 
 ## Quick Start
 
 **Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
-cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"<key>" : "<value>"} # Cookies may vary by account or region. Consider sending the entire cookie file.
 client = Gemini(cookies=cookies) # You can use various args
 
 response = client.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
 **Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
-cookies = {"key" : "value"} # Cookies may vary by account or region. Consider sending the entire cookie file.
+cookies = {"<key>" : "<value>"}
 client = Gemini(cookies=cookies) # You can use various args
 
 response = client.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
@@ -254,14 +254,19 @@
 <br>
 
 ### # 02. Generate content
 Returns Gemini's response, but the first one might be empty. 
 
 
 ```python
+from gemini import Gemini
+
+cookies = {}
+client = Gemini(cookies=cookies)
+
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = client.generate_content(prompt)
 print(response.payload)
 ```
 
 
 > [!IMPORTANT]
@@ -285,107 +290,136 @@
 
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
 from gemini import Gemini
 
-cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
-client = Gemini(cookies=cookies) # You can use various args
+cookies = {} 
+client = Gemini(cookies=cookies) 
 
 response_text, response_status = client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
 You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
+from gemini import Gemini
+
+cookies = {}
+client = Gemini(cookies=cookies)
+
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = client.generate_content(prompt)
 print(response.text)
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
 
 *Async downloader*
 
 ```python
+from gemini import Gemini, GeminiImage
+
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 generated_images = response.generated_images # Check generated images [Dict]
 
-await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
+await image_client.save(generated_images, "save_dir", cookies=cookies)
+# image_data_dict = await image_client.fetch_images_dict(generated_images, cookies=cookies)
+# await image_client.save_images(image_data_dict, "save_dir")
 ```
 
 
 <details><summary>Further</summary>
 
 *Display images in IPython*
   You can display the image or transmit it to another application in byte format.
   
   ```python
-  bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
-  from IPython.display import display, Image
   import io
+  from gemini import Gemini, GeminiImage
+  from IPython.display import display, Image
+  
+  cookies = {}
+  client = Gemini(cookies=cookies)
+  image_client = GeminiImage(cookies=cookies)
+
+  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies) # Save default folder is `cached`
 
 # You can use byte type image dict for printing images as follow:
-# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
 ```
 
 *Async downloader wrapper*
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
+    await image_client.save(generated_imagse, save_path=save_path, cookies=cookies)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  
     asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
 ```
 
 `GeminiImage.save` method logic
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    image_data_dict = await GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
-    await GeminiImage.save_images(image_data_dict, save_path=save_path)  
+    image_data_dict = await image_client.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
+    await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  # Check response images [Dict]
     asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
 ```
@@ -399,64 +433,82 @@
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
 
 *Async downloader*
 ```python
+from gemini import Gemini, GeminiImage
+
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
-await GeminiImage.save(response_images, "save_dir")
-# image_data_dict = await GeminiImage.fetch_images_dict(response_images)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
+await image_client.save(response_images, "save_dir")
+# image_data_dict = await image_client.fetch_images_dict(response_images)
+# await image_client.save_images(image_data_dict, "save_dir")
 ```
 
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
 GeminiImage.save_sync(response_images, save_path="save_dir")
 
 # You can use byte type image dict as follow:
-# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+# bytes_images_dict = image_client.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
 ```
 
 *Async downloader wrapper*
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
-async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    await GeminiImage.save(response_images, save_path=save_path, cookies=cookies)
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
+async def save_response_web_imagse(response_images, save_path="save_dir"):
+    await image_client.save(response_images, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     response_images = response.web_images  
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
 ```
 
 `GeminiImage.save` method logic
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
+cookies = {}
+client = Gemini(cookies=cookies)
+image_client = GeminiImage(cookies=cookies)
+
 async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    image_data_dict = await GeminiImage.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
-    await GeminiImage.save_images(image_data_dict, save_path=save_path)  
+    image_data_dict = await image_client.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
+    await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     response_images = response.web_images  # Check response images [Dict]
     asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
 ```
 
@@ -467,14 +519,15 @@
 ### # 07. Generate content from images
 Takes an image as input and returns a response.
 
 ```python
 image = 'folder/image.jpg'
 # image = open('folder/image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported.
 
+# Image file path or Byte-formatted image array
 response = client.generate_content("What does the text in this image say?", image=image)
 response.response_dict
 ```
 
 <br>
 
 ### # 08. Generate content using Google Services
@@ -570,25 +623,28 @@
 https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
 ### Use rotating proxies via [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api)
 
-If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
+If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks. The argument at the [Secure Sockets Layer (SSL)](https://en.wikipedia.org/wiki/Transport_Layer_Security) level may need to be added to the header. Use it in conjunction with `verify=False`.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
 
-client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+client = Gemini(cookies=cookies, proxies=proxies, timeout=30, verify=False)
+client.session.header["crawlbaseAPI-Parameters"] = "country=US"
 client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
+
+
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
 import requests
 from gemini import Gemini, Headers
 
 cookies = {} 
@@ -693,17 +749,28 @@
 
 
 
 
 
 <br>
 
-## Sponsor, [Crawlbase](https://crawlbase.com/)
+## Sponsor
+
+<p align="left">
+  <img src="assets/crawlbase.png" width="240">
+</p>
+
 Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
 
+
+
+
+
+
+
 <br>
 
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md)
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.7 Summary: The
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.8 Summary: The
 python package that returns Response of Google Gemini through API. Home-page:
 https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
 Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -126,26 +126,24 @@
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
 reference. > [!IMPORTANT] > Experiment with different Google accounts and
 browser settings to find a working cookie. Success may vary by IP and account
 status. Once connected, a cookie typically remains effective over a month. Keep
 testing until successful.
 ## Quick Start **Generate content:** returns parsed response. ```python from
-gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
-or region. Consider sending the entire cookie file. client = Gemini
+gemini import Gemini cookies = {"" : ""} # Cookies may vary by account or
+region. Consider sending the entire cookie file. client = Gemini
 (cookies=cookies) # You can use various args response = client.generate_content
 ("Hello, Gemini. What's the weather like in Seoul today?") response.payload ```
 **Generate content from image:** you can use image as input. ```python from
-gemini import Gemini cookies = {"key" : "value"} # Cookies may vary by account
-or region. Consider sending the entire cookie file. client = Gemini
-(cookies=cookies) # You can use various args response = client.generate_content
-("What does the text in this image say?", image='folder/image.jpg')
-response.payload ``` > [!NOTE] > If the generate_content method returns an
-empty payload, try executing it again without reinitializing the Gemini object.
-
+gemini import Gemini cookies = {"" : ""} client = Gemini(cookies=cookies) # You
+can use various args response = client.generate_content("What does the text in
+this image say?", image='folder/image.jpg') response.payload ``` > [!NOTE] > If
+the generate_content method returns an empty payload, try executing it again
+without reinitializing the Gemini object.
 
 ## Usage *Setting language and Gemini version using environment variables:
 * Setting Gemini response language (Optional): Check supported languages [here]
 (https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
 Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
 Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
 Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
@@ -161,111 +159,123 @@
 (cookies=cookies) # client = Gemini(cookie_fp="folder/cookie_file.json") #
 (*.json, *.txt) are supported. # client = Gemini(auto_cookies=True) # Or use
 auto_cookies paprameter ``` ##### Auto Cookie Update For `auto_cookie` to be
 set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the
 browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3)
 enables automatic cookie collection, though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
-be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
+be empty. ```python from gemini import Gemini cookies = {} client = Gemini
+(cookies=cookies) prompt = "Hello, Gemini. What's the weather like in Seoul
 today?" response = client.generate_content(prompt) print(response.payload) ```
 > [!IMPORTANT] > DO NOT send same prompt repeatly. **If the session connects
 successfully and `generate_content` runs well, CLOSE Gemini website.** If
 Gemini web stays open in the browser, cookies may expire faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
 following structure: - *rcid*: returns the response candidate id of the chosen
 candidate. - *text*: returns the text of the chosen candidate. - *code*:
 returns the codes of the chosen candidate. - *web_images*: returns a list of
 web images from the chosen candidate. - *generated_images*: returns a list of
 generated images from the chosen candidate. - *payload*: returns the response
 dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
 fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
-cookies = {} # Cookies may vary by account or region. Consider sending the
-entire cookie file. client = Gemini(cookies=cookies) # You can use various args
-response_text, response_status = client.send_request("Hello, Gemini. What's the
-weather like in Seoul today?") print(response_text) ``` You can track the total
-number of requests made by accessing the `request_count` property within the
-`Gemini` class.
-### # 04. Text generation Returns text generated by Gemini. ```python prompt =
+cookies = {} client = Gemini(cookies=cookies) response_text, response_status =
+client.send_request("Hello, Gemini. What's the weather like in Seoul today?")
+print(response_text) ``` You can track the total number of requests made by
+accessing the `request_count` property within the `Gemini` class.
+### # 04. Text generation Returns text generated by Gemini. ```python from
+gemini import Gemini cookies = {} client = Gemini(cookies=cookies) prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
-downloader* ```python response = client.generate_content("Create illustrations
-of Seoul, South Korea.") generated_images = response.generated_images # Check
-generated images [Dict] await GeminiImage.save(generated_images, "save_dir",
-cookies=cookies) # image_data_dict = await GeminiImage.fetch_images_dict
-(generated_images, cookies=cookies) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Further *Display images in IPython* You can
-display the image or transmit it to another application in byte format.
-```python bytes_images_dict = GeminiImage.fetch_images_dict_sync
-(generated_images, cookies) # Get bytes images dict from IPython.display import
-display, Image import io for image_name, image_bytes in bytes_images_dict.items
-(): print(image_name) image = Image(data=image_bytes) display(image) ``` *Sync
-downloader* ```python from gemini import Gemini, GeminiImage response =
-client.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# You can use byte type image dict for printing images as follow: #
-bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
-cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ``` *Async
-downloader wrapper* ```python import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): await GeminiImage.save
-(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
-function if __name__ == "__main__": cookies = {"key" : "value"}
-generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
-(generated_imagse, save_path="save_dir", cookies=cookies)) ```
-`GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): image_data_dict = await
-GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
-images dict asynchronously await GeminiImage.save_images(image_data_dict,
-save_path=save_path) # Run the async function if __name__ == "__main__":
-cookies = {"key" : "value"} generated_imagse = response.generated_imagse #
-Check response images [Dict] asyncio.run(save_generated_imagse
-(generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
-GeminiImage for image processing. `web_images` works without cookies, but for
-images like `generated_image` from Gemini, pass cookies. Cookies are needed to
-download images from Google's storage. Check the response or use existing
-cookies variable.
+downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+response = client.generate_content("Create illustrations of Seoul, South
+Korea.") generated_images = response.generated_images # Check generated images
+[Dict] await image_client.save(generated_images, "save_dir", cookies=cookies) #
+image_data_dict = await image_client.fetch_images_dict(generated_images,
+cookies=cookies) # await image_client.save_images(image_data_dict, "save_dir")
+``` Further *Display images in IPython* You can display the image or transmit
+it to another application in byte format. ```python import io from gemini
+import Gemini, GeminiImage from IPython.display import display, Image cookies =
+{} client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+bytes_images_dict = image_client.fetch_images_dict_sync(generated_images,
+cookies) # Get bytes images dict for image_name, image_bytes in
+bytes_images_dict.items(): print(image_name) image = Image(data=image_bytes)
+display(image) ``` *Sync downloader* ```python from gemini import Gemini,
+GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client =
+GeminiImage(cookies=cookies) response = client.generate_content("Create
+illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict]
+image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+# Save default folder is `cached` # You can use byte type image dict for
+printing images as follow: # bytes_images_dict =
+image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
+bytes images dict # image_client.save_images_sync(bytes_images_dict,
+path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
+```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies): await image_client.save(generated_imagse,
+save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+"__main__": cookies = {"key" : "value"} generated_imagse =
+response.generated_imagse asyncio.run(save_generated_imagse(generated_imagse,
+save_path="save_dir", cookies=cookies)) ``` `GeminiImage.save` method logic
+```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies): image_data_dict = await image_client.fetch_images_dict
+(generated_imagse, cookies=cookies) # Get bytes images dict asynchronously
+await image_client.save_images(image_data_dict, save_path=save_path) # Run the
+async function if __name__ == "__main__": cookies = {"key" : "value"}
+generated_imagse = response.generated_imagse # Check response images [Dict]
+asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir",
+cookies=cookies)) ``` > [!NOTE] > Use GeminiImage for image processing.
+`web_images` works without cookies, but for images like `generated_image` from
+Gemini, pass cookies. Cookies are needed to download images from Google's
+storage. Check the response or use existing cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Async downloader* ```python response = client.generate_content("Create
-illustrations of Seoul, South Korea.") response_images = response.web_images #
-Check generated images [Dict] await GeminiImage.save(response_images,
-"save_dir") # image_data_dict = await GeminiImage.fetch_images_dict
-(response_images) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Further *Sync downloader* ```python from gemini import Gemini, GeminiImage
+Gemini. *Async downloader* ```python from gemini import Gemini, GeminiImage
+cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
+(cookies=cookies) response = client.generate_content("Create illustrations of
+Seoul, South Korea.") response_images = response.web_images # Check generated
+images [Dict] await image_client.save(response_images, "save_dir") #
+image_data_dict = await image_client.fetch_images_dict(response_images) # await
+image_client.save_images(image_data_dict, "save_dir") ``` Further *Sync
+downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
+client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Please recommend a travel itinerary for
 Seoul.") response_images = response.web_images # Check response images [Dict]
 GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
-type image dict as follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync
+type image dict as follow: # bytes_images_dict = image_client.fetch_bytes_sync
 (response_images, cookies) # Get bytes images dict #
-GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
-``` *Async downloader wrapper* ```python import asyncio from gemini import
-Gemini, GeminiImage async def save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies): await GeminiImage.save(response_images,
-save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to
+path ``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_response_web_imagse
+(response_images, save_path="save_dir"): await image_client.save
+(response_images, save_path=save_path) # Run the async function if __name__ ==
 "__main__": cookies = {"key" : "value"} response_images = response.web_images
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
-gemini import Gemini, GeminiImage async def save_response_web_imagse
+asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
+``` `GeminiImage.save` method logic ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_response_web_imagse
 (response_images, save_path="save_dir", cookies=cookies): image_data_dict =
-await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
-bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
-save_path=save_path) # Run the async function if __name__ == "__main__":
-response_images = response.web_images # Check response images [Dict]
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
-cookies=cookies)) ```
+await image_client.fetch_images_dict(response_images, cookies=cookies) # Get
+bytes images dict asynchronously await image_client.save_images
+(image_data_dict, save_path=save_path) # Run the async function if __name__ ==
+"__main__": response_images = response.web_images # Check response images
+[Dict] asyncio.run(save_response_web_imagse(response_images,
+save_path="save_dir", cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
-image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
-client.generate_content("What does the text in this image say?", image=image)
-response.response_dict ```
+image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. # Image file
+path or Byte-formatted image array response = client.generate_content("What
+does the text in this image say?", image=image) response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
 gemini.google.com/extensions). Please refer to the [official notice](https://
 support.google.com/gemini/answer/13695044) and review the [privacy policies]
 (https://support.google.com/gemini/answer/13594961?visit_id=638457301410420313-
 1578971242&p=privacy_help&rd=1) for more details. *extention flags* ``` @Gmail,
 @Google Drive, @Google Docs, @Google Maps, @Google Flights, @Google Hotels,
@@ -319,18 +329,22 @@
 crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
 **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
 //crawlbase.com/docs/smart-proxy/
 ?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
 your connection requests to a **randomly rotating IP address** in a pool of
 proxies before reaching the target website. The combination of AI and ML make
-it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
-at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
-xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
-proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+it more effective to avoid CAPTCHAs and blocks. The argument at the [Secure
+Sockets Layer (SSL)](https://en.wikipedia.org/wiki/Transport_Layer_Security)
+level may need to be added to the header. Use it in conjunction with
+`verify=False`. ```python # Get your proxy url at crawlbase https://
+crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://xxxxx:
+@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
+proxy_url} client = Gemini(cookies=cookies, proxies=proxies, timeout=30,
+verify=False) client.session.header["crawlbaseAPI-Parameters"] = "country=US"
 client.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's
 scenery.") ``` ### Reusable session object For standard cases, use Gemini
 class; for exceptions, use session objects. When creating a new bot Gemini
 server, adjust Headers.MAIN. ```python import requests from gemini import
 Gemini, Headers cookies = {} session = requests.Session() session.headers =
 Headers.MAIN for key, value in cookies.items(): session.cookies.update({key:
 value}) client = Gemini(session=session) # You can use various args response =
@@ -396,18 +410,20 @@
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
 huggingface.co/jondurbin/cinematika-7b-v0.1) - `undi95/toppy-m-7b:free` -
 [Undi95/Toppy-M-7B](https://huggingface.co/Undi95/Toppy-M-7B?not-for-all-
 audiences=true) - `gryphe/mythomist-7b:free` - [Gryphe/MythoMist-7b](https://
 huggingface.co/Gryphe/MythoMist-7b) - `nousresearch/nous-capybara-7b:free` -
 [NousResearch/Nous-Capybara-7B-V1](https://huggingface.co/NousResearch/Nous-
 Capybara-7B-V1) from Nous Research
-## Sponsor, [Crawlbase](https://crawlbase.com/) Use [Crawlbase](https://
-crawlbase.com/) API for efficient data scraping to train AI models, boasting a
-98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant,
-supports massive data extraction, and is trusted by 70k+ developers.
+## Sponsor
+[assets/crawlbase.png]
+Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to
+train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to
+start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by
+70k+ developers.
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) First review [HanaokaYuzu/Gemini-API](https://github.com/
 HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://
 aistudio.google.com/) before using this package. You can find most help on the
 [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues)
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
```

### Comparing `python_gemini_api-2.4.7/python_gemini_api.egg-info/SOURCES.txt` & `python_gemini_api-2.4.8/python_gemini_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.7/setup.py` & `python_gemini_api-2.4.8/setup.py`

 * *Files identical despite different names*

