# Comparing `tmp/yaconfiglib-0.1.0.tar.gz` & `tmp/yaconfiglib-0.1.1.tar.gz`

## Comparing `yaconfiglib-0.1.0.tar` & `yaconfiglib-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/examples/config.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/examples/includeme.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/examples/jinja.yaml.j2
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/src/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/src/yaconfiglib/__init__.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/src/yaconfiglib/jinja2.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/src/yaconfiglib/loader.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/src/yaconfiglib/reader.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/src/yaconfiglib/toml.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/src/yaconfiglib/yaml.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/LICENSE
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 yaconfiglib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/examples/config.toml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/examples/hiera.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/examples/includeme.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/examples/jinja.yaml.j2
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/__init__.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/hiera.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/jinja2.py
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/loader.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/reader.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/toml.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/yaml.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/utils/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/utils/enum.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/utils/log.py
+-rw-r--r--   0        0        0    13130 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/utils/merge.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/LICENSE
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/PKG-INFO
```

### Comparing `yaconfiglib-0.1.0/src/yaconfiglib/loader.py` & `yaconfiglib-0.1.1/src/yaconfiglib/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,38 @@
+import io
 import logging
 import typing
 
 from pathlib_next import LocalPath, Path, Pathname, PosixPathname, glob
+from pathlib_next.mempath import MemPath
 
 try:
-    from .jinja2 import _load_from_text
+    from .jinja2 import jinja2_eval
 except ImportError:
     ...
 
 from .reader import Reader
 
 _LOGGER = logging.getLogger("yaconfiglib")
 
 __all__ = ["Include"]
 
 
+class ConfigBackend(typing.Protocol):
+
+    def load(self, stream: io.IOBase, **options) -> object:
+        raise NotImplementedError()
+
+    def load_all(self, stream: io.IOBase, **options) -> typing.Iterable[object]:
+        yield self.load(stream, **options)
+
+    def dumps(self, data: str, **options) -> str:
+        raise NotImplementedError
+
+
 class ConfigLoader:
 
     DEFAULT_PATH_GENERATOR = LocalPath
     DEFAULT_ENCODING = "utf-8"
 
     def __init__(
         self,
@@ -30,19 +44,15 @@
         recursive: bool = None,
         key_factory: typing.Callable[[Path, object], str] = None,
     ) -> None:
         self.path_factory = path_factory or self.DEFAULT_PATH_GENERATOR
         self.base_dir = base_dir or ""
         self.encoding = encoding or self.DEFAULT_ENCODING
         self.recursive = False if recursive is None else recursive
-        self.reader_factory = reader_factory or (
-            lambda path, *args, **kwargs: Reader.get_class_by_path(path)(
-                path, *args, **kwargs
-            )
-        )
+        self.reader_factory = reader_factory or Reader
         self.key_factory = key_factory or (lambda path, value: path.stem)
 
     def _getpath(self, path: str | Path):
         return path if isinstance(path, Path) else self.path_factory(path)
 
     @property
     def base_dir(self):
@@ -50,62 +60,84 @@
 
     @base_dir.setter
     def base_dir(self, value: str | Path):
         self._base_dir = self._getpath(value)
 
     def _load(
         self,
-        pathname: Path | typing.Sequence[Path],
+        pathname: Path | typing.Sequence[Path] | io.IOBase,
         *,
         recursive: bool = None,
         encoding: str = None,
         reader: str = None,
         transform: str = None,
+        key_factory: str | typing.Callable[[Path], str] = None,
         **reader_args,
     ):
-        pathname = (
-            [self.base_dir / path for path in pathname]
-            if not isinstance(pathname, (str, Pathname))
-            and isinstance(pathname, typing.Sequence)
-            else self.base_dir / pathname
-        )
 
         encoding = encoding or self.encoding
         recursive = self.recursive if recursive is None else recursive
         reader_factory = (
             Reader.get_class_by_name(reader) if reader else self.reader_factory
         )
 
+        if isinstance(pathname, io.IOBase):
+            text = pathname.read()
+            if isinstance(text, str):
+                text = text.encode()
+            filename = reader_args.get("filename", "unknown")
+            pathname = MemPath(filename)
+            pathname.write_bytes(text)
+
+        else:
+            pathname = (
+                [self.base_dir / path for path in pathname]
+                if not isinstance(pathname, (str, Pathname))
+                and isinstance(pathname, typing.Sequence)
+                else self.base_dir / pathname
+            )
+
         paths = [pathname] if isinstance(pathname, Path) else pathname
-        results = []
+        results: list[tuple[str, object]] = []
+        key_factory = key_factory or self.key_factory
+        if not callable(key_factory):
+            if key_factory.startswith("%"):
+                _eval = jinja2_eval(key_factory.removeprefix("%"))
+
+                def _key(path: Path, value):
+                    return _eval(value=value, pathname=PosixPathname(path.as_posix()))
+
+            else:
+                _keyname = key_factory
+
+                def _key(path: Path, value):
+                    val = getattr(path, _keyname)
+                    if callable(val):
+                        val = val()
+                    return str(val)
+
+            key_factory = _key
         for _pathname in paths:
             for path in _pathname.glob("", recursive=self.recursive):
                 _LOGGER.debug(f"Loading file: {path}")
-
                 _reader = reader_factory(
                     path,
                     encoding=self.encoding,
                     path_factory=self.path_factory,
                     reader_factory=self.reader_factory,
                     base_dir=self.base_dir,
                     **reader_args,
                 )
                 value = _reader()
                 if transform:
-                    _globals = {}
-                    _load_from_text(
-                        "{% do _globals.__setitem__('result', " + transform + ") %}"
-                    ).render(
-                        value=value,
-                        _globals=_globals,
-                        pathname=PosixPathname(path.as_posix()),
+                    value = jinja2_eval(transform)(
+                        value=value, pathname=PosixPathname(path.as_posix())
                     )
-                    value = _globals["result"]
 
-                results.append((path, value))
+                results.append((key_factory(path, value), value))
 
         return (
             results,
             isinstance(pathname, Pathname)
             and glob.WILCARD_PATTERN.match(pathname.as_posix()) is None,
         )
 
@@ -125,48 +157,19 @@
     ):
         results, single = self._load(
             pathname,
             recursive=recursive,
             encoding=encoding,
             reader=reader,
             transform=transform,
+            key_factory=key_factory,
             **reader_args,
         )
         if not type:
             type = "single" if single else "list"
-        key_factory = key_factory or self.key_factory
-        if not callable(key_factory):
-            if key_factory.startswith("%"):
-                key_factory = key_factory.removeprefix("%")
-                template = _load_from_text(
-                    "{% do _globals.__setitem__('result', " + key_factory + ") %}"
-                )
-
-                def _key(path: Path, value):
-                    _globals = {}
-                    template.render(
-                        value=value,
-                        _globals=_globals,
-                        pathname=PosixPathname(path.as_posix()),
-                    )
-                    return _globals["result"]
-
-            else:
-                _keyname = key_factory
-
-                def _key(path: Path, value):
-                    val = getattr(path, _keyname)
-                    if callable(val):
-                        val = val()
-                    return str(val)
-
-            key_factory = _key
-
-        results = [(key_factory(path, result), result) for path, result in results]
-
         type = type.lower()
         match type:
             case "single" | "scalar":
                 return results[-1][1] if results else default
             case "list" | "array":
                 results: list[dict[str]] = [result[1] for result in results]
             case "map" | "dict" | "hash":
@@ -185,7 +188,18 @@
                     for path, result in results.items()
                     for prop, value in result.items()
                 }
         else:
             result = results
 
         return result
+
+    def load_all(
+        self,
+        pathname: Path | typing.Sequence[Path],
+        **reader_args,
+    ):
+        return self.load(pathname, type="list", flatten=False, **reader_args)
+        ...
+
+
+DEFAULT_LOADER = ConfigLoader()
```

### Comparing `yaconfiglib-0.1.0/src/yaconfiglib/yaml.py` & `yaconfiglib-0.1.1/src/yaconfiglib/yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 import yaml
 from pathlib_next import Path, Pathname
 
 from .loader import ConfigLoader
 from .reader import Reader
 
-__all__ = ["Include", "YamlReader"]
+__all__ = ["YamlConfigLoader", "YamlReader"]
 
 
-class Include(ConfigLoader):
+class YamlConfigLoader(ConfigLoader):
     def __call__(self, loader: yaml.Loader, node: yaml.Node):
         args = ()
         kwargs = {}
         pathname: str | Pathname | typing.Sequence[str | Pathname]
         if isinstance(node, yaml.nodes.ScalarNode):
             pathname = loader.construct_scalar(node)
         elif isinstance(node, yaml.nodes.SequenceNode):
```

### Comparing `yaconfiglib-0.1.0/LICENSE` & `yaconfiglib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.1.0/pyproject.toml` & `yaconfiglib-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yaconfiglib"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Jose A" }]
 description = "Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `yaconfiglib-0.1.0/PKG-INFO` & `yaconfiglib-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yaconfiglib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating.
 Project-URL: Homepage, https://github.com/jose-pr/yaconfiglib/
 Project-URL: Issues, https://github.com/jose-pr/yaconfiglib/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,8 +23,11 @@
 
 # yaconfiglib
 Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating.
 
 # Inspire/Based on v1 of yamlinclude:
 Source: https://github.com/tanbro/pyyaml-include 
 
+# Also based on hiyapyco for chain loading/merge template support
+Source: https://github.com/zerwes/hiyapyco
+
```

