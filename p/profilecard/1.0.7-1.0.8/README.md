# Comparing `tmp/profilecard-1.0.7.tar.gz` & `tmp/profilecard-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profilecard-1.0.7.tar", last modified: Wed Apr 24 10:24:35 2024, max compression
+gzip compressed data, was "profilecard-1.0.8.tar", last modified: Sun Apr 28 13:35:42 2024, max compression
```

## Comparing `profilecard-1.0.7.tar` & `profilecard-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:24:35.753131 profilecard-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 10:24:14.000000 profilecard-1.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-24 10:24:35.753131 profilecard-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-24 10:24:14.000000 profilecard-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:24:35.749132 profilecard-1.0.7/profilecard/
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:24:35.749132 profilecard-1.0.7/profilecard/simple/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/simple/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/simple/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/simple/valmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:24:35.753131 profilecard-1.0.7/profilecard/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/styles/style1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/styles/style2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-24 10:24:14.000000 profilecard-1.0.7/profilecard/styles/style3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:24:35.753131 profilecard-1.0.7/profilecard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-24 10:24:35.000000 profilecard-1.0.7/profilecard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 10:24:35.000000 profilecard-1.0.7/profilecard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:24:35.000000 profilecard-1.0.7/profilecard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 10:24:35.000000 profilecard-1.0.7/profilecard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 10:24:35.000000 profilecard-1.0.7/profilecard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:24:35.753131 profilecard-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 10:24:14.000000 profilecard-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:42.609784 profilecard-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-28 13:35:29.000000 profilecard-1.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-28 13:35:42.609784 profilecard-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-28 13:35:29.000000 profilecard-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:42.609784 profilecard-1.0.8/profilecard/
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:42.609784 profilecard-1.0.8/profilecard/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/simple/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/simple/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/simple/valmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:42.609784 profilecard-1.0.8/profilecard/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/styles/style1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/styles/style2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-28 13:35:29.000000 profilecard-1.0.8/profilecard/styles/style3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:35:42.609784 profilecard-1.0.8/profilecard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-28 13:35:42.000000 profilecard-1.0.8/profilecard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-28 13:35:42.000000 profilecard-1.0.8/profilecard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:35:42.000000 profilecard-1.0.8/profilecard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 13:35:42.000000 profilecard-1.0.8/profilecard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 13:35:42.000000 profilecard-1.0.8/profilecard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:35:42.609784 profilecard-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-28 13:35:29.000000 profilecard-1.0.8/setup.py
```

### Comparing `profilecard-1.0.7/LICENSE.md` & `profilecard-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.7/PKG-INFO` & `profilecard-1.0.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,121 @@
 Metadata-Version: 2.1
 Name: profilecard
-Version: 1.0.7
+Version: 1.0.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests
 
+[[English](README.md)|[中文](README_zh.md)]
+
 # Personal Profile Card Module
 
-This module provides a simple way to create and manage personal profile cards for various platforms like GitHub, YouTube, and Reddit. It includes customization options such as style, type, theme, and more. You can also use it for advertising your channel on your project.
+This module provides a simple way to create a personal profile cards , it can copy user data from various platforms like GitHub, YouTube, and Reddit. It includes customization options such as style, type, theme, and more. You can also use it for advertising your channel on your project.
 
 ## Features
 
 - Customize the style of the profile card with predefined styles.
 - Set the type of profile card to platforms like GitHub, YouTube, Reddit, or custom.
 - Customize the theme to be either light or dark.
 - Add badges, background pictures, profile pictures, and more.
 
 ![Example image](example.png)
+
+```python
+from profilecard import Pf
+
+profile = Pf()
+
+profile.set_style(style="2")
+
+profile.set_type(type="custom")
+
+profile.set_name("James &#128511;") #emoji -> &#128511
+
+profile.set_pic("https://i.pinimg.com/564x/40/86/36/40863654e0c78c453f86539d12390405.jpg")
+
+profile.set_theme(theme="light")
+
+profile.set_site_title(title="Introduce")
+
+profile.set_background_pic("https://www.hdwallpapers.in/download/white_wallpaper_5_4k_hd_white-1920x1080.jpg")
+
+profile.add_badge(icon="discord", text="My discord", color="blue", bg_color="gray")
+profile.add_badge(icon="github", text="My GitHub", color="white", link="https://github.com/jyst06", bg_color="gray")
+profile.add_badge(icon="youtube", text="My Youtube", color="red", bg_color="gray")
+profile.add_info("Some information<br>here &#128511;") #emoji -> &#128511
+
+profile.pack()
+profile.show()
+profile.reset()
+```
+
 ![Example image](example2.png)
+
+```python
+from profilecard import Pf
+
+profile = Pf()
+
+profile.set_type(type="github", link="https://github.com/jyst06")
+
+profile.set_background_pic("https://wallpapercave.com/wp/wp13902559.png")
+
+profile.add_badge(icon="discord", text="My discord", color="blue", style="flat")
+profile.add_badge(icon="github", text="My GitHub", color="white", link="https://github.com/jyst06", style="flat")
+profile.add_badge(icon="youtube", text="My Youtube", color="red", style="flat")
+
+profile.add_info("Some information<br>here &#128511;")
+
+profile.pack()
+profile.show()
+profile.reset()
+```
+
 ![Example image](example3.png)
 
+```python
+from profilecard import Pf
+
+root = Pf(first=False)
+root.set_style("2")
+root.set_type(type="custom")
+root.add_id("jyst06")
+root.set_name("James")
+root.set_pic("https://i.pinimg.com/564x/59/dc/8d/59dc8d6797b835e746dd99a2df7dcedd.jpg")
+
+root.add_badge(icon="github", text="GitHub", link="https://github.com/jyst06", bg_color="white", color="black")
+
+root.set_theme("light")
+root.add_info("Hello")
+root.set_card_title("About Me")
+root.set_site_title("my site")
+root.add_contect("Nope :(")
+root.set_background_pic(r"https://images6.alphacoders.com/133/1330710.png")
+
+root.pack()
+root.show()
+root.reset()
+```
+
 ## Pip Installation
 
 To install this module, use the following pip command:
 
 ```bash
 pip install profilecard
 ```
 
 ## Basic Usage
 
 Here's how you can use the `Pf` class from this module:
 
 ```python
-from profilecard import *
+from profilecard import Pf
 
 # Create a profile card instance (default is False)
 profile = Pf(first=False)
 
 # Change page style (default is style 1)
 profile.set_style("2")  # Three styles available: 1, 2, 3
 
@@ -74,14 +151,17 @@
 profile.set_card_title("Handsome guy")
 
 # Pack all
 profile.pack()
 
 # Display site
 profile.show()
+
+# Make sure the config reset to default
+profile.reset()
 ```
 
 ## API Reference
 
 The following functions are available in the `Pf` class:
 
 ### `help(profilecard)` get the usage in python IDE
@@ -94,15 +174,15 @@
   - `style`: A string representing the style ('1', '2', '3'). Default is '1'.
 
 ---
 
 ### `set_type(type: str, link: str)`
 Sets the type of profile card and optionally the profile page link.
 - **Parameters**:
-  - `type`: A string representing the type ('github', 'youtube', 'reddit', 'custom').
+  - `type`: A string representing the type ('github', 'youtube', 'reddit', 'leetcode', 'custom').
   - `link`: A string representing the link to the profile page.
 
 ---
 
 ### `set_theme(theme: str)`
 Sets the theme of the card.
 - **Parameters**:
@@ -122,14 +202,18 @@
 
 ---
 
 ### Additional methods include `set_pic`, `set_name`, `set_background_pic`, `add_info`, `add_contect`, `set_site_title`, `set_card_title`, `pack`, `show`, and `reset`.
 
 ---
 
+### Other methods in init file `reset_profilecard_config()`, `show_without_repacking()`
+
+---
+
 ## Contributing
 
 Contributions are welcome! Please fork the repository and open a pull request with your changes.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `profilecard-1.0.7/profilecard/__init__.py` & `profilecard-1.0.8/profilecard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 from .simple import Pack, show
 from .simple import set_val, get_val, reset_config as rc
 
 
 class Pf:
     """
@@ -48,15 +48,15 @@
         This function is use to set the type of profile card
         type : support -> ('github' , 'youtube' , 'reddit' , 'custom')
         link : ('LINK OF PROFILE PAGE')
         """
         if type == 'custom':
             set_val(type='Parameters', name="type", val=type)
 
-        elif type in ['github', 'youtube', 'reddit']:
+        elif type in ['github', 'youtube', 'reddit', 'leetcode']:
             set_val(type='Parameters', name="type", val=type)
             set_val(type='Parameters', name="profile_page_link", val=link)
 
         else:
             raise ValueError(f'ProfileCard Error : Invalid type "{type}"')
 
         self.type = type
@@ -224,8 +224,8 @@
     rc()
 
 
 def show_without_repacking(*, first : bool = False):
     """
     This function is use to show the profile card without repacking
     """
-    show(first=first)
+    show(first=first)
```

### Comparing `profilecard-1.0.7/profilecard/simple/pack.py` & `profilecard-1.0.8/profilecard/simple/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 
         elif type == 'youtube':
             self.youtube_parse(link)
 
         elif type == 'reddit':
             self.reddit_parse(link)
 
+        elif type == 'leetcode':
+            self.leetcode_parse(link)
+
         elif type == 'custom':
             self.custom_parse(profile_pic_link, profile_name, profile_id)
 
         else:
             raise ValueError(f'Type:{type} is not supported')
 
 
@@ -93,14 +96,33 @@
     def reddit_parse(self, link) -> None:
         soup = BeautifulSoup(requests.get(link).text, 'html.parser')
         self.profile_pic = soup.find("img").get("src")
         self.profile_name = soup.find("h1").text.strip()
         self.profile_id = soup.find("p").text.strip()
 
 
+    def leetcode_parse(self, link) -> None:
+        temp = link.split('/')
+        if temp[-1]:
+            account = temp[-1]
+        else:
+            account = temp[-2]
+
+        original_string = '{ matchedUser(username: "account") { profile { realName userAvatar } } }'
+        query = original_string.replace('account', account)
+        data = {
+            "query": query,
+        }
+        res = requests.post(url='https://leetcode.com/graphql/', json=data)
+        profile = res.json()["data"]['matchedUser']['profile']
+        self.profile_pic = profile['userAvatar']
+        self.profile_name = profile['realName']
+        self.profile_id = None
+
+
     def custom_parse(self, profile_pic_link, profile_name, profile_id) -> None:
         self.profile_pic = profile_pic_link
         self.profile_name = profile_name
         if profile_id:
             self.profile_id = profile_id
 
         else:
```

### Comparing `profilecard-1.0.7/profilecard/simple/valmanager.py` & `profilecard-1.0.8/profilecard/simple/valmanager.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.7/profilecard/styles/style1.py` & `profilecard-1.0.8/profilecard/styles/style1.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.7/profilecard/styles/style2.py` & `profilecard-1.0.8/profilecard/styles/style2.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.7/profilecard/styles/style3.py` & `profilecard-1.0.8/profilecard/styles/style3.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.7/profilecard.egg-info/PKG-INFO` & `profilecard-1.0.8/profilecard.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,121 @@
 Metadata-Version: 2.1
 Name: profilecard
-Version: 1.0.7
+Version: 1.0.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests
 
+[[English](README.md)|[中文](README_zh.md)]
+
 # Personal Profile Card Module
 
-This module provides a simple way to create and manage personal profile cards for various platforms like GitHub, YouTube, and Reddit. It includes customization options such as style, type, theme, and more. You can also use it for advertising your channel on your project.
+This module provides a simple way to create a personal profile cards , it can copy user data from various platforms like GitHub, YouTube, and Reddit. It includes customization options such as style, type, theme, and more. You can also use it for advertising your channel on your project.
 
 ## Features
 
 - Customize the style of the profile card with predefined styles.
 - Set the type of profile card to platforms like GitHub, YouTube, Reddit, or custom.
 - Customize the theme to be either light or dark.
 - Add badges, background pictures, profile pictures, and more.
 
 ![Example image](example.png)
+
+```python
+from profilecard import Pf
+
+profile = Pf()
+
+profile.set_style(style="2")
+
+profile.set_type(type="custom")
+
+profile.set_name("James &#128511;") #emoji -> &#128511
+
+profile.set_pic("https://i.pinimg.com/564x/40/86/36/40863654e0c78c453f86539d12390405.jpg")
+
+profile.set_theme(theme="light")
+
+profile.set_site_title(title="Introduce")
+
+profile.set_background_pic("https://www.hdwallpapers.in/download/white_wallpaper_5_4k_hd_white-1920x1080.jpg")
+
+profile.add_badge(icon="discord", text="My discord", color="blue", bg_color="gray")
+profile.add_badge(icon="github", text="My GitHub", color="white", link="https://github.com/jyst06", bg_color="gray")
+profile.add_badge(icon="youtube", text="My Youtube", color="red", bg_color="gray")
+profile.add_info("Some information<br>here &#128511;") #emoji -> &#128511
+
+profile.pack()
+profile.show()
+profile.reset()
+```
+
 ![Example image](example2.png)
+
+```python
+from profilecard import Pf
+
+profile = Pf()
+
+profile.set_type(type="github", link="https://github.com/jyst06")
+
+profile.set_background_pic("https://wallpapercave.com/wp/wp13902559.png")
+
+profile.add_badge(icon="discord", text="My discord", color="blue", style="flat")
+profile.add_badge(icon="github", text="My GitHub", color="white", link="https://github.com/jyst06", style="flat")
+profile.add_badge(icon="youtube", text="My Youtube", color="red", style="flat")
+
+profile.add_info("Some information<br>here &#128511;")
+
+profile.pack()
+profile.show()
+profile.reset()
+```
+
 ![Example image](example3.png)
 
+```python
+from profilecard import Pf
+
+root = Pf(first=False)
+root.set_style("2")
+root.set_type(type="custom")
+root.add_id("jyst06")
+root.set_name("James")
+root.set_pic("https://i.pinimg.com/564x/59/dc/8d/59dc8d6797b835e746dd99a2df7dcedd.jpg")
+
+root.add_badge(icon="github", text="GitHub", link="https://github.com/jyst06", bg_color="white", color="black")
+
+root.set_theme("light")
+root.add_info("Hello")
+root.set_card_title("About Me")
+root.set_site_title("my site")
+root.add_contect("Nope :(")
+root.set_background_pic(r"https://images6.alphacoders.com/133/1330710.png")
+
+root.pack()
+root.show()
+root.reset()
+```
+
 ## Pip Installation
 
 To install this module, use the following pip command:
 
 ```bash
 pip install profilecard
 ```
 
 ## Basic Usage
 
 Here's how you can use the `Pf` class from this module:
 
 ```python
-from profilecard import *
+from profilecard import Pf
 
 # Create a profile card instance (default is False)
 profile = Pf(first=False)
 
 # Change page style (default is style 1)
 profile.set_style("2")  # Three styles available: 1, 2, 3
 
@@ -74,14 +151,17 @@
 profile.set_card_title("Handsome guy")
 
 # Pack all
 profile.pack()
 
 # Display site
 profile.show()
+
+# Make sure the config reset to default
+profile.reset()
 ```
 
 ## API Reference
 
 The following functions are available in the `Pf` class:
 
 ### `help(profilecard)` get the usage in python IDE
@@ -94,15 +174,15 @@
   - `style`: A string representing the style ('1', '2', '3'). Default is '1'.
 
 ---
 
 ### `set_type(type: str, link: str)`
 Sets the type of profile card and optionally the profile page link.
 - **Parameters**:
-  - `type`: A string representing the type ('github', 'youtube', 'reddit', 'custom').
+  - `type`: A string representing the type ('github', 'youtube', 'reddit', 'leetcode', 'custom').
   - `link`: A string representing the link to the profile page.
 
 ---
 
 ### `set_theme(theme: str)`
 Sets the theme of the card.
 - **Parameters**:
@@ -122,14 +202,18 @@
 
 ---
 
 ### Additional methods include `set_pic`, `set_name`, `set_background_pic`, `add_info`, `add_contect`, `set_site_title`, `set_card_title`, `pack`, `show`, and `reset`.
 
 ---
 
+### Other methods in init file `reset_profilecard_config()`, `show_without_repacking()`
+
+---
+
 ## Contributing
 
 Contributions are welcome! Please fork the repository and open a pull request with your changes.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

