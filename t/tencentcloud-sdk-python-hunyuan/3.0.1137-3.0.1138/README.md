# Comparing `tmp/tencentcloud-sdk-python-hunyuan-3.0.1137.tar.gz` & `tmp/tencentcloud-sdk-python-hunyuan-3.0.1138.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1137.tar", last modified: Thu Apr 25 20:52:12 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1138.tar", last modified: Sun Apr 28 20:52:45 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137.tar` & `tencentcloud-sdk-python-hunyuan-3.0.1138.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/
--rw-r--r--   0 root         (0) root         (0)     2032 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39586 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/hunyuan_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/setup.py
--rw-r--r--   0 root         (0) root         (0)      749 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      539 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/v20230901/
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/v20230901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39983 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/v20230901/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/v20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7419 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/v20230901/hunyuan_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/setup.py
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud_sdk_python_hunyuan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-28 20:52:45.000000 tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1138/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1137
+Version: 3.0.1138
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1137'
+__version__ = '3.0.1138'
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/errorcodes.py` & `tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/v20230901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/models.py` & `tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/v20230901/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 不同的模型计费不同，请根据 [购买指南](https://cloud.tencent.com/document/product/1729/97731) 按需调用。
         :type Model: str
         :param _Messages: 聊天上下文信息。
 说明：
 1. 长度最多为 40，按对话时间从旧到新在数组中排列。
 2. Message.Role 可选值：system、user、assistant。
 其中，system 角色可选，如存在则必须位于列表的最开始。user 和 assistant 需交替出现（一问一答），以 user 提问开始和结束，且 Content 不能为空。Role 的顺序示例：[system（可选） user assistant user assistant user ...]。
-3. Messages 中 Content 总长度不超过 16000 Token，超过则会截断最前面的内容，只保留尾部内容。建议不超过 4000 Token。
+3. Messages 中 Content 总长度不能超过模型输入长度上限（可参考 [产品概述](https://cloud.tencent.com/document/product/1729/104753) 文档），超过则会截断最前面的内容，只保留尾部内容。
         :type Messages: list of Message
         :param _Stream: 流式调用开关。
 说明：
 1. 未传值时默认为非流式调用（false）。
 2. 流式调用时以 SSE 协议增量返回结果（返回值取 Choices[n].Delta 中的值，需要拼接增量数据才能获得完整结果）。
 3. 非流式调用时：
 调用方式与普通 HTTP 请求无异。
@@ -48,18 +48,18 @@
 只返回一次最终结果（返回值取 Choices[n].Message 中的值）。
 
 注意：
 通过 SDK 调用时，流式和非流式调用需用**不同的方式**获取返回值，具体参考 SDK 中的注释或示例（在各语言 SDK 代码仓库的 examples/hunyuan/v20230901/ 目录中）。
         :type Stream: bool
         :param _StreamModeration: 流式输出审核开关。
 说明：
-1. 输出审核有流式和同步两种模式，**流式模式首包响应更快**。
-2. 当使用流式输出（Stream 字段值为 true）时，该字段生效。
+1. 当使用流式输出（Stream 字段值为 true）时，该字段生效。
+2. 输出审核有流式和同步两种模式，**流式模式首包响应更快**。未传值时默认为流式模式（true）。
 3. 如果值为 true，将对输出内容进行分段审核，审核通过的内容流式输出返回。如果出现审核不过，响应中的 FinishReason 值为 sensitive。
-4. 如果未传值或值为 false，则不使用流式输出审核，需要审核完所有输出内容后再返回结果。
+4. 如果值为 false，则不使用流式输出审核，需要审核完所有输出内容后再返回结果。
 
 注意：
 当选择流式输出审核时，可能会出现部分内容已输出，但中间某一段响应中的 FinishReason 值为 sensitive，此时说明安全审核未通过。如果业务场景有实时文字上屏的需求，需要自行撤回已上屏的内容，并建议自定义替换为一条提示语，如 “这个问题我不方便回答，不如我们换个话题试试”，以保障终端体验。
         :type StreamModeration: bool
         :param _TopP: 说明：
 1. 影响输出文本的多样性，取值越大，生成文本的多样性越强。
 2. 默认 1.0，取值区间为 [0.0, 1.0]。
@@ -264,16 +264,17 @@
     """
 
     def __init__(self):
         r"""
         :param _Messages: 聊天上下文信息。
 说明：
 1. 长度最多为 40，按对话时间从旧到新在数组中排列。
-2. Message 的 Role 当前可选值：system、user、assistant。其中，system 角色是可选的，如果存在，必须位于列表的最开始。此外，user 和 assistant 需交替出现（一问一答），以 user 提问开始和结束，且 Content 不能为空。Role 的顺序示例：[system（可选） user assistant user assistant user ...]。
-3. Messages 中 Content 总长度不超过 16000 Token，超过则会截断最前面的内容，只保留尾部内容。建议不超过 4000 Token。
+2. Message.Role 可选值：system、user、assistant。
+其中，system 角色可选，如存在则必须位于列表的最开始。user 和 assistant 需交替出现（一问一答），以 user 提问开始和结束，且 Content 不能为空。Role 的顺序示例：[system（可选） user assistant user assistant user ...]。
+3. Messages 中 Content 总长度不能超过 hunyuan-pro 模型输入长度上限（可参考 [产品概述](https://cloud.tencent.com/document/product/1729/104753) 文档），超过则会截断最前面的内容，只保留尾部内容。
         :type Messages: list of Message
         :param _TopP: 说明：
 1. 影响输出文本的多样性，取值越大，生成文本的多样性越强。
 2. 默认 1.0，取值区间为 [0.0, 1.0]。
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type TopP: float
         :param _Temperature: 说明：
@@ -485,17 +486,17 @@
     """
 
     def __init__(self):
         r"""
         :param _Messages: 聊天上下文信息。
 说明：
 1. 长度最多为 40，按对话时间从旧到新在数组中排列。
-2. Message 的 Role 当前可选值：user、assistant。其中，user 和 assistant 需交替出现（一问一答），以 user 提问开始和结束，且 Content 不能为空。Role 的顺序示例：[user assistant user assistant user ...]。
-3. Messages 中 Content 总长度不超过 16000 Token，超过则会截断最前面的内容，只保留尾部内容。建议不超过 4000 Token。
-
+2. Message 的 Role 当前可选值：user、assistant。
+其中，user 和 assistant 需交替出现（一问一答），以 user 提问开始和结束，且 Content 不能为空。Role 的顺序示例：[user assistant user assistant user ...]。
+3. Messages 中 Content 总长度不能超过 hunyuan-standard 模型输入长度上限（可参考 [产品概述](https://cloud.tencent.com/document/product/1729/104753) 文档），超过则会截断最前面的内容，只保留尾部内容。
         :type Messages: list of Message
         :param _TopP: 说明：
 1. 影响输出文本的多样性，取值越大，生成文本的多样性越强。
 2. 默认 1.0，取值区间为 [0.0, 1.0]。
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type TopP: float
         :param _Temperature: 说明：
@@ -704,15 +705,16 @@
 class Choice(AbstractModel):
     """返回的回复, 支持多个
 
     """
 
     def __init__(self):
         r"""
-        :param _FinishReason: 结束标志位，为 stop 则表示尾包。
+        :param _FinishReason: 结束标志位，可能为 stop 或 sensitive。
+stop 表示输出正常结束，sensitive 只在开启流式输出审核时会出现，表示安全审核未通过。
         :type FinishReason: str
         :param _Delta: 增量返回值，流式调用时使用该字段。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Delta: :class:`tencentcloud.hunyuan.v20230901.models.Delta`
         :param _Message: 返回值，非流式调用时使用该字段。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Message: :class:`tencentcloud.hunyuan.v20230901.models.Message`
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/hunyuan_client.py` & `tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud/hunyuan/v20230901/hunyuan_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChatPro(self, request):
-        """腾讯混元大模型（hunyuan-pro）是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
+        """<span style="font-size:1.5em;">注意：本接口将于 5 月 15 日下线；下线后将不再提供文档指引，接口本身可继续调用，建议使用 [hunyuan](https://cloud.tencent.com/document/api/1729/105701) 接入。</span>
+
+        腾讯混元大模型（hunyuan-pro）是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
 
          1. 本接口暂不支持返回图片内容。
          2. 默认单账号限制并发数为 5 路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
          3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。SDK 链接在文档下方 “**开发者资源 - SDK**” 部分提供。
 
         :param request: Request instance for ChatPro.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatProRequest`
@@ -67,15 +69,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChatStd(self, request):
-        """腾讯混元大模型标准版是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
+        """<span style="font-size:1.5em;">注意：本接口将于 5 月 15 日下线；下线后将不再提供文档指引，接口本身可继续调用，建议使用 [hunyuan](https://cloud.tencent.com/document/api/1729/105701) 接入。</span>
+
+        腾讯混元大模型标准版是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
 
          1. 本接口暂不支持返回图片内容。
          2. 默认单账号限制并发数为 5 路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
          3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。SDK 链接在文档下方 “**开发者资源 - SDK**” 部分提供。
 
         :param request: Request instance for ChatStd.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatStdRequest`
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/setup.py` & `tencentcloud-sdk-python-hunyuan-3.0.1138/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hunyuan',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1137"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1138"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hunyuan SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/README.rst` & `tencentcloud-sdk-python-hunyuan-3.0.1138/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1137
+Version: 3.0.1138
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-hunyuan-3.0.1138/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

