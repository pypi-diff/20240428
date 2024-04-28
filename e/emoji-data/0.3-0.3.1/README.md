# Comparing `tmp/emoji_data-0.3.tar.gz` & `tmp/emoji_data-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emoji_data-0.3.tar", last modified: Sat Apr 20 16:44:38 2024, max compression
+gzip compressed data, was "emoji_data-0.3.1.tar", last modified: Sun Apr 28 14:19:31 2024, max compression
```

## Comparing `emoji_data-0.3.tar` & `emoji_data-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.438801 emoji_data-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-20 16:44:32.000000 emoji_data-0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-20 16:44:32.000000 emoji_data-0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-20 16:44:32.000000 emoji_data-0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 16:44:32.000000 emoji_data-0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-20 16:44:38.438801 emoji_data-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-20 16:44:32.000000 emoji_data-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-20 16:44:32.000000 emoji_data-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-20 16:44:32.000000 emoji_data-0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 16:44:38.438801 emoji_data-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.430801 emoji_data-0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.434801 emoji_data-0.3/src/emoji_data/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/character.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.434801 emoji_data-0.3/src/emoji_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   111503 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-data.txt
--rw-r--r--   0 runner    (1001) docker     (127)   191562 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-sequences.txt
--rw-r--r--   0 runner    (1001) docker     (127)   639404 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38358 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-variation-sequences.txt
--rw-r--r--   0 runner    (1001) docker     (127)   251595 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-zwj-sequences.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.434801 emoji_data-0.3/src/emoji_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:19:31.227084 emoji_data-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-28 14:19:25.000000 emoji_data-0.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-28 14:19:25.000000 emoji_data-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-28 14:19:25.000000 emoji_data-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 14:19:25.000000 emoji_data-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-28 14:19:31.227084 emoji_data-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-28 14:19:25.000000 emoji_data-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-28 14:19:25.000000 emoji_data-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-28 14:19:25.000000 emoji_data-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 14:19:31.227084 emoji_data-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:19:31.223084 emoji_data-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:19:31.223084 emoji_data-0.3.1/src/emoji_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 14:19:31.000000 emoji_data-0.3.1/src/emoji_data/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:19:31.227084 emoji_data-0.3.1/src/emoji_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/data/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/data/README
+-rw-r--r--   0 runner    (1001) docker     (127)   111503 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/data/emoji-data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191562 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/data/emoji-sequences.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   639404 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/data/emoji-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38358 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/data/emoji-variation-sequences.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   251595 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/data/emoji-zwj-sequences.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-28 14:19:25.000000 emoji_data-0.3.1/src/emoji_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:19:31.227084 emoji_data-0.3.1/src/emoji_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-28 14:19:31.000000 emoji_data-0.3.1/src/emoji_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-28 14:19:31.000000 emoji_data-0.3.1/src/emoji_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 14:19:31.000000 emoji_data-0.3.1/src/emoji_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-28 14:19:31.000000 emoji_data-0.3.1/src/emoji_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 14:19:31.000000 emoji_data-0.3.1/src/emoji_data.egg-info/top_level.txt
```

### Comparing `emoji_data-0.3/CHANGELOG.md` & `emoji_data-0.3.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # CHANGELOG
 
+## 0.3.1
+
+> 📅 **Date** 2024-4-28
+
+- 🆕 New:
+  - `version` property for `EmojiCharacter` and `EmojiSequence` class, it records in which Emoji version the character or sequence was defined.
+  - `variation` property for `EmojiSequence` class
+
 ## 0.3
 
 > 📅 **Date** 2024-4-21
 
 - 🌞 Highlights:
   - Update to Emoji version 15.1
 - 🆕 New Features:
```

### Comparing `emoji_data-0.3/LICENSE.txt` & `emoji_data-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emoji_data-0.3/PKG-INFO` & `emoji_data-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emoji-data
-Version: 0.3
+Version: 0.3.1
 Summary: A library represents emoji sequences and characters in Unicode® Technical Standard #51 Data Files
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: AGPLv3+
 Project-URL: homepage, https://github.com/tanbro/emoji-data
 Project-URL: repository, https://github.com/tanbro/emoji-data.git
 Keywords: emoji,unicode
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -41,8 +41,8 @@
 
 ```sh
 pip install emoji-data
 ```
 
 ## How to use
 
-See `notebooks/example.ipynb`
+See `docs/notebooks/example.ipynb`
```

### Comparing `emoji_data-0.3/README.md` & `emoji_data-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
 ```sh
 pip install emoji-data
 ```
 
 ## How to use
 
-See `notebooks/example.ipynb`
+See `docs/notebooks/example.ipynb`
```

### Comparing `emoji_data-0.3/pyproject.toml` & `emoji_data-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emoji_data-0.3/src/emoji_data/__init__.py` & `emoji_data-0.3.1/src/emoji_data/__init__.py`

 * *Files identical despite different names*

### Comparing `emoji_data-0.3/src/emoji_data/character.py` & `emoji_data-0.3.1/src/emoji_data/character.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from __future__ import annotations
 
+import re
 import sys
 from enum import Enum
-from typing import Union
+from typing import Iterable, Iterator, MutableSequence, Optional, Sequence, Tuple, Union, final
 
 if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import Self
 else:  # pragma: no cover
     from typing import Self
 
-if sys.version_info < (3, 9):  # pragma: no cover
-    from typing import Iterable, MutableSequence, Sequence, Tuple
-else:  # pragma: no cover
-    from collections.abc import Iterable, Sequence, MutableSequence
-
 from .types import BaseDictContainer
-from .utils import code_point_to_regex, data_file, read_data_file_iterable
+from .utils import code_point_to_regex, emoji_data_lines
 
 __all__ = [
     "EmojiCharProperty",
     "EmojiCharacter",
     "TEXT_PRESENTATION_SELECTOR",
     "EMOJI_PRESENTATION_SELECTOR",
     "EMOJI_KEYCAP",
@@ -59,15 +55,16 @@
 
 
 class EmojiCharProperty(Enum):
     """Emoji Character Properties
 
     character properties are available for emoji characters.
 
-    see: http://www.unicode.org/reports/tr51/#Emoji_Properties
+    See also:
+        http://www.unicode.org/reports/tr51/#Emoji_Properties
     """
 
     EMOJI = "Emoji"
     """for characters that are emoji"""
 
     EPRES = "Emoji_Presentation"
     """ for characters that have emoji presentation by default"""
@@ -89,196 +86,200 @@
     EXTPICT = "Extended_Pictographic"
     """for characters that are used to future-proof segmentation.
 
     The Extended_Pictographic characters contain all the Emoji characters except for some Emoji_Component characters.
     """
 
 
-class MetaClass(BaseDictContainer):
+class MetaClass(BaseDictContainer[int, "EmojiCharacter"]):
     pass
 
 
-class EmojiCharacter(metaclass=MetaClass):
+@final
+class EmojiCharacter(metaclass=MetaClass):  # pyright: ignore[reportGeneralTypeIssues]
     """emoji character — A character that has the Emoji property.
 
     These characters are recommended for use as emoji.
 
-    see: http://www.unicode.org/reports/tr51/#Emoji_Characters
+    See also:
+        http://www.unicode.org/reports/tr51/#Emoji_Characters
     """
 
     def __init__(
         self,
         code_point: int,
-        properties: Union[Iterable[EmojiCharProperty], EmojiCharProperty, None] = None,
-        comments: Union[Iterable[str], str, None] = None,
+        properties: Union[EmojiCharProperty, Iterable[EmojiCharProperty], None] = None,
+        version: Optional[str] = None,
+        description: Optional[str] = None,
     ):
         self._code_point = code_point
         self._string = chr(self._code_point)
         self._regex = code_point_to_regex(code_point)
         #
+        self._properties: MutableSequence[EmojiCharProperty]
         if properties is None:
-            self._properties: MutableSequence[EmojiCharProperty] = []
+            self._properties = []
         elif isinstance(properties, EmojiCharProperty):
             self._properties = [properties]
         elif isinstance(properties, Iterable):
             self._properties = list(properties)
         else:
-            raise TypeError(
-                f"Argument `properties` expects `EmojiCharProperty`, `Iterable[EmojiCharProperty]`, or `None`, but actual {type(properties)}"
-            )
+            raise TypeError(f"{type(properties)}")
         #
-        if comments is None:
-            self._comments: MutableSequence[str] = []
-        elif isinstance(comments, str):
-            self._comments = [comments]
-        elif isinstance(comments, Iterable):
-            self._comments = [s for s in comments if isinstance(s, str)]
-        else:
-            raise TypeError(f"Argument `comments` expects `str`, `Iterable[str]`, or `None`, but actual {type(comments)}")
+        self._version = version or ""
+        self._description = description or ""
 
     def __str__(self):
         return self._string
 
     def __repr__(self):
-        return "<{} code_point={} char={!r}>".format(
-            type(self).__name__,
-            self.code_point_string,
-            self.string,
+        return "<{} code_point={} char={!r} version={!r} description={!r}>".format(
+            type(self).__name__, self.code_point_string, self.string, self.version, self.description
         )
 
+    _comment_split_regex = re.compile(r"\[\d+\]\s*\(.*\)")
+
     _initialed = False
 
     @classmethod
     def initial(cls):
         """Initial the class
 
         Load Emoji Characters and it's properties from package data file into class internal dictionary
         """
         if cls._initialed:
             return
-        with data_file("emoji-data.txt").open(encoding="utf8") as fp:
-            for content, comment in read_data_file_iterable(fp):
-                cps, property_text = (part.strip() for part in content.split(";", 1))
-                cps_parts = cps.split("..", 1)
-                property_ = EmojiCharProperty(property_text)
-                for cp in range(int(cps_parts[0], 16), 1 + int(cps_parts[-1], 16)):
-                    try:
-                        inst: Self = cls[cp]  # type:ignore[annotation-unchecked]
-                    except KeyError:
-                        cls[cp] = cls(cp, property_, comment)
-                    else:
-                        inst._add_property(property_)
-                        inst._add_comment(comment)
-            for cp in TEXT_PRESENTATION_SELECTOR, EMOJI_PRESENTATION_SELECTOR, EMOJI_KEYCAP:
-                if cp not in cls:
-                    cls[cp] = cls(cp)
+        for content, comment in emoji_data_lines("emoji-data.txt"):
+            cps, property_text = (part.strip() for part in content.split(";", 1))
+            cps_parts = cps.split("..", 1)
+            property_ = EmojiCharProperty(property_text)
+            version, description = (s.strip() for s in cls._comment_split_regex.split(comment, maxsplit=1))
+            for cp in range(int(cps_parts[0], 16), 1 + int(cps_parts[-1], 16)):
+                try:
+                    inst = cls[cp]
+                except KeyError:
+                    cls[cp] = cls(cp, property_, version, description)
+                else:
+                    inst._add_property(property_)
+        for cp in (TEXT_PRESENTATION_SELECTOR, EMOJI_PRESENTATION_SELECTOR, EMOJI_KEYCAP):
+            if cp not in cls:
+                cls[cp] = cls(cp, [])
         # OK!
         cls._initialed = True
 
     @classmethod
     def release(cls):
         if not cls._initialed:
             return
         keys = list(cls)
         for k in keys:
             del cls[k]
         cls._initialed = False
 
-    if sys.version_info < (3, 9):  # pragma: no cover
-
-        @classmethod
-        def items(cls) -> Iterable[Tuple[int, Self]]:
-            return ((k, cls[k]) for k in cls)
-
-    else:
-
-        @classmethod
-        def items(cls) -> Iterable[tuple[int, Self]]:
-            """Return an iterator of all code-point -> emoji-character pairs of the class"""
-            return ((k, cls[k]) for k in cls)
+    @classmethod
+    def items(cls) -> Iterator[Tuple[int, Self]]:
+        """Returns an iterator of all code-point -> emoji-character pairs of the class"""
+        return ((k, cls[k]) for k in cls)  # pyright: ignore[reportReturnType]
 
     @classmethod
-    def keys(cls) -> Iterable[int]:
-        """Return an iterator of each emoji-character's key code-point of the class"""
-        return (k for k in cls)
+    def keys(cls) -> Iterator[int]:
+        """Returns an iterator of each emoji-character's key code-point of the class"""
+        yield from cls
 
     @classmethod
-    def values(cls) -> Iterable[Self]:
-        """Return an iterator of all emoji-characters of the class"""
-        return (cls[k] for k in cls)
+    def values(cls) -> Iterator[Self]:
+        """Returns an iterator of all emoji-characters of the class"""
+        return (cls[k] for k in cls)  # pyright: ignore[reportReturnType]
 
     def _add_property(self, val: EmojiCharProperty):
         if val not in self._properties:
             self._properties.append(val)
 
-    def _add_comment(self, val: str):
-        if val not in self._properties:
-            self._comments.append(val)
-
     @property
     def code_point(self) -> int:
         """Unicode integer value of the emoji-characters"""
         return self._code_point
 
     @property
     def code_point_string(self) -> str:
         """Unicode style hex string of the emoji-characters's code-point
 
-        eg: ``25FB``
+        Example:
+            ``"25FB"``
         """
         return f"{self._code_point:04X}"
 
     @property
     def properties(self) -> Sequence[EmojiCharProperty]:
         """Property description text of the emoji-characters"""
         return self._properties
 
     @property
-    def comments(self) -> Sequence[str]:
-        """Comments of the Emoji"""
-        return self._comments
+    def version(self) -> str:
+        """Version of the Emoji.
+
+        Example:
+            ``E0.0``, ``E0.6``, ``E11.0``
+        """
+        return self._description
+
+    @property
+    def description(self) -> str:
+        """Description comment of the Emoji"""
+        return self._description
 
     @property
     def regex(self) -> str:
         """Regular express for the emoji-characters"""
         return self._regex
 
     @property
     def hex(self) -> str:
         """Python style hex string of the emoji-characters's code-pint
 
-        eg: ``0x25fb``
+        Example:
+            ``"0x25fb"``
         """
         return hex(self._code_point)
 
     @property
     def string(self) -> str:
         """Emoji character string"""
         return self._string
 
     @classmethod
     def from_character(cls, c: str) -> Self:
         """Get :class:`EmojiCharacter` instance from a single Emoji Unicode character
 
-        .. note::
-            ``c`` should be a single unicode character.
+        Args:
+            c: Emoji character
 
-        :param c: Emoji character
-        :return: Instance returned from the class's internal dictionary
-        :raise KeyError: When character not found in the class' internal dictionary
+                Note:
+                    ``c`` should be a **single** unicode character, that is: ``len(c) == 1``.
+
+        Returns:
+            Instance returned from the class's internal dictionary
+
+        Raises:
+            KeyError: When character not found in the class' internal dictionary
         """
-        return cls[ord(c)]
+        return cls[ord(c)]  # pyright: ignore[reportReturnType]
 
     @classmethod
     def from_hex(cls, value: Union[int, str]) -> Self:
         """Get an :class:`EmojiCharacter` instance by Emoji Unicode integer value or it's hex string
 
-        :param value: Emoji Unicode, either integer value or hex string
-        :return: Instance returned from the class's internal dictionary
-        :raises KeyError: When code not found in the class' internal dictionary
+        Args:
+            value: Emoji Unicode, either integer value or hex string
+
+        Returns:
+            Instance returned from the class's internal dictionary
+
+        Raises:
+            KeyError: When code not found in the class' internal dictionary
         """
         if isinstance(value, str):
-            return cls[int(value, 16)]
-        return cls[int(value)]
+            return cls[int(value, 16)]  # pyright: ignore[reportReturnType]
+        return cls[int(value)]  # pyright: ignore[reportReturnType]
 
 
 EmojiCharacter.initial()
```

### Comparing `emoji_data-0.3/src/emoji_data/data/emoji-data.txt` & `emoji_data-0.3.1/src/emoji_data/data/emoji-data.txt`

 * *Files identical despite different names*

### Comparing `emoji_data-0.3/src/emoji_data/data/emoji-sequences.txt` & `emoji_data-0.3.1/src/emoji_data/data/emoji-sequences.txt`

 * *Files identical despite different names*

### Comparing `emoji_data-0.3/src/emoji_data/data/emoji-test.txt` & `emoji_data-0.3.1/src/emoji_data/data/emoji-test.txt`

 * *Files identical despite different names*

### Comparing `emoji_data-0.3/src/emoji_data/data/emoji-variation-sequences.txt` & `emoji_data-0.3.1/src/emoji_data/data/emoji-variation-sequences.txt`

 * *Files identical despite different names*

### Comparing `emoji_data-0.3/src/emoji_data/data/emoji-zwj-sequences.txt` & `emoji_data-0.3.1/src/emoji_data/data/emoji-zwj-sequences.txt`

 * *Files identical despite different names*

### Comparing `emoji_data-0.3/src/emoji_data/definitions.py` & `emoji_data-0.3.1/src/emoji_data/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 """Regular expressions for Emoji Definitions
 
 ref: http://www.unicode.org/reports/tr51/#Definitions
 """
 
-import sys
 import re
 from enum import Enum
-from typing import Pattern
-
-if sys.version_info < (3, 9):  # pragma: no cover
-    from typing import Mapping, MutableMapping
-else:  # pragma: no cover
-    from collections.abc import Mapping, MutableMapping
+from typing import Pattern, Mapping, MutableMapping
 
 from .character import (
     EMOJI_KEYCAP,
     EMOJI_PRESENTATION_SELECTOR,
     REGIONAL_INDICATORS,
     TAGS,
     TEXT_PRESENTATION_SELECTOR,
@@ -56,15 +50,15 @@
 
 class QualifiedType(Enum):
     FULLY_QUALIFIED = "fully-qualified"
     MINIMALLY_QUALIFIED = "minimally-qualified"
     UNQUALIFIED = "unqualified"
 
 
-def _make_regex_dict() -> Mapping[str, str]:
+def make_regex_dict() -> Mapping[str, str]:
     d: MutableMapping[str, str] = {}
     d.update(
         {
             "EMOJI_CHARACTER": r"["
             + "".join(m.regex for m in EmojiCharacter.values() if EmojiCharProperty.EMOJI in m.properties)
             + r"]"
         }
@@ -136,29 +130,30 @@
     )
     d.update({"EMOJI_ZWJ_ELEMENT": r"({EMOJI_CHARACTER}|{EMOJI_PRESENTATION_SEQUENCE}|{EMOJI_MODIFIER_SEQUENCE})".format(**d)})
     d.update({"EMOJI_ZWJ_SEQUENCE": r"({EMOJI_ZWJ_ELEMENT}({0}{EMOJI_ZWJ_ELEMENT})+)".format(code_point_to_regex(ZWJ), **d)})
     d.update({"EMOJI_SEQUENCE": r"({EMOJI_CORE_SEQUENCE}|{EMOJI_ZWJ_SEQUENCE}|{EMOJI_TAG_SEQUENCE})".format(**d)})
     return d
 
 
-EMOJI_PATTERNS: Mapping[str, Pattern[str]] = {k: re.compile(v) for k, v in _make_regex_dict().items()}
+EMOJI_PATTERNS: Mapping[str, Pattern[str]] = {k: re.compile(v) for k, v in make_regex_dict().items()}
 
 
 def is_emoji_character(c: str) -> bool:
     """detect emoji character
 
     A character that has the Emoji property.
 
     ::
 
         emoji_character := \\p{Emoji}
 
     - These characters are recommended for use as emoji.
 
-    ref: https://unicode.org/reports/tr51/#Emoji_Characters
+    See also:
+        https://unicode.org/reports/tr51/#Emoji_Characters
     """
     _c = chr(ord(c))
     return EMOJI_PATTERNS["EMOJI_CHARACTER"].fullmatch(_c) is not None
 
 
 def is_default_emoji_presentation_character(c: str) -> bool:
     """detect default emoji presentation character
@@ -167,57 +162,62 @@
 
     ::
 
         default_emoji_presentation_character := \\p{Emoji_Presentation}
 
     - These characters have the Emoji_Presentation property.
 
-    ref: https://unicode.org/reports/tr51/#def_emoji_presentation
+    See also:
+        https://unicode.org/reports/tr51/#def_emoji_presentation
     """
     _c = chr(ord(c))
     return EMOJI_PATTERNS["DEFAULT_EMOJI_PRESENTATION_CHARACTER"].fullmatch(_c) is not None
 
 
 def is_default_text_presentation_character(c: str) -> bool:
     """detect default text presentation character
 
     A character that, by default, should appear with a text presentation, rather than an emoji presentation.
 
-    ref: https://unicode.org/reports/tr51/#def_text_presentation_sequence
+    See also:
+        https://unicode.org/reports/tr51/#def_text_presentation_sequence
     """
     _c = chr(ord(c))
     return EMOJI_PATTERNS["DEFAULT_TEXT_PRESENTATION_CHARACTER"].fullmatch(_c) is not None
 
 
 def is_text_presentation_selector(c: str) -> bool:
     """detect text presentation selector
 
     The character U+FE0E VARIATION SELECTOR-15 (VS15), used to request a text presentation for an emoji character. (Also known as text variation selector in prior versions of this specification.)
 
-    ref: https://unicode.org/reports/tr51/#def_emoji_presentation_selector
+    See also:
+        https://unicode.org/reports/tr51/#def_emoji_presentation_selector
     """
     return EMOJI_PATTERNS["TEXT_PRESENTATION_SELECTOR"].fullmatch(c) is not None
 
 
 def is_text_presentation_sequence(s: str) -> bool:
     """detect text presentation selector
 
     The character U+FE0E VARIATION SELECTOR-15 (VS15), used to request a text presentation for an emoji character. (Also known as text variation selector in prior versions of this specification.)
 
-    ref: https://unicode.org/reports/tr51/#def_text_presentation_sequence
+    See also:
+        https://unicode.org/reports/tr51/#def_text_presentation_sequence
     """
     return EMOJI_PATTERNS["TEXT_PRESENTATION_SEQUENCE"].fullmatch(s) is not None
 
 
 def is_emoji_presentation_selector(c: str) -> bool:
     """detect emoji presentation selector
 
     The character U+FE0F VARIATION SELECTOR-16 (VS16), used to request an emoji presentation for an emoji character. (Also known as emoji variation selector in prior versions of this specification.)
 
-    ref: https://unicode.org/reports/tr51/#def_emoji_presentation_selector
+    See also:
+        https://unicode.org/reports/tr51/#def_emoji_presentation_selector
     """
     return EMOJI_PATTERNS["EMOJI_PRESENTATION_SELECTOR"].fullmatch(c) is not None
 
 
 def is_emoji_presentation_sequence(s: str) -> bool:
     """detect emoji presentation sequence
 
@@ -225,36 +225,39 @@
 
     ::
 
         emoji_presentation_sequence := emoji_character emoji_presentation_selector
 
     - The only valid emoji presentation sequences are those listed in emoji-variation-sequences.txt
 
-    ref: https://unicode.org/reports/tr51/#def_emoji_presentation_sequence
+    See also:
+        https://unicode.org/reports/tr51/#def_emoji_presentation_sequence
     """
     return EMOJI_PATTERNS["EMOJI_PRESENTATION_SEQUENCE"].fullmatch(s) is not None
 
 
 def is_emoji_modifier(c: str) -> bool:
     """detect emoji modifier
 
     A character that can be used to modify the appearance of a preceding emoji in an emoji modifier sequence.
 
-    ref: https://unicode.org/reports/tr51/#def_emoji_modifier
+    See also:
+        https://unicode.org/reports/tr51/#def_emoji_modifier
     """
     _c = chr(ord(c))
     return EMOJI_PATTERNS["EMOJI_MODIFIER"].fullmatch(_c) is not None
 
 
 def is_emoji_modifier_base(c: str) -> bool:
     """Detect emoji modifier base
 
     A character whose appearance can be modified by a subsequent emoji modifier in an emoji modifier sequence.
 
-    ref: https://unicode.org/reports/tr51/#def_emoji_modifier_base
+    See also:
+        https://unicode.org/reports/tr51/#def_emoji_modifier_base
     """
     _c = chr(ord(c))
     return EMOJI_PATTERNS["EMOJI_MODIFIER_BASE"].fullmatch(_c) is not None
 
 
 def is_emoji_modifier_sequence(s: str) -> bool:
     """Detect emoji modifier sequence
@@ -318,25 +321,32 @@
 
 
 def is_emoji_sequence(s: str) -> bool:
     return EMOJI_PATTERNS["EMOJI_SEQUENCE"].fullmatch(s) is not None
 
 
 def is_qualified_emoji_character(s: str, i: int) -> bool:
-    """An emoji character in a string that
+    """check if an emoji character in a string is qualified.
+
+    An emoji character in a string that
 
     - (a) has default emoji presentation or
     - (b) is the first character in an emoji modifier sequence or
     - (c) is not a default emoji presentation character, but is the first character in an emoji presentation sequence.
 
-    :param s: the string where the character in it
-    :param i: index of the character in the string to check if qualified
-    :return: ``True`` or ``False``
+    is qualified.
+
+    Args:
+        s: the string where the character in it
+        i: index of the character in the string to check if qualified
+
+    Returns: :data:`True` if qualified else :data:`False`
 
-    ref: http://www.unicode.org/reports/tr51/#def_qualified_emoji_character
+    See also:
+        http://www.unicode.org/reports/tr51/#def_qualified_emoji_character
     """
     c = s[i]
     if not is_emoji_character(c):
         return False
     if is_default_emoji_presentation_character(c):  # default emoji presentation
         return True
     if EMOJI_PATTERNS["EMOJI_MODIFIER_SEQUENCE"].match(s[i:]):  # first character in an emoji modifier sequence
@@ -355,15 +365,16 @@
         - (b) is the first character in an emoji modifier sequence or
         - (c) is not a default emoji presentation character, but is the first character in an emoji presentation sequence.
 
     - fully-qualified emoji — A qualified emoji character, or an emoji sequence in which each emoji character is qualified.
     - minimally-qualified emoji — An emoji sequence in which the first character is qualified but the sequence is not fully qualified.
     - unqualified emoji — An emoji that is neither fully-qualified nor minimally qualified.
 
-    :param s: string to detect
+    Args:
+        s: string to detect
     """
     if not s:
         raise ValueError("Argument `s` should not be empty or null")
     if is_qualified_emoji_character(s, 0):
         n = len(s)
         if n == 1:
             return QualifiedType.FULLY_QUALIFIED
```

### Comparing `emoji_data-0.3/src/emoji_data/sequence.py` & `emoji_data-0.3.1/src/emoji_data/sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,79 @@
 from __future__ import annotations
 
 import re
 import sys
-from typing import Pattern, Union
+from typing import ClassVar, Generator, Iterable, Iterator, Optional, Pattern, Sequence, Tuple, Union, final
 
 if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import Self
 else:  # pragma: no cover
     from typing import Self
 
-if sys.version_info < (3, 9):  # pragma: no cover
-    from typing import Iterable, Sequence, Tuple, Generator
-else:  # pragma: no cover
-    from collections.abc import Iterable, Sequence, Generator
-
 from .character import EmojiCharacter
 from .types import BaseDictContainer
-from .utils import data_file, read_data_file_iterable
+from .utils import emoji_data_lines
 
 __all__ = ["EmojiSequence"]
 
 # http://www.unicode.org/reports/tr51/#Data_Files_Table
 # keep the order!
-DATA_FILES = [
-    "emoji-variation-sequences.txt",
-    "emoji-zwj-sequences.txt",
-    "emoji-sequences.txt",
-]
+DATA_FILES = ("emoji-variation-sequences.txt", "emoji-zwj-sequences.txt", "emoji-sequences.txt")
 
 
-class MetaClass(BaseDictContainer):
+class MetaClass(BaseDictContainer[str, "EmojiSequence"]):
     pass
 
 
-class EmojiSequence(metaclass=MetaClass):
+@final
+class EmojiSequence(metaclass=MetaClass):  # pyright: ignore[reportGeneralTypeIssues]
     """Emoji and Text Presentation Sequences used to represent emoji
 
-    see: http://www.unicode.org/reports/tr51/#Emoji_Sequences
+    See also:
+        http://www.unicode.org/reports/tr51/#Emoji_Sequences
     """
 
     def __init__(
         self,
-        code_points: Union[Iterable[int], int],
-        type_field: str = "",
-        description: str = "",
-        comment: str = "",
+        code_points: Union[int, Iterable[int]],
+        type_field: Optional[str] = None,
+        version: Optional[str] = None,
+        variation: Optional[str] = None,
+        description: Optional[str] = None,
     ):
         if isinstance(code_points, Iterable):
             self._code_points = list(code_points)
         else:
             self._code_points = [code_points]
         self._string = "".join(chr(n) for n in self._code_points)
         self._characters = [EmojiCharacter.from_hex(n) for n in self._code_points]
-        self._type_field = type_field.strip()
-        self._comment = comment.strip()
-        self._description = description
+        self._type_field = type_field or ""
+        self._version = version or ""
+        self._variation = variation or ""
+        self._description = description or ""
         # regex
         self._regex = r""
         if not self._regex:
             self._regex = "".join(m.regex for m in self._characters)
         self._regex_pat = re.compile(self._regex)
 
     def __len__(self):
         return len(self._code_points)
 
     def __str__(self):
         return self._string
 
     def __repr__(self):
-        return "<{} code_points={!r} string={!r}, description={!r}>".format(
-            type(self).__name__,
-            self.code_points_string,
-            self.string,
-            self.description,
+        return "<{} code_points={!r} string={!r} version={!r} description={!r}>".format(
+            type(self).__name__, self.code_points_string, self.string, self.version, self.description
         )
 
     _initialed = False
 
-    pattern: Pattern
+    pattern: ClassVar[Pattern[str]]
     """Compiled regular expression pattern object for all-together Emoji sequences.
     """
 
     @classmethod
     def initial(cls):
         """Initial the class
 
@@ -101,119 +93,134 @@
             else:
                 # begin..end form: A range of single char emoji-seq
                 for _cp in range(int(_cp_head, 16), 1 + int(_cp_tail, 16)):
                     _seq = cls(_cp, **_kwargs)
                     cls[_seq.string] = _seq
 
         for fname in DATA_FILES:
-            with data_file(fname).open(encoding="utf8") as fp:
-                for content, comment in read_data_file_iterable(fp):
-                    if fname in ("emoji-sequences.txt", "emoji-zwj-sequences.txt"):
-                        cps, type_field, description = (part.strip() for part in content.split(";", 2))
-                        _decode_code_points(cps, type_field=type_field, description=description, comment=comment)
-                    elif fname == "emoji-variation-sequences.txt":
-                        cps, description = (part.strip() for part in content.split(";", 1))
-                        _decode_code_points(cps, description=description, comment=comment)
-                    else:
-                        raise RuntimeError(f"Invalid data file name {fname}")
+            for content, comment in emoji_data_lines(fname):
+                if fname in ("emoji-sequences.txt", "emoji-zwj-sequences.txt"):
+                    cps, type_field, description = (part.strip() for part in content.split(";", 2))
+                    version = comment.split(maxsplit=1)[0]
+                    _decode_code_points(cps, type_field=type_field, version=version, description=description)
+                elif fname == "emoji-variation-sequences.txt":
+                    cps, variation, _ = (part.strip() for part in content.split(";", 2))
+                    version, description = (x.strip() for x in comment.split(maxsplit=1))
+                    version = "E" + version.lstrip("(").rstrip(")").strip()
+                    description = f"{description.lower()} ({variation})"
+                    _decode_code_points(cps, version=version, variation=variation, description=description)
+                else:
+                    raise RuntimeError(f"Invalid data file name {fname}")
         # build regex
         cls.pattern = re.compile(
-            r"|".join(m.regex for m in sorted((m for m in cls.values()), key=lambda x: len(x.code_points), reverse=True))
+            r"|".join(
+                m.regex
+                for m in sorted(
+                    (m for m in cls.values()),
+                    key=lambda x: len(x.code_points),
+                    reverse=True,
+                )
+            )
         )
         # initialed OK
         cls._initialed = True
 
     @classmethod
     def release(cls):
         if not cls._initialed:
             return
         keys = list(cls)
         for k in keys:
             del cls[k]
         cls._initialed = False
 
-    if sys.version_info < (3, 9):
-
-        @classmethod
-        def items(cls) -> Iterable[Tuple[str, Self]]:
-            return ((k, cls[k]) for k in cls)
-
-    else:
-
-        @classmethod
-        def items(cls) -> Iterable[tuple[str, Self]]:
-            """Return an iterator of all string -> emoji-sequence pairs of the class"""
-            return ((k, cls[k]) for k in cls)
+    @classmethod
+    def items(cls) -> Iterator[Tuple[str, Self]]:
+        """Returns an iterator of all string -> emoji-sequence pairs of the class"""
+        return ((k, cls[k]) for k in cls)  # pyright: ignore[reportReturnType]
 
     @classmethod
-    def keys(cls) -> Iterable[str]:
-        """Return an iterator of each emoji-sequence's key string of the class"""
-        return (k for k in cls)
+    def keys(cls) -> Iterator[str]:
+        """Returns an iterator of each emoji-sequence's key string of the class"""
+        yield from cls
 
     @classmethod
-    def values(cls) -> Iterable[Self]:
-        """Return an iterator of all emoji-sequences of the class"""
-        return (cls[k] for k in cls)
+    def values(cls) -> Iterator[Self]:
+        """Returns an iterator of all emoji-sequences of the class"""
+        return (cls[k] for k in cls)  # pyright: ignore[reportReturnType]
 
     @classmethod
     def from_string(cls, s: str) -> Self:
         """Get an :class:`EmojiSequence` instance from string
 
-        :param s: Emoji string
-        :return: Instance from internal dictionary
-        :raise KeyError: When passed-in ``s`` not found in internal dictionary
+        Args:
+            s: Emoji string
+
+        Returns:
+            Instance from internal dictionary
+
+        Raises:
+            KeyError: When passed-in ``s`` not found in internal dictionary
         """
-        return cls[s]
+        return cls[s]  # pyright: ignore[reportReturnType]
 
     @classmethod
     def from_characters(cls, value: Union[EmojiCharacter, Iterable[EmojiCharacter]]) -> Self:
         """Get an :class:`EmojiSequence` instance from :class:`EmojiCharacter` object or list
 
-        :param value: Single or iterable object of :class:`EmojiCharacter`, composing the sequence
-        :return: Instance from internal dictionary
-        :raise KeyError: When passed-in value not found in internal dictionary
-        :raise TypeError: When passed-in value is not :class:`.EmojiCharacter` object or list
+        Args:
+            value: Single or iterable object of :class:`EmojiCharacter`, composing the sequence
+
+        Returns:
+            Instance from internal dictionary
+
+        Raises:
+            KeyError: When passed-in value not found in internal dictionary
+            TypeError: When passed-in value is not :class:`.EmojiCharacter` object or list
         """
         if isinstance(value, EmojiCharacter):
             s = value.string
         elif isinstance(value, Iterable):
             s = "".join(m.string for m in value)
         else:
             raise TypeError("Argument `value` must be one of `EmojiCharacter` or `Iterable[EmojiCharacter]`")
         return cls.from_string(s)
 
     @classmethod
-    def from_hex(cls, value: Union[str, int, Iterable[str], Iterable[int]]) -> Self:
+    def from_hex(cls, value: Union[int, str, Iterable[Union[int, str]]]) -> Self:
         """Get an :class:`EmojiSequence` instance by unicode code point(s)
 
-        :type value: Union[str, int, Iterable[str], Iterable[int]]
-        :param value: A single or sequence of HEX string/code.
+        Args:
+            value: A single or sequence of HEX string/code.
 
-            - it could be:
+                it could be:
 
-              - one or more code-point(s) in HEX format string, separated by spaces
-              - a single code-point integer
-              - An iterable object whose members are code-point string in HEX format
-              - An iterable object whose members are code-point integer
+                - one or more code-point(s) in HEX format string, separated by spaces
+                - a single code-point integer
+                - An iterable object whose members are code-point string in HEX format
+                - An iterable object whose members are code-point integer
 
-        :return: Instance returned from the class's internal dictionary
+        Returns:
+            Instance returned from the class's internal dictionary
 
-        :raise KeyError: When passed-in value not found in the class' internal dictionary
+        Raises:
+            KeyError: When passed-in value not found in the class internal dictionary
         """
+        cps_array: Iterable[Union[int, str]]
         if isinstance(value, str):
-            cps_array = value.split()  # type: ignore[assignment]
+            cps_array = value.split()
         elif isinstance(value, int):
-            cps_array = (value,)  # type: ignore[assignment]
-        elif isinstance(value, Iterable) and not isinstance(value, str) and all(isinstance(m, (str, int)) for m in value):
-            cps_array = value  # type: ignore[assignment]
+            cps_array = (value,)
+        elif isinstance(value, Iterable):
+            cps_array = value
         else:
             raise TypeError(
                 f"Argument `value` expects to be one of `str`, `bytes`, `int`, or a sequence of that, but actual is {type(value)}"
             )
-        return cls.from_characters(EmojiCharacter.from_hex(cp) for cp in cps_array)
+        return cls.from_characters(EmojiCharacter.from_hex(cp) for cp in cps_array)  # pyright: ignore[reportReturnType]
 
     @property
     def type_field(self) -> str:
         """A convenience for parsing the emoji sequence files, and is not intended to be maintained as a property.
 
         may be one of:
 
@@ -224,30 +231,42 @@
         - `"Emoji_Modifier_Sequence"`
         - `"RGI_Emoji_ZWJ_Sequence"`
         """
         return self._type_field
 
     @property
     def description(self) -> str:
+        """Description"""
         return self._description
 
     @property
-    def comment(self) -> str:
-        return self._comment
+    def version(self) -> str:
+        """Version of the Emoji.
+
+        Example:
+            ``E0.0``, ``E0.6``, ``E11.0``
+        """
+        return self._version
+
+    @property
+    def variation(self) -> str:
+        """``"emoji style"`` or ``"text style"`` of a variable sequence"""
+        return self._variation
 
     @property
     def characters(self) -> Sequence[EmojiCharacter]:
         """Emoji character objects list which makes up the Emoji Sequence"""
         return self._characters
 
     @property
     def hex(self) -> str:
         """Python style hex string of each emoji-characters's code-point, separated by spaces
 
-        eg: ``0xa9 0xfe0f``
+        Example:
+            ``"0xa9 0xfe0f"``
         """
         return " ".join(c.hex for c in self.characters)
 
     @property
     def string(self) -> str:
         """string of the Emoji Sequence"""
         return self._string
@@ -260,72 +279,53 @@
     @property
     def regex_pattern(self):
         """Compiled regular expression pattern of the Emoji Sequence"""
         return self._regex_pat
 
     @property
     def code_points(self) -> Sequence[int]:
-        """List of unicode integer value of the characters who make up Emoji Sequence"""
+        """List of unicode integer value of the characters who make up this Emoji Sequence"""
         return self._code_points
 
     @property
     def code_points_string(self) -> str:
         """Unicode style hex string of each emoji-characters's code-point, separated by spaces
 
-        eg: ``00A9 FE0F``
+        eg: ``"00A9 FE0F"``
         """
         return " ".join(c.code_point_string for c in self.characters)
 
-    if sys.version_info < (3, 9):
-
-        @classmethod
-        def find_all(cls, s: str) -> Sequence[Tuple[Self, int, int]]:
-            return list(cls.find(s))
-
-    else:
-
-        @classmethod
-        def find_all(cls, s: str) -> Sequence[tuple[Self, int, int]]:
-            """Find out all emoji sequences in a string, and return them in a list
-
-            Item of the returned list is as same as that in the iterator of :meth:`find`
-
-            The function equals::
-
-                list(EmojiSequence.find(s))
+    @classmethod
+    def find_all(cls, s: str) -> Sequence[Tuple[Self, int, int]]:
+        """Find out all emoji sequences in a string, and return them in a list
 
-            or ::
+        Items of the returned list is the same as ``yield`` result of :meth:`find`
 
-                [x for x in EmojiSequence.find(s)]
-            """
-            return list(cls.find(s))
+        The function equals::
 
-    if sys.version_info < (3, 9):
+            list(EmojiSequence.find(s))
 
-        @classmethod
-        def find(cls, s: str) -> Generator[Tuple[Self, int, int], None, None]:
-            m = cls.pattern.search(s)
-            while m:
-                yield cls.from_string(m.group()), m.start(), m.end()
-                m = cls.pattern.search(s, m.end())
+        or ::
 
-    else:
+            [x for x in EmojiSequence.find(s)]
+        """
+        return list(cls.find(s))  # pyright: ignore[reportReturnType]
 
-        @classmethod
-        def find(cls, s: str) -> Generator[tuple[Self, int, int], None, None]:
-            """Return an iterator which yields all emoji sequences in a string, without actually storing them all simultaneously.
+    @classmethod
+    def find(cls, s: str) -> Generator[Tuple[Self, int, int], None, None]:
+        """Return an iterator which yields all emoji sequences in a string, without actually storing them all simultaneously.
 
-            :param s: The string to find emoji sequences in it
+        Args:
+            s: The string to find emoji sequences in it
 
-            :return: Item of the iterator is a 3-member tuple:
+        Yields:
+            : Yields at every matched emoji sequence as a 3-members tuple, whose members are:
 
                 0. The found :class:`.EmojiSequence` object
                 1. Begin position of the emoji sequence in the string
                 2. End position of the emoji sequence in the string
-            """
-            m = cls.pattern.search(s)
-            while m:
-                yield cls.from_string(m.group()), m.start(), m.end()
-                m = cls.pattern.search(s, m.end())
+        """
+        for m in cls.pattern.finditer(s):
+            yield cls.from_string(m.group()), m.start(), m.end()
 
 
 EmojiSequence.initial()
```

### Comparing `emoji_data-0.3/src/emoji_data/types.py` & `emoji_data-0.3.1/src/emoji_data/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-import sys
-from typing import Generic, TypeVar
-
-if sys.version_info < (3, 9):  # pragma: no cover
-    from typing import Generator, MutableMapping
-else:  # pragma: no cover
-    from collections.abc import Generator, MutableMapping
+from typing import Any, Dict, Generator, Generic, MutableMapping, Tuple, Type, TypeVar
 
 __all__ = ["BaseDictContainer"]
 
 TK = TypeVar("TK")
 TV = TypeVar("TV")
 
 
-class BaseDictContainer(Generic[TK, TV], type):
-    def __new__(cls, name, bases, attrs):
-        cls.__data__: MutableMapping[TK, TV] = {}  # type:ignore[annotation-unchecked]
+class BaseDictContainer(type, Generic[TK, TV]):
+    __data__: MutableMapping[TK, TV]
+
+    def __new__(cls, name: str, bases: Tuple[Type, ...], attrs: Dict[str, Any]):
+        cls.__data__ = {}
         return super().__new__(cls, name, bases, attrs)
 
     def __setitem__(self, key: TK, value: TV):
         self.__data__[key] = value
 
     def __delitem__(self, key: TK):
         del self.__data__[key]
```

### Comparing `emoji_data-0.3/src/emoji_data.egg-info/PKG-INFO` & `emoji_data-0.3.1/src/emoji_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emoji-data
-Version: 0.3
+Version: 0.3.1
 Summary: A library represents emoji sequences and characters in Unicode® Technical Standard #51 Data Files
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: AGPLv3+
 Project-URL: homepage, https://github.com/tanbro/emoji-data
 Project-URL: repository, https://github.com/tanbro/emoji-data.git
 Keywords: emoji,unicode
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -41,8 +41,8 @@
 
 ```sh
 pip install emoji-data
 ```
 
 ## How to use
 
-See `notebooks/example.ipynb`
+See `docs/notebooks/example.ipynb`
```

### Comparing `emoji_data-0.3/src/emoji_data.egg-info/SOURCES.txt` & `emoji_data-0.3.1/src/emoji_data.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 src/emoji_data/types.py
 src/emoji_data/utils.py
 src/emoji_data.egg-info/PKG-INFO
 src/emoji_data.egg-info/SOURCES.txt
 src/emoji_data.egg-info/dependency_links.txt
 src/emoji_data.egg-info/requires.txt
 src/emoji_data.egg-info/top_level.txt
-src/emoji_data/data/README.txt
+src/emoji_data/data/.markdownlint.json
+src/emoji_data/data/README
 src/emoji_data/data/emoji-data.txt
 src/emoji_data/data/emoji-sequences.txt
 src/emoji_data/data/emoji-test.txt
 src/emoji_data/data/emoji-variation-sequences.txt
 src/emoji_data/data/emoji-zwj-sequences.txt
```

