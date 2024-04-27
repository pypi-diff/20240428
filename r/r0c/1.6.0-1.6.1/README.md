# Comparing `tmp/r0c-1.6.0.tar.gz` & `tmp/r0c-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r0c-1.6.0.tar", last modified: Thu Apr  4 23:56:32 2024, max compression
+gzip compressed data, was "r0c-1.6.1.tar", last modified: Sat Apr 27 23:07:47 2024, max compression
```

## Comparing `r0c-1.6.0.tar` & `r0c-1.6.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.988482 r0c-1.6.0/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-19 15:14:09.000000 r0c-1.6.0/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)      248 2024-04-04 23:56:32.000000 r0c-1.6.0/MANIFEST.in
--rw-r--r--   0 ed        (1000) ed        (1000)     9139 2024-04-04 23:56:32.988482 r0c-1.6.0/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     7219 2024-04-02 16:47:55.000000 r0c-1.6.0/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.985482 r0c-1.6.0/clients/
--rwxr-xr-x   0 ed        (1000) ed        (1000)     1002 2021-09-19 15:14:09.000000 r0c-1.6.0/clients/bash.sh
--rw-r--r--   0 ed        (1000) ed        (1000)     5605 2023-09-19 18:59:16.000000 r0c-1.6.0/clients/powershell.ps1
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.985482 r0c-1.6.0/docs/
--rw-r--r--   0 ed        (1000) ed        (1000)      333 2021-09-19 15:14:09.000000 r0c-1.6.0/docs/help-about.md
--rw-r--r--   0 ed        (1000) ed        (1000)     2730 2024-04-04 22:12:04.000000 r0c-1.6.0/docs/help-commands.md
--rw-r--r--   0 ed        (1000) ed        (1000)      836 2023-09-17 18:02:49.000000 r0c-1.6.0/docs/help-hotkeys.md
--rw-r--r--   0 ed        (1000) ed        (1000)      197 2023-09-19 19:21:36.000000 r0c-1.6.0/docs/help-topics.md
--rw-r--r--   0 ed        (1000) ed        (1000)      670 2023-09-20 00:08:59.000000 r0c-1.6.0/docs/help-ui.md
--rw-r--r--   0 ed        (1000) ed        (1000)     2367 2024-04-04 23:26:14.000000 r0c-1.6.0/docs/todo.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.987482 r0c-1.6.0/r0c/
--rw-------   0 ed        (1000) ed        (1000)     2543 2022-08-31 21:02:50.000000 r0c-1.6.0/r0c/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    24287 2024-04-04 23:35:45.000000 r0c-1.6.0/r0c/__main__.py
--rw-------   0 ed        (1000) ed        (1000)      211 2024-04-04 23:27:04.000000 r0c-1.6.0/r0c/__version__.py
--rw-------   0 ed        (1000) ed        (1000)     8453 2024-04-04 22:25:29.000000 r0c-1.6.0/r0c/chat.py
--rw-------   0 ed        (1000) ed        (1000)     2227 2022-09-01 21:50:46.000000 r0c-1.6.0/r0c/diag.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3538 2023-10-09 23:43:46.000000 r0c-1.6.0/r0c/inetcat.py
--rw-r--r--   0 ed        (1000) ed        (1000)     8648 2024-04-04 23:36:51.000000 r0c-1.6.0/r0c/irc.py
--rw-r--r--   0 ed        (1000) ed        (1000)    13828 2023-10-09 23:43:58.000000 r0c-1.6.0/r0c/itelnet.py
--rw-r--r--   0 ed        (1000) ed        (1000)   108688 2024-04-04 22:28:29.000000 r0c-1.6.0/r0c/ivt100.py
--rw-r--r--   0 ed        (1000) ed        (1000)    37076 2024-04-04 23:44:07.000000 r0c-1.6.0/r0c/user.py
--rw-r--r--   0 ed        (1000) ed        (1000)    20569 2024-04-04 22:23:55.000000 r0c-1.6.0/r0c/util.py
--rw-------   0 ed        (1000) ed        (1000)    21402 2024-04-04 23:43:38.000000 r0c-1.6.0/r0c/world.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.988482 r0c-1.6.0/r0c.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)     9139 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)      493 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       42 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        4 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2024-04-04 23:56:32.988482 r0c-1.6.0/setup.cfg
--rwxr-xr-x   0 ed        (1000) ed        (1000)     4658 2023-05-14 22:32:58.000000 r0c-1.6.0/setup.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-27 23:07:47.059800 r0c-1.6.1/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-19 15:14:09.000000 r0c-1.6.1/LICENSE
+-rw-r--r--   0 ed        (1000) ed        (1000)      248 2024-04-27 23:07:46.000000 r0c-1.6.1/MANIFEST.in
+-rw-r--r--   0 ed        (1000) ed        (1000)    10187 2024-04-27 23:07:47.059800 r0c-1.6.1/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)     8227 2024-04-27 23:02:56.000000 r0c-1.6.1/README.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-27 23:07:47.056800 r0c-1.6.1/clients/
+-rwxr-xr-x   0 ed        (1000) ed        (1000)     1002 2021-09-19 15:14:09.000000 r0c-1.6.1/clients/bash.sh
+-rw-r--r--   0 ed        (1000) ed        (1000)     5605 2023-09-19 18:59:16.000000 r0c-1.6.1/clients/powershell.ps1
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-27 23:07:47.056800 r0c-1.6.1/docs/
+-rw-r--r--   0 ed        (1000) ed        (1000)      333 2021-09-19 15:14:09.000000 r0c-1.6.1/docs/help-about.md
+-rw-r--r--   0 ed        (1000) ed        (1000)     2730 2024-04-04 22:12:04.000000 r0c-1.6.1/docs/help-commands.md
+-rw-r--r--   0 ed        (1000) ed        (1000)      836 2023-09-17 18:02:49.000000 r0c-1.6.1/docs/help-hotkeys.md
+-rw-r--r--   0 ed        (1000) ed        (1000)      197 2023-09-19 19:21:36.000000 r0c-1.6.1/docs/help-topics.md
+-rw-r--r--   0 ed        (1000) ed        (1000)      670 2023-09-20 00:08:59.000000 r0c-1.6.1/docs/help-ui.md
+-rw-r--r--   0 ed        (1000) ed        (1000)     2367 2024-04-04 23:26:14.000000 r0c-1.6.1/docs/todo.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-27 23:07:47.058801 r0c-1.6.1/r0c/
+-rw-------   0 ed        (1000) ed        (1000)     2543 2022-08-31 21:02:50.000000 r0c-1.6.1/r0c/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    24586 2024-04-26 22:09:48.000000 r0c-1.6.1/r0c/__main__.py
+-rw-------   0 ed        (1000) ed        (1000)      212 2024-04-27 19:23:22.000000 r0c-1.6.1/r0c/__version__.py
+-rw-------   0 ed        (1000) ed        (1000)     8453 2024-04-04 22:25:29.000000 r0c-1.6.1/r0c/chat.py
+-rw-------   0 ed        (1000) ed        (1000)     2227 2022-09-01 21:50:46.000000 r0c-1.6.1/r0c/diag.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3538 2023-10-09 23:43:46.000000 r0c-1.6.1/r0c/inetcat.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     8648 2024-04-04 23:36:51.000000 r0c-1.6.1/r0c/irc.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    13828 2023-10-09 23:43:58.000000 r0c-1.6.1/r0c/itelnet.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   109350 2024-04-27 21:14:11.000000 r0c-1.6.1/r0c/ivt100.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    37422 2024-04-27 21:17:13.000000 r0c-1.6.1/r0c/user.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20569 2024-04-04 22:23:55.000000 r0c-1.6.1/r0c/util.py
+-rw-------   0 ed        (1000) ed        (1000)    21402 2024-04-27 18:34:21.000000 r0c-1.6.1/r0c/world.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-27 23:07:47.059800 r0c-1.6.1/r0c.egg-info/
+-rw-r--r--   0 ed        (1000) ed        (1000)    10187 2024-04-27 23:07:46.000000 r0c-1.6.1/r0c.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)      493 2024-04-27 23:07:46.000000 r0c-1.6.1/r0c.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        1 2024-04-27 23:07:46.000000 r0c-1.6.1/r0c.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       42 2024-04-27 23:07:46.000000 r0c-1.6.1/r0c.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        4 2024-04-27 23:07:46.000000 r0c-1.6.1/r0c.egg-info/top_level.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       38 2024-04-27 23:07:47.059800 r0c-1.6.1/setup.cfg
+-rwxr-xr-x   0 ed        (1000) ed        (1000)     4658 2023-05-14 22:32:58.000000 r0c-1.6.1/setup.py
```

### Comparing `r0c-1.6.0/LICENSE` & `r0c-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/PKG-INFO` & `r0c-1.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r0c
-Version: 1.6.0
+Version: 1.6.1
 Summary: retr0chat telnet/vt100 chat server
 Home-page: https://github.com/9001/r0c
 Author: ed
 Author-email: r0c@ocv.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -49,28 +49,29 @@
 imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
 
 retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
 
 * tries to be irssi
 * zero dependencies on python 2.6, 2.7, 3.x
 * supports telnet, netcat, /dev/tcp, TLS clients
-* is not an irc server, but can bridge to/from irc servers
+* is not an irc server, but can [bridge to/from irc servers](#irc)
 * [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
 * fallbacks for inhumane conditions
   * linemode
   * no vt100 / ansi escape codes
 
 ## endorsements
 
 * the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
 
 ## compatibility
 
 * 1980: [TVI 920C](https://a.ocv.me/pub/g/nerd-stuff/r0c-tvi-920c.jpg)
 * 1987: [IBM 3151](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.jpg) (also [video](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.webm)), using gnu-screen to translate VT100 sequences
+* 1993: [windows 3.11](https://a.ocv.me/pub/g/nerd-stuff/r0c-for-workgroups.png)
 
 ## features
 
 irc-like:
 * public channels with persistent history (pgup/pgdn)
 * private messages (`/msg acidburn hey`)
 * nick completion with `Tab ↹`
@@ -80,15 +81,15 @@
 
 technical:
 * client behavior detection (echo, colors, charset, newline)
 * message input with readline-like editing (arrow-left/right, home/end, backspace)
   * history of sent messages (arrow-up/down)
 * bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
 * fast enough; 600 clients @ 750 msgs/sec, or 1'000 cli @ 350 msg/s
-* bridge several irc channels from several networks into one r0c channel
+* [bridge](#irc) several irc channels from several networks into one r0c channel
 
 ## windows clients
 
 * use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
 * or [the powershell client](https://github.com/9001/r0c/blob/master/clients/powershell.ps1)
 * or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
 
@@ -140,14 +141,30 @@
 
 you can run it as a service so it autostarts on boot:
 
 * on most linux distros: [systemd service](https://github.com/9001/r0c/blob/master/docs/systemd/r0c.service) (automatically does port-forwarding)
 * on alpine / gentoo: [openrc service](https://github.com/9001/r0c/blob/master/docs/openrc/r0c)
 * on windows: [nssm](https://nssm.cc/) probably
 
+## irc
+
+if you want to connect your r0c instance to an irc network and bridge channels between them, you can do that:
+
+![screenshot of a r0c channel being bridged to an irc channel](https://github.com/9001/r0c/blob/master/docs/r0c-irc.png)
+
+```bash
+python3 r0c.py --ircn a,127.0.0.1,6667,r0c --ircb a,chat,g
+```
+
+run that command to start r0c with irc bridging enabled; r0c will then connect to an irc server (which we nicknamed `a`) on `127.0.0.1:6667` with the irc-nick `r0c` and bridge the irc-channel `#chat` with the r0c-channel `#g`
+
+if you then start an irc server locally, for example [miniircd](https://github.com/jrosdahl/miniircd/blob/master/miniircd) by running `python3 miniircd --verbose` then you're all set, people can now join r0c by connecting via irc
+
+to bridge additional channels on the same network, add more `--ircb` args, for example `--ircb a,tech,tech` like in the screenshot, and optionally add more networks with `--ircn`
+
 ## firewall rules
 
 skip this section if:
 * you are using the systemd service
 * or you are running as root and do not have a firewall
 * or you're on windows
```

### Comparing `r0c-1.6.0/README.md` & `r0c-1.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
 
 retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
 
 * tries to be irssi
 * zero dependencies on python 2.6, 2.7, 3.x
 * supports telnet, netcat, /dev/tcp, TLS clients
-* is not an irc server, but can bridge to/from irc servers
+* is not an irc server, but can [bridge to/from irc servers](#irc)
 * [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
 * fallbacks for inhumane conditions
   * linemode
   * no vt100 / ansi escape codes
 
 ## endorsements
 
 * the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
 
 ## compatibility
 
 * 1980: [TVI 920C](https://a.ocv.me/pub/g/nerd-stuff/r0c-tvi-920c.jpg)
 * 1987: [IBM 3151](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.jpg) (also [video](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.webm)), using gnu-screen to translate VT100 sequences
+* 1993: [windows 3.11](https://a.ocv.me/pub/g/nerd-stuff/r0c-for-workgroups.png)
 
 ## features
 
 irc-like:
 * public channels with persistent history (pgup/pgdn)
 * private messages (`/msg acidburn hey`)
 * nick completion with `Tab ↹`
@@ -44,15 +45,15 @@
 
 technical:
 * client behavior detection (echo, colors, charset, newline)
 * message input with readline-like editing (arrow-left/right, home/end, backspace)
   * history of sent messages (arrow-up/down)
 * bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
 * fast enough; 600 clients @ 750 msgs/sec, or 1'000 cli @ 350 msg/s
-* bridge several irc channels from several networks into one r0c channel
+* [bridge](#irc) several irc channels from several networks into one r0c channel
 
 ## windows clients
 
 * use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
 * or [the powershell client](clients/powershell.ps1)
 * or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
 
@@ -104,14 +105,30 @@
 
 you can run it as a service so it autostarts on boot:
 
 * on most linux distros: [systemd service](docs/systemd/r0c.service) (automatically does port-forwarding)
 * on alpine / gentoo: [openrc service](docs/openrc/r0c)
 * on windows: [nssm](https://nssm.cc/) probably
 
+## irc
+
+if you want to connect your r0c instance to an irc network and bridge channels between them, you can do that:
+
+![screenshot of a r0c channel being bridged to an irc channel](docs/r0c-irc.png)
+
+```bash
+python3 r0c.py --ircn a,127.0.0.1,6667,r0c --ircb a,chat,g
+```
+
+run that command to start r0c with irc bridging enabled; r0c will then connect to an irc server (which we nicknamed `a`) on `127.0.0.1:6667` with the irc-nick `r0c` and bridge the irc-channel `#chat` with the r0c-channel `#g`
+
+if you then start an irc server locally, for example [miniircd](https://github.com/jrosdahl/miniircd/blob/master/miniircd) by running `python3 miniircd --verbose` then you're all set, people can now join r0c by connecting via irc
+
+to bridge additional channels on the same network, add more `--ircb` args, for example `--ircb a,tech,tech` like in the screenshot, and optionally add more networks with `--ircn`
+
 ## firewall rules
 
 skip this section if:
 * you are using the systemd service
 * or you are running as root and do not have a firewall
 * or you're on windows
```

### Comparing `r0c-1.6.0/clients/bash.sh` & `r0c-1.6.1/clients/bash.sh`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/clients/powershell.ps1` & `r0c-1.6.1/clients/powershell.ps1`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/docs/help-commands.md` & `r0c-1.6.1/docs/help-commands.md`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/docs/help-hotkeys.md` & `r0c-1.6.1/docs/help-hotkeys.md`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/docs/help-ui.md` & `r0c-1.6.1/docs/help-ui.md`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/docs/todo.md` & `r0c-1.6.1/docs/todo.md`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c/__init__.py` & `r0c-1.6.1/r0c/__init__.py`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c/__main__.py` & `r0c-1.6.1/r0c/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,23 @@
         ar.ircb = ar.ircb or []
         ar.i_rate_b, ar.i_rate_s = [float(x) for x in ar.i_rate.split(",")]
         ar.proxy = ar.proxy.split(",")
         if "127.0.0.1" in ar.proxy or "::1" in ar.proxy:
             t = "\033[33mWARNING: you have localhost in --proxy, you probably want --ara too\033[0m"
             print(t)
 
+        taken = {}
+        for zs in "pt pn tpt tpn".split():
+            zi = getattr(ar, zs, 0)
+            if zi in taken:
+                t = "port %d was specified for both -%s and -%s"
+                raise Exception(t % (zi, taken[zi], zs))
+            if zi:
+                taken[zi] = zs
+
         Util.HEX_WIDTH = ar.hex_w
         Itelnet.init(ar)
 
         cert = EP.app + "cert.pem"
         if ar.tpt or ar.tpn:
             print("  *  Loading certificate {0}".format(cert))
             import ssl
```

### Comparing `r0c-1.6.0/r0c/chat.py` & `r0c-1.6.1/r0c/chat.py`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c/diag.py` & `r0c-1.6.1/r0c/diag.py`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c/inetcat.py` & `r0c-1.6.1/r0c/inetcat.py`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c/irc.py` & `r0c-1.6.1/r0c/irc.py`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c/itelnet.py` & `r0c-1.6.1/r0c/itelnet.py`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c/ivt100.py` & `r0c-1.6.1/r0c/ivt100.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,15 @@
         try:
             x = b"\xfe"
             x.decode("utf-8")
         except UnicodeDecodeError as uee:
             self.uee_offset = -uee.start
 
         # outgoing data
+        self.info_q = []
         self.outbox = []
         self.replies = []
         self.last_tx = None
 
         # incoming data
         self.backlog = b""
         self.in_bytes = b""
@@ -369,14 +370,15 @@
         self.handshake_sz = False
         self.handshake_world = False
         self.last_2smol = 0
         self.last_beep = 0
         self.show_hilight_tutorial = True
         self.need_full_redraw = False
         self.too_small = False
+        self.bad_naws = False
         self.screen = []
         self.w = 80
         self.h = 24
         self.first_dsr = 0.0
         self.pending_size_request = 0.0
         self.size_request_action = None
         self.re_cursor_pos = re.compile(r"\033\[([0-9]{1,4});([0-9]{1,4})R")
@@ -437,14 +439,16 @@
         # putty
         self.add_esc(u"\x1b\x5b\x33\x7e", "del")
 
         # hotkeys
         self.add_esc(u"\x0c", "redraw")  # ^L (readline-compat)
         self.add_esc(u"\x12", "redraw")  # ^R
         self.add_esc(u"\x0e", "view")  # ^N
+        self.add_esc(u"\x15", "pgup")  # ^U
+        self.add_esc(u"\x04", "pgdn")  # ^D
         self.add_esc(u"\x01", "prev-chan")  # ^A
         self.add_esc(u"\x18", "next-chan")  # ^X
         self.add_esc(u"\x05", "alt-tab")  # ^E
 
         Util.Daemon(self.handshake_timeout, "hs_to")
 
         if IRONPY:
@@ -614,31 +618,40 @@
 
         self.reassign_retkey(crlf)
         t = "client crlf:  {0}  {1}  {2}"
         print(t.format(self.user.nick, self.adr[0], Util.b2hex(nl)))
         return len(nonl)
 
     def set_term_size(self, w, h):
-        self.w = w
-        self.h = h
+        wh = (w, h)
+        nick = self.user.nick
+
         if self.ar.dbg:
-            print("terminal sz:  {0}x{1}".format(self.w, self.h))
+            print("terminal sz:  %dx%d  @%s" % (w, h, nick))
 
-        if self.w >= 512:
-            print("screen width {0} reduced to 80".format(self.w))
-            self.w = 80
-        if self.h >= 512:
-            print("screen height {0} reduced to 24".format(self.h))
-            self.h = 24
-
-        self.user.nick_len = len(self.user.nick)
-        if self.user.nick_len > self.w * 0.25:
-            self.user.nick_len = int(self.w * 0.25)
+        if w >= 512 or not w:  # always 0 on win3.11
+            w = 80
+        if h >= 512 or not h:  # never seen 0 but hey
+            h = 24
 
+        self.w = w
+        self.h = h
         self.handshake_sz = True
+        self.user.nick_len = min(len(nick), int(w * 0.25))
+
+        if wh != (w, h) and not self.bad_naws:
+            self.bad_naws = True
+            t = u"%dx%d; will assume %dx%d" % (wh[0], wh[1], w, h)
+            print(u"   bad naws:  %s  @%s" % (t, self.user.nick))
+
+            t = u"your client reported windowsize " + t
+            if self.user.chans:
+                self.world.send_chan_msg(u"-nfo-", self.user.chans[0].nchan, t, False)
+            else:
+                self.info_q.append(t)
 
     def handshake_timeout(self):
         if self.ar.dbg:
             print("handshake_sz  init")
 
         time.sleep(1)
 
@@ -2605,14 +2618,18 @@
             self.wizard_stage = None
             self.in_text = u""
             self.in_text_full = u""
             self.user.create_channels()
             if not self.slowmo_tx:
                 self.world.cserial += 1
 
+            while self.info_q:
+                t = self.info_q.pop(0)
+                self.world.send_chan_msg(u"-nfo-", self.user.chans[0].nchan, t, False)
+
     def check_correct_iface(self, next_stage):
         self.wizard_stage = next_stage
 
         if self.iface_confirmed or not self.host.other_if:
             return True
 
         self.iface_confirmed = True
@@ -2830,14 +2847,22 @@
                                 + self.linebuf[self.linepos :]
                             )
                             self.linepos -= 1
                     elif act == "ret":
                         self.last_beep = time.time() - 0.9
                         if self.echo_on:
                             self.need_full_redraw = True
+                        if not self.user.active_chan:
+                            t = "XXX sendmsg without %s <%s> %r" % (
+                                "active chan??" if self.handshake_sz else "termsz",
+                                self.user.nick,
+                                self.linebuf,
+                            )
+                            print(t)
+                            self.linebuf = u""
                         if self.linebuf:
                             # add this to the message/command ("input") history
                             if not self.msg_hist or self.msg_hist[-1] != self.linebuf:
                                 self.msg_hist.append(self.linebuf)
 
                             self.msg_not_from_hist = False
                             self.pending_size_request = 0.0
@@ -2865,29 +2890,18 @@
                                         % (ircb.irc_cname, self.user.nick, t)
                                     )
 
                             self.msg_hist_n = None
                             self.linebuf = u""
                             self.linepos = 0
 
-                    elif act == "pgup" or act == "pgdn":
-
-                        steps = self.h - 4
-                        if self.scroll_i is not None:
-                            steps = self.scroll_i
-                        elif self.scroll_f is not None:
-                            steps = int(steps * self.scroll_f)
-                        else:
-                            print("no scroll size?!")
-
-                        if act == "pgup":
-                            steps *= -1
-
-                        self.scroll_cmd += steps
-
+                    elif act == "pgup":
+                        self.user.exec_cmd("u")
+                    elif act == "pgdn":
+                        self.user.exec_cmd("d")
                     elif act == "redraw":
                         self.user.exec_cmd("r")
                     elif act == "view":
                         self.user.exec_cmd("v")
                     elif act == "prev-chan":
                         chan_shift = -1
                     elif act == "next-chan":
```

### Comparing `r0c-1.6.0/r0c/user.py` & `r0c-1.6.1/r0c/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
 Keybinds:
   \033[36mUp\033[0m / \033[36mDown\033[0m       input history
   \033[36mLeft\033[0m / \033[36mRight\033[0m    input field traversing
   \033[36mHome\033[0m / \033[36mEnd\033[0m      input field jump
   \033[36mPgUp\033[0m / \033[36mPgDown\033[0m   chatlog scrolling... \033[1mtry it :-)\033[0m
 
-if you are using a mac, PgUp is fn-Shift-PgUp
-if your terminal is tiny, try \033[36m/mn\033[0m and \033[36m/cy\033[0m
+* if your terminal is tiny, try commands \033[36m/mn\033[0m and \033[36m/cy\033[0m
+* Cannot scroll? try these:  \033[36mCTRL-U\033[0m  \033[36mCTRL-D\033[0m  \033[36m/u\033[0m  \033[36m/d\033[0m
 """
 
 
 class User(object):
     def __init__(self, world, address):
         # type: (World.World, tuple[str, int]) -> User
         self.ar = world.ar
@@ -145,15 +145,15 @@
   `1;36m/^^  | |  /^^      `0mgithub.com/9001/r0c
   `1;34m|    \\_/  \\__      `0;36m------b. r0c_build `0m
 """
 
             # the messy version
             text = u"""
 `1;30m______    `37m_`30m    ______
-`1;30m\\\\\\\\\\\\\\  `37m/ \\  `30m///////   `0mret`1mr0c`22mhat r0c_ver `36m-----
+`1;30m\\\\\\\\\\\\\\  `37m/ \\  `30m///////   `0mret`1mr0c`22mhat r0c_ver `36m---
  `1;30m\\\\ `36m/`37m^^  | |  `36m/^`0;36m^`1;30m //    `0mgithub.com/9001/r0c
   `1;30m\\ `0;36m|    `1m\\_/  `0;36m\\__ `1;30m/     `0;36m------b. r0c_build `0m
 """
 
         pad1 = pad2 = u"──"
         if len(S_VERSION) > 3:
             pad1 = pad1[1:]
@@ -459,19 +459,28 @@
 
             print("       /msg:  %s  %s" % (self.nick, arg1))
             uchan = self.world.join_priv_chan(self, arg1)
             self.new_active_chan = uchan
             self.world.send_chan_msg(self.nick, uchan.nchan, arg2)
             self.client.refresh(False, True)
 
-        elif cmd == u"up" or cmd == u"u":
-            self.client.scroll_cmd += -(self.client.h - 4)
+        elif cmd == u"up" or cmd == u"u" or cmd == u"down" or cmd == u"d":
+            cli = self.client
+            steps = cli.h - 4
+            if cli.scroll_i is not None:
+                steps = cli.scroll_i
+            elif cli.scroll_f is not None:
+                steps = int(steps * cli.scroll_f)
+            else:
+                print("no scroll size?!")
+
+            if cmd == u"up" or cmd == u"u":
+                steps *= -1
 
-        elif cmd == u"down" or cmd == u"d":
-            self.client.scroll_cmd += +(self.client.h - 4)
+            cli.scroll_cmd += steps
 
         elif cmd == u"latest" or cmd == u"l":
             self.active_chan.lock_to_bottom = True
             self.client.need_full_redraw = True
             self.client.refresh(False)
 
         elif cmd == u"view" or cmd == u"v":
```

### Comparing `r0c-1.6.0/r0c/util.py` & `r0c-1.6.1/r0c/util.py`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c/world.py` & `r0c-1.6.1/r0c/world.py`

 * *Files identical despite different names*

### Comparing `r0c-1.6.0/r0c.egg-info/PKG-INFO` & `r0c-1.6.1/r0c.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r0c
-Version: 1.6.0
+Version: 1.6.1
 Summary: retr0chat telnet/vt100 chat server
 Home-page: https://github.com/9001/r0c
 Author: ed
 Author-email: r0c@ocv.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -49,28 +49,29 @@
 imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
 
 retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
 
 * tries to be irssi
 * zero dependencies on python 2.6, 2.7, 3.x
 * supports telnet, netcat, /dev/tcp, TLS clients
-* is not an irc server, but can bridge to/from irc servers
+* is not an irc server, but can [bridge to/from irc servers](#irc)
 * [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
 * fallbacks for inhumane conditions
   * linemode
   * no vt100 / ansi escape codes
 
 ## endorsements
 
 * the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
 
 ## compatibility
 
 * 1980: [TVI 920C](https://a.ocv.me/pub/g/nerd-stuff/r0c-tvi-920c.jpg)
 * 1987: [IBM 3151](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.jpg) (also [video](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.webm)), using gnu-screen to translate VT100 sequences
+* 1993: [windows 3.11](https://a.ocv.me/pub/g/nerd-stuff/r0c-for-workgroups.png)
 
 ## features
 
 irc-like:
 * public channels with persistent history (pgup/pgdn)
 * private messages (`/msg acidburn hey`)
 * nick completion with `Tab ↹`
@@ -80,15 +81,15 @@
 
 technical:
 * client behavior detection (echo, colors, charset, newline)
 * message input with readline-like editing (arrow-left/right, home/end, backspace)
   * history of sent messages (arrow-up/down)
 * bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
 * fast enough; 600 clients @ 750 msgs/sec, or 1'000 cli @ 350 msg/s
-* bridge several irc channels from several networks into one r0c channel
+* [bridge](#irc) several irc channels from several networks into one r0c channel
 
 ## windows clients
 
 * use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
 * or [the powershell client](https://github.com/9001/r0c/blob/master/clients/powershell.ps1)
 * or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
 
@@ -140,14 +141,30 @@
 
 you can run it as a service so it autostarts on boot:
 
 * on most linux distros: [systemd service](https://github.com/9001/r0c/blob/master/docs/systemd/r0c.service) (automatically does port-forwarding)
 * on alpine / gentoo: [openrc service](https://github.com/9001/r0c/blob/master/docs/openrc/r0c)
 * on windows: [nssm](https://nssm.cc/) probably
 
+## irc
+
+if you want to connect your r0c instance to an irc network and bridge channels between them, you can do that:
+
+![screenshot of a r0c channel being bridged to an irc channel](https://github.com/9001/r0c/blob/master/docs/r0c-irc.png)
+
+```bash
+python3 r0c.py --ircn a,127.0.0.1,6667,r0c --ircb a,chat,g
+```
+
+run that command to start r0c with irc bridging enabled; r0c will then connect to an irc server (which we nicknamed `a`) on `127.0.0.1:6667` with the irc-nick `r0c` and bridge the irc-channel `#chat` with the r0c-channel `#g`
+
+if you then start an irc server locally, for example [miniircd](https://github.com/jrosdahl/miniircd/blob/master/miniircd) by running `python3 miniircd --verbose` then you're all set, people can now join r0c by connecting via irc
+
+to bridge additional channels on the same network, add more `--ircb` args, for example `--ircb a,tech,tech` like in the screenshot, and optionally add more networks with `--ircn`
+
 ## firewall rules
 
 skip this section if:
 * you are using the systemd service
 * or you are running as root and do not have a firewall
 * or you're on windows
```

### Comparing `r0c-1.6.0/setup.py` & `r0c-1.6.1/setup.py`

 * *Files identical despite different names*

