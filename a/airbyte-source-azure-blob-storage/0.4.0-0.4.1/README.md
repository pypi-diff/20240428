# Comparing `tmp/airbyte_source_azure_blob_storage-0.4.0.tar.gz` & `tmp/airbyte_source_azure_blob_storage-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_azure_blob_storage-0.4.0.tar", max compression
+gzip compressed data, was "airbyte_source_azure_blob_storage-0.4.1.tar", max compression
```

## Comparing `airbyte_source_azure_blob_storage-0.4.0.tar` & `airbyte_source_azure_blob_storage-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     5422 2024-04-15 09:33:52.668413 airbyte_source_azure_blob_storage-0.4.0/README.md
--rw-r--r--   0        0        0     1016 2024-04-15 09:36:59.723759 airbyte_source_azure_blob_storage-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      281 2024-04-15 09:33:52.672412 airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/__init__.py
--rw-r--r--   0        0        0     3949 2024-04-15 09:33:52.672412 airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/config.py
--rw-r--r--   0        0        0     2712 2024-04-15 09:33:52.672412 airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/config_migrations.py
--rw-r--r--   0        0        0     1306 2024-04-15 09:33:52.672412 airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/legacy_config_transformer.py
--rw-r--r--   0        0        0     1890 2024-04-15 09:33:52.672412 airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/run.py
--rw-r--r--   0        0        0     3456 2024-04-15 09:33:52.672412 airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/source.py
--rw-r--r--   0        0        0     4227 2024-04-15 09:33:52.672412 airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/stream_reader.py
--rw-r--r--   0        0        0     6246 1970-01-01 00:00:00.000000 airbyte_source_azure_blob_storage-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     5422 2024-04-28 19:25:58.625856 airbyte_source_azure_blob_storage-0.4.1/README.md
+-rw-r--r--   0        0        0     1037 2024-04-28 19:28:41.706029 airbyte_source_azure_blob_storage-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      319 2024-04-28 19:25:58.629856 airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/__init__.py
+-rw-r--r--   0        0        0     4328 2024-04-28 19:25:58.629856 airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/config_migrations.py
+-rw-r--r--   0        0        0     2009 2024-04-28 19:25:58.629856 airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/run.py
+-rw-r--r--   0        0        0     2579 2024-04-28 19:25:58.629856 airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/source.py
+-rw-r--r--   0        0        0     3969 2024-04-28 19:25:58.629856 airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/spec.py
+-rw-r--r--   0        0        0     4261 2024-04-28 19:25:58.629856 airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/stream_reader.py
+-rw-r--r--   0        0        0     6246 1970-01-01 00:00:00.000000 airbyte_source_azure_blob_storage-0.4.1/PKG-INFO
```

### Comparing `airbyte_source_azure_blob_storage-0.4.0/README.md` & `airbyte_source_azure_blob_storage-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_azure_blob_storage-0.4.0/pyproject.toml` & `airbyte_source_azure_blob_storage-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.4.0"
+version = "0.4.1"
 name = "airbyte-source-azure-blob-storage"
 description = "Source implementation for Azure Blob Storage."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -37,11 +37,12 @@
 version = "==6.4.0"
 
 [tool.poetry.scripts]
 source-azure-blob-storage = "source_azure_blob_storage.run:run"
 
 [tool.poetry.group.dev.dependencies]
 docker = "^7.0.0"
+freezegun = "^1.4.0"
 pytest-mock = "^3.6.1"
 requests-mock = "^1.9.3"
 pandas = "2.2.1"
 pytest = "^6.2"
```

### Comparing `airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/config.py` & `airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         description="The Azure blob storage account key.",
         airbyte_secret=True,
         examples=["Z8ZkZpteggFx394vm+PJHnGTvdRncaYS+JhLKdj789YNmD+iyGTnG+PV+POiuYNhBg/ACS+LKjd%4FG3FHGN12Nd=="],
         order=3,
     )
 
 
-class Config(AbstractFileBasedSpec):
+class SourceAzureBlobStorageSpec(AbstractFileBasedSpec):
     """
     NOTE: When this Spec is changed, legacy_config_transformer.py must also be modified to uptake the changes
     because it is responsible for converting legacy Azure Blob Storage v0 configs into v1 configs using the File-Based CDK.
     """
 
     @classmethod
     def documentation_url(cls) -> AnyUrl:
```

### Comparing `airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/config_migrations.py` & `airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/config_migrations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 import logging
+from abc import ABC, abstractmethod
 from typing import Any, List, Mapping
 
 from airbyte_cdk.config_observation import create_connector_config_control_message
 from airbyte_cdk.entrypoint import AirbyteEntrypoint
 from airbyte_cdk.sources import Source
 
 logger = logging.getLogger("airbyte_logger")
 
 
-class MigrateCredentials:
-    """
-    This class stands for migrating the config azure_blob_storage_account_key inside object `credentials`
-    """
-
+class MigrateConfig(ABC):
     @classmethod
+    @abstractmethod
     def should_migrate(cls, config: Mapping[str, Any]) -> bool:
-        return "credentials" not in config
+        ...
 
     @classmethod
-    def set_azure_blob_storage_account_key(cls, config: Mapping[str, Any]) -> Mapping[str, Any]:
-        config["credentials"] = {
-            "auth_type": "storage_account_key",
-            "azure_blob_storage_account_key": config.pop("azure_blob_storage_account_key"),
-        }
-        return config
+    @abstractmethod
+    def migrate_config(cls, config: Mapping[str, Any]) -> Mapping[str, Any]:
+        ...
 
     @classmethod
     def modify_and_save(cls, config_path: str, source: Source, config: Mapping[str, Any]) -> Mapping[str, Any]:
         """
         Modifies the configuration and then saves it back to the source.
 
         Args:
         - config_path (str): The path where the configuration is stored.
         - source (Source): The data source.
         - config (Mapping[str, Any]): The current configuration.
 
         Returns:
         - Mapping[str, Any]: The updated configuration.
         """
-        migrated_config = cls.set_azure_blob_storage_account_key(config)
+        migrated_config = cls.migrate_config(config)
         source.write_config(migrated_config, config_path)
         return migrated_config
 
     @classmethod
     def emit_control_message(cls, migrated_config: Mapping[str, Any]) -> None:
         """
         Emits the control messages related to configuration migration.
@@ -71,7 +66,54 @@
         - source (Source): The data source.
         """
         config_path = AirbyteEntrypoint(source).extract_config(args)
         if config_path:
             config = source.read_config(config_path)
             if cls.should_migrate(config):
                 cls.emit_control_message(cls.modify_and_save(config_path, source, config))
+
+
+class MigrateLegacyConfig(MigrateConfig):
+    """
+    Class that takes in Azure Blob Storage source configs in the legacy format and transforms them into
+    configs that can be used by the new Azure Blob Storage source built with the file-based CDK.
+    """
+
+    @classmethod
+    def should_migrate(cls, config: Mapping[str, Any]) -> bool:
+        return "streams" not in config
+
+    @classmethod
+    def migrate_config(cls, legacy_config: Mapping[str, Any]) -> Mapping[str, Any]:
+        azure_blob_storage_blobs_prefix = legacy_config.get("azure_blob_storage_blobs_prefix", "")
+        return {
+            "azure_blob_storage_endpoint": legacy_config.get("azure_blob_storage_endpoint", None),
+            "azure_blob_storage_account_name": legacy_config["azure_blob_storage_account_name"],
+            "azure_blob_storage_account_key": legacy_config["azure_blob_storage_account_key"],
+            "azure_blob_storage_container_name": legacy_config["azure_blob_storage_container_name"],
+            "streams": [
+                {
+                    "name": legacy_config["azure_blob_storage_container_name"],
+                    "legacy_prefix": azure_blob_storage_blobs_prefix,
+                    "validation_policy": "Emit Record",
+                    "format": {"filetype": "jsonl"},
+                }
+            ],
+        }
+
+
+class MigrateCredentials(MigrateConfig):
+    """
+    This class stands for migrating the config azure_blob_storage_account_key inside object `credentials`
+    """
+
+    @classmethod
+    def should_migrate(cls, config: Mapping[str, Any]) -> bool:
+        return "credentials" not in config
+
+    @classmethod
+    def migrate_config(cls, config: Mapping[str, Any]) -> Mapping[str, Any]:
+        config["credentials"] = {
+            "auth_type": "storage_account_key",
+            "azure_blob_storage_account_key": config.pop("azure_blob_storage_account_key"),
+        }
+        return config
```

### Comparing `airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/run.py` & `airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 import sys
 import traceback
 from datetime import datetime
 
 from airbyte_cdk.entrypoint import AirbyteEntrypoint, launch
 from airbyte_cdk.models import AirbyteErrorTraceMessage, AirbyteMessage, AirbyteTraceMessage, TraceType, Type
 from airbyte_cdk.sources.file_based.stream.cursor import DefaultFileBasedCursor
-from source_azure_blob_storage import Config, SourceAzureBlobStorage, SourceAzureBlobStorageStreamReader
-from source_azure_blob_storage.config_migrations import MigrateCredentials
+from source_azure_blob_storage import SourceAzureBlobStorage, SourceAzureBlobStorageSpec, SourceAzureBlobStorageStreamReader
+from source_azure_blob_storage.config_migrations import MigrateCredentials, MigrateLegacyConfig
 
 
 def run():
     args = sys.argv[1:]
     catalog_path = AirbyteEntrypoint.extract_catalog(args)
     config_path = AirbyteEntrypoint.extract_config(args)
     state_path = AirbyteEntrypoint.extract_state(args)
     try:
         source = SourceAzureBlobStorage(
             SourceAzureBlobStorageStreamReader(),
-            Config,
+            SourceAzureBlobStorageSpec,
             SourceAzureBlobStorage.read_catalog(catalog_path) if catalog_path else None,
             SourceAzureBlobStorage.read_config(config_path) if catalog_path else None,
             SourceAzureBlobStorage.read_state(state_path) if catalog_path else None,
             cursor_cls=DefaultFileBasedCursor,
         )
+        MigrateLegacyConfig.migrate(sys.argv[1:], source)
         MigrateCredentials.migrate(sys.argv[1:], source)
     except Exception:
         print(
             AirbyteMessage(
                 type=Type.TRACE,
                 trace=AirbyteTraceMessage(
                     type=TraceType.ERROR,
```

### Comparing `airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/source.py` & `airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/source.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,36 +5,16 @@
 from typing import Any, Mapping
 
 from airbyte_cdk.config_observation import emit_configuration_as_airbyte_control_message
 from airbyte_cdk.sources.declarative.models import OAuthConfigSpecification
 from airbyte_cdk.sources.file_based.file_based_source import FileBasedSource
 from airbyte_protocol.models import AdvancedAuth, ConnectorSpecification
 
-from .legacy_config_transformer import LegacyConfigTransformer
-
 
 class SourceAzureBlobStorage(FileBasedSource):
-    @classmethod
-    def read_config(cls, config_path: str) -> Mapping[str, Any]:
-        """
-        Used to override the default read_config so that when the new file-based Azure Blob Storage connector processes a config
-        in the legacy format, it can be transformed into the new config. This happens in entrypoint before we
-        validate the config against the new spec.
-        """
-        config = FileBasedSource.read_config(config_path)
-        if not cls._is_v1_config(config):
-            converted_config = LegacyConfigTransformer.convert(config)
-            emit_configuration_as_airbyte_control_message(converted_config)
-            return converted_config
-        return config
-
-    @staticmethod
-    def _is_v1_config(config: Mapping[str, Any]) -> bool:
-        return "streams" in config
-
     def spec(self, *args: Any, **kwargs: Any) -> ConnectorSpecification:
         """
         Returns the specification describing what fields can be configured by a user when setting up a file-based source.
         """
 
         return ConnectorSpecification(
             documentationUrl=self.spec_class.documentation_url(),
```

### Comparing `airbyte_source_azure_blob_storage-0.4.0/source_azure_blob_storage/stream_reader.py` & `airbyte_source_azure_blob_storage-0.4.1/source_azure_blob_storage/stream_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from airbyte_cdk.sources.file_based.file_based_stream_reader import AbstractFileBasedStreamReader, FileReadMode
 from airbyte_cdk.sources.file_based.remote_file import RemoteFile
 from airbyte_cdk.sources.streams.http.requests_native_auth import Oauth2Authenticator
 from azure.core.credentials import AccessToken
 from azure.storage.blob import BlobServiceClient, ContainerClient
 from smart_open import open
 
-from .config import Config
+from .spec import SourceAzureBlobStorageSpec
 
 
 class AzureOauth2Authenticator(Oauth2Authenticator):
     """
     Authenticator for Azure Blob Storage SDK to align with azure.core.credentials.TokenCredential protocol
     """
 
@@ -31,19 +31,19 @@
     _credentials = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._config = None
 
     @property
-    def config(self) -> Config:
+    def config(self) -> SourceAzureBlobStorageSpec:
         return self._config
 
     @config.setter
-    def config(self, value: Config) -> None:
+    def config(self, value: SourceAzureBlobStorageSpec) -> None:
         self._config = value
 
     @property
     def account_url(self) -> str:
         if not self.config.azure_blob_storage_endpoint:
             return f"https://{self.config.azure_blob_storage_account_name}.blob.core.windows.net"
         return self.config.azure_blob_storage_endpoint
@@ -79,16 +79,15 @@
         logger: logging.Logger,
     ) -> Iterable[RemoteFile]:
         prefixes = [prefix] if prefix else self.get_prefixes_from_globs(globs)
         prefixes = prefixes or [None]
         for prefix in prefixes:
             for blob in self.azure_container_client.list_blobs(name_starts_with=prefix):
                 remote_file = RemoteFile(uri=blob.name, last_modified=blob.last_modified.astimezone(pytz.utc).replace(tzinfo=None))
-                if not globs or self.file_matches_globs(remote_file, globs):
-                    yield remote_file
+                yield from self.filter_files_by_globs_and_start_date([remote_file], globs)
 
     def open_file(self, file: RemoteFile, mode: FileReadMode, encoding: Optional[str], logger: logging.Logger) -> IOBase:
         try:
             result = open(
                 f"azure://{self.config.azure_blob_storage_container_name}/{file.uri}",
                 transport_params={"client": self.azure_blob_service_client},
                 mode=mode.value,
```

### Comparing `airbyte_source_azure_blob_storage-0.4.0/PKG-INFO` & `airbyte_source_azure_blob_storage-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-azure-blob-storage
-Version: 0.4.0
+Version: 0.4.1
 Summary: Source implementation for Azure Blob Storage.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

