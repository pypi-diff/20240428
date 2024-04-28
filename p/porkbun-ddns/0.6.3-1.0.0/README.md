# Comparing `tmp/porkbun_ddns-0.6.3-py3-none-any.whl.zip` & `tmp/porkbun_ddns-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 9170 bytes, number of entries: 10
--rw-r--r--  2.0 unx       82 b- defN 24-Apr-25 12:44 porkbun_ddns/__init__.py
--rw-r--r--  2.0 unx     3254 b- defN 24-Apr-25 12:44 porkbun_ddns/cli.py
--rw-r--r--  2.0 unx     1475 b- defN 24-Apr-25 12:44 porkbun_ddns/helpers.py
--rw-r--r--  2.0 unx    10274 b- defN 24-Apr-25 12:44 porkbun_ddns/porkbun_ddns.py
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5532 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      832 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/RECORD
-10 files, 22670 bytes uncompressed, 7742 bytes compressed:  65.8%
+Zip file size: 11055 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-28 05:08 porkbun_ddns/__init__.py
+-rw-r--r--  2.0 unx     3593 b- defN 24-Apr-28 05:08 porkbun_ddns/cli.py
+-rw-r--r--  2.0 unx     3796 b- defN 24-Apr-28 05:08 porkbun_ddns/config.py
+-rw-r--r--  2.0 unx       45 b- defN 24-Apr-28 05:08 porkbun_ddns/errors.py
+-rw-r--r--  2.0 unx     1507 b- defN 24-Apr-28 05:08 porkbun_ddns/helpers.py
+-rw-r--r--  2.0 unx     9822 b- defN 24-Apr-28 05:08 porkbun_ddns/porkbun_ddns.py
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6905 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      987 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/RECORD
+12 files, 27914 bytes uncompressed, 9387 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,31 +1,37 @@
 Filename: porkbun_ddns/__init__.py
 Comment: 
 
 Filename: porkbun_ddns/cli.py
 Comment: 
 
+Filename: porkbun_ddns/config.py
+Comment: 
+
+Filename: porkbun_ddns/errors.py
+Comment: 
+
 Filename: porkbun_ddns/helpers.py
 Comment: 
 
 Filename: porkbun_ddns/porkbun_ddns.py
 Comment: 
 
-Filename: porkbun_ddns-0.6.3.dist-info/LICENSE
+Filename: porkbun_ddns-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: porkbun_ddns-0.6.3.dist-info/METADATA
+Filename: porkbun_ddns-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: porkbun_ddns-0.6.3.dist-info/WHEEL
+Filename: porkbun_ddns-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: porkbun_ddns-0.6.3.dist-info/entry_points.txt
+Filename: porkbun_ddns-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: porkbun_ddns-0.6.3.dist-info/top_level.txt
+Filename: porkbun_ddns-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: porkbun_ddns-0.6.3.dist-info/RECORD
+Filename: porkbun_ddns-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## porkbun_ddns/__init__.py

```diff
@@ -1,2 +1 @@
 from .porkbun_ddns import PorkbunDDNS
-from .porkbun_ddns import PorkbunDDNS_Error
```

## porkbun_ddns/cli.py

```diff
@@ -1,97 +1,99 @@
 import argparse
+import logging
 import sys
-import os
 import traceback
-import logging
-from porkbun_ddns import PorkbunDDNS, PorkbunDDNS_Error
 
+from porkbun_ddns import PorkbunDDNS
+from porkbun_ddns.config import extract_config, get_config_file_default
+from porkbun_ddns.errors import PorkbunDDNS_Error
 
-logger = logging.getLogger('porkbun_ddns')
+logger = logging.getLogger("porkbun_ddns")
 logger.setLevel(logging.INFO)
 handler = logging.StreamHandler(sys.stdout)
 handler.setLevel(logging.INFO)
-formatter = logging.Formatter('%(message)s')
+formatter = logging.Formatter("%(message)s")
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
 
 def main(argv=sys.argv[1:]):
     parser = argparse.ArgumentParser(
-        description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
+        description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    parser.add_argument("config", help="Path to config file")
     parser.add_argument("domain", help="Domain to be updated")
 
+    parser.add_argument("-c", "--config", help=f"Path to config file "
+                                               f"(default: {get_config_file_default()})",
+                        default=get_config_file_default())
+    parser.add_argument("-e", "--endpoint", help="The endpoint")
+    parser.add_argument("-pk", "--apikey", help="The Porkbun-API-key")
+    parser.add_argument("-sk", "--secretapikey", help="The secret API-key")
+
     subdomains = parser.add_mutually_exclusive_group()
-    subdomains.add_argument('subdomains', nargs='*',
+    subdomains.add_argument("subdomains", nargs="*",
                            default=None, help="Subdomain(s)")
 
     public_ips = parser.add_mutually_exclusive_group()
-    public_ips.add_argument('-i', '--public-ips', nargs='*',
+    public_ips.add_argument("-i", "--public-ips", nargs="*",
                             default=None, help="Public IPs (v4 and or v6)")
 
     fritzbox = parser.add_mutually_exclusive_group()
-    fritzbox.add_argument('-f', '--fritzbox', default=None,
+    fritzbox.add_argument("-f", "--fritzbox", default=None,
                           help="IP or Domain of your Fritz!Box")
 
     ip = parser.add_mutually_exclusive_group()
-    ip.add_argument('-4', '--ipv4-only', action='store_true',
+    ip.add_argument("-4", "--ipv4-only", action="store_true",
                     help="Only set/update IPv4 A Records")
-    ip.add_argument('-6', '--ipv6-only', action='store_true',
+    ip.add_argument("-6", "--ipv6-only", action="store_true",
                     help="Only set/update IPv6 AAAA Records")
 
     verbose = parser.add_mutually_exclusive_group()
-    verbose.add_argument('-v', '--verbose', action='store_true',
+    verbose.add_argument("-v", "--verbose", action="store_true",
                     help="Show Debug Output")
 
-    if argv and len(argv) == 1:
-        parser.print_help()
-        exit(1)
+    env_only = parser.add_mutually_exclusive_group()
+    env_only.add_argument("--env_only", action="store_true",
+                    help="Don't use any config, "
+                    "get all variables from the environment")
+
     if not argv:
         parser.print_help()
-        exit()
+        exit(1)
+    try:
+        args = parser.parse_args(argv)
 
-    args = parser.parse_args(argv)
+        if args.env_only:
+            args.config = None
 
-    if args.config == "-":
-        try:
-            config = {
-                "apikey": os.environ["PORKBUN_APIKEY"],
-                "secretapikey": os.environ["PORKBUN_SECRETAPIKEY"],
-            }
-            config["endpoint"] =  os.environ.get("PORKBUN_DDNS_ENDPOINT", "https://porkbun.com/api/json/v3")
-        except KeyError:
-            logger.error("Invalid config environment variables.")
-    else:
-        config = args.config
-
-    ipv4 = args.ipv4_only
-    ipv6 = args.ipv6_only
-    if not any([ipv4, ipv6]):
-        ipv4 = ipv6 = True
-
-    if args.verbose:
-        logger.setLevel(logging.DEBUG)
-        for handler in logger.handlers:
-            handler.setLevel(logging.DEBUG)
+        if args.verbose:
+            logger.setLevel(logging.DEBUG)
+            for handler in logger.handlers:
+                handler.setLevel(logging.DEBUG)
+
+        config = extract_config(args)
+        ipv4 = args.ipv4_only
+        ipv6 = args.ipv6_only
+        if not any([ipv4, ipv6]):
+            ipv4 = ipv6 = True
 
-    try:
         porkbun_ddns = PorkbunDDNS(config=config, domain=args.domain,
                                    public_ips=args.public_ips, fritzbox_ip=args.fritzbox,
                                    ipv4=ipv4, ipv6=ipv6)
         if args.subdomains:
             for s in args.subdomains:
                 porkbun_ddns.set_subdomain(s)
                 porkbun_ddns.update_records()
         else:
             porkbun_ddns.update_records()
     except PorkbunDDNS_Error as e:
         logger.error("Error: " + str(e))
+        exit(1)
     except Exception as e:
         logger.error("This shouldn't have happened!")
         logger.error("Error: " + str(e))
         logger.error(traceback.format_exc())
+        exit(1)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## porkbun_ddns/helpers.py

```diff
@@ -1,40 +1,43 @@
+import logging
 import urllib.request
 import xml.etree.ElementTree as ET
-import logging
 
 logger = logging.getLogger()
 
 
 def get_ips_from_fritzbox(fritzbox_ip):
     """Retrieves the IP address of the Fritzbox router's external network interface.
 
     Args:
+    ----
         fritzbox_ip (str): The IP address of the Fritzbox router.
 
     Returns:
+    -------
         str: The IP address of the Fritzbox router's external network interface.
 
     Raises:
+    ------
         urllib.error.URLError: If there is a problem opening the URL.
 
         ValueError: If the provided `fritzbox_ip` is not a valid IP address.
 
         AttributeError: If the requested field is not found in the XML response.
-    """
 
-    schema = 'GetExternalIPAddress'
-    field = 'NewExternalIPAddress'
+    """
+    schema = "GetExternalIPAddress"
+    field = "NewExternalIPAddress"
 
     req = urllib.request.Request(
-        'http://' + fritzbox_ip + ':49000/igdupnp/control/WANIPConn1')
-    req.add_header('Content-Type', 'text/xml; charset="utf-8"')
+        "http://" + fritzbox_ip + ":49000/igdupnp/control/WANIPConn1")
+    req.add_header("Content-Type", 'text/xml; charset="utf-8"')
     req.add_header(
-        'SOAPAction', 'urn:schemas-upnp-org:service:WANIPConnection:1#' + schema)
+        "SOAPAction", "urn:schemas-upnp-org:service:WANIPConnection:1#" + schema)
     data = '<?xml version="1.0" encoding="utf-8"?>' + \
         '<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" s:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/">' + \
-        '<s:Body>' + \
-        '<u:' + schema + ' xmlns:u="urn:schemas-upnp-org:service:WANIPConnection:1" />' + \
-        '</s:Body>' + \
-        '</s:Envelope>'
-    req.data = data.encode('utf8')
-    return ET.fromstring(urllib.request.urlopen(req).read()).find('.//' + field).text
+        "<s:Body>" + \
+        "<u:" + schema + ' xmlns:u="urn:schemas-upnp-org:service:WANIPConnection:1" />' + \
+        "</s:Body>" + \
+        "</s:Envelope>"
+    req.data = data.encode("utf8")
+    return ET.fromstring(urllib.request.urlopen(req).read()).find(".//" + field).text
```

## porkbun_ddns/porkbun_ddns.py

```diff
@@ -1,229 +1,207 @@
 from __future__ import annotations
 
-import logging
 import json
-import ipaddress
+import logging
 import urllib.request
+from ipaddress import IPv4Address, IPv6Address, ip_address
 from urllib.error import HTTPError, URLError
-from porkbun_ddns.helpers import get_ips_from_fritzbox
-
-logger = logging.getLogger('porkbun_ddns')
 
+from porkbun_ddns.config import Config
+from porkbun_ddns.errors import PorkbunDDNS_Error
+from porkbun_ddns.helpers import get_ips_from_fritzbox
 
-class PorkbunDDNS_Error(Exception):
-    pass
+logger = logging.getLogger("porkbun_ddns")
 
 
-class PorkbunDDNS():
+class PorkbunDDNS:
     """A class for updating dynamic DNS records for a Porkbun domain.
     """
 
     def __init__(
-        self,
-        config: dict | str,
-        domain: str,
-        public_ips: list | None = None,
-        fritzbox_ip: str | None = None,
-        ipv4: bool = True,
-        ipv6: bool = True
+            self,
+            config: Config,
+            domain: str,
+            public_ips: list | None = None,
+            fritzbox_ip: str | None = None,
+            ipv4: bool = True,
+            ipv6: bool = True,
     ) -> None:
-        if isinstance(config, dict):
-            self.config = config
-        else:
-            if isinstance(config, str):
-                try:
-                    self._load_config(config)
-                except FileNotFoundError as err:
-                    raise FileNotFoundError(
-                        "Config path is invalid!\nPath:\n{}".format(config)) from err
-            else:
-                raise TypeError("Invalid config! Config should be a str (filepath) or dict!\nYour config:\n{}\nType: {}".format(
-                    config, type(config)))
 
-        self._check_config()
+        self.config = config._asdict()
         self.static_ips = public_ips
         self.domain = domain.lower()
         self.records = None
         self.fritzbox_ip = fritzbox_ip
         self.ipv4 = ipv4
         self.ipv6 = ipv6
         self.fqdn = self.domain
-        self.subdomain = '@'
-
-    def _load_config(self, config: str) -> None:
-        """Load a JSON configuration file.
-        """
-        with open(config) as fid:
-            self.config = json.load(fid)
-
-    def _check_config(self) -> None:
-        """Check if the configuration is valid.
-        """
-        required_keys = ["secretapikey", "apikey"]
-        if all(x not in self.config for x in required_keys):
-            raise PorkbunDDNS_Error("Missing keys! All of the following are required: '{}'\nYour config:\n{}".format(
-                required_keys, self.config))
-        if 'endpoint' not in self.config.keys():
-            self.config["endpoint"] = "https://porkbun.com/api/json/v3"
+        self.subdomain = "@"
 
     def set_subdomain(self, subdomain: str) -> None:
         self.subdomain = subdomain.lower()
-        if self.subdomain == '@':
+        if self.subdomain == "@":
             self.fqdn = self.domain
         else:
-            self.fqdn = '.'.join([self.subdomain, self.domain])
+            self.fqdn = ".".join([self.subdomain, self.domain])
 
     def get_public_ips(self) -> list:
         """Retrieve the public IP addresses of the network.
         """
+        public_ips: set | list | None
         if self.static_ips:
             public_ips = self.static_ips
         else:
             public_ips = []
             if self.fritzbox_ip:
                 if self.ipv4:
                     public_ips.append(
                         get_ips_from_fritzbox(self.fritzbox_ip))
             else:
                 if self.ipv4:
-                    urls = ['https://v4.ident.me',
-                    'https://api.ipify.org',
-                    'https://ipv4.icanhazip.com']
+                    urls = ["https://v4.ident.me",
+                            "https://api.ipify.org",
+                            "https://ipv4.icanhazip.com"]
                     for url in urls:
                         try:
-                            with urllib.request.urlopen(url) as response:
+                            with urllib.request.urlopen(url, timeout=10) as response:
                                 if response.getcode() == 200:
-                                    public_ips.append(response.read().decode('utf-8'))
+                                    public_ips.append(
+                                        response.read().decode("utf-8"))
                                     break
-                                logger.warning("Failed to retrieve IPv4 Address from %s! HTTP status code: %s", url, str(response.code()))
+                                logger.warning(
+                                    "Failed to retrieve IPv4 Address from %s! HTTP status code: %s", url, str(response.code()))
                         except URLError as err:
-                            logger.warning("Error reaching %s! Error: %s", url, repr(err))
+                            logger.warning(
+                                "Error reaching %s! - %s", url, err.reason)
                 if self.ipv6:
-                    urls = ['https://v6.ident.me',
-                    'https://api6.ipify.org',
-                    'https://ipv6.icanhazip.com']
+                    urls = ["https://v6.ident.me",
+                            "https://api6.ipify.org",
+                            "https://ipv6.icanhazip.com"]
                     for url in urls:
                         try:
-                            with urllib.request.urlopen(url) as response:
+                            with urllib.request.urlopen(url, timeout=10) as response:
                                 if response.getcode() == 200:
-                                    public_ips.append(response.read().decode('utf-8'))
+                                    public_ips.append(
+                                        response.read().decode("utf-8"))
                                     break
-                                logger.warning("Failed to retrieve IPv6 Address from %s! HTTP status code: %s", url, str(response.code()))
+                                logger.warning(
+                                    "Failed to retrieve IPv6 Address from %s! HTTP status code: %s", url, str(response.code()))
                         except URLError as err:
-                            logger.warning("Error reaching %s! Error: %s", url, repr(err))
+                            logger.warning(
+                                "Error reaching %s! - %s", url, err.reason)
 
             public_ips = set(public_ips)
 
         if not public_ips:
-            raise PorkbunDDNS_Error('Failed to obtain IP Addresses!')
+            raise PorkbunDDNS_Error("Failed to obtain IP Addresses!")
 
-        return [ipaddress.ip_address(x) for x in public_ips if not ipaddress.ip_address(x).is_unspecified]
+        return [ip_address(x) for x in public_ips if not ip_address(x).is_unspecified]
 
-    def _api(self, target: str, data: dict = None) -> dict:
+    def _api(self, target: str, data: dict | None = None) -> dict:
         """Send an API request to a specified target.
         """
-
         data = data or self.config
-        req = urllib.request.Request(self.config['endpoint'] + target)
-        req.data = json.dumps(data).encode('utf8')
+        req = urllib.request.Request(self.config["endpoint"] + target)
+        req.data = json.dumps(data).encode("utf8")
         try:
-            response = urllib.request.urlopen(req).read()
+            response = urllib.request.urlopen(req,  timeout=10).read()
         except HTTPError as err:
             if err.code == 400:
-                raise PorkbunDDNS_Error('Invalid API Keys!')
+                raise PorkbunDDNS_Error("Invalid API Keys!")
             else:
                 raise err
-        return json.loads(response.decode('utf-8'))
+        return json.loads(response.decode("utf-8"))
 
     def get_records(self) -> dict:
         """Retrieve the DNS records for the specified domain.
         """
-
         records = self._api("/dns/retrieve/" + self.domain)
         if records["status"] == "SUCCESS":
-            return records['records']
+            return records["records"]
         else:
             raise PorkbunDDNS_Error(
-                'Failed to get records.\n' +
-                'Make sure you specified the correct domain ({}),\n'.format(self.domain) +
-                'and that API access has been enabled for this domain.'
+                "Failed to get records.\n" +
+                f"Make sure you specified the correct domain ({self.domain}),\n" +
+                "and that API access has been enabled for this domain.",
             )
 
     def update_records(self):
         """Update DNS records for the specified domain.
         """
         self.records = self.get_records()
-        domain_names = [x['name'] for x in self.records if x['type']
+        domain_names = [x["name"] for x in self.records if x["type"]
                         in ["A", "AAAA", "ALIAS", "CNAME"]]
         for ip in self.get_public_ips():
             record_type = "A" if ip.version == 4 else "AAAA"
             if self.fqdn in domain_names:
                 for i in self.records:
                     if i["name"] == self.fqdn:
                         # Overwrite ALIAS and CNAME
                         if i["type"] in ["ALIAS", "CNAME"]:
-                            logger.debug('Overwrite ALIAS and CNAME, with:\n{}'.format(json.dumps(
+                            logger.debug("Overwrite ALIAS and CNAME, with:\n{}".format(json.dumps(
                                 {"name": self.fqdn, "type": record_type, "content": str(ip.exploded)})))
-                            self._delete_record(i['id'])
+                            self._delete_record(i["id"])
                             self._create_records(ip, record_type)
                         # Update existing entry
-                        if i["type"] == record_type and i['content'] != ip.exploded:
-                            logger.debug('Update existing entry, with:\n{}'.format(json.dumps(
+                        if i["type"] == record_type and i["content"] != ip.exploded:
+                            logger.debug("Update existing entry, with:\n{}".format(json.dumps(
                                 {"name": self.fqdn, "type": record_type, "content": str(ip.exploded)})))
-                            self._delete_record(i['id'])
+                            self._delete_record(i["id"])
                             self._create_records(ip, record_type)
                         # Create missing A or AAAA entry
-                        if i["type"] in ["A", "AAAA"] and record_type not in [x['type'] for x in self.records if x['name'] == self.fqdn]:
-                            logger.debug('Create missing A or AAAA entry, with:\n{}'.format(json.dumps(
+                        if i["type"] in ["A", "AAAA"] and record_type not in [x["type"] for x in self.records if
+                                                                              x["name"] == self.fqdn]:
+                            logger.debug("Create missing A or AAAA entry, with:\n{}".format(json.dumps(
                                 {"name": self.fqdn, "type": record_type, "content": str(ip.exploded)})))
                             self._create_records(ip, record_type)
                             # Update records
                             self.records = self.get_records()
                         # Everything is up to date
-                        if i["type"] == record_type and i['content'] == ip.exploded:
-                            logger.info('{}-Record of {} is up to date!'.format(
+                        if i["type"] == record_type and i["content"] == ip.exploded:
+                            logger.info("{}-Record of {} is up to date!".format(
                                 i["type"], i["name"]))
             else:
-                logger.debug('Create new record, with:\n{}'.format(json.dumps(
+                logger.debug("Create new record, with:\n{}".format(json.dumps(
                     {"name": self.fqdn, "type": record_type, "content": str(ip.exploded)})))
                 # Create new record
                 self._create_records(ip, record_type)
                 # Update records
                 self.records = self.get_records()
 
     def delete_records(self):
-        """Delete A and AAAA DNS record for set record.
-        """
-        self.records = self.get_records()
-        domain_names = [x['name'] for x in self.records if x['type']
-                        in ["A", "AAAA"]]
-        if self.fqdn in domain_names:
-            for i in self.records:
-                if i["name"] == self.fqdn and i['type'] in ["A", "AAAA"]:
-                    logger.debug('Deleting existing entry:\n{}'.format(json.dumps(
-                        {"name": self.fqdn, "type": i['type'], "content": str(i['content'])})))
-                    self._delete_record(i['id'])
-        else:
-            logger.debug('Record not found:\n{}'.format(json.dumps(
-                {"name": self.fqdn, "type": i['type'], "content": str(i['content'])})))
+            """Delete A and AAAA DNS record for set record.
+            """
+            self.records = self.get_records()
+            domain_names = [x["name"] for x in self.records if x["type"]
+                            in ["A", "AAAA"]]
+            if self.fqdn in domain_names:
+                for i in self.records:
+                    if i["name"] == self.fqdn and i["type"] in ["A", "AAAA"]:
+                        logger.debug("Deleting existing entry:\n{}".format(json.dumps(
+                            {"name": self.fqdn, "type": i["type"], "content": str(i["content"])})))
+                        self._delete_record(i["id"])
+            else:
+                logger.debug("Record not found:\n{}".format(json.dumps(
+                    {"name": self.fqdn, "type": i["type"], "content": str(i["content"])})))
 
     def _delete_record(self, domain_id: str):
         """Delete a DNS record with the given domain ID.
         """
+        if self.records:
+            type, name, content = [(x["type"], x["name"], x["content"])
+                                   for x in self.records if x["id"] == domain_id][0]
+            status = self._api("/dns/delete/" + self.domain + "/" + domain_id)
+            logger.info("Deleting {}-Record for {} with content: {}, Status: {}".format(type,
+                                                                                        name, content,
+                                                                                        status["status"]))
 
-        type, name, content = [(x['type'], x['name'], x['content'])
-                               for x in self.records if x['id'] == domain_id][0]
-        status = self._api("/dns/delete/" + self.domain + "/" + domain_id)
-        logger.info('Deleting {}-Record for {} with content: {}, Status: {}'.format(type,
-                                                                                    name, content, status["status"]))
-
-    def _create_records(self, ip: ipaddress, record_type: str):
+    def _create_records(self, ip: IPv4Address | IPv6Address, record_type: str):
         """Create DNS records for the subdomain with the given IP address and type.
         """
-
         data = self.config.copy()
         data.update({"name": self.subdomain, "type": record_type,
-                    "content": ip.exploded, "ttl": 600})
+                     "content": ip.exploded, "ttl": 600})
         status = self._api("/dns/create/" + self.domain, data)
-        logger.info('Creating {}-Record for {} with content: {}, Status: {}'.format(record_type,
-                                                                                    self.fqdn, ip.exploded, status["status"]))
+        logger.info("Creating {}-Record for {} with content: {}, Status: {}".format(record_type,
+                                                                                    self.fqdn, ip.exploded,
+                                                                                    status["status"]))
```

## Comparing `porkbun_ddns-0.6.3.dist-info/LICENSE` & `porkbun_ddns-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `porkbun_ddns-0.6.3.dist-info/RECORD` & `porkbun_ddns-1.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-porkbun_ddns/__init__.py,sha256=4E9knps0KH0NhbKGNNEeixpexHTNnxHbfUvhJD7rOUU,82
-porkbun_ddns/cli.py,sha256=WQJEcM4qsmpODHd83X_gA9fDJ-OTNbjzceZlO4EpL24,3254
-porkbun_ddns/helpers.py,sha256=i3OPqrDzMJTuhuGC18V2qerYI_i77dSF-nFIQMBcSEM,1475
-porkbun_ddns/porkbun_ddns.py,sha256=RwhP3CRGSTRHxtgYrLhHaF1tzDCTncNaJWFDQfuZeNU,10274
-porkbun_ddns-0.6.3.dist-info/LICENSE,sha256=WbmjIVUkxwQ1vDNiEe2eMKL3-6nYRBN1qUv7rdvvSvY,1061
-porkbun_ddns-0.6.3.dist-info/METADATA,sha256=rJyI6UUe0rHD9KbJbn0mXqfNbWqpr-GKOKYTCr-DcTs,5532
-porkbun_ddns-0.6.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-porkbun_ddns-0.6.3.dist-info/entry_points.txt,sha256=Ux4_6ekA_PZiOxw-7MbJOvQVo_7IJQzaYS24EzSjwbg,55
-porkbun_ddns-0.6.3.dist-info/top_level.txt,sha256=8hi5L7CGOlYLIOlnnPPToRxZqnZ1UkpUmCYbgYZO2JA,13
-porkbun_ddns-0.6.3.dist-info/RECORD,,
+porkbun_ddns/__init__.py,sha256=XumKSWFK5qfGiCSkPPcNCaE44OLJ4r1upBBwJm5s_1Q,38
+porkbun_ddns/cli.py,sha256=0ulurkVBJNBKNAYAX_4vVbCjN75jgACPqA-FFKRcSi8,3593
+porkbun_ddns/config.py,sha256=QMvapsNLQw8HajK6XkW6asJz-XsMs51mnmjQxXz4PVw,3796
+porkbun_ddns/errors.py,sha256=Kv2CY-7lQf6WtYJGUfjjGFKMpvgP85qo4SX38f09_NU,45
+porkbun_ddns/helpers.py,sha256=j6_auR6ffQr51NFOY1i9-EJ7_D4FPFovhpVf5c3hkbE,1507
+porkbun_ddns/porkbun_ddns.py,sha256=h6-HyGfwTENNk5FRKUJcsxT3XOinrUuyjfwNCufEBik,9822
+porkbun_ddns-1.0.0.dist-info/LICENSE,sha256=WbmjIVUkxwQ1vDNiEe2eMKL3-6nYRBN1qUv7rdvvSvY,1061
+porkbun_ddns-1.0.0.dist-info/METADATA,sha256=EscoXJVf_3SwpHtg50btUQe8YMItxY4R9pIKaStVgEA,6905
+porkbun_ddns-1.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+porkbun_ddns-1.0.0.dist-info/entry_points.txt,sha256=Ux4_6ekA_PZiOxw-7MbJOvQVo_7IJQzaYS24EzSjwbg,55
+porkbun_ddns-1.0.0.dist-info/top_level.txt,sha256=8hi5L7CGOlYLIOlnnPPToRxZqnZ1UkpUmCYbgYZO2JA,13
+porkbun_ddns-1.0.0.dist-info/RECORD,,
```

