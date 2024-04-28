# Comparing `tmp/py_ucan-0.3.1.tar.gz` & `tmp/py_ucan-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ucan-0.3.1.tar", max compression
+gzip compressed data, was "py_ucan-0.4.0.tar", max compression
```

## Comparing `py_ucan-0.3.1.tar` & `py_ucan-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-04-27 11:06:17.782066 py_ucan-0.3.1/LICENSE
--rw-r--r--   0        0        0       10 2024-04-27 11:06:17.782066 py_ucan-0.3.1/README.md
--rw-r--r--   0        0        0    10293 2024-04-27 11:06:19.634090 py_ucan-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1630 2024-04-27 11:06:19.642090 py_ucan-0.3.1/src/ucan/__init__.py
--rw-r--r--   0        0        0      744 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/constants.py
--rw-r--r--   0        0        0       30 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/__init__.py
--rw-r--r--   0        0        0     6739 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/attenuation.py
--rw-r--r--   0        0        0     1754 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/plugins.py
--rw-r--r--   0        0        0     1484 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/semver.py
--rw-r--r--   0        0        0     6735 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/token.py
--rw-r--r--   0        0        0     4284 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/types.py
--rw-r--r--   0        0        0     5889 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/core/verify.py
--rw-r--r--   0        0        0      181 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/default_plugins/__init__.py
--rw-r--r--   0        0        0     2851 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/default_plugins/ed25519.py
--rw-r--r--   0        0        0        0 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/py.typed
--rw-r--r--   0        0        0      914 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/schemas.py
--rw-r--r--   0        0        0      205 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/typing.py
--rw-r--r--   0        0        0     2192 2024-04-27 11:06:17.782066 py_ucan-0.3.1/src/ucan/utils.py
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 py_ucan-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 03:25:15.512725 py_ucan-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3707 2024-04-28 03:25:15.512725 py_ucan-0.4.0/README.md
+-rw-r--r--   0        0        0    10266 2024-04-28 03:25:16.516728 py_ucan-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2277 2024-04-28 03:25:16.524728 py_ucan-0.4.0/src/ucan/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/constants.py
+-rw-r--r--   0        0        0       30 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/__init__.py
+-rw-r--r--   0        0        0     6739 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/attenuation.py
+-rw-r--r--   0        0        0     3059 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/plugins.py
+-rw-r--r--   0        0        0     1484 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/semver.py
+-rw-r--r--   0        0        0     6731 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/token.py
+-rw-r--r--   0        0        0     4121 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/types.py
+-rw-r--r--   0        0        0     5965 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/verify.py
+-rw-r--r--   0        0        0      181 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/default_plugins/__init__.py
+-rw-r--r--   0        0        0     2853 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/default_plugins/ed25519.py
+-rw-r--r--   0        0        0        0 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/py.typed
+-rw-r--r--   0        0        0      849 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/schemas.py
+-rw-r--r--   0        0        0      205 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/typing.py
+-rw-r--r--   0        0        0     2192 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/utils.py
+-rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 py_ucan-0.4.0/PKG-INFO
```

### Comparing `py_ucan-0.3.1/LICENSE` & `py_ucan-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.1/pyproject.toml` & `py_ucan-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # ----------------------------------------------------------------------------------------------------------------------
 # poetry
 [tool.poetry]
 package-mode = true
 name = "py-ucan"
-version = "0.3.1"
+version = "0.4.0"
 description = "Python Ucan"
 readme = "README.md"
 authors = [
     "Subham Agarwal <subhamagr@users.noreply.github.com>",
 ]
 maintainers = []
 # links
@@ -38,32 +38,31 @@
 ]
 exclude = [
     "**/tests/**/*.*",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typing_extensions = "4.10.0"
+typing_extensions = "4.11.0"
 pydantic = "2.7.1"
-pydantic-settings = "2.2.1"
 cryptography = "42.0.5"
 base58 = "2.1.1"
 pyjwt = "2.8.0"
 
 [tool.poetry.group.release.dependencies]
 python-semantic-release = "9.5.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "8.1.1"
+pytest = "8.2.0"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
 
 [tool.poetry.group.qa.dependencies]
-mypy = "1.9.0"
-ruff = "0.4.1"
+mypy = "1.10.0"
+ruff = "0.4.2"
 
 [tool.poetry.urls]
 # adding this section to avoid poetry formating issues
 "Bug Tracker" = "https://github.com/fileverse/py-ucan/issues"
 
 # ----------------------------------------------------------------------------------------------------------------------
 # ci::semantic_release
```

### Comparing `py_ucan-0.3.1/src/ucan/__init__.py` & `py_ucan-0.4.0/src/ucan/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,28 +7,63 @@
 import pydantic as pyd
 import pydantic.dataclasses
 
 from ucan.core import attenuation as attenuationlib
 from ucan.core import token as tokenlib
 from ucan.core import verify as verifylib
 from ucan.core.plugins import Plugins
+from ucan.core.types import (
+    Ability,
+    Capability,
+    ResourcePointer,
+    Ucan,
+    UcanHeader,
+    UcanParts,
+    UcanPayload,
+)
+from ucan.core.verify import (
+    RequiredCapability,
+    Verification,
+    VerifyResult,
+    VerifyResultError,
+    VerifyResultOk,
+)
 from ucan.default_plugins import ed25519_plugin, EdKeypair
 
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 
 __all__ = (
+    # attrs of this module
     "Plugins",
     "PluginInjectedAPI",
     "default_plugins",
     "injected_api",
+    "delegation_chains",
+    "validate",
+    "validate_proofs",
+    "verify",
     # plugins
     "EdKeypair",
     "ed25519_plugin",
+    # types
+    "Ability",
+    "Capability",
+    "ResourcePointer",
+    "Ucan",
+    "UcanHeader",
+    "UcanParts",
+    "UcanPayload",
+    # verify types
+    "RequiredCapability",
+    "Verification",
+    "VerifyResult",
+    "VerifyResultError",
+    "VerifyResultOk",
 )
 
 
 @pyd.dataclasses.dataclass(
     frozen=True,
     kw_only=True,
     config=pyd.ConfigDict(extra="forbid", frozen=True, arbitrary_types_allowed=True),
```

### Comparing `py_ucan-0.3.1/src/ucan/constants.py` & `py_ucan-0.4.0/src/ucan/constants.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.1/src/ucan/core/attenuation.py` & `py_ucan-0.4.0/src/ucan/core/attenuation.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.1/src/ucan/core/semver.py` & `py_ucan-0.4.0/src/ucan/core/semver.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.3.1/src/ucan/core/token.py` & `py_ucan-0.4.0/src/ucan/core/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             await plugins.verify_signature(
                 parsed.payload.iss, signed_data_bytes, signature_bytes
             )
 
         ucan = Ucan(
             header=parsed.header,
             payload=parsed.payload,
-            signedData=signed_data,
+            signed_data=signed_data,
             signature=encoded_signature,
         )
 
         if check_is_expired and is_expired(ucan):
             msg = f"Invalid UCAN: {encoded_ucan}: Expired."
             raise ValueError(msg)
 
@@ -173,29 +173,29 @@
                     )
                 if (
                     check_time_bounds_subset
                     and proof.payload.nbf is not None
                     and ucan.payload.exp > proof.payload.nbf
                 ):
                     yield ProofError(
-                        f"Invalid Proof: 'Not before' (${proof.payload.nbf}) is after parent's expiration (${ucan.payload.exp})"
+                        f"Invalid Proof: 'Not before' ({proof.payload.nbf}) is after parent's expiration ({ucan.payload.exp})"
                     )
 
                 if (
                     check_time_bounds_subset
                     and ucan.payload.nbf is not None
                     and ucan.payload.nbf > proof.payload.exp
                 ):
                     yield ProofError(
-                        f"Invalid Proof: Expiration (${proof.payload.exp}) is before parent's 'not before' (${ucan.payload.nbf})"
+                        f"Invalid Proof: Expiration ({proof.payload.exp}) is before parent's 'not before' ({ucan.payload.nbf})"
                     )
 
                 if check_version_monotonic and ucan.header.ucv.lt(proof.header.ucv):
                     yield ProofError(
-                        f"Invalid Proof: Version (${proof.header.ucv}) is higher "
+                        f"Invalid Proof: Version ({proof.header.ucv}) is higher "
                         f"than parent's version ({ucan.header.ucv})"
                     )
 
                 yield proof
 
             except ProofError as e:  # noqa: PERF203
                 yield e
```

### Comparing `py_ucan-0.3.1/src/ucan/core/types.py` & `py_ucan-0.4.0/src/ucan/core/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,101 +3,71 @@
 import abc
 import typing as t
 import typing_extensions as te
 
 import pydantic as pyd
 
 from ucan.core.semver import SemVer
-from ucan.schemas import BaseModel, T_BaseModel
+from ucan.schemas import BaseModel
 
 
 # Function types
 
 
 @te.runtime_checkable
-class SignatureVerifyFunc(te.Protocol):
-    async def __call__(self, did: str, data: bytes, signature: bytes) -> bool: ...
-
-
-@te.runtime_checkable
 class IsRevokedFunc(te.Protocol):
     async def __call__(self, ucan: Ucan) -> bool: ...
 
 
-# CRYPTOGRAPHY
-
-
-class Didable(abc.ABC):
-    @abc.abstractmethod
-    def did(self) -> str:
-        """Create a DID."""
-
-
-class Keypair(abc.ABC):
-    @property
-    @abc.abstractmethod
-    def jwt_alg(self) -> str:
-        """Algorithm."""
-
-    @abc.abstractmethod
-    def sign(self, msg: bytes) -> bytes:
-        """Sign a message `msg`."""
-
-
-class DidableKey(Didable, Keypair):
-    @property
-    @abc.abstractmethod
-    def prefix(self) -> bytes:
-        """DID prefix."""
-
-
-class ExportableKey(abc.ABC, t.Generic[T_BaseModel]):
-    @classmethod
-    @abc.abstractmethod
-    def import_key(cls, data: T_BaseModel) -> te.Self:
-        """Import a key."""
-
-    @abc.abstractmethod
-    def export(self) -> T_BaseModel:
-        """Export a key."""
-
-
-class DidKeyPlugin(BaseModel):
-    prefix: bytes
-    jwt_alg: str
-    # async func(did: str, data: bytes, signature: bytes) -> bool: ...
-    verify_signature: SignatureVerifyFunc
-
-
 # SCHEMAS
 
 
 class ResourcePointer(BaseModel):
     scheme: str
-    hier_part: str = pyd.Field(..., alias="hierPart")
+    hier_part: str = pyd.Field(alias="hierPart")
 
     SEPARATOR: t.ClassVar[str] = ":"
 
     @pyd.model_serializer
     def ser_model(self) -> dict[str, t.Any]:
         # https://github.com/pydantic/pydantic/issues/8379
         # for now, hard code the serializer
         return {"scheme": self.scheme, "hierPart": self.hier_part}
 
     @classmethod
     def from_string(cls, data: str) -> te.Self:
+        """Load ResourcePointer from string.
+
+        `data` must be in the format: {scheme}{SEPARATOR}{hier_part}.
+
+        Args:
+            data (str): string representation of ResourcePointer.
+
+        Raises:
+            TypeError: Expected {separater} in the value.
+
+        Returns:
+            te.Self: ResourcePointer object.
+        """
         parts = data.split(cls.SEPARATOR)
         if len(parts) < 2:  # noqa: PLR2004
             msg = f"Expected '{cls.SEPARATOR}' in the value"
             raise TypeError(msg)
 
-        return cls(scheme=parts[0], hierPart=cls.SEPARATOR.join(parts[1:]))
+        return cls(scheme=parts[0], hier_part=cls.SEPARATOR.join(parts[1:]))
 
     def encode(self) -> str:
-        return f"{self.scheme}${self.__class__.SEPARATOR}${self.hier_part}"
+        """Returns a string representation of the ResourcePointer.
+
+        The returned value is in the format: {scheme}{SEPARATOR}{hier_part}.
+
+        Returns:
+            str: String represenation of ResourcePointer.
+        """
+        return f"{self.scheme}{self.__class__.SEPARATOR}{self.hier_part}"
 
 
 class Ability(BaseModel):
     namespace: str
     segments: list[str]
 
     SEPARATOR: t.ClassVar[str] = "/"
@@ -112,15 +82,15 @@
         return cls(namespace=parts[0], segments=parts[1:])
 
     def encode(self) -> str:
         return self.__class__.SEPARATOR.join([self.namespace, *self.segments])
 
 
 class Capability(BaseModel):
-    with_: ResourcePointer = pyd.Field(..., alias="with")
+    with_: ResourcePointer = pyd.Field(alias="with")
     can: Ability
 
     @pyd.field_validator("with_", mode="before")
     def validate_with(cls, data: str | t.Any) -> ResourcePointer | t.Any:
         if isinstance(data, str):
             return ResourcePointer.from_string(data)
 
@@ -167,9 +137,20 @@
 class UcanParts(BaseModel):
     header: UcanHeader
     payload: UcanPayload
 
 
 class Ucan(UcanParts):
     # We need to keep the encoded version around to preserve the signature
-    signed_data: str = pyd.Field(..., alias="signedData")
+    signed_data: str = pyd.Field(alias="signedData")
     signature: str
+
+    @pyd.model_serializer
+    def ser_model(self) -> dict[str, t.Any]:
+        # https://github.com/pydantic/pydantic/issues/8379
+        # for now, hard code the serializer
+        return {
+            "header": self.header,
+            "payload": self.payload,
+            "signedData": self.signed_data,
+            "signature": self.signature,
+        }
```

### Comparing `py_ucan-0.3.1/src/ucan/core/verify.py` & `py_ucan-0.4.0/src/ucan/core/verify.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from ucan.schemas import BaseModel, DidString, validate_call
 
 
 __all__ = (
     # models
     "RequiredCapability",
     "Verification",
-    "ResultOk",
-    "ResultError",
-    "Result",
+    "VerifyResult",
+    "VerifyResultError",
+    "VerifyResultOk",
     # typing
     "VerifyTokenFunc",
     # utils
     "default_is_revoked",
     "verify",
 )
 
@@ -42,25 +42,25 @@
     root_issuer: DidString
 
 
 class Verification(RequiredCapability):
     proof: DelegationChain
 
 
-class ResultOk(BaseModel):
+class VerifyResultOk(BaseModel):
     ok: t.Literal[True]
     value: list[Verification]
 
 
-class ResultError(BaseModel):
+class VerifyResultError(BaseModel):
     ok: t.Literal[False]
     errors: list[Exception]
 
 
-Result = ResultOk | ResultError
+VerifyResult = VerifyResultOk | VerifyResultError
 
 
 # typing
 
 
 @te.runtime_checkable
 class VerifyTokenFunc(te.Protocol):
@@ -69,15 +69,15 @@
     async def __call__(
         self,
         encoded_ucan: str,
         audience: DidString,
         required_capabilities: list[RequiredCapability],
         semantics: DelegationSemantics | None = ...,
         is_revoked: IsRevokedFunc | None = ...,
-    ) -> Result: ...
+    ) -> VerifyResult: ...
 
 
 # utils
 
 
 async def default_is_revoked(ucan: Ucan) -> bool:  # noqa: ARG001
     """Assumes all tokens are valid.
@@ -96,15 +96,15 @@
     @validate_call
     async def _verify_inner(
         encoded_ucan: str,
         audience: DidString,
         required_capabilities: list[RequiredCapability],
         semantics: DelegationSemantics | None = None,
         is_revoked: IsRevokedFunc | None = None,
-    ) -> Result:
+    ) -> VerifyResult:
         """Verify a UCAN for an invocation.
 
         Args:
             encoded_ucan (str): a UCAN to verify for invocation in JWT format.
                 (starts with 'eyJ...' and has two '.' in it)
             audience (str): the DID of the callee of this function.
                 The expected audience of the outermost level of the UCAN.
@@ -136,16 +136,16 @@
 
         try:
             # Verify the UCAN
             ucan = await tokenlib.validate(plugins)(encoded_ucan)
 
             if ucan.payload.aud != audience:
                 msg = (
-                    f"Invalid UCAN: Expected audience to be ${audience}, "
-                    f"but it's ${ucan.payload.aud}"
+                    f"Invalid UCAN: Expected audience to be {audience}, "
+                    f"but it's {ucan.payload.aud}"
                 )
                 raise ValueError(msg)  # noqa: TRY301
 
             errors: list[Exception] = []
             proven: list[Verification] = []
             remaining = required_capabilities.copy()
             async for chain_item in delegation_chains(plugins)(
@@ -173,19 +173,19 @@
                         )
 
                 # If we've already verified all, we don't need to keep looking
                 if not remaining:
                     break
 
             return (
-                ResultError(ok=False, errors=errors)
+                VerifyResultError(ok=False, errors=errors)
                 if len(remaining) > 0
-                else ResultOk(ok=True, value=proven)
+                else VerifyResultOk(ok=True, value=proven)
             )
 
         except Exception as e:
-            return ResultError(
+            return VerifyResultError(
                 ok=False,
                 errors=[Exception(f"Unknown error during UCAN verification: {e}")],
             )
 
     return _verify_inner
```

### Comparing `py_ucan-0.3.1/src/ucan/default_plugins/ed25519.py` & `py_ucan-0.4.0/src/ucan/default_plugins/ed25519.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Ed25519PrivateKey as PrivateKey,
 )
 from cryptography.hazmat.primitives.asymmetric.ed25519 import (
     Ed25519PublicKey as PublicKey,
 )
 
 from ucan.constants import PREFIX_DID_ALG_ED25519
-from ucan.core.types import DidableKey, DidKeyPlugin, ExportableKey
+from ucan.core.plugins import DidableKey, DidKeyPlugin, ExportableKey
 from ucan.schemas import BaseModel
 from ucan.utils import did_from_key_bytes, did_to_key_bytes
 
 
 __all__ = (
     "EdKeypair",
     "ed25519_plugin",
```

### Comparing `py_ucan-0.3.1/src/ucan/schemas.py` & `py_ucan-0.4.0/src/ucan/schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 
 
 # base model
 class BaseModel(pyd.BaseModel):
     """base pydantic model class."""
 
     model_config = pyd.ConfigDict(
-        strict=True,
+        strict=False,
         frozen=True,
         arbitrary_types_allowed=True,
-        use_enum_values=False,
         validate_assignment=True,
         extra="forbid",
         revalidate_instances="always",
         validate_default=True,
         validate_return=True,
-        hide_input_in_errors=True,
         from_attributes=False,
         populate_by_name=True,
         coerce_numbers_to_str=False,
     )
 
 
 # Custom Pydantic Fields
```

### Comparing `py_ucan-0.3.1/src/ucan/utils.py` & `py_ucan-0.4.0/src/ucan/utils.py`

 * *Files identical despite different names*

