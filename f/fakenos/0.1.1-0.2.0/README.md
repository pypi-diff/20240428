# Comparing `tmp/fakenos-0.1.1.tar.gz` & `tmp/fakenos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakenos-0.1.1.tar", max compression
+gzip compressed data, was "fakenos-0.2.0.tar", max compression
```

## Comparing `fakenos-0.1.1.tar` & `fakenos-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,62 @@
--rw-r--r--   0        0        0       90 2022-04-18 22:07:22.000000 fakenos-0.1.1/fakenos/__init__.py
--rw-r--r--   0        0        0        0 2022-04-17 09:31:05.000000 fakenos-0.1.1/fakenos/core/__init__.py
--rw-r--r--   0        0        0     7874 2022-04-23 01:14:15.871383 fakenos-0.1.1/fakenos/core/fakenos.py
--rw-r--r--   0        0        0     1775 2022-04-21 07:24:33.948037 fakenos-0.1.1/fakenos/core/host.py
--rw-r--r--   0        0        0     4716 2022-04-23 01:13:35.658965 fakenos-0.1.1/fakenos/core/nos.py
--rw-r--r--   0        0        0     3693 2022-04-23 00:55:53.750931 fakenos-0.1.1/fakenos/core/pydantic_models.py
--rw-r--r--   0        0        0     3055 2022-04-21 07:24:33.916790 fakenos-0.1.1/fakenos/core/servers.py
--rw-r--r--   0        0        0        0 2022-04-17 09:32:23.000000 fakenos-0.1.1/fakenos/plugins/__init__.py
--rw-r--r--   0        0        0       64 2022-04-18 21:39:36.000000 fakenos-0.1.1/fakenos/plugins/nos/__init__.py
--rw-r--r--   0        0        0     7958 2022-04-24 04:22:56.580408 fakenos-0.1.1/fakenos/plugins/nos/cisco_ios.py
--rw-r--r--   0        0        0      111 2022-04-17 09:31:35.000000 fakenos-0.1.1/fakenos/plugins/servers/__init__.py
--rw-r--r--   0        0        0    10378 2022-04-23 00:39:59.147632 fakenos-0.1.1/fakenos/plugins/servers/ssh_server_paramiko.py
--rw-r--r--   0        0        0       72 2022-04-17 09:31:48.000000 fakenos-0.1.1/fakenos/plugins/shell/__init__.py
--rw-r--r--   0        0        0     4310 2022-04-24 03:55:47.780265 fakenos-0.1.1/fakenos/plugins/shell/cmd_shell.py
--rw-r--r--   0        0        0        0 2022-04-17 09:32:01.000000 fakenos-0.1.1/fakenos/plugins/tapes/__init__.py
--rw-r--r--   0        0        0       76 2022-04-17 04:38:20.000000 fakenos-0.1.1/fakenos/plugins/tapes/netmiko_tape.py
--rw-r--r--   0        0        0        0 2022-04-17 09:32:14.000000 fakenos-0.1.1/fakenos/plugins/utils/__init__.py
--rw-r--r--   0        0        0      913 2022-04-23 00:39:57.848875 fakenos-0.1.1/fakenos/plugins/utils/cli.py
--rw-r--r--   0        0        0     1071 2022-04-17 09:29:21.664280 fakenos-0.1.1/LICENSE
--rw-r--r--   0        0        0     1576 2022-04-24 05:00:08.855491 fakenos-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4694 2022-04-23 22:55:20.276464 fakenos-0.1.1/README.md
--rw-r--r--   0        0        0     5681 2022-04-24 05:00:32.335169 fakenos-0.1.1/setup.py
--rw-r--r--   0        0        0     5441 2022-04-24 05:00:32.339074 fakenos-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      327 2024-04-27 22:56:37.034664 fakenos-0.2.0/fakenos/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:14.936145 fakenos-0.2.0/fakenos/core/__init__.py
+-rw-r--r--   0        0        0    11573 2024-04-28 09:05:10.058072 fakenos-0.2.0/fakenos/core/fakenos.py
+-rw-r--r--   0        0        0     3181 2024-04-27 22:56:37.034664 fakenos-0.2.0/fakenos/core/host.py
+-rw-r--r--   0        0        0     7301 2024-04-28 09:02:15.902070 fakenos-0.2.0/fakenos/core/nos.py
+-rw-r--r--   0        0        0     5065 2024-04-27 22:56:37.034664 fakenos-0.2.0/fakenos/core/pydantic_models.py
+-rw-r--r--   0        0        0     3505 2024-04-28 08:45:19.811914 fakenos-0.2.0/fakenos/core/servers.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:15.107288 fakenos-0.2.0/fakenos/plugins/__init__.py
+-rw-r--r--   0        0        0     1352 2024-04-27 23:57:55.382418 fakenos-0.2.0/fakenos/plugins/nos/__init__.py
+-rw-r--r--   0        0        0     6515 2024-04-28 07:50:08.143682 fakenos-0.2.0/fakenos/plugins/nos/arista_eos.py
+-rw-r--r--   0        0        0     8596 2024-04-28 00:08:52.164892 fakenos-0.2.0/fakenos/plugins/nos/cisco_ios.py
+-rw-r--r--   0        0        0     1139 2024-04-28 09:11:08.895513 fakenos-0.2.0/fakenos/plugins/nos/platforms/alcatel_aos.yaml
+-rw-r--r--   0        0        0    52601 2024-04-28 09:11:30.025274 fakenos-0.2.0/fakenos/plugins/nos/platforms/alcatel_sros.yaml
+-rw-r--r--   0        0        0    24693 2024-04-28 09:11:46.047819 fakenos-0.2.0/fakenos/plugins/nos/platforms/allied_telesis_awplus.yaml
+-rw-r--r--   0        0        0   101390 2024-04-28 00:19:03.430855 fakenos-0.2.0/fakenos/plugins/nos/platforms/arista_eos.yaml
+-rw-r--r--   0        0        0    12448 2024-04-28 09:12:03.687914 fakenos-0.2.0/fakenos/plugins/nos/platforms/aruba_os.yaml
+-rw-r--r--   0        0        0    23369 2024-04-28 09:12:28.023286 fakenos-0.2.0/fakenos/plugins/nos/platforms/avaya_ers.yaml
+-rw-r--r--   0        0        0     1092 2024-04-28 09:12:42.233520 fakenos-0.2.0/fakenos/plugins/nos/platforms/avaya_vsp.yaml
+-rw-r--r--   0        0        0     8628 2024-04-28 09:12:57.095002 fakenos-0.2.0/fakenos/plugins/nos/platforms/broadcom_icos.yaml
+-rw-r--r--   0        0        0    67942 2024-04-28 09:13:21.551116 fakenos-0.2.0/fakenos/plugins/nos/platforms/brocade_fastiron.yaml
+-rw-r--r--   0        0        0    44706 2024-04-28 08:51:40.978320 fakenos-0.2.0/fakenos/plugins/nos/platforms/brocade_netiron.yaml
+-rw-r--r--   0        0        0    10034 2024-04-28 08:52:02.337493 fakenos-0.2.0/fakenos/plugins/nos/platforms/checkpoint_gaia.yaml
+-rw-r--r--   0        0        0    15188 2024-04-28 08:52:22.505013 fakenos-0.2.0/fakenos/plugins/nos/platforms/ciena_saos.yaml
+-rw-r--r--   0        0        0    98498 2024-04-28 08:52:40.875352 fakenos-0.2.0/fakenos/plugins/nos/platforms/cisco_asa.yaml
+-rw-r--r--   0        0        0     2110 2024-04-28 08:53:00.842586 fakenos-0.2.0/fakenos/plugins/nos/platforms/cisco_ftd.yaml
+-rw-r--r--   0        0        0   339604 2024-04-27 23:56:49.638466 fakenos-0.2.0/fakenos/plugins/nos/platforms/cisco_ios.yaml
+-rw-r--r--   0        0        0   368517 2024-04-28 08:53:27.729275 fakenos-0.2.0/fakenos/plugins/nos/platforms/cisco_nxos.yaml
+-rw-r--r--   0        0        0    10643 2024-04-28 08:53:46.034065 fakenos-0.2.0/fakenos/plugins/nos/platforms/cisco_s300.yaml
+-rw-r--r--   0        0        0   478717 2024-04-28 08:54:04.916829 fakenos-0.2.0/fakenos/plugins/nos/platforms/cisco_xr.yaml
+-rw-r--r--   0        0        0     9821 2024-04-28 08:54:19.593994 fakenos-0.2.0/fakenos/plugins/nos/platforms/dell_force10.yaml
+-rw-r--r--   0        0        0     8894 2024-04-28 08:56:01.736830 fakenos-0.2.0/fakenos/plugins/nos/platforms/dell_powerconnect.yaml
+-rw-r--r--   0        0        0      983 2024-04-28 08:56:15.440837 fakenos-0.2.0/fakenos/plugins/nos/platforms/dlink_ds.yaml
+-rw-r--r--   0        0        0   103435 2024-04-28 08:56:29.882300 fakenos-0.2.0/fakenos/plugins/nos/platforms/eltex.yaml
+-rw-r--r--   0        0        0     7086 2024-04-28 08:56:49.827233 fakenos-0.2.0/fakenos/plugins/nos/platforms/ericsson_ipos.yaml
+-rw-r--r--   0        0        0    20692 2024-04-28 08:57:05.467447 fakenos-0.2.0/fakenos/plugins/nos/platforms/extreme_exos.yaml
+-rw-r--r--   0        0        0    15732 2024-04-28 08:57:22.513348 fakenos-0.2.0/fakenos/plugins/nos/platforms/fortinet.yaml
+-rw-r--r--   0        0        0    28671 2024-04-28 08:57:36.158732 fakenos-0.2.0/fakenos/plugins/nos/platforms/hp_comware.yaml
+-rw-r--r--   0        0        0    36269 2024-04-28 08:57:48.379228 fakenos-0.2.0/fakenos/plugins/nos/platforms/hp_procurve.yaml
+-rw-r--r--   0        0        0    33538 2024-04-28 08:58:06.913081 fakenos-0.2.0/fakenos/plugins/nos/platforms/huawei_smartax.yaml
+-rw-r--r--   0        0        0    42804 2024-04-28 08:58:25.347132 fakenos-0.2.0/fakenos/plugins/nos/platforms/huawei_vrp.yaml
+-rw-r--r--   0        0        0     2054 2024-04-28 08:59:58.594762 fakenos-0.2.0/fakenos/plugins/nos/platforms/ipinfusion_ocnos.yaml
+-rw-r--r--   0        0        0    34977 2024-04-28 09:00:20.040998 fakenos-0.2.0/fakenos/plugins/nos/platforms/juniper_junos.yaml
+-rw-r--r--   0        0        0     1392 2024-04-28 09:06:23.719625 fakenos-0.2.0/fakenos/plugins/nos/platforms/juniper_screenos.yaml
+-rw-r--r--   0        0        0     5198 2024-04-28 09:06:50.111828 fakenos-0.2.0/fakenos/plugins/nos/platforms/linux.yaml
+-rw-r--r--   0        0        0    20056 2024-04-28 09:05:59.438054 fakenos-0.2.0/fakenos/plugins/nos/platforms/mikrotik_routeros.yaml
+-rw-r--r--   0        0        0    22999 2024-04-28 09:07:24.223709 fakenos-0.2.0/fakenos/plugins/nos/platforms/paloalto_panos.yaml
+-rw-r--r--   0        0        0    52127 2024-04-28 09:07:43.304990 fakenos-0.2.0/fakenos/plugins/nos/platforms/ruckus_fastiron.yaml
+-rw-r--r--   0        0        0    10219 2024-04-28 09:08:42.674111 fakenos-0.2.0/fakenos/plugins/nos/platforms/ubiquiti_edgerouter.yaml
+-rw-r--r--   0        0        0     2940 2024-04-28 09:10:02.618301 fakenos-0.2.0/fakenos/plugins/nos/platforms/ubiquiti_edgeswitch.yaml
+-rw-r--r--   0        0        0     3352 2024-04-28 09:10:21.937156 fakenos-0.2.0/fakenos/plugins/nos/platforms/vyatta_vyos.yaml
+-rw-r--r--   0        0        0     2130 2024-04-28 09:10:37.807839 fakenos-0.2.0/fakenos/plugins/nos/platforms/yamaha.yaml
+-rw-r--r--   0        0        0    13212 2024-04-28 09:10:53.081736 fakenos-0.2.0/fakenos/plugins/nos/platforms/zyxel_os.yaml
+-rw-r--r--   0        0        0      194 2024-04-27 22:56:37.050292 fakenos-0.2.0/fakenos/plugins/servers/__init__.py
+-rw-r--r--   0        0        0    12143 2024-04-28 08:22:50.998177 fakenos-0.2.0/fakenos/plugins/servers/ssh_server_paramiko.py
+-rw-r--r--   0        0        0      152 2024-04-27 22:56:37.050292 fakenos-0.2.0/fakenos/plugins/shell/__init__.py
+-rw-r--r--   0        0        0     5725 2024-04-28 08:18:26.661827 fakenos-0.2.0/fakenos/plugins/shell/cmd_shell.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:14.939513 fakenos-0.2.0/fakenos/plugins/utils/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-28 07:45:04.329410 fakenos-0.2.0/fakenos/plugins/utils/cli.py
+-rw-r--r--   0        0        0     1071 2022-10-02 22:26:28.688575 fakenos-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2864 2024-04-27 22:56:37.050292 fakenos-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4686 2024-04-27 22:56:37.003424 fakenos-0.2.0/README.md
+-rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 fakenos-0.2.0/PKG-INFO
```

### Comparing `fakenos-0.1.1/fakenos/core/pydantic_models.py` & `fakenos-0.2.0/fakenos/core/pydantic_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,172 @@
 """
 File to contain pydantic models for plugins input/output data validation
 """
-from pydantic import (
-    BaseModel,
-    StrictBool,
-    StrictInt,
-    StrictFloat,
-    StrictStr,
-    conlist,
-    IPvAnyAddress,
-    conint,
-    root_validator,
-)
-from typing import Union, Optional, List, Any, Dict, Callable, Tuple
 
-try:
+from __future__ import annotations
+import sys
+
+from typing import Union, Optional, List, Dict, Callable
+
+from pydantic import model_validator, BaseModel, StrictStr, StrictInt, IPvAnyAddress
+
+if sys.version_info >= (3, 8):
     from typing import Literal  # works with >=py3.8
-except ImportError:
-    from typing_extensions import Literal  # works with <py3.8
+else:
+    from typing_extensions import Literal  # works with <py3.8I
+
+# ---------------------------------------------------------------------------------------
+# NOS plugin commands model
+# ---------------------------------------------------------------------------------------
+
+
+class ModelNosCommand(BaseModel):
+    """
+    Pydantic model for NOS command attributes.
+    """
+
+    output: Optional[Union[StrictStr, None, Callable]] = None
+    help: Optional[StrictStr] = None
+    prompt: Optional[Union[StrictStr, List[StrictStr]]] = None
+    new_prompt: Optional[StrictStr] = None
+    alias: Optional[StrictStr] = None
+
+
+class ModelNosAttributes(BaseModel):
+    """
+    Pydantic model for NOS attributes.
+    """
+
+    commands: Dict[StrictStr, ModelNosCommand]
+    name: StrictStr
+    initial_prompt: StrictStr
+
+
+class ModelHost(BaseModel):
+    """
+    Pydantic model for Host Attributes
+    """
+
+    name: StrictStr
+    username: StrictStr
+    password: StrictStr
+    port: StrictInt
+    platform: Optional[StrictStr] = None
 
 
 # ---------------------------------------------------------------------------------------
 # FakeNOS inventory data model components
 # ---------------------------------------------------------------------------------------
 
 
+class NosPluginConfig(BaseModel):
+    """
+    Pydantic model for NOS plugin configuration.
+    """
+
+    commands: Optional[Dict[StrictStr, ModelNosCommand]] = None
+
+
 class NosPlugin(BaseModel):
+    """
+    Pydantic model for NOS plugin.
+    """
+
     plugin: StrictStr
-    configuration: Optional[Dict]
+    configuration: Optional[NosPluginConfig] = None
 
 
 class ParamikoSshServerConfig(BaseModel):
+    """
+    Pydantic model for Paramiko SSH server configuration.
+    """
+
     ssh_key_file: Optional[StrictStr] = None
     ssh_key_file_password: Optional[StrictStr] = None
     ssh_banner: Optional[StrictStr] = "FakeNOS Paramiko SSH Server"
     timeout: Optional[StrictInt] = 1
-    address: Optional[Union[Literal["localhost"], IPvAnyAddress]]
+    address: Optional[Union[Literal["localhost"], IPvAnyAddress]] = None
     watchdog_interval: Optional[StrictInt] = 1
 
 
 class ParamikoSshServerPlugin(BaseModel):
+    """
+    Pydantic model for Paramiko SSH server plugin.
+    """
+
     plugin: Literal["ParamikoSshServer"]
-    configuration: Optional[ParamikoSshServerConfig]
+    configuration: Optional[ParamikoSshServerConfig] = None
 
 
 class CMDShellConfig(BaseModel):
+    """
+    Pydantic model for CMD shell configuration.
+    """
+
     intro: Optional[StrictStr] = "Custom SSH Shell"
     ruler: Optional[StrictStr] = ""
     completekey: Optional[StrictStr] = "tab"
     newline: Optional[StrictStr] = "\r\n"
 
 
 class CMDShellPlugin(BaseModel):
+    """
+    Pydantic model for CMD shell plugin.
+    """
+
     plugin: Literal["CMDShell"]
-    configuration: Optional[CMDShellConfig]
+    configuration: Optional[CMDShellConfig] = None
 
 
 class InventoryDefaultSection(BaseModel):
-    username: Optional[StrictStr]
-    password: Optional[StrictStr]
-    # port: Optional[Union[conint(strict=True, gt=0, le=65535), conlist(conint(strict=True, gt=0, le=65535), min_items=2, max_items=2, unique_items=True)]]
-    # use this for now, mkdocstring having issue with pydantic - https://github.com/mkdocstrings/griffe/issues/66
-    port: Optional[Union[StrictInt, List[StrictInt]]]
-    server: Optional[Union[ParamikoSshServerPlugin]]
-    shell: Optional[Union[CMDShellPlugin]]
-    nos: Optional[NosPlugin]
+    """
+    Pydantic model for FakeNOS inventory default section.
+    """
+
+    username: Optional[StrictStr] = None
+    password: Optional[StrictStr] = None
+    # port: Optional[Union[conint(strict=True, gt=0, le=65535),
+    # conlist(conint(strict=True, gt=0, le=65535),
+    # min_items=2, max_items=2, unique_items=True)]]
+    # use this for now, mkdocstring having issue with pydantic
+    # https://github.com/mkdocstrings/griffe/issues/66
+    port: Optional[Union[StrictInt, List[StrictInt]]] = None
+    server: Optional[Union[ParamikoSshServerPlugin]] = None
+    shell: Optional[Union[CMDShellPlugin]] = None
+    nos: Optional[NosPlugin] = None
 
 
 class HostConfig(InventoryDefaultSection):
+    """
+    Pydantic model for FakeNOS inventory host configuration.
+    """
+
     # count: Optional[conint(strict=True, gt=0)]
-    # use this for now, mkdocstring having issue with pydantic - https://github.com/mkdocstrings/griffe/issues/66
-    count: Optional[StrictInt]
+    # use this for now, mkdocstring having issue with pydantic
+    # https://github.com/mkdocstrings/griffe/issues/66
+    replicas: Optional[StrictInt] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def check_port_value(cls, values):
+        """
+        Method to validate port value based on 'replicas' value.
+        """
         port = values.get("port")
-        if "count" not in values and port:
-            assert isinstance(
-                port, int
-            ), "If no host 'count' given, port must be an integer"
-        elif "count" in values and port:
-            assert isinstance(port, list), "If host 'count' given, port must be a list"
+        if "replicas" not in values and port:
+            assert isinstance(port, int), "If no host 'replicas' given, port must be an integer"
+        elif "replicas" in values and port:
+            assert isinstance(port, list), "If host 'replicas' given, port must be a list"
         return values
 
 
-class model_fakenos_inventory(BaseModel):
+class ModelFakenosInventory(BaseModel):
     """FakeNOS inventory data schema"""
 
-    default: Optional[InventoryDefaultSection]
+    default: Optional[InventoryDefaultSection] = None
     hosts: Dict[StrictStr, HostConfig]
 
-    class Config:
-        extra = "forbid"
+    # pylint: disable=too-few-public-methods
+    class ConfigDict:
+        """Pydantic model configuration"""
 
-
-# ---------------------------------------------------------------------------------------
-# NOS plugin commands model
-# ---------------------------------------------------------------------------------------
-
-class model_nos_command(BaseModel):
-    output: Union[StrictStr, None, Callable]
-    help: Optional[StrictStr]
-    prompt: Optional[Union[StrictStr, List[StrictStr]]]
-    new_prompt: Optional[StrictStr]
-    
-class model_nos_attributes(BaseModel):
-    commands: Dict[StrictStr, model_nos_command]
-    name: StrictStr
-    initial_prompt: StrictStr
+        extra = "forbid"
```

### Comparing `fakenos-0.1.1/LICENSE` & `fakenos-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fakenos-0.1.1/README.md` & `fakenos-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 > "Reality is merely an illusion, albeit a very persistent one."
 >
 > ~ Albert Einstein
 
 FakeNOS created to simulate Network Operating Systems interactions.
 
-[Documentation](https://dmulyalin.github.io/fakenos/)
+[Documentation](https://fakenos.github.io/fakenos/)
 
 ## Why?
 
 Crucial aspect of writing applications or scripts for Network Automation is 
 testing, often testing done using physical or virtual instances of network
 appliances running certain version of Network Operating System (NOS). That
 approach, while gives best integration results, in many cases carries a lot
@@ -74,19 +74,19 @@
 - [PythonSSHServerTutorial](https://github.com/ramonmeza/PythonSSHServerTutorial) - tutorial on creating paramiko based SSH server
 - [fake-switches](https://github.com/internap/fake-switches) - pluggable switch/router command-line simulator
 - [ncs-netsim](https://developer.cisco.com/docs/nso/guides/#!the-network-simulator) - tool to simulate a network of devices
 - [cisshgo](https://github.com/tbotnz/cisshgo) - concurrent SSH server to emulate network equipment for testing purposes
 - [scrapli-replay](https://pypi.org/project/scrapli-replay/) - tools to enable easy testing of SSH programs and to create semi-interactive SSH servers
 
 
-[github-discussions-link]:     https://github.com/dmulyalin/fakenos/discussions
+[github-discussions-link]:     https://github.com/fakenos/fakenos/discussions
 [github-discussions-badge]:    https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [black-badge]:                 https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]:                  https://github.com/psf/black
 [pypi-pyversion-link]:         https://pypi.python.org/pypi/fakenos/
 [pypi-pyversion-badge]:        https://img.shields.io/pypi/pyversions/fakenos.svg
 [pepy-downloads-link]:         https://pepy.tech/project/fakenos
 [pepy-downloads-badge]:        https://pepy.tech/badge/fakenos
-[github-tests-badge]:          https://github.com/dmulyalin/fakenos/actions/workflows/main.yml/badge.svg
-[github-tests-link]:           https://github.com/dmulyalin/fakenos/actions
+[github-tests-badge]:          https://github.com/fakenos/fakenos/actions/workflows/main.yml/badge.svg
+[github-tests-link]:           https://github.com/fakenos/fakenos/actions
 [pypi-latest-release-badge]:   https://img.shields.io/pypi/v/fakenos.svg
 [pypi-latest-release-link]:    https://pypi.python.org/pypi/fakenos
```

### Comparing `fakenos-0.1.1/setup.py` & `fakenos-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,124 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fakenos
+Version: 0.2.0
+Summary: Fake Network Operating System
+License: MIT
+Keywords: NetworkAutomation,Testing,SSH
+Author: Denis Mulyalin
+Author-email: d.mulyalin@gmail.com
+Maintainer: Denis Mulyalin
+Maintainer-email: d.mulyalin@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Utilities
+Provides-Extra: test
+Requires-Dist: detect (>=2020.12.0,<2020.13.0)
+Requires-Dist: paramiko (<4.0)
+Requires-Dist: pydantic (<3.0)
+Requires-Dist: pyyaml (<7.0)
+Description-Content-Type: text/markdown
+
+[![Downloads][pepy-downloads-badge]][pepy-downloads-link]
+[![PyPI][pypi-latest-release-badge]][pypi-latest-release-link]
+[![PyPI versions][pypi-pyversion-badge]][pypi-pyversion-link]
+[![GitHub Discussion][github-discussions-badge]][github-discussions-link]
+[![Code style: black][black-badge]][black-link]
+[![Tests][github-tests-badge]][github-tests-link]
+
+# Fake Network Operating Systems - FakeNOS
+
+> "Reality is merely an illusion, albeit a very persistent one."
+>
+> ~ Albert Einstein
+
+FakeNOS created to simulate Network Operating Systems interactions.
+
+[Documentation](https://fakenos.github.io/fakenos/)
+
+## Why?
+
+Crucial aspect of writing applications or scripts for Network Automation is 
+testing, often testing done using physical or virtual instances of network
+appliances running certain version of Network Operating System (NOS). That
+approach, while gives best integration results, in many cases carries a lot
+of overhead to setup, run and tear down as well as putting significant burden
+on compute and storage resource utilization.
+
+Other approach is to mock underlying libraries methods to fool applications
+under testing into believing that it is getting output from real devices. That
+approach works very well for unit testing, but fails to simulate such aspects
+as connection establishment and handling.
+
+FakeNOS positions itself somewhere in the middle between full integration testing
+and testing that mocks device interactions. FakeNOS allows to create NOS plugins
+to produce pre-defined output to test applications behavior while running servers 
+to establish connections with.
+
+## What?
+
+FakeNOS can:
+
+- Run thousands of servers to stress test applications
+- Simulate Network Operating Systems Command Line Interface (CLI) interactions
+- Provide high-level API to create custom NOS plugins
+- Run in docker container to simplify integration with your infrastructure
+- Make use of FakeNOS CLI tool for quick run and prototype simulations
+- Works on Windows, MAC and Linux under major Python version
+
+## How?
+
+Send input and get the output - this is how we interact with many 
+Network Operating Systems, FakeNOS allows to pre-define the output 
+to sent in response to certain input commands, making it ideal for
+isolated feature testing.
+
+FakeNOS is a micro-kernel framework that can be extended using plugins. 
+The core is kept small and optimized while most of the functionality 
+offloaded to plugins.
+
+FakeNOS has these pluggable systems:
+
+- Server Plugins - plugins responsible for running various servers to connect with
+- Shell Plugins - plugins to simulate command line interface shell
+- NOS plugins - plugins to simulate Network Operating System commands
+
+## What not?
+
+FakeNOS is a simulator, it does not emulate any of Network Control, Data 
+or Management planes, it merely takes the commands as input and responds
+with predefined output.
+
+## FakeNOS inspired by and borrowed from
+
+- [sshim](https://pythonhosted.org/sshim/) - library for testing and debugging SSH automation clients
+- [PythonSSHServerTutorial](https://github.com/ramonmeza/PythonSSHServerTutorial) - tutorial on creating paramiko based SSH server
+- [fake-switches](https://github.com/internap/fake-switches) - pluggable switch/router command-line simulator
+- [ncs-netsim](https://developer.cisco.com/docs/nso/guides/#!the-network-simulator) - tool to simulate a network of devices
+- [cisshgo](https://github.com/tbotnz/cisshgo) - concurrent SSH server to emulate network equipment for testing purposes
+- [scrapli-replay](https://pypi.org/project/scrapli-replay/) - tools to enable easy testing of SSH programs and to create semi-interactive SSH servers
+
+
+[github-discussions-link]:     https://github.com/fakenos/fakenos/discussions
+[github-discussions-badge]:    https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
+[black-badge]:                 https://img.shields.io/badge/code%20style-black-000000.svg
+[black-link]:                  https://github.com/psf/black
+[pypi-pyversion-link]:         https://pypi.python.org/pypi/fakenos/
+[pypi-pyversion-badge]:        https://img.shields.io/pypi/pyversions/fakenos.svg
+[pepy-downloads-link]:         https://pepy.tech/project/fakenos
+[pepy-downloads-badge]:        https://pepy.tech/badge/fakenos
+[github-tests-badge]:          https://github.com/fakenos/fakenos/actions/workflows/main.yml/badge.svg
+[github-tests-link]:           https://github.com/fakenos/fakenos/actions
+[pypi-latest-release-badge]:   https://img.shields.io/pypi/v/fakenos.svg
+[pypi-latest-release-link]:    https://pypi.python.org/pypi/fakenos
 
-packages = \
-['fakenos',
- 'fakenos.core',
- 'fakenos.plugins',
- 'fakenos.plugins.nos',
- 'fakenos.plugins.servers',
- 'fakenos.plugins.shell',
- 'fakenos.plugins.tapes',
- 'fakenos.plugins.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['paramiko>=2.10.3,<3.0.0', 'pydantic>=1.9.0,<2.0.0', 'pyyaml>=6.0.0,<7.0.0']
-
-entry_points = \
-{'console_scripts': ['fakenos = fakenos.plugins.utils.cli:run_cli']}
-
-setup_kwargs = {
-    'name': 'fakenos',
-    'version': '0.1.1',
-    'description': 'Fake Network Operating System',
-    'long_description': '[![Downloads][pepy-downloads-badge]][pepy-downloads-link]\n[![PyPI][pypi-latest-release-badge]][pypi-latest-release-link]\n[![PyPI versions][pypi-pyversion-badge]][pypi-pyversion-link]\n[![GitHub Discussion][github-discussions-badge]][github-discussions-link]\n[![Code style: black][black-badge]][black-link]\n[![Tests][github-tests-badge]][github-tests-link]\n\n# Fake Network Operating Systems - FakeNOS\n\n> "Reality is merely an illusion, albeit a very persistent one."\n>\n> ~ Albert Einstein\n\nFakeNOS created to simulate Network Operating Systems interactions.\n\n[Documentation](https://dmulyalin.github.io/fakenos/)\n\n## Why?\n\nCrucial aspect of writing applications or scripts for Network Automation is \ntesting, often testing done using physical or virtual instances of network\nappliances running certain version of Network Operating System (NOS). That\napproach, while gives best integration results, in many cases carries a lot\nof overhead to setup, run and tear down as well as putting significant burden\non compute and storage resource utilization.\n\nOther approach is to mock underlying libraries methods to fool applications\nunder testing into believing that it is getting output from real devices. That\napproach works very well for unit testing, but fails to simulate such aspects\nas connection establishment and handling.\n\nFakeNOS positions itself somewhere in the middle between full integration testing\nand testing that mocks device interactions. FakeNOS allows to create NOS plugins\nto produce pre-defined output to test applications behavior while running servers \nto establish connections with.\n\n## What?\n\nFakeNOS can:\n\n- Run thousands of servers to stress test applications\n- Simulate Network Operating Systems Command Line Interface (CLI) interactions\n- Provide high-level API to create custom NOS plugins\n- Run in docker container to simplify integration with your infrastructure\n- Make use of FakeNOS CLI tool for quick run and prototype simulations\n- Works on Windows, MAC and Linux under major Python version\n\n## How?\n\nSend input and get the output - this is how we interact with many \nNetwork Operating Systems, FakeNOS allows to pre-define the output \nto sent in response to certain input commands, making it ideal for\nisolated feature testing.\n\nFakeNOS is a micro-kernel framework that can be extended using plugins. \nThe core is kept small and optimized while most of the functionality \noffloaded to plugins.\n\nFakeNOS has these pluggable systems:\n\n- Server Plugins - plugins responsible for running various servers to connect with\n- Shell Plugins - plugins to simulate command line interface shell\n- NOS plugins - plugins to simulate Network Operating System commands\n\n## What not?\n\nFakeNOS is a simulator, it does not emulate any of Network Control, Data \nor Management planes, it merely takes the commands as input and responds\nwith predefined output.\n\n## FakeNOS inspired by and borrowed from\n\n- [sshim](https://pythonhosted.org/sshim/) - library for testing and debugging SSH automation clients\n- [PythonSSHServerTutorial](https://github.com/ramonmeza/PythonSSHServerTutorial) - tutorial on creating paramiko based SSH server\n- [fake-switches](https://github.com/internap/fake-switches) - pluggable switch/router command-line simulator\n- [ncs-netsim](https://developer.cisco.com/docs/nso/guides/#!the-network-simulator) - tool to simulate a network of devices\n- [cisshgo](https://github.com/tbotnz/cisshgo) - concurrent SSH server to emulate network equipment for testing purposes\n- [scrapli-replay](https://pypi.org/project/scrapli-replay/) - tools to enable easy testing of SSH programs and to create semi-interactive SSH servers\n\n\n[github-discussions-link]:     https://github.com/dmulyalin/fakenos/discussions\n[github-discussions-badge]:    https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github\n[black-badge]:                 https://img.shields.io/badge/code%20style-black-000000.svg\n[black-link]:                  https://github.com/psf/black\n[pypi-pyversion-link]:         https://pypi.python.org/pypi/fakenos/\n[pypi-pyversion-badge]:        https://img.shields.io/pypi/pyversions/fakenos.svg\n[pepy-downloads-link]:         https://pepy.tech/project/fakenos\n[pepy-downloads-badge]:        https://pepy.tech/badge/fakenos\n[github-tests-badge]:          https://github.com/dmulyalin/fakenos/actions/workflows/main.yml/badge.svg\n[github-tests-link]:           https://github.com/dmulyalin/fakenos/actions\n[pypi-latest-release-badge]:   https://img.shields.io/pypi/v/fakenos.svg\n[pypi-latest-release-link]:    https://pypi.python.org/pypi/fakenos\n',
-    'author': 'Denis Mulyalin',
-    'author_email': 'd.mulyalin@gmail.com',
-    'maintainer': 'Denis Mulyalin',
-    'maintainer_email': 'd.mulyalin@gmail.com',
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6.5,<3.10',
-}
-
-
-setup(**setup_kwargs)
```

