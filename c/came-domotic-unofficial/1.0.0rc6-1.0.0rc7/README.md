# Comparing `tmp/came_domotic_unofficial-1.0.0rc6.tar.gz` & `tmp/came_domotic_unofficial-1.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "came_domotic_unofficial-1.0.0rc6.tar", max compression
+gzip compressed data, was "came_domotic_unofficial-1.0.0rc7.tar", max compression
```

## Comparing `came_domotic_unofficial-1.0.0rc6.tar` & `came_domotic_unofficial-1.0.0rc7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-03-11 21:08:36.821597 came_domotic_unofficial-1.0.0rc6/LICENSE
--rw-r--r--   0        0        0     9596 2024-03-11 21:08:36.821819 came_domotic_unofficial-1.0.0rc6/README.rst
--rw-r--r--   0        0        0     1633 2024-04-13 13:24:34.787305 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/__init__.py
--rw-r--r--   0        0        0     8116 2024-04-16 20:10:21.308799 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/auth.py
--rw-r--r--   0        0        0     3729 2024-04-15 20:45:14.873945 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/came_domotic_api.py
--rw-r--r--   0        0        0     1650 2024-04-10 18:33:11.416261 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/errors.py
--rw-r--r--   0        0        0     4354 2024-04-15 20:42:31.032668 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models.py
--rw-r--r--   0        0        0     1333 2024-04-09 20:21:25.760095 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-09 20:20:36.804257 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/came_entity.py
--rw-r--r--   0        0        0     8532 2024-04-09 20:21:25.831718 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/digital_input.py
--rw-r--r--   0        0        0     2768 2024-04-09 20:20:56.300919 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/enums.py
--rw-r--r--   0        0        0     2002 2024-03-11 21:08:36.822901 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/exceptions.py
--rw-r--r--   0        0        0     3589 2024-04-09 20:20:59.699037 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/feature.py
--rw-r--r--   0        0        0     1587 2024-04-09 20:21:25.819166 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/helpers.py
--rw-r--r--   0        0        0     5930 2024-04-09 20:16:55.199276 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/light.py
--rw-r--r--   0        0        0     6451 2024-04-09 20:21:11.120716 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/opening.py
--rw-r--r--   0        0        0     6912 2024-04-09 20:21:19.053448 came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/scenario.py
--rw-r--r--   0        0        0     2854 2024-04-16 20:26:47.798539 came_domotic_unofficial-1.0.0rc6/pyproject.toml
--rw-r--r--   0        0        0    10933 1970-01-01 00:00:00.000000 came_domotic_unofficial-1.0.0rc6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/LICENSE
+-rw-r--r--   0        0        0     5155 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/README.rst
+-rw-r--r--   0        0        0     1633 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/__init__.py
+-rw-r--r--   0        0        0     9212 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/auth.py
+-rw-r--r--   0        0        0     4893 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/came_domotic_api.py
+-rw-r--r--   0        0        0     1771 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/errors.py
+-rw-r--r--   0        0        0     6343 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models.py
+-rw-r--r--   0        0        0     1333 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/came_entity.py
+-rw-r--r--   0        0        0     8532 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/digital_input.py
+-rw-r--r--   0        0        0     2768 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/enums.py
+-rw-r--r--   0        0        0     2002 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/exceptions.py
+-rw-r--r--   0        0        0     3589 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/feature.py
+-rw-r--r--   0        0        0     1587 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/helpers.py
+-rw-r--r--   0        0        0     5930 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/light.py
+-rw-r--r--   0        0        0     6451 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/opening.py
+-rw-r--r--   0        0        0     6912 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/scenario.py
+-rw-r--r--   0        0        0     2902 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 came_domotic_unofficial-1.0.0rc7/PKG-INFO
```

### Comparing `came_domotic_unofficial-1.0.0rc6/LICENSE` & `came_domotic_unofficial-1.0.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/__init__.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/__init__.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/auth.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,28 +8,42 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""
+This module manages the HTTP interaction with the Came Domotic API.
+
+Note:
+   As a consumer of the CAME Domotic Unofficial library, **it's quite unlikely that you
+   will need to use this class directly**: you should use the ``CameDomoticAPI`` and the
+   CameEntity classes instead.
+
+   In case of special needs, consider requesting the implementation of the desired
+   feature in the Came Domotic Unofficial library, or forking the library and implement
+   the feature yourself.
+"""
+
+
 from datetime import datetime, timezone, timedelta
 import json
 from typing import Optional
 import requests
 from aiohttp import ClientSession, ClientResponse
 from .errors import (
     CameDomoticAuthError,
     CameDomoticServerError,
     CameDomoticServerNotFoundError,
 )
 
 
 class Auth:
-    """Class to make authenticated requests."""
+    """Class to make authenticated requests to the CAME Domotic API server."""
 
     def __init__(
         self, websession: ClientSession, host: str, username: str, password: str
     ):
         """Initialize the Auth instance.
 
         Args:
@@ -47,20 +61,32 @@
         self.websession = websession
         self.host = host
         self.username = username
         self.password = password
 
         self.session_expiration_timestamp = datetime(2000, 1, 1, tzinfo=timezone.utc)
 
-        self._client_id = ""
-        self._keep_alive_timeout_sec = 0
+        self.client_id = ""
+        self.keep_alive_timeout_sec = 0
         self.cseq = 0
 
-        if not self.validate_host():
-            raise CameDomoticServerNotFoundError(f"Server '{host}' not found")
+        try:
+            self.validate_host()
+        except requests.RequestException as e:
+            raise CameDomoticServerNotFoundError(f"Server '{host}' not found") from e
+
+    # region Context manager
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.async_dispose()
+
+    # endregion
 
     def get_endpoint_url(self) -> str:
         """Get the CAME Domotic endpoint URL.
 
         Returns:
             str: the endpoint URL.
         """
@@ -88,15 +114,15 @@
 
         Raises:
             CameDomoticAuthError: if an error occurs during the login.
         """
 
         if not self.validate_session():
             await self.async_login()
-        return self._client_id
+        return self.client_id
 
     async def async_send_command(
         self, payload: dict, timeout: Optional[int] = 10
     ) -> ClientResponse:
         """Send a command to the Came Domotic server.
 
         Args:
@@ -122,122 +148,126 @@
 
         # Check if the response HTTP status is 2xx
         if 200 <= response.status < 300:
             # Increment the command sequence number
             self.cseq += 1
             # Refresh the session expiration timestamp, keeping 30 secs of "safe zone"
             self.session_expiration_timestamp = datetime.now(timezone.utc) + timedelta(
-                seconds=max(0, self._keep_alive_timeout_sec - 30)
+                seconds=max(0, self.keep_alive_timeout_sec - 30)
             )
 
-        await self._async_raise_for_status_and_ack(response)
+        await self.async_raise_for_status_and_ack(response)
 
         return response
 
-    def validate_host(self, timeout: Optional[int] = 10) -> bool:
+    # The following method is not async because it is used in the __init__ method
+    def validate_host(self, timeout: Optional[int] = 10):
         """Validate the host.
 
         Args:
             timeout (int, optional): the timeout in seconds (default: 10s).
 
-        Returns:
-            bool: True if the host is available, False otherwise.
+        Raises:
+            requests.RequestException: if an error occurs during the request.
         """
-        try:
-            with requests.get(
-                self.get_endpoint_url(),
-                timeout=timeout,
-            ) as resp:
-                return resp.status_code == 200
-        except Exception:  # pylint: disable=broad-except
-            return False
+        # Use the "requests" library (sync) to check if the server is available
+        with requests.get(
+            self.get_endpoint_url(),
+            timeout=timeout,
+        ) as resp:
+            # Ensure that the server URL is available
+            resp.raise_for_status()
+            if resp.status_code != 200:
+                raise requests.HTTPError(f"HTTP error {resp.status_code}.")
 
     async def async_login(self) -> None:
-        """Login to the host.
+        """Login to the Came Domotic server.
 
         Raises:
             CameDomoticAuthError: if an error occurs during the login.
         """
 
         payload = {
             "sl_cmd": "sl_registration_req",
             "sl_login": self.username,
             "sl_pwd": self.password,
         }
 
         try:
             response = await self.async_send_command(payload)
-            response.raise_for_status()
+            data = await response.json(content_type=None)
+            self.client_id = data.get("sl_client_id")
+            self.keep_alive_timeout_sec = data.get("sl_keep_alive_timeout_sec")
         except Exception as e:
             raise CameDomoticAuthError("Generic error logging in") from e
 
-        try:
-            data = await response.json(content_type=None)
-        except json.JSONDecodeError as e:
-            raise CameDomoticServerError("Error decoding the response") from e
-
-        if data.get("sl_data_ack_reason") != 0:
-            raise CameDomoticAuthError(
-                "Error logging in: bad credentials? "
-                f"(Ack code: {data.get('sl_data_ack_reason')})."
-            )
-
-        self._client_id = data.get("sl_client_id")
-        self._keep_alive_timeout_sec = data.get("sl_keep_alive_timeout_sec")
+        self.session_expiration_timestamp = datetime.now(timezone.utc) + timedelta(
+            seconds=max(0, self.keep_alive_timeout_sec - 30)
+        )
 
     async def async_keep_alive(self) -> None:
         """Keep the session alive, eventually logging in again if needed.
 
         Raises:
             CameDomoticServerError: if an error occurs during the keep-alive.
             CameDomoticAuthError: if an error occurs during the login.
         """
 
         if not self.validate_session():
             await self.async_login()
         else:
             payload = {
-                "sl_client_id": self._client_id,
+                "sl_client_id": self.client_id,
                 "sl_cmd": "sl_keep_alive_req",
             }
             await self.async_send_command(payload)
 
     async def async_logout(self) -> None:
         """Logout from the Came Domotic server.
 
         Raises:
             CameDomoticServerError: if an error occurs during the logout.
         """
 
         # Logout only if the session is still valid
         if self.validate_session():
             payload = {
-                "sl_client_id": self._client_id,
+                "sl_client_id": self.client_id,
                 "sl_cmd": "sl_logout_req",
             }
             await self.async_send_command(payload)
+            self.client_id = ""
+            self.session_expiration_timestamp = datetime.now(timezone.utc)
 
     async def async_dispose(self):
         """Dispose the Auth instance, eventually logging out if needed."""
         if self.validate_session():
             try:
                 await self.async_logout()
             except CameDomoticServerError:
                 pass
         await self.websession.close()
 
     # region Utilities
 
     def validate_session(self) -> bool:
-        """Check if the session is still valid."""
+        """Check whether the session is still valid or not."""
         return self.session_expiration_timestamp > datetime.now(timezone.utc)
 
     @staticmethod
-    async def _async_raise_for_status_and_ack(response: ClientResponse):
-        """Check the response status and raise an error if necessary."""
+    async def async_raise_for_status_and_ack(response: ClientResponse):
+        """Check the response status and raise an error if necessary.
+
+        Args:
+            response (ClientResponse): the response.
+
+        Raises:
+            CameDomoticServerError: if there is an error interacting with
+                the remote Came Domotic server.
+        """
         try:
             response.raise_for_status()
         except Exception as e:
             raise CameDomoticServerError() from e
 
         try:
             resp_json = await response.json(content_type=None)
```

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/errors.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""
+CAME Domotic exceptions.
+"""
+
 
 class CameDomoticError(Exception):
     """Base exception class for the Came Domotic package."""
 
 
 class CameDomoticServerNotFoundError(CameDomoticError):
     """Raised when the specified host is not available"""
@@ -23,21 +27,33 @@
 
 # Authentication exception class
 class CameDomoticAuthError(CameDomoticError):
     """Raised when there is an authentication error with the remote server."""
 
 
 # Server exception class
-class CameDomoticServerError(CameDomoticError):
-    """Error raised when interacting the remote Came Domotic server"""
+class CameDomoticRemoteServerError(CameDomoticError):
+    """Raised when there is an error related to the Came Domotic server."""
+
+
+class CameDomoticRequestError(CameDomoticError):
+    """Raised when the server doesn't accept a user request."""
+
+
+class CameDomoticBadAckError(CameDomoticRequestError):
+    """Raised when the server returns a bad ack code/reason.
+
+    :param ack_code: the ack code returned by the server.
+    :param reason: the reason returned by the server."""
 
-    @staticmethod
-    def format_ack_error(ack_code: str = "N/A", reason: str = "N/A") -> str:
-        """Formats the ack code and reason in a human-readable format.
+    def __init__(self, ack_code=None, reason=None):
+        """Constructor for the CameDomoticBadAckError class.
 
-        :param ack_code: the ack code returned by the server (optional).
+        :param ack_code: the ack code returned by the server.
         :param reason: the reason returned by the server (optional).
-        :return: a human-readable string with the ack code and reason.
         """
 
         # Convert with str() to ensure that will never raise an exception
-        return f"Bad ack code: {str(ack_code)} - Reason: {str(reason)}"
+        super().__init__(
+            f"Bad ack code: {str(ack_code) if ack_code else 'N/A'} - "
+            f"Reason: {str(reason) if reason else 'N/A'}"
+        )
```

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/__init__.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/__init__.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/came_entity.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/came_entity.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/digital_input.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/digital_input.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/enums.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/enums.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/feature.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/feature.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/helpers.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/helpers.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/light.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/light.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/opening.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/opening.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/came_domotic_unofficial/models_OLD/scenario.py` & `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/scenario.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc6/pyproject.toml` & `came_domotic_unofficial-1.0.0rc7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
 [tool.poetry]
 name = "came_domotic_unofficial"
-version = "1.0.0rc6"
+version = "1.0.0rc7"
 description = "Python library to interact with a CAME ETI/Domo domotic server."
 license = "Apache-2.0"
 authors = ["camedomotic-unofficial <camedomotic-unofficial@gmail.com>"]
 maintainers = ["camedomotic-unofficial <camedomotic-unofficial@gmail.com>"]
 readme = "README.rst"
 
 homepage = "https://github.com/camedomotic-unofficial/came_domotic_unofficial"
@@ -48,24 +48,26 @@
 
 [tool.poetry.urls]
 "Bug tracker" = "https://github.com/camedomotic-unofficial/came_domotic_unofficial/issues"
 
 [tool.poetry.dependencies]
 python = '^3.12'
 aiohttp = '^3.9.3'
+requests = '^2.31.0'
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 freezegun = '^1.4.0'
 hypothesis = '^6.98.17'
 pytest = '^8.0.2'
 pytest-cov = '>=4.1,<6.0'
 pytest-timeout = '^2.3.1'
+pytest-asyncio = '^0.23.6'
 
 [tool.poetry.group.code-quality]
 optional = true
 
 [tool.poetry.group.code-quality.dependencies]
 black = '^24.3.0'
 pylint = '^3.1.0'
```

