# Comparing `tmp/concopilot_examples-0.0.4.tar.gz` & `tmp/concopilot_examples-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concopilot_examples-0.0.4.tar", last modified: Mon Mar 18 10:02:27 2024, max compression
+gzip compressed data, was "concopilot_examples-0.0.5.tar", last modified: Sun Apr 28 02:36:06 2024, max compression
```

## Comparing `concopilot_examples-0.0.4.tar` & `concopilot_examples-0.0.5.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.714556 concopilot_examples-0.0.4/
--rw-rw-rw-   0        0        0    11558 2023-10-22 06:22:39.000000 concopilot_examples-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      841 2024-03-18 10:02:27.713548 concopilot_examples-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-12-01 03:56:05.000000 concopilot_examples-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.213406 concopilot_examples-0.0.4/concopilot_examples/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.233320 concopilot_examples-0.0.4/concopilot_examples/cerebrum/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.253267 concopilot_examples-0.0.4/concopilot_examples/cerebrum/glmcerebrum/
--rw-rw-rw-   0        0        0      197 2023-11-07 12:38:34.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/glmcerebrum/__init__.py
--rw-rw-rw-   0        0        0     3976 2024-03-16 02:16:33.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/glmcerebrum/glmcerebrum.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.289170 concopilot_examples-0.0.4/concopilot_examples/cerebrum/openaicerebrum/
--rw-rw-rw-   0        0        0      206 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/openaicerebrum/__init__.py
--rw-rw-rw-   0        0        0     9950 2024-03-16 05:56:04.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/openaicerebrum/openaicerebrum.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.312312 concopilot_examples-0.0.4/concopilot_examples/cerebrum/rwkvcerebrum/
--rw-rw-rw-   0        0        0      200 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/rwkvcerebrum/__init__.py
--rw-rw-rw-   0        0        0     3445 2024-03-16 02:16:33.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/rwkvcerebrum/rwkvcerebrum.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.319628 concopilot_examples-0.0.4/concopilot_examples/cerebrum/zhipuaicerebrum/
--rw-rw-rw-   0        0        0      209 2024-03-15 12:05:48.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/zhipuaicerebrum/__init__.py
--rw-rw-rw-   0        0        0    10571 2024-03-16 05:28:02.000000 concopilot_examples-0.0.4/concopilot_examples/cerebrum/zhipuaicerebrum/zhipuaicerebrum.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.329594 concopilot_examples-0.0.4/concopilot_examples/interactor/
--rw-rw-rw-   0        0        0        0 2023-11-14 13:08:35.000000 concopilot_examples-0.0.4/concopilot_examples/interactor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.332610 concopilot_examples-0.0.4/concopilot_examples/interactor/auto/
--rw-rw-rw-   0        0        0      216 2023-11-14 13:08:35.000000 concopilot_examples-0.0.4/concopilot_examples/interactor/auto/__init__.py
--rw-rw-rw-   0        0        0    14847 2024-03-16 03:00:21.000000 concopilot_examples-0.0.4/concopilot_examples/interactor/auto/interactor.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.347736 concopilot_examples-0.0.4/concopilot_examples/interactor/chat/
--rw-rw-rw-   0        0        0      216 2023-11-14 13:08:35.000000 concopilot_examples-0.0.4/concopilot_examples/interactor/chat/__init__.py
--rw-rw-rw-   0        0        0     5836 2024-03-16 06:36:06.000000 concopilot_examples-0.0.4/concopilot_examples/interactor/chat/interactor.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.384084 concopilot_examples-0.0.4/concopilot_examples/interactor/chatwithtool/
--rw-rw-rw-   0        0        0      232 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/interactor/chatwithtool/__init__.py
--rw-rw-rw-   0        0        0    15858 2024-03-16 06:36:06.000000 concopilot_examples-0.0.4/concopilot_examples/interactor/chatwithtool/interactor.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.396572 concopilot_examples-0.0.4/concopilot_examples/interface/
--rw-rw-rw-   0        0        0        0 2023-11-30 05:28:06.000000 concopilot_examples-0.0.4/concopilot_examples/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.397572 concopilot_examples-0.0.4/concopilot_examples/interface/chat/
--rw-rw-rw-   0        0        0        0 2023-11-30 05:28:28.000000 concopilot_examples-0.0.4/concopilot_examples/interface/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.416579 concopilot_examples-0.0.4/concopilot_examples/interface/chat/webchat/
--rw-rw-rw-   0        0        0      213 2023-11-30 06:08:38.000000 concopilot_examples-0.0.4/concopilot_examples/interface/chat/webchat/__init__.py
--rw-rw-rw-   0        0        0     6477 2024-03-17 08:04:02.000000 concopilot_examples-0.0.4/concopilot_examples/interface/chat/webchat/interface.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.428571 concopilot_examples-0.0.4/concopilot_examples/plugin/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.430567 concopilot_examples-0.0.4/concopilot_examples/plugin/duckduckgosearch/
--rw-rw-rw-   0        0        0      212 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/duckduckgosearch/__init__.py
--rw-rw-rw-   0        0        0     1206 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/duckduckgosearch/duckduckgosearch.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.438598 concopilot_examples-0.0.4/concopilot_examples/plugin/image/
--rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.465626 concopilot_examples-0.0.4/concopilot_examples/plugin/image/cropper/
--rw-rw-rw-   0        0        0      193 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/image/cropper/__init__.py
--rw-rw-rw-   0        0        0     1887 2024-03-15 13:56:02.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/image/cropper/cropper.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.477639 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/
--rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.481631 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/card_detection_correction/
--rw-rw-rw-   0        0        0      255 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/card_detection_correction/__init__.py
--rw-rw-rw-   0        0        0     2860 2024-03-12 12:42:15.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/card_detection_correction/card_detection_correction.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.484625 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/ocr_detection/
--rw-rw-rw-   0        0        0      221 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/ocr_detection/__init__.py
--rw-rw-rw-   0        0        0     2790 2024-03-12 12:42:15.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/ocr_detection/ocr_detection.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.494697 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/ocr_recognition/
--rw-rw-rw-   0        0        0      227 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/ocr_recognition/__init__.py
--rw-rw-rw-   0        0        0     2806 2024-03-12 12:42:14.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/ocr_recognition/ocr_recognition.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.500681 concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/
--rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.502676 concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/lmgen/
--rw-rw-rw-   0        0        0      241 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/lmgen/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/lmgen/generator.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.515726 concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/yamlgen/
--rw-rw-rw-   0        0        0      223 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/yamlgen/__init__.py
--rw-rw-rw-   0        0        0      707 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/yamlgen/generator.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.519564 concopilot_examples-0.0.4/concopilot_examples/plugin/summarizer/
--rw-rw-rw-   0        0        0      194 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/summarizer/__init__.py
--rw-rw-rw-   0        0        0     1855 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/summarizer/summarizer.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.532791 concopilot_examples-0.0.4/concopilot_examples/plugin/translator/
--rw-rw-rw-   0        0        0      194 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/translator/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/plugin/translator/translator.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.536783 concopilot_examples-0.0.4/concopilot_examples/resource/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.537780 concopilot_examples-0.0.4/concopilot_examples/resource/category/
--rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.539774 concopilot_examples-0.0.4/concopilot_examples/resource/category/http/
--rw-rw-rw-   0        0        0        0 2023-11-30 05:18:13.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/http/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.541768 concopilot_examples-0.0.4/concopilot_examples/resource/category/http/server/
--rw-rw-rw-   0        0        0        0 2023-11-30 05:18:25.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/http/server/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.544765 concopilot_examples-0.0.4/concopilot_examples/resource/category/http/server/simpleserver/
--rw-rw-rw-   0        0        0      202 2023-11-28 04:56:02.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/http/server/simpleserver/__init__.py
--rw-rw-rw-   0        0        0     1506 2023-11-30 04:10:10.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/http/server/simpleserver/server.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.559720 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/
--rw-rw-rw-   0        0        0        0 2023-11-30 05:16:11.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.563709 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/glmmodel/
--rw-rw-rw-   0        0        0      188 2023-11-07 12:18:32.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/glmmodel/__init__.py
--rw-rw-rw-   0        0        0     5843 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/glmmodel/glmmodel.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.579668 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/modelscope/
--rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/modelscope/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.626539 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/modelscope/pipeline/
--rw-rw-rw-   0        0        0      208 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/modelscope/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1907 2024-03-18 09:32:15.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/modelscope/pipeline/pipeline.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.629531 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/openaimodel/
--rw-rw-rw-   0        0        0      193 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/openaimodel/__init__.py
--rw-rw-rw-   0        0        0     7830 2024-03-16 05:50:52.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/openaimodel/openaimodel.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.633521 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/rwkvmodel/
--rw-rw-rw-   0        0        0      191 2023-10-22 06:44:20.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/rwkvmodel/__init__.py
--rw-rw-rw-   0        0        0     7576 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/rwkvmodel/rwkvmodel.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.654520 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/zhipuaimodel/
--rw-rw-rw-   0        0        0      196 2024-03-15 11:06:51.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/zhipuaimodel/__init__.py
--rw-rw-rw-   0        0        0     3814 2024-03-16 05:36:31.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/model/zhipuaimodel/zhipuaimodel.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.656532 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/
--rw-rw-rw-   0        0        0        0 2023-11-30 05:16:11.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.657696 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/client/
--rw-rw-rw-   0        0        0        0 2023-11-30 05:18:04.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.659693 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/client/simpleclient/
--rw-rw-rw-   0        0        0      212 2023-11-30 06:08:38.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/client/simpleclient/__init__.py
--rw-rw-rw-   0        0        0     1477 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/client/simpleclient/client.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.681756 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/server/
--rw-rw-rw-   0        0        0        0 2023-11-30 05:17:00.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/server/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.684775 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/server/simpleserver/
--rw-rw-rw-   0        0        0      212 2023-11-30 06:08:38.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/server/simpleserver/__init__.py
--rw-rw-rw-   0        0        0     2251 2023-11-30 06:08:38.000000 concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/server/simpleserver/server.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.697807 concopilot_examples-0.0.4/concopilot_examples/util/
--rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/util/__init__.py
--rw-rw-rw-   0        0        0      793 2024-02-24 15:02:37.000000 concopilot_examples-0.0.4/concopilot_examples/util/images.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:02:27.711570 concopilot_examples-0.0.4/concopilot_examples.egg-info/
--rw-rw-rw-   0        0        0      841 2024-03-18 10:02:27.000000 concopilot_examples-0.0.4/concopilot_examples.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4398 2024-03-18 10:02:27.000000 concopilot_examples-0.0.4/concopilot_examples.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 10:02:27.000000 concopilot_examples-0.0.4/concopilot_examples.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-18 10:02:27.000000 concopilot_examples-0.0.4/concopilot_examples.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-18 10:02:27.000000 concopilot_examples-0.0.4/concopilot_examples.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      605 2024-03-10 12:14:51.000000 concopilot_examples-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-18 10:02:27.715545 concopilot_examples-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.247075 concopilot_examples-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2023-10-22 06:22:39.000000 concopilot_examples-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      841 2024-04-28 02:36:06.246079 concopilot_examples-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-12-01 03:56:05.000000 concopilot_examples-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.110442 concopilot_examples-0.0.5/concopilot_examples/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.128393 concopilot_examples-0.0.5/concopilot_examples/cerebrum/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.130387 concopilot_examples-0.0.5/concopilot_examples/cerebrum/glmcerebrum/
+-rw-rw-rw-   0        0        0      197 2023-11-07 12:38:34.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/glmcerebrum/__init__.py
+-rw-rw-rw-   0        0        0     3976 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/glmcerebrum/glmcerebrum.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.135374 concopilot_examples-0.0.5/concopilot_examples/cerebrum/openaicerebrum/
+-rw-rw-rw-   0        0        0      206 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/openaicerebrum/__init__.py
+-rw-rw-rw-   0        0        0     9950 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/openaicerebrum/openaicerebrum.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.138367 concopilot_examples-0.0.5/concopilot_examples/cerebrum/rwkvcerebrum/
+-rw-rw-rw-   0        0        0      200 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/rwkvcerebrum/__init__.py
+-rw-rw-rw-   0        0        0     3445 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/rwkvcerebrum/rwkvcerebrum.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.141358 concopilot_examples-0.0.5/concopilot_examples/cerebrum/zhipuaicerebrum/
+-rw-rw-rw-   0        0        0      209 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/zhipuaicerebrum/__init__.py
+-rw-rw-rw-   0        0        0    10571 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/cerebrum/zhipuaicerebrum/zhipuaicerebrum.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.143353 concopilot_examples-0.0.5/concopilot_examples/interactor/
+-rw-rw-rw-   0        0        0        0 2023-11-14 13:08:35.000000 concopilot_examples-0.0.5/concopilot_examples/interactor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.146345 concopilot_examples-0.0.5/concopilot_examples/interactor/auto/
+-rw-rw-rw-   0        0        0      216 2023-11-14 13:08:35.000000 concopilot_examples-0.0.5/concopilot_examples/interactor/auto/__init__.py
+-rw-rw-rw-   0        0        0    15068 2024-04-26 06:04:24.000000 concopilot_examples-0.0.5/concopilot_examples/interactor/auto/interactor.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.152338 concopilot_examples-0.0.5/concopilot_examples/interactor/chat/
+-rw-rw-rw-   0        0        0      216 2023-11-14 13:08:35.000000 concopilot_examples-0.0.5/concopilot_examples/interactor/chat/__init__.py
+-rw-rw-rw-   0        0        0     6010 2024-04-26 06:04:23.000000 concopilot_examples-0.0.5/concopilot_examples/interactor/chat/interactor.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.154326 concopilot_examples-0.0.5/concopilot_examples/interactor/chatwithtool/
+-rw-rw-rw-   0        0        0      232 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/interactor/chatwithtool/__init__.py
+-rw-rw-rw-   0        0        0    15998 2024-04-26 06:04:23.000000 concopilot_examples-0.0.5/concopilot_examples/interactor/chatwithtool/interactor.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.155322 concopilot_examples-0.0.5/concopilot_examples/interface/
+-rw-rw-rw-   0        0        0        0 2023-11-30 05:28:06.000000 concopilot_examples-0.0.5/concopilot_examples/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.156319 concopilot_examples-0.0.5/concopilot_examples/interface/chat/
+-rw-rw-rw-   0        0        0        0 2023-11-30 05:28:28.000000 concopilot_examples-0.0.5/concopilot_examples/interface/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.158315 concopilot_examples-0.0.5/concopilot_examples/interface/chat/webchat/
+-rw-rw-rw-   0        0        0      213 2023-11-30 06:08:38.000000 concopilot_examples-0.0.5/concopilot_examples/interface/chat/webchat/__init__.py
+-rw-rw-rw-   0        0        0     7523 2024-04-26 09:44:17.000000 concopilot_examples-0.0.5/concopilot_examples/interface/chat/webchat/interface.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.160321 concopilot_examples-0.0.5/concopilot_examples/plugin/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.162303 concopilot_examples-0.0.5/concopilot_examples/plugin/duckduckgosearch/
+-rw-rw-rw-   0        0        0      212 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/duckduckgosearch/__init__.py
+-rw-rw-rw-   0        0        0     1206 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/duckduckgosearch/duckduckgosearch.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.166292 concopilot_examples-0.0.5/concopilot_examples/plugin/image/
+-rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.168287 concopilot_examples-0.0.5/concopilot_examples/plugin/image/cropper/
+-rw-rw-rw-   0        0        0      193 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/image/cropper/__init__.py
+-rw-rw-rw-   0        0        0     1887 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/image/cropper/cropper.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.170292 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/
+-rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.173272 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/card_detection_correction/
+-rw-rw-rw-   0        0        0      255 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/card_detection_correction/__init__.py
+-rw-rw-rw-   0        0        0     2860 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/card_detection_correction/card_detection_correction.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.176265 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/ocr_detection/
+-rw-rw-rw-   0        0        0      221 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/ocr_detection/__init__.py
+-rw-rw-rw-   0        0        0     2790 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/ocr_detection/ocr_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.182256 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/ocr_recognition/
+-rw-rw-rw-   0        0        0      227 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/ocr_recognition/__init__.py
+-rw-rw-rw-   0        0        0     2806 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/ocr_recognition/ocr_recognition.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.183246 concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/
+-rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.185240 concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/lmgen/
+-rw-rw-rw-   0        0        0      241 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/lmgen/__init__.py
+-rw-rw-rw-   0        0        0     1390 2024-04-04 12:46:54.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/lmgen/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.187237 concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/yamlgen/
+-rw-rw-rw-   0        0        0      223 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/yamlgen/__init__.py
+-rw-rw-rw-   0        0        0      694 2024-04-04 12:46:54.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/yamlgen/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.189231 concopilot_examples-0.0.5/concopilot_examples/plugin/summarizer/
+-rw-rw-rw-   0        0        0      194 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/summarizer/__init__.py
+-rw-rw-rw-   0        0        0     1855 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/summarizer/summarizer.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.191225 concopilot_examples-0.0.5/concopilot_examples/plugin/translator/
+-rw-rw-rw-   0        0        0      194 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/translator/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/plugin/translator/translator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.197209 concopilot_examples-0.0.5/concopilot_examples/resource/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.198207 concopilot_examples-0.0.5/concopilot_examples/resource/category/
+-rw-rw-rw-   0        0        0        0 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.199204 concopilot_examples-0.0.5/concopilot_examples/resource/category/http/
+-rw-rw-rw-   0        0        0        0 2023-11-30 05:18:13.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/http/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.200201 concopilot_examples-0.0.5/concopilot_examples/resource/category/http/server/
+-rw-rw-rw-   0        0        0        0 2023-11-30 05:18:25.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/http/server/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.202198 concopilot_examples-0.0.5/concopilot_examples/resource/category/http/server/simpleserver/
+-rw-rw-rw-   0        0        0      202 2023-11-28 04:56:02.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/http/server/simpleserver/__init__.py
+-rw-rw-rw-   0        0        0     1506 2023-11-30 04:10:10.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/http/server/simpleserver/server.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.203193 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/
+-rw-rw-rw-   0        0        0        0 2023-11-30 05:16:11.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.205201 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/glmmodel/
+-rw-rw-rw-   0        0        0      188 2023-11-07 12:18:32.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/glmmodel/__init__.py
+-rw-rw-rw-   0        0        0     5843 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/glmmodel/glmmodel.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.207183 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/modelscope/
+-rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/modelscope/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.213165 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/modelscope/pipeline/
+-rw-rw-rw-   0        0        0      208 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/modelscope/pipeline/__init__.py
+-rw-rw-rw-   0        0        0     1907 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/modelscope/pipeline/pipeline.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.218153 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/openaimodel/
+-rw-rw-rw-   0        0        0      193 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/openaimodel/__init__.py
+-rw-rw-rw-   0        0        0     7830 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/openaimodel/openaimodel.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.220153 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/rwkvmodel/
+-rw-rw-rw-   0        0        0      191 2023-10-22 06:44:20.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/rwkvmodel/__init__.py
+-rw-rw-rw-   0        0        0     7576 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/rwkvmodel/rwkvmodel.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.223152 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/zhipuaimodel/
+-rw-rw-rw-   0        0        0      196 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/zhipuaimodel/__init__.py
+-rw-rw-rw-   0        0        0     3814 2024-03-18 12:46:17.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/model/zhipuaimodel/zhipuaimodel.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.229123 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/
+-rw-rw-rw-   0        0        0        0 2023-11-30 05:16:11.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.230121 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/client/
+-rw-rw-rw-   0        0        0        0 2023-11-30 05:18:04.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.232116 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/client/simpleclient/
+-rw-rw-rw-   0        0        0      212 2023-11-30 06:08:38.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/client/simpleclient/__init__.py
+-rw-rw-rw-   0        0        0     1477 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/client/simpleclient/client.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.234110 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/server/
+-rw-rw-rw-   0        0        0        0 2023-11-30 05:17:00.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/server/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.236105 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/server/simpleserver/
+-rw-rw-rw-   0        0        0      212 2023-11-30 06:08:38.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/server/simpleserver/__init__.py
+-rw-rw-rw-   0        0        0     2251 2023-11-30 06:08:38.000000 concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/server/simpleserver/server.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.243086 concopilot_examples-0.0.5/concopilot_examples/util/
+-rw-rw-rw-   0        0        0        0 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/util/__init__.py
+-rw-rw-rw-   0        0        0      793 2024-02-24 15:02:37.000000 concopilot_examples-0.0.5/concopilot_examples/util/images.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:36:06.244084 concopilot_examples-0.0.5/concopilot_examples.egg-info/
+-rw-rw-rw-   0        0        0      841 2024-04-28 02:36:05.000000 concopilot_examples-0.0.5/concopilot_examples.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4398 2024-04-28 02:36:06.000000 concopilot_examples-0.0.5/concopilot_examples.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 02:36:05.000000 concopilot_examples-0.0.5/concopilot_examples.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 02:36:05.000000 concopilot_examples-0.0.5/concopilot_examples.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-28 02:36:05.000000 concopilot_examples-0.0.5/concopilot_examples.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      605 2024-04-04 12:46:54.000000 concopilot_examples-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 02:36:06.247075 concopilot_examples-0.0.5/setup.cfg
```

### Comparing `concopilot_examples-0.0.4/LICENSE` & `concopilot_examples-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/PKG-INFO` & `concopilot_examples-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: concopilot_examples
-Version: 0.0.4
+Version: 0.0.5
 Summary: ConCopilot simple examples.
 Author-email: ZHONG Weikun <zhong.weikun@live.com>
 Project-URL: Homepage, https://github.com/ConCopilot/concopilot-examples
 Project-URL: Bug Tracker, https://github.com/ConCopilot/concopilot-examples/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: concopilot>=0.0.4
+Requires-Dist: concopilot>=0.0.5
 
 # ConCopilot Example Components
 
 This repository provides examples of ConCopilot components varying in various types.
 
 These components are fully functional and can be directly used in ConCopilot framework for LLM Agents.
```

### Comparing `concopilot_examples-0.0.4/concopilot_examples/cerebrum/glmcerebrum/glmcerebrum.py` & `concopilot_examples-0.0.5/concopilot_examples/cerebrum/glmcerebrum/glmcerebrum.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/cerebrum/openaicerebrum/openaicerebrum.py` & `concopilot_examples-0.0.5/concopilot_examples/cerebrum/openaicerebrum/openaicerebrum.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/cerebrum/rwkvcerebrum/rwkvcerebrum.py` & `concopilot_examples-0.0.5/concopilot_examples/cerebrum/rwkvcerebrum/rwkvcerebrum.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/cerebrum/zhipuaicerebrum/zhipuaicerebrum.py` & `concopilot_examples-0.0.5/concopilot_examples/cerebrum/zhipuaicerebrum/zhipuaicerebrum.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/interactor/auto/interactor.py` & `concopilot_examples-0.0.5/concopilot_examples/interactor/auto/interactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,33 +71,35 @@
             asset_id=self.message_summary_key,
             name='message summary',
             description='The summary of interaction messages between you, plugins, and the user. This is for reminding you with events from your past.',
             content_type='text/plain',
             content=msg_summary
         )
         self.context.assets.update(self.context.storage.get_or_default(self.assets_key, {}))
-        while True:
+        msg=None
+        self.status=BasicInteractor.Status.RUNNING
+        while self.status==BasicInteractor.Status.RUNNING:
             try:
                 if self.context.user_interface.has_user_msg():
                     count=0
                     while msg:=self.context.user_interface.get_user_msg():
                         if msg is not None:
                             if msg.receiver and msg.receiver.role=='interactor':
-                                self.context.user_interface.send_msg_user(self.on_msg(msg))
+                                self.context.user_interface.send_msg_to_user(self.on_msg(msg))
                             else:
                                 self._check_msg(msg, Identity(role='user', id=None, name=None))
                                 self.message_history.append(msg)
                                 count+=1
                         if not self.context.user_interface.has_user_msg():
                             break
                     cerebrum_command=cerebrum_command+f' Note that {count} incoming user message detected.'
 
                 response, message_history_start=self._interact_with_cerebrum(cerebrum_command, message_history_start, self.context.assets)
                 try:
-                    msg=self.message_manager.parse(response)[0]
+                    msg=self.message_manager.parse(response, thrd_id=msg.thrd_id if msg else None)[0]
                 except Exception as e:
                     logger.error('Failed to parse the cerebrum response message.', exc_info=e)
                     raise ValueError('Failed to parse the cerebrum response message, maybe the response format is not acceptable.')
                 self._check_msg(msg, Identity(role='cerebrum', id=self.cerebrum.id, name=self.cerebrum.name))
 
                 self.message_history.append(Message(
                     sender=Identity(role='user'),
@@ -121,19 +123,19 @@
                             else:
                                 raise ValueError(f'Unknown "command" in the "content" section! Got "{msg.content.command}", but only "error" and "exit" are acceptable.')
                         else:
                             raise ValueError('The "content" section is supposed to be a Dict!')
                     elif msg.receiver.role=='cerebrum':
                         pass
                     elif msg.receiver.role=='user':
-                        self.context.user_interface.send_msg_user(msg)
+                        self.context.user_interface.send_msg_to_user(msg)
                         while msg:=self.context.user_interface.wait_user_msg():
                             if msg is not None:
                                 if msg.receiver and msg.receiver.role=='interactor':
-                                    self.context.user_interface.send_msg_user(self.on_msg(msg))
+                                    self.context.user_interface.send_msg_to_user(self.on_msg(msg))
                                 else:
                                     break
                             else:
                                 logger.error('User interface pipeline is broken. Will exit.')
                                 break
                         if not msg:
                             break
@@ -161,29 +163,31 @@
                         detail=str(e)
                     )
                 )
                 self._check_msg(msg, Identity(role='system', id=None, name=None))
                 self.message_history.append(msg)
                 cerebrum_command='An error happened during the thinking loop. Check the error in the interaction messages, and try to fix the error and determine which next command to use, and respond using the json format specified above.'
 
+        self.status=BasicInteractor.Status.STOPPED
+
     def _check_msg(self, msg: Message, sender: Identity) -> Message:
         if sender is not None:
             msg.sender=sender
         msg.time=settings.current_time()
         if msg.content and not Asset.is_trivial(msg.content):
             asset=Asset(
                 asset_type=f'message content from `{sender if isinstance(sender, str) else "::".join([sender.role, sender.name])}`',
                 content_type=str(type(msg.content)),
                 content=msg.content
             )
             msg.content_type='asset_ref'
             self.context.assets[str(asset.asset_id)]=asset
             msg.content=AssetRef(asset_id=asset.asset_id)
         if AutoInteractor._need_convert_to_status(msg):
-            self.context.user_interface.send_msg_user(AutoInteractor._status_msg(msg))
+            self.context.user_interface.send_msg_to_user(AutoInteractor._status_msg(msg))
         logger.debug('\n'+json.dumps(msg, cls=JsonEncoder, ensure_ascii=False, indent=4)+'\n')
         return msg
 
     @staticmethod
     def _need_convert_to_status(msg: Message) -> bool:
         return (not msg.sender or msg.sender.role!='user') and (not msg.receiver or msg.receiver.role!='user')
 
@@ -207,23 +211,23 @@
             msg=Message(
                 sender=Identity(role='system'),
                 content_type='text/plain',
                 content='Please input your goals:',
                 time=settings.current_time()
             )
             self._goal_prompt_msg_list.append(msg)
-            self.context.user_interface.send_msg_user(msg)
+            self.context.user_interface.send_msg_to_user(msg)
             while msg:=self.context.user_interface.wait_user_msg():
                 if msg is not None:
                     if msg.receiver and msg.receiver.role=='interactor':
-                        self.context.user_interface.send_msg_user(self.on_msg(msg))
+                        self.context.user_interface.send_msg_to_user(self.on_msg(msg))
                     else:
                         break
                 else:
-                    logger.error('User interface pipeline is broken. Will exit.')
+                    logger.warning('User interface pipeline is broken. Will exit.')
                     return False
             self._goal_prompt_msg_list.append(msg)
             self.goals=msg.content.split('\n')
 
         instruction=self.instruction\
             .replace('{ai_name}', self.cerebrum.name)\
             .replace('{ai_role}', self.cerebrum.role)\
```

### Comparing `concopilot_examples-0.0.4/concopilot_examples/interactor/chat/interactor.py` & `concopilot_examples-0.0.5/concopilot_examples/interactor/chat/interactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,18 @@
                 sender=Identity(role='cerebrum', name=self.cerebrum.name),
                 receiver=Identity(role='user'),
                 content_type='text/plain',
                 content=self.hello_msg_content,
                 time=settings.current_time()
             )
             self.message_history.append(msg)
-        while True:
+        self.status=BasicInteractor.Status.RUNNING
+        while self.status==BasicInteractor.Status.RUNNING:
             try:
-                self.context.user_interface.send_msg_user(msg)
+                self.context.user_interface.send_msg_to_user(msg)
                 msg=self._check_user_msg()
                 if msg is None or msg.content in self.exit_tokens:
                     break
                 msg=self._interact_with_cerebrum(msg)
             except Exception as e:
                 logger.error('An error happened.', exc_info=e)
                 msg=Message(
@@ -82,37 +83,39 @@
                     ),
                     time=settings.current_time()
                 )
 
         if self.persist_history:
             self.context.storage.put(self.message_history_key, self.message_history)
 
+        self.status=BasicInteractor.Status.STOPPED
+
     def _check_user_msg(self):
         while msg:=self.context.user_interface.wait_user_msg():
             if msg is not None:
                 if msg.receiver and msg.receiver.role=='interactor':
-                    self.context.user_interface.send_msg_user(self.on_msg(msg))
+                    self.context.user_interface.send_msg_to_user(self.on_msg(msg))
                 else:
                     break
             else:
-                logger.error('User interface pipeline is broken. Will exit.')
+                logger.warning('User interface pipeline is broken. Will exit.')
                 break
         return msg
 
     def _interact_with_cerebrum(self, msg):
         self.message_history.append(msg)
         response=self.cerebrum.interact(param=InteractParameter(
             instructions=self.instructions,
             command=None,
             message_history=self.message_history,
             assets=[asset for asset in self.context.assets.values()],
             require_token_len=False,
             require_cost=False
         ), **self.llm_param)
-        msg=self.message_manager.parse(response)[0]
+        msg=self.message_manager.parse(response, thrd_id=msg.thrd_id)[0]
         msg.sender=Identity(role='cerebrum', id=self.cerebrum.id, name=self.cerebrum.name)
         if msg.receiver is None:
             msg.receiver=Identity(role='user')
         self.message_history.append(msg)
         return msg
 
     def set_llm_param(self, update: Dict, remove: List) -> Dict:
```

### Comparing `concopilot_examples-0.0.4/concopilot_examples/interactor/chatwithtool/interactor.py` & `concopilot_examples-0.0.5/concopilot_examples/interactor/chatwithtool/interactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         self.wait_user_comment: bool = self.config.config.wait_user_comment
         self.exit_tokens: set[str] = set(self.config.config.exit_tokens)
 
         self.llm_param={}
         self.message_history: List[Message] = []
         self.message_history_start: int = 0
 
+        self._thrd_id=None
+
     def setup_prompts(self):
         super(ChatWithToolInteractor, self).setup_prompts()
         if self.config.config.instruction_file:
             with open(self.config_file_path(self.config.config.instruction_file), encoding='utf8') as file:
                 instruction=file.read()
             instruction=instruction\
                 .replace('{ai_name}', self.cerebrum.name)\
@@ -100,15 +102,16 @@
             )
             self.message_history.append(msg)
             self._check_and_send_msg_to_user(msg)
             if not self._wait_user_msg():
                 return
             msg_list=self._interact_with_cerebrum()
 
-        while True:
+        self.status=BasicInteractor.Status.RUNNING
+        while self.status==BasicInteractor.Status.RUNNING:
             try:
                 has_user_msg=False
                 for msg in msg_list:
                     try:
                         self._check_and_send_msg_to_user(msg)
                         if msg.receiver is None:
                             raise ValueError(f'A `receiver` section is required in message `{json.dumps(msg, cls=JsonEncoder, ensure_ascii=False, indent=2)}`!')
@@ -161,14 +164,16 @@
                     time=settings.current_time()
                 )
                 self.message_history.append(msg)
                 self._check_and_send_msg_to_user(msg)
                 if not self._wait_user_msg():
                     break
 
+        self.status=BasicInteractor.Status.STOPPED
+
     def _check_msg_serializable(self, msg: Message) -> Message:
         msg.time=settings.current_time()
         if msg.content and not Asset.is_trivial(msg.content):
             asset=Asset(
                 asset_type=f'message content from `{msg.sender if isinstance(msg.sender, str) else "::".join([msg.sender.role, msg.sender.name])}`',
                 content_type=str(type(msg.content)),
                 content=msg.content
@@ -224,60 +229,60 @@
                         else:
                             return None
 
         return msg_to_user
 
     def _check_and_send_msg_to_user(self, msg):
         if (msg:=self._get_msg_to_user(msg)) is not None:
-            self.context.user_interface.send_msg_user(msg)
+            self.context.user_interface.send_msg_to_user(msg)
 
     def _check_user_msg(self) -> bool:
-        if self.context.user_interface.has_user_msg():
-            while msg:=self.context.user_interface.get_user_msg():
-                if msg is not None:
-                    if msg.receiver and msg.receiver.role=='interactor':
-                        self.context.user_interface.send_msg_user(self.on_msg(msg))
-                    else:
-                        if msg is None or msg.content in self.exit_tokens:
-                            return False
-                        msg.sender=Identity(role='user')
-                        msg=self._check_msg_serializable(msg)
-                        self.message_history.append(msg)
-                if not self.context.user_interface.has_user_msg():
-                    break
+        while self.context.user_interface.has_user_msg():
+            msg=self.context.user_interface.get_user_msg()
+            if msg is not None:
+                if msg.receiver and msg.receiver.role=='interactor':
+                    self.context.user_interface.send_msg_to_user(self.on_msg(msg))
+                else:
+                    if msg.content in self.exit_tokens:
+                        return False
+                    msg.sender=Identity(role='user')
+                    self._thrd_id=msg.thrd_id
+                    msg=self._check_msg_serializable(msg)
+                    self.message_history.append(msg)
         return True
 
     def _wait_user_msg(self) -> bool:
         while msg:=self.context.user_interface.wait_user_msg():
             if msg is not None:
                 if msg.receiver and msg.receiver.role=='interactor':
-                    self.context.user_interface.send_msg_user(self.on_msg(msg))
+                    self.context.user_interface.send_msg_to_user(self.on_msg(msg))
                 else:
                     break
             else:
-                logger.error('User interface pipeline is broken. Will exit.')
+                logger.warning('User interface pipeline is broken. Will exit.')
                 break
         if msg is None or msg.content in self.exit_tokens:
             return False
         msg.sender=Identity(role='user')
+        self._thrd_id=msg.thrd_id
         msg=self._check_msg_serializable(msg)
         self.message_history.append(msg)
         return True
 
     def _interact_with_cerebrum(self) -> List[Message]:
         response=self.cerebrum.interact(param=InteractParameter(
             instructions=self.instructions,
             command=None,
             message_history=self.message_history,
             assets=[asset for asset in self.context.assets.values()],
             require_token_len=False,
             require_cost=False
         ), **self.llm_param)
         try:
-            msg_list=self.message_manager.parse(response)
+            msg_list=self.message_manager.parse(response, thrd_id=self._thrd_id)
         except Exception as e:
             logger.error('Failed to parse the cerebrum response message.', exc_info=e)
             raise ValueError('Failed to parse the cerebrum response message, maybe the response format is not a legal JSON.')
         for msg in msg_list:
             msg.sender=Identity(role='cerebrum', id=self.cerebrum.id, name=self.cerebrum.name)
             if msg.receiver is None:
                 msg.receiver=Identity(role='user')
```

### Comparing `concopilot_examples-0.0.4/concopilot_examples/interface/chat/webchat/interface.py` & `concopilot_examples-0.0.5/concopilot_examples/interface/chat/webchat/interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 
 import os
 import re
 import json
 import uuid
 import yaml
 import zipfile
+import threading
 import logging
 import numpy as np
 from PIL import Image
 
 from typing import Dict, Optional
 
-from concopilot.framework.interface import UserInterface
+from concopilot.framework.interface import AgentDrivenSimplexUserInterface
 from concopilot.framework.message import Message
 from concopilot.framework.asset import AssetRef
 from concopilot.framework.asset import asset_regex
 from concopilot.util.jsons import JsonEncoder
 from concopilot.util.yamls import YamlDumper
 from concopilot.util import ClassDict
 from ....util import images
 
 
 logger=logging.getLogger(__file__)
 
 
-class WebChatUserInterface(UserInterface):
+class WebChatUserInterface(AgentDrivenSimplexUserInterface):
     def __init__(self, config: Dict):
         super(WebChatUserInterface, self).__init__(config)
         self._role_mapping=self.config.config.role_mapping
         self._dist_path=self.config.config.dist_path if self.config.config.dist_path else self.config_file_path('dist')
         self._websocket=None
         self._msg_cache=[]
         self._msg=None
@@ -44,23 +45,38 @@
             slider_params=self.config.config.slider_params,
             role_mapping=self.config.config.role_mapping,
             options=self.config.config.options
         )
         with open(os.path.join(self._dist_path, 'config.yaml'), 'w', encoding='utf8') as f:
             yaml.dump(web_config, f, Dumper=YamlDumper)
 
+        self._interrupt_checking_timeout=self.config.config.interrupt_checking_timeout if (self.config.config.interrupt_checking_timeout is not None and self.config.config.interrupt_checking_timeout>0) else 1
+        self._interrupted: threading.Event = threading.Event()
+
     @property
     def websocket(self):
         if self._websocket is None:
             self._websocket=self.resources[0]
         return self._websocket
 
     def _recv_msg(self, timeout):
         try:
-            msg=self.websocket.recv(timeout=timeout)
+            if timeout is None:
+                while not self.interrupted:
+                    try:
+                        msg=self.websocket.recv(timeout=self._interrupt_checking_timeout)
+                        break
+                    except TimeoutError:
+                        pass
+                else:
+                    raise InterruptedError('_recv_msg has been interrupted.')
+            elif not self.interrupted:
+                msg=self.websocket.recv(timeout=timeout)
+            else:
+                raise InterruptedError('_recv_msg has been interrupted.')
         except TimeoutError:
             msg=None
         if msg is not None:
             msg=Message(**json.loads(msg))
             if isinstance(msg.content, str):
                 msg.content=msg.content.strip()
         return msg
@@ -69,41 +85,41 @@
         if self._msg is None:
             if len(self._msg_cache)>0:
                 self._msg=self._msg_cache.pop(0)
             else:
                 self._msg=self._recv_msg(timeout=timeout)
         return self._msg
 
-    def send_msg_user(self, msg: Message):
+    def send_msg_to_user(self, msg: Message):
         if msg.sender and msg.sender.role=='interactor' and msg.content_type=='command' and msg.content and msg.content.command=='retrieve_history' and msg.content.response:
             histories=msg.content.response.histories
             msg.content.response.histories=[]
-            self._send_msg_user_single(msg)
+            self._send_msg_to_user_single(msg)
             for m in histories:
-                self._send_msg_user_single(m)
+                self._send_msg_to_user_single(m)
         else:
-            self._send_msg_user_single(msg)
+            self._send_msg_to_user_single(msg)
 
-    def _send_msg_user_single(self, msg: Message):
+    def _send_msg_to_user_single(self, msg: Message):
         if not msg.id and self.config.config.add_msg_id:
             msg.id=uuid.uuid4()
         if msg.content_type and ((content_type:=msg.content_type.strip()).startswith('image/') or content_type=='image' or content_type=='img'):
             msg.content=WebChatUserInterface._convert_img_src(AssetRef.try_retrieve(msg.content, self.context.assets))
             msg=json.dumps(msg, cls=JsonEncoder, ensure_ascii=False)
         else:
             msg=json.dumps(msg, cls=JsonEncoder, ensure_ascii=False)
             msg='```'.join([(self._check_asset_refs(x) if idx%2==0 else x) for idx, x in enumerate(msg.split('```'))])
         self.websocket.send(msg)
 
-    def on_msg_user(self, msg: Message) -> Optional[Message]:
+    def on_msg_to_user(self, msg: Message) -> Optional[Message]:
         if not msg.thrd_id:
             msg=Message(**msg)
             msg.thrd_id=str(uuid.uuid4())
         thrd_id=msg.thrd_id
-        self.send_msg_user(msg)
+        self.send_msg_to_user(msg)
         while msg:=self._recv_msg(timeout=None):
             if msg.thrd_id==thrd_id:
                 return msg
             else:
                 self._msg_cache.append(msg)
 
     def has_user_msg(self) -> bool:
@@ -159,7 +175,14 @@
                 data=asset_ref.retrieve(self.context.assets)
                 return str(data)
             else:
                 return match_obj.group(0)
         except Exception as e:
             logger.error('AssetRef error during converting.', exc_info=e)
             return match_obj.group(0)
+
+    def interrupt(self):
+        self._interrupted.set()
+
+    @property
+    def interrupted(self) -> bool:
+        return self._interrupted.is_set()
```

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/duckduckgosearch/duckduckgosearch.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/duckduckgosearch/duckduckgosearch.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/image/cropper/cropper.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/image/cropper/cropper.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/card_detection_correction/card_detection_correction.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/card_detection_correction/card_detection_correction.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/ocr_detection/ocr_detection.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/ocr_detection/ocr_detection.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/modelscope/ocr_recognition/ocr_recognition.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/modelscope/ocr_recognition/ocr_recognition.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/lmgen/generator.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/lmgen/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 
 import yaml
-import uuid
 
 from typing import Dict
 
 from concopilot.framework.plugin import Plugin, PluginPromptGenerator
 from concopilot.framework.resource.category import LLM
 from concopilot.util.yamls import YamlDumper
```

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/promptgenerator/yamlgen/generator.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/promptgenerator/yamlgen/generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 
 import yaml
-import uuid
 
 from typing import Dict
 
 from concopilot.framework.plugin import Plugin, PluginPromptGenerator
 from concopilot.util.yamls import YamlDumper
```

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/summarizer/summarizer.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/summarizer/summarizer.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/plugin/translator/translator.py` & `concopilot_examples-0.0.5/concopilot_examples/plugin/translator/translator.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/resource/category/http/server/simpleserver/server.py` & `concopilot_examples-0.0.5/concopilot_examples/resource/category/http/server/simpleserver/server.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/resource/category/model/glmmodel/glmmodel.py` & `concopilot_examples-0.0.5/concopilot_examples/resource/category/model/glmmodel/glmmodel.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/resource/category/model/modelscope/pipeline/pipeline.py` & `concopilot_examples-0.0.5/concopilot_examples/resource/category/model/modelscope/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/resource/category/model/openaimodel/openaimodel.py` & `concopilot_examples-0.0.5/concopilot_examples/resource/category/model/openaimodel/openaimodel.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/resource/category/model/rwkvmodel/rwkvmodel.py` & `concopilot_examples-0.0.5/concopilot_examples/resource/category/model/rwkvmodel/rwkvmodel.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/resource/category/model/zhipuaimodel/zhipuaimodel.py` & `concopilot_examples-0.0.5/concopilot_examples/resource/category/model/zhipuaimodel/zhipuaimodel.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/client/simpleclient/client.py` & `concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/client/simpleclient/client.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/resource/category/websocket/server/simpleserver/server.py` & `concopilot_examples-0.0.5/concopilot_examples/resource/category/websocket/server/simpleserver/server.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples/util/images.py` & `concopilot_examples-0.0.5/concopilot_examples/util/images.py`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/concopilot_examples.egg-info/PKG-INFO` & `concopilot_examples-0.0.5/concopilot_examples.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: concopilot_examples
-Version: 0.0.4
+Version: 0.0.5
 Summary: ConCopilot simple examples.
 Author-email: ZHONG Weikun <zhong.weikun@live.com>
 Project-URL: Homepage, https://github.com/ConCopilot/concopilot-examples
 Project-URL: Bug Tracker, https://github.com/ConCopilot/concopilot-examples/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: concopilot>=0.0.4
+Requires-Dist: concopilot>=0.0.5
 
 # ConCopilot Example Components
 
 This repository provides examples of ConCopilot components varying in various types.
 
 These components are fully functional and can be directly used in ConCopilot framework for LLM Agents.
```

### Comparing `concopilot_examples-0.0.4/concopilot_examples.egg-info/SOURCES.txt` & `concopilot_examples-0.0.5/concopilot_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `concopilot_examples-0.0.4/pyproject.toml` & `concopilot_examples-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name="concopilot_examples"
-version="0.0.4"
+version="0.0.5"
 authors=[
     {name="ZHONG Weikun", email="zhong.weikun@live.com"}
 ]
 description="ConCopilot simple examples."
 readme="README.md"
 requires-python=">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies=[
-    "concopilot>=0.0.4"
+    "concopilot>=0.0.5"
 ]
 
 [project.urls]
 "Homepage"="https://github.com/ConCopilot/concopilot-examples"
 "Bug Tracker"="https://github.com/ConCopilot/concopilot-examples/issues"
 
 [tool.setuptools.packages.find]
```

