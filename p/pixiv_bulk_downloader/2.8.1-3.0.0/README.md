# Comparing `tmp/pixiv_bulk_downloader-2.8.1.tar.gz` & `tmp/pixiv_bulk_downloader-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixiv_bulk_downloader-2.8.1.tar", last modified: Tue Jan 31 18:32:06 2023, max compression
+gzip compressed data, was "pixiv_bulk_downloader-3.0.0.tar", max compression
```

## Comparing `pixiv_bulk_downloader-2.8.1.tar` & `pixiv_bulk_downloader-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:32:06.026748 pixiv_bulk_downloader-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-31 18:32:06.026748 pixiv_bulk_downloader-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:32:06.026748 pixiv_bulk_downloader-2.8.1/pbd/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/pbd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/pbd/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/pbd/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/pbd/followings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/pbd/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/pbd/pixiv_types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/pbd/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:32:06.026748 pixiv_bulk_downloader-2.8.1/pixiv_bulk_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-31 18:32:05.000000 pixiv_bulk_downloader-2.8.1/pixiv_bulk_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-31 18:32:05.000000 pixiv_bulk_downloader-2.8.1/pixiv_bulk_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 18:32:05.000000 pixiv_bulk_downloader-2.8.1/pixiv_bulk_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 18:32:05.000000 pixiv_bulk_downloader-2.8.1/pixiv_bulk_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-31 18:32:05.000000 pixiv_bulk_downloader-2.8.1/pixiv_bulk_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-31 18:32:05.000000 pixiv_bulk_downloader-2.8.1/pixiv_bulk_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-31 18:32:06.026748 pixiv_bulk_downloader-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 18:31:53.000000 pixiv_bulk_downloader-2.8.1/setup.py
+-rw-r--r--   0        0        0     1075 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2357 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/README.md
+-rw-r--r--   0        0        0      546 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/__init__.py
+-rw-r--r--   0        0        0     3341 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/base.py
+-rw-r--r--   0        0        0     1910 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/bookmarks.py
+-rw-r--r--   0        0        0     3167 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/followings.py
+-rw-r--r--   0        0        0     2126 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/main.py
+-rw-r--r--   0        0        0      573 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/pixiv_types.py
+-rw-r--r--   0        0        0        0 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/py.typed
+-rw-r--r--   0        0        0     2008 2024-04-28 21:12:43.467297 pixiv_bulk_downloader-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3381 1970-01-01 00:00:00.000000 pixiv_bulk_downloader-3.0.0/PKG-INFO
```

### Comparing `pixiv_bulk_downloader-2.8.1/LICENSE` & `pixiv_bulk_downloader-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixiv_bulk_downloader-2.8.1/PKG-INFO` & `pixiv_bulk_downloader-3.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: pixiv_bulk_downloader
-Version: 2.8.1
-Summary: Pixiv Bulk Downloader for bookmarks and works of followed authors
+Version: 3.0.0
+Summary: Pixiv Bulk Downloader for bookmarks and works of following authors
 Home-page: https://github.com/eggplants/pixiv-bulk-downloader
+License: MIT
+Keywords: downloader,cli,commandline-tool,pixivpy
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
-License: MIT
+Requires-Python: >=3.9,<4.0
+Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Dist: gppt (>=4.1.0,<5.0.0)
+Requires-Dist: pixivpy3 (>=3.7.5,<4.0.0)
+Requires-Dist: pwinput (>=1.0.3,<2.0.0)
+Project-URL: Repository, https://github.com/eggplants/pixiv-bulk-downloader
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
 
 # pixiv-bulk-downloader
 
 [![PyPI version](
   <https://badge.fury.io/py/pixiv-bulk-downloader.svg>
   )](
   <https://badge.fury.io/py/pixiv-bulk-downloader>
@@ -54,17 +61,19 @@
 [?]: Download all bookmarked? (1909 works) (n/y):
 ```
 
 ### From PyPI
 
 Note: _In advance, please setup google-chrome-stable + selenium + webdriver_
 
+<!-- markdownlint-disable MD033 -->
 <details>
 
 <summary>Ubuntu</summary>
+<!-- markdownlint-enable MD033 -->
 
 ```bash
 # google-chrome-stable
 wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
 sudo apt install ./google-chrome-stable_current_amd64.deb -y
 google-chrome --version  # check
 
@@ -74,15 +83,17 @@
 
 # webdriver
 pip install chromedriver-binary-auto
 # add this to rc or env: export PATH="$PATH:`chromedriver-path`"
 chromedriver -v  # check
 ```
 
+<!-- markdownlint-disable MD033 -->
 </details>
+<!-- markdownlint-enable MD033 -->
 
 ```shellsession
 # Python>=3.9
 $ pip install pixiv-bulk-downloader
 
 $ pbd
 [+]: ID is mail address, userid, account name.
@@ -99,7 +110,8 @@
 ![image](https://user-images.githubusercontent.com/42153744/132086124-7a7634f9-7fe0-47b9-98b5-840716c4db34.png)
 
 ![image](https://user-images.githubusercontent.com/42153744/132086141-b0b82493-ed7d-44a6-80c8-dea7c47297a1.png)
 
 ## License
 
 MIT
+
```

### Comparing `pixiv_bulk_downloader-2.8.1/README.md` & `pixiv_bulk_downloader-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -36,17 +36,19 @@
 [?]: Download all bookmarked? (1909 works) (n/y):
 ```
 
 ### From PyPI
 
 Note: _In advance, please setup google-chrome-stable + selenium + webdriver_
 
+<!-- markdownlint-disable MD033 -->
 <details>
 
 <summary>Ubuntu</summary>
+<!-- markdownlint-enable MD033 -->
 
 ```bash
 # google-chrome-stable
 wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
 sudo apt install ./google-chrome-stable_current_amd64.deb -y
 google-chrome --version  # check
 
@@ -56,15 +58,17 @@
 
 # webdriver
 pip install chromedriver-binary-auto
 # add this to rc or env: export PATH="$PATH:`chromedriver-path`"
 chromedriver -v  # check
 ```
 
+<!-- markdownlint-disable MD033 -->
 </details>
+<!-- markdownlint-enable MD033 -->
 
 ```shellsession
 # Python>=3.9
 $ pip install pixiv-bulk-downloader
 
 $ pbd
 [+]: ID is mail address, userid, account name.
```

### Comparing `pixiv_bulk_downloader-2.8.1/pbd/__init__.py` & `pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from .base import PixivBaseDownloader
 from .bookmarks import PixivBookmarksDownloader
 from .followings import PixivFollowingsDownloader
 from .pixiv_types import (
     IllustInfo,
     LoginCred,
-    LoginFailed,
+    LoginFailedError,
     NextBookmarksRequest,
     NextFollowingsRequest,
     UserInfo,
 )
 
-__version__ = "2.8.1"
+__version__ = "3.0.0"
 __all__ = [
     "PixivBaseDownloader",
     "PixivBookmarksDownloader",
     "PixivFollowingsDownloader",
     "IllustInfo",
     "LoginCred",
-    "LoginFailed",
+    "LoginFailedError",
     "NextBookmarksRequest",
     "NextFollowingsRequest",
     "UserInfo",
 ]
```

### Comparing `pixiv_bulk_downloader-2.8.1/pbd/base.py` & `pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 from __future__ import annotations
 
-import os
 import random
 import time
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from gppt import LoginInfo
-from pixivpy3 import AppPixivAPI
-from pixivpy3.utils import JsonDict
+if TYPE_CHECKING:
+    from pathlib import Path
 
-from .pixiv_types import IllustInfo
+    from gppt import LoginInfo
+    from pixivpy3 import AppPixivAPI
+    from pixivpy3.utils import JsonDict
+
+    from .pixiv_types import IllustInfo
 
 
 class PixivBaseDownloader:
-    def __init__(self, aapi: AppPixivAPI, login_info: LoginInfo, save_dir: str):
+    def __init__(
+        self, aapi: AppPixivAPI, login_info: LoginInfo, save_dir: Path
+    ) -> None:
         self.aapi = aapi
         self.login_info = login_info
         self.save_dir = save_dir
 
     @staticmethod
     def rand_sleep(base: float = 0.1, rand: float = 2.5) -> None:
-        time.sleep(base + rand * random.random())
+        time.sleep(base + rand * random.random())  # noqa: S311
 
     @staticmethod
     def ext_links(illust: JsonDict) -> list[str] | str:
         links: list[str] = [page.image_urls.original for page in illust.meta_pages]
         link: str = illust.meta_single_page.get(
-            "original_image_url", illust.image_urls.large
+            "original_image_url",
+            illust.image_urls.large,
         )
 
         return links if links != [] else link
 
     def retrieve_works(self, target_id: int) -> list[IllustInfo]:
         urls: list[IllustInfo] = []
         next_qs: dict[str, Any] | None = {}
@@ -39,49 +44,52 @@
                 res_json = self.aapi.user_illusts(target_id, type="illust")
             else:
                 res_json = self.aapi.user_illusts(**next_qs)
             if "error" in res_json and "invalid_grant" in res_json["error"]["message"]:
                 self.aapi.auth()
                 continue
             for illust in res_json["illusts"]:
-                urls.append(
+                urls.append(  # noqa: PERF401
                     {
                         "id": illust.id,
                         "title": illust.title,
                         "link": self.ext_links(illust),
-                    }
+                    },
                 )
             next_qs = self.aapi.parse_qs(res_json["next_url"])
             self.rand_sleep(1.5)
-        else:
-            return urls
+        return urls
 
-    def download(self, data: list[IllustInfo], save_path: str) -> None:
-        os.makedirs(save_path, exist_ok=True)
+    def download(self, data: list[IllustInfo], save_path: Path) -> None:
+        save_path.mkdir(parents=True, exist_ok=True)
         data_len = len(data)
         d_width = len(str(data_len))
         for idx, image_data in enumerate(data):
             title, id_ = image_data["title"].replace("/", "／"), image_data["id"]
             links = image_data["link"]
             print(
                 f"\033[K[%0{d_width}d/%0{d_width}d]: %s (id: %d)"
-                % (idx + 1, data_len, title, id_)
+                % (idx + 1, data_len, title, id_),
             )
             self.__download(links, title, id_, save_path)
 
             print("\033[K\033[A\033[K", end="", flush=True)
 
     def __download(
-        self, links: str | list[str], title: str, id_: int, save_path: str
+        self,
+        links: str | list[str],
+        title: str,
+        id_: int,
+        save_path: Path,
     ) -> None:
-        if type(links) is list:
+        if isinstance(links, list):
             for link in links:
                 basename_: str = link.split("/")[-1]
                 fname = "{}_{}_{}".format(id_, title, basename_.split("_")[-1])
                 print("\033[K" + fname, end="\r")
-                self.aapi.download(link, path=save_path, fname=fname)
-        elif type(links) is str:
+                self.aapi.download(link, path=str(save_path), fname=fname)
+        elif isinstance(links, str):
             link = links
             basename_ = link.split("/")[-1]
             fname = "{}_{}_{}".format(id_, title, basename_.split("_")[-1])
             print("\033[K" + fname, end="\r")
-            self.aapi.download(link, path=save_path, fname=fname)
+            self.aapi.download(link, path=str(save_path), fname=fname)
```

### Comparing `pixiv_bulk_downloader-2.8.1/pbd/bookmarks.py` & `pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/bookmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
-import os
-from typing import Any
-
-from pixivpy3.utils import JsonDict
+from pathlib import Path
+from typing import TYPE_CHECKING, Any
 
 from .base import PixivBaseDownloader
-from .pixiv_types import IllustInfo
+
+if TYPE_CHECKING:
+    from pixivpy3.utils import JsonDict
+
+    from .pixiv_types import IllustInfo
 
 
 class PixivBookmarksDownloader(PixivBaseDownloader):
     def get_all_bookmarked_works(self) -> None:
         print("[+]: Fetching information of bookmarked works...")
         bookmarked_data = self.retrieve_bookmarks()
         print("\n[+]: Downloading bookmarked works...")
-        self.download(bookmarked_data, os.path.join(self.save_dir, "bookmarks"))
+        self.download(bookmarked_data, Path(self.save_dir) / "bookmarks")
 
     def retrieve_bookmarks(self) -> list[IllustInfo]:
         urls: list[IllustInfo] = []
         next_qs: dict[str, Any] | None = {}
         target_id = self.login_info["response"]["user"]["id"]
         total = self.aapi.user_detail(self.aapi.user_id)["profile"][
             "total_illust_bookmarks_public"
@@ -38,14 +40,13 @@
                     flush=True,
                 )
                 urls.append(
                     {
                         "id": illust.id,
                         "title": illust.title,
                         "link": self.ext_links(illust),
-                    }
+                    },
                 )
             next_qs = self.aapi.parse_qs(res_json["next_url"])
             urls_len = len(urls)
             self.rand_sleep(0.5)
-        else:
-            return urls
+        return urls
```

### Comparing `pixiv_bulk_downloader-2.8.1/pbd/followings.py` & `pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/followings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 from __future__ import annotations
 
-import os
-from typing import Any
-
-from pixivpy3.utils import JsonDict
+from pathlib import Path
+from typing import TYPE_CHECKING, Any
 
 from .base import PixivBaseDownloader
-from .pixiv_types import UserInfo
+
+if TYPE_CHECKING:
+    from pixivpy3.utils import JsonDict
+
+    from .pixiv_types import UserInfo
 
 
 class PixivFollowingsDownloader(PixivBaseDownloader):
     def retrieve_following(self) -> list[UserInfo]:
         users: list[UserInfo] = []
         next_qs: dict[str, Any] | None = {}
         my_info = self.aapi.user_detail(self.aapi.user_id)
         total = my_info["profile"]["total_follow_users"]
         while next_qs is not None:
             if "user_id" not in next_qs:
                 res_json: JsonDict = self.aapi.user_following(
-                    self.login_info["response"]["user"]["id"]
+                    self.login_info["response"]["user"]["id"],
                 )
             else:
                 res_json = self.aapi.user_following(**next_qs)
 
             next_qs = self.aapi.parse_qs(res_json.next_url)
             now_retrieved_len = len(users)
             users.extend(
                 self.extract_artist_info(
-                    res_json.user_previews, total, now_retrieved_len
-                )
+                    res_json.user_previews,
+                    total,
+                    now_retrieved_len,
+                ),
             )
             self.rand_sleep(1.5)
 
         return users
 
     def extract_artist_info(
-        self, user_previews: Any, following_total: int, retrieved: int
+        self,
+        user_previews: Any,  # noqa: ANN401
+        following_total: int,
+        retrieved: int,
     ) -> list[Any]:
         users: list[Any] = []
         d_width = len(str(following_total))
         if user_previews is None:
             print("\n[!]Warning: artist info seems to be empty.")
             return users
         for idx, user in enumerate(user_previews):
@@ -52,32 +59,33 @@
             )
             users.append(
                 {
                     "id": user_info.id,
                     "name": user_info.name,
                     "account": user_info.account,
                     "illusts": self.retrieve_works(user_info.id),
-                }
+                },
             )
             self.rand_sleep(1.5)
-        else:
-            return users
+        return users
 
     def get_all_following_works(self) -> None:
         print("[+]: Fetching information of works of following artists...")
         following_data = self.retrieve_following()
         print("[+]: Downloading works of following artists...")
         following_len = len(following_data)
         d_width = len(str(following_len))
         for idx, author_data in enumerate(following_data):
             dirname = "{}_{}_{}".format(
-                author_data["id"], author_data["name"], author_data["account"]
+                author_data["id"],
+                author_data["name"],
+                author_data["account"],
             ).replace("/", "／")
             print(
                 f"\033[K[Artist][%0{d_width}d/%0{d_width}d]: %s"
-                % (idx + 1, following_len, dirname)
+                % (idx + 1, following_len, dirname),
             )
             self.download(
                 author_data["illusts"],
-                os.path.join(self.save_dir, "following", dirname),
+                Path(self.save_dir) / "following" / dirname,
             )
             print("\033[K\033[A\033[K", end="", flush=True)
```

### Comparing `pixiv_bulk_downloader-2.8.1/pbd/main.py` & `pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 from __future__ import annotations
 
 import os
 import sys
+from pathlib import Path
+from typing import TYPE_CHECKING
 
-import pwinput  # type: ignore[import]
+import pwinput  # type: ignore[import-untyped]
 from gppt import PixivAuth
-from pixivpy3.aapi import AppPixivAPI
 
 from .bookmarks import PixivBookmarksDownloader
 from .followings import PixivFollowingsDownloader
-from .pixiv_types import LoginFailed
+from .pixiv_types import LoginFailedError
 
-SAVE_DIR = os.getenv("SAVE_DIR", os.path.join(os.path.expanduser("~"), "pbd"))
+if TYPE_CHECKING:
+    from pixivpy3.aapi import AppPixivAPI
+
+SAVE_DIR = Path(os.getenv("SAVE_DIR", Path.home() / "pbd"))
 """client.json
 {
   'pixiv_id' : '<change this>',
   'password' : '<change this>'
 }
 """
 
 
 def interact(
-    aapi: AppPixivAPI, f: PixivFollowingsDownloader, b: PixivBookmarksDownloader
+    aapi: AppPixivAPI,
+    f: PixivFollowingsDownloader,
+    b: PixivBookmarksDownloader,
 ) -> None:
     def getch() -> str:
         c = pwinput.getch()
         print()
         return str(c)
 
     my_info = aapi.user_detail(aapi.user_id)
     total_following_len = my_info["profile"]["total_follow_users"]
     total_bookmark_len = my_info["profile"]["total_illust_bookmarks_public"]
     print(
         "[?]: Download all works of following? "
-        "({} artists) (n/y): ".format(total_following_len),
+        f"({total_following_len} artists) (n/y): ",
         flush=True,
         end="",
     )
     if getch() == "y":
         f.get_all_following_works()
         print("\033[K[+]: Finish!")
     print(
-        "[?]: Download all bookmarked? "
-        "({} works) (n/y): ".format(total_bookmark_len),
+        "[?]: Download all bookmarked? " f"({total_bookmark_len} works) (n/y): ",
         flush=True,
         end="",
     )
     if getch() == "y":
         b.get_all_bookmarked_works()
         print("\033[K[+]: Finish!")
 
@@ -63,16 +68,16 @@
     else:
         interact(aapi, f, b)
 
 
 def main() -> None:
     try:
         _main()
-    except (KeyError, LoginFailed):
-        print("\n[!]: Request limit seem to be exceeded. " "Try again later.")
+    except (KeyError, LoginFailedError):
+        print("\n[!]: Request limit seem to be exceeded. Try again later.")
     except KeyboardInterrupt:
         print("\n[!]: SIGINT")
     finally:
         print("\x1b[?25h", end="")
 
 
 if __name__ == "__main__":
```

### Comparing `pixiv_bulk_downloader-2.8.1/pbd/pixiv_types.py` & `pixiv_bulk_downloader-3.0.0/pixiv_bulk_downloader/pixiv_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import TypedDict
 
 
-class LoginFailed(Exception):
+class LoginFailedError(Exception):
     pass
 
 
 class LoginCred(TypedDict):
     pixiv_id: str
     password: str
```

