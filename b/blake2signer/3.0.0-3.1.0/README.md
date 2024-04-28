# Comparing `tmp/blake2signer-3.0.0.tar.gz` & `tmp/blake2signer-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blake2signer-3.0.0.tar", max compression
+gzip compressed data, was "blake2signer-3.1.0.tar", max compression
```

## Comparing `blake2signer-3.0.0.tar` & `blake2signer-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    16725 2024-01-25 22:20:20.597646 blake2signer-3.0.0/LICENSE
--rw-r--r--   0        0        0    10947 2024-01-25 22:20:20.598646 blake2signer-3.0.0/README.md
--rw-r--r--   0        0        0     1769 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/__init__.py
--rw-r--r--   0        0        0    29686 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/bases.py
--rw-r--r--   0        0        0     1906 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/compressors.py
--rw-r--r--   0        0        0     2412 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/encoders.py
--rw-r--r--   0        0        0     6308 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/errors.py
--rw-r--r--   0        0        0      528 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/hashers/__init__.py
--rw-r--r--   0        0        0      756 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/hashers/blake3_package.py
--rw-r--r--   0        0        0     9161 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/hashers/blakehashers.py
--rw-r--r--   0        0        0     4115 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/interfaces.py
--rw-r--r--   0        0        0    12838 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/mixins.py
--rw-r--r--   0        0        0        0 2024-01-25 22:20:20.630646 blake2signer-3.0.0/blake2signer/py.typed
--rw-r--r--   0        0        0     1799 2024-01-25 22:20:20.598646 blake2signer-3.0.0/blake2signer/serializers.py
--rw-r--r--   0        0        0    39413 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/signers.py
--rw-r--r--   0        0        0       29 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/tests/__init__.py
--rw-r--r--   0        0        0    35779 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/tests/bases.py
--rw-r--r--   0        0        0     9140 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/tests/test_hashers.py
--rw-r--r--   0        0        0    54961 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/tests/test_serializersigner.py
--rw-r--r--   0        0        0     6357 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/tests/test_signer.py
--rw-r--r--   0        0        0    19091 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/tests/test_timestampsigner.py
--rw-r--r--   0        0        0     4666 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/tests/test_utils.py
--rw-r--r--   0        0        0     3761 2024-01-25 22:20:20.599646 blake2signer-3.0.0/blake2signer/utils.py
--rw-r--r--   0        0        0     3326 2024-01-25 22:20:20.605646 blake2signer-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    12732 1970-01-01 00:00:00.000000 blake2signer-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-04-28 19:12:04.945084 blake2signer-3.1.0/LICENSE
+-rw-r--r--   0        0        0    10945 2024-04-28 19:12:04.945084 blake2signer-3.1.0/README.md
+-rw-r--r--   0        0        0     1767 2024-04-28 19:12:04.945084 blake2signer-3.1.0/blake2signer/__init__.py
+-rw-r--r--   0        0        0    29724 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/bases.py
+-rw-r--r--   0        0        0     1906 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/compressors.py
+-rw-r--r--   0        0        0     3308 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/encoders.py
+-rw-r--r--   0        0        0     6308 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/errors.py
+-rw-r--r--   0        0        0      528 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/hashers/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/hashers/blake3_package.py
+-rw-r--r--   0        0        0     9161 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/hashers/blakehashers.py
+-rw-r--r--   0        0        0     4115 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/interfaces.py
+-rw-r--r--   0        0        0    12838 2024-04-28 19:12:04.946084 blake2signer-3.1.0/blake2signer/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:12:04.979085 blake2signer-3.1.0/blake2signer/py.typed
+-rw-r--r--   0        0        0     1799 2024-04-28 19:12:04.947084 blake2signer-3.1.0/blake2signer/serializers.py
+-rw-r--r--   0        0        0    39413 2024-04-28 19:12:04.947084 blake2signer-3.1.0/blake2signer/signers.py
+-rw-r--r--   0        0        0       29 2024-04-28 19:12:04.947084 blake2signer-3.1.0/blake2signer/tests/__init__.py
+-rw-r--r--   0        0        0    35935 2024-04-28 19:12:04.947084 blake2signer-3.1.0/blake2signer/tests/bases.py
+-rw-r--r--   0        0        0     9709 2024-04-28 19:12:04.947084 blake2signer-3.1.0/blake2signer/tests/test_hashers.py
+-rw-r--r--   0        0        0    53214 2024-04-28 19:12:04.947084 blake2signer-3.1.0/blake2signer/tests/test_serializersigner.py
+-rw-r--r--   0        0        0     6357 2024-04-28 19:12:04.948084 blake2signer-3.1.0/blake2signer/tests/test_signer.py
+-rw-r--r--   0        0        0    15662 2024-04-28 19:12:04.948084 blake2signer-3.1.0/blake2signer/tests/test_timestampsigner.py
+-rw-r--r--   0        0        0     6713 2024-04-28 19:12:04.948084 blake2signer-3.1.0/blake2signer/tests/test_utils.py
+-rw-r--r--   0        0        0     5820 2024-04-28 19:12:04.948084 blake2signer-3.1.0/blake2signer/utils.py
+-rw-r--r--   0        0        0     3326 2024-04-28 19:12:04.954084 blake2signer-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12730 1970-01-01 00:00:00.000000 blake2signer-3.1.0/PKG-INFO
```

### Comparing `blake2signer-3.0.0/LICENSE` & `blake2signer-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/README.md` & `blake2signer-3.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 * [Erus](https://gitlab.com/erudin): docs title logo, code review.
 * [NoonSleeper](https://gitlab.com/noonsleeper): project icons.
 
 ## License
 
 **Blake2Signer** is made by [HacKan](https://hackan.net) under MPL v2.0. You are free to use, share, modify and share modifications under the terms of that [license](LICENSE).  Derived works may link back to the canonical repository: `https://gitlab.com/hackancuba/blake2signer`.
 
-    Copyright (C) 2020 - 2024 HacKan (https://hackan.net)
+    Copyright (C) 2020-2024 HacKan (https://hackan.net)
     This Source Code Form is subject to the terms of the Mozilla Public
     License, v. 2.0. If a copy of the MPL was not distributed with this
     file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 ----
 
 [![CC BY-SA 4.0](https://i.creativecommons.org/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) *Blake2Signer icons* by [NoonSleeper](https://gitlab.com/noonsleeper) are licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/). You are free to use, share, modify and share modifications under the terms of that [license](https://creativecommons.org/licenses/by-sa/4.0/). They were based on *Blake2Signer logo* by [HacKan](https://hackan.net) which was based on [this sword](https://thenounproject.com/term/samurai-sword/2044449/) by *Hamza Wahbi* and [this signature](https://thenounproject.com/term/sign/184638/) by *Nick Bluth*, both licensed under [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/), and inspired by [It's dangerous logo](https://itsdangerous.palletsprojects.com/en/1.1.x/_images/itsdangerous-logo.png).
```

### Comparing `blake2signer-3.0.0/blake2signer/__init__.py` & `blake2signer-3.1.0/blake2signer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
-# by HacKan (https://hackan.net), 2020 - 2024.
+# by HacKan (https://hackan.net), 2020-2024.
 # This software is provided as-is. You are free to use, share, modify
 # and share modifications under the terms of that license, even with
 # proprietary code. Attribution is not required to share but is
 # appreciated.
 """Blake2Signer: use BLAKE in keyed hashing mode to sign and verify signed data.
 
 The goal of this module is to provide a simple way to securely sign data and the
@@ -29,15 +29,15 @@
 from . import errors
 from .signers import Blake2SerializerSigner
 from .signers import Blake2Signature
 from .signers import Blake2SignatureDump
 from .signers import Blake2Signer
 from .signers import Blake2TimestampSigner
 
-__version__ = '3.0.0'
+__version__ = '3.1.0'
 
 __all__ = (
     'errors',
     'Blake2SerializerSigner',
     'Blake2Signature',
     'Blake2SignatureDump',
     'Blake2Signer',
```

### Comparing `blake2signer-3.0.0/blake2signer/bases.py` & `blake2signer-3.1.0/blake2signer/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import os
 import typing
 from abc import ABC
 from abc import abstractmethod
 from datetime import timedelta
 from secrets import compare_digest
-from time import time
 
 from .encoders import B64URLEncoder
 from .errors import ExpiredSignatureError
 from .errors import FileError
 from .errors import InvalidOptionError
 from .errors import InvalidSignatureError
 from .errors import SignatureError
@@ -18,14 +17,15 @@
 from .hashers import BLAKE3Hasher
 from .hashers import BLAKEHasher
 from .hashers import HasherChoice
 from .interfaces import EncoderInterface
 from .mixins import EncoderMixin
 from .mixins import Mixin
 from .utils import file_mode_is_text
+from .utils import get_current_time
 from .utils import ordinal
 from .utils import timestamp_to_aware_datetime
 
 
 class SignedDataParts(typing.NamedTuple):
     """Parts of a signed data container."""
 
@@ -482,15 +482,15 @@
 
 
 class Blake2TimestampSignerBase(Blake2SignerBase, ABC):
     """Base class for a timestamp signer based on BLAKE in keyed hashing mode."""
 
     def _get_timestamp(self) -> bytes:
         """Get the encoded timestamp value."""
-        timestamp = int(time())  # It's easier to encode and decode an integer
+        timestamp = int(get_current_time())  # It's easier to encode and decode an integer
         try:
             timestamp_b = timestamp.to_bytes(4, 'big', signed=False)
         except OverflowError as exc:  # This will happen in ~2106-02-07
             raise RuntimeError(
                 'can not represent this timestamp in bytes: this library is '
                 + 'too old and needs to be updated!',
             ) from exc
@@ -595,15 +595,15 @@
         timestamped_data = self._unsign(parts)
 
         timestamped_parts = self._decompose_timestamp(timestamped_data)
 
         if max_age is None:
             return timestamped_parts.data
 
-        now = time()
+        now = get_current_time()
         age = now - timestamped_parts.timestamp
         ttl = self._get_ttl_from_max_age(max_age)
 
         if age > ttl:
             raise ExpiredSignatureError(
                 f'signature has expired, age {age} > {ttl} seconds',
                 timestamp=timestamp_to_aware_datetime(timestamped_parts.timestamp),
```

### Comparing `blake2signer-3.0.0/blake2signer/compressors.py` & `blake2signer-3.1.0/blake2signer/compressors.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/encoders.py` & `blake2signer-3.1.0/blake2signer/encoders.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Encoders: classes that implement the EncoderInterface."""
 
 from .interfaces import EncoderInterface
+from .utils import B58_ALPHABET
 from .utils import b32decode
 from .utils import b32encode
+from .utils import b58decode
+from .utils import b58encode
 from .utils import b64decode
 from .utils import b64encode
 from .utils import hexdecode
 from .utils import hexencode
 
 
 class B64URLEncoder(EncoderInterface):
@@ -96,7 +99,42 @@
         Args:
             data: Data to decode.
 
         Returns:
             Original data.
         """
         return hexdecode(data)
+
+
+class B58Encoder(EncoderInterface):
+    """Base58 encoder.
+
+    It contains characters from a-z (except `l`), A-Z (except `I` and `O`), and numbers 1-9,
+    to improve readability and reduce transcription errors.
+    """
+
+    @property
+    def alphabet(self) -> bytes:
+        """Return the encoder alphabet characters."""
+        return B58_ALPHABET
+
+    def encode(self, data: bytes) -> bytes:
+        """Encode given data to base58.
+
+        Args:
+            data: Data to encode.
+
+        Returns:
+            Encoded data.
+        """
+        return b58encode(data)
+
+    def decode(self, data: bytes) -> bytes:
+        """Decode given encoded data from base58.
+
+        Args:
+            data: Data to decode.
+
+        Returns:
+            Original data.
+        """
+        return b58decode(data)
```

### Comparing `blake2signer-3.0.0/blake2signer/errors.py` & `blake2signer-3.1.0/blake2signer/errors.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/hashers/__init__.py` & `blake2signer-3.1.0/blake2signer/hashers/__init__.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/hashers/blake3_package.py` & `blake2signer-3.1.0/blake2signer/hashers/blake3_package.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/hashers/blakehashers.py` & `blake2signer-3.1.0/blake2signer/hashers/blakehashers.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/interfaces.py` & `blake2signer-3.1.0/blake2signer/interfaces.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/mixins.py` & `blake2signer-3.1.0/blake2signer/mixins.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/serializers.py` & `blake2signer-3.1.0/blake2signer/serializers.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/signers.py` & `blake2signer-3.1.0/blake2signer/signers.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/tests/bases.py` & `blake2signer-3.1.0/blake2signer/tests/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from .. import errors
 from ..bases import Blake2Signature
 from ..bases import Blake2SignatureDump
 from ..bases import HasherChoice
 from ..bases import Secret
 from ..encoders import B32Encoder
+from ..encoders import B58Encoder
 from ..encoders import B64URLEncoder
 from ..encoders import HexEncoder
 from ..hashers import BLAKE2Hasher
 from ..hashers import BLAKE3Hasher
 from ..hashers import BLAKEHasher
 from ..hashers import has_blake3
 from ..interfaces import EncoderInterface
@@ -602,14 +603,15 @@
     )
     @pytest.mark.parametrize(
         ('encoder', 'regex'),
         (
             (B64URLEncoder, r'^[a-zA-Z0-9_\-]+(\.[a-zA-Z0-9_\-]+)?\.datadata$'),
             (B32Encoder, r'^[A-Z2-7]+(\.[A-Z2-7]+)?\.datadata$'),
             (HexEncoder, r'^[A-F0-9]+(\.[A-F0-9]+)?\.datadata$'),
+            (B58Encoder, r'^[1-9A-HJ-NP-Za-km-z]+(\.[1-9A-HJ-NP-Za-km-z]+)?\.datadata$'),
         ),
     )
     def test_sign_unsign_with_encoder(
         self,
         encoder: typing.Type[EncoderInterface],
         regex: str,
         hasher: HasherChoice,
@@ -869,14 +871,15 @@
     )
     @pytest.mark.parametrize(
         ('encoder', 'separator'),
         (
             (B64URLEncoder, b'A'),
             (B32Encoder, b'A'),
             (HexEncoder, b'A'),
+            (B58Encoder, b'A'),
         ),
     )
     def test_separator_in_encoder_alphabet(
         self,
         encoder: typing.Type[EncoderInterface],
         separator: bytes,
         hasher: HasherChoice,
```

### Comparing `blake2signer-3.0.0/blake2signer/tests/test_hashers.py` & `blake2signer-3.1.0/blake2signer/tests/test_hashers.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         # Ensure keys are actually derived
         with mock.patch.object(self.hasher_class, '_derive_key') as mock_derive_key:
             hasher = self.get_hasher(choice)
 
         person = hasher._person  # pylint: disable=W0212
         calls = [mock.call(secret, person=person) for secret in self.secrets]
         mock_derive_key.assert_has_calls(calls)
+        assert len(calls) == mock_derive_key.call_count
 
         # Ensure the hasher gets called properly
         hasher_to_patch = f'blake2signer.hashers.blakehashers.hashlib.{choice.value}'
         with mock.patch(hasher_to_patch) as mock_hasher:
             mock_hasher.PERSON_SIZE = 8
             mock_hasher.MAX_KEY_SIZE = 12
             mock_hasher.MAX_DIGEST_SIZE = 16
@@ -128,14 +129,17 @@
             self.get_hasher(choice)
 
         calls = [mock.call(self.person, digest_size=8), mock.call().digest()]
         for secret in self.secrets:
             calls.append(mock.call(secret, digest_size=12, person=b'abc123'))
             calls.append(mock.call().digest())
         mock_hasher.assert_has_calls(calls)
+        expected_call_count = len(calls) // 2
+        assert expected_call_count == mock_hasher.call_count
+        assert expected_call_count == mock_hasher.return_value.digest.call_count
 
     @pytest.mark.parametrize(
         ('choice', 'data', 'salt', 'expected_digest'),
         (
             (
                 HasherChoice.blake2b,
                 b'datadata',
@@ -235,28 +239,33 @@
         # Ensure keys are actually derived
         with mock.patch.object(self.hasher_class, '_derive_key') as mock_derive_key:
             hasher = self.get_hasher()
 
         person = hasher._person  # pylint: disable=W0212
         calls = [mock.call(secret, person=person) for secret in self.secrets]
         mock_derive_key.assert_has_calls(calls)
+        assert len(calls) == mock_derive_key.call_count
 
         # Ensure the hasher gets called properly
         with mock.patch('blake2signer.hashers.blakehashers.blake3') as mock_hasher:
             mock_hasher.return_value.key_size = 16
 
             self.get_hasher()
 
         calls = []  # person is not derived
         derive_key_context = 'blake2signer 2021-12-29 18:04:37 BLAKE3Hasher key derivation'
         for secret in self.secrets:
             calls.append(mock.call(secret, derive_key_context=derive_key_context))
             calls.append(mock.call().update(self.person))
             calls.append(mock.call().digest(length=16))
         mock_hasher.assert_has_calls(calls)
+        expected_call_count = len(calls) // 3
+        assert expected_call_count == mock_hasher.call_count
+        assert expected_call_count == mock_hasher.return_value.update.call_count
+        assert expected_call_count == mock_hasher.return_value.digest.call_count
 
     @pytest.mark.parametrize(
         ('data', 'salt', 'expected_digest'),
         (
             (b'datadata', b'', b"\xfe\x88\x96\xe5\xdf:\xb6f\xe1}\x9f\x18\x9a'\xad\x8d"),
             (b'datadata', b'salt', b'\xeez6\xf20\xca\xcae\x93\xc3\xcchh\x90(\xdf'),
         ),
```

### Comparing `blake2signer-3.0.0/blake2signer/tests/test_serializersigner.py` & `blake2signer-3.1.0/blake2signer/tests/test_serializersigner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 import io
 import json
 import typing
 import zlib
 from abc import ABC
 from datetime import timedelta
+from math import isclose
 from secrets import token_bytes
-from time import time
 from unittest import mock
 
 import pytest
 
 from .bases import BaseTests
 from .bases import Signature
 from .bases import Signer
 from .test_timestampsigner import TimestampSignerTestsBase
 from .. import errors
+from ..bases import Secret
 from ..compressors import GzipCompressor
 from ..compressors import ZlibCompressor
 from ..encoders import B32Encoder
+from ..encoders import B58Encoder
 from ..encoders import B64URLEncoder
 from ..encoders import HexEncoder
 from ..hashers import HasherChoice
 from ..hashers import has_blake3
 from ..interfaces import CompressorInterface
 from ..interfaces import EncoderInterface
 from ..serializers import JSONSerializer
@@ -140,14 +142,18 @@
     )
     @pytest.mark.parametrize(
         ('encoder', 'regex'),
         (
             (B64URLEncoder, r'^[a-zA-Z0-9_\-]+(\.[a-zA-Z0-9_\-]+)?\.[a-zA-Z0-9_\-]+$'),
             (B32Encoder, r'^[A-Z2-7]+(\.[A-Z2-7]+)?\.[A-Z2-7]+$'),
             (HexEncoder, r'^[A-F0-9]+(\.[A-F0-9]+)?\.[A-F0-9]+$'),
+            (
+                B58Encoder,
+                r'^[1-9A-HJ-NP-Za-km-z]+(\.[1-9A-HJ-NP-Za-km-z]+)?\.[1-9A-HJ-NP-Za-km-z]+$',
+            ),
         ),
     )
     def test_sign_unsign_with_encoder(
         self,
         encoder: typing.Type[EncoderInterface],
         regex: str,
         hasher: HasherChoice,
@@ -705,39 +711,38 @@
             hasher=hasher,
         )
         data = {
             'a': 'b',
             1: 2,
         }
 
-        with mock.patch('blake2signer.bases.time', return_value=time()):
-            signed1 = self.sign(
-                signer,
-                data,
-                serializer_kwargs={
-                    'separators': ('.', ';'),
-                },
-            )
-            signed1_1 = self.sign(
-                signer,
-                data,
-                serializer_kwargs={
-                    'separators': ('.', ';'),
-                },
-            )
-            assert signed1 == signed1_1  # It is effectively deterministic
-
-            signed2 = self.sign(
-                signer,
-                data,
-                serializer_kwargs={
-                    'separators': ('.', ','),
-                },
-            )
-            assert signed1 != signed2  # Change due only to the serializer options
+        signed1 = self.sign(
+            signer,
+            data,
+            serializer_kwargs={
+                'separators': ('.', ';'),
+            },
+        )
+        signed1_1 = self.sign(
+            signer,
+            data,
+            serializer_kwargs={
+                'separators': ('.', ';'),
+            },
+        )
+        assert signed1 == signed1_1  # It is effectively deterministic
+
+        signed2 = self.sign(
+            signer,
+            data,
+            serializer_kwargs={
+                'separators': ('.', ','),
+            },
+        )
+        assert signed1 != signed2  # Change due only to the serializer options
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
@@ -759,43 +764,42 @@
             hasher=hasher,
         )
         data = {
             'a': 'b',
             1: 2,
         }
 
-        with mock.patch('blake2signer.bases.time', return_value=time()):
-            signer.dump(
-                data,
-                file1,
-                serializer_kwargs={
-                    'separators': ('.', ';'),
-                },
-            )
-            signer.dump(
-                data,
-                file1_1,
-                serializer_kwargs={
-                    'separators': ('.', ';'),
-                },
-            )
-            file1.seek(0)
-            file1_1.seek(0)
-            assert file1.read() == file1_1.read()  # It is effectively deterministic
-
-            signer.dump(
-                data,
-                file2,
-                serializer_kwargs={
-                    'separators': ('.', ','),
-                },
-            )
-            file1.seek(0)
-            file2.seek(0)
-            assert file1.read() != file2.read()  # Change due only to the serializer options
+        signer.dump(
+            data,
+            file1,
+            serializer_kwargs={
+                'separators': ('.', ';'),
+            },
+        )
+        signer.dump(
+            data,
+            file1_1,
+            serializer_kwargs={
+                'separators': ('.', ';'),
+            },
+        )
+        file1.seek(0)
+        file1_1.seek(0)
+        assert file1.read() == file1_1.read()  # It is effectively deterministic
+
+        signer.dump(
+            data,
+            file2,
+            serializer_kwargs={
+                'separators': ('.', ','),
+            },
+        )
+        file1.seek(0)
+        file2.seek(0)
+        assert file1.read() != file2.read()  # Change due only to the serializer options
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
@@ -814,39 +818,38 @@
             hasher=hasher,
         )
         data = {
             'a': 'b',
             1: 2,
         }
 
-        with mock.patch('blake2signer.bases.time', return_value=time()):
-            signed1 = self.sign_parts(
-                signer,
-                data,
-                serializer_kwargs={
-                    'separators': ('.', ';'),
-                },
-            )
-            signed1_1 = self.sign_parts(
-                signer,
-                data,
-                serializer_kwargs={
-                    'separators': ('.', ';'),
-                },
-            )
-            assert signed1 == signed1_1  # It is effectively deterministic
-
-            signed2 = self.sign_parts(
-                signer,
-                data,
-                serializer_kwargs={
-                    'separators': ('.', ','),
-                },
-            )
-            assert signed1 != signed2  # Change due only to the serializer options
+        signed1 = self.sign_parts(
+            signer,
+            data,
+            serializer_kwargs={
+                'separators': ('.', ';'),
+            },
+        )
+        signed1_1 = self.sign_parts(
+            signer,
+            data,
+            serializer_kwargs={
+                'separators': ('.', ';'),
+            },
+        )
+        assert signed1 == signed1_1  # It is effectively deterministic
+
+        signed2 = self.sign_parts(
+            signer,
+            data,
+            serializer_kwargs={
+                'separators': ('.', ','),
+            },
+        )
+        assert signed1 != signed2  # Change due only to the serializer options
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
@@ -1139,14 +1142,15 @@
     )
     @pytest.mark.parametrize(
         ('encoder', 'flag'),
         (
             (B64URLEncoder, b'A'),
             (B32Encoder, b'A'),
             (HexEncoder, b'A'),
+            (B58Encoder, b'A'),
         ),
     )
     def test_compression_flag_in_encoder_alphabet(
         self,
         encoder: typing.Type[EncoderInterface],
         flag: bytes,
         hasher: HasherChoice,
@@ -1264,21 +1268,31 @@
         TimestampSignerTestsBase,
         SerializerSignerTestsBase,
 ):
     """Blake2SerializerSigner tests with timestamp."""
 
     def signer(
         self,
-        secret: typing.Union[None, str, bytes] = None,
+        secret: typing.Union[Secret, typing.Sequence[Secret], None] = None,
         **kwargs: typing.Any,
     ) -> Signer:
         """Get the signer to test."""
         kwargs.setdefault('max_age', 5)
+
         return super().signer(secret, **kwargs)
 
+    @staticmethod
+    def get_expired_signature_error_data(
+        exc: errors.ExpiredSignatureError,
+        *,
+        signer: Signer,
+    ) -> typing.Any:
+        """Get expired signature error data."""
+        return signer.data_from_exc(exc)
+
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
         'hasher',
@@ -1288,43 +1302,40 @@
             HasherChoice.blake3,
         ),
     )
     @pytest.mark.parametrize(
         'max_age',
         (None, 2, 2.5, timedelta(hours=2)),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_max_age_can_be_changed(
         self,
-        mock_time: mock.MagicMock,
         max_age: typing.Union[None, int, float, timedelta],
         hasher: HasherChoice,
     ) -> None:
         """Test that max age can be changed correctly."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(max_age=max_age, hasher=hasher)
-
         signed = self.sign(signer, self.data)
+
         assert self.data == self.unsign(signer, signed)
 
         if max_age:
             if isinstance(max_age, timedelta):
-                mock_time.return_value += max_age.total_seconds()
+                self.mock_time.return_value += max_age.total_seconds()
             else:
-                mock_time.return_value += max_age
-            mock_time.return_value += 0.1  # It has to be a bit bigger than max_age
+                self.mock_time.return_value += max_age
+            self.mock_time.return_value += 0.1  # It has to be a bit bigger than max_age
 
             with pytest.raises(
                     errors.ExpiredSignatureError,
                     match='signature has expired',
             ) as exc:
                 self.unsign(signer, signed)
+
             assert exc.value.__cause__ is None
-            assert exc.value.timestamp.timestamp() == timestamp
+            assert isclose(self.now, exc.value.timestamp.timestamp())
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
@@ -1459,72 +1470,32 @@
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
-    def test_sign_unsign_timestamp_expired(
-        self,
-        mock_time: mock.MagicMock,
-        hasher: HasherChoice,
-    ) -> None:
-        """Test unsigning with timestamp is correct."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
-        signer = self.signer(self.secret, hasher=hasher)
-
-        signed = self.sign(signer, self.data)
-
-        mock_time.return_value += 10
-        with pytest.raises(
-                errors.ExpiredSignatureError,
-                match='signature has expired',
-        ) as exc:
-            self.unsign(signer, signed)
-        assert exc.value.__cause__ is None
-        assert timestamp == exc.value.timestamp.timestamp()
-        assert b'ImRhdGFkYXRhIg' == exc.value.data  # serialized+encoded data
-        assert self.data == signer.data_from_exc(exc.value)
-
-    @pytest.mark.xfail(
-        not has_blake3(),
-        reason='blake3 is not installed',
-        raises=errors.MissingDependencyError,
-    )
-    @pytest.mark.parametrize(
-        'hasher',
-        (
-            HasherChoice.blake2b,
-            HasherChoice.blake2s,
-            HasherChoice.blake3,
-        ),
-    )
-    @mock.patch('blake2signer.bases.time')
     def test_data_from_exc_with_null_serializer(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test that data_from_exc works with a NullSerializer."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(self.secret, hasher=hasher, serializer=NullSerializer)
         data = b'datadata'
         signed = self.sign(signer, data)
 
-        mock_time.return_value += 10
+        self.mock_time.return_value += 10
         with pytest.raises(
                 errors.ExpiredSignatureError,
                 match='signature has expired',
         ) as exc:
             self.unsign(signer, signed)
+
         assert exc.value.__cause__ is None
-        assert timestamp == exc.value.timestamp.timestamp()
+        assert isclose(self.now, exc.value.timestamp.timestamp())
         assert data == signer.data_from_exc(exc.value)
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
@@ -1532,35 +1503,32 @@
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_data_from_exc_with_null_serializer_with_compression(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test that data_from_exc works with compression."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(self.secret, hasher=hasher, serializer=NullSerializer)
         data = b'datadatadatadata'
         signed = self.sign(signer, data, force_compression=True)
 
-        mock_time.return_value += 10
+        self.mock_time.return_value += 10
         with pytest.raises(
                 errors.ExpiredSignatureError,
                 match='signature has expired',
         ) as exc:
             self.unsign(signer, signed)
+
         assert exc.value.__cause__ is None
-        assert timestamp == exc.value.timestamp.timestamp()
+        assert isclose(self.now, exc.value.timestamp.timestamp())
         assert data == signer.data_from_exc(exc.value)
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
@@ -1568,61 +1536,60 @@
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_data_from_exc_raises_exceptions(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test that data_from_exc raises exceptions."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(
             self.secret,
             hasher=hasher,
             compressor=ZlibCompressor,
             serializer=JSONSerializer,
             encoder=B64URLEncoder,
         )
         signed = self.sign(signer, self.data_compressible, force_compression=True)
 
-        mock_time.return_value += 10
+        self.mock_time.return_value += 10
         with pytest.raises(
                 errors.ExpiredSignatureError,
                 match='signature has expired',
         ) as expired_sig_exc:
             self.unsign(signer, signed)
 
         with mock.patch('blake2signer.compressors.zlib.decompress', side_effect=zlib.error):
             with pytest.raises(
                     errors.DecompressionError,
                     match='data can not be decompressed',
             ) as exc:
                 signer.data_from_exc(expired_sig_exc.value)
+
             assert isinstance(exc.value.__cause__, zlib.error)
 
         with mock.patch('blake2signer.serializers.json.loads', side_effect=ValueError):
             with pytest.raises(
                     errors.UnserializationError,
                     match='data can not be unserialized',
             ) as exc:
                 signer.data_from_exc(expired_sig_exc.value)
+
             assert isinstance(exc.value.__cause__, ValueError)
 
         with mock.patch('blake2signer.utils.base64.urlsafe_b64decode', side_effect=TypeError):
             with pytest.raises(
                     errors.DecodeError,
                     match='data can not be decoded',
             ) as exc:
                 signer.data_from_exc(expired_sig_exc.value)
+
             assert isinstance(exc.value.__cause__, TypeError)
 
 
 class TestsBlake2SerializerSigner(SerializerSignerTestsBase):
     """Blake2SerializerSigner tests (without timestamp)."""
 
     def test_sign_unsign_with_different_signer(self) -> None:
```

### Comparing `blake2signer-3.0.0/blake2signer/tests/test_signer.py` & `blake2signer-3.1.0/blake2signer/tests/test_signer.py`

 * *Files identical despite different names*

### Comparing `blake2signer-3.0.0/blake2signer/tests/test_timestampsigner.py` & `blake2signer-3.1.0/blake2signer/tests/test_timestampsigner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Timestamp signers tests."""
 # pylint: disable=R0801
 
 import typing
 from abc import ABC
-from abc import abstractmethod
 from datetime import timedelta
-from time import time
+from math import isclose
 from unittest import mock
 
 import pytest
 
 from .bases import BaseTests
 from .bases import Signature
 from .bases import Signer
@@ -20,213 +19,128 @@
 from ..signers import Blake2Signer
 from ..signers import Blake2TimestampSigner
 
 
 class TimestampSignerTestsBase(BaseTests, ABC):
     """Base to test a timestamp signer."""
 
-    @pytest.mark.xfail(
-        not has_blake3(),
-        reason='blake3 is not installed',
-        raises=errors.MissingDependencyError,
-    )
-    @pytest.mark.parametrize(
-        'hasher',
-        (
-            HasherChoice.blake2b,
-            HasherChoice.blake2s,
-            HasherChoice.blake3,
-        ),
-    )
-    @mock.patch('blake2signer.bases.time')
-    def test_sign_unsign_deterministic(  # pylint: disable=W0221
-        self,
-        mock_time: mock.MagicMock,
-        hasher: HasherChoice,
-    ) -> None:
-        """Test sign and unsign with a deterministic signature."""
-        mock_time.return_value = time()
-
-        super().test_sign_unsign_deterministic(hasher)
-
-    @pytest.mark.xfail(
-        not has_blake3(),
-        reason='blake3 is not installed',
-        raises=errors.MissingDependencyError,
-    )
-    @pytest.mark.parametrize(
-        'hasher',
-        (
-            HasherChoice.blake2b,
-            HasherChoice.blake2s,
-            HasherChoice.blake3,
-        ),
-    )
-    @mock.patch('blake2signer.bases.time')
-    def test_sign_unsign_parts_deterministic(  # pylint: disable=W0221
-        self,
-        mock_time: mock.MagicMock,
-        hasher: HasherChoice,
-    ) -> None:
-        """Test signing and unsigning in parts deterministically."""
-        mock_time.return_value = time()
-
-        super().test_sign_unsign_parts_deterministic(hasher)
-
-    @pytest.mark.xfail(
-        not has_blake3(),
-        reason='blake3 is not installed',
-        raises=errors.MissingDependencyError,
-    )
-    @pytest.mark.parametrize(
-        'hasher',
-        (
-            HasherChoice.blake2b,
-            HasherChoice.blake2s,
-            HasherChoice.blake3,
-        ),
-    )
-    @mock.patch('blake2signer.bases.time')
-    def test_sign_is_unique_non_deterministic(  # pylint: disable=W0221
-        self,
-        mock_time: mock.MagicMock,
-        hasher: HasherChoice,
-    ) -> None:
-        """Test that each signing is unique because of salt."""
-        mock_time.return_value = time()
-
-        super().test_sign_is_unique_non_deterministic(hasher)
-
-    @pytest.mark.xfail(
-        not has_blake3(),
-        reason='blake3 is not installed',
-        raises=errors.MissingDependencyError,
-    )
-    @pytest.mark.parametrize(
-        'hasher',
-        (
-            HasherChoice.blake2b,
-            HasherChoice.blake2s,
-            HasherChoice.blake3,
-        ),
-    )
-    @mock.patch('blake2signer.bases.time')
-    def test_sign_parts_is_unique_non_deterministic(  # pylint: disable=W0221
-        self,
-        mock_time: mock.MagicMock,
-        hasher: HasherChoice,
-    ) -> None:
-        """Test that each signing in parts is unique because of salt."""
-        mock_time.return_value = time()
-
-        super().test_sign_parts_is_unique_non_deterministic(hasher)
+    now = 531810000.0  # Signatures for version compat test were made with this time
+    patch_time = mock.patch('blake2signer.bases.get_current_time', return_value=now)
+    mock_time: mock.MagicMock
+
+    def setup_method(self):
+        """Tests set-up."""
+        self.mock_time = self.patch_time.start()
+
+    def teardown_method(self):
+        """Tests teardown."""
+        self.patch_time.stop()
+
+    @staticmethod
+    def get_expired_signature_error_data(
+        exc: errors.ExpiredSignatureError,
+        *,
+        signer: Signer,  # pylint: disable=W0613
+    ) -> typing.Any:
+        """Get expired signature error data."""
+        return exc.data
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_sign_unsign_timestamp_expired(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test unsigning with timestamp is correct."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(self.secret, hasher=hasher)
-
         signed = self.sign(signer, self.data)
 
-        mock_time.return_value += 10
+        self.mock_time.return_value += 10
         with pytest.raises(
                 errors.ExpiredSignatureError,
                 match='signature has expired',
         ) as exc:
             self.unsign(signer, signed)
+
         assert exc.value.__cause__ is None
-        assert timestamp == exc.value.timestamp.timestamp()
-        assert self.data == exc.value.data
+        assert isclose(self.now, exc.value.timestamp.timestamp())
+        assert self.data == self.get_expired_signature_error_data(exc.value, signer=signer)
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_sign_unsign_timestamp_future(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test signing in the future, then unsigning, causes an exception."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(hasher=hasher)
         signed = self.sign(signer, self.data)
 
         # Back to the future
-        mock_time.return_value -= 10
+        self.mock_time.return_value -= 10
         with pytest.raises(
                 errors.ExpiredSignatureError,
                 match='< 0 seconds',
         ) as exc:
             self.unsign(signer, signed, max_age=5)
-        assert timestamp == exc.value.timestamp.timestamp()
+
+        assert isclose(self.now, exc.value.timestamp.timestamp())
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_sign_unsign_timestamp_in_exc_is_an_aware_datetime(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test that the timestamp in ExpiredSignatureError is an aware datetime."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(hasher=hasher)
         signed = self.sign(signer, self.data)
 
-        mock_time.return_value += 10
+        self.mock_time.return_value += 10
         with pytest.raises(
                 errors.ExpiredSignatureError,
                 match='signature has expired',
         ) as exc:
             self.unsign(signer, signed, max_age=5)
+
         assert exc.value.__cause__ is None
-        assert timestamp == exc.value.timestamp.timestamp()
+        assert isclose(self.now, exc.value.timestamp.timestamp())
         assert timedelta() == exc.value.timestamp.utcoffset()  # Aware in UTC
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
@@ -237,32 +151,35 @@
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
     def test_unsign_wrong_data_without_timestamp(self, hasher: HasherChoice) -> None:
         """Test unsign wrong data."""
         signer = self.signer(hasher=hasher)
-
         trick_signed = self.trick_sign(signer, self.data)
+
         with pytest.raises(
                 errors.SignatureError,
                 match='separator not found in timestamped data',
         ) as exc:
             self.unsign(signer, trick_signed)
+
         assert exc.value.__cause__ is None
 
         trick_signed = self.trick_sign(
             signer,
             signer._separator + signer._force_bytes(self.data),  # pylint: disable=W0212
         )
+
         with pytest.raises(
                 errors.SignatureError,
                 match='timestamp information is missing',
         ) as exc:
             self.unsign(signer, trick_signed, max_age=1)
+
         assert exc.value.__cause__ is None
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
@@ -273,21 +190,22 @@
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
     def test_unsign_wrong_timestamped_data(self, hasher: HasherChoice) -> None:
         """Test unsign wrong timestamped data."""
         signer = self.signer(hasher=hasher)
-
         trick_signed = self.trick_sign(
             signer,
             b'-' + signer._separator + signer._force_bytes(self.data),  # pylint: disable=W0212
         )
+
         with pytest.raises(errors.DecodeError, match='can not be decoded') as exc:
             self.unsign(signer, trick_signed)
+
         assert exc.value.__cause__ is not None
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
@@ -295,28 +213,26 @@
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_sign_timestamp_overflow(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test signing with timestamp after 2106 which causes an integer overflow.
 
         With four unsigned bytes, we can represent up to 2106-02-07 3:28:15.
         """
-        mock_time.return_value = int.from_bytes(b'\xff' * 4, 'big', signed=False) + 1
+        self.mock_time.return_value = int.from_bytes(b'\xff' * 4, 'big') + 1
         signer = self.signer(hasher=hasher)
 
-        with pytest.raises(RuntimeError):
+        with pytest.raises(RuntimeError, match='can not represent this timestamp in bytes'):
             self.sign(signer, self.data)
 
     def test_sign_unsign_with_different_signer(self) -> None:
         """Test signing and unsigning with different signers fails correctly."""
         signer1 = self.signer()
         signer2 = Blake2Signer(self.secret)
 
@@ -324,28 +240,14 @@
         with pytest.raises(errors.InvalidSignatureError):
             signer2.unsign(signed1)
 
         signed2 = signer2.sign(self.data)
         with pytest.raises(errors.InvalidSignatureError):
             self.unsign(signer1, signed2)
 
-    @abstractmethod
-    def test_versions_compat(
-        self,
-        version: str,
-        hasher: HasherChoice,
-        signed: str,
-        compat: bool,
-    ) -> None:
-        """Test if previous versions' signed data is compatible with the current one."""
-        timestamp: int = 531810000  # Signatures were made w/ this timestamp, too.
-
-        with mock.patch('blake2signer.bases.time', return_value=timestamp):
-            super().test_versions_compat(version, hasher, signed, compat)
-
 
 class TestsBlake2TimestampSigner(TimestampSignerTestsBase, TestsBlake2Signer):
     """Blake2TimestampSigner tests."""
 
     @property
     def signer_class(self) -> typing.Type[Signer]:
         """Get the signer class to test."""
@@ -384,110 +286,102 @@
             HasherChoice.blake3,
         ),
     )
     @pytest.mark.parametrize(
         'max_age',
         (2, 2.5, timedelta(hours=2)),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_max_age_can_be_changed(
         self,
-        mock_time: mock.MagicMock,
         max_age: typing.Union[int, float, timedelta],
         hasher: HasherChoice,
     ) -> None:
         """Test that max age can be changed correctly."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(hasher=hasher)
-
         signed = self.sign(signer, self.data)
+
         assert self.data == self.unsign(signer, signed, max_age=max_age)
 
+        # called twice, during sign and unsign
+        assert 2 == self.mock_time.call_count
+
         if isinstance(max_age, timedelta):
-            mock_time.return_value += max_age.total_seconds()
+            self.mock_time.return_value += max_age.total_seconds()
         else:
-            mock_time.return_value += max_age
-        mock_time.return_value += 0.1  # It has to be a bit bigger than max_age
+            self.mock_time.return_value += max_age
+        self.mock_time.return_value += 0.1  # It has to be a bit bigger than max_age
 
         with pytest.raises(
                 errors.ExpiredSignatureError,
                 match='signature has expired',
         ) as exc:
             self.unsign(signer, signed, max_age=max_age)
+
         assert exc.value.__cause__ is None
-        assert timestamp == exc.value.timestamp.timestamp()
+        assert isclose(self.now, exc.value.timestamp.timestamp())
         assert self.data == exc.value.data
 
-        # called twice, during sign and unsign
-        mock_time.assert_has_calls([mock.call(), mock.call()])
+        # called one more time during unsign
+        assert 3 == self.mock_time.call_count
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_max_age_can_be_null(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test that `max_age` can be null."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(hasher=hasher)
 
         signed = self.sign(signer, self.data)
         unsigned = self.unsign(signer, signed, max_age=None)
 
         assert self.data == unsigned
 
         # called once when getting the time during sign, and not during unsign
-        mock_time.assert_called_once_with()
+        self.mock_time.assert_called_once_with()
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
         'hasher',
         (
             HasherChoice.blake2b,
             HasherChoice.blake2s,
             HasherChoice.blake3,
         ),
     )
-    @mock.patch('blake2signer.bases.time')
     def test_max_age_can_be_null_in_parts(
         self,
-        mock_time: mock.MagicMock,
         hasher: HasherChoice,
     ) -> None:
         """Test that `max_age` can be null."""
-        timestamp = int(time())
-        mock_time.return_value = timestamp
         signer = self.signer(hasher=hasher)
 
         signed = self.sign_parts(signer, self.data)
         unsigned = self.unsign_parts(signer, signed, max_age=None)
 
         assert self.data == unsigned
 
         # called once when getting the time during sign, and not during unsign
-        mock_time.assert_called_once_with()
+        self.mock_time.assert_called_once_with()
 
     @pytest.mark.xfail(
         not has_blake3(),
         reason='blake3 is not installed',
         raises=errors.MissingDependencyError,
     )
     @pytest.mark.parametrize(
```

### Comparing `blake2signer-3.0.0/blake2signer/tests/test_utils.py` & `blake2signer-3.1.0/blake2signer/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Utils module tests."""
 
 import io
 import typing
 from datetime import datetime
 from datetime import timedelta
+from unittest import mock
 
 import pytest
 
 from .. import utils
 
 
 def test_b64encode_strips_padding() -> None:
@@ -66,14 +67,56 @@
 
 def test_hexencode_accepts_bytes() -> None:
     """Test hexencode accepts bytes correctly."""
     encoded = utils.hexencode(b'abc')
     assert encoded == b'616263'
 
 
+def test_b58decode_works() -> None:
+    """Test b58decode works correctly."""
+    decoded = utils.b58decode(b'ZiCa')
+    assert decoded == b'abc'
+
+
+def test_b58decode_adds_leading_zeroes() -> None:
+    """Test b58decode adds leading zeroes correctly."""
+    decoded = utils.b58decode(b'111ZiCa')
+    assert decoded == b'\x00\x00\x00abc'
+
+
+def test_b58decode_fails_unknown_char() -> None:
+    """Test b58decode fails when unknown char is passed."""
+    with pytest.raises(KeyError, match=str(int.from_bytes(b'I', 'big'))):
+        utils.b58decode(b'abcI')
+
+
+def test_b58encode_works() -> None:
+    """Test b58encode works correctly."""
+    encoded = utils.b58encode(b'abc')
+    assert encoded == b'ZiCa'
+
+    # Test vectors from "The Base58 Encoding Scheme"
+    # https://datatracker.ietf.org/doc/html/draft-msporny-base58#page-6
+    encoded = utils.b58encode(b'Hello World!')
+    assert encoded == b'2NEpo7TZRRrLZSi2U'
+
+    encoded = utils.b58encode(b'The quick brown fox jumps over the lazy dog.')
+    assert encoded == b'USm3fpXnKG5EUBx2ndxBDMPVciP5hGey2Jh4NDv6gmeo1LkMeiKrLJUUBk6Z'
+
+    num = 0x0000287fb4cd
+    encoded = utils.b58encode(num.to_bytes(2 + (num.bit_length() + 7) // 8, 'big'))
+    assert encoded == b'11233QC4'
+
+
+def test_b58encode_encodes_leading_zeroes() -> None:
+    """Test b58encode encodes leading zeroes correctly."""
+    encoded = utils.b58encode(b'\x00\x00\x00abc')
+    assert encoded == b'111ZiCa'
+
+
 def test_timestamp_to_aware_datetime_accepts_int() -> None:
     """Test timestamp_to_aware_datetime accepts int timestamps."""
     timestamp = 1619064799
     converted_timestamp = utils.timestamp_to_aware_datetime(timestamp)
 
     assert isinstance(converted_timestamp, datetime)
     assert timedelta() == converted_timestamp.utcoffset()  # Aware in UTC
@@ -151,7 +194,28 @@
     assert expected == forced
 
 
 def test_force_string_wrong_type() -> None:
     """Test that force_string raises exception on a wrong type."""
     with pytest.raises(TypeError, match='value must be bytes or str'):
         utils.force_string(1)  # type: ignore
+
+
+def test_get_current_time() -> None:
+    """Test that get_current_time returns the result of `time.time()`."""
+    now = 1709782484.3680992
+
+    with mock.patch.object(utils, 'time', return_value=now) as mock_time:
+        assert now == utils.get_current_time()
+
+        mock_time.assert_called_once_with()
+
+
+def test_generate_secret() -> None:
+    """Test that generate_secret returns a value.
+
+    We are not checking entropy nor anything like that, it would be pointless.
+    """
+    key = utils.generate_secret()
+
+    assert isinstance(key, str)
+    assert key  # Assert we have a value
```

### Comparing `blake2signer-3.0.0/pyproject.toml` & `blake2signer-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blake2signer"
-version = "3.0.0"
+version = "3.1.0"
 description = "A library to use BLAKE in keyed hashing mode to sign and verify signed data"
 authors = ["HacKan <hackan@gmail.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://gitlab.com/hackancuba/blake2signer"
 documentation = "https://blake2signer.hackan.net"
 keywords = [
```

### Comparing `blake2signer-3.0.0/PKG-INFO` & `blake2signer-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blake2signer
-Version: 3.0.0
+Version: 3.1.0
 Summary: A library to use BLAKE in keyed hashing mode to sign and verify signed data
 Home-page: https://gitlab.com/hackancuba/blake2signer
 License: MPL-2.0
 Keywords: blake,cryptography,crypto,signer,signature,keyed-hashing,hashing,mac,digest
 Author: HacKan
 Author-email: hackan@gmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -187,15 +187,15 @@
 * [Erus](https://gitlab.com/erudin): docs title logo, code review.
 * [NoonSleeper](https://gitlab.com/noonsleeper): project icons.
 
 ## License
 
 **Blake2Signer** is made by [HacKan](https://hackan.net) under MPL v2.0. You are free to use, share, modify and share modifications under the terms of that [license](LICENSE).  Derived works may link back to the canonical repository: `https://gitlab.com/hackancuba/blake2signer`.
 
-    Copyright (C) 2020 - 2024 HacKan (https://hackan.net)
+    Copyright (C) 2020-2024 HacKan (https://hackan.net)
     This Source Code Form is subject to the terms of the Mozilla Public
     License, v. 2.0. If a copy of the MPL was not distributed with this
     file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 ----
 
 [![CC BY-SA 4.0](https://i.creativecommons.org/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) *Blake2Signer icons* by [NoonSleeper](https://gitlab.com/noonsleeper) are licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/). You are free to use, share, modify and share modifications under the terms of that [license](https://creativecommons.org/licenses/by-sa/4.0/). They were based on *Blake2Signer logo* by [HacKan](https://hackan.net) which was based on [this sword](https://thenounproject.com/term/samurai-sword/2044449/) by *Hamza Wahbi* and [this signature](https://thenounproject.com/term/sign/184638/) by *Nick Bluth*, both licensed under [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/), and inspired by [It's dangerous logo](https://itsdangerous.palletsprojects.com/en/1.1.x/_images/itsdangerous-logo.png).
```

