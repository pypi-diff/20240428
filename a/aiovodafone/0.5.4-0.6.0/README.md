# Comparing `tmp/aiovodafone-0.5.4.tar.gz` & `tmp/aiovodafone-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiovodafone-0.5.4.tar", max compression
+gzip compressed data, was "aiovodafone-0.6.0.tar", max compression
```

## Comparing `aiovodafone-0.5.4.tar` & `aiovodafone-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11346 2024-01-21 17:00:14.135100 aiovodafone-0.5.4/LICENSE
--rw-r--r--   0        0        0     3314 2024-01-21 17:00:14.135100 aiovodafone-0.5.4/README.md
--rw-r--r--   0        0        0     1973 2024-01-21 17:00:15.131104 aiovodafone-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      497 2024-01-21 17:00:14.135100 aiovodafone-0.5.4/src/aiovodafone/__init__.py
--rw-r--r--   0        0        0    21302 2024-01-21 17:00:14.135100 aiovodafone-0.5.4/src/aiovodafone/api.py
--rw-r--r--   0        0        0      582 2024-01-21 17:00:14.135100 aiovodafone-0.5.4/src/aiovodafone/const.py
--rw-r--r--   0        0        0      635 2024-01-21 17:00:14.135100 aiovodafone-0.5.4/src/aiovodafone/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-21 17:00:14.135100 aiovodafone-0.5.4/src/aiovodafone/py.typed
--rw-r--r--   0        0        0     4363 1970-01-01 00:00:00.000000 aiovodafone-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-04-28 04:07:07.214879 aiovodafone-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3314 2024-04-28 04:07:07.214879 aiovodafone-0.6.0/README.md
+-rw-r--r--   0        0        0     2246 2024-04-28 04:07:10.698858 aiovodafone-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      525 2024-04-28 04:07:10.702858 aiovodafone-0.6.0/src/aiovodafone/__init__.py
+-rw-r--r--   0        0        0    23473 2024-04-28 04:07:07.218879 aiovodafone-0.6.0/src/aiovodafone/api.py
+-rw-r--r--   0        0        0      707 2024-04-28 04:07:07.218879 aiovodafone-0.6.0/src/aiovodafone/const.py
+-rw-r--r--   0        0        0      636 2024-04-28 04:07:07.218879 aiovodafone-0.6.0/src/aiovodafone/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 04:07:07.218879 aiovodafone-0.6.0/src/aiovodafone/py.typed
+-rw-r--r--   0        0        0     4363 1970-01-01 00:00:00.000000 aiovodafone-0.6.0/PKG-INFO
```

### Comparing `aiovodafone-0.5.4/LICENSE` & `aiovodafone-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovodafone-0.5.4/README.md` & `aiovodafone-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aiovodafone-0.5.4/pyproject.toml` & `aiovodafone-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiovodafone"
-version = "0.5.4"
+version = "0.6.0"
 description = "Python library to control Vodafone Station"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aiovodafone"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -23,23 +23,38 @@
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "*"
 beautifulsoup4 = "*"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.0"
-pytest-cov = ">=3,<5"
+pytest = "^8.1"
+pytest-cov = "^5.0"
 
 [tool.semantic_release]
-branch = "main"
 version_toml = ["pyproject.toml:tool.poetry.version"]
-version_variable = ["src/aiovodafone/__init__.py:__version__"]
+version_variables = ["src/aiovodafone/__init__.py:__version__",]
 build_command = "pip install poetry && poetry build"
 
+[tool.semantic_release.changelog]
+exclude_commit_patterns = [
+    "chore*",
+    "ci*",
+]
+
+[tool.semantic_release.changelog.environment]
+keep_trailing_newline = true
+
+[tool.semantic_release.branches.main]
+match = "main"
+
+[tool.semantic_release.branches.noop]
+match = "(?!main$)"
+prerelease = true
+
 [tool.pytest.ini_options]
 addopts = "-v -Wdefault --cov=aiovodafone --cov-report=term-missing:skip-covered"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 branch = true
 
@@ -48,17 +63,16 @@
     "pragma: no cover",
     "@overload",
     "if TYPE_CHECKING",
     "raise NotImplementedError",
     'if __name__ == "__main__":',
 ]
 
-[tool.isort]
-profile = "black"
-known_first_party = ["aiovodafone", "tests"]
+[tool.ruff.isort]
+known-first-party = ["aioamazondevices", "tests"]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 mypy_path = "src/"
```

### Comparing `aiovodafone-0.5.4/src/aiovodafone/api.py` & `aiovodafone-0.6.0/src/aiovodafone/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 """Support for Vodafone Station."""
+
 import asyncio
 import hashlib
 import hmac
 import re
 import urllib.parse
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from datetime import datetime, timedelta, timezone
+from datetime import UTC, datetime, timedelta
+from http import HTTPStatus
 from http.cookies import SimpleCookie
-from typing import Any
+from typing import Any, cast
 
 import aiohttp
 from bs4 import BeautifulSoup, Tag
 
-from .const import _LOGGER, HEADERS, LOGIN, USER_ALREADY_LOGGED_IN, DeviceType
+from .const import (
+    _LOGGER,
+    FULL_FIELDS_NUM,
+    HEADERS,
+    LOGIN,
+    USER_ALREADY_LOGGED_IN,
+    DeviceType,
+)
 from .exceptions import (
     AlreadyLogged,
     CannotAuthenticate,
     CannotConnect,
     GenericLoginError,
     ModelNotSupported,
 )
@@ -37,46 +46,65 @@
 
 
 class VodafoneStationCommonApi(ABC):
     """Common API calls for Vodafone Station routers."""
 
     @staticmethod
     async def get_device_type(
-        host: str, session: aiohttp.ClientSession
+        host: str,
+        session: aiohttp.ClientSession,
     ) -> DeviceType | None:
-        """Finds out the device type of a Vodafone Stations and returns it as enum.
+        """Find out the device type of a Vodafone Stations and returns it as enum.
+
         The Technicolor devices always answer with a valid HTTP response, the
         Sercomm returns 404 on a missing page. This helps to determine which we are
         talking with.
         For detecting the Sercomm devices, a look up for a CSRF token is used.
 
         Args:
+        ----
             host (str): The router's address, e.g. `192.168.1.1`
-            session (aiohttp.ClientSession): the client session to issue HTTP request with
+            session (aiohttp.ClientSession): the client session for HTTP requests
 
         Returns:
-            DeviceType: If the device is a Technicolor, it returns
-            `DeviceType.TECHNICOLOR`. If the device is a Sercomm, it returns `DeviceType.SERCOMM`.
+        -------
+            DeviceType:
+            If the device is a Technicolor, it returns `DeviceType.TECHNICOLOR`.
+            If the device is a Sercomm,     it returns `DeviceType.SERCOMM`.
             If neither of the device types match, it returns `None`.
+
         """
         async with session.get(
-            f"http://{host}/api/v1/login_conf", headers=HEADERS
+            f"http://{host}/api/v1/login_conf",
+            headers=HEADERS,
         ) as response:
-            if response.status == 200:
+            if response.status == HTTPStatus.OK:
                 response_json = await response.json()
                 if "data" in response_json and "ModelName" in response_json["data"]:
                     return DeviceType.TECHNICOLOR
-        async with session.get(
-            f"https://{host}/login.html", headers=HEADERS, ssl=False
-        ) as response:
-            if response.status == 200:
-                # To identify the Sercomm devices before the login
-                # There's no other sure way to identify a Sercomm device without login
-                if "var csrf_token = " in await response.text():
-                    return DeviceType.SERCOMM
+
+        for protocol in ["https", "http"]:
+            try:
+                async with session.get(
+                    f"{protocol}://{host}/login.html",
+                    headers=HEADERS,
+                    ssl=False,
+                ) as response:
+                    # To identify the Sercomm devices before the login
+                    # There's no other sure way to identify a Sercomm device
+                    # without login
+                    if (
+                        response.status == HTTPStatus.OK
+                        and "var csrf_token = " in await response.text()
+                    ):
+                        return DeviceType.SERCOMM
+            except aiohttp.client_exceptions.ClientConnectorSSLError:
+                _LOGGER.debug("Unable to login using protocol %s", protocol)
+                continue
+
         return None
 
     def __init__(self, host: str, username: str, password: str) -> None:
         """Initialize the scanner."""
         self.host = host
         self.protocol = "http"
         self.username = username
@@ -87,127 +115,135 @@
         self.csrf_token: str = ""
         self.encryption_key: str = ""
         self._unique_id: str | None = None
         self._overview: dict[str, Any] = {}
         self._devices: dict[str, VodafoneStationDevice] = {}
 
     def _client_session(self) -> None:
-        """Create aiohttp ClientSession"""
-
+        """Create aiohttp ClientSession."""
         if not hasattr(self, "session") or self.session.closed:
             _LOGGER.debug("Creating HTTP ClientSession")
             jar = aiohttp.CookieJar(unsafe=True)
             self.session = aiohttp.ClientSession(cookie_jar=jar)
 
     def _base_url(self) -> str:
-        """Create base URL"""
+        """Create base URL."""
         return f"{self.protocol}://{self.host}"
 
     async def _set_cookie(self) -> None:
         """Enable required session cookie."""
         self.session.cookie_jar.update_cookies(
-            SimpleCookie(f"domain={self.host}; name=login_uid; value=1;")
+            SimpleCookie(f"domain={self.host}; name=login_uid; value=1;"),
         )
 
     async def _post_page_result(
-        self, page: str, payload: dict[str, Any], timeout: int = 10
+        self,
+        page: str,
+        payload: dict[str, Any],
+        timeout: int = 10,
     ) -> aiohttp.ClientResponse:
         """Get data from a web page via POST."""
         _LOGGER.debug("POST page  %s from host %s", page, self.host)
-        timestamp = int(datetime.now().timestamp())
+        timestamp = int(datetime.now(tz=UTC).timestamp())
         url = f"{self.base_url}{page}?_={timestamp}&csrf_token={self.csrf_token}"
         return await self.session.post(
             url,
             data=payload,
             headers=self.headers,
             timeout=timeout,
             ssl=False,
             allow_redirects=True,
         )
 
     async def _get_page_result(self, page: str) -> aiohttp.ClientResponse:
         """Get data from a web page via GET."""
         _LOGGER.debug("GET page  %s [%s]", page, self.host)
-        timestamp = int(datetime.now().timestamp())
+        timestamp = int(datetime.now(tz=UTC).timestamp())
         url = f"{self.base_url}{page}?_={timestamp}&csrf_token={self.csrf_token}"
 
         return await self.session.get(
             url,
             headers=self.headers,
             timeout=10,
             ssl=False,
             allow_redirects=False,
         )
 
     @abstractmethod
     def convert_uptime(self, uptime: str) -> datetime:
-        pass
+        """Convert uptime to datetime."""
 
     async def close(self) -> None:
         """Router close session."""
         if hasattr(self, "session"):
             await self.session.close()
 
     @abstractmethod
     async def login(self) -> bool:
-        pass
+        """Router login."""
 
     @abstractmethod
     async def get_devices_data(self) -> dict[str, VodafoneStationDevice]:
-        pass
+        """Get router device data."""
 
     @abstractmethod
     async def get_sensor_data(self) -> dict[Any, Any]:
-        pass
+        """Get router sensor data."""
 
     @abstractmethod
     async def logout(self) -> None:
-        pass
+        """Router logout."""
 
 
 class VodafoneStationTechnicolorApi(VodafoneStationCommonApi):
     """Queries Vodafone Station running Technicolor firmware."""
 
     async def _encrypt_string(
-        self, credential: str, salt: str, salt_web_ui: str
+        self,
+        credential: str,
+        salt: str,
+        salt_web_ui: str,
     ) -> str:
-        """Calculates login hash from the password, the salt and the salt from the web UI.
+        """Calculate login hash (password), the salt and the salt (web UI).
 
         Args:
+        ----
             credential (str): login password for the user
             salt (str): salt given by the login response
             salt_web_ui (str): salt given by the web UI
 
         Returns:
+        -------
             str: the hash for the session API
+
         """
         _LOGGER.debug("Calculate credential hash")
         a = hashlib.pbkdf2_hmac(
             "sha256",
             bytes(credential, "utf-8"),
             bytes(salt, "utf-8"),
             1000,
         ).hex()[:32]
-        b = hashlib.pbkdf2_hmac(
+        return hashlib.pbkdf2_hmac(
             "sha256",
             bytes(a, "utf-8"),
             bytes(salt_web_ui, "utf-8"),
             1000,
         ).hex()[:32]
-        return b
 
     async def login(self) -> bool:
         """Router login."""
         _LOGGER.debug("Logging into %s", self.host)
         self._client_session()
 
         _LOGGER.debug("Get salt for login")
         payload = {"username": self.username, "password": "seeksalthash"}
         salt_response = await self._post_page_result(
-            page="/api/v1/session/login", payload=payload
+            page="/api/v1/session/login",
+            payload=payload,
         )
 
         salt_json = await salt_response.json()
 
         salt = salt_json["salt"]
         salt_web_ui = salt_json["saltwebui"]
 
@@ -230,211 +266,222 @@
         # Request menu otherwise the next call fails
         _LOGGER.debug("Get menu")
         await self._get_page_result("/api/v1/session/menu")
 
         return True
 
     async def get_devices_data(self) -> dict[str, VodafoneStationDevice]:
-        """
-        Get all connected devices as a map of MAC address and device object
+        """Get all connected devices as a map of MAC address and device object.
 
-        Returns:
+        Returns
+        -------
             dict[str, VodafoneStationDevice]: MAC address maps to VodafoneStationDevice
+
         """
         _LOGGER.debug("Get hosts")
         host_response = await self._get_page_result("/api/v1/host/hostTbl")
         host_json = await host_response.json()
 
         devices_dict = {}
         for device in host_json["data"]["hostTbl"]:
             connected = device["active"] == "true"
             connection_type = (
                 "WiFi" if "WiFi" in device["layer1interface"] else "Ethernet"
             )
             ip_address = device["ipaddress"]
             name = device["hostname"]
             mac = device["physaddress"]
-            type = device["type"]
+            dev_type = device["type"]
             wifi = ""  # Technicolor Vodafone Station does not report wifi band
 
             vdf_device = VodafoneStationDevice(
                 connected=connected,
                 connection_type=connection_type,
                 ip_address=ip_address,
                 name=name,
                 mac=mac,
-                type=type,
+                type=dev_type,
                 wifi=wifi,
             )
             devices_dict[mac] = vdf_device
 
         return devices_dict
 
     async def get_sensor_data(self) -> dict[Any, Any]:
+        """Get all sensors data."""
         status_response = await self._get_page_result("/api/v1/sta_status")
         status_json = await status_response.json()
         _LOGGER.debug("GET reply (%s)", status_json)
 
         data = {}
         data["sys_serial_number"] = status_json["data"]["serialnumber"]
         data["sys_firmware_version"] = status_json["data"]["firmwareversion"]
         data["sys_hardware_version"] = status_json["data"]["hardwaretype"]
         data["sys_uptime"] = status_json["data"]["uptime"]
         return data
 
     def convert_uptime(self, uptime: str) -> datetime:
-        return datetime.utcnow().replace(tzinfo=timezone.utc) - timedelta(
-            seconds=int(uptime)
+        """Convert uptime to datetime."""
+        return datetime.now(tz=UTC) - timedelta(
+            seconds=int(uptime),
         )
 
     async def logout(self) -> None:
-        # Logout
+        """Router logout."""
         _LOGGER.debug("Logout")
         await self._post_page_result("/api/v1/session/logout", payload={})
 
 
 class VodafoneStationSercommApi(VodafoneStationCommonApi):
     """Queries Vodafone Station running Sercomm firmware."""
 
     async def _list_2_dict(self, data: dict[Any, Any]) -> dict[Any, Any]:
-        """Transform list in a dict"""
-
-        kv_tuples = [(list(v.keys())[0], (list(v.values())[0])) for v in data]
+        """Transform list in a dict."""
+        kv_tuples = [((next(iter(v.keys()))), (next(iter(v.values())))) for v in data]
         key_values = {}
         for entry in kv_tuples:
             key_values[entry[0]] = entry[1]
 
         _LOGGER.debug("Data retrieved (key_values): %s", key_values)
         return key_values
 
     async def _get_sercomm_page(self, page: str) -> dict[Any, Any]:
         """Get html page and process reply."""
-
         reply = await self._get_page_result(page)
         reply_json = await reply.json(content_type="text/html")
         _LOGGER.debug("GET reply (%s): %s", page, reply_json)
         return await self._list_2_dict(reply_json)
 
     async def _post_sercomm_page(
-        self, page: str, payload: dict[str, Any], timeout: int = 10
-    ) -> dict[Any, Any]:
+        self,
+        page: str,
+        payload: dict[str, Any],
+        timeout: int = 10,
+    ) -> dict[Any, Any] | str:
         """Post html page and process reply."""
-
         reply = await self._post_page_result(page, payload, timeout)
         _LOGGER.debug("POST raw reply (%s): %s", page, await reply.text())
         reply_json = await reply.json(content_type="text/html")
         _LOGGER.debug("POST json reply (%s): %s", page, reply_json)
-        return reply_json
+        return cast(dict, reply_json)
 
     async def _check_logged_in(self) -> bool:
         """Check if logged in or not."""
         reply = await self._post_sercomm_page(
-            "/data/login.json", {"loginUserChkLoginTimeout": self.username}
+            "/data/login.json",
+            {"loginUserChkLoginTimeout": self.username},
         )
         index = int(str(reply)) if reply else 0
         _LOGGER.debug("Login status: %s[%s]", LOGIN[index], reply)
         return bool(reply)
 
     async def _find_login_url(self) -> str:
-        """
-        Find the login page
+        """Find the login page.
 
         Router reply with 200 and a html body instead of a formal redirect
         """
-
         url = f"{self.base_url}/login.html"
         _LOGGER.debug("Requested login url: <%s>", url)
         reply = await self.session.get(
             url,
             headers=self.headers,
             timeout=10,
             ssl=False,
             allow_redirects=True,
         )
-        if reply.status in [403, 404]:
+        if reply.status in [HTTPStatus.FORBIDDEN, HTTPStatus.NOT_FOUND]:
             raise ModelNotSupported
         reply_text = await reply.text()
         soup = BeautifulSoup(reply_text, "html.parser")
         meta_refresh = soup.find("meta", {"http-equiv": "Refresh"})
-        if isinstance(meta_refresh, Tag) and "content" in meta_refresh.attrs.keys():
+        if isinstance(meta_refresh, Tag) and "content" in meta_refresh.attrs:
             meta_content = meta_refresh.get("content")
             parsed_qs = urllib.parse.parse_qs(str(meta_content), separator="; ")
             reply_url: str = parsed_qs["URL"][0]
             redirect_url = urllib.parse.urlparse(reply_url)
             if redirect_url.scheme != self.protocol:
                 self.protocol = redirect_url.scheme
                 self.base_url = self._base_url()
                 _LOGGER.debug("Redirected login!")
                 reply_text = await self._find_login_url()
 
-        return reply_text
+        return cast(str, reply_text)
 
     async def _get_csrf_token(self, reply_text: str) -> None:
         """Load login page to get csrf token."""
-
         soup = BeautifulSoup(reply_text, "html.parser")
         script_tag = soup.find("script", string=True)
         try:
             token = re.findall("(?<=csrf_token)|[^']+", str(script_tag))[1]
-        except IndexError:
-            raise ModelNotSupported
+        except IndexError as err:
+            raise ModelNotSupported from err
         if not token:
-            return None
+            return
         self.csrf_token = token
         _LOGGER.debug("csrf_token: <%s>", self.csrf_token)
 
     async def _get_user_lang(self) -> None:
         """Load user_lang page to get."""
-
         return_dict = await self._get_sercomm_page("/data/user_lang.json")
         self.encryption_key = return_dict["encryption_key"]
         _LOGGER.debug("encryption_key: <%s>", self.encryption_key)
 
     async def _encrypt_string(self, credential: str) -> str:
         """Encrypt username or password for login."""
-
         hash1_str = hmac.new(
             bytes("$1$SERCOMM$", "latin-1"),
             msg=bytes(credential, "latin-1"),
             digestmod=hashlib.sha256,
         ).hexdigest()
 
         return hmac.new(
             bytes(self.encryption_key, "latin-1"),
             msg=bytes(hash1_str, "latin-1"),
             digestmod=hashlib.sha256,
         ).hexdigest()
 
+    async def _encrypt_with_challenge(self, challenge: str) -> str:
+        """Encrypt password with challenge for login."""
+        return hashlib.sha256(
+            bytes(self.password + challenge, "utf-8"),
+        ).hexdigest()
+
+    async def _get_challenge(self) -> str:
+        """Return challenge or login."""
+        return_dict = await self._get_sercomm_page("/data/login.json")
+        challenge: str = return_dict["challenge"]
+        _LOGGER.debug("challenge: <%s>", challenge)
+        return challenge
+
     async def _reset(self) -> bool:
         """Reset page content before loading."""
-
         payload = {"chk_sys_busy": ""}
         reply = await self._post_page_result("/data/reset.json", payload)
         if isinstance(reply, aiohttp.ClientResponse):
-            return reply.status == 200
+            return bool(reply.status == HTTPStatus.OK)
 
         return False
 
-    async def _login_json(self, username: str, password: str) -> bool:
-        """Login via json page"""
-
-        payload = {
-            "LoginName": username,
-            "LoginPWD": password,
-        }
+    async def _login_json(self, payload: dict[str, Any]) -> bool:
+        """Login via json page."""
         reply_json = await self._post_sercomm_page("/data/login.json", payload)
-        _LOGGER.debug("Login result: %s[%s]", LOGIN[int(str(reply_json))], reply_json)
+        reply_str = str(reply_json)
+        _LOGGER.debug(
+            "Login result: %s[%s]",
+            LOGIN[int(reply_str)] if 0 <= int(reply_str) < len(LOGIN) else "unknown",
+            reply_json,
+        )
 
-        if reply_json == "1":
+        if reply_str == "1":
             return True
 
-        if reply_json == "2":
+        if reply_str == "2":
             raise AlreadyLogged
 
-        if reply_json in ["3", "4", "5"]:
+        if reply_str in ["3", "4", "5", "7"]:
             raise CannotAuthenticate
 
         raise GenericLoginError
 
     async def get_sensor_data(self) -> dict[Any, Any]:
         """Load user_data page information."""
         _LOGGER.debug("Getting sensor data for host %s", self.host)
@@ -443,15 +490,14 @@
         reply_dict_2 = await self._get_sercomm_page("/data/statussupportstatus.json")
         reply_dict_3 = await self._get_sercomm_page("/data/statussupportrestart.json")
 
         return reply_dict_1 | reply_dict_2 | reply_dict_3 | self._overview
 
     async def get_devices_data(self) -> dict[str, VodafoneStationDevice]:
         """Get all connected devices."""
-
         _LOGGER.debug("Getting all devices for host %s", self.host)
         return_dict = await self._get_sercomm_page("/data/overview.json")
 
         # Cleanup sensor data from devices in order to be merged later
         self._overview.update(return_dict)
         for info in ["wifi_user", "wifi_guest", "ethernet"]:
             if info in self._overview:
@@ -461,15 +507,14 @@
             "wifi_user" not in return_dict
             and "wifi_guest" not in return_dict
             and "ethernet" not in return_dict
         ):
             _LOGGER.info("No device in response from %s", self.host)
             return self._devices
 
-        # 'on|smartphone|Telefono Nora (2.4GHz)|00:0a:f5:6d:8b:38|192.168.1.128||2.4G;'
         arr_devices = []
         arr_wifi_user = return_dict["wifi_user"].split(";")
         arr_wifi_user = filter(lambda x: x.strip() != "", arr_wifi_user)
         arr_wifi_user = ["Wifi (Main)|" + dev for dev in arr_wifi_user]
         arr_wifi_guest = return_dict["wifi_guest"].split(";")
         arr_wifi_guest = filter(lambda x: x.strip() != "", arr_wifi_guest)
         arr_wifi_guest = ["[Wifi (Guest)|" + dev for dev in arr_wifi_guest]
@@ -480,15 +525,17 @@
         arr_ethernet = ["Ethernet|on|" + dev + "|||" for dev in arr_ethernet]
         arr_devices.append(arr_ethernet)
         arr_devices = [item for sublist in arr_devices for item in sublist]
         _LOGGER.debug("Array of devices: %s", arr_devices)
 
         for device_line in arr_devices:
             device_fields: list[Any] = device_line.split("|")
-            wifi_band = device_fields[7] if len(device_fields) == 8 else ""
+            wifi_band = (
+                device_fields[7] if len(device_fields) == FULL_FIELDS_NUM else ""
+            )
             try:
                 dev_info = VodafoneStationDevice(
                     connection_type=device_fields[0],
                     connected=device_fields[1] == "on",
                     type=device_fields[2],
                     name=device_fields[3],
                     mac=device_fields[4],
@@ -503,16 +550,18 @@
 
     def convert_uptime(self, uptime: str) -> datetime:
         """Convert router uptime to last boot datetime."""
         d = int(uptime.split(":")[0])
         h = int(uptime.split(":")[1])
         m = int(uptime.split(":")[2])
 
-        return datetime.utcnow().replace(tzinfo=timezone.utc) - timedelta(
-            days=d, hours=h, minutes=m
+        return datetime.now(tz=UTC) - timedelta(
+            days=d,
+            hours=h,
+            minutes=m,
         )
 
     async def login(self) -> bool:
         """Router login."""
         _LOGGER.debug("Logging into %s", self.host)
         try:
             self._client_session()
@@ -522,27 +571,46 @@
             raise CannotConnect from exc
 
         await self._get_csrf_token(html_page)
         await self._get_user_lang()
         await self._set_cookie()
         await self._reset()
 
-        # First  try with both  username and password encrypted
-        # Second try with plain username and password encrypted
-        try:
-            _LOGGER.debug("Login first try: username[encrypted], password[encrypted]")
-            logged = await self._login_json(
-                await self._encrypt_string(self.username),
-                await self._encrypt_string(self.password),
-            )
-        except CannotAuthenticate:
-            _LOGGER.debug("Login second try: username[plain], password[encrypted]")
+        if not self.encryption_key:
+            _LOGGER.debug("Login: username[plain], password[challenge encrypted]")
+
+            challenge = await self._get_challenge()
             logged = await self._login_json(
-                self.username, await self._encrypt_string(self.password)
+                {
+                    "LoginName": self.username,
+                    "LoginPWD": await self._encrypt_with_challenge(challenge),
+                    "challenge": challenge,
+                },
             )
+        else:
+            # First  try with both  username and password encrypted
+            # Second try with plain username and password encrypted
+            try:
+                _LOGGER.debug(
+                    "Login first try: username[encrypted], password[encrypted]",
+                )
+                logged = await self._login_json(
+                    {
+                        "LoginName": await self._encrypt_string(self.username),
+                        "LoginPWD": await self._encrypt_string(self.password),
+                    },
+                )
+            except CannotAuthenticate:
+                _LOGGER.debug("Login second try: username[plain], password[encrypted]")
+                logged = await self._login_json(
+                    {
+                        "LoginName": self.username,
+                        "LoginPWD": await self._encrypt_string(self.password),
+                    },
+                )
 
         return logged
 
     async def restart_connection(self, connection_type: str) -> None:
         """Internet Connection restart."""
         _LOGGER.debug(
             "Restarting %s connection for router %s",
@@ -552,20 +620,21 @@
         payload = {f"{connection_type}_reconnect": "1"}
         try:
             if not await self._check_logged_in():
                 await self.login()
             await self._post_sercomm_page("/data/statussupportrestart.json", payload)
         except aiohttp.ClientResponseError as ex:
             _LOGGER.debug(
-                'Client response error for "restart_connection" is: %s', ex.message
+                'Client response error for "restart_connection" is: %s',
+                ex.message,
             )
-            # Some models dump a text reply with wrong HTML headers as reply to a reconnection request
+            # Some models dump a text reply with wrong HTML headers
+            # as reply to a reconnection request
             if not ex.message.startswith("Invalid header token"):
-                raise ex
-            pass
+                raise
 
     async def restart_router(self) -> None:
         """Router restart."""
         _LOGGER.debug("Restarting router %s", self.host)
         payload = {"restart_device": "1"}
         try:
             if not await self._check_logged_in():
```

### Comparing `aiovodafone-0.5.4/src/aiovodafone/const.py` & `aiovodafone-0.6.0/src/aiovodafone/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 """Constants for Vodafone Station."""
+
 import logging
 from enum import Enum
 
 _LOGGER = logging.getLogger(__package__)
 
 HEADERS = {
-    "User-Agent": "Mozilla/5.0 (X11; Fedora; Linux x86_64; rv:78.0) Gecko/20100101 Firefox/78.0",
+    "User-Agent": (
+        "Mozilla/5.0 (X11; Fedora; Linux x86_64; rv:78.0) Gecko/20100101 Firefox/78.0"
+    ),
     "Accept-Language": "en-GB,en;q=0.5",
     "X-Requested-With": "XMLHttpRequest",
 }
 
 LOGIN = [
     "not logged",
     "logged",
     "already logged",
     "credential error",
     "credential error",
     "password mismatch",
+    "incorrect challenge",
+    "password mismatch",
 ]
 
 USER_ALREADY_LOGGED_IN = "MSG_LOGIN_150"
 
+FULL_FIELDS_NUM = 8
+
 
 class DeviceType(str, Enum):
+    """Supported device types."""
+
     SERCOMM = "Sercomm"
     TECHNICOLOR = "Technicolor"
```

### Comparing `aiovodafone-0.5.4/src/aiovodafone/exceptions.py` & `aiovodafone-0.6.0/src/aiovodafone/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Vodafone Station library exceptions."""
+
 from __future__ import annotations
 
 
 class VodafoneError(Exception):
     """Base class for aiovodafone errors."""
```

### Comparing `aiovodafone-0.5.4/PKG-INFO` & `aiovodafone-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovodafone
-Version: 0.5.4
+Version: 0.6.0
 Summary: Python library to control Vodafone Station
 Home-page: https://github.com/chemelli74/aiovodafone
 License: Apache Software License 2.0
 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiovodafone Version: 0.5.4 Summary: Python library
+Metadata-Version: 2.1 Name: aiovodafone Version: 0.6.0 Summary: Python library
 to control Vodafone Station Home-page: https://github.com/chemelli74/
 aiovodafone License: Apache Software License 2.0 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: Other/Proprietary License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

