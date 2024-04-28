# Comparing `tmp/tencentcloud-sdk-python-lke-3.0.1137.tar.gz` & `tmp/tencentcloud-sdk-python-lke-3.0.1138.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1137.tar", last modified: Thu Apr 25 20:56:55 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1138.tar", last modified: Sun Apr 28 20:56:15 2024, max compression
```

## Comparing `tencentcloud-sdk-python-lke-3.0.1137.tar` & `tencentcloud-sdk-python-lke-3.0.1138.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud_sdk_python_lke.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud_sdk_python_lke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud_sdk_python_lke.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/v20231130/
--rw-r--r--   0 root         (0) root         (0)      707 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/v20231130/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   359667 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/v20231130/models.py
--rw-r--r--   0 root         (0) root         (0)    63936 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/v20231130/lke_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/v20231130/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/setup.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-04-25 20:56:55.000000 tencentcloud-sdk-python-lke-3.0.1137/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:56:15.000000 tencentcloud-sdk-python-lke-3.0.1138/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-28 20:56:15.000000 tencentcloud-sdk-python-lke-3.0.1138/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:56:15.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud_sdk_python_lke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud_sdk_python_lke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud_sdk_python_lke.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:56:15.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:56:15.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 20:56:15.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/v20231130/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/v20231130/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   379477 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/v20231130/models.py
+-rw-r--r--   0 root         (0) root         (0)    66032 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/v20231130/lke_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/v20231130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-28 20:56:15.000000 tencentcloud-sdk-python-lke-3.0.1138/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/setup.py
+-rw-r--r--   0 root         (0) root         (0)      737 2024-04-28 20:56:14.000000 tencentcloud-sdk-python-lke-3.0.1138/README.rst
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1137/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1138/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1137
+Version: 3.0.1138
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1137/tencentcloud_sdk_python_lke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1138/tencentcloud_sdk_python_lke.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1137
+Version: 3.0.1138
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/v20231130/models.py` & `tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/v20231130/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -975,17 +975,21 @@
         r"""
         :param _Model: 模型配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type Model: :class:`tencentcloud.lke.v20231130.models.AppModel`
         :param _Labels: 标签列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type Labels: list of ClassifyLabel
+        :param _Greeting: 欢迎语，200字符以内
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Greeting: str
         """
         self._Model = None
         self._Labels = None
+        self._Greeting = None
 
     @property
     def Model(self):
         return self._Model
 
     @Model.setter
     def Model(self, Model):
@@ -995,25 +999,34 @@
     def Labels(self):
         return self._Labels
 
     @Labels.setter
     def Labels(self, Labels):
         self._Labels = Labels
 
+    @property
+    def Greeting(self):
+        return self._Greeting
+
+    @Greeting.setter
+    def Greeting(self, Greeting):
+        self._Greeting = Greeting
+
 
     def _deserialize(self, params):
         if params.get("Model") is not None:
             self._Model = AppModel()
             self._Model._deserialize(params.get("Model"))
         if params.get("Labels") is not None:
             self._Labels = []
             for item in params.get("Labels"):
                 obj = ClassifyLabel()
                 obj._deserialize(item)
                 self._Labels.append(obj)
+        self._Greeting = params.get("Greeting")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2567,28 +2580,34 @@
         :type NameInAppeal: bool
         :param _GreetingInAppeal: 欢迎语是否在申诉中
         :type GreetingInAppeal: bool
         :param _BareAnswerInAppeal: 未知问题回复语是否在申诉中
         :type BareAnswerInAppeal: bool
         :param _AppKey: 应用appKey
         :type AppKey: str
+        :param _AppStatus: 应用状态，1：未上线，2：运行中，3：停用
+        :type AppStatus: int
+        :param _AppStatusDesc: 状态说明
+        :type AppStatusDesc: str
         :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._AppBizId = None
         self._AppType = None
         self._AppTypeDesc = None
         self._BaseConfig = None
         self._AppConfig = None
         self._AvatarInAppeal = None
         self._RoleInAppeal = None
         self._NameInAppeal = None
         self._GreetingInAppeal = None
         self._BareAnswerInAppeal = None
         self._AppKey = None
+        self._AppStatus = None
+        self._AppStatusDesc = None
         self._RequestId = None
 
     @property
     def AppBizId(self):
         return self._AppBizId
 
     @AppBizId.setter
@@ -2672,14 +2691,30 @@
         return self._AppKey
 
     @AppKey.setter
     def AppKey(self, AppKey):
         self._AppKey = AppKey
 
     @property
+    def AppStatus(self):
+        return self._AppStatus
+
+    @AppStatus.setter
+    def AppStatus(self, AppStatus):
+        self._AppStatus = AppStatus
+
+    @property
+    def AppStatusDesc(self):
+        return self._AppStatusDesc
+
+    @AppStatusDesc.setter
+    def AppStatusDesc(self, AppStatusDesc):
+        self._AppStatusDesc = AppStatusDesc
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -2696,14 +2731,16 @@
             self._AppConfig._deserialize(params.get("AppConfig"))
         self._AvatarInAppeal = params.get("AvatarInAppeal")
         self._RoleInAppeal = params.get("RoleInAppeal")
         self._NameInAppeal = params.get("NameInAppeal")
         self._GreetingInAppeal = params.get("GreetingInAppeal")
         self._BareAnswerInAppeal = params.get("BareAnswerInAppeal")
         self._AppKey = params.get("AppKey")
+        self._AppStatus = params.get("AppStatus")
+        self._AppStatusDesc = params.get("AppStatusDesc")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeAttributeLabelRequest(AbstractModel):
     """DescribeAttributeLabel请求参数结构体
 
     """
@@ -4120,28 +4157,52 @@
 
     """
 
     def __init__(self):
         r"""
         :param _BotBizId: 机器人ID
         :type BotBizId: str
+        :param _FileType: 文件类型
+        :type FileType: str
+        :param _IsPublic: 权限场景，是否公有权限
+        :type IsPublic: bool
         """
         self._BotBizId = None
+        self._FileType = None
+        self._IsPublic = None
 
     @property
     def BotBizId(self):
         return self._BotBizId
 
     @BotBizId.setter
     def BotBizId(self, BotBizId):
         self._BotBizId = BotBizId
 
+    @property
+    def FileType(self):
+        return self._FileType
+
+    @FileType.setter
+    def FileType(self, FileType):
+        self._FileType = FileType
+
+    @property
+    def IsPublic(self):
+        return self._IsPublic
+
+    @IsPublic.setter
+    def IsPublic(self, IsPublic):
+        self._IsPublic = IsPublic
+
 
     def _deserialize(self, params):
         self._BotBizId = params.get("BotBizId")
+        self._FileType = params.get("FileType")
+        self._IsPublic = params.get("IsPublic")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -4169,26 +4230,29 @@
         :type FilePath: str
         :param _Type: 存储类型
         :type Type: str
         :param _CorpUin: 主号
         :type CorpUin: str
         :param _ImagePath: 图片存储目录
         :type ImagePath: str
+        :param _UploadPath: 上传存储目录
+        :type UploadPath: str
         :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Credentials = None
         self._ExpiredTime = None
         self._StartTime = None
         self._Bucket = None
         self._Region = None
         self._FilePath = None
         self._Type = None
         self._CorpUin = None
         self._ImagePath = None
+        self._UploadPath = None
         self._RequestId = None
 
     @property
     def Credentials(self):
         return self._Credentials
 
     @Credentials.setter
@@ -4256,14 +4320,22 @@
         return self._ImagePath
 
     @ImagePath.setter
     def ImagePath(self, ImagePath):
         self._ImagePath = ImagePath
 
     @property
+    def UploadPath(self):
+        return self._UploadPath
+
+    @UploadPath.setter
+    def UploadPath(self, UploadPath):
+        self._UploadPath = UploadPath
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -4276,14 +4348,15 @@
         self._StartTime = params.get("StartTime")
         self._Bucket = params.get("Bucket")
         self._Region = params.get("Region")
         self._FilePath = params.get("FilePath")
         self._Type = params.get("Type")
         self._CorpUin = params.get("CorpUin")
         self._ImagePath = params.get("ImagePath")
+        self._UploadPath = params.get("UploadPath")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeUnsatisfiedReplyContextRequest(AbstractModel):
     """DescribeUnsatisfiedReplyContext请求参数结构体
 
     """
@@ -5329,20 +5402,23 @@
         :type Count: int
         :param _SessionId: 会话sessionid
         :type SessionId: str
         :param _LastRecordId: 最后一条记录ID
         :type LastRecordId: str
         :param _BotAppKey: 机器人AppKey
         :type BotAppKey: str
+        :param _Scene: 场景, 体验: 1; 正式: 2
+        :type Scene: int
         """
         self._Type = None
         self._Count = None
         self._SessionId = None
         self._LastRecordId = None
         self._BotAppKey = None
+        self._Scene = None
 
     @property
     def Type(self):
         return self._Type
 
     @Type.setter
     def Type(self, Type):
@@ -5376,21 +5452,30 @@
     def BotAppKey(self):
         return self._BotAppKey
 
     @BotAppKey.setter
     def BotAppKey(self, BotAppKey):
         self._BotAppKey = BotAppKey
 
+    @property
+    def Scene(self):
+        return self._Scene
+
+    @Scene.setter
+    def Scene(self, Scene):
+        self._Scene = Scene
+
 
     def _deserialize(self, params):
         self._Type = params.get("Type")
         self._Count = params.get("Count")
         self._SessionId = params.get("SessionId")
         self._LastRecordId = params.get("LastRecordId")
         self._BotAppKey = params.get("BotAppKey")
+        self._Scene = params.get("Scene")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5402,29 +5487,41 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Records: 会话记录
         :type Records: list of MsgRecord
+        :param _SessionDisassociatedTimestamp: session 清除关联上下文时间, 单位 ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionDisassociatedTimestamp: str
         :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Records = None
+        self._SessionDisassociatedTimestamp = None
         self._RequestId = None
 
     @property
     def Records(self):
         return self._Records
 
     @Records.setter
     def Records(self, Records):
         self._Records = Records
 
     @property
+    def SessionDisassociatedTimestamp(self):
+        return self._SessionDisassociatedTimestamp
+
+    @SessionDisassociatedTimestamp.setter
+    def SessionDisassociatedTimestamp(self, SessionDisassociatedTimestamp):
+        self._SessionDisassociatedTimestamp = SessionDisassociatedTimestamp
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -5432,14 +5529,15 @@
     def _deserialize(self, params):
         if params.get("Records") is not None:
             self._Records = []
             for item in params.get("Records"):
                 obj = MsgRecord()
                 obj._deserialize(item)
                 self._Records.append(obj)
+        self._SessionDisassociatedTimestamp = params.get("SessionDisassociatedTimestamp")
         self._RequestId = params.get("RequestId")
 
 
 class GetTaskStatusRequest(AbstractModel):
     """GetTaskStatus请求参数结构体
 
     """
@@ -6170,18 +6268,30 @@
         :type Method: int
         :param _UseGeneralKnowledge: 通用模型回复
 注意：此字段可能返回 null，表示取不到有效值。
         :type UseGeneralKnowledge: bool
         :param _BareAnswer: 未知回复语，300字符以内
 注意：此字段可能返回 null，表示取不到有效值。
         :type BareAnswer: str
+        :param _ShowQuestionClarify: 是否展示问题澄清开关
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ShowQuestionClarify: bool
+        :param _UseQuestionClarify: 是否打开问题澄清
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UseQuestionClarify: bool
+        :param _QuestionClarifyKeywords: 问题澄清关键词列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QuestionClarifyKeywords: list of str
         """
         self._Method = None
         self._UseGeneralKnowledge = None
         self._BareAnswer = None
+        self._ShowQuestionClarify = None
+        self._UseQuestionClarify = None
+        self._QuestionClarifyKeywords = None
 
     @property
     def Method(self):
         return self._Method
 
     @Method.setter
     def Method(self, Method):
@@ -6199,19 +6309,46 @@
     def BareAnswer(self):
         return self._BareAnswer
 
     @BareAnswer.setter
     def BareAnswer(self, BareAnswer):
         self._BareAnswer = BareAnswer
 
+    @property
+    def ShowQuestionClarify(self):
+        return self._ShowQuestionClarify
+
+    @ShowQuestionClarify.setter
+    def ShowQuestionClarify(self, ShowQuestionClarify):
+        self._ShowQuestionClarify = ShowQuestionClarify
+
+    @property
+    def UseQuestionClarify(self):
+        return self._UseQuestionClarify
+
+    @UseQuestionClarify.setter
+    def UseQuestionClarify(self, UseQuestionClarify):
+        self._UseQuestionClarify = UseQuestionClarify
+
+    @property
+    def QuestionClarifyKeywords(self):
+        return self._QuestionClarifyKeywords
+
+    @QuestionClarifyKeywords.setter
+    def QuestionClarifyKeywords(self, QuestionClarifyKeywords):
+        self._QuestionClarifyKeywords = QuestionClarifyKeywords
+
 
     def _deserialize(self, params):
         self._Method = params.get("Method")
         self._UseGeneralKnowledge = params.get("UseGeneralKnowledge")
         self._BareAnswer = params.get("BareAnswer")
+        self._ShowQuestionClarify = params.get("ShowQuestionClarify")
+        self._UseQuestionClarify = params.get("UseQuestionClarify")
+        self._QuestionClarifyKeywords = params.get("QuestionClarifyKeywords")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -10415,14 +10552,19 @@
         :type Type: int
         :param _References: 引用来源
         :type References: list of MsgRecordReference
         :param _Reasons: 评价原因
         :type Reasons: list of str
         :param _IsLlmGenerated: 是否大模型
         :type IsLlmGenerated: bool
+        :param _ImageUrls: 图片链接，可公有读
+        :type ImageUrls: list of str
+        :param _TokenStat: 当次 token 统计信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TokenStat: :class:`tencentcloud.lke.v20231130.models.TokenStat`
         """
         self._Content = None
         self._RecordId = None
         self._RelatedRecordId = None
         self._IsFromSelf = None
         self._FromName = None
         self._FromAvatar = None
@@ -10430,14 +10572,16 @@
         self._HasRead = None
         self._Score = None
         self._CanRating = None
         self._Type = None
         self._References = None
         self._Reasons = None
         self._IsLlmGenerated = None
+        self._ImageUrls = None
+        self._TokenStat = None
 
     @property
     def Content(self):
         return self._Content
 
     @Content.setter
     def Content(self, Content):
@@ -10543,14 +10687,30 @@
     def IsLlmGenerated(self):
         return self._IsLlmGenerated
 
     @IsLlmGenerated.setter
     def IsLlmGenerated(self, IsLlmGenerated):
         self._IsLlmGenerated = IsLlmGenerated
 
+    @property
+    def ImageUrls(self):
+        return self._ImageUrls
+
+    @ImageUrls.setter
+    def ImageUrls(self, ImageUrls):
+        self._ImageUrls = ImageUrls
+
+    @property
+    def TokenStat(self):
+        return self._TokenStat
+
+    @TokenStat.setter
+    def TokenStat(self, TokenStat):
+        self._TokenStat = TokenStat
+
 
     def _deserialize(self, params):
         self._Content = params.get("Content")
         self._RecordId = params.get("RecordId")
         self._RelatedRecordId = params.get("RelatedRecordId")
         self._IsFromSelf = params.get("IsFromSelf")
         self._FromName = params.get("FromName")
@@ -10564,14 +10724,18 @@
             self._References = []
             for item in params.get("References"):
                 obj = MsgRecordReference()
                 obj._deserialize(item)
                 self._References.append(obj)
         self._Reasons = params.get("Reasons")
         self._IsLlmGenerated = params.get("IsLlmGenerated")
+        self._ImageUrls = params.get("ImageUrls")
+        if params.get("TokenStat") is not None:
+            self._TokenStat = TokenStat()
+            self._TokenStat._deserialize(params.get("TokenStat"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -10728,14 +10892,209 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ParseDocRequest(AbstractModel):
+    """ParseDoc请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: 文件名称(需要包括文件后缀, 最大长度1024字节)
+        :type Name: str
+        :param _Url: 文件下载链接 (支持的文件类型: docx, txt, markdown, pdf)
+        :type Url: str
+        :param _TaskId: 任务ID, 用于幂等去重, 业务自行定义(最大长度64字节)
+        :type TaskId: str
+        :param _Policy: 切分策略
+        :type Policy: str
+        :param _Operate: 默认值: parse
+        :type Operate: str
+        """
+        self._Name = None
+        self._Url = None
+        self._TaskId = None
+        self._Policy = None
+        self._Operate = None
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Url(self):
+        return self._Url
+
+    @Url.setter
+    def Url(self, Url):
+        self._Url = Url
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def Policy(self):
+        return self._Policy
+
+    @Policy.setter
+    def Policy(self, Policy):
+        self._Policy = Policy
+
+    @property
+    def Operate(self):
+        warnings.warn("parameter `Operate` is deprecated", DeprecationWarning) 
+
+        return self._Operate
+
+    @Operate.setter
+    def Operate(self, Operate):
+        warnings.warn("parameter `Operate` is deprecated", DeprecationWarning) 
+
+        self._Operate = Operate
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        self._Url = params.get("Url")
+        self._TaskId = params.get("TaskId")
+        self._Policy = params.get("Policy")
+        self._Operate = params.get("Operate")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ParseDocResponse(AbstractModel):
+    """ParseDoc返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TaskId = None
+        self._RequestId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        self._RequestId = params.get("RequestId")
+
+
+class Procedure(AbstractModel):
+    """执行过程信息记录
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: 执行过程英语名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param _Title: 中文名, 用于展示
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Title: str
+        :param _Status: 状态常量: 使用中: processing, 成功: success, 失败: failed
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param _Count: 消耗 token 数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Count: int
+        """
+        self._Name = None
+        self._Title = None
+        self._Status = None
+        self._Count = None
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Title(self):
+        return self._Title
+
+    @Title.setter
+    def Title(self, Title):
+        self._Title = Title
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        self._Title = params.get("Title")
+        self._Status = params.get("Status")
+        self._Count = params.get("Count")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class QACate(AbstractModel):
     """获取QA分类分组
 
     """
 
     def __init__(self):
         r"""
@@ -11095,14 +11454,134 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class QueryParseDocResultRequest(AbstractModel):
+    """QueryParseDocResult请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        """
+        self._TaskId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class QueryParseDocResultResponse(AbstractModel):
+    """QueryParseDocResult返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Status: 等待 / 执行中 / 成功 / 失败
+        :type Status: str
+        :param _Name: 解析后的文件内容
+        :type Name: str
+        :param _Url: 文件下载地址
+        :type Url: str
+        :param _Reason: 解析失败原因
+        :type Reason: str
+        :param _Usage: 消耗量，输出页数
+        :type Usage: :class:`tencentcloud.lke.v20231130.models.Usage`
+        :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Status = None
+        self._Name = None
+        self._Url = None
+        self._Reason = None
+        self._Usage = None
+        self._RequestId = None
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Url(self):
+        return self._Url
+
+    @Url.setter
+    def Url(self, Url):
+        self._Url = Url
+
+    @property
+    def Reason(self):
+        return self._Reason
+
+    @Reason.setter
+    def Reason(self, Reason):
+        self._Reason = Reason
+
+    @property
+    def Usage(self):
+        return self._Usage
+
+    @Usage.setter
+    def Usage(self, Usage):
+        self._Usage = Usage
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Status = params.get("Status")
+        self._Name = params.get("Name")
+        self._Url = params.get("Url")
+        self._Reason = params.get("Reason")
+        if params.get("Usage") is not None:
+            self._Usage = Usage()
+            self._Usage._deserialize(params.get("Usage"))
+        self._RequestId = params.get("RequestId")
+
+
 class QueryRewriteRequest(AbstractModel):
     """QueryRewrite请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12053,28 +12532,40 @@
 
     """
 
     def __init__(self):
         r"""
         :param _SessionId: 会话ID
         :type SessionId: str
+        :param _IsOnlyEmptyTheDialog: 是否仅清空会话关联
+        :type IsOnlyEmptyTheDialog: bool
         """
         self._SessionId = None
+        self._IsOnlyEmptyTheDialog = None
 
     @property
     def SessionId(self):
         return self._SessionId
 
     @SessionId.setter
     def SessionId(self, SessionId):
         self._SessionId = SessionId
 
+    @property
+    def IsOnlyEmptyTheDialog(self):
+        return self._IsOnlyEmptyTheDialog
+
+    @IsOnlyEmptyTheDialog.setter
+    def IsOnlyEmptyTheDialog(self, IsOnlyEmptyTheDialog):
+        self._IsOnlyEmptyTheDialog = IsOnlyEmptyTheDialog
+
 
     def _deserialize(self, params):
         self._SessionId = params.get("SessionId")
+        self._IsOnlyEmptyTheDialog = params.get("IsOnlyEmptyTheDialog")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -12687,17 +13178,21 @@
         r"""
         :param _Model: 模型配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type Model: :class:`tencentcloud.lke.v20231130.models.AppModel`
         :param _Output: 知识摘要输出配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.lke.v20231130.models.SummaryOutput`
+        :param _Greeting: 欢迎语，200字符以内
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Greeting: str
         """
         self._Model = None
         self._Output = None
+        self._Greeting = None
 
     @property
     def Model(self):
         return self._Model
 
     @Model.setter
     def Model(self, Model):
@@ -12707,22 +13202,31 @@
     def Output(self):
         return self._Output
 
     @Output.setter
     def Output(self, Output):
         self._Output = Output
 
+    @property
+    def Greeting(self):
+        return self._Greeting
+
+    @Greeting.setter
+    def Greeting(self, Greeting):
+        self._Greeting = Greeting
+
 
     def _deserialize(self, params):
         if params.get("Model") is not None:
             self._Model = AppModel()
             self._Model._deserialize(params.get("Model"))
         if params.get("Output") is not None:
             self._Output = SummaryOutput()
             self._Output._deserialize(params.get("Output"))
+        self._Greeting = params.get("Greeting")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -12816,14 +13320,183 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TokenStat(AbstractModel):
+    """当前执行的 token 统计信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _SessionId: 会话 ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionId: str
+        :param _RequestId: 请求 ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RequestId: str
+        :param _RecordId: 对应哪条会话, 会话 ID, 用于回答的消息存储使用, 可提前生成, 保存消息时使用
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RecordId: str
+        :param _UsedCount: token 已使用数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UsedCount: int
+        :param _FreeCount: 免费 token 数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FreeCount: int
+        :param _OrderCount: 订单总 token 数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OrderCount: int
+        :param _StatusSummary: 当前执行状态汇总, 常量: 使用中: processing, 成功: success, 失败: failed
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StatusSummary: str
+        :param _StatusSummaryTitle: 当前执行状态汇总后中文展示
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StatusSummaryTitle: str
+        :param _Elapsed: 当前请求执行时间, 单位 ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Elapsed: int
+        :param _TokenCount: 当前请求消耗 token 数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TokenCount: int
+        :param _Procedures: 执行过程信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Procedures: list of Procedure
+        """
+        self._SessionId = None
+        self._RequestId = None
+        self._RecordId = None
+        self._UsedCount = None
+        self._FreeCount = None
+        self._OrderCount = None
+        self._StatusSummary = None
+        self._StatusSummaryTitle = None
+        self._Elapsed = None
+        self._TokenCount = None
+        self._Procedures = None
+
+    @property
+    def SessionId(self):
+        return self._SessionId
+
+    @SessionId.setter
+    def SessionId(self, SessionId):
+        self._SessionId = SessionId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+    @property
+    def RecordId(self):
+        return self._RecordId
+
+    @RecordId.setter
+    def RecordId(self, RecordId):
+        self._RecordId = RecordId
+
+    @property
+    def UsedCount(self):
+        return self._UsedCount
+
+    @UsedCount.setter
+    def UsedCount(self, UsedCount):
+        self._UsedCount = UsedCount
+
+    @property
+    def FreeCount(self):
+        return self._FreeCount
+
+    @FreeCount.setter
+    def FreeCount(self, FreeCount):
+        self._FreeCount = FreeCount
+
+    @property
+    def OrderCount(self):
+        return self._OrderCount
+
+    @OrderCount.setter
+    def OrderCount(self, OrderCount):
+        self._OrderCount = OrderCount
+
+    @property
+    def StatusSummary(self):
+        return self._StatusSummary
+
+    @StatusSummary.setter
+    def StatusSummary(self, StatusSummary):
+        self._StatusSummary = StatusSummary
+
+    @property
+    def StatusSummaryTitle(self):
+        return self._StatusSummaryTitle
+
+    @StatusSummaryTitle.setter
+    def StatusSummaryTitle(self, StatusSummaryTitle):
+        self._StatusSummaryTitle = StatusSummaryTitle
+
+    @property
+    def Elapsed(self):
+        return self._Elapsed
+
+    @Elapsed.setter
+    def Elapsed(self, Elapsed):
+        self._Elapsed = Elapsed
+
+    @property
+    def TokenCount(self):
+        return self._TokenCount
+
+    @TokenCount.setter
+    def TokenCount(self, TokenCount):
+        self._TokenCount = TokenCount
+
+    @property
+    def Procedures(self):
+        return self._Procedures
+
+    @Procedures.setter
+    def Procedures(self, Procedures):
+        self._Procedures = Procedures
+
+
+    def _deserialize(self, params):
+        self._SessionId = params.get("SessionId")
+        self._RequestId = params.get("RequestId")
+        self._RecordId = params.get("RecordId")
+        self._UsedCount = params.get("UsedCount")
+        self._FreeCount = params.get("FreeCount")
+        self._OrderCount = params.get("OrderCount")
+        self._StatusSummary = params.get("StatusSummary")
+        self._StatusSummaryTitle = params.get("StatusSummaryTitle")
+        self._Elapsed = params.get("Elapsed")
+        self._TokenCount = params.get("TokenCount")
+        if params.get("Procedures") is not None:
+            self._Procedures = []
+            for item in params.get("Procedures"):
+                obj = Procedure()
+                obj._deserialize(item)
+                self._Procedures.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class UnsatisfiedReply(AbstractModel):
     """不满意回复
 
     """
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1137/tencentcloud/lke/v20231130/lke_client.py` & `tencentcloud-sdk-python-lke-3.0.1138/tencentcloud/lke/v20231130/lke_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1472,14 +1472,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def ParseDoc(self, request):
+        """解析拆分文档。该接口需开通文档解析原子能力后调用。文档解析原子能力内测中，如有需要请联系架构师或 [联系客服](https://cloud.tencent.com/act/event/Online_service)  。
+
+        :param request: Request instance for ParseDoc.
+        :type request: :class:`tencentcloud.lke.v20231130.models.ParseDocRequest`
+        :rtype: :class:`tencentcloud.lke.v20231130.models.ParseDocResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ParseDoc", params, headers=headers)
+            response = json.loads(body)
+            model = models.ParseDocResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def QueryParseDocResult(self, request):
+        """查询文档解析结果。该接口需开通文档解析原子能力后调用。文档解析原子能力内测中，如有需要请联系架构师或[联系客服](https://cloud.tencent.com/act/event/Online_service) 。
+
+        :param request: Request instance for QueryParseDocResult.
+        :type request: :class:`tencentcloud.lke.v20231130.models.QueryParseDocResultRequest`
+        :rtype: :class:`tencentcloud.lke.v20231130.models.QueryParseDocResultResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("QueryParseDocResult", params, headers=headers)
+            response = json.loads(body)
+            model = models.QueryParseDocResultResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def QueryRewrite(self, request):
         """多轮改写
         本接口有单账号调用上限控制，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
 
         :param request: Request instance for QueryRewrite.
         :type request: :class:`tencentcloud.lke.v20231130.models.QueryRewriteRequest`
         :rtype: :class:`tencentcloud.lke.v20231130.models.QueryRewriteResponse`
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1137/setup.py` & `tencentcloud-sdk-python-lke-3.0.1138/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-lke',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1137"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1138"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Lke SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1137/README.rst` & `tencentcloud-sdk-python-lke-3.0.1138/README.rst`

 * *Files identical despite different names*

