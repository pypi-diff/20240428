# Comparing `tmp/limoon-0.0.7.tar.gz` & `tmp/limoon-0.0.8.tar.gz`

## Comparing `limoon-0.0.7.tar` & `limoon-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 limoon-0.0.7/DOCUMENTATION.md
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 limoon-0.0.7/README.md
--rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 limoon-0.0.7/limoon-logo.png
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 limoon-0.0.7/.github/workflows/doc.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 limoon-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 limoon-0.0.7/.github/workflows/test.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/constant.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/core.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/exception.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/model.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 limoon-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 limoon-0.0.7/tests/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 limoon-0.0.7/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 limoon-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 limoon-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 limoon-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6441 2020-02-02 00:00:00.000000 limoon-0.0.8/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 limoon-0.0.8/README.md
+-rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 limoon-0.0.8/limoon-logo.png
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 limoon-0.0.8/.github/workflows/doc.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 limoon-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 limoon-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 limoon-0.0.8/src/limoon/__init__.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 limoon-0.0.8/src/limoon/constant.py
+-rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 limoon-0.0.8/src/limoon/core.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 limoon-0.0.8/src/limoon/exception.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 limoon-0.0.8/src/limoon/model.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 limoon-0.0.8/src/limoon/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 limoon-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 limoon-0.0.8/tests/test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 limoon-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 limoon-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 limoon-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 limoon-0.0.8/PKG-INFO
```

### Comparing `limoon-0.0.7/DOCUMENTATION.md` & `limoon-0.0.8/DOCUMENTATION.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 * [limoon](#limoon)
 * [limoon.core](#limoon.core)
   * [get\_topic](#limoon.core.get_topic)
   * [get\_entry](#limoon.core.get_entry)
   * [get\_author](#limoon.core.get_author)
   * [get\_author\_rank](#limoon.core.get_author_rank)
+  * [get\_author\_badges](#limoon.core.get_author_badges)
   * [get\_author\_topic](#limoon.core.get_author_topic)
   * [get\_agenda](#limoon.core.get_agenda)
   * [get\_debe](#limoon.core.get_debe)
 * [limoon.utils](#limoon.utils)
 * [limoon.constant](#limoon.constant)
 * [limoon.model](#limoon.model)
-  * [Rank](#limoon.model.Rank)
   * [Entry](#limoon.model.Entry)
   * [Topic](#limoon.model.Topic)
+  * [Rank](#limoon.model.Rank)
+  * [Badge](#limoon.model.Badge)
   * [Author](#limoon.model.Author)
 * [limoon.exception](#limoon.exception)
   * [TopicNotFound](#limoon.exception.TopicNotFound)
   * [EntryNotFound](#limoon.exception.EntryNotFound)
   * [AuthorNotFound](#limoon.exception.AuthorNotFound)
   * [PageNotFound](#limoon.exception.PageNotFound)
 
@@ -106,14 +108,33 @@
 - `nickname` _str_ - Unique author nickname.
   
 
 **Returns**:
 
 - `model.Rank` _class_ - Rank data class.
 
+<a id="limoon.core.get_author_badges"></a>
+
+#### get\_author\_badges
+
+```python
+def get_author_badges(nickname: Nickname) -> Iterator[model.Badge]
+```
+
+This function get Ekşi Sözlük author badges.
+
+**Arguments**:
+
+- `nickname` _str_ - Unique author nickname.
+  
+
+**Returns**:
+
+- `Iterator[model.Badge]` - Badge data classes.
+
 <a id="limoon.core.get_author_topic"></a>
 
 #### get\_author\_topic
 
 ```python
 def get_author_topic(nickname: Nickname, max_entry: int = None) -> model.Topic
 ```
@@ -178,30 +199,14 @@
 
 # limoon.constant
 
 <a id="limoon.model"></a>
 
 # limoon.model
 
-<a id="limoon.model.Rank"></a>
-
-## Rank Objects
-
-```python
-@dataclass
-class Rank()
-```
-
-Rank data class.
-
-**Arguments**:
-
-- `name` _str_ - Custom rank name.
-- `karma` _int_ - Rank karma number.
-
 <a id="limoon.model.Entry"></a>
 
 ## Entry Objects
 
 ```python
 @dataclass
 class Entry()
@@ -235,14 +240,47 @@
 - `id` _int_ - Unique topic identity.
 - `title` _str_ - Topic title.
 - `path` _str_ - Unique topic path.
 - `entrys` _class_ - Entrys written for topic.
 - `page_count` _int|None_ - Topic total page count.
 - `url` _str_ - Topic HTTP link.
 
+<a id="limoon.model.Rank"></a>
+
+## Rank Objects
+
+```python
+@dataclass
+class Rank()
+```
+
+Rank data class.
+
+**Arguments**:
+
+- `name` _str_ - Custom rank name.
+- `karma` _int_ - Rank karma number.
+
+<a id="limoon.model.Badge"></a>
+
+## Badge Objects
+
+```python
+@dataclass
+class Badge()
+```
+
+Badge data class.
+
+**Arguments**:
+
+  name (str):
+  description (str):
+  icon_url (str):
+
 <a id="limoon.model.Author"></a>
 
 ## Author Objects
 
 ```python
 @dataclass
 class Author()
@@ -255,14 +293,15 @@
 - `nickname` _str_ - Unique author nickname.
 - `biography` _str|None_ - Author biography (with HTML tags).
 - `total_entry` _int_ - Author total entry count.
 - `follower_count` _int_ - Author total follower count.
 - `following_count` _int_ - Author total following count.
 - `avatar_url` _str_ - Author avatar HTTP link.
 - `rank` _class_ - Author rank.
+- `badges` _class_ - Author badges.
 - `url` _str_ - Author HTTP link.
 
 <a id="limoon.exception"></a>
 
 # limoon.exception
 
 <a id="limoon.exception.TopicNotFound"></a>
```

### Comparing `limoon-0.0.7/README.md` & `limoon-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 # "programcılıgın 8. harikası"
 dir(entry)
 # [..., 'author_nickname', 'content', 'created', 'edited', 'favorite_count', 'id', 'url']
 
 author = limoon.get_author("ssg")
 # Author(ssg)
 dir(author)
-# [..., 'avatar_url', 'biography', 'follower_count', 'following_count', 'nickname', 'rank', 'total_entry', 'url']
+# [..., 'avatar_url', 'badges', 'biography', 'follower_count', 'following_count', 'nickname', 'rank', 'total_entry', 'url']
 ```
 
 ## Documentation
 
-Documentation is [here](DOCUMENTATION.md)!
+Documentation is [here](DOCUMENTATION.md). This page is auto generated. Don't edit!
 
 ## License
 
 `limoon` is distributed under the terms of the [MIT](LICENSE.txt) license. Also the logo was made by @beucismis.
```

### Comparing `limoon-0.0.7/limoon-logo.png` & `limoon-0.0.8/limoon-logo.png`

 * *Files identical despite different names*

### Comparing `limoon-0.0.7/.github/workflows/doc.yml` & `limoon-0.0.8/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.7/.github/workflows/publish.yml` & `limoon-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.7/.github/workflows/test.yml` & `limoon-0.0.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.7/src/limoon/core.py` & `limoon-0.0.8/src/limoon/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -123,14 +123,35 @@
     """
 
     author = get_author(nickname)
 
     return model.Rank(name=author.rank.name, karma=author.rank.karma)
 
 
+def get_author_badges(nickname: Nickname) -> Iterator[model.Badge]:
+    """This function get Ekşi Sözlük author badges.
+
+    Arguments:
+    nickname (str): Unique author nickname.
+
+    Returns:
+    Iterator[model.Badge]: Badge data classes.
+    """
+
+    r = request(constant.AUTHOT_BADGES_TOPIC.format(nickname))
+
+    for badge in r.html.find("li.badge-item-otheruser"):
+        if badge.attrs["data-owned"] != "False":
+            yield model.Badge(
+                badge.find("p", first=True).text,  # name
+                badge.find("a", first=True).attrs["data-title"],  # description
+                badge.find("img", first=True).attrs["src"],  # icon_url
+            )
+
+
 def get_author_topic(nickname: Nickname, max_entry: int = None) -> model.Topic:
     """This function get Ekşi Sözlük author topic.
 
     Arguments:
     nickname (str): Unique author nickname.
     max_entry (int=None): Maximum number of entrys get from per page.
```

### Comparing `limoon-0.0.7/src/limoon/model.py` & `limoon-0.0.8/src/limoon/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 import re
 from dataclasses import dataclass, field
 from typing import Callable, Iterator, TypeVar, Union
 
-from limoon import constant
+from limoon import constant, core
 
 # Typings
 URL = TypeError("URL", Callable, str)
 
 
 @dataclass
-class Rank:
-    """Rank data class.
-
-    Arguments:
-    name (str): Custom rank name.
-    karma (int): Rank karma number.
-    """
-
-    name: str
-    karma: int
-
-    def __repr__(self):
-        return "Rank()"
-
-
-@dataclass
 class Entry:
     """Entry data class.
 
     Arguments:
     id (int): Unique entry identity.
     author_nickname (str): Author who created entry.
     content (str): Entry content (with HTML tags).
@@ -86,42 +70,79 @@
         return f"Topic({self.id})"
 
     def __post_init__(self):
         self.url = constant.BASE_URL + constant.TOPIC_ROUTE.format(self.path)
 
 
 @dataclass
+class Rank:
+    """Rank data class.
+
+    Arguments:
+    name (str): Custom rank name.
+    karma (int): Rank karma number.
+    """
+
+    name: str
+    karma: int
+
+    def __repr__(self):
+        return "Rank()"
+
+
+@dataclass
+class Badge:
+    """Badge data class.
+
+    Arguments:
+    name (str):
+    description (str):
+    icon_url (str):
+    """
+
+    name: str
+    description: str
+    icon_url: URL
+
+    def __repr__(self):
+        return f"Badge({self.name})"
+
+
+@dataclass
 class Author:
     """Author data class.
 
     Arguments:
     nickname (str): Unique author nickname.
     biography (str|None): Author biography (with HTML tags).
     total_entry (int): Author total entry count.
     follower_count (int): Author total follower count.
     following_count (int): Author total following count.
     avatar_url (str): Author avatar HTTP link.
     rank (class): Author rank.
+    badges (class): Author badges.
     url (str): Author HTTP link.
     """
 
     nickname: str
     biography: Union[str, None]
     total_entry: int
     follower_count: int
     following_count: int
     avatar_url: URL
     rank: Union[Rank, None] = field(init=True)
+    badges: Iterator[Badge] = field(init=False)
     url: URL = field(init=False)
 
     def __repr__(self):
         return f"Author({self.nickname})"
 
     def __post_init__(self):
         self.rank = self._parse_rank(self.rank)
+        self.badges = core.get_author_badges(self.nickname)
         self.url = constant.BASE_URL + constant.AUTHOR_ROUTE.format(self.nickname)
 
     def _parse_rank(self, stuff: Union[str, None]) -> Union[Rank, None]:
         if isinstance(stuff, type(None)):
             return None
         result = re.match(r"(\D+) \((\d+)\)", stuff.text)
         return Rank(result.group(1), int(result.group(2)))
```

### Comparing `limoon-0.0.7/src/limoon/utils.py` & `limoon-0.0.8/src/limoon/utils.py`

 * *Files identical despite different names*

### Comparing `limoon-0.0.7/tests/test.py` & `limoon-0.0.8/tests/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,27 +45,33 @@
         assert type(author) is limoon.Author
         assert author.nickname == "ssg"
         assert type(author.biography) is str
         assert author.total_entry > 1
         assert author.follower_count > 1
         assert author.following_count > 1
         assert "https://img.ekstat.com" in author.avatar_url
-        assert type(author.rank) is limoon.Rank
-        assert type(author.rank.name) is str
-        assert type(author.rank.karma) is int
         assert author.url == "https://eksisozluk.com/biri/ssg"
 
     def test_get_author_rank(self):
         author_rank = limoon.get_author_rank("ssg")
 
         assert type(author_rank) is limoon.Rank
         assert type(author_rank.name) is str
         assert type(author_rank.karma) is int
         assert author_rank.karma > 1
 
+    def test_get_author_badges(self):
+        author_badges = list(limoon.get_author_badges("ssg"))
+
+        assert type(author_badges) is list
+        assert type(author_badges[0]) is limoon.Badge
+        assert type(author_badges[0].name) is str
+        assert type(author_badges[0].description) is str
+        assert type(author_badges[0].icon_url) is str
+
     def test_get_author_topic(self):
         author_topic = limoon.get_author_topic("ssg")
 
         assert type(author_topic) is limoon.Topic
         assert author_topic.id == 31795
         assert author_topic.title == "ssg"
         assert author_topic.path == "ssg--31795"
```

### Comparing `limoon-0.0.7/.gitignore` & `limoon-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `limoon-0.0.7/LICENSE.txt` & `limoon-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `limoon-0.0.7/pyproject.toml` & `limoon-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.7/PKG-INFO` & `limoon-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: limoon
-Version: 0.0.7
+Version: 0.0.8
 Summary: Web scraper base Pythonic API for Ekşi Sözlük
 Project-URL: Source, https://github.com/beucismis/limoon
 Project-URL: Issues, https://github.com/beucismis/limoon/issues
 Project-URL: Documentation, https://github.com/beucismis/limoon/DOCUMENTATION.md
 Author-email: beucismis <beucismis@tutamail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -58,17 +58,17 @@
 # "programcılıgın 8. harikası"
 dir(entry)
 # [..., 'author_nickname', 'content', 'created', 'edited', 'favorite_count', 'id', 'url']
 
 author = limoon.get_author("ssg")
 # Author(ssg)
 dir(author)
-# [..., 'avatar_url', 'biography', 'follower_count', 'following_count', 'nickname', 'rank', 'total_entry', 'url']
+# [..., 'avatar_url', 'badges', 'biography', 'follower_count', 'following_count', 'nickname', 'rank', 'total_entry', 'url']
 ```
 
 ## Documentation
 
-Documentation is [here](DOCUMENTATION.md)!
+Documentation is [here](DOCUMENTATION.md). This page is auto generated. Don't edit!
 
 ## License
 
 `limoon` is distributed under the terms of the [MIT](LICENSE.txt) license. Also the logo was made by @beucismis.
```

