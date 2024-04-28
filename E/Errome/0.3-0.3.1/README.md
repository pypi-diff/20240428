# Comparing `tmp/Errome-0.3.tar.gz` & `tmp/Errome-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Errome-0.3.tar", last modified: Sun Apr 14 11:50:28 2024, max compression
+gzip compressed data, was "Errome-0.3.1.tar", last modified: Sun Apr 28 11:16:45 2024, max compression
```

## Comparing `Errome-0.3.tar` & `Errome-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 11:50:28.284399 Errome-0.3/
-drwxrwxrwx   0        0        0        0 2024-04-14 11:50:28.276399 Errome-0.3/Errome/
--rw-rw-rw-   0        0        0     3186 2024-04-14 11:43:27.000000 Errome-0.3/Errome/Errome.py
--rw-rw-rw-   0        0        0        0 2024-04-08 17:11:09.000000 Errome-0.3/Errome/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 11:50:28.282399 Errome-0.3/Errome/templates/
--rw-rw-rw-   0        0        0     1851 2024-04-08 16:46:21.000000 Errome-0.3/Errome/templates/erro.html
--rw-rw-rw-   0        0        0     1451 2024-04-08 16:38:51.000000 Errome-0.3/Errome/templates/ok.html
-drwxrwxrwx   0        0        0        0 2024-04-14 11:50:28.281400 Errome-0.3/Errome.egg-info/
--rw-rw-rw-   0        0        0     2239 2024-04-14 11:50:28.000000 Errome-0.3/Errome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-04-14 11:50:28.000000 Errome-0.3/Errome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 11:50:28.000000 Errome-0.3/Errome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-14 11:50:28.000000 Errome-0.3/Errome.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       47 2024-04-12 11:06:28.000000 Errome-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2239 2024-04-14 11:50:28.283399 Errome-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1975 2024-04-12 12:05:45.000000 Errome-0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 11:50:28.284399 Errome-0.3/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-04-14 11:50:17.000000 Errome-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:16:45.100384 Errome-0.3.1/
+drwxrwxrwx   0        0        0        0 2024-04-28 11:16:45.091383 Errome-0.3.1/Errome/
+-rw-rw-rw-   0        0        0     3730 2024-04-28 11:01:36.000000 Errome-0.3.1/Errome/Errome.py
+-rw-rw-rw-   0        0        0        0 2024-04-08 17:11:09.000000 Errome-0.3.1/Errome/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 11:16:45.098384 Errome-0.3.1/Errome/templates/
+-rw-rw-rw-   0        0        0     1909 2024-04-28 10:51:08.000000 Errome-0.3.1/Errome/templates/erro.html
+-rw-rw-rw-   0        0        0     1512 2024-04-28 10:35:47.000000 Errome-0.3.1/Errome/templates/ok.html
+drwxrwxrwx   0        0        0        0 2024-04-28 11:16:45.097385 Errome-0.3.1/Errome.egg-info/
+-rw-rw-rw-   0        0        0     2433 2024-04-28 11:16:45.000000 Errome-0.3.1/Errome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-04-28 11:16:45.000000 Errome-0.3.1/Errome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 11:16:45.000000 Errome-0.3.1/Errome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 11:16:45.000000 Errome-0.3.1/Errome.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       47 2024-04-12 11:06:28.000000 Errome-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2433 2024-04-28 11:16:45.099383 Errome-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2167 2024-04-28 11:08:51.000000 Errome-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 11:16:45.100384 Errome-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-28 11:16:41.000000 Errome-0.3.1/setup.py
```

### Comparing `Errome-0.3/Errome/Errome.py` & `Errome-0.3.1/Errome/Errome.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import smtplib
+import sys
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 import datetime
 from pkg_resources import resource_filename
 from functools import wraps
 import traceback
 
@@ -10,39 +11,45 @@
 class Errome:
     def __init__(self,sender_email, password,recever):
         self.sender_email = sender_email
         self.sender_name = "程序运行情况"
         self.password = password
         self.recever = recever
         self.start_time = datetime.datetime.now()
+        self.platform = sys.platform
+        self.file_header = 'templates\\' if 'windows' in self.platform else 'templates/'
 
     def set_start(self):
         self.start_time = datetime.datetime.now()
 
-    def send_email(self, statu):
+    def send_email(self, statu, project_name=None):
         
         message = MIMEMultipart("alternative")
         
         message["From"] = f"{self.sender_name}"
         message["To"] = self.recever
         current_time = datetime.datetime.now()
         time_cost = current_time - self.start_time
+        if project_name is None:
+            project_name = f'{self.start_time.strftime("%Y-%m-%d %H:%M:%S")}'
         if statu == "ok":
             message["Subject"] = "运行完成"
-            with open(resource_filename('Errome','templates\ok.html'), 'r', encoding='utf-8') as file:
+            with open(resource_filename('Errome',self.file_header+'ok.html'), 'r', encoding='utf-8') as file:
                 html_content = file.read()
             html_content = html_content.replace(f"NowTime", current_time.strftime("%Y-%m-%d %H:%M:%S"))
             html_content = html_content.replace(f"Timeuse", str(time_cost.seconds)+"秒")
+            html_content = html_content.replace(f"project_name", project_name)
 
             part = MIMEText(html_content, "html")
             message.attach(part)
         else:
             message["Subject"] = "运行错误"
-            with open(resource_filename('Errome','templates\erro.html'), 'r', encoding='utf-8') as file:
+            with open(resource_filename('Errome',self.file_header+'erro.html'), 'r', encoding='utf-8') as file:
                 html_content = file.read()
+            html_content = html_content.replace(f"project_name", project_name)
             html_content = html_content.replace(f"NowTime", current_time.strftime("%Y-%m-%d %H:%M:%S"))
             html_content = html_content.replace(f"Timeuse", str(time_cost.seconds)+"秒")
             html_content = html_content.replace(f"erro_code", statu)
             part = MIMEText(html_content, "html")
             message.attach(part)
 
         try:
@@ -52,29 +59,30 @@
                 print("Email sent")
         except :
             print("Email sent erro")
     def notify(self, func):
         @wraps(func)
         def wrapped(*args, **kwargs):
             self.start_time = datetime.datetime.now()
+            project_name = func.__name__
             try:
                 result = func(*args, **kwargs)
-                self.send_email("ok")
+                self.send_email("ok",project_name=project_name)
                 return result
             except Exception as e:
                 error_message = traceback.format_exc()
-                self.send_email(error_message)
+                self.send_email(error_message,project_name=project_name)
                 raise
         return wrapped
     
 if __name__ == "__main__":
     # 邮件发送者和接收者
-    sender_email = "xxxxxxx@163.com"  # 替换为你的163邮箱地址
-    receiver_email = "xxxxxx@qq.com"  # 接收者的邮箱地址
-    password = "xxxxxxxxxxxx"  # 你的163邮箱密码
+    sender_email = "XXXXXXXXXXX@163.com"  # 替换为你的163邮箱地址
+    receiver_email = "xxxxxxxxx@qq.com"  # 接收者的邮箱地址
+    password = "*********"  # 你的163邮箱密码
     Email = Errome(sender_email=sender_email, recever=receiver_email, password=password)
 
     @Email.notify
     def test_function():
         print("apple")
```

### Comparing `Errome-0.3/Errome/templates/erro.html` & `Errome-0.3.1/Errome/templates/ok.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,52 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta charset="UTF-8">
-    <title>程序错误报告</title>
+    <title>程序运行状态更新</title>
     <style>
         body {
             font-family: Arial, sans-serif;
-            background-color: #fff3f3; /* 浅红色背景强调错误 */
+            background-color: #f0f9ff; /* 浅蓝色背景 */
             color: #333;
             padding: 20px;
             max-width: 600px;
             margin: auto;
         }
         .header {
-            background-color: #ff6b6b; /* 明亮的红色，引起注意 */
+            background-color: #50b3a2; /* 活泼的青色 */
             color: #fff;
             padding: 10px;
             text-align: center;
             border-radius: 5px;
         }
         .content {
             background-color: #ffffff;
             padding: 20px;
             border-radius: 5px;
             margin-top: 20px;
             box-shadow: 0 2px 4px rgba(0,0,0,0.1);
         }
-        .error-detail {
-            background-color: #ffebeb; /* 轻微红色背景 */
-            color: #d9534f; /* 错误信息的颜色 */
-            padding: 10px;
-            margin: 10px 0;
-            border-left: 5px solid #d9534f; /* 红色边框强调错误 */
-            border-radius: 5px;
-        }
         .footer {
             margin-top: 20px;
             text-align: center;
             font-size: 12px;
             color: #777;
         }
     </style>
 </head>
 <body>
     <div class="header">
-        <h1>程序错误报告</h1>
+        <h1>程序运行状态报告</h1>
     </div>
     <div class="content">
-        <p><strong>报错时间：</strong>NowTime</p>
+        <p><strong>程序名称：</strong>project_name</p>
+        <p><strong>报告时间：</strong>NowTime</p>
+        <p><strong>程序运行情况：</strong>运行完成。</p>
         <p><strong>运行耗时：</strong>Timeuse</p>
-        <div class="error-detail">
-            <p><strong>报错信息：</strong>erro_code</p>
-            <p><strong>ChatGPT的解析:</strong>gpt_analysis</p>
-        </div>
+        <!-- 根据需要自定义程序状态 -->
     </div>
     <div class="footer">
         <p>这是一封自动生成的邮件，请勿回复。</p>
     </div>
-
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-************ ?程?序?错?误?报?告 ************
-?报?错?时?间?：NowTime
+************ ?程?序?运?行?状?态?报?告 ************
+?程?序?名?称?：project_name
+?报?告?时?间?：NowTime
+?程?序?运?行?情?况?：运行完成。
 ?运?行?耗?时?：Timeuse
-?报?错?信?息?：erro_code
-CChhaattGGPPTT?的?解?析::gpt_analysis
 这是一封自动生成的邮件，请勿回复。
```

### Comparing `Errome-0.3/Errome.egg-info/PKG-INFO` & `Errome-0.3.1/Errome.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Errome
-Version: 0.3
+Version: 0.3.1
 Summary: A program error or completion email notification tool.
 Home-page: https://github.com/Becomingw/Errome.git
 Author: BecomingW
 Author-email: Becomingw@qq.com
 Description-Content-Type: text/markdown
 
 # Errome
@@ -15,36 +15,48 @@
 
 - 监控函数的执行时间
 - 在函数成功执行后发送运行成功的邮件通知
 - 捕获函数运行时的异常，并发送包含错误信息的邮件通知
 
 ## 示例：
 
-![图](fig.png)
+<img src="示例.jpg" alt="图" width=120 />
 
 ## 安装
 
-通过克隆 GitHub 仓库的方式安装 Errome：
+1.通过克隆 GitHub 仓库的方式安装 Errome：
 
 ```bash
 git clone https://github.com/Becomingw/Errome.git
 cd Errome
 pip install .
 ```
+2.通过pip安装：
+```bash
+pip install Errome
+```
+
+## 使用
+
+在 Python 文件中导入 Errome 库：
+
+```python
+from Errome.Errome import Errome
+```
 
 ## 快速开始
 
 首先，确保你有一个可以发送邮件的 SMTP 服务器。目前仅支持smtp.163.com(网易邮箱)。
 
 创建一个 Errome 实例：
 
 ```python
 from Errome.Errome import Errome
 #### 初始化邮件发送器
-email_sender = Errome(sender_email="your_email@example.com",
+email_sender = Errome(sender_email="your_email@163.com",
                     password="your_password",
                     receiver="receiver_email@example.com")
 ```
 
 使用 @email_sender.notify 装饰器来监控你的函数：
 
 ```python
```

### Comparing `Errome-0.3/PKG-INFO` & `Errome-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Errome
-Version: 0.3
+Version: 0.3.1
 Summary: A program error or completion email notification tool.
 Home-page: https://github.com/Becomingw/Errome.git
 Author: BecomingW
 Author-email: Becomingw@qq.com
 Description-Content-Type: text/markdown
 
 # Errome
@@ -15,36 +15,48 @@
 
 - 监控函数的执行时间
 - 在函数成功执行后发送运行成功的邮件通知
 - 捕获函数运行时的异常，并发送包含错误信息的邮件通知
 
 ## 示例：
 
-![图](fig.png)
+<img src="示例.jpg" alt="图" width=120 />
 
 ## 安装
 
-通过克隆 GitHub 仓库的方式安装 Errome：
+1.通过克隆 GitHub 仓库的方式安装 Errome：
 
 ```bash
 git clone https://github.com/Becomingw/Errome.git
 cd Errome
 pip install .
 ```
+2.通过pip安装：
+```bash
+pip install Errome
+```
+
+## 使用
+
+在 Python 文件中导入 Errome 库：
+
+```python
+from Errome.Errome import Errome
+```
 
 ## 快速开始
 
 首先，确保你有一个可以发送邮件的 SMTP 服务器。目前仅支持smtp.163.com(网易邮箱)。
 
 创建一个 Errome 实例：
 
 ```python
 from Errome.Errome import Errome
 #### 初始化邮件发送器
-email_sender = Errome(sender_email="your_email@example.com",
+email_sender = Errome(sender_email="your_email@163.com",
                     password="your_password",
                     receiver="receiver_email@example.com")
 ```
 
 使用 @email_sender.notify 装饰器来监控你的函数：
 
 ```python
```

### Comparing `Errome-0.3/README.md` & `Errome-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,36 +6,48 @@
 
 - 监控函数的执行时间
 - 在函数成功执行后发送运行成功的邮件通知
 - 捕获函数运行时的异常，并发送包含错误信息的邮件通知
 
 ## 示例：
 
-![图](fig.png)
+<img src="示例.jpg" alt="图" width=120 />
 
 ## 安装
 
-通过克隆 GitHub 仓库的方式安装 Errome：
+1.通过克隆 GitHub 仓库的方式安装 Errome：
 
 ```bash
 git clone https://github.com/Becomingw/Errome.git
 cd Errome
 pip install .
 ```
+2.通过pip安装：
+```bash
+pip install Errome
+```
+
+## 使用
+
+在 Python 文件中导入 Errome 库：
+
+```python
+from Errome.Errome import Errome
+```
 
 ## 快速开始
 
 首先，确保你有一个可以发送邮件的 SMTP 服务器。目前仅支持smtp.163.com(网易邮箱)。
 
 创建一个 Errome 实例：
 
 ```python
 from Errome.Errome import Errome
 #### 初始化邮件发送器
-email_sender = Errome(sender_email="your_email@example.com",
+email_sender = Errome(sender_email="your_email@163.com",
                     password="your_password",
                     receiver="receiver_email@example.com")
 ```
 
 使用 @email_sender.notify 装饰器来监控你的函数：
 
 ```python
```

### Comparing `Errome-0.3/setup.py` & `Errome-0.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 setup(
     name='Errome',
-    version='0.3',
+    version='0.3.1',
     packages=find_packages(),
     description='A program error or completion email notification tool.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='BecomingW',
     author_email='Becomingw@qq.com',
     url='https://github.com/Becomingw/Errome.git',
```

