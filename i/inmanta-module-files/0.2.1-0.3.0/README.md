# Comparing `tmp/inmanta_module_files-0.2.1-py3-none-any.whl.zip` & `tmp/inmanta_module_files-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 21124 bytes, number of entries: 19
--rw-r--r--  2.0 unx      602 b- defN 24-Apr-21 08:19 inmanta_plugins/files/__init__.py
--rw-r--r--  2.0 unx     2624 b- defN 24-Apr-21 08:19 inmanta_plugins/files/base.py
--rw-r--r--  2.0 unx     3188 b- defN 24-Apr-21 08:19 inmanta_plugins/files/directory.py
--rw-r--r--  2.0 unx     6585 b- defN 24-Apr-21 08:19 inmanta_plugins/files/host.py
--rw-r--r--  2.0 unx     5848 b- defN 24-Apr-21 08:19 inmanta_plugins/files/json.py
--rw-r--r--  2.0 unx     2170 b- defN 24-Apr-21 08:19 inmanta_plugins/files/setup.cfg
--rw-r--r--  2.0 unx     2258 b- defN 24-Apr-21 08:19 inmanta_plugins/files/systemd_unit.py
--rw-r--r--  2.0 unx     2200 b- defN 24-Apr-21 08:19 inmanta_plugins/files/text.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-21 08:19 inmanta_plugins/files/files/.gitkeep
--rw-r--r--  2.0 unx     3706 b- defN 24-Apr-21 08:19 inmanta_plugins/files/model/_init.cf
--rw-r--r--  2.0 unx     1661 b- defN 24-Apr-21 08:19 inmanta_plugins/files/model/host.cf
--rw-r--r--  2.0 unx     1586 b- defN 24-Apr-21 08:19 inmanta_plugins/files/model/json.cf
--rw-r--r--  2.0 unx    10884 b- defN 24-Apr-21 08:19 inmanta_plugins/files/model/systemd_unit.cf
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-21 08:19 inmanta_plugins/files/templates/.gitkeep
--rw-r--r--  2.0 unx     2950 b- defN 24-Apr-21 08:19 inmanta_plugins/files/templates/systemd_unit.j2
--rw-r--r--  2.0 unx      742 b- defN 24-Apr-21 08:19 inmanta_module_files-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 08:19 inmanta_module_files-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-21 08:19 inmanta_module_files-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-21 08:19 inmanta_module_files-0.2.1.dist-info/RECORD
-19 files, 48833 bytes uncompressed, 18252 bytes compressed:  62.6%
+Zip file size: 21581 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      602 b- defN 24-Apr-27 22:30 inmanta_plugins/files/__init__.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Apr-27 22:30 inmanta_plugins/files/base.py
+-rw-r--r--  2.0 unx     3188 b- defN 24-Apr-27 22:30 inmanta_plugins/files/directory.py
+-rw-r--r--  2.0 unx     6585 b- defN 24-Apr-27 22:30 inmanta_plugins/files/host.py
+-rw-r--r--  2.0 unx     7436 b- defN 24-Apr-27 22:30 inmanta_plugins/files/json.py
+-rw-r--r--  2.0 unx     2170 b- defN 24-Apr-27 22:31 inmanta_plugins/files/setup.cfg
+-rw-r--r--  2.0 unx     2258 b- defN 24-Apr-27 22:30 inmanta_plugins/files/systemd_unit.py
+-rw-r--r--  2.0 unx     2200 b- defN 24-Apr-27 22:30 inmanta_plugins/files/text.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 22:30 inmanta_plugins/files/files/.gitkeep
+-rw-r--r--  2.0 unx     3856 b- defN 24-Apr-27 22:30 inmanta_plugins/files/model/_init.cf
+-rw-r--r--  2.0 unx     1661 b- defN 24-Apr-27 22:30 inmanta_plugins/files/model/host.cf
+-rw-r--r--  2.0 unx     1586 b- defN 24-Apr-27 22:30 inmanta_plugins/files/model/json.cf
+-rw-r--r--  2.0 unx    10884 b- defN 24-Apr-27 22:30 inmanta_plugins/files/model/systemd_unit.cf
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 22:30 inmanta_plugins/files/templates/.gitkeep
+-rw-r--r--  2.0 unx     2950 b- defN 24-Apr-27 22:30 inmanta_plugins/files/templates/systemd_unit.j2
+-rw-r--r--  2.0 unx      742 b- defN 24-Apr-27 22:31 inmanta_module_files-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 22:31 inmanta_module_files-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-27 22:31 inmanta_module_files-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-27 22:31 inmanta_module_files-0.3.0.dist-info/RECORD
+19 files, 50571 bytes uncompressed, 18709 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: inmanta_plugins/files/templates/.gitkeep
 Comment: 
 
 Filename: inmanta_plugins/files/templates/systemd_unit.j2
 Comment: 
 
-Filename: inmanta_module_files-0.2.1.dist-info/METADATA
+Filename: inmanta_module_files-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_files-0.2.1.dist-info/WHEEL
+Filename: inmanta_module_files-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_files-0.2.1.dist-info/top_level.txt
+Filename: inmanta_module_files-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_files-0.2.1.dist-info/RECORD
+Filename: inmanta_module_files-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/files/json.py

```diff
@@ -15,14 +15,17 @@
 
 Contact: edvgui@gmail.com
 """
 
 import copy
 import enum
 import json
+import typing
+
+import yaml
 
 import inmanta.agent.agent
 import inmanta.agent.handler
 import inmanta.agent.io.local
 import inmanta.const
 import inmanta.execute.proxy
 import inmanta.export
@@ -78,17 +81,19 @@
     name="files::JsonFile",
     id_attribute="path",
     agent="host.name",
 )
 class JsonFileResource(inmanta_plugins.files.base.BaseFileResource):
     fields = (
         "indent",
+        "format",
         "values",
     )
     values: list[dict]
+    format: typing.Literal["json", "yaml"]
     indent: int
 
     @classmethod
     def get_values(cls, _, entity: inmanta.execute.proxy.DynamicProxy) -> list[dict]:
         return [
             {
                 "path": value.path,
@@ -99,23 +104,59 @@
         ]
 
 
 @inmanta.agent.handler.provider("files::JsonFile", "")
 class JsonFileHandler(inmanta_plugins.files.base.BaseFileHandler[JsonFileResource]):
     _io: inmanta.agent.io.local.LocalIO
 
+    def from_json(self, raw: str, *, format: typing.Literal["json", "yaml"]) -> object:
+        """
+        Convert a json-like raw string in the expected format to the corresponding
+        python dict-like object.
+
+        :param raw: The raw value, as read in the file.
+        :param format: The format of the value.
+        """
+        if format == "json":
+            return json.loads(raw)
+        if format == "yaml":
+            return yaml.safe_load(raw)
+        raise ValueError(f"Unsupported format: {format}")
+
+    def to_json(
+        self,
+        value: object,
+        *,
+        format: typing.Literal["json", "yaml"],
+        indent: typing.Optional[int] = None,
+    ) -> str:
+        """
+        Dump a dict-like structure into a json-like string.  The string can
+        be in different formats, depending on the value specified.
+
+        :param value: The dict-like value, to be written to file.
+        :param format: The format of the value.
+        :param indent: Whether any indentation should be applied to the
+            value written to file.
+        """
+        if format == "json":
+            return json.dumps(value, indent=indent)
+        if format == "yaml":
+            return yaml.safe_dump(value, indent=indent)
+        raise ValueError(f"Unsupported format: {format}")
+
     def read_resource(
         self, ctx: inmanta.agent.handler.HandlerContext, resource: JsonFileResource
     ) -> None:
         super().read_resource(ctx, resource)
 
         # Load the content of the existing file
         raw_content = self._io.read_binary(resource.path).decode()
         ctx.debug("Reading existing file", raw_content=raw_content)
-        ctx.set("current_content", json.loads(raw_content))
+        ctx.set("current_content", self.from_json(raw_content, format=resource.format))
 
     def calculate_diff(
         self,
         ctx: inmanta.agent.handler.HandlerContext,
         current: JsonFileResource,
         desired: JsonFileResource,
     ) -> dict[str, dict[str, object]]:
@@ -154,23 +195,31 @@
                 content,
                 dict_path.to_path(value["path"]),
                 Operation(value["operation"]),
                 value["value"],
             )
 
         indent = resource.indent if resource.indent != 0 else None
-        raw_content = json.dumps(content, indent=indent)
+        raw_content = self.to_json(
+            content,
+            format=resource.format,
+            indent=indent,
+        )
         self._io.put(resource.path, raw_content.encode())
         super().create_resource(ctx, resource)
 
     def update_resource(
         self,
         ctx: inmanta.agent.handler.HandlerContext,
         changes: dict[str, dict[str, object]],
         resource: JsonFileResource,
     ) -> None:
         if "content" in changes:
             indent = resource.indent if resource.indent != 0 else None
-            raw_content = json.dumps(changes["content"]["desired"], indent=indent)
+            raw_content = self.to_json(
+                changes["content"]["desired"],
+                format=resource.format,
+                indent=indent,
+            )
             self._io.put(resource.path, raw_content.encode())
 
         super().update_resource(ctx, changes, resource)
```

## inmanta_plugins/files/setup.cfg

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inmanta-module-files
-version = 0.2.1
+version = 0.3.0
 description = Simple module containing various types of resource to manage files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Guillaume Everarts de Velp
 author_email = edvgui@gmail.com
 license = ASL 2.0
 copyright = 2023 Guillaume Everarts de Velp
```

## inmanta_plugins/files/model/_init.cf

```diff
@@ -24,14 +24,16 @@
 """
 Define the type of operation to apply for a batch of data in a desired state.
 These operations are inspired from the netconf yang specifications and have the
 same semantic.
 cf. https://datatracker.ietf.org/doc/html/rfc4741#section-7.2
 """
 
+typedef json_format_t as string matching self in ["json", "yaml"]
+
 
 entity BaseFile extends std::PurgeableResource, std::ManagedResource:
     """
     Base entity representing a file on a host.
 
     :attr path: The path where the file should be managed.
     :attr permissions: The permissions to set on the file
@@ -87,17 +89,18 @@
 entity JsonFile extends BaseFile:
     """
     A JsonFile on the given host.  The resource contains a set of values
     that needs to be enforced on the given file.  See files::json::Value for
     more information about the usage of said values.
 
     :attr indent: The indentiation to use when writing in the file.
+    :attr format: The format the json content is supposed to be written in.
     """
     int indent = 2
-    bool send_event = true
+    json_format_t format = "json"
 end
 JsonFile.values [0:] -- files::json::Value.json_file [1]
 """
 The set of values that will be enforced in the file.
 """
 
 index JsonFile(host, path)
```

## Comparing `inmanta_module_files-0.2.1.dist-info/METADATA` & `inmanta_module_files-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-module-files
-Version: 0.2.1
+Version: 0.3.0
 Summary: Simple module containing various types of resource to manage files.
 Author: Guillaume Everarts de Velp
 Author-email: edvgui@gmail.com
 License: ASL 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: inmanta-module-std
```

## Comparing `inmanta_module_files-0.2.1.dist-info/RECORD` & `inmanta_module_files-0.3.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 inmanta_plugins/files/__init__.py,sha256=BUgfj_qgct0U3NELQUglCpB81sjkDRMCrHtloSL4ylM,602
 inmanta_plugins/files/base.py,sha256=nIuZ5q3mj876P6n6aeZ_ramQUHzR7NjJ4G_tsuRPKrc,2624
 inmanta_plugins/files/directory.py,sha256=pqCVFBLz_zQUHQ6e5rG43ht0njicMop-4GCXBsWYo_w,3188
 inmanta_plugins/files/host.py,sha256=c4pcP8zroNLc2RbVgOnQYlA5mdqQnP45cnS8941cMHk,6585
-inmanta_plugins/files/json.py,sha256=kY6ql6QB9BUA2bPTrX7LSgYrNcIlJlYzTQDoIMrahNg,5848
-inmanta_plugins/files/setup.cfg,sha256=j2-IfC8YZzA4JxNieMmTkObetLmSnpAmBJJvRXXiBi8,2170
+inmanta_plugins/files/json.py,sha256=0RCdzY1sOGMd9j_bmTdnpmd1jhZOjjsa-JnjTWBpm94,7436
+inmanta_plugins/files/setup.cfg,sha256=k2DifyK03qLRtKYBRW7W7ODfTH3YcSzmTG8MZGf1XBI,2170
 inmanta_plugins/files/systemd_unit.py,sha256=x_-yy9Bl_8O_SNViIkwtpH8ma-NZskmqlGkGBzkSoN4,2258
 inmanta_plugins/files/text.py,sha256=h6ZoDGtZYlC2yEGiLpopL96rOMKUrw-AxPULEysO8-I,2200
 inmanta_plugins/files/files/.gitkeep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inmanta_plugins/files/model/_init.cf,sha256=rCoI_LIQxT6xgGzNixEnl3OgI8NfaBm7bEUgAqqjGxM,3706
+inmanta_plugins/files/model/_init.cf,sha256=OPZT5KC2BW_Tvnk9MXLyzJY6JbhmgrigiY1nafLok_w,3856
 inmanta_plugins/files/model/host.cf,sha256=tpW8EhP9ECeZ_Q97Q7giwIrjj6HlVd9XzvchFkCS4XA,1661
 inmanta_plugins/files/model/json.cf,sha256=6Om8bihPKrZX7-hfyZLZ_rn7G-CLwf0BNvggJOdkTx8,1586
 inmanta_plugins/files/model/systemd_unit.cf,sha256=prsWy4r9ofpeQoHcszIc89usgkGl_UtC3gcRILpQ4QQ,10884
 inmanta_plugins/files/templates/.gitkeep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inmanta_plugins/files/templates/systemd_unit.j2,sha256=fp-_5ggm2U_YPCGhPzKWrOigQZMbqTJ6AdhwUd7nQ9A,2950
-inmanta_module_files-0.2.1.dist-info/METADATA,sha256=9T2Sd6HqAYwdlsYiySNq7U-qHG0tjrBZ7CyF8FWR1wI,742
-inmanta_module_files-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-inmanta_module_files-0.2.1.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_files-0.2.1.dist-info/RECORD,,
+inmanta_module_files-0.3.0.dist-info/METADATA,sha256=i-8skP-RD48uU-pu18kR-1fB9Ukw83O3_Ihj0PYYTmk,742
+inmanta_module_files-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+inmanta_module_files-0.3.0.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_files-0.3.0.dist-info/RECORD,,
```

