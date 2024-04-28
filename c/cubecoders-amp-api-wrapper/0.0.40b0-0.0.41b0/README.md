# Comparing `tmp/cubecoders_amp_api_wrapper-0.0.40b0.tar.gz` & `tmp/cubecoders_amp_api_wrapper-0.0.41b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubecoders_amp_api_wrapper-0.0.40b0.tar", last modified: Wed Apr  3 23:12:58 2024, max compression
+gzip compressed data, was "cubecoders_amp_api_wrapper-0.0.41b0.tar", last modified: Sun Apr 28 19:16:11 2024, max compression
```

## Comparing `cubecoders_amp_api_wrapper-0.0.40b0.tar` & `cubecoders_amp_api_wrapper-0.0.41b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-03 23:12:58.195540 cubecoders_amp_api_wrapper-0.0.40b0/
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     7535 2024-04-03 23:12:56.000000 cubecoders_amp_api_wrapper-0.0.40b0/CHANGELOG.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    35823 2024-02-19 17:57:42.000000 cubecoders_amp_api_wrapper-0.0.40b0/LICENSE
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       79 2024-03-28 19:08:10.000000 cubecoders_amp_api_wrapper-0.0.40b0/MANIFEST.in
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     5436 2024-04-03 23:12:58.193957 cubecoders_amp_api_wrapper-0.0.40b0/PKG-INFO
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     3570 2024-04-03 23:06:15.000000 cubecoders_amp_api_wrapper-0.0.40b0/README.md
-drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-03 23:12:58.067871 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     1628 2024-04-03 23:12:06.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/__init__.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2473 2024-04-03 23:06:44.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/ads.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    78168 2024-04-03 23:06:45.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/adsmodule.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    15528 2024-04-03 23:06:46.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/base.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     1660 2024-04-03 23:06:47.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/bridge.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    77162 2024-04-03 23:06:49.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/core.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)      272 2024-04-03 23:06:51.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/emailsender.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     8197 2024-04-03 23:06:52.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/filebackup.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    23110 2024-04-03 23:06:53.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/filemanager.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2918 2024-04-03 23:06:54.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/instance.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    20234 2024-04-03 23:06:54.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/minecraft.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    36107 2024-04-03 23:06:56.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/types.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     3678 2024-04-03 23:06:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/util.py
-drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-03 23:12:58.118435 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     5436 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)      696 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        1 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       59 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/requires.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        7 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
-drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-03 23:12:58.182922 cubecoders_amp_api_wrapper-0.0.40b0/docs/
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    44207 2024-02-29 23:02:05.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/ADS_api_spec.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    29522 2024-02-28 00:01:43.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/Minecraft_api_spec.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    10703 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/permission_nodes.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    10703 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/permission_nodes.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     4816 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/setting_nodes.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     4774 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/setting_nodes.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       59 2024-03-28 18:44:49.000000 cubecoders_amp_api_wrapper-0.0.40b0/requirements.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       38 2024-04-03 23:12:58.196279 cubecoders_amp_api_wrapper-0.0.40b0/setup.cfg
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2195 2024-04-03 23:07:00.000000 cubecoders_amp_api_wrapper-0.0.40b0/setup.py
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-28 19:16:10.190452 cubecoders_amp_api_wrapper-0.0.41b0/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     7842 2024-04-28 19:16:08.000000 cubecoders_amp_api_wrapper-0.0.41b0/CHANGELOG.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35149 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/LICENSE
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       76 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/MANIFEST.in
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4772 2024-04-28 19:16:10.185501 cubecoders_amp_api_wrapper-0.0.41b0/PKG-INFO
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3475 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/README.md
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-28 19:16:09.758454 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1575 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/__init__.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2408 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/ads.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    76652 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/adsmodule.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    14988 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/base.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1614 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/bridge.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    75470 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/core.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      258 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/emailsender.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8024 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/filebackup.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    22707 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/filemanager.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2836 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/instance.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    19719 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/minecraft.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    34975 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/types.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3570 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/util.py
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-28 19:16:10.151452 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4772 2024-04-28 19:16:08.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      696 2024-04-28 19:16:09.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        1 2024-04-28 19:16:08.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-04-28 19:16:08.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/requires.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        7 2024-04-28 19:16:09.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-28 19:16:10.123452 cubecoders_amp_api_wrapper-0.0.41b0/docs/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    44032 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/ADS_api_spec.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    29384 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/Minecraft_api_spec.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/permission_nodes.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/permission_nodes.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4691 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/setting_nodes.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4649 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/setting_nodes.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-04-12 19:04:59.000000 cubecoders_amp_api_wrapper-0.0.41b0/requirements.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       38 2024-04-28 19:16:10.216585 cubecoders_amp_api_wrapper-0.0.41b0/setup.cfg
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2134 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/setup.py
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/CHANGELOG.md` & `cubecoders_amp_api_wrapper-0.0.41b0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## Version - 0.0.41b - [5b0aed8](https://github.com/k8thekat/AMPAPI_Python/commit/5b0aed8)
+#### __init__.py
+- Version bump `0.0.41b
+
+#### types.py
+- Added `LastExecuteError` and `LastErrorReason` to `Triggers()` dataclass.
+
+#### base.py
+- Removed un-used code.
+
+#### Changelog.md
+- Version log - `0.0.40b`
+
 ## Version - 0.0.40b - [b055fb3](https://github.com/k8thekat/AMPAPI_Python/commit/b055fb3)
 #### Readme.md
 - Changed TestPypi to Pypi
 	- Updated bash commands for installing package.
 
 #### init.py
 - Version bump `0.0.40b`
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/LICENSE` & `cubecoders_amp_api_wrapper-0.0.41b0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/PKG-INFO` & `cubecoders_amp_api_wrapper-0.0.41b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,17 @@
 Metadata-Version: 2.1
 Name: cubecoders_amp_api_wrapper
-Version: 0.0.40b0
+Version: 0.0.41b0
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
-Description: # AMPAPI_Python_wrapper
-        ___
-        CubeCoders AMP API wrapper in Python. 
-        
-        ### Key Features
-        ___
-        
-        - Pythonic API wrapper using `async` and `await`.
-        - Data is in dataclasses for easier management and interaction.
-            - Optional parameter per function or global to disable formatting of data.
-        - Parent classes `ADSInstance` and `AMPInstance` to group endpoints together and make handling of multiple Instances easier.
-            - This will also limit Instance specific API endpoints (eg. Minecraft) to that Instance type only.
-        
-        ### Installing
-        ___
-        
-        *Python 3.9 or higher is required*
-        
-        To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
-        
-        ### Pypi 
-        -> https://pypi.org/project/cubecoders-amp-api-wrapper/
-        ```bash
-        # Linux/macOS
-        pip install cubecoders-amp-api-wrapper
-        
-        # Windows
-        pip install cubecoders-amp-api-wrapper
-        ```
-        
-        
-        ### Quick Example -
-        
-        ```py
-        # You can pull these values from an `.ini` or a `.env` file,
-        # then populate the NamedTuple APIparams from `types -> APIParams`
-        _params = APIParams(url="http://192.168.13.130:8080",
-                            user="amp_username",
-                            password="amp_password")
-        
-        async def Sample_API():
-            """
-            Example API Function to call method Endpoints.
-            """
-            _bridge = Bridge(api_params=_params)
-            ADS: ADSInstance = ADSInstance()
-            # This would populate the ADS class property .AvailableInstances
-            ADS.get_instances()
-            # We can break out all our instances into their own attributes.
-            arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
-            mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
-        
-            # Pre populated from the dataclass and has the API methods too!
-            # You can take a backup really easily.
-            await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
-        
-            # Then you can call instance type specific API methods.
-            await mcinstance.mc_add_to_whitelist(user_or_uuid="k8_thekat")
-        
-            # You can also check attributes and other fields of the instance.
-            mcinstance.InstanceName
-            mcinstance.InstanceID
-        
-            # The State of the Instance. eg. Running, Offline, Restarting. See `types.py -> State_enum
-            # This is NOT updated constantly. See about using `get_status()` to keep it current.
-            if mcinstance.AppState == State_enum.Stopped:
-                await mcinstance.start_instance()
-        
-            # You can also check Metrics of an Instance easily.
-            mcinstance.Status.Metrics
-        
-            # Want to kick a random person? Here ya go~
-            players: list[Players] = await mcinstance.get_user_list()
-            await mcinstance.mc_kick_user_by_id(id=players[0].id)
-        ```
-        
-        
-        ### Controlling data formatting -
-        - All JSON data returned from the API endpoints is formatted into a Dataclass/Enum/etc if possible.
-        - Data formatting can be controlled globally or locally by changing the `format_data` parameter of the method to `False`.
-            - When turning off the data formatting, typically you will get a `dictionary` back.
-        
-        ### Example -
-        ```py
-        # By default all API calls will be formatted into Dataclasses if possible.
-        # You can toggle format_data off with ANY of the API classes that inherit Base().
-        ADS.format_data = False
-        
-        # You can turn data formatting back on globally through any Instance object.
-        arkinstance.format_data = True
-        
-        # You can turn off or on data formatting per function also.
-        await arkinstance.get_updates(format_data=False)
-        await arkinstance.get_role_data(format_data=True)
-        
-        ```
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -117,7 +20,108 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.7.4.post0
+Requires-Dist: dataclass_wizard==0.22.2
+Requires-Dist: pyotp==2.6.0
+
+# AMPAPI_Python_wrapper
+___
+CubeCoders AMP API wrapper in Python. 
+
+### Key Features
+___
+
+- Pythonic API wrapper using `async` and `await`.
+- Data is in dataclasses for easier management and interaction.
+    - Optional parameter per function or global to disable formatting of data.
+- Parent classes `ADSInstance` and `AMPInstance` to group endpoints together and make handling of multiple Instances easier.
+    - This will also limit Instance specific API endpoints (eg. Minecraft) to that Instance type only.
+
+### Installing
+___
+
+*Python 3.9 or higher is required*
+
+To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
+
+### Pypi 
+-> https://pypi.org/project/cubecoders-amp-api-wrapper/
+```bash
+# Linux/macOS
+pip install cubecoders-amp-api-wrapper
+
+# Windows
+pip install cubecoders-amp-api-wrapper
+```
+
+
+### Quick Example -
+
+```py
+# You can pull these values from an `.ini` or a `.env` file,
+# then populate the NamedTuple APIparams from `types -> APIParams`
+_params = APIParams(url="http://192.168.13.130:8080",
+                    user="amp_username",
+                    password="amp_password")
+
+async def Sample_API():
+    """
+    Example API Function to call method Endpoints.
+    """
+    _bridge = Bridge(api_params=_params)
+    ADS: ADSInstance = ADSInstance()
+    # This would populate the ADS class property .AvailableInstances
+    ADS.get_instances()
+    # We can break out all our instances into their own attributes.
+    arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
+    mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
+
+    # Pre populated from the dataclass and has the API methods too!
+    # You can take a backup really easily.
+    await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
+
+    # Then you can call instance type specific API methods.
+    await mcinstance.mc_add_to_whitelist(user_or_uuid="k8_thekat")
+
+    # You can also check attributes and other fields of the instance.
+    mcinstance.InstanceName
+    mcinstance.InstanceID
+
+    # The State of the Instance. eg. Running, Offline, Restarting. See `types.py -> State_enum
+    # This is NOT updated constantly. See about using `get_status()` to keep it current.
+    if mcinstance.AppState == State_enum.Stopped:
+        await mcinstance.start_instance()
+
+    # You can also check Metrics of an Instance easily.
+    mcinstance.Status.Metrics
+
+    # Want to kick a random person? Here ya go~
+    players: list[Players] = await mcinstance.get_user_list()
+    await mcinstance.mc_kick_user_by_id(id=players[0].id)
+```
+
+
+### Controlling data formatting -
+- All JSON data returned from the API endpoints is formatted into a Dataclass/Enum/etc if possible.
+- Data formatting can be controlled globally or locally by changing the `format_data` parameter of the method to `False`.
+    - When turning off the data formatting, typically you will get a `dictionary` back.
+
+### Example -
+```py
+# By default all API calls will be formatted into Dataclasses if possible.
+# You can toggle format_data off with ANY of the API classes that inherit Base().
+ADS.format_data = False
+
+# You can turn data formatting back on globally through any Instance object.
+arkinstance.format_data = True
+
+# You can turn off or on data formatting per function also.
+await arkinstance.get_updates(format_data=False)
+await arkinstance.get_role_data(format_data=True)
+
+```
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/README.md` & `cubecoders_amp_api_wrapper-0.0.41b0/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-# AMPAPI_Python_wrapper
-___
-CubeCoders AMP API wrapper in Python. 
-
-### Key Features
-___
-
-- Pythonic API wrapper using `async` and `await`.
-- Data is in dataclasses for easier management and interaction.
-    - Optional parameter per function or global to disable formatting of data.
-- Parent classes `ADSInstance` and `AMPInstance` to group endpoints together and make handling of multiple Instances easier.
-    - This will also limit Instance specific API endpoints (eg. Minecraft) to that Instance type only.
-
-### Installing
-___
-
-*Python 3.9 or higher is required*
-
-To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
-
-### Pypi 
--> https://pypi.org/project/cubecoders-amp-api-wrapper/
-```bash
-# Linux/macOS
-pip install cubecoders-amp-api-wrapper
-
-# Windows
-pip install cubecoders-amp-api-wrapper
-```
-
-
-### Quick Example -
-
-```py
-# You can pull these values from an `.ini` or a `.env` file,
-# then populate the NamedTuple APIparams from `types -> APIParams`
-_params = APIParams(url="http://192.168.13.130:8080",
-                    user="amp_username",
-                    password="amp_password")
-
-async def Sample_API():
-    """
-    Example API Function to call method Endpoints.
-    """
-    _bridge = Bridge(api_params=_params)
-    ADS: ADSInstance = ADSInstance()
-    # This would populate the ADS class property .AvailableInstances
-    ADS.get_instances()
-    # We can break out all our instances into their own attributes.
-    arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
-    mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
-
-    # Pre populated from the dataclass and has the API methods too!
-    # You can take a backup really easily.
-    await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
-
-    # Then you can call instance type specific API methods.
-    await mcinstance.mc_add_to_whitelist(user_or_uuid="k8_thekat")
-
-    # You can also check attributes and other fields of the instance.
-    mcinstance.InstanceName
-    mcinstance.InstanceID
-
-    # The State of the Instance. eg. Running, Offline, Restarting. See `types.py -> State_enum
-    # This is NOT updated constantly. See about using `get_status()` to keep it current.
-    if mcinstance.AppState == State_enum.Stopped:
-        await mcinstance.start_instance()
-
-    # You can also check Metrics of an Instance easily.
-    mcinstance.Status.Metrics
-
-    # Want to kick a random person? Here ya go~
-    players: list[Players] = await mcinstance.get_user_list()
-    await mcinstance.mc_kick_user_by_id(id=players[0].id)
-```
-
-
-### Controlling data formatting -
-- All JSON data returned from the API endpoints is formatted into a Dataclass/Enum/etc if possible.
-- Data formatting can be controlled globally or locally by changing the `format_data` parameter of the method to `False`.
-    - When turning off the data formatting, typically you will get a `dictionary` back.
-
-### Example -
-```py
-# By default all API calls will be formatted into Dataclasses if possible.
-# You can toggle format_data off with ANY of the API classes that inherit Base().
-ADS.format_data = False
-
-# You can turn data formatting back on globally through any Instance object.
-arkinstance.format_data = True
-
-# You can turn off or on data formatting per function also.
-await arkinstance.get_updates(format_data=False)
-await arkinstance.get_role_data(format_data=True)
-
+# AMPAPI_Python_wrapper
+___
+CubeCoders AMP API wrapper in Python. 
+
+### Key Features
+___
+
+- Pythonic API wrapper using `async` and `await`.
+- Data is in dataclasses for easier management and interaction.
+    - Optional parameter per function or global to disable formatting of data.
+- Parent classes `ADSInstance` and `AMPInstance` to group endpoints together and make handling of multiple Instances easier.
+    - This will also limit Instance specific API endpoints (eg. Minecraft) to that Instance type only.
+
+### Installing
+___
+
+*Python 3.9 or higher is required*
+
+To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
+
+### Pypi 
+-> https://pypi.org/project/cubecoders-amp-api-wrapper/
+```bash
+# Linux/macOS
+pip install cubecoders-amp-api-wrapper
+
+# Windows
+pip install cubecoders-amp-api-wrapper
+```
+
+
+### Quick Example -
+
+```py
+# You can pull these values from an `.ini` or a `.env` file,
+# then populate the NamedTuple APIparams from `types -> APIParams`
+_params = APIParams(url="http://192.168.13.130:8080",
+                    user="amp_username",
+                    password="amp_password")
+
+async def Sample_API():
+    """
+    Example API Function to call method Endpoints.
+    """
+    _bridge = Bridge(api_params=_params)
+    ADS: ADSInstance = ADSInstance()
+    # This would populate the ADS class property .AvailableInstances
+    ADS.get_instances()
+    # We can break out all our instances into their own attributes.
+    arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
+    mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
+
+    # Pre populated from the dataclass and has the API methods too!
+    # You can take a backup really easily.
+    await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
+
+    # Then you can call instance type specific API methods.
+    await mcinstance.mc_add_to_whitelist(user_or_uuid="k8_thekat")
+
+    # You can also check attributes and other fields of the instance.
+    mcinstance.InstanceName
+    mcinstance.InstanceID
+
+    # The State of the Instance. eg. Running, Offline, Restarting. See `types.py -> State_enum
+    # This is NOT updated constantly. See about using `get_status()` to keep it current.
+    if mcinstance.AppState == State_enum.Stopped:
+        await mcinstance.start_instance()
+
+    # You can also check Metrics of an Instance easily.
+    mcinstance.Status.Metrics
+
+    # Want to kick a random person? Here ya go~
+    players: list[Players] = await mcinstance.get_user_list()
+    await mcinstance.mc_kick_user_by_id(id=players[0].id)
+```
+
+
+### Controlling data formatting -
+- All JSON data returned from the API endpoints is formatted into a Dataclass/Enum/etc if possible.
+- Data formatting can be controlled globally or locally by changing the `format_data` parameter of the method to `False`.
+    - When turning off the data formatting, typically you will get a `dictionary` back.
+
+### Example -
+```py
+# By default all API calls will be formatted into Dataclasses if possible.
+# You can toggle format_data off with ANY of the API classes that inherit Base().
+ADS.format_data = False
+
+# You can turn data formatting back on globally through any Instance object.
+arkinstance.format_data = True
+
+# You can turn off or on data formatting per function also.
+await arkinstance.get_updates(format_data=False)
+await arkinstance.get_role_data(format_data=True)
+
 ```
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/__init__.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-'''
-   Copyright (C) 2021-2022 Katelynn Cadwallader.
-
-   This file is part of Gatekeeper, the AMP API.
-
-   Gatekeeper is free software; you can redistribute it and/or modify
-   it under the terms of the GNU General Public License as published by
-   the Free Software Foundation; either version 3, or (at your option)
-   any later version.
-
-   Gatekeeper is distributed in the hope that it will be useful, but WITHOUT
-   ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
-   or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public
-   License for more details.
-
-   You should have received a copy of the GNU General Public License
-   along with Gatekeeper; see the file COPYING.  If not, write to the Free
-   Software Foundation, 51 Franklin Street - Fifth Floor, Boston, MA
-   02110-1301, USA. 
-'''
-from __future__ import annotations
-
-__title__ = "CubeCoders AMP API"
-__author__ = "k8thekat"
-__license__ = "GNU"
-__version__ = "0.0.40b"
-__credits__ = "AMP by CubeCoders and associates."
-
-from typing import Literal, NamedTuple
-
-from .ads import *
-from .adsmodule import *
-from .bridge import *
-from .core import *
-from .emailsender import *
-from .filebackup import *
-from .filemanager import *
-from .instance import *
-from .minecraft import *
-from .types import *
-from .util import *
-
-
-class VersionInfo(NamedTuple):
-    Major: int
-    Minor: int
-    Revision: int
-    releaseLevel: Literal["alpha", "beta", "release"]
-
-
-version_info: VersionInfo = VersionInfo(Major=0, Minor=0, Revision=33, releaseLevel="alpha")
-
-del NamedTuple, Literal, VersionInfo
+'''
+   Copyright (C) 2021-2022 Katelynn Cadwallader.
+
+   This file is part of Gatekeeper, the AMP API.
+
+   Gatekeeper is free software; you can redistribute it and/or modify
+   it under the terms of the GNU General Public License as published by
+   the Free Software Foundation; either version 3, or (at your option)
+   any later version.
+
+   Gatekeeper is distributed in the hope that it will be useful, but WITHOUT
+   ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+   or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public
+   License for more details.
+
+   You should have received a copy of the GNU General Public License
+   along with Gatekeeper; see the file COPYING.  If not, write to the Free
+   Software Foundation, 51 Franklin Street - Fifth Floor, Boston, MA
+   02110-1301, USA. 
+'''
+from __future__ import annotations
+
+__title__ = "CubeCoders AMP API"
+__author__ = "k8thekat"
+__license__ = "GNU"
+__version__ = "0.0.41b"
+__credits__ = "AMP by CubeCoders and associates."
+
+from typing import Literal, NamedTuple
+
+from .ads import *
+from .adsmodule import *
+from .bridge import *
+from .core import *
+from .emailsender import *
+from .filebackup import *
+from .filemanager import *
+from .instance import *
+from .minecraft import *
+from .types import *
+from .util import *
+
+
+class VersionInfo(NamedTuple):
+    Major: int
+    Minor: int
+    Revision: int
+    releaseLevel: Literal["alpha", "beta", "release"]
+
+
+version_info: VersionInfo = VersionInfo(Major=0, Minor=0, Revision=33, releaseLevel="alpha")
+
+del NamedTuple, Literal, VersionInfo
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/ads.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/ads.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from typing import TYPE_CHECKING, Self, Union
-
-from .adsmodule import ADSModule
-from .core import Core
-from .emailsender import EmailSenderPlugin
-from .filebackup import LocalFileBackupPlugin
-from .filemanager import FileManagerPlugin
-from .instance import AMPInstance, AMPMinecraftInstance
-from .types import Controller, Instance
-
-__all__ = ("ADSInstance",)
-
-
-class ADSInstance(ADSModule, Core, EmailSenderPlugin, LocalFileBackupPlugin, FileManagerPlugin, Controller):
-    """
-    The ADS class is the top most level of Instances inside of AMP, may also be referred to as the "Controller".
-
-    """
-
-    Module: str = "ADS"
-
-    @property
-    def AvailableInstances(self) -> list[AMPInstance | AMPMinecraftInstance]:
-        return self._AvailableInstances
-
-    @AvailableInstances.setter
-    def AvailableInstances(self, instances: list[Instance]) -> None:
-        self._AvailableInstances: list[AMPInstance] = []
-        if isinstance(instances, list) and len(instances) > 0:
-            for i in range(0, len(instances)):
-                if instances[i].Module == "ADS":
-                    continue
-
-                elif instances[i].Module == "Minecraft":
-                    self._AvailableInstances.append(AMPMinecraftInstance(data=instances[i]))
-
-                else:
-                    self._AvailableInstances.append(AMPInstance(data=instances[i]))
-
-    def __init__(self):
-        # print(f"DEBUG {type(self).__name__} __init__")
-        super().__init__()
-
-    async def get_instances(self, format_data: Union[bool, None] = None) -> list[Controller | Self]:
-        """
-        Returns a list of all Instances on the AMP Panel and updates our self object.
-        `**ADSInstance Only**`
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[Self] | str | bool | int | None: On success returns a list of Self dataclasses. 
-
-        """
-
-        ads_list = []
-        result: list[Controller] = await super().get_instances(format_data=format_data)
-        if isinstance(result, list):
-            self.parse_data(data=result[0])  # Need to update our self object.
-            for i in range(1, len(result)):
-                ads_list.append(ADSInstance().parse_data(data=result[i]))
-            return ads_list
-        else:
-            return result
+from typing import TYPE_CHECKING, Self, Union
+
+from .adsmodule import ADSModule
+from .core import Core
+from .emailsender import EmailSenderPlugin
+from .filebackup import LocalFileBackupPlugin
+from .filemanager import FileManagerPlugin
+from .instance import AMPInstance, AMPMinecraftInstance
+from .types import Controller, Instance
+
+__all__ = ("ADSInstance",)
+
+
+class ADSInstance(ADSModule, Core, EmailSenderPlugin, LocalFileBackupPlugin, FileManagerPlugin, Controller):
+    """
+    The ADS class is the top most level of Instances inside of AMP, may also be referred to as the "Controller".
+
+    """
+
+    Module: str = "ADS"
+
+    @property
+    def AvailableInstances(self) -> list[AMPInstance | AMPMinecraftInstance]:
+        return self._AvailableInstances
+
+    @AvailableInstances.setter
+    def AvailableInstances(self, instances: list[Instance]) -> None:
+        self._AvailableInstances: list[AMPInstance] = []
+        if isinstance(instances, list) and len(instances) > 0:
+            for i in range(0, len(instances)):
+                if instances[i].Module == "ADS":
+                    continue
+
+                elif instances[i].Module == "Minecraft":
+                    self._AvailableInstances.append(AMPMinecraftInstance(data=instances[i]))
+
+                else:
+                    self._AvailableInstances.append(AMPInstance(data=instances[i]))
+
+    def __init__(self):
+        # print(f"DEBUG {type(self).__name__} __init__")
+        super().__init__()
+
+    async def get_instances(self, format_data: Union[bool, None] = None) -> list[Controller | Self]:
+        """
+        Returns a list of all Instances on the AMP Panel and updates our self object.
+        `**ADSInstance Only**`
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[Self] | str | bool | int | None: On success returns a list of Self dataclasses. 
+
+        """
+
+        ads_list = []
+        result: list[Controller] = await super().get_instances(format_data=format_data)
+        if isinstance(result, list):
+            self.parse_data(data=result[0])  # Need to update our self object.
+            for i in range(1, len(result)):
+                ads_list.append(ADSInstance().parse_data(data=result[i]))
+            return ads_list
+        else:
+            return result
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/adsmodule.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/adsmodule.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,1516 +1,1516 @@
-from __future__ import annotations
-
-from dataclasses import fields
-from typing import Union
-
-from .base import Base
-from .types import *
-
-__all__ = ("ADSModule",)
-
-
-class ADSModule(Base):
-    """
-    Contains the base functions for any `/API/ADSModule/` AMP API endpoints.
-
-    """
-    # ADSModule.AddDatastore:({'Parameters': [{'Name': 'newDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def add_datastore(self, new_datastore: InstanceDatastore, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Add a new datastore.
-        **Requires ADS**
-
-        Args:
-            new_datastore (InstanceDatastore): InstanceDatastore dataclass. See `types.py -> InstanceDatastore`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None) 
-
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-
-        if isinstance(new_datastore, InstanceDatastore):
-            data = self.dataclass_to_dict(dataclass=new_datastore)
-        else:
-            raise TypeError("new_datastore must be of type InstanceDatastore")
-
-        parameters = {
-            "newDatastore": data
-        }
-        result = await self._call_api(api="ADSModule/AddDatastore", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.DeleteDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_datastore(self, datastore_id: int, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Delete a datastore.
-        **Requires ADS**
-
-        Args:
-            datastore_id (int): The datastore ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass. 
-                See `types.py -> ActionResult`
-
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        parameters = {
-            "id": datastore_id
-        }
-        result = await self._call_api(api="ADSModule/DeleteDatastore", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.UpdateDatastore:({'Parameters': [{'Name': 'updatedDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def update_datastore(self, updated_datastore: InstanceDatastore, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Update an existing datastore.
-        **Requires ADS**
-
-        Args:
-            updated_datastore (InstanceDatastore): The updated datastore. See `types.py -> InstanceDatastore`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-
-        if isinstance(updated_datastore, InstanceDatastore):
-            data = self.dataclass_to_dict(dataclass=updated_datastore)
-
-        parameters = {
-            "updatedDatastore": data
-        }
-        result = await self._call_api(api="ADSModule/UpdateDatastore", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.GetDatastores:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_datastores(self, format_data: Union[bool, None] = None) -> list[InstanceDatastore]:
-        """
-        Get a list of Datastores.
-        **Requires ADS**
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-           list[DatastoreInstance]: On success returns a list of DatastoreInstance dataclasses.
-                See `types.py -> DatastoreInstance`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api="ADSModule/GetDatastores", format_data=format_data, format=InstanceDatastore)
-        return result
-
-    # ADSModule.RequestDatastoreSizeCalculation:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def request_datastore_size_calculation(self, datastore_id: int, format_data: Union[bool, None] = None) -> RunningTask:
-        """
-        Request a calculation of the size of the specified datastore.
-        **Requires ADS**
-
-        Args:
-            datastore_id (int): The datastore ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RunningTask: On success returns a RunningTask dataclass.
-                See `types.py -> RunningTask`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "datastoreId": datastore_id
-        }
-
-        await self._connect()
-        result = await self._call_api(api="ADSModule/RequestDatastoreSizeCalculation", parameters=parameters, format_data=format_data, format=RunningTask)
-        return result
-
-    # ADSModule.GetDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_datastore(self, datastore_id: int, format_data: Union[bool, None] = None) -> InstanceDatastore:
-        """
-        Get the information for the specified datastore.
-        **Requires ADS**
-
-        Args:
-            datastore_id (int): The datastore ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            InstanceDataStore: On success returns an InstanceDataStore dataclass.
-                See `types.py -> InstanceDataStore`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "id": datastore_id
-        }
-
-        await self._connect()
-        result = await self._call_api(api="ADSModule/GetDatastore", parameters=parameters, format_data=format_data, format=InstanceDatastore)
-        return result
-
-    # ADSModule.RepairDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def repair_datastore(self, datastore_id: int, format_data: Union[bool, None] = None) -> RunningTask:
-        """
-        Repair the specified datastore.
-        **Requires ADS**
-
-        Args:
-            datastore_id (int): The datastore ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RunningTask: On success returns a RunningTask dataclass.
-                See `types.py -> RunningTask`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "id": datastore_id
-        }
-        await self._connect()
-        result = await self._call_api(api="ADSModule/RepairDatastore", parameters=parameters, format_data=format_data, format=RunningTask)
-        return result
-
-    # ADSModule.GetDatastoreInstances:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_datastore_instances(self, datastore_id: int, format_data: Union[bool, None] = None) -> list[Instance]:
-        """
-        Get a list of Instances tied to the specified datastore.
-        **Requires ADS**
-
-        Args:
-            datastore_id (int): The datastore ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-
-        Returns:
-            list[Instance]: On success returns a list of Instance dataclasses.
-                See `types.py -> Instance`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "datastoreId": datastore_id
-        }
-        await self._connect()
-        result = await self._call_api(api="ADSModule/GetDatastoreInstances", parameters=parameters, format_data=format_data, format=Instance)
-        return result
-
-    # ADSModule.MoveInstanceDatastore:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def move_instance_datastore(self, instance_id: str, datastore_id: int, format_data: Union[bool, None] = None) -> RunningTask:
-        """
-        Move an Instance to a different datastore.
-        **Requires ADS**
-
-        Args:
-            instance_id (str): The Instance ID to move.
-            datastore_id (int): The datastore ID to move the Instance to.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RunningTask: On success returns a RunningTask dataclass.
-                See `types.py -> RunningTask`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        parameters = {
-            "instanceId": instance_id,
-            "datastoreId": datastore_id
-        }
-        result = await self._call_api(api="ADSModule/MoveInstanceDatastore", parameters=parameters, format_data=format_data, format=RunningTask)
-        return result
-
-    # ADSModule.GetInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_instance(self, instance_id: str, format_data: Union[bool, None] = None) -> Instance:
-        """
-        Returns the Instance information for the provided Instance ID.\n
-        **Requires ADS**
-
-        Args:
-            instance_id (str): The Instance ID to get information for.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Instance | str | bool | int | None: On success returns a Instance dataclass. 
-                See `types.py -> Instance`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        parameters = {
-            "InstanceId": instance_id
-        }
-        result = await self._call_api(api="ADSModule/GetInstance", parameters=parameters, format_data=format_data, format=Instance)
-        return result
-
-    # ADSModule.GetInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_instances(self, format_data: Union[bool, None] = None) -> list[Controller]:
-        """
-        Returns a list of all Instances on the AMP Panel.\n
-        **Requires ADS**
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[Controller] | str | bool | int | None: On success returns a list of Controller dataclasses. 
-                See `types.py -> Controller`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api="ADSModule/GetInstances", format_data=format_data, format=Controller)
-        return result
-
-    # ADSModule.GetInstanceStatuses:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_instance_statuses(self, format_data: Union[bool, None] = None) -> list[InstanceStatus]:
-        """
-        Returns a dictionary of the Server/Instance Status. \n
-        **Requires ADS**
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-
-        Returns:
-            list[InstanceStatus]: On success returns a list of InstanceStatus dataclasses.
-                See `types.py -> InstanceStatus`
-
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetInstanceStatuses', format_data=format_data, format=InstanceStatus)
-        return result
-
-    # ADSModule.GetDeploymentTemplates:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_deployment_templates(self, format_data: Union[bool, None] = None) -> list[DeploymentTemplate]:
-        """
-        Gets a list of Deployment Templates.
-        **Requires ADS**
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[DeploymentTemplate]: On success returns a list of DeploymentTemplate dataclasses.
-                See `types.py -> DeploymentTemplate`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetDeploymentTemplates', format_data=format_data, format=DeploymentTemplate)
-        return result
-
-    # ADSModule.CreateDeploymentTemplate:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def create_deployment_template(self, template_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Create a new Deployment Template. Typically used in conjunction with `update_deployment_template()`.
-        **Requires ADS**
-
-        Args:
-            template_name (str): Template name.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        parameters = {
-            "Name": template_name
-        }
-        result = await self._call_api(api='ADSModule/CreateDeploymentTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.UpdateDeploymentTemplate:({'Parameters': [{'Name': 'templateToUpdate', 'TypeName': 'DeploymentTemplate', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def update_deployment_template(self, template_to_update: DeploymentTemplate, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Update an existing Deployment Template.
-        **Requires ADS**
-
-        Args:
-            template_name (str): Template name.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        if isinstance(template_to_update, DeploymentTemplate):
-            data = self.dataclass_to_dict(dataclass=template_to_update)
-        else:
-            raise TypeError("template_to_update must be of type DeploymentTemplate")
-
-        parameters = {
-            "templateToUpdate": data
-        }
-        result = await self._call_api(api='ADSModule/UpdateDeploymentTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.DeleteDeploymentTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_deployment_template(self, template_id: int, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Delete an existing Deployment Template.
-        **Requires ADS**
-
-        Args:
-            template_id (int): Template ID
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        parameters = {
-            "Id": template_id
-        }
-        result = await self._call_api(api='ADSModule/DeleteDeploymentTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.CloneTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def clone_template(self, template_id: int, new_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Clone an existing Template.
-        **Requires ADS**
-
-        Args:
-            template_id (int): Template ID.
-            new_name (str): New Template name.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        parameters = {
-            "Id": template_id,
-            "NewName": new_name
-        }
-        result = await self._call_api(api='ADSModule/CloneTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.ApplyTemplate:({'Description': "Overlays an existing template on an existing instance. Used to perform package reconfigurations. Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.", 'Returns': '', 'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewFriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'RestartIfPreviouslyRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def apply_template(self, instance_id: str, template_id: int, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Overlays an existing template on an existing instance. 
-        Used to perform package reconfigurations. 
-        **Requires ADS**
-
-        `**Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.**`
-
-        Args:
-            instance_id (str): The Instance ID to apply the template to.
-            template_id (int): The Template ID to apply.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        parameters = {
-            "InstanceID": instance_id,
-            "TemplateID": template_id
-        }
-        result = await self._call_api(api='ADSModule/ApplyTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.DeployTemplate:({'Parameters': [{'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': 'The ID of the template to be deployed, as per the Template Management UI in AMP itself.', 'Optional': False}, {'Name': 'NewUsername', 'TypeName': 'String', 'Description': 'If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user.', 'Optional': True}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user.", 'Optional': True}, {'Name': 'NewEmail', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user.", 'Optional': True}, {'Name': 'RequiredTags', 'TypeName': 'List<String>', 'Description': "If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings.", 'Optional': True}, {'Name': 'Tag', 'TypeName': 'String', 'Description': "Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique.", 'Optional': True}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': 'A friendly name for this instance. If left blank, AMP will generate one for you.', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': 'Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'ExtraProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': 'A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.', 'Optional': True}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def deploy_template(self, template: Template, format_data: Union[bool, None] = None) -> ActionResult:
-        # async def deploy_template(self, template: Template | None = None, template_id: int | None = None, new_username: str | None = None, new_password: str | None = None, new_email: str | None = None,
-        #                           required_tags: list[str] | None = None, tag: str | None = None, friendly_name: str | None = None, secret: str | None = None, post_create: PostCreateActions = PostCreateActions.DoNothing,
-        #                           extra_provision_settings: dict[str, str] | None = None) -> ActionResult:
-        # Args:
-        # template_id (int): The ID of the template to be deployed, as per the Template Management UI in AMP itself.
-        # new_username (str | None, optional): If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user. `Defaults to None.`
-        # new_password (str | None, optional): If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user. `Defaults to None.`
-        # new_email (str | None, optional): If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user. `Defaults to None.`
-        # required_tags (list[str] | None, optional): If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings. `Defaults to None.`
-        # tag (str | None, optional): Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique. `Defaults to None.`
-        # friendly_name (str | None, optional): A friendly name for this instance. If left blank, AMP will generate one for you. `Defaults to None.`
-        # secret (str | None, optional): Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request. `Defaults to None.`
-        # post_create: 0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup, 16: Every time. `Default to 0.`
-        # extra_provision_settings (dict[str, str] | None, optional): A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself. `Defaults to None.`
-
-        """
-        Deploy a Instance template.
-        **Requires ADS**
-
-        Args:
-            template (Template | None, optional): The Template to deploy. See `types.py -> Template`.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`.
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = self.dataclass_to_dict(dataclass=template)
-
-        # for field in fields(Template):
-        #     value = getattr(template, field.name)
-        #     if value == None:
-        #         continue
-        #     parameters[field.name] = value
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/DeployTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.GetTargetInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_target_info(self, format_data: Union[bool, None] = None) -> RemoteTargetInfo:
-        """
-        Get target info.
-        **Requires ADS**
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RemoteTargetInfo: On success returns a RemoteTargetInfo dataclass.
-                See `types.py -> RemoteTargetInfo`.
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetTargetInfo', format_data=format_data, format=RemoteTargetInfo)
-        return result
-
-    # ADSModule.GetSupportedApplications:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_supported_applications(self, format_data: Union[bool, None] = None) -> list[Application]:
-        """
-        Get supported applications.
-        **Requires ADS**
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[dict[str, Any]] | str | dict[str, Any] | bool | int | None: Returns a list of all applications that can be deployed.
-
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetSupportedApplications', format_data=format_data, format=Application)
-        return result
-
-    # ADSModule.RefreshAppCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def refresh_app_cache(self) -> None:
-        """
-        Refresh the application cache.
-
-        Returns:
-            None
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        await self._call_api(api='ADSModule/RefreshAppCache')
-        return
-
-    # ADSModule.RefreshRemoteConfigStores:({'Parameters': [{'Name': 'force', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def refresh_remote_config_stores(self, force: bool = False) -> None:
-        """
-        Refresh remote config stores.
-
-        Args:
-            force (bool, optional): Force refresh. Defaults to False.
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "force": force
-        }
-
-        await self._connect()
-        await self._call_api(api='ADSModule/RefreshRemoteConfigStores', parameters=parameters)
-        return
-
-    # ADSModule.GetApplicationEndpoints:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_application_endpoints(self, instance_id: str, format_data: Union[bool, None] = None) -> list[Endpoints]:
-        """
-        Get the application endpoints for the specified instance.
-
-        Args:
-            instance_id (str): Instance ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-
-        Returns:
-            list[Endpoints]: Returns a list of endpoints for the specified instance.
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "instanceId": instance_id
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetApplicationEndpoints', parameters=parameters, format_data=format_data, format=Endpoints)
-        return result
-
-    # ADSModule.ReactivateLocalInstances:({'Parameters': [], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def reactivate_local_instances(self, format_data: Union[bool, None] = None) -> RunningTask:
-        """
-        Reactivate local instances.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RunningTask: On success returns a RunningTask dataclass.
-                See `types.py -> RunningTask`.
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/ReactivateLocalInstances', format_data=format_data, format=RunningTask)
-        return result
-
-    # ADSModule.ModifyCustomFirewallRule:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Range', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Protocol', 'TypeName': 'PortProtocol', 'Description': '', 'Optional': False, 'ParamEnumValues': {'TCP': 0, 'UDP': 1, 'Both': 2}}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Open', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def modify_custom_firewall_rule(self, instance_id: str, port_number: int, range: int, protocol: int, description: str, open: bool = True, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Modify the Firewall Rule of the specified instance.
-
-        Args:
-            instance_id (str): The Instance ID.
-            port_number (int): Port number.
-            range (int): Port range.
-            protocol (int): UDP/TCP/Both.
-            description (str): Description for which the rule is applied.
-            open (bool): Open or close the port mapping. Defaults to True.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "instanceId": instance_id,
-            "portNumber": port_number,
-            "range": range,
-            "protocol": protocol,
-            "description": description,
-            "open": open
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/ModifyCustomFirewallRule', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.ManageInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True})
-    async def manage_instance(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Manage the specified instance.\n
-        *Note* May be used for AMP instance management via the web interface.
-
-        Args:
-            instance_id (str): The Instance ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass. 
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "instanceId": instance_id
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/ManageInstance', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.GetGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_group(self, group_id: str, format_data: Union[bool, None] = None) -> dict:
-        """
-        Get the specified group.
-        *Note* Unsure what this is used for or does. May return ADS information/Instances related to it.
-
-        Args:
-            group_id (str): Group ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            dict: On success returns an dictionary.
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "groupId": group_id
-        }
-        await self._connect()
-        result = await self._call_api('ADSModule/GetGroup', parameters, format_data=format_data)
-        return result
-
-    # ADSModule.RefreshGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def refresh_group(self, group_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Refresh the specified group.
-
-        Args:
-            group_id (str): Group ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "groupId": group_id
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/RefreshGroup', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.GetLocalInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_local_instances(self, format_data: Union[bool, None] = None) -> list[Instance]:
-        """
-        Gets the local instances related to the ADS/Controller. 
-
-        Returns:
-            list[Instance]: Returns a list of Instance dataclass objects.
-                See `types.py -> Instance`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetLocalInstances', format_data=format_data, format=Instance)
-        return result
-
-    # ADSModule.GetProvisionFitness:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_provision_fitness(self, format_data: Union[bool, None] = None) -> Provision:
-        """
-        Get the provision fitness of the ADS/Controller.
-
-        Returns:
-            Provision: On success returns a Provision dataclass object.
-                See `types.py -> Provision`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetProvisionFitness', format_data=format_data, format=Provision)
-        return result
-
-    # ADSModule.AttachADS:({'Parameters': [{'Name': 'Friendly', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IsHTTPS', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Host', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Port', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def attach_ads(self, friendly: str, is_https: bool, host: str, port: int, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Attach an Instance to the ADS.
-
-
-        Args:
-            friendly (str): Name of the ADS.
-            is_https (bool): To use HTTPS.
-            host (str): URL/URi.
-            port (int): Port.
-            instance_id (str): Instance ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "friendly": friendly,
-            "isHttps": is_https,
-            "host": host,
-            "port": port,
-            "instanceId": instance_id
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/AttachADS', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.DetatchTarget:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def detatch_target(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        De-tach an Instance from the ADS.
-
-        Args:
-            instance_id (str): Instance ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "id": instance_id
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/DetatchTarget', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.UpdateTargetInfo:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Url', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Tags', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def update_target_info(self, instance_id: str, friendly_name: str, url: str, description: str, tags: list[str], format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Update a target Instance information.
-
-        Args:
-            instance_id (str): Instance ID.
-            friendly_name (str): Instance Friendly Name.
-            url (str): Instance URL.
-            description (str): The description for the Instance.
-            tags (list[str]): Tags.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "id": instance_id,
-            "friendlyName": friendly_name,
-            "url": url,
-            "description": description,
-            "tags": tags
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/UpdateTargetInfo', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.ConvertToManaged:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def convert_to_managed(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Convert an instance to managed.
-
-        Args:
-            instance_name (str): Instance name.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "instanceName": instance_name
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/ConvertToManaged', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.GetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_instance_network_info(self, instance_name: str, format_data: Union[bool, None] = None) -> list[PortInfo]:
-        """
-        Get the Port/Network information of an Instance.
-
-        Args:
-            instance_name (str): The Instance Name (NOT Friendly Name).
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[PortInfo]: On success returns a list of PortInfo dataclasses.
-                See `types.py -> PortInfo`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "instanceName": instance_name
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetInstanceNetworkInfo', parameters=parameters, format_data=format_data, format=PortInfo)
-        return result
-
-    # ADSModule.SetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortMappings', 'TypeName': 'Dictionary<String, Int32>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def set_instance_network_info(self, instance_id: str, port_mappings: dict[str, int], format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Set the Port mappings for an Instance.
-
-        Args:
-            instance_id (str): The Instance ID.
-            port_mappings (dict[str, int]): Port ranges and protocols to map.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "instanceId": instance_id,
-            "portMappings": port_mappings
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/SetInstanceNetworkInfo', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.ApplyInstanceConfiguration:({'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Args', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'RebuildConfiguration', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def apply_instance_configuration(self, instance_id: str, args: dict[str, str], rebuild_configuration: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Apply an Instance configuration. 
-
-        Args:
-            instance_id (str): The Instance ID.
-            args (dict[str, str]): UNK.
-            rebuild_configuration (bool, optional): UNK. Defaults to False.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "instanceId": instance_id,
-            "args": args,
-            "rebuildConfiguration": rebuild_configuration
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/ApplyInstanceConfiguration', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.CreateLocalInstance:({'Parameters': [{'Name': 'Instance', 'TypeName': 'LocalAMPInstance', 'Description': '', 'Optional': False}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def create_local_instance(self, instance: CreateInstance, post_create: PostCreateActions = PostCreateActions.DoNothing, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Create a local AMP Instance.
-
-        Args:
-            instance (LocalAMPInstance): CreateInstance dataclass. See `types.py -> CreateInstance`
-            post_create (PostCreateActions, optional): The action to take after creating the local instance. Defaults to PostCreateActions.DoNothing.
-                See `types.py -> PostCreateActions`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        if isinstance(instance, CreateInstance):
-            data = self.dataclass_to_dict(dataclass=instance)
-        else:
-            raise TypeError("instance must be of type CreateInstance")
-
-        parameters = {
-            "instance": data,
-            "postCreate": post_create
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/CreateLocalInstance', parameters=parameters, format_data=format_data, format=ActionResult)
-
-        return result
-
-    # ADSModule.CreateInstance:({'Parameters': [{'Name': 'TargetADSInstance', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewInstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Module', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IPBinding', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'AdminUsername', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AdminPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'AutoConfigure', 'TypeName': 'Boolean', 'Description': 'When enabled, all settings other than the Module, Target and FriendlyName are ignored and replaced with automatically generated values.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}, {'Name': 'DisplayImageSource', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'TargetDatastore', 'TypeName': 'Int32', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def create_instance(self, instance: CreateInstance, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Create an AMP Instance.
-
-        Args:
-            instance (CreateInstance): A CreateInstance dataclass. See `types.py -> CreateInstance`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {}
-
-        for field in fields(CreateInstance):
-            value = getattr(instance, field.name)
-            if value == None:
-                continue
-            parameters[field.name] = value
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/CreateInstance', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.SetInstanceConfig:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def set_instance_config(self, instance_name: str, setting_node: str, value: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Set an Instance Configuration.
-
-        Args:
-            instance_name (str): The Instance Name
-            setting_node (str): A setting node. See "./docs/setting_nodes.md"
-            value (str): The value for the setting node.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceName": instance_name,
-            "SettingNode": setting_node,
-            "Value": value
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/SetInstanceConfig', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.RefreshInstanceConfig:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def refresh_instance_config(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Refresh an Instance Configuration.
-
-        Args:
-            instance_id (str): The Instance ID
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceId": instance_id
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/RefreshInstanceConfig', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.HandoutInstanceConfigs:({'Parameters': [{'Name': 'ForModule', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Values', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def handout_instance_configs(self, for_module: str, setting_node: str, values: list[str], format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Handout Instance Configuration.
-
-        Args:
-            for_module (str): The Module Name. eg. "Minecraft"
-            setting_node (str): A setting node. See "./docs/setting_nodes.md"
-            values (list[str]): The values for the setting node.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "ForModule": for_module,
-            "SettingNode": setting_node,
-            "Values": values
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/HandoutInstanceConfigs', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.GetProvisionArguments:({'Parameters': [{'Name': 'ModuleName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<ProvisionSettingInfo>', 'IsComplexType': True})
-    async def get_provision_arguments(self, module_name: str, format_data: Union[bool, None] = None) -> list[ProvisionSettingInfo]:
-        """
-        Get Provision Arguments.
-
-        Args:
-            module_name (str): The Module Name (eg. "Minecraft")
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[ProvisionSettingInfo]: On success returns a list of ProvisionSettingInfo dataclasses.
-                See `types.py -> ProvisionSettingInfo`
-
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "ModuleName": module_name
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/GetProvisionArguments', parameters=parameters, format_data=format_data, format=ProvisionSettingInfo)
-        return result
-
-    # ADSModule.RegisterTarget:({'Parameters': [{'Name': 'controllerUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'myUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'twoFactorToken', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'friendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def register_target(self, controller_url: str, my_url: str, username: str, password: str,
-                              friendly_name: str, two_factor_token: str = "", format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Registers a Target to a Controller.
-
-        Args:
-            controller_url (str): The Controller(Main) AMP panel url.
-            my_url (str): The Target AMP panel url.
-            username (str): The username for logging into the Target AMP panel.
-            password (str): The password for logging into the Target AMP panel.
-            friendly_name (str): Instance Friendly Name.
-            two_factor_token (str): The two-factor authentication token for the username. Defaults to ""
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "controllerUrl": controller_url,
-            "myUrl": my_url,
-            "username": username,
-            "password": password,
-            "twoFactorToken": two_factor_token,
-            "friendlyName": friendly_name
-        }
-        await self._connect()
-        result = await self._call_api(api='ADSModule/RegisterTarget', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.UpdateTarget:({'Parameters': [{'Name': 'TargetID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def update_target(self, target_id: str) -> None:
-        """
-        Update Target Instance.
-
-        Args:
-            target_id (str): The Target Instance ID.
-
-        Returns:
-            None
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "TargetID": target_id
-        }
-
-        await self._connect()
-        await self._call_api(api='ADSModule/UpdateTarget', parameters=parameters)
-        return
-
-    # ADSModule.UpdateInstanceInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ExcludeFromFirewall', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'RunInContainer', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ContainerMemory', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'MemoryPolicy', 'TypeName': 'ContainerMemoryPolicy', 'Description': '', 'Optional': False, 'ParamEnumValues': {'NotSpecified': 0, 'Reserve': 100, 'Restrict': 200}}, {'Name': 'ContainerMaxCPU', 'TypeName': 'Single', 'Description': '', 'Optional': False}, {'Name': 'ContainerImage', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def update_instance_info(self, instance_info: InstanceInfo, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Update an Instances info.
-
-        Args:
-            instance_info (InstanceInfo): The InstanceInfo dataclass.
-                See `types.py -> InstanceInfo`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {}
-
-        for field in fields(InstanceInfo):
-            value = getattr(instance_info, field.name)
-            if value == None:
-                continue
-            parameters[field.name] = value
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/UpdateInstanceInfo', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.SetInstanceSuspended:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def set_instance_suspended(self, instance_name: str, suspended: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Set an Instances suspended State.
-
-        Args:
-            instance_name (str): The Instance Name
-            suspended (bool): The Suspended value. Default False
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceName": instance_name,
-            "Suspended": suspended
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/SetInstanceSuspended', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.UpgradeInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def upgrade_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Upgrade an Instance.
-
-        Args:
-            instance_name (str): The Instance Name
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceName": instance_name
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/UpgradeInstance', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.StartAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def start_all_instances(self, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Start all Instances.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/StartAllInstances', format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.StopAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def stop_all_instances(self, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Stop all Instances.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/StopAllInstances', format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.UpgradeAllInstances:({'Parameters': [{'Name': 'RestartRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def upgrade_all_instances(self, restart_running: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Upgrade all Instances.
-
-        Args:
-            restart_running (bool): Restart running Instances. Default False
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "RestartRunning": restart_running
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/UpgradeAllInstances', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.StartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def start_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Start an Instance.
-
-        Args:
-            instance_name (str): The Instance Name
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceName": instance_name
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/StartInstance', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.RestartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def restart_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Restart an Instance.
-
-        Args:
-            instance_name (str): The Instance Name
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceName": instance_name
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/RestartInstance', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.StopInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def stop_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Stop an Instance.
-
-        Args:
-            instance_name (str): The Instance Name
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceName": instance_name
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/StopInstance', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_instance_users(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Delete all Users from an Instance.
-
-        Args:
-            instance_id (str): The Instance ID
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceId": instance_id
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/DeleteInstanceUsers', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.DeleteInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def delete_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> RunningTask:
-        """
-        Delete an Instance.
-
-        Args:
-            instance_name (str): The Instance name.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RunningTask: On success returns a RunningTask dataclass.
-                See `types.py -> RunningTask`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "InstanceName": instance_name
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/DeleteInstance', parameters=parameters, format_data=format_data, format=RunningTask)
-        return result
-
-    # ADSModule.ExtractEverywhere:({'Parameters': [{'Name': 'SourceArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def extract_everywhere(self, source_archive: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Extracts everything from an archive.
-
-        Args:
-            source_archive (str): The source archive.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "SourceArchive": source_archive
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/ExtractEverywhere', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # ADSModule.Servers:({'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'REQ_RAWJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
-    async def servers(self, id: str, req_rawjson: str = "application/json", format_data: Union[bool, None] = None) -> Any:
-        """
-        Used for proxy authentication.
-
-        Args:
-            id (str): _description_
-            req_rawjson (str): _description_
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Any: UNK.
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        parameters = {
-            "id": id,
-            "REQ_RAWJSON": req_rawjson
-        }
-
-        await self._connect()
-        result = await self._call_api(api='ADSModule/Servers', parameters=parameters, format_data=format_data)
-        return result
+from __future__ import annotations
+
+from dataclasses import fields
+from typing import Union
+
+from .base import Base
+from .types import *
+
+__all__ = ("ADSModule",)
+
+
+class ADSModule(Base):
+    """
+    Contains the base functions for any `/API/ADSModule/` AMP API endpoints.
+
+    """
+    # ADSModule.AddDatastore:({'Parameters': [{'Name': 'newDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def add_datastore(self, new_datastore: InstanceDatastore, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Add a new datastore.
+        **Requires ADS**
+
+        Args:
+            new_datastore (InstanceDatastore): InstanceDatastore dataclass. See `types.py -> InstanceDatastore`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None) 
+
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+
+        if isinstance(new_datastore, InstanceDatastore):
+            data = self.dataclass_to_dict(dataclass=new_datastore)
+        else:
+            raise TypeError("new_datastore must be of type InstanceDatastore")
+
+        parameters = {
+            "newDatastore": data
+        }
+        result = await self._call_api(api="ADSModule/AddDatastore", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.DeleteDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_datastore(self, datastore_id: int, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Delete a datastore.
+        **Requires ADS**
+
+        Args:
+            datastore_id (int): The datastore ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass. 
+                See `types.py -> ActionResult`
+
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        parameters = {
+            "id": datastore_id
+        }
+        result = await self._call_api(api="ADSModule/DeleteDatastore", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.UpdateDatastore:({'Parameters': [{'Name': 'updatedDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def update_datastore(self, updated_datastore: InstanceDatastore, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Update an existing datastore.
+        **Requires ADS**
+
+        Args:
+            updated_datastore (InstanceDatastore): The updated datastore. See `types.py -> InstanceDatastore`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+
+        if isinstance(updated_datastore, InstanceDatastore):
+            data = self.dataclass_to_dict(dataclass=updated_datastore)
+
+        parameters = {
+            "updatedDatastore": data
+        }
+        result = await self._call_api(api="ADSModule/UpdateDatastore", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.GetDatastores:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_datastores(self, format_data: Union[bool, None] = None) -> list[InstanceDatastore]:
+        """
+        Get a list of Datastores.
+        **Requires ADS**
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+           list[DatastoreInstance]: On success returns a list of DatastoreInstance dataclasses.
+                See `types.py -> DatastoreInstance`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api="ADSModule/GetDatastores", format_data=format_data, format=InstanceDatastore)
+        return result
+
+    # ADSModule.RequestDatastoreSizeCalculation:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def request_datastore_size_calculation(self, datastore_id: int, format_data: Union[bool, None] = None) -> RunningTask:
+        """
+        Request a calculation of the size of the specified datastore.
+        **Requires ADS**
+
+        Args:
+            datastore_id (int): The datastore ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RunningTask: On success returns a RunningTask dataclass.
+                See `types.py -> RunningTask`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "datastoreId": datastore_id
+        }
+
+        await self._connect()
+        result = await self._call_api(api="ADSModule/RequestDatastoreSizeCalculation", parameters=parameters, format_data=format_data, format=RunningTask)
+        return result
+
+    # ADSModule.GetDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_datastore(self, datastore_id: int, format_data: Union[bool, None] = None) -> InstanceDatastore:
+        """
+        Get the information for the specified datastore.
+        **Requires ADS**
+
+        Args:
+            datastore_id (int): The datastore ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            InstanceDataStore: On success returns an InstanceDataStore dataclass.
+                See `types.py -> InstanceDataStore`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "id": datastore_id
+        }
+
+        await self._connect()
+        result = await self._call_api(api="ADSModule/GetDatastore", parameters=parameters, format_data=format_data, format=InstanceDatastore)
+        return result
+
+    # ADSModule.RepairDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def repair_datastore(self, datastore_id: int, format_data: Union[bool, None] = None) -> RunningTask:
+        """
+        Repair the specified datastore.
+        **Requires ADS**
+
+        Args:
+            datastore_id (int): The datastore ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RunningTask: On success returns a RunningTask dataclass.
+                See `types.py -> RunningTask`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "id": datastore_id
+        }
+        await self._connect()
+        result = await self._call_api(api="ADSModule/RepairDatastore", parameters=parameters, format_data=format_data, format=RunningTask)
+        return result
+
+    # ADSModule.GetDatastoreInstances:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_datastore_instances(self, datastore_id: int, format_data: Union[bool, None] = None) -> list[Instance]:
+        """
+        Get a list of Instances tied to the specified datastore.
+        **Requires ADS**
+
+        Args:
+            datastore_id (int): The datastore ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+
+        Returns:
+            list[Instance]: On success returns a list of Instance dataclasses.
+                See `types.py -> Instance`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "datastoreId": datastore_id
+        }
+        await self._connect()
+        result = await self._call_api(api="ADSModule/GetDatastoreInstances", parameters=parameters, format_data=format_data, format=Instance)
+        return result
+
+    # ADSModule.MoveInstanceDatastore:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def move_instance_datastore(self, instance_id: str, datastore_id: int, format_data: Union[bool, None] = None) -> RunningTask:
+        """
+        Move an Instance to a different datastore.
+        **Requires ADS**
+
+        Args:
+            instance_id (str): The Instance ID to move.
+            datastore_id (int): The datastore ID to move the Instance to.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RunningTask: On success returns a RunningTask dataclass.
+                See `types.py -> RunningTask`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        parameters = {
+            "instanceId": instance_id,
+            "datastoreId": datastore_id
+        }
+        result = await self._call_api(api="ADSModule/MoveInstanceDatastore", parameters=parameters, format_data=format_data, format=RunningTask)
+        return result
+
+    # ADSModule.GetInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_instance(self, instance_id: str, format_data: Union[bool, None] = None) -> Instance:
+        """
+        Returns the Instance information for the provided Instance ID.\n
+        **Requires ADS**
+
+        Args:
+            instance_id (str): The Instance ID to get information for.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Instance | str | bool | int | None: On success returns a Instance dataclass. 
+                See `types.py -> Instance`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        parameters = {
+            "InstanceId": instance_id
+        }
+        result = await self._call_api(api="ADSModule/GetInstance", parameters=parameters, format_data=format_data, format=Instance)
+        return result
+
+    # ADSModule.GetInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_instances(self, format_data: Union[bool, None] = None) -> list[Controller]:
+        """
+        Returns a list of all Instances on the AMP Panel.\n
+        **Requires ADS**
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[Controller] | str | bool | int | None: On success returns a list of Controller dataclasses. 
+                See `types.py -> Controller`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api="ADSModule/GetInstances", format_data=format_data, format=Controller)
+        return result
+
+    # ADSModule.GetInstanceStatuses:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_instance_statuses(self, format_data: Union[bool, None] = None) -> list[InstanceStatus]:
+        """
+        Returns a dictionary of the Server/Instance Status. \n
+        **Requires ADS**
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+
+        Returns:
+            list[InstanceStatus]: On success returns a list of InstanceStatus dataclasses.
+                See `types.py -> InstanceStatus`
+
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetInstanceStatuses', format_data=format_data, format=InstanceStatus)
+        return result
+
+    # ADSModule.GetDeploymentTemplates:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_deployment_templates(self, format_data: Union[bool, None] = None) -> list[DeploymentTemplate]:
+        """
+        Gets a list of Deployment Templates.
+        **Requires ADS**
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[DeploymentTemplate]: On success returns a list of DeploymentTemplate dataclasses.
+                See `types.py -> DeploymentTemplate`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetDeploymentTemplates', format_data=format_data, format=DeploymentTemplate)
+        return result
+
+    # ADSModule.CreateDeploymentTemplate:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def create_deployment_template(self, template_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Create a new Deployment Template. Typically used in conjunction with `update_deployment_template()`.
+        **Requires ADS**
+
+        Args:
+            template_name (str): Template name.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        parameters = {
+            "Name": template_name
+        }
+        result = await self._call_api(api='ADSModule/CreateDeploymentTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.UpdateDeploymentTemplate:({'Parameters': [{'Name': 'templateToUpdate', 'TypeName': 'DeploymentTemplate', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def update_deployment_template(self, template_to_update: DeploymentTemplate, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Update an existing Deployment Template.
+        **Requires ADS**
+
+        Args:
+            template_name (str): Template name.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        if isinstance(template_to_update, DeploymentTemplate):
+            data = self.dataclass_to_dict(dataclass=template_to_update)
+        else:
+            raise TypeError("template_to_update must be of type DeploymentTemplate")
+
+        parameters = {
+            "templateToUpdate": data
+        }
+        result = await self._call_api(api='ADSModule/UpdateDeploymentTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.DeleteDeploymentTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_deployment_template(self, template_id: int, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Delete an existing Deployment Template.
+        **Requires ADS**
+
+        Args:
+            template_id (int): Template ID
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        parameters = {
+            "Id": template_id
+        }
+        result = await self._call_api(api='ADSModule/DeleteDeploymentTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.CloneTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def clone_template(self, template_id: int, new_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Clone an existing Template.
+        **Requires ADS**
+
+        Args:
+            template_id (int): Template ID.
+            new_name (str): New Template name.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        parameters = {
+            "Id": template_id,
+            "NewName": new_name
+        }
+        result = await self._call_api(api='ADSModule/CloneTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.ApplyTemplate:({'Description': "Overlays an existing template on an existing instance. Used to perform package reconfigurations. Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.", 'Returns': '', 'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewFriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'RestartIfPreviouslyRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def apply_template(self, instance_id: str, template_id: int, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Overlays an existing template on an existing instance. 
+        Used to perform package reconfigurations. 
+        **Requires ADS**
+
+        `**Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.**`
+
+        Args:
+            instance_id (str): The Instance ID to apply the template to.
+            template_id (int): The Template ID to apply.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        parameters = {
+            "InstanceID": instance_id,
+            "TemplateID": template_id
+        }
+        result = await self._call_api(api='ADSModule/ApplyTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.DeployTemplate:({'Parameters': [{'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': 'The ID of the template to be deployed, as per the Template Management UI in AMP itself.', 'Optional': False}, {'Name': 'NewUsername', 'TypeName': 'String', 'Description': 'If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user.', 'Optional': True}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user.", 'Optional': True}, {'Name': 'NewEmail', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user.", 'Optional': True}, {'Name': 'RequiredTags', 'TypeName': 'List<String>', 'Description': "If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings.", 'Optional': True}, {'Name': 'Tag', 'TypeName': 'String', 'Description': "Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique.", 'Optional': True}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': 'A friendly name for this instance. If left blank, AMP will generate one for you.', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': 'Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'ExtraProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': 'A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.', 'Optional': True}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def deploy_template(self, template: Template, format_data: Union[bool, None] = None) -> ActionResult:
+        # async def deploy_template(self, template: Template | None = None, template_id: int | None = None, new_username: str | None = None, new_password: str | None = None, new_email: str | None = None,
+        #                           required_tags: list[str] | None = None, tag: str | None = None, friendly_name: str | None = None, secret: str | None = None, post_create: PostCreateActions = PostCreateActions.DoNothing,
+        #                           extra_provision_settings: dict[str, str] | None = None) -> ActionResult:
+        # Args:
+        # template_id (int): The ID of the template to be deployed, as per the Template Management UI in AMP itself.
+        # new_username (str | None, optional): If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user. `Defaults to None.`
+        # new_password (str | None, optional): If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user. `Defaults to None.`
+        # new_email (str | None, optional): If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user. `Defaults to None.`
+        # required_tags (list[str] | None, optional): If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings. `Defaults to None.`
+        # tag (str | None, optional): Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique. `Defaults to None.`
+        # friendly_name (str | None, optional): A friendly name for this instance. If left blank, AMP will generate one for you. `Defaults to None.`
+        # secret (str | None, optional): Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request. `Defaults to None.`
+        # post_create: 0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup, 16: Every time. `Default to 0.`
+        # extra_provision_settings (dict[str, str] | None, optional): A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself. `Defaults to None.`
+
+        """
+        Deploy a Instance template.
+        **Requires ADS**
+
+        Args:
+            template (Template | None, optional): The Template to deploy. See `types.py -> Template`.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`.
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = self.dataclass_to_dict(dataclass=template)
+
+        # for field in fields(Template):
+        #     value = getattr(template, field.name)
+        #     if value == None:
+        #         continue
+        #     parameters[field.name] = value
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/DeployTemplate', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.GetTargetInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_target_info(self, format_data: Union[bool, None] = None) -> RemoteTargetInfo:
+        """
+        Get target info.
+        **Requires ADS**
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RemoteTargetInfo: On success returns a RemoteTargetInfo dataclass.
+                See `types.py -> RemoteTargetInfo`.
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetTargetInfo', format_data=format_data, format=RemoteTargetInfo)
+        return result
+
+    # ADSModule.GetSupportedApplications:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_supported_applications(self, format_data: Union[bool, None] = None) -> list[Application]:
+        """
+        Get supported applications.
+        **Requires ADS**
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[dict[str, Any]] | str | dict[str, Any] | bool | int | None: Returns a list of all applications that can be deployed.
+
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetSupportedApplications', format_data=format_data, format=Application)
+        return result
+
+    # ADSModule.RefreshAppCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def refresh_app_cache(self) -> None:
+        """
+        Refresh the application cache.
+
+        Returns:
+            None
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        await self._call_api(api='ADSModule/RefreshAppCache')
+        return
+
+    # ADSModule.RefreshRemoteConfigStores:({'Parameters': [{'Name': 'force', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def refresh_remote_config_stores(self, force: bool = False) -> None:
+        """
+        Refresh remote config stores.
+
+        Args:
+            force (bool, optional): Force refresh. Defaults to False.
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "force": force
+        }
+
+        await self._connect()
+        await self._call_api(api='ADSModule/RefreshRemoteConfigStores', parameters=parameters)
+        return
+
+    # ADSModule.GetApplicationEndpoints:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_application_endpoints(self, instance_id: str, format_data: Union[bool, None] = None) -> list[Endpoints]:
+        """
+        Get the application endpoints for the specified instance.
+
+        Args:
+            instance_id (str): Instance ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+
+        Returns:
+            list[Endpoints]: Returns a list of endpoints for the specified instance.
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "instanceId": instance_id
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetApplicationEndpoints', parameters=parameters, format_data=format_data, format=Endpoints)
+        return result
+
+    # ADSModule.ReactivateLocalInstances:({'Parameters': [], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def reactivate_local_instances(self, format_data: Union[bool, None] = None) -> RunningTask:
+        """
+        Reactivate local instances.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RunningTask: On success returns a RunningTask dataclass.
+                See `types.py -> RunningTask`.
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/ReactivateLocalInstances', format_data=format_data, format=RunningTask)
+        return result
+
+    # ADSModule.ModifyCustomFirewallRule:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Range', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Protocol', 'TypeName': 'PortProtocol', 'Description': '', 'Optional': False, 'ParamEnumValues': {'TCP': 0, 'UDP': 1, 'Both': 2}}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Open', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def modify_custom_firewall_rule(self, instance_id: str, port_number: int, range: int, protocol: int, description: str, open: bool = True, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Modify the Firewall Rule of the specified instance.
+
+        Args:
+            instance_id (str): The Instance ID.
+            port_number (int): Port number.
+            range (int): Port range.
+            protocol (int): UDP/TCP/Both.
+            description (str): Description for which the rule is applied.
+            open (bool): Open or close the port mapping. Defaults to True.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "instanceId": instance_id,
+            "portNumber": port_number,
+            "range": range,
+            "protocol": protocol,
+            "description": description,
+            "open": open
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/ModifyCustomFirewallRule', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.ManageInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True})
+    async def manage_instance(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Manage the specified instance.\n
+        *Note* May be used for AMP instance management via the web interface.
+
+        Args:
+            instance_id (str): The Instance ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass. 
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "instanceId": instance_id
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/ManageInstance', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.GetGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_group(self, group_id: str, format_data: Union[bool, None] = None) -> dict:
+        """
+        Get the specified group.
+        *Note* Unsure what this is used for or does. May return ADS information/Instances related to it.
+
+        Args:
+            group_id (str): Group ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            dict: On success returns an dictionary.
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "groupId": group_id
+        }
+        await self._connect()
+        result = await self._call_api('ADSModule/GetGroup', parameters, format_data=format_data)
+        return result
+
+    # ADSModule.RefreshGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def refresh_group(self, group_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Refresh the specified group.
+
+        Args:
+            group_id (str): Group ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "groupId": group_id
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/RefreshGroup', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.GetLocalInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_local_instances(self, format_data: Union[bool, None] = None) -> list[Instance]:
+        """
+        Gets the local instances related to the ADS/Controller. 
+
+        Returns:
+            list[Instance]: Returns a list of Instance dataclass objects.
+                See `types.py -> Instance`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetLocalInstances', format_data=format_data, format=Instance)
+        return result
+
+    # ADSModule.GetProvisionFitness:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_provision_fitness(self, format_data: Union[bool, None] = None) -> Provision:
+        """
+        Get the provision fitness of the ADS/Controller.
+
+        Returns:
+            Provision: On success returns a Provision dataclass object.
+                See `types.py -> Provision`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetProvisionFitness', format_data=format_data, format=Provision)
+        return result
+
+    # ADSModule.AttachADS:({'Parameters': [{'Name': 'Friendly', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IsHTTPS', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Host', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Port', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def attach_ads(self, friendly: str, is_https: bool, host: str, port: int, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Attach an Instance to the ADS.
+
+
+        Args:
+            friendly (str): Name of the ADS.
+            is_https (bool): To use HTTPS.
+            host (str): URL/URi.
+            port (int): Port.
+            instance_id (str): Instance ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "friendly": friendly,
+            "isHttps": is_https,
+            "host": host,
+            "port": port,
+            "instanceId": instance_id
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/AttachADS', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.DetatchTarget:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def detatch_target(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        De-tach an Instance from the ADS.
+
+        Args:
+            instance_id (str): Instance ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "id": instance_id
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/DetatchTarget', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.UpdateTargetInfo:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Url', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Tags', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def update_target_info(self, instance_id: str, friendly_name: str, url: str, description: str, tags: list[str], format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Update a target Instance information.
+
+        Args:
+            instance_id (str): Instance ID.
+            friendly_name (str): Instance Friendly Name.
+            url (str): Instance URL.
+            description (str): The description for the Instance.
+            tags (list[str]): Tags.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "id": instance_id,
+            "friendlyName": friendly_name,
+            "url": url,
+            "description": description,
+            "tags": tags
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/UpdateTargetInfo', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.ConvertToManaged:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def convert_to_managed(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Convert an instance to managed.
+
+        Args:
+            instance_name (str): Instance name.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "instanceName": instance_name
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/ConvertToManaged', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.GetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_instance_network_info(self, instance_name: str, format_data: Union[bool, None] = None) -> list[PortInfo]:
+        """
+        Get the Port/Network information of an Instance.
+
+        Args:
+            instance_name (str): The Instance Name (NOT Friendly Name).
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[PortInfo]: On success returns a list of PortInfo dataclasses.
+                See `types.py -> PortInfo`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "instanceName": instance_name
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetInstanceNetworkInfo', parameters=parameters, format_data=format_data, format=PortInfo)
+        return result
+
+    # ADSModule.SetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortMappings', 'TypeName': 'Dictionary<String, Int32>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def set_instance_network_info(self, instance_id: str, port_mappings: dict[str, int], format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Set the Port mappings for an Instance.
+
+        Args:
+            instance_id (str): The Instance ID.
+            port_mappings (dict[str, int]): Port ranges and protocols to map.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "instanceId": instance_id,
+            "portMappings": port_mappings
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/SetInstanceNetworkInfo', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.ApplyInstanceConfiguration:({'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Args', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'RebuildConfiguration', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def apply_instance_configuration(self, instance_id: str, args: dict[str, str], rebuild_configuration: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Apply an Instance configuration. 
+
+        Args:
+            instance_id (str): The Instance ID.
+            args (dict[str, str]): UNK.
+            rebuild_configuration (bool, optional): UNK. Defaults to False.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "instanceId": instance_id,
+            "args": args,
+            "rebuildConfiguration": rebuild_configuration
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/ApplyInstanceConfiguration', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.CreateLocalInstance:({'Parameters': [{'Name': 'Instance', 'TypeName': 'LocalAMPInstance', 'Description': '', 'Optional': False}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def create_local_instance(self, instance: CreateInstance, post_create: PostCreateActions = PostCreateActions.DoNothing, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Create a local AMP Instance.
+
+        Args:
+            instance (LocalAMPInstance): CreateInstance dataclass. See `types.py -> CreateInstance`
+            post_create (PostCreateActions, optional): The action to take after creating the local instance. Defaults to PostCreateActions.DoNothing.
+                See `types.py -> PostCreateActions`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        if isinstance(instance, CreateInstance):
+            data = self.dataclass_to_dict(dataclass=instance)
+        else:
+            raise TypeError("instance must be of type CreateInstance")
+
+        parameters = {
+            "instance": data,
+            "postCreate": post_create
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/CreateLocalInstance', parameters=parameters, format_data=format_data, format=ActionResult)
+
+        return result
+
+    # ADSModule.CreateInstance:({'Parameters': [{'Name': 'TargetADSInstance', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewInstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Module', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IPBinding', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'AdminUsername', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AdminPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'AutoConfigure', 'TypeName': 'Boolean', 'Description': 'When enabled, all settings other than the Module, Target and FriendlyName are ignored and replaced with automatically generated values.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}, {'Name': 'DisplayImageSource', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'TargetDatastore', 'TypeName': 'Int32', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def create_instance(self, instance: CreateInstance, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Create an AMP Instance.
+
+        Args:
+            instance (CreateInstance): A CreateInstance dataclass. See `types.py -> CreateInstance`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {}
+
+        for field in fields(CreateInstance):
+            value = getattr(instance, field.name)
+            if value == None:
+                continue
+            parameters[field.name] = value
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/CreateInstance', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.SetInstanceConfig:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def set_instance_config(self, instance_name: str, setting_node: str, value: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Set an Instance Configuration.
+
+        Args:
+            instance_name (str): The Instance Name
+            setting_node (str): A setting node. See "./docs/setting_nodes.md"
+            value (str): The value for the setting node.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceName": instance_name,
+            "SettingNode": setting_node,
+            "Value": value
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/SetInstanceConfig', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.RefreshInstanceConfig:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def refresh_instance_config(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Refresh an Instance Configuration.
+
+        Args:
+            instance_id (str): The Instance ID
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceId": instance_id
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/RefreshInstanceConfig', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.HandoutInstanceConfigs:({'Parameters': [{'Name': 'ForModule', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Values', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def handout_instance_configs(self, for_module: str, setting_node: str, values: list[str], format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Handout Instance Configuration.
+
+        Args:
+            for_module (str): The Module Name. eg. "Minecraft"
+            setting_node (str): A setting node. See "./docs/setting_nodes.md"
+            values (list[str]): The values for the setting node.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "ForModule": for_module,
+            "SettingNode": setting_node,
+            "Values": values
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/HandoutInstanceConfigs', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.GetProvisionArguments:({'Parameters': [{'Name': 'ModuleName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<ProvisionSettingInfo>', 'IsComplexType': True})
+    async def get_provision_arguments(self, module_name: str, format_data: Union[bool, None] = None) -> list[ProvisionSettingInfo]:
+        """
+        Get Provision Arguments.
+
+        Args:
+            module_name (str): The Module Name (eg. "Minecraft")
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[ProvisionSettingInfo]: On success returns a list of ProvisionSettingInfo dataclasses.
+                See `types.py -> ProvisionSettingInfo`
+
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "ModuleName": module_name
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/GetProvisionArguments', parameters=parameters, format_data=format_data, format=ProvisionSettingInfo)
+        return result
+
+    # ADSModule.RegisterTarget:({'Parameters': [{'Name': 'controllerUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'myUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'twoFactorToken', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'friendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def register_target(self, controller_url: str, my_url: str, username: str, password: str,
+                              friendly_name: str, two_factor_token: str = "", format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Registers a Target to a Controller.
+
+        Args:
+            controller_url (str): The Controller(Main) AMP panel url.
+            my_url (str): The Target AMP panel url.
+            username (str): The username for logging into the Target AMP panel.
+            password (str): The password for logging into the Target AMP panel.
+            friendly_name (str): Instance Friendly Name.
+            two_factor_token (str): The two-factor authentication token for the username. Defaults to ""
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "controllerUrl": controller_url,
+            "myUrl": my_url,
+            "username": username,
+            "password": password,
+            "twoFactorToken": two_factor_token,
+            "friendlyName": friendly_name
+        }
+        await self._connect()
+        result = await self._call_api(api='ADSModule/RegisterTarget', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.UpdateTarget:({'Parameters': [{'Name': 'TargetID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def update_target(self, target_id: str) -> None:
+        """
+        Update Target Instance.
+
+        Args:
+            target_id (str): The Target Instance ID.
+
+        Returns:
+            None
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "TargetID": target_id
+        }
+
+        await self._connect()
+        await self._call_api(api='ADSModule/UpdateTarget', parameters=parameters)
+        return
+
+    # ADSModule.UpdateInstanceInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ExcludeFromFirewall', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'RunInContainer', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ContainerMemory', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'MemoryPolicy', 'TypeName': 'ContainerMemoryPolicy', 'Description': '', 'Optional': False, 'ParamEnumValues': {'NotSpecified': 0, 'Reserve': 100, 'Restrict': 200}}, {'Name': 'ContainerMaxCPU', 'TypeName': 'Single', 'Description': '', 'Optional': False}, {'Name': 'ContainerImage', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def update_instance_info(self, instance_info: InstanceInfo, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Update an Instances info.
+
+        Args:
+            instance_info (InstanceInfo): The InstanceInfo dataclass.
+                See `types.py -> InstanceInfo`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {}
+
+        for field in fields(InstanceInfo):
+            value = getattr(instance_info, field.name)
+            if value == None:
+                continue
+            parameters[field.name] = value
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/UpdateInstanceInfo', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.SetInstanceSuspended:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def set_instance_suspended(self, instance_name: str, suspended: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Set an Instances suspended State.
+
+        Args:
+            instance_name (str): The Instance Name
+            suspended (bool): The Suspended value. Default False
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceName": instance_name,
+            "Suspended": suspended
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/SetInstanceSuspended', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.UpgradeInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def upgrade_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Upgrade an Instance.
+
+        Args:
+            instance_name (str): The Instance Name
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceName": instance_name
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/UpgradeInstance', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.StartAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def start_all_instances(self, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Start all Instances.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/StartAllInstances', format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.StopAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def stop_all_instances(self, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Stop all Instances.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/StopAllInstances', format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.UpgradeAllInstances:({'Parameters': [{'Name': 'RestartRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def upgrade_all_instances(self, restart_running: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Upgrade all Instances.
+
+        Args:
+            restart_running (bool): Restart running Instances. Default False
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "RestartRunning": restart_running
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/UpgradeAllInstances', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.StartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def start_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Start an Instance.
+
+        Args:
+            instance_name (str): The Instance Name
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceName": instance_name
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/StartInstance', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.RestartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def restart_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Restart an Instance.
+
+        Args:
+            instance_name (str): The Instance Name
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceName": instance_name
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/RestartInstance', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.StopInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def stop_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Stop an Instance.
+
+        Args:
+            instance_name (str): The Instance Name
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceName": instance_name
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/StopInstance', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_instance_users(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Delete all Users from an Instance.
+
+        Args:
+            instance_id (str): The Instance ID
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceId": instance_id
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/DeleteInstanceUsers', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.DeleteInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def delete_instance(self, instance_name: str, format_data: Union[bool, None] = None) -> RunningTask:
+        """
+        Delete an Instance.
+
+        Args:
+            instance_name (str): The Instance name.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RunningTask: On success returns a RunningTask dataclass.
+                See `types.py -> RunningTask`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "InstanceName": instance_name
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/DeleteInstance', parameters=parameters, format_data=format_data, format=RunningTask)
+        return result
+
+    # ADSModule.ExtractEverywhere:({'Parameters': [{'Name': 'SourceArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def extract_everywhere(self, source_archive: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Extracts everything from an archive.
+
+        Args:
+            source_archive (str): The source archive.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "SourceArchive": source_archive
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/ExtractEverywhere', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # ADSModule.Servers:({'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'REQ_RAWJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
+    async def servers(self, id: str, req_rawjson: str = "application/json", format_data: Union[bool, None] = None) -> Any:
+        """
+        Used for proxy authentication.
+
+        Args:
+            id (str): _description_
+            req_rawjson (str): _description_
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Any: UNK.
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        parameters = {
+            "id": id,
+            "REQ_RAWJSON": req_rawjson
+        }
+
+        await self._connect()
+        result = await self._call_api(api='ADSModule/Servers', parameters=parameters, format_data=format_data)
+        return result
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/base.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,364 +1,361 @@
-from __future__ import annotations
-
-import json
-import logging
-import traceback
-from dataclasses import fields
-from datetime import timedelta
-from typing import TYPE_CHECKING, Any, Union
-
-import aiohttp
-from aiohttp import ClientResponse
-from dataclass_wizard import fromdict
-from pyotp import TOTP
-
-from ampapi.types import APISession  # 2Factor Authentication Python Module
-
-from .bridge import Bridge
-from .types import *
-
-if TYPE_CHECKING:
-    from typing import Self
-
-__all__ = ("Base",)
-
-FORMAT_DATA: bool = True
-
-
-class Base():
-    """
-    Contains the base functions for all AMP API endpoints and handles the parsing of Bridge data.
-
-    """
-    _logger: logging.Logger = logging.getLogger()
-    InstanceID: str = "0"
-    Module: str = ""
-    # Seconds (Typically a session expires after 5 minutes of inactivity.)
-    session_ttl: int = 240
-    url: str = ""
-
-    # self.FAILED_LOGIN: str = ""
-    NO_DATA: str = "Failed to receive any data from post request."
-    ADS_ONLY: str = "This API call is only available on ADS instances."
-    UNAUTHORIZED_ACCESS: str = "The user does not have the required permissions to interact with this instance."
-    NO_BRIDGE: str = "Failed to setup connection. You need to initiate `<class Bridge>` first."
-    MINECRAFT_ONLY: str = "This API call is only available on Minecraft instances."
-    FAILED_API: str = "The API call returned a non-proper response."
-    # NO_VALID_SESSION: str = "Failed to find a valid session id, please login again."
-
-    def __init__(self) -> None:
-        bridge: Bridge = Bridge.get_bridge()
-        # Validate the bridge object is at the same memory address.
-        self._logger.debug(f"bridge object -> {bridge}")
-        # print("DEBUG", f"bridge object -> {bridge}")
-        if bridge == None:
-            raise ValueError(self.NO_BRIDGE)
-
-        if isinstance(bridge, Bridge):
-            self.parse_bridge(bridge=bridge)  # type:ignore
-
-    @property
-    def format_data(self) -> bool:
-        """
-        Controls whether the data returned from the API endpoint is formatted or not. \n
-        `True` = formatted \n
-        `False` = unformatted
-
-        Returns:
-            bool: `True` or `False`, defaults to `True`.
-        """
-        global FORMAT_DATA
-        return FORMAT_DATA
-
-    @format_data.setter
-    def format_data(self, value: bool):
-        global FORMAT_DATA
-        FORMAT_DATA = value
-
-    # def set_format_data(self, value: bool = True) -> bool:
-    #     """
-    #     Controls whether the data returned from the API endpoint is formatted or not. \n
-    #     `True` = formatted \n
-    #     `False` = unformatted
-
-    #     Returns:
-    #         bool: `True` or `False`, defaults to `True`.
-    #     """
-    #     FORMAT_DATA: bool = value
-    #     return FORMAT_DATA
-
-    def parse_bridge(self, bridge: Bridge):
-        """
-        Takes the Bridge class object and pulls the APIparams data from it and set's the class attributes for API usage.
-
-        Args:
-            bridge (Bridge): The Bridge class object to parse.
-
-        Raises:
-            ValueError: If 2FA Token is not provided and `_use_2fa == True`.
-            ValueError: If 2FA Token is not enclosed in single(',') or double(",") quotes.
-        """
-        # We use this later on in _connect to update `_session_id`;
-        # so all connections will use the same session id (if possible)
-        self._bridge: Bridge = bridge
-        self.url = bridge.url
-        if bridge.use_2fa == True:
-            if bridge.token == "":
-                raise ValueError("You must provide a 2FA Token if you are using 2FA.")
-            if bridge.token.startswith(("'", '"')) == False or bridge.token.endswith(("'", '"')) == False:
-                raise ValueError("2FA Token must be enclosed in quotes.")
-
-    def parse_data(self, data: Controller | Instance | AppStatus | Updates) -> Self:
-        """
-        Takes in a Controller or Instance dataclass and iterates through it's attributes and 
-        set's the values as attributes of the class that called this function.
-
-        Args:
-            data (Controller | Instance): The Controller or Instance dataclass.
-
-        Returns:
-            Self: Returns the class that called this function.
-        """
-        for field in fields(data):
-            # This is to deal with improperly cased InstanceId.
-            if field.name == "InstanceId":
-                setattr(self, "InstanceID", getattr(data, field.name))
-                continue
-            setattr(self, field.name, getattr(data, field.name))
-        return self
-
-    def camel_case_data(self, data: dict[str, str | bool | int | None]) -> dict[str, str | int | bool]:
-        """
-        Camel case the keys of a dictionary.
-
-        Args:
-            data (dict[str, str  |  bool  |  None]): The dictionary to camel case.
-
-        Returns:
-            dict[str, str | bool]: The camel cased dictionary.
-        """
-        new: dict[str, str | bool | int] = {}
-        for key, value in data.items():
-            if value is not None:
-                new[key.title()] = value
-        return new
-
-    def dataclass_to_dict(self, dataclass: Any) -> dict[Any, Any]:
-        """
-        Convert a dataclass to a dictionary.
-
-        Args:
-            dataclass (Any): The dataclass to convert.
-
-        Returns:
-            dict[Any, Any]: The converted dataclass as a dictionary.
-        """
-        parameters = {}
-        for field in fields(dataclass):
-            value = getattr(dataclass, field.name)
-            if value == None:
-                continue
-            parameters[field.name] = value
-        return parameters
-
-    def json_to_dataclass(self, json: Any, format: Any, _use_from_dict: bool, _auto_unpack: bool) -> Any | list[Any]:
-        """
-        Format the JSON response data to a dataclass.
-
-        Args:
-            json (Any): JSON data to format.
-            format (Any): Dataclass or similar to unpack the JSON data into.
-            _use_from_dict (bool): Use dataclass wizard `fromdict()` or not.
-            _auto_unpack (bool): Use **data or not to unpack the data.
-
-        Returns:
-            Any | list[Any]: A list of the format object or a single format object.
-
-        """
-        if isinstance(json, list):
-            if _use_from_dict is True:
-                return list(fromdict(format, data) for data in json)
-
-            elif _auto_unpack is True:
-                return list(format(**data)for data in json)
-
-            else:
-                return list(format(data)for data in json)
-        else:
-            if _use_from_dict is True:
-                return fromdict(format, json)
-
-            elif _auto_unpack is True:
-                return format(**json)
-
-            else:
-                return format(json)
-
-    async def _call_api(self, api: str, parameters: Union[None, dict[str, Any]] = None, format_data: Union[bool, None] = None, format: Any = None, _use_from_dict: bool = True, _auto_unpack: bool = True) -> Any:
-        # TODO - Possibly convert the ending args to *args or similar.
-        """
-        Uses aiohttp.ClientSession() post request to access the AMP API endpoints. \n
-        Will automatically populate the `SESSIONID` parameter if it is not provided.
-
-        Args:
-            api (str): The API endpoint to call. eg `Core/GetModuleInfo`
-            parameters (dict[str, str]): The parameters to pass to the API endpoint.
-            format_data (Union[bool, None]): Controls whether the data returned from the API endpoint is formatted or not. Defaults to `None`.
-            format (Any): The dataclass the Response json will return. Defaults to `None`.
-            _use_from_dict (bool): Controls whether the data will use `fromdict` of dataclass wizard to unpack the data. Typical usage case is nested Dataclasses. Defaults to `True`.
-            _auto_unpack (bool): Controls whether the data will be unpacked automatically. Defaults to `True`.
-
-        Raises:
-            ValueError: When the API call returns no data or raises any exception.
-            ConnectionError: When the API call returns a status code other than 200.
-            PermissionError: When the API call returns a `Unauthorized Access` error or permission related error.
-
-        Returns:
-            Any: Returns the JSON response, either formatted or unformatted depending on `format_data`.
-        """
-        global FORMAT_DATA
-        header: dict = {"Accept": "text/javascript"}
-        post_req: ClientResponse | None
-        self._logger.debug(f"_call_api -> {api} was called with {parameters}")
-
-        # This should save us some boiler plate code throughout our API calls.
-        if parameters == None:
-            parameters = {}
-
-        api_session: APISession = self._bridge._sessions.get(self.InstanceID, APISession(id="0", ttl=datetime.now()))
-        if isinstance(api_session, APISession):
-            parameters["SESSIONID"] = api_session.id
-
-        json_data = json.dumps(parameters)
-
-        _url: str = self.url + "/API/" + api
-        # print("DEBUG", self.InstanceID, api, _url)
-        async with aiohttp.ClientSession() as session:
-            try:
-                post_req = await session.post(_url, headers=header, data=json_data)
-            # TODO - Need to not catch all Excepts..
-            # So I can handle each exception properly.
-            except Exception as e:
-                self._logger.error(f"DEBUG _call_api exception type: {type(e)}")
-                raise ValueError(e)
-
-            if post_req.content_length == 0:
-                raise ValueError(self.NO_DATA)
-
-            if post_req.status != 200:
-                raise ConnectionError(self.NO_DATA)
-
-            post_req_json: Any = await post_req.json()
-
-        if post_req_json == None:
-            raise ConnectionError(self.NO_DATA)
-
-        # They removed "result" from all replies thus breaking most if not all future code.
-        # This was an old example from pre 2.3 AMP API that could have the following return:
-        # `{'resultReason': 'Internal Auth - No reason given', 'success': False, 'result': 0}`
-        # print("DEBUG", "API CALL---->", api, type(post_req_json), parameters)
-        # print("DEBUG", post_req_json)
-        if isinstance(post_req_json, dict):
-            if api == "Core/Login":
-                return LoginResults(**post_req_json)
-
-            elif "result" in post_req_json:
-                post_req_json = post_req_json["result"]
-
-            elif "Title" in post_req_json:
-                post_req_json = post_req_json["Title"]
-                if isinstance(post_req_json, str) and post_req_json == "Unauthorized Access":
-                    self._logger.error(f'{api} failed because of {post_req_json}')
-                    api_session = APISession(id="0", ttl=datetime.now())
-                    self._bridge._sessions.update({self.InstanceID: api_session})
-                    raise PermissionError(self.UNAUTHORIZED_ACCESS)
-
-            elif isinstance(post_req_json, bool) and post_req_json == False:
-                self._logger.error(f"{api} failed because of {post_req_json}")
-                raise ConnectionError(self.FAILED_API)
-
-            elif isinstance(post_req_json, dict) and "Status" in post_req_json and post_req_json["Status"] == False:
-                self._logger.error(f"{api} failed because of Status: {post_req_json}")
-                return ConnectionError(self.FAILED_API)
-
-        # print("DEBUG", "FORMAT->", format_data, format)
-        if format is None or format_data is False:
-            return post_req_json
-
-        elif format_data is True or format_data is None and FORMAT_DATA is True:
-            return self.json_to_dataclass(json=post_req_json, format=format, _use_from_dict=_use_from_dict, _auto_unpack=_auto_unpack)
-
-    async def _connect(self) -> LoginResults | None:
-        """
-        Handles your 2FA code and logging into AMP while also handling the session ID. \n
-
-        Raises:
-            ValueError: If session ID is not a string or 2FA code is not a formatted properly.
-            TypeError: If the session is not an APISession object.
-
-        Returns:
-            bool | None: Returns False if an exception is thrown or the login attempt fails to provide a sessionID value. \n
-            Otherwise returns true and sets the class's sessionID value.
-        """
-        code: Union[str, TOTP] = ""
-
-        # get our InstanceID and use it to key for session_id
-        session: APISession = self._bridge._sessions.get(self.InstanceID, APISession(id="0", ttl=datetime.now()))
-        if isinstance(session, APISession):
-            ttl: timedelta = datetime.now() - session.ttl
-            if ttl.seconds > 240:
-                sessionID = "0"
-            else:
-                sessionID: str = session.id
-        else:
-            raise TypeError(f"session must be of type APISession. Received {type(session)}")
-
-        if sessionID == "0":
-            if self._bridge.use_2fa == True:
-                try:
-                    # Handles time based 2Factory Auth Key/Code
-                    code = TOTP(self._bridge.token).now()
-
-                except AttributeError:
-                    raise ValueError("Please check your 2 Factor Code, should not contain spaces, escape characters and it must be enclosed in quotes!")
-            else:
-                try:
-
-                    parameters = {
-                        'username': self._bridge.user,
-                        'password': self._bridge.password,
-                        'token': code,
-                        'rememberMe': True}
-
-                    result = await self._call_api(api='Core/Login', parameters=parameters, format_data=True, format=LoginResults)
-                    if isinstance(result, LoginResults):
-                        # This is our new sessions table to correlate InstanceID to a sessionID.
-                        api_session = APISession(id=result.sessionID, ttl=datetime.now())
-                        self._bridge._sessions.update({self.InstanceID: api_session})
-                        return result
-
-                    else:
-                        self._logger.warning("Failed response from Core/Login in _connect()")
-                        return result
-
-                except Exception as e:
-                    self._logger.warning(f'Core/Login Exception: {traceback.format_exc()}')
-        else:
-            return
-
-    async def call_end_point(self, api: str, parameters: None | dict[str, Any] = None) -> Any:
-        """
-        Universal API method for calling any API endpoint. Some API endpoints require ADS and some may require an Instance ID. \n
-
-        The Data returned will be unmodified. No DATACLASS returns.
-
-        Args:
-            api (str): API endpoint to call. `eg "Core/GetModuleInfo"` (Assume this starts with www.yourAMPURL.com/API/)
-            parameters (None | dict[str, str]): Parameters to pass to the API endpoint. Session ID is already handled for you. Defaults to None
-
-        Returns:
-            Any: Returns the JSON response from the API call.
-        """
-
-        result = await self._call_api(api=api, parameters=parameters)
-        return result
+from __future__ import annotations
+
+import json
+import logging
+import traceback
+from dataclasses import fields
+from datetime import timedelta
+from typing import TYPE_CHECKING, Any, Union
+
+import aiohttp
+from aiohttp import ClientResponse
+from dataclass_wizard import fromdict
+from pyotp import TOTP
+
+from ampapi.types import APISession  # 2Factor Authentication Python Module
+
+from .bridge import Bridge
+from .types import *
+
+if TYPE_CHECKING:
+    from typing import Self
+
+__all__ = ("Base",)
+
+FORMAT_DATA: bool = True
+
+
+class Base():
+    """
+    Contains the base functions for all AMP API endpoints and handles the parsing of Bridge data.
+
+    """
+    _logger: logging.Logger = logging.getLogger()
+    InstanceID: str = "0"
+    Module: str = ""
+    # Seconds (Typically a session expires after 5 minutes of inactivity.)
+    session_ttl: int = 240
+    url: str = ""
+
+    NO_DATA: str = "Failed to receive any data from post request."
+    ADS_ONLY: str = "This API call is only available on ADS instances."
+    UNAUTHORIZED_ACCESS: str = "The user does not have the required permissions to interact with this instance."
+    NO_BRIDGE: str = "Failed to setup connection. You need to initiate `<class Bridge>` first."
+    MINECRAFT_ONLY: str = "This API call is only available on Minecraft instances."
+    FAILED_API: str = "The API call returned a non-proper response."
+
+    def __init__(self) -> None:
+        bridge: Bridge = Bridge.get_bridge()
+        # Validate the bridge object is at the same memory address.
+        self._logger.debug(f"bridge object -> {bridge}")
+        if bridge == None:
+            raise ValueError(self.NO_BRIDGE)
+
+        if isinstance(bridge, Bridge):
+            self.parse_bridge(bridge=bridge)  # type:ignore
+
+    @property
+    def format_data(self) -> bool:
+        """
+        Controls whether the data returned from the API endpoint is formatted or not. \n
+        `True` = formatted \n
+        `False` = unformatted
+
+        Returns:
+            bool: `True` or `False`, defaults to `True`.
+        """
+        global FORMAT_DATA
+        return FORMAT_DATA
+
+    @format_data.setter
+    def format_data(self, value: bool):
+        global FORMAT_DATA
+        FORMAT_DATA = value
+
+    # def set_format_data(self, value: bool = True) -> bool:
+    #     """
+    #     Controls whether the data returned from the API endpoint is formatted or not. \n
+    #     `True` = formatted \n
+    #     `False` = unformatted
+
+    #     Returns:
+    #         bool: `True` or `False`, defaults to `True`.
+    #     """
+    #     FORMAT_DATA: bool = value
+    #     return FORMAT_DATA
+
+    def parse_bridge(self, bridge: Bridge):
+        """
+        Takes the Bridge class object and pulls the APIparams data from it and set's the class attributes for API usage.
+
+        Args:
+            bridge (Bridge): The Bridge class object to parse.
+
+        Raises:
+            ValueError: If 2FA Token is not provided and `_use_2fa == True`.
+            ValueError: If 2FA Token is not enclosed in single(',') or double(",") quotes.
+        """
+        # We use this later on in _connect to update `_session_id`;
+        # so all connections will use the same session id (if possible)
+        self._bridge: Bridge = bridge
+        self.url = bridge.url
+        if bridge.use_2fa == True:
+            if bridge.token == "":
+                raise ValueError("You must provide a 2FA Token if you are using 2FA.")
+            if bridge.token.startswith(("'", '"')) == False or bridge.token.endswith(("'", '"')) == False:
+                raise ValueError("2FA Token must be enclosed in quotes.")
+
+    def parse_data(self, data: Controller | Instance | AppStatus | Updates) -> Self:
+        """
+        Takes in a Controller or Instance dataclass and iterates through it's attributes and 
+        set's the values as attributes of the class that called this function.
+
+        Args:
+            data (Controller | Instance): The Controller or Instance dataclass.
+
+        Returns:
+            Self: Returns the class that called this function.
+        """
+        for field in fields(data):
+            # This is to deal with improperly cased InstanceId.
+            if field.name == "InstanceId":
+                setattr(self, "InstanceID", getattr(data, field.name))
+                continue
+            setattr(self, field.name, getattr(data, field.name))
+        return self
+
+    def camel_case_data(self, data: dict[str, str | bool | int | None]) -> dict[str, str | int | bool]:
+        """
+        Camel case the keys of a dictionary.
+
+        Args:
+            data (dict[str, str  |  bool  |  None]): The dictionary to camel case.
+
+        Returns:
+            dict[str, str | bool]: The camel cased dictionary.
+        """
+        new: dict[str, str | bool | int] = {}
+        for key, value in data.items():
+            if value is not None:
+                new[key.title()] = value
+        return new
+
+    def dataclass_to_dict(self, dataclass: Any) -> dict[Any, Any]:
+        """
+        Convert a dataclass to a dictionary.
+
+        Args:
+            dataclass (Any): The dataclass to convert.
+
+        Returns:
+            dict[Any, Any]: The converted dataclass as a dictionary.
+        """
+        parameters = {}
+        for field in fields(dataclass):
+            value = getattr(dataclass, field.name)
+            if value == None:
+                continue
+            parameters[field.name] = value
+        return parameters
+
+    def json_to_dataclass(self, json: Any, format: Any, _use_from_dict: bool, _auto_unpack: bool) -> Any | list[Any]:
+        """
+        Format the JSON response data to a dataclass.
+
+        Args:
+            json (Any): JSON data to format.
+            format (Any): Dataclass or similar to unpack the JSON data into.
+            _use_from_dict (bool): Use dataclass wizard `fromdict()` or not.
+            _auto_unpack (bool): Use **data or not to unpack the data.
+
+        Returns:
+            Any | list[Any]: A list of the format object or a single format object.
+
+        """
+        if isinstance(json, list):
+            if _use_from_dict is True:
+                return list(fromdict(format, data) for data in json)
+
+            elif _auto_unpack is True:
+                return list(format(**data)for data in json)
+
+            else:
+                return list(format(data)for data in json)
+        else:
+            if _use_from_dict is True:
+                return fromdict(format, json)
+
+            elif _auto_unpack is True:
+                return format(**json)
+
+            else:
+                return format(json)
+
+    async def _call_api(self, api: str, parameters: Union[None, dict[str, Any]] = None, format_data: Union[bool, None] = None, format: Any = None, _use_from_dict: bool = True, _auto_unpack: bool = True) -> Any:
+        # TODO - Possibly convert the ending args to *args or similar.
+        """
+        Uses aiohttp.ClientSession() post request to access the AMP API endpoints. \n
+        Will automatically populate the `SESSIONID` parameter if it is not provided.
+
+        Args:
+            api (str): The API endpoint to call. eg `Core/GetModuleInfo`
+            parameters (dict[str, str]): The parameters to pass to the API endpoint.
+            format_data (Union[bool, None]): Controls whether the data returned from the API endpoint is formatted or not. Defaults to `None`.
+            format (Any): The dataclass the Response json will return. Defaults to `None`.
+            _use_from_dict (bool): Controls whether the data will use `fromdict` of dataclass wizard to unpack the data. Typical usage case is nested Dataclasses. Defaults to `True`.
+            _auto_unpack (bool): Controls whether the data will be unpacked automatically. Defaults to `True`.
+
+        Raises:
+            ValueError: When the API call returns no data or raises any exception.
+            ConnectionError: When the API call returns a status code other than 200.
+            PermissionError: When the API call returns a `Unauthorized Access` error or permission related error.
+
+        Returns:
+            Any: Returns the JSON response, either formatted or unformatted depending on `format_data`.
+        """
+        global FORMAT_DATA
+        header: dict = {"Accept": "text/javascript"}
+        post_req: ClientResponse | None
+        self._logger.debug(f"_call_api -> {api} was called with {parameters}")
+
+        # This should save us some boiler plate code throughout our API calls.
+        if parameters == None:
+            parameters = {}
+
+        api_session: APISession = self._bridge._sessions.get(self.InstanceID, APISession(id="0", ttl=datetime.now()))
+        if isinstance(api_session, APISession):
+            parameters["SESSIONID"] = api_session.id
+
+        json_data = json.dumps(parameters)
+
+        _url: str = self.url + "/API/" + api
+        # print("DEBUG", self.InstanceID, api, _url)
+        async with aiohttp.ClientSession() as session:
+            try:
+                post_req = await session.post(_url, headers=header, data=json_data)
+            # TODO - Need to not catch all Excepts..
+            # So I can handle each exception properly.
+            except Exception as e:
+                self._logger.error(f"DEBUG _call_api exception type: {type(e)}")
+                raise ValueError(e)
+
+            if post_req.content_length == 0:
+                raise ValueError(self.NO_DATA)
+
+            if post_req.status != 200:
+                raise ConnectionError(self.NO_DATA)
+
+            post_req_json: Any = await post_req.json()
+
+        if post_req_json == None:
+            raise ConnectionError(self.NO_DATA)
+
+        # They removed "result" from all replies thus breaking most if not all future code.
+        # This was an old example from pre 2.3 AMP API that could have the following return:
+        # `{'resultReason': 'Internal Auth - No reason given', 'success': False, 'result': 0}`
+        # print("DEBUG", "API CALL---->", api, type(post_req_json), parameters)
+        # print("DEBUG", post_req_json)
+        if isinstance(post_req_json, dict):
+            if api == "Core/Login":
+                return LoginResults(**post_req_json)
+
+            elif "result" in post_req_json:
+                post_req_json = post_req_json["result"]
+
+            elif "Title" in post_req_json:
+                post_req_json = post_req_json["Title"]
+                if isinstance(post_req_json, str) and post_req_json == "Unauthorized Access":
+                    self._logger.error(f'{api} failed because of {post_req_json}')
+                    api_session = APISession(id="0", ttl=datetime.now())
+                    self._bridge._sessions.update({self.InstanceID: api_session})
+                    raise PermissionError(self.UNAUTHORIZED_ACCESS)
+
+            elif isinstance(post_req_json, bool) and post_req_json == False:
+                self._logger.error(f"{api} failed because of {post_req_json}")
+                raise ConnectionError(self.FAILED_API)
+
+            elif isinstance(post_req_json, dict) and "Status" in post_req_json and post_req_json["Status"] == False:
+                self._logger.error(f"{api} failed because of Status: {post_req_json}")
+                return ConnectionError(self.FAILED_API)
+
+        # print("DEBUG", "FORMAT->", format_data, format)
+        if format is None or format_data is False:
+            return post_req_json
+
+        elif format_data is True or format_data is None and FORMAT_DATA is True:
+            return self.json_to_dataclass(json=post_req_json, format=format, _use_from_dict=_use_from_dict, _auto_unpack=_auto_unpack)
+
+    async def _connect(self) -> LoginResults | None:
+        """
+        Handles your 2FA code and logging into AMP while also handling the session ID. \n
+
+        Raises:
+            ValueError: If session ID is not a string or 2FA code is not a formatted properly.
+            TypeError: If the session is not an APISession object.
+
+        Returns:
+            bool | None: Returns False if an exception is thrown or the login attempt fails to provide a sessionID value. \n
+            Otherwise returns true and sets the class's sessionID value.
+        """
+        code: Union[str, TOTP] = ""
+
+        # get our InstanceID and use it to key for session_id
+        session: APISession = self._bridge._sessions.get(self.InstanceID, APISession(id="0", ttl=datetime.now()))
+        if isinstance(session, APISession):
+            ttl: timedelta = datetime.now() - session.ttl
+            if ttl.seconds > 240:
+                sessionID = "0"
+            else:
+                sessionID: str = session.id
+        else:
+            raise TypeError(f"session must be of type APISession. Received {type(session)}")
+
+        if sessionID == "0":
+            if self._bridge.use_2fa == True:
+                try:
+                    # Handles time based 2Factory Auth Key/Code
+                    code = TOTP(self._bridge.token).now()
+
+                except AttributeError:
+                    raise ValueError("Please check your 2 Factor Code, should not contain spaces, escape characters and it must be enclosed in quotes!")
+            else:
+                try:
+
+                    parameters = {
+                        'username': self._bridge.user,
+                        'password': self._bridge.password,
+                        'token': code,
+                        'rememberMe': True}
+
+                    result = await self._call_api(api='Core/Login', parameters=parameters, format_data=True, format=LoginResults)
+                    if isinstance(result, LoginResults):
+                        # This is our new sessions table to correlate InstanceID to a sessionID.
+                        api_session = APISession(id=result.sessionID, ttl=datetime.now())
+                        self._bridge._sessions.update({self.InstanceID: api_session})
+                        return result
+
+                    else:
+                        self._logger.warning("Failed response from Core/Login in _connect()")
+                        return result
+
+                except Exception as e:
+                    self._logger.warning(f'Core/Login Exception: {traceback.format_exc()}')
+        else:
+            return
+
+    async def call_end_point(self, api: str, parameters: None | dict[str, Any] = None) -> Any:
+        """
+        Universal API method for calling any API endpoint. Some API endpoints require ADS and some may require an Instance ID. \n
+
+        The Data returned will be unmodified. No DATACLASS returns.
+
+        Args:
+            api (str): API endpoint to call. `eg "Core/GetModuleInfo"` (Assume this starts with www.yourAMPURL.com/API/)
+            parameters (None | dict[str, str]): Parameters to pass to the API endpoint. Session ID is already handled for you. Defaults to None
+
+        Returns:
+            Any: Returns the JSON response from the API call.
+        """
+
+        result = await self._call_api(api=api, parameters=parameters)
+        return result
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/core.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/core.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,1692 +1,1692 @@
-from __future__ import annotations
-
-from typing import Any, Union
-
-from .base import Base
-from .types import *
-
-__all__ = ("Core",)
-
-
-class Core(Base):
-    """
-    Contains the base functions for any `/API/Core/` AMP API endpoints.
-
-    """
-    async def login(self, amp_user: str, amp_password: str, token: str = "", rememberME: bool = False, format_data: Union[bool, None] = None) -> LoginResults:
-        """
-        AMP API login function. \n
-
-        Args:
-            amp_user (str): The username for logging into the AMP Panel
-            amp_password (str): The password for logging into the AMP Panel
-            token (str, optional): AMP 2 Factor auth code; typically using `TOTP.now()`. Defaults to "".
-            rememberME (bool, optional): Remember me token.. Defaults to False.
-
-        Returns:
-            LoginResults: On success returns a LoginResult dataclass.
-                See `types.py -> LoginResult`
-        """
-        parameters = {
-            'username': amp_user,
-            'password': amp_password,
-            'token': token,
-            'rememberMe': rememberME}
-        result = await self._call_api(api='Core/Login', parameters=parameters, format_data=format_data, format=LoginResults)
-        return result
-
-    # Core.Logout:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def logout(self) -> None:
-        """
-        Logout from AMP. 
-
-        Returns:
-            None
-        """
-        await self._connect()
-        await self._call_api(api='Core/Logout')
-        return
-
-    async def get_api_spec(self) -> dict:
-        """
-        Get's all the API specs for the ADS or Instance.
-         - See `docs/api_spec.md`
-
-        Returns:
-            dict: A dictionary containing all of the API specs, their parameters and return types for the ADS or Instance.
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/GetAPISpec')
-        return result
-
-    async def get_updates(self, format_data: Union[bool, None] = None) -> Updates:
-        """
-        Requests the recent entries of the Instance Updates; will acquire all updates from previous API call of `getUpdate()`
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Updates: On success returns a Updates dataclass.
-                See `types.py -> Updates`
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/GetUpdates', format_data=format_data, format=Updates)
-        return result
-
-    async def send_console_message(self, msg: str) -> None:
-        """
-        Sends a string to the Console. (eg `/list`)
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        parameters = {'message': msg}
-        await self._call_api(api='Core/SendConsoleMessage', parameters=parameters)
-        return
-
-    async def start_instance(self, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Starts the AMP Server/Instance
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: Results from the API call.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/Start', format_data=format_data, format=ActionResult)
-        return result
-
-    async def stop_instance(self) -> None:
-        """
-        Stops the AMP Server/Instance
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        await self._call_api(api='Core/Stop')
-        return
-
-    async def restart_instance(self, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Restarts the AMP Server/Instance
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: Results from the API call.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/Restart', format_data=format_data, format=ActionResult)
-        return result
-
-    async def kill_instance(self) -> None:
-        """
-        Kills the AMP Server/Instance
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        await self._call_api(api='Core/Kill')
-        return
-
-    # Core.Suspend:({'Description': "Prevents the current instance from being started, and stops it if it's currently running.", 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def suspend_instance(self) -> None:
-        """
-        Prevents the current instance from being started, and stops it if it's currently running.
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        await self._call_api(api='Core/Suspend')
-        return
-
-    # Core.Resume:({'Description': 'Allows the service to be re-started after previously being suspended.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def resume_instance(self) -> None:
-        """
-        Allows the service to be re-started after previously being suspended.
-
-        Returns:
-            None: ""
-        """
-        await self._connect()
-        await self._call_api(api='Core/Resume')
-        return
-
-    async def get_status(self, format_data: Union[bool, None] = None) -> AppStatus:
-        """
-        Gets the AMP Server/Instance Status information.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Status: On success returns a Status dataclass.
-                See `types.py -> Status`
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/GetStatus', format_data=format_data, format=AppStatus)
-        return result
-
-    async def get_user_list(self, format_data: Union[bool, None] = None) -> list[Players]:
-        """
-        Returns a dictionary of the connected Users to the Server.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Players: on success returns a Player dataclass.
-                See `types.py -> list[Players]`
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/GetUserList', format_data=format_data, format=Players, _use_from_dict=False, _auto_unpack=False)
-        return result
-
-    async def get_schedule_data(self, format_data: Union[bool, None] = None) -> ScheduleData:
-        """
-        Returns a dictionary of the Server/Instance Schedule events and triggers.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ScheduleData: On success returns a ScheduleData dataclass.
-                See `types.py -> ScheduleData`
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/GetScheduleData', format_data=format_data, format=ScheduleData)
-        return result
-
-    async def end_user_session(self, session_id: str) -> None:
-        """
-        Closes the specified User's session ID to AMP.\n
-        **Requires ADS**
-
-        Args:
-            session_id (str): session ID to end.
-
-        Returns:
-            None: ""
-        """
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        parameters = {
-            'Id': session_id
-        }
-        await self._call_api(api='Core/EndUserSession', parameters=parameters)
-        return
-
-    async def get_active_amp_sessions(self, format_data: Union[bool, None] = None) -> list[Session]:
-        """
-        Returns currently active AMP Sessions.\n
-        **Requires ADS**
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Session: Returns a dataclass Session.
-                See `types.py -> Session`
-        """
-
-        if self.Module != "ADS":
-            raise RuntimeError(self.ADS_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='Core/GetActiveAMPSessions', format_data=format_data, format=Session, _use_from_dict=False)
-        return result
-
-    async def get_amp_user_info(self, name: str, format_data: Union[bool, None] = None) -> User:
-        """
-        Retrieves the AMP User information for the provided username.\n
-
-        Args:
-            name (str): AMP User name.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            User: On success returns a User dataclass. 
-                See `types.py -> User`
-        """
-
-        await self._connect()
-        parameters = {
-            'Username': name
-        }
-        result = await self._call_api(api='Core/GetAMPUserInfo', parameters=parameters, format_data=format_data, format=User, _use_from_dict=False)
-        return result
-
-    async def current_session_has_permission(self, permission_node: str) -> bool:
-        """
-        Retrieves the current Session IDs permissions. This will differ between the ADS and a Server/Instance.
-
-        Args:
-            permission_node (str): The permission node to check for. eg `Core.RoleManagement.DeleteRoles` \n
-                - Supports looking for a blocked permission node simply by appending `-` in front of the permission node. eg `-Core.RoleManagement.DeleteRoles`\n
-                - Supports wildcards `*`. eg `Core.RoleManagement.*`
-
-
-        Returns:
-            str | dict[str, Any] | list | bool | int | None: On success returns a bool.
-        """
-
-        await self._connect()
-        parameters = {
-            'PermissionNode': permission_node
-        }
-        result = await self._call_api(api='Core/CurrentSessionHasPermission', parameters=parameters)
-        return result
-
-    async def get_amp_role_permissions(self, role_id: str) -> list[Any]:
-        """
-        Retrieves the AMP Role permission nodes for the provided role ID.
-
-        Args:
-            role_id (str): The role ID. eg `5d6566e0-fae2-41d7-bfb6-d21033247f2e`
-
-        Returns:
-            list[Any]: On success returns a list containing all the permission nodes for the provided role ID.
-        """
-
-        await self._connect()
-        parameters = {
-            'RoleId': role_id
-        }
-        result = await self._call_api(api="Core/GetAMPRolePermissions", parameters=parameters)
-        return result
-
-    async def get_permissions_spec(self) -> dict[str, Any]:
-        """
-        Retrieves the AMP Permissions node tree.
-
-        Returns:
-            dict[str, Any]: On success returns a dictionary containing all the permission nodes, descriptions and other attributes.
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetPermissionsSpec")
-        return result
-
-    async def get_role_ids(self) -> dict[str, Any]:
-        """
-        Retrieves all the Roles AMP currently has and the role IDs.
-
-        Returns:
-            Roles: On success returns a dictionary containing all the roles and their IDs. \n
-            *Example*
-            `{'00000000-0000-0000-0000-000000000000': 'Default','cb984b09-a1c6-4cc0-b005-df8907f06590': 'Super Admins'}`
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/GetRoleIds')
-        return result
-
-    async def create_role(self, name: str, as_common_role: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Creates an AMP Role.
-
-        Args:
-            name (str): The name of the role.
-            as_common_role (bool, optional): A role that everyone has. Defaults to False.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a ActionResult dataclass.
-                See `types.py -> ActionResult`
-
-        """
-
-        await self._connect()
-        parameters = {
-            'Name': name,
-            'AsCommonRole': as_common_role
-        }
-        result = await self._call_api(api='Core/CreateRole', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    async def get_role(self, role_id: str, format_data: Union[bool, None] = None) -> Role:
-        """
-        Retrieves the AMP Role information for the provided role ID.
-
-        Args:
-            role_id (str): The role ID to get information for.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Role: On success returns a Role dataclass.
-                See `types.py -> Role`
-
-        """
-
-        await self._connect()
-        parameters = {
-            'RoleId': role_id
-        }
-        result = await self._call_api(api='Core/GetRole', parameters=parameters, format_data=format_data, format=Role)
-        return result
-
-    async def set_amp_user_role_membership(self, user_id: str, role_id: str, is_member: bool, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Adds a user to an AMP role.
-
-        Args:
-            user_id (str): User ID to add to the role.
-            role_id (str): Role ID to add the user to.
-            is_member (bool): `True` to add the user to the role, `False` to remove the user from the role.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'UserId': user_id,
-            'RoleId': role_id,
-            'IsMember': is_member
-        }
-        result = await self._call_api(api='Core/SetAMPUserRoleMembership', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    async def set_amp_role_permission(self, role_id: str, permission_node: str, enabled: Union[None, bool], format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Set a permission node to `True` or `False` for the provided AMP role.
-
-        Args:
-            role_id (str): AMP role id.
-            permission_node (str): AMP permission node. eg `Core.RoleManagement.DeleteRoles`
-            enabled (Union[None, bool]): Set a permission to `True`, `False` or `None` depending on the results you can disable or enable an entire tree node of permissions.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'RoleId': role_id,
-            'PermissionNode': permission_node,
-            'Enabled': enabled
-        }
-        result = await self._call_api(api='Core/SetAMPRolePermission', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    async def get_settings_spec(self) -> dict[str, Any]:
-        """
-        Retrieves a Server/Instance nodes list.
-            - See `util.getNodespec` for a list of possible nodes.
-
-        Returns:
-            dict[str, Any]: On success returns a dictionary containing all of the Server/Instance nodes and there information.
-        """
-
-        await self._connect()
-        result = await self._call_api(api='Core/GetSettingsSpec')
-        return result
-
-    async def get_config(self, node: str, format_data: Union[bool, None] = None) -> SettingSpec:
-        """
-        Returns the config settings for a specific node.\n
-
-        Args:
-            node (str): The AMP node to inspect eg `ADSModule.Networking.BaseURL`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Node: On success returns a dictionary containing the following. \n
-        """
-
-        await self._connect()
-        parameters = {
-            "node": node
-        }
-        result = await self._call_api(api="Core/GetConfig", parameters=parameters, format_data=format_data, format=SettingSpec)
-        return result
-
-    async def get_configs(self, nodes: list[str], format_data: Union[bool, None] = None) -> list[SettingSpec]:
-        """
-        Returns the config settings for each node in the list.\n
-
-        Args:
-            node (list[str]): List of nodes to look at.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[Node]: On success returns a list of Node dataclasses.
-                See `types.py -> Node`
-        """
-
-        await self._connect()
-        parameters = {
-            "nodes": nodes
-        }
-        result = await self._call_api(api="Core/GetConfigs", parameters=parameters, format_data=format_data, format=SettingSpec)
-        return result
-
-    async def get_update_info(self, format_data: Union[bool, None] = None) -> UpdateInfo:
-        """
-        Returns a data class `UpdateInfo` and `UpdateInfo.Build = AMP_Version` to access Version information for AMP.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            UpdateInfo: On success returns a UpdateInfo dataclass.
-                See `types.py -> UpdateInfo`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetUpdateInfo", format_data=format_data, format=UpdateInfo)
-        return result
-
-    async def get_all_amp_user_info(self, format_data: Union[bool, None] = None) -> list[User]:
-        """
-        Represents all the AMP User info.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[User]: On success returns a list of User dataclasses.
-                See `types.py -> User`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetAllAMPUserInfo", format_data=format_data, format=User, _use_from_dict=False)
-        return result
-
-    # Core.GetAuditLogEntries:({'Parameters': [{'Name': 'Before', 'TypeName': 'Nullable<DateTime>', 'Description': '', 'Optional': False}, {'Name': 'Count', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<IAuditLogEntry>', 'IsComplexType': True})
-    async def get_audit_log_entries(self, before: float, count: int, format_data: Union[bool, None] = None) -> list[AuditLogEntry]:
-        """
-        Returns the last X number of audit log entries.
-
-        Args:
-            before (float): A POSIX timestamp.
-            count (int): Number of entries to return.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[AuditLogEntry]: On success returns a list of AuditLogEntry dataclasses.
-                See `types.py -> AuditLogEntry`
-        """
-
-        await self._connect()
-        parameters = {
-            "Before": before,
-            "Count": count
-        }
-        result = await self._call_api(api="Core/GetAuditLogEntries", parameters=parameters, format_data=format_data, format=AuditLogEntry, _use_from_dict=False)
-        return result
-
-    # Core.GetSettingsSpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, IEnumerable<JObject>>', 'IsComplexType': True})
-    async def get_setting_spec(self, format_data: Union[bool, None] = None) -> list[SettingSpec]:
-        """
-        Returns a list of settings that can be changed.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[SettingSpec]: On success returns a list of Setting dataclasses.
-                See `types.py -> Setting`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetSettingsSpec", format_data=format_data, format=SettingSpec)
-        return result
-
-    # Core.RefreshSettingValueList:({'Parameters': [{'Name': 'Node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def refresh_setting_value_list(self, node: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Refreshes a setting's value list.
-
-        Args:
-            name (str): Setting name.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Name": node,
-        }
-        result = await self._call_api(api="Core/RefreshSettingValueList", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.RefreshSettingsSourceCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def refresh_settings_source_cache(self, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Refreshes the settings source cache.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/RefreshSettingsSourceCache", format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.GetSettingValues:({'Parameters': [{'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'WithRefresh', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'IDictionary<String, String>', 'IsComplexType': False})
-    async def get_setting_values(self, setting_node: str) -> dict[str, str]:
-        """
-        Returns the setting values.
-
-        Args:
-            name (str): Setting name.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            dict[str, str]: On success returns a dictionary of setting values.
-        """
-
-        await self._connect()
-        parameters = {
-            "SettingNode": setting_node
-        }
-        result = await self._call_api(api="Core/GetSettingValues", parameters=parameters)
-        return result
-
-    # Core.GetProvisionSpec:({'Parameters': [], 'ReturnTypeName': 'List<JObject>', 'IsComplexType': True})
-    async def get_provision_spec(self, format_data: Union[bool, None] = None) -> list[SettingSpec]:
-        """
-        Returns the provisioning spec.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[SettingSpec]: On success returns a list of provisioning spec.
-                See `types.py -> JObject`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetProvisionSpec", format_data=format_data, format=SettingSpec)
-        return result
-
-    # Core.SetConfigs:({'Parameters': [{'Name': 'data', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False})
-    async def set_configs(self, data: dict[str, str], format_data: Union[bool, None] = None) -> bool:
-        """
-        Set's multiple config node values.
-
-        Args:
-            data (dict[str, str]): Dictionary of configs to set.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            bool: On success returns a boolean.
-        """
-
-        await self._connect()
-        parameters = {
-            "data": data
-        }
-        result = await self._call_api(api="Core/SetConfigs", parameters=parameters)
-        return result
-
-    # Core.SetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def set_config(self, node: str, value: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Set a config node value.
-
-        Args:
-            name (str): Config node name.
-            value (str): Config node value.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "node": node,
-            "value": value
-        }
-        result = await self._call_api(api="Core/SetConfig", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.ActivateAMPLicence:({'Parameters': [{'Name': 'LicenceKey', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'QueryOnly', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<JObject>', 'IsComplexType': True})
-    async def activate_amp_license(self, license_key: str, query_only: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Activates an AMP license key.
-
-        Args:
-            license_key (str): The license key to activate.
-            query_only (bool, optional): Whether to query only. Defaults to False.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "LicenceKey": license_key,
-            "QueryOnly": query_only
-        }
-        result = await self._call_api(api="Core/ActivateAMPLicence", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.GetRoleData:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<AuthRoleSummary>', 'IsComplexType': True})
-    async def get_role_data(self, format_data: Union[bool, None] = None) -> list[Role]:
-        """
-        Get's a list of all the roles.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[Role]: On success returns a list of Role dataclasses.
-                See `types.py -> Role`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetRoleData", format_data=format_data, format=Role)
-        return result
-
-    # Core.DeleteRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_role(self, role_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Deletes a role.
-
-        Args:
-            role_id (str): The ID of the role to delete.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "RoleId": role_id
-        }
-        result = await self._call_api(api="Core/DeleteRole", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.RenameRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def rename_role(self, role_id: str, new_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Renames a role.
-
-        Args:
-            role_id (str): The ID of the role to rename.
-            new_name (str): The new name for the role.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "RoleId": role_id,
-            "NewName": new_name
-        }
-        result = await self._call_api(api="Core/RenameRole", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.AddEventTrigger:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def add_event_trigger(self, trigger_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Adds an event trigger.
-
-        Args:
-            trigger_id (str): The ID of the event trigger to add.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TriggerId": trigger_id
-        }
-        result = await self._call_api(api="Core/AddEventTrigger", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.RunEventTriggerImmediately:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def run_event_trigger_immediately(self, trigger_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Runs an event trigger immediately.
-
-        Args:
-            trigger_id (str): The ID of the event trigger to run.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TriggerId": trigger_id
-        }
-        result = await self._call_api(api="Core/RunEventTriggerImmediately", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.GetTimeIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_time_interval_trigger(self, id: str, format_data: Union[bool, None] = None) -> TimedTrigger:
-        """
-        Gets a time interval trigger information.
-
-        Args:
-            id (str): The ID of the time interval trigger to get.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            JObject: On success returns a JObject dataclass.
-                See `types.py -> JObject`
-        """
-
-        await self._connect()
-        parameters = {
-            "Id": id
-        }
-        result = await self._call_api(api="Core/GetTimeIntervalTrigger", parameters=parameters, format_data=format_data, format=TimedTrigger)
-        return result
-
-    # Core.EditIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def edit_interval_trigger(self, id: str, months: int, days: int, hours: int, minutes: int, days_of_month: int,
-                                    description: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Edits an interval trigger.
-        Args:
-            id (str): The ID of the interval trigger to edit.
-            months (int): The months of the interval trigger to edit.
-            days (int): The days of the interval trigger to edit.
-            hours (int): The hours of the interval trigger to edit.
-            minutes (int): The minutes of the interval trigger to edit.
-            days_of_month (int): The days of the month of the interval trigger to edit.
-            description (str): The description of the interval trigger to edit.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Id": id,
-            "months": months,
-            "days": days,
-            "hours": hours,
-            "minutes": minutes,
-            "daysOfMonth": days_of_month,
-            "description": description
-        }
-        result = await self._call_api(api="Core/EditIntervalTrigger", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.SetTriggerEnabled:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def set_trigger_enabled(self, id: str, enabled: bool, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Sets the enabled state of a trigger.
-
-        Args:
-            id (str): The ID of the trigger to edit.
-            enabled (bool): The enabled state of the trigger to edit.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Id": id,
-            "Enabled": enabled
-        }
-        result = await self._call_api(api="Core/SetTriggerEnabled", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.AddTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'MethodID', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def add_task(self, trigger_id: str, method_id: str, parameter_mapping: dict[str, str], format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Add a task.\n
-
-
-        Args:
-            trigger_id (str): The ID of the trigger to add.
-            method_id (str): The Task Method Name. eg. `Event.MinecraftModule.SendGlobalTitle`
-            parameter_mapping (dict[str, str]): The parameters to be populated related to the trigger_id/method_id.\n
-                - Example: `{ "Subtitle": "Hello World", Title: "Hello {@UserID}" }`
-
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TriggerID": trigger_id,
-            "MethodID": method_id,
-            "ParameterMapping": parameter_mapping
-        }
-        result = await self._call_api(api="Core/AddTask", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.EditTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def edit_task(self, trigger_id: str, task_id: str, parameter_mapping: dict[str, str], format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Edit a task.
-
-        Args:
-            trigger_id (str): The ID of the trigger to edit.
-            task_id (str): The ID of the task to edit. See `get_schedule_data().Tasks` to get IDs
-            parameter_mapping (dict[str, str]): The parameters to be updated on the task.\n
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TriggerID": trigger_id,
-            "TaskID": task_id,
-            "ParameterMapping": parameter_mapping
-        }
-        result = await self._call_api(api="Core/EditTask", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.ChangeTaskOrder:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewOrder', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def change_task_order(self, trigger_id: str, task_id: str, new_order: int, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Change the order of a task.
-
-        Args:
-            trigger_id (str): The ID of the trigger to modify.
-            task_id (str): The ID of the task to modify. See `get_schedule_data().Tasks` to get IDs
-            new_order (int): The new task position.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TriggerID": trigger_id,
-            "TaskID": task_id,
-            "NewOrder": new_order
-        }
-        result = await self._call_api(api="Core/ChangeTaskOrder", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.DeleteTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_task(self, trigger_id: str, task_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Delete a task.
-
-
-        Args:
-            trigger_id (_type_): The ID of the trigger to delete.
-            task_id (str): The ID of the task to delete. See `get_schedule_data().Tasks` to get IDs
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TriggerID": trigger_id,
-            "TaskID": task_id
-        }
-        result = await self._call_api(api="Core/DeleteTask", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.DeleteTrigger:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_trigger(self, trigger_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Delete a trigger.
-
-        Args:
-            trigger_id (str): The ID of the trigger to delete.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TriggerID": trigger_id
-        }
-        result = await self._call_api(api="Core/DeleteTrigger", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.GetAMPUsersSummary:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfoSummary>', 'IsComplexType': True})
-    async def get_amp_users_summary(self, format_data: Union[bool, None] = None) -> list[Login_UserInfo]:
-        """
-        Get all AMP users summary.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[UserInfoSummary]: On success returns a list of UserInfoSummary dataclass.
-                See `types.py -> UserInfoSummary`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetAMPUsersSummary", format_data=format_data, format=Login_UserInfo)
-        return result
-
-    # Core.CreateUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True})
-    async def create_user(self, username: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Create an AMP user.
-
-        Args:
-            username (str): Username.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = parameters = parameters = parameters = {
-            "Username": username
-        }
-        result = await self._call_api(api="Core/CreateUser", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.DeleteUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_user(self, username: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Delete an AMP user.
-
-        Args:
-            username (str): Username.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Username": username
-        }
-        result = await self._call_api(api="Core/DeleteUser", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.UpdateUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False},
-    # {'Name': 'Disabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'PasswordExpires', 'TypeName': 'Boolean', 'Description': '', 'Optional': False},
-    # {'Name': 'CannotChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'MustChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False},
-    # {'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def update_user_info(self, user_name: str, disabled: bool = False, password_expires: bool = False, cannot_change_password: bool = False,
-                               must_change_password: bool = False, email_address: str = "", format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Update an AMP user.
-
-        Args:
-            user_name (str): Username.
-            disabled (bool, optional): Disabled. Defaults to False.
-            password_expires (bool, optional): User password expires. Defaults to False.
-            cannot_change_password (bool, optional): User cannot change password. Defaults to False.
-            must_change_password (bool, optional): User must change password upon next login. Defaults to False.
-            email_address (str, optional): Email address. Defaults to "".
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Username": user_name,
-            "Disabled": disabled,
-            "PasswordExpires": password_expires,
-            "CannotChangePassword": cannot_change_password,
-            "MustChangePassword": must_change_password,
-            "EmailAddress": email_address
-        }
-        result = await self._call_api(api="Core/UpdateUserInfo", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.GetWebauthnChallenge:({'Parameters': [], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True})
-    async def get_webauthn_challenge(self, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Get a webauthn challenge.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetWebauthnChallenge", format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.GetWebauthnCredentialIDs:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_webauthn_credential_ids(self, username: str, format_data: Union[bool, None] = None) -> list[Any]:
-        """
-        Get a webauthn credential IDs.
-
-        Args:
-            username (str): Username.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "username": username
-        }
-        result = await self._call_api(api="Core/GetWebauthnCredentialIDs", parameters=parameters, format_data=format_data)
-        return result
-
-    # Core.WebauthnRegister:({'Parameters': [{'Name': 'attestationObject', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'clientDataJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def webauthn_register(self, attestation_object: str, client_data_json: str, description: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Webauthn register.
-
-        Args:
-            attestation_object (str): Attestation object.
-            client_data_json (str): Client data JSON.
-            description (str): Description.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "attestationObject": attestation_object,
-            "clientDataJSON": client_data_json,
-            "description": description
-        }
-        result = await self._call_api(api="Core/WebauthnRegister", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.GetWebauthnCredentialSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<WebauthnCredentialSummary>', 'IsComplexType': True})
-    async def get_webauthn_credential_summary(self, format_data: Union[bool, None] = None) -> list[Any]:
-        """
-        Get the webauthn credential summaries.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[Any] : List of webauthn credential summaries.
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetWebauthnCredentialSummaries", format_data=format_data)
-        return result
-
-    # Core.RevokeWebauthnCredential:({'Parameters': [{'Name': 'ID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def revoke_webauthn_credential(self, id: int, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Revoke a webauthn credential.
-
-        Args:
-            id (int): ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "ID": id
-        }
-        result = await self._call_api(api="Core/RevokeWebauthnCredential", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.UpdateAccountInfo:({'Parameters': [{'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def update_account_info(self, email_address: str, two_factor_pin: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Update account info.
-
-        Args:
-            email_address (str): Email address.
-            two_factor_pin (str): Two factor PIN.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "EmailAddress": email_address,
-            "TwoFactorPIN": two_factor_pin
-        }
-        result = await self._call_api(api="Core/UpdateAccountInfo", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.EnableTwoFactor:({'Description': 'Sets up two-factor authentication for the given user. ConfirmTwoFactorSetup must be invoked to complete setup.', 'Returns': 'Data container the URI for a QR code that should be scanned by a mobile authenticator.', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<TwoFactorSetupInfo>', 'IsComplexType': True})
-    async def enable_two_factor(self, username: str, password: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Sets up two-factor authentication for the given user. \n 
-        `**WARNING**` ConfirmTwoFactorSetup must be invoked to complete setup.
-
-        Args:
-            username (str): Username.
-            password (str): Password.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an dictionary with the structure \n
-            `{"Result" : {"ManualKey" : str, "Url" : str}, "Status": bool}`.
-        """
-
-        await self._connect()
-        parameters = {
-            "Username": username,
-            "Password": password
-        }
-        result = await self._call_api(api="Core/EnableTwoFactor", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.ConfirmTwoFactorSetup:({'Description': 'Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def confirm_two_factor_setup(self, username: str, two_factor_code: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor.
-
-        Args:
-            username (str): Username.
-            two_factor_code (str): Two factor code.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Username": username,
-            "TwoFactorCode": two_factor_code
-        }
-        result = await self._call_api(api="Core/ConfirmTwoFactorSetup", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.DisableTwoFactor:({'Parameters': [{'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def disable_two_factor(self, password: str, two_factor_code: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Disables two-factor authentication for the given user.
-
-        Args:
-            password (str): Password.
-            two_factor_code (str): Two factor code.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Password": password,
-            "TwoFactorCode": two_factor_code
-        }
-        result = await self._call_api(api="Core/DisableTwoFactor", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.ResetUserPassword:({'Description': 'For administrative users to alter the password of another user', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def reset_user_password(self, username: str, new_password: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        For administrative users to alter the password of another user.
-
-        Args:
-            username (str): Username.
-            new_password (str): New password.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Username": username,
-            "NewPassword": new_password
-        }
-        result = await self._call_api(api="Core/ResetUserPassword", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_instance_users(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Delete an Instances User list.
-
-        Args:
-            instance_id (str): The AMP Instance ID
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "InstanceId": instance_id
-        }
-
-        results = await self._call_api(api="Core/DeleteInstanceUsers", parameters=parameters, format_data=format_data, format=ActionResult)
-        return results
-
-    # Core.ChangeUserPassword:({'Description': 'For a user to change their own password, requires knowing the old password', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'OldPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False},
-    # {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def change_user_password(self, username: str, old_password: str, new_password: str, two_factor_pin: str = "", format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        For a user to change their own password, requires knowing the old password.
-
-        Args:
-            username (str): AMP user name.
-            old_password (str): Current AMP user password.
-            new_password (str): New AMP user password.
-            two_factor_pin (str): Two Factor PIN, if enabled. Defaults to "".
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Username": username,
-            "OldPassword": old_password,
-            "NewPassword": new_password,
-            "TwoFactorPIN": two_factor_pin
-        }
-
-        results = await self._call_api(api="Core/ChangeUserPassword", parameters=parameters, format_data=format_data, format=ActionResult)
-        return results
-
-    # Core.GetNewGuid:({'Parameters': [], 'ReturnTypeName': 'Guid', 'IsComplexType': False})
-    async def get_new_guid(self, format_data: Union[bool, None] = None) -> dict[str, Any]:
-        """
-        Get a new GUID.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a GUID.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetNewGuid", format_data=format_data)
-        return result
-
-    # Core.GetTasks:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<RunningTask>', 'IsComplexType': True})
-    async def get_tasks(self, format_data: Union[bool, None] = None) -> list[RunningTask]:
-        """
-        Get all tasks.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[RunningTask]: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetTasks", format_data=format_data, format=RunningTask)
-        return result
-
-    # Core.GetPortSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<ListeningPortSummary>', 'IsComplexType': True})
-    async def get_port_summaries(self, format_data: Union[bool, None] = None) -> list[Port]:
-        """
-        Get a summary of the instance's open ports.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[Port]: On success returns a list of Port dataclass.
-                See `types.py -> Port`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetPortSummaries", format_data=format_data, format=Port)
-        if format_data is None:
-            format_data = self.format_data
-
-        if format_data == False:
-            return result
-
-        elif isinstance(result, list):
-            return list(Port(**port) for port in result)
-        return result
-
-    # Core.CancelTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def cancel_task(self, task_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Cancel a task.
-
-        Args:
-            task_id (str): _description_
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a GUID.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TaskId": task_id
-        }
-        result = await self._call_api(api="Core/CancelTask", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.DismissTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def dismiss_task(self, task_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Dismiss a task notification.
-
-        Args:
-            task_id (str): _description_
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a GUID.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "TaskId": task_id
-        }
-        result = await self._call_api(api="Core/DismissTask", parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.DismissAllTasks:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def dismiss_all_tasks(self, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Dismiss all task notifications.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a GUID.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/DismissAllTasks", format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.GetUserInfo:({'Description': 'Provides information about a given in-application user (as opposed to AMP system users)', 'Returns': '', 'Parameters': [{'Name': 'UID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'SimpleUser', 'IsComplexType': True})
-    async def get_user_info(self, uid: str, format_data: Union[bool, None] = None) -> dict:
-        """
-        Provides information about a given in-application user (as opposed to AMP system users).
-
-        Args:
-            uid (str): _description_
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            dict: On success returns a dict.
-        """
-
-        await self._connect()
-        parameters = {
-            "UID": uid
-        }
-        result = await self._call_api(api="Core/GetUserInfo", parameters=parameters, format_data=format_data)
-        return result
-
-    # Core.UpdateApplication:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def update_application(self, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Update the Instance application.
-
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a GUID.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/UpdateApplication", format_data=format_data, format=ActionResult)
-        return result
-
-    # Core.AcknowledgeAMPUpdate:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def acknowledge_amp_update(self) -> None:
-        """
-        Approves an AMP update.
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        await self._call_api(api="Core/AcknowledgeAMPUpdate")
-        return
-
-    # Core.GetModuleInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_module_info(self, format_data: Union[bool, None] = None) -> Module:
-        """
-        Returns the module information.
-
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Module: On success returns a Module dataclass.
-                See `types.py -> Module`
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetModuleInfo", format_data=format_data, format=Module)
-        return result
-
-    # Core.GetUserActionsSpec:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False})
-    async def get_user_action_spec(self, format_data: Union[bool, None] = None) -> dict[str, Any]:
-        """
-        Get a specification of the user actions.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            dict[str, Any]: On success returns a dict.\n
-                - {'ADSModule': {},'CommonCorePlugin': {},'Core': {},'EmailSenderPlugin': {},'FileManagerPlugin': {},'LocalFileBackupPlugin': {}}
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetUserActionsSpec", format_data=format_data)
-        return result
-
-    # Core.GetRemoteLoginToken:({'Parameters': [{'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'IsTemporary', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'String', 'IsComplexType': False})
-    async def get_remote_login_token(self, description: Union[str, None] = None, is_temporary: Union[bool, None] = None, format_data: Union[bool, None] = None) -> str:
-        """
-        Get the remote login token.
-
-        Args:
-            description (Union[str, None], optional): Description. Defaults to None.
-            is_temporary (Union[bool, None], optional): Is temporary. Defaults to None.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            str: On success returns a str.
-                See `types.py -> str`
-        """
-
-        await self._connect()
-        parameters = {
-            "Description": description,
-            "IsTemporary": is_temporary
-        }
-        result = await self._call_api(api="Core/GetRemoteLoginToken", parameters=parameters, format_data=format_data)
-        return result
-
-    # Core.UpdateAMPInstance:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def update_amp_instance(self) -> None:
-        """
-        update_amp_instance 
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        await self._call_api(api="Core/UpdateAMPInstance")
-        return
-
-    # Core.RestartAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def restart_amp(self) -> None:
-        """
-        restart_amp 
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        await self._call_api(api="Core/RestartAMP")
-        return
-
-    # Core.UpgradeAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def upgrade_amp(self) -> None:
-        """
-        upgrade_amp 
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        await self._call_api(api="Core/UpgradeAMP")
-        return
-
-    # Core.GetDiagnosticsInfo:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False})
-    async def get_diagnostics_info(self, format_data: Union[bool, None] = None) -> Diagnostics:
-        """
-        Get's the system diagnostics information.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Diagnostics: On success returns a dictionary.\n
-
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetDiagnosticsInfo", format_data=format_data, format=Diagnostics, _use_from_dict=False, _auto_unpack=False)
-        return result
-
-    # Core.GetWebserverMetrics:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False})
-    async def get_webserver_metrics(self, format_data: Union[bool, None] = None) -> Any:
-        """
-        Gets the webserver metrics.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Any: UNK data returned by the API.
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/GetWebserverMetrics", format_data=format_data)
-        return result
-
-    # Core.CreateTestTask:({'Description': 'DEV: Creates a non-ending task with 50% progress for testing purposes', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def create_test_task(self) -> None:
-        """
-        **DEV**: Creates a non-ending task with 50% progress for testing purposes
-
-
-        Returns:
-            None: ""
-        """
-
-        await self._connect()
-        await self._call_api(api="Core/CreateTestTask")
-        return
-
-    # Core.AsyncTest:({'Description': 'DEV: Async test method', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False})
-    async def async_test(self) -> str:
-        """
-        **DEV**: Async test method
-
-
-        Returns:
-            str: Returns a string.
-        """
-
-        await self._connect()
-        result = await self._call_api(api="Core/AsyncTest")
-        return result
+from __future__ import annotations
+
+from typing import Any, Union
+
+from .base import Base
+from .types import *
+
+__all__ = ("Core",)
+
+
+class Core(Base):
+    """
+    Contains the base functions for any `/API/Core/` AMP API endpoints.
+
+    """
+    async def login(self, amp_user: str, amp_password: str, token: str = "", rememberME: bool = False, format_data: Union[bool, None] = None) -> LoginResults:
+        """
+        AMP API login function. \n
+
+        Args:
+            amp_user (str): The username for logging into the AMP Panel
+            amp_password (str): The password for logging into the AMP Panel
+            token (str, optional): AMP 2 Factor auth code; typically using `TOTP.now()`. Defaults to "".
+            rememberME (bool, optional): Remember me token.. Defaults to False.
+
+        Returns:
+            LoginResults: On success returns a LoginResult dataclass.
+                See `types.py -> LoginResult`
+        """
+        parameters = {
+            'username': amp_user,
+            'password': amp_password,
+            'token': token,
+            'rememberMe': rememberME}
+        result = await self._call_api(api='Core/Login', parameters=parameters, format_data=format_data, format=LoginResults)
+        return result
+
+    # Core.Logout:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def logout(self) -> None:
+        """
+        Logout from AMP. 
+
+        Returns:
+            None
+        """
+        await self._connect()
+        await self._call_api(api='Core/Logout')
+        return
+
+    async def get_api_spec(self) -> dict:
+        """
+        Get's all the API specs for the ADS or Instance.
+         - See `docs/api_spec.md`
+
+        Returns:
+            dict: A dictionary containing all of the API specs, their parameters and return types for the ADS or Instance.
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/GetAPISpec')
+        return result
+
+    async def get_updates(self, format_data: Union[bool, None] = None) -> Updates:
+        """
+        Requests the recent entries of the Instance Updates; will acquire all updates from previous API call of `getUpdate()`
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Updates: On success returns a Updates dataclass.
+                See `types.py -> Updates`
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/GetUpdates', format_data=format_data, format=Updates)
+        return result
+
+    async def send_console_message(self, msg: str) -> None:
+        """
+        Sends a string to the Console. (eg `/list`)
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        parameters = {'message': msg}
+        await self._call_api(api='Core/SendConsoleMessage', parameters=parameters)
+        return
+
+    async def start_instance(self, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Starts the AMP Server/Instance
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: Results from the API call.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/Start', format_data=format_data, format=ActionResult)
+        return result
+
+    async def stop_instance(self) -> None:
+        """
+        Stops the AMP Server/Instance
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        await self._call_api(api='Core/Stop')
+        return
+
+    async def restart_instance(self, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Restarts the AMP Server/Instance
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: Results from the API call.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/Restart', format_data=format_data, format=ActionResult)
+        return result
+
+    async def kill_instance(self) -> None:
+        """
+        Kills the AMP Server/Instance
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        await self._call_api(api='Core/Kill')
+        return
+
+    # Core.Suspend:({'Description': "Prevents the current instance from being started, and stops it if it's currently running.", 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def suspend_instance(self) -> None:
+        """
+        Prevents the current instance from being started, and stops it if it's currently running.
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        await self._call_api(api='Core/Suspend')
+        return
+
+    # Core.Resume:({'Description': 'Allows the service to be re-started after previously being suspended.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def resume_instance(self) -> None:
+        """
+        Allows the service to be re-started after previously being suspended.
+
+        Returns:
+            None: ""
+        """
+        await self._connect()
+        await self._call_api(api='Core/Resume')
+        return
+
+    async def get_status(self, format_data: Union[bool, None] = None) -> AppStatus:
+        """
+        Gets the AMP Server/Instance Status information.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Status: On success returns a Status dataclass.
+                See `types.py -> Status`
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/GetStatus', format_data=format_data, format=AppStatus)
+        return result
+
+    async def get_user_list(self, format_data: Union[bool, None] = None) -> list[Players]:
+        """
+        Returns a dictionary of the connected Users to the Server.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Players: on success returns a Player dataclass.
+                See `types.py -> list[Players]`
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/GetUserList', format_data=format_data, format=Players, _use_from_dict=False, _auto_unpack=False)
+        return result
+
+    async def get_schedule_data(self, format_data: Union[bool, None] = None) -> ScheduleData:
+        """
+        Returns a dictionary of the Server/Instance Schedule events and triggers.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ScheduleData: On success returns a ScheduleData dataclass.
+                See `types.py -> ScheduleData`
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/GetScheduleData', format_data=format_data, format=ScheduleData)
+        return result
+
+    async def end_user_session(self, session_id: str) -> None:
+        """
+        Closes the specified User's session ID to AMP.\n
+        **Requires ADS**
+
+        Args:
+            session_id (str): session ID to end.
+
+        Returns:
+            None: ""
+        """
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        parameters = {
+            'Id': session_id
+        }
+        await self._call_api(api='Core/EndUserSession', parameters=parameters)
+        return
+
+    async def get_active_amp_sessions(self, format_data: Union[bool, None] = None) -> list[Session]:
+        """
+        Returns currently active AMP Sessions.\n
+        **Requires ADS**
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Session: Returns a dataclass Session.
+                See `types.py -> Session`
+        """
+
+        if self.Module != "ADS":
+            raise RuntimeError(self.ADS_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='Core/GetActiveAMPSessions', format_data=format_data, format=Session, _use_from_dict=False)
+        return result
+
+    async def get_amp_user_info(self, name: str, format_data: Union[bool, None] = None) -> User:
+        """
+        Retrieves the AMP User information for the provided username.\n
+
+        Args:
+            name (str): AMP User name.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            User: On success returns a User dataclass. 
+                See `types.py -> User`
+        """
+
+        await self._connect()
+        parameters = {
+            'Username': name
+        }
+        result = await self._call_api(api='Core/GetAMPUserInfo', parameters=parameters, format_data=format_data, format=User, _use_from_dict=False)
+        return result
+
+    async def current_session_has_permission(self, permission_node: str) -> bool:
+        """
+        Retrieves the current Session IDs permissions. This will differ between the ADS and a Server/Instance.
+
+        Args:
+            permission_node (str): The permission node to check for. eg `Core.RoleManagement.DeleteRoles` \n
+                - Supports looking for a blocked permission node simply by appending `-` in front of the permission node. eg `-Core.RoleManagement.DeleteRoles`\n
+                - Supports wildcards `*`. eg `Core.RoleManagement.*`
+
+
+        Returns:
+            str | dict[str, Any] | list | bool | int | None: On success returns a bool.
+        """
+
+        await self._connect()
+        parameters = {
+            'PermissionNode': permission_node
+        }
+        result = await self._call_api(api='Core/CurrentSessionHasPermission', parameters=parameters)
+        return result
+
+    async def get_amp_role_permissions(self, role_id: str) -> list[Any]:
+        """
+        Retrieves the AMP Role permission nodes for the provided role ID.
+
+        Args:
+            role_id (str): The role ID. eg `5d6566e0-fae2-41d7-bfb6-d21033247f2e`
+
+        Returns:
+            list[Any]: On success returns a list containing all the permission nodes for the provided role ID.
+        """
+
+        await self._connect()
+        parameters = {
+            'RoleId': role_id
+        }
+        result = await self._call_api(api="Core/GetAMPRolePermissions", parameters=parameters)
+        return result
+
+    async def get_permissions_spec(self) -> dict[str, Any]:
+        """
+        Retrieves the AMP Permissions node tree.
+
+        Returns:
+            dict[str, Any]: On success returns a dictionary containing all the permission nodes, descriptions and other attributes.
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetPermissionsSpec")
+        return result
+
+    async def get_role_ids(self) -> dict[str, Any]:
+        """
+        Retrieves all the Roles AMP currently has and the role IDs.
+
+        Returns:
+            Roles: On success returns a dictionary containing all the roles and their IDs. \n
+            *Example*
+            `{'00000000-0000-0000-0000-000000000000': 'Default','cb984b09-a1c6-4cc0-b005-df8907f06590': 'Super Admins'}`
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/GetRoleIds')
+        return result
+
+    async def create_role(self, name: str, as_common_role: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Creates an AMP Role.
+
+        Args:
+            name (str): The name of the role.
+            as_common_role (bool, optional): A role that everyone has. Defaults to False.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a ActionResult dataclass.
+                See `types.py -> ActionResult`
+
+        """
+
+        await self._connect()
+        parameters = {
+            'Name': name,
+            'AsCommonRole': as_common_role
+        }
+        result = await self._call_api(api='Core/CreateRole', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    async def get_role(self, role_id: str, format_data: Union[bool, None] = None) -> Role:
+        """
+        Retrieves the AMP Role information for the provided role ID.
+
+        Args:
+            role_id (str): The role ID to get information for.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Role: On success returns a Role dataclass.
+                See `types.py -> Role`
+
+        """
+
+        await self._connect()
+        parameters = {
+            'RoleId': role_id
+        }
+        result = await self._call_api(api='Core/GetRole', parameters=parameters, format_data=format_data, format=Role)
+        return result
+
+    async def set_amp_user_role_membership(self, user_id: str, role_id: str, is_member: bool, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Adds a user to an AMP role.
+
+        Args:
+            user_id (str): User ID to add to the role.
+            role_id (str): Role ID to add the user to.
+            is_member (bool): `True` to add the user to the role, `False` to remove the user from the role.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'UserId': user_id,
+            'RoleId': role_id,
+            'IsMember': is_member
+        }
+        result = await self._call_api(api='Core/SetAMPUserRoleMembership', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    async def set_amp_role_permission(self, role_id: str, permission_node: str, enabled: Union[None, bool], format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Set a permission node to `True` or `False` for the provided AMP role.
+
+        Args:
+            role_id (str): AMP role id.
+            permission_node (str): AMP permission node. eg `Core.RoleManagement.DeleteRoles`
+            enabled (Union[None, bool]): Set a permission to `True`, `False` or `None` depending on the results you can disable or enable an entire tree node of permissions.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'RoleId': role_id,
+            'PermissionNode': permission_node,
+            'Enabled': enabled
+        }
+        result = await self._call_api(api='Core/SetAMPRolePermission', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    async def get_settings_spec(self) -> dict[str, Any]:
+        """
+        Retrieves a Server/Instance nodes list.
+            - See `util.getNodespec` for a list of possible nodes.
+
+        Returns:
+            dict[str, Any]: On success returns a dictionary containing all of the Server/Instance nodes and there information.
+        """
+
+        await self._connect()
+        result = await self._call_api(api='Core/GetSettingsSpec')
+        return result
+
+    async def get_config(self, node: str, format_data: Union[bool, None] = None) -> SettingSpec:
+        """
+        Returns the config settings for a specific node.\n
+
+        Args:
+            node (str): The AMP node to inspect eg `ADSModule.Networking.BaseURL`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Node: On success returns a dictionary containing the following. \n
+        """
+
+        await self._connect()
+        parameters = {
+            "node": node
+        }
+        result = await self._call_api(api="Core/GetConfig", parameters=parameters, format_data=format_data, format=SettingSpec)
+        return result
+
+    async def get_configs(self, nodes: list[str], format_data: Union[bool, None] = None) -> list[SettingSpec]:
+        """
+        Returns the config settings for each node in the list.\n
+
+        Args:
+            node (list[str]): List of nodes to look at.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[Node]: On success returns a list of Node dataclasses.
+                See `types.py -> Node`
+        """
+
+        await self._connect()
+        parameters = {
+            "nodes": nodes
+        }
+        result = await self._call_api(api="Core/GetConfigs", parameters=parameters, format_data=format_data, format=SettingSpec)
+        return result
+
+    async def get_update_info(self, format_data: Union[bool, None] = None) -> UpdateInfo:
+        """
+        Returns a data class `UpdateInfo` and `UpdateInfo.Build = AMP_Version` to access Version information for AMP.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            UpdateInfo: On success returns a UpdateInfo dataclass.
+                See `types.py -> UpdateInfo`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetUpdateInfo", format_data=format_data, format=UpdateInfo)
+        return result
+
+    async def get_all_amp_user_info(self, format_data: Union[bool, None] = None) -> list[User]:
+        """
+        Represents all the AMP User info.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[User]: On success returns a list of User dataclasses.
+                See `types.py -> User`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetAllAMPUserInfo", format_data=format_data, format=User, _use_from_dict=False)
+        return result
+
+    # Core.GetAuditLogEntries:({'Parameters': [{'Name': 'Before', 'TypeName': 'Nullable<DateTime>', 'Description': '', 'Optional': False}, {'Name': 'Count', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<IAuditLogEntry>', 'IsComplexType': True})
+    async def get_audit_log_entries(self, before: float, count: int, format_data: Union[bool, None] = None) -> list[AuditLogEntry]:
+        """
+        Returns the last X number of audit log entries.
+
+        Args:
+            before (float): A POSIX timestamp.
+            count (int): Number of entries to return.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[AuditLogEntry]: On success returns a list of AuditLogEntry dataclasses.
+                See `types.py -> AuditLogEntry`
+        """
+
+        await self._connect()
+        parameters = {
+            "Before": before,
+            "Count": count
+        }
+        result = await self._call_api(api="Core/GetAuditLogEntries", parameters=parameters, format_data=format_data, format=AuditLogEntry, _use_from_dict=False)
+        return result
+
+    # Core.GetSettingsSpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, IEnumerable<JObject>>', 'IsComplexType': True})
+    async def get_setting_spec(self, format_data: Union[bool, None] = None) -> list[SettingSpec]:
+        """
+        Returns a list of settings that can be changed.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[SettingSpec]: On success returns a list of Setting dataclasses.
+                See `types.py -> Setting`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetSettingsSpec", format_data=format_data, format=SettingSpec)
+        return result
+
+    # Core.RefreshSettingValueList:({'Parameters': [{'Name': 'Node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def refresh_setting_value_list(self, node: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Refreshes a setting's value list.
+
+        Args:
+            name (str): Setting name.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Name": node,
+        }
+        result = await self._call_api(api="Core/RefreshSettingValueList", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.RefreshSettingsSourceCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def refresh_settings_source_cache(self, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Refreshes the settings source cache.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/RefreshSettingsSourceCache", format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.GetSettingValues:({'Parameters': [{'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'WithRefresh', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'IDictionary<String, String>', 'IsComplexType': False})
+    async def get_setting_values(self, setting_node: str) -> dict[str, str]:
+        """
+        Returns the setting values.
+
+        Args:
+            name (str): Setting name.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            dict[str, str]: On success returns a dictionary of setting values.
+        """
+
+        await self._connect()
+        parameters = {
+            "SettingNode": setting_node
+        }
+        result = await self._call_api(api="Core/GetSettingValues", parameters=parameters)
+        return result
+
+    # Core.GetProvisionSpec:({'Parameters': [], 'ReturnTypeName': 'List<JObject>', 'IsComplexType': True})
+    async def get_provision_spec(self, format_data: Union[bool, None] = None) -> list[SettingSpec]:
+        """
+        Returns the provisioning spec.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[SettingSpec]: On success returns a list of provisioning spec.
+                See `types.py -> JObject`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetProvisionSpec", format_data=format_data, format=SettingSpec)
+        return result
+
+    # Core.SetConfigs:({'Parameters': [{'Name': 'data', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False})
+    async def set_configs(self, data: dict[str, str], format_data: Union[bool, None] = None) -> bool:
+        """
+        Set's multiple config node values.
+
+        Args:
+            data (dict[str, str]): Dictionary of configs to set.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            bool: On success returns a boolean.
+        """
+
+        await self._connect()
+        parameters = {
+            "data": data
+        }
+        result = await self._call_api(api="Core/SetConfigs", parameters=parameters)
+        return result
+
+    # Core.SetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def set_config(self, node: str, value: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Set a config node value.
+
+        Args:
+            name (str): Config node name.
+            value (str): Config node value.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "node": node,
+            "value": value
+        }
+        result = await self._call_api(api="Core/SetConfig", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.ActivateAMPLicence:({'Parameters': [{'Name': 'LicenceKey', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'QueryOnly', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<JObject>', 'IsComplexType': True})
+    async def activate_amp_license(self, license_key: str, query_only: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Activates an AMP license key.
+
+        Args:
+            license_key (str): The license key to activate.
+            query_only (bool, optional): Whether to query only. Defaults to False.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "LicenceKey": license_key,
+            "QueryOnly": query_only
+        }
+        result = await self._call_api(api="Core/ActivateAMPLicence", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.GetRoleData:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<AuthRoleSummary>', 'IsComplexType': True})
+    async def get_role_data(self, format_data: Union[bool, None] = None) -> list[Role]:
+        """
+        Get's a list of all the roles.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[Role]: On success returns a list of Role dataclasses.
+                See `types.py -> Role`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetRoleData", format_data=format_data, format=Role)
+        return result
+
+    # Core.DeleteRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_role(self, role_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Deletes a role.
+
+        Args:
+            role_id (str): The ID of the role to delete.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "RoleId": role_id
+        }
+        result = await self._call_api(api="Core/DeleteRole", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.RenameRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def rename_role(self, role_id: str, new_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Renames a role.
+
+        Args:
+            role_id (str): The ID of the role to rename.
+            new_name (str): The new name for the role.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "RoleId": role_id,
+            "NewName": new_name
+        }
+        result = await self._call_api(api="Core/RenameRole", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.AddEventTrigger:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def add_event_trigger(self, trigger_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Adds an event trigger.
+
+        Args:
+            trigger_id (str): The ID of the event trigger to add.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TriggerId": trigger_id
+        }
+        result = await self._call_api(api="Core/AddEventTrigger", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.RunEventTriggerImmediately:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def run_event_trigger_immediately(self, trigger_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Runs an event trigger immediately.
+
+        Args:
+            trigger_id (str): The ID of the event trigger to run.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TriggerId": trigger_id
+        }
+        result = await self._call_api(api="Core/RunEventTriggerImmediately", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.GetTimeIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_time_interval_trigger(self, id: str, format_data: Union[bool, None] = None) -> TimedTrigger:
+        """
+        Gets a time interval trigger information.
+
+        Args:
+            id (str): The ID of the time interval trigger to get.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            JObject: On success returns a JObject dataclass.
+                See `types.py -> JObject`
+        """
+
+        await self._connect()
+        parameters = {
+            "Id": id
+        }
+        result = await self._call_api(api="Core/GetTimeIntervalTrigger", parameters=parameters, format_data=format_data, format=TimedTrigger)
+        return result
+
+    # Core.EditIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def edit_interval_trigger(self, id: str, months: int, days: int, hours: int, minutes: int, days_of_month: int,
+                                    description: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Edits an interval trigger.
+        Args:
+            id (str): The ID of the interval trigger to edit.
+            months (int): The months of the interval trigger to edit.
+            days (int): The days of the interval trigger to edit.
+            hours (int): The hours of the interval trigger to edit.
+            minutes (int): The minutes of the interval trigger to edit.
+            days_of_month (int): The days of the month of the interval trigger to edit.
+            description (str): The description of the interval trigger to edit.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Id": id,
+            "months": months,
+            "days": days,
+            "hours": hours,
+            "minutes": minutes,
+            "daysOfMonth": days_of_month,
+            "description": description
+        }
+        result = await self._call_api(api="Core/EditIntervalTrigger", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.SetTriggerEnabled:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def set_trigger_enabled(self, id: str, enabled: bool, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Sets the enabled state of a trigger.
+
+        Args:
+            id (str): The ID of the trigger to edit.
+            enabled (bool): The enabled state of the trigger to edit.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Id": id,
+            "Enabled": enabled
+        }
+        result = await self._call_api(api="Core/SetTriggerEnabled", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.AddTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'MethodID', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def add_task(self, trigger_id: str, method_id: str, parameter_mapping: dict[str, str], format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Add a task.\n
+
+
+        Args:
+            trigger_id (str): The ID of the trigger to add.
+            method_id (str): The Task Method Name. eg. `Event.MinecraftModule.SendGlobalTitle`
+            parameter_mapping (dict[str, str]): The parameters to be populated related to the trigger_id/method_id.\n
+                - Example: `{ "Subtitle": "Hello World", Title: "Hello {@UserID}" }`
+
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TriggerID": trigger_id,
+            "MethodID": method_id,
+            "ParameterMapping": parameter_mapping
+        }
+        result = await self._call_api(api="Core/AddTask", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.EditTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def edit_task(self, trigger_id: str, task_id: str, parameter_mapping: dict[str, str], format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Edit a task.
+
+        Args:
+            trigger_id (str): The ID of the trigger to edit.
+            task_id (str): The ID of the task to edit. See `get_schedule_data().Tasks` to get IDs
+            parameter_mapping (dict[str, str]): The parameters to be updated on the task.\n
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TriggerID": trigger_id,
+            "TaskID": task_id,
+            "ParameterMapping": parameter_mapping
+        }
+        result = await self._call_api(api="Core/EditTask", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.ChangeTaskOrder:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewOrder', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def change_task_order(self, trigger_id: str, task_id: str, new_order: int, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Change the order of a task.
+
+        Args:
+            trigger_id (str): The ID of the trigger to modify.
+            task_id (str): The ID of the task to modify. See `get_schedule_data().Tasks` to get IDs
+            new_order (int): The new task position.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TriggerID": trigger_id,
+            "TaskID": task_id,
+            "NewOrder": new_order
+        }
+        result = await self._call_api(api="Core/ChangeTaskOrder", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.DeleteTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_task(self, trigger_id: str, task_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Delete a task.
+
+
+        Args:
+            trigger_id (_type_): The ID of the trigger to delete.
+            task_id (str): The ID of the task to delete. See `get_schedule_data().Tasks` to get IDs
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TriggerID": trigger_id,
+            "TaskID": task_id
+        }
+        result = await self._call_api(api="Core/DeleteTask", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.DeleteTrigger:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_trigger(self, trigger_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Delete a trigger.
+
+        Args:
+            trigger_id (str): The ID of the trigger to delete.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TriggerID": trigger_id
+        }
+        result = await self._call_api(api="Core/DeleteTrigger", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.GetAMPUsersSummary:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfoSummary>', 'IsComplexType': True})
+    async def get_amp_users_summary(self, format_data: Union[bool, None] = None) -> list[Login_UserInfo]:
+        """
+        Get all AMP users summary.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[UserInfoSummary]: On success returns a list of UserInfoSummary dataclass.
+                See `types.py -> UserInfoSummary`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetAMPUsersSummary", format_data=format_data, format=Login_UserInfo)
+        return result
+
+    # Core.CreateUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True})
+    async def create_user(self, username: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Create an AMP user.
+
+        Args:
+            username (str): Username.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = parameters = parameters = parameters = {
+            "Username": username
+        }
+        result = await self._call_api(api="Core/CreateUser", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.DeleteUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_user(self, username: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Delete an AMP user.
+
+        Args:
+            username (str): Username.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Username": username
+        }
+        result = await self._call_api(api="Core/DeleteUser", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.UpdateUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False},
+    # {'Name': 'Disabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'PasswordExpires', 'TypeName': 'Boolean', 'Description': '', 'Optional': False},
+    # {'Name': 'CannotChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'MustChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False},
+    # {'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def update_user_info(self, user_name: str, disabled: bool = False, password_expires: bool = False, cannot_change_password: bool = False,
+                               must_change_password: bool = False, email_address: str = "", format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Update an AMP user.
+
+        Args:
+            user_name (str): Username.
+            disabled (bool, optional): Disabled. Defaults to False.
+            password_expires (bool, optional): User password expires. Defaults to False.
+            cannot_change_password (bool, optional): User cannot change password. Defaults to False.
+            must_change_password (bool, optional): User must change password upon next login. Defaults to False.
+            email_address (str, optional): Email address. Defaults to "".
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Username": user_name,
+            "Disabled": disabled,
+            "PasswordExpires": password_expires,
+            "CannotChangePassword": cannot_change_password,
+            "MustChangePassword": must_change_password,
+            "EmailAddress": email_address
+        }
+        result = await self._call_api(api="Core/UpdateUserInfo", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.GetWebauthnChallenge:({'Parameters': [], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True})
+    async def get_webauthn_challenge(self, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Get a webauthn challenge.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetWebauthnChallenge", format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.GetWebauthnCredentialIDs:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_webauthn_credential_ids(self, username: str, format_data: Union[bool, None] = None) -> list[Any]:
+        """
+        Get a webauthn credential IDs.
+
+        Args:
+            username (str): Username.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "username": username
+        }
+        result = await self._call_api(api="Core/GetWebauthnCredentialIDs", parameters=parameters, format_data=format_data)
+        return result
+
+    # Core.WebauthnRegister:({'Parameters': [{'Name': 'attestationObject', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'clientDataJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def webauthn_register(self, attestation_object: str, client_data_json: str, description: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Webauthn register.
+
+        Args:
+            attestation_object (str): Attestation object.
+            client_data_json (str): Client data JSON.
+            description (str): Description.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "attestationObject": attestation_object,
+            "clientDataJSON": client_data_json,
+            "description": description
+        }
+        result = await self._call_api(api="Core/WebauthnRegister", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.GetWebauthnCredentialSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<WebauthnCredentialSummary>', 'IsComplexType': True})
+    async def get_webauthn_credential_summary(self, format_data: Union[bool, None] = None) -> list[Any]:
+        """
+        Get the webauthn credential summaries.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[Any] : List of webauthn credential summaries.
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetWebauthnCredentialSummaries", format_data=format_data)
+        return result
+
+    # Core.RevokeWebauthnCredential:({'Parameters': [{'Name': 'ID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def revoke_webauthn_credential(self, id: int, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Revoke a webauthn credential.
+
+        Args:
+            id (int): ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "ID": id
+        }
+        result = await self._call_api(api="Core/RevokeWebauthnCredential", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.UpdateAccountInfo:({'Parameters': [{'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def update_account_info(self, email_address: str, two_factor_pin: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Update account info.
+
+        Args:
+            email_address (str): Email address.
+            two_factor_pin (str): Two factor PIN.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "EmailAddress": email_address,
+            "TwoFactorPIN": two_factor_pin
+        }
+        result = await self._call_api(api="Core/UpdateAccountInfo", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.EnableTwoFactor:({'Description': 'Sets up two-factor authentication for the given user. ConfirmTwoFactorSetup must be invoked to complete setup.', 'Returns': 'Data container the URI for a QR code that should be scanned by a mobile authenticator.', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<TwoFactorSetupInfo>', 'IsComplexType': True})
+    async def enable_two_factor(self, username: str, password: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Sets up two-factor authentication for the given user. \n 
+        `**WARNING**` ConfirmTwoFactorSetup must be invoked to complete setup.
+
+        Args:
+            username (str): Username.
+            password (str): Password.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an dictionary with the structure \n
+            `{"Result" : {"ManualKey" : str, "Url" : str}, "Status": bool}`.
+        """
+
+        await self._connect()
+        parameters = {
+            "Username": username,
+            "Password": password
+        }
+        result = await self._call_api(api="Core/EnableTwoFactor", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.ConfirmTwoFactorSetup:({'Description': 'Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def confirm_two_factor_setup(self, username: str, two_factor_code: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor.
+
+        Args:
+            username (str): Username.
+            two_factor_code (str): Two factor code.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Username": username,
+            "TwoFactorCode": two_factor_code
+        }
+        result = await self._call_api(api="Core/ConfirmTwoFactorSetup", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.DisableTwoFactor:({'Parameters': [{'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def disable_two_factor(self, password: str, two_factor_code: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Disables two-factor authentication for the given user.
+
+        Args:
+            password (str): Password.
+            two_factor_code (str): Two factor code.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Password": password,
+            "TwoFactorCode": two_factor_code
+        }
+        result = await self._call_api(api="Core/DisableTwoFactor", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.ResetUserPassword:({'Description': 'For administrative users to alter the password of another user', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def reset_user_password(self, username: str, new_password: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        For administrative users to alter the password of another user.
+
+        Args:
+            username (str): Username.
+            new_password (str): New password.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Username": username,
+            "NewPassword": new_password
+        }
+        result = await self._call_api(api="Core/ResetUserPassword", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_instance_users(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Delete an Instances User list.
+
+        Args:
+            instance_id (str): The AMP Instance ID
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "InstanceId": instance_id
+        }
+
+        results = await self._call_api(api="Core/DeleteInstanceUsers", parameters=parameters, format_data=format_data, format=ActionResult)
+        return results
+
+    # Core.ChangeUserPassword:({'Description': 'For a user to change their own password, requires knowing the old password', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'OldPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False},
+    # {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def change_user_password(self, username: str, old_password: str, new_password: str, two_factor_pin: str = "", format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        For a user to change their own password, requires knowing the old password.
+
+        Args:
+            username (str): AMP user name.
+            old_password (str): Current AMP user password.
+            new_password (str): New AMP user password.
+            two_factor_pin (str): Two Factor PIN, if enabled. Defaults to "".
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Username": username,
+            "OldPassword": old_password,
+            "NewPassword": new_password,
+            "TwoFactorPIN": two_factor_pin
+        }
+
+        results = await self._call_api(api="Core/ChangeUserPassword", parameters=parameters, format_data=format_data, format=ActionResult)
+        return results
+
+    # Core.GetNewGuid:({'Parameters': [], 'ReturnTypeName': 'Guid', 'IsComplexType': False})
+    async def get_new_guid(self, format_data: Union[bool, None] = None) -> dict[str, Any]:
+        """
+        Get a new GUID.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a GUID.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetNewGuid", format_data=format_data)
+        return result
+
+    # Core.GetTasks:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<RunningTask>', 'IsComplexType': True})
+    async def get_tasks(self, format_data: Union[bool, None] = None) -> list[RunningTask]:
+        """
+        Get all tasks.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[RunningTask]: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetTasks", format_data=format_data, format=RunningTask)
+        return result
+
+    # Core.GetPortSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<ListeningPortSummary>', 'IsComplexType': True})
+    async def get_port_summaries(self, format_data: Union[bool, None] = None) -> list[Port]:
+        """
+        Get a summary of the instance's open ports.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[Port]: On success returns a list of Port dataclass.
+                See `types.py -> Port`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetPortSummaries", format_data=format_data, format=Port)
+        if format_data is None:
+            format_data = self.format_data
+
+        if format_data == False:
+            return result
+
+        elif isinstance(result, list):
+            return list(Port(**port) for port in result)
+        return result
+
+    # Core.CancelTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def cancel_task(self, task_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Cancel a task.
+
+        Args:
+            task_id (str): _description_
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a GUID.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TaskId": task_id
+        }
+        result = await self._call_api(api="Core/CancelTask", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.DismissTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def dismiss_task(self, task_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Dismiss a task notification.
+
+        Args:
+            task_id (str): _description_
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a GUID.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "TaskId": task_id
+        }
+        result = await self._call_api(api="Core/DismissTask", parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.DismissAllTasks:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def dismiss_all_tasks(self, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Dismiss all task notifications.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a GUID.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/DismissAllTasks", format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.GetUserInfo:({'Description': 'Provides information about a given in-application user (as opposed to AMP system users)', 'Returns': '', 'Parameters': [{'Name': 'UID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'SimpleUser', 'IsComplexType': True})
+    async def get_user_info(self, uid: str, format_data: Union[bool, None] = None) -> dict:
+        """
+        Provides information about a given in-application user (as opposed to AMP system users).
+
+        Args:
+            uid (str): _description_
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            dict: On success returns a dict.
+        """
+
+        await self._connect()
+        parameters = {
+            "UID": uid
+        }
+        result = await self._call_api(api="Core/GetUserInfo", parameters=parameters, format_data=format_data)
+        return result
+
+    # Core.UpdateApplication:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def update_application(self, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Update the Instance application.
+
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a GUID.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/UpdateApplication", format_data=format_data, format=ActionResult)
+        return result
+
+    # Core.AcknowledgeAMPUpdate:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def acknowledge_amp_update(self) -> None:
+        """
+        Approves an AMP update.
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        await self._call_api(api="Core/AcknowledgeAMPUpdate")
+        return
+
+    # Core.GetModuleInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_module_info(self, format_data: Union[bool, None] = None) -> Module:
+        """
+        Returns the module information.
+
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Module: On success returns a Module dataclass.
+                See `types.py -> Module`
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetModuleInfo", format_data=format_data, format=Module)
+        return result
+
+    # Core.GetUserActionsSpec:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False})
+    async def get_user_action_spec(self, format_data: Union[bool, None] = None) -> dict[str, Any]:
+        """
+        Get a specification of the user actions.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            dict[str, Any]: On success returns a dict.\n
+                - {'ADSModule': {},'CommonCorePlugin': {},'Core': {},'EmailSenderPlugin': {},'FileManagerPlugin': {},'LocalFileBackupPlugin': {}}
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetUserActionsSpec", format_data=format_data)
+        return result
+
+    # Core.GetRemoteLoginToken:({'Parameters': [{'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'IsTemporary', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'String', 'IsComplexType': False})
+    async def get_remote_login_token(self, description: Union[str, None] = None, is_temporary: Union[bool, None] = None, format_data: Union[bool, None] = None) -> str:
+        """
+        Get the remote login token.
+
+        Args:
+            description (Union[str, None], optional): Description. Defaults to None.
+            is_temporary (Union[bool, None], optional): Is temporary. Defaults to None.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            str: On success returns a str.
+                See `types.py -> str`
+        """
+
+        await self._connect()
+        parameters = {
+            "Description": description,
+            "IsTemporary": is_temporary
+        }
+        result = await self._call_api(api="Core/GetRemoteLoginToken", parameters=parameters, format_data=format_data)
+        return result
+
+    # Core.UpdateAMPInstance:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def update_amp_instance(self) -> None:
+        """
+        update_amp_instance 
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        await self._call_api(api="Core/UpdateAMPInstance")
+        return
+
+    # Core.RestartAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def restart_amp(self) -> None:
+        """
+        restart_amp 
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        await self._call_api(api="Core/RestartAMP")
+        return
+
+    # Core.UpgradeAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def upgrade_amp(self) -> None:
+        """
+        upgrade_amp 
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        await self._call_api(api="Core/UpgradeAMP")
+        return
+
+    # Core.GetDiagnosticsInfo:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False})
+    async def get_diagnostics_info(self, format_data: Union[bool, None] = None) -> Diagnostics:
+        """
+        Get's the system diagnostics information.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Diagnostics: On success returns a dictionary.\n
+
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetDiagnosticsInfo", format_data=format_data, format=Diagnostics, _use_from_dict=False, _auto_unpack=False)
+        return result
+
+    # Core.GetWebserverMetrics:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False})
+    async def get_webserver_metrics(self, format_data: Union[bool, None] = None) -> Any:
+        """
+        Gets the webserver metrics.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Any: UNK data returned by the API.
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/GetWebserverMetrics", format_data=format_data)
+        return result
+
+    # Core.CreateTestTask:({'Description': 'DEV: Creates a non-ending task with 50% progress for testing purposes', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def create_test_task(self) -> None:
+        """
+        **DEV**: Creates a non-ending task with 50% progress for testing purposes
+
+
+        Returns:
+            None: ""
+        """
+
+        await self._connect()
+        await self._call_api(api="Core/CreateTestTask")
+        return
+
+    # Core.AsyncTest:({'Description': 'DEV: Async test method', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False})
+    async def async_test(self) -> str:
+        """
+        **DEV**: Async test method
+
+
+        Returns:
+            str: Returns a string.
+        """
+
+        await self._connect()
+        result = await self._call_api(api="Core/AsyncTest")
+        return result
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/filebackup.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/filebackup.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-from __future__ import annotations
-
-from typing import Union
-
-from .base import Base
-from .types import *
-
-__all__ = ("LocalFileBackupPlugin",)
-
-
-class LocalFileBackupPlugin(Base):
-    """
-    Contains the base functions for any `/API/LocalFileBackupPlugin/` AMP API endpoints.
-
-    """
-    # LocalFileBackupPlugin.TakeBackup:({'Parameters': [{'Name': 'Title', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def take_backup(self, title: str, description: str, sticky: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Takes a backup of the AMP Server/Instance.
-
-        Args:
-            title (str): Title of the backup; aka `Name`
-            description (str): Brief description of why or what the backup is for.
-            sticky (bool, optional): Sticky backups won't be deleted to make room for automatic backups. Defaults to `False`.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: Results from the API call. 
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            "Title": title,
-            "Description": description,
-            "Sticky": sticky
-        }
-        result = await self._call_api(api='LocalFileBackupPlugin/TakeBackup', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # LocalFileBackupPlugin.UploadToS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def upload_to_s3(self, backup_id: str, format_data: Union[bool, None] = None) -> RunningTask:
-        """
-        Upload a backup to S3.
-
-        Args:
-            backup_id (str): The backup ID to upload.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RunningTask: Returns a RunningTask dataclass.
-                See `types.py -> RunningTask` 
-        """
-        await self._connect()
-        parameters = {
-            "BackupId": backup_id
-        }
-        result = await self._call_api(api='LocalFileBackupPlugin/UploadToS3', parameters=parameters, format_data=format_data, format=RunningTask)
-        return result
-
-    # LocalFileBackupPlugin.DownloadFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def download_from_s3(self, backup_id: str, format_data: Union[bool, None] = None) -> RunningTask:
-        """
-        Download a backup from S3.
-
-
-        Args:
-            backup_id (str): The backup ID to download.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RunningTask: Returns a RunningTask dataclass.
-                See `types.py -> RunningTask`
-        """
-        await self._connect()
-        parameters = {
-            "BackupId": backup_id
-        }
-        result = await self._call_api(api='LocalFileBackupPlugin/DownloadFromS3', parameters=parameters, format_data=format_data, format=RunningTask)
-        return result
-
-    # LocalFileBackupPlugin.DeleteFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def delete_from_s3(self, backup_id: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Delete a backup from S3.
-
-        Args:
-            backup_id (str): The backup ID to delete.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns a ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "BackupId": backup_id
-        }
-        result = await self._call_api(api='LocalFileBackupPlugin/DeleteFromS3', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # LocalFileBackupPlugin.GetBackups:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_backups(self, format_data: Union[bool, None] = None) -> list[Backup]:
-        """
-        Get a list of Backups.
-
-        Returns:
-            list[Backup]: List of backups.
-                See `types.py -> Backup`
-        """
-        await self._connect()
-        result = await self._call_api(api='LocalFileBackupPlugin/GetBackups', format_data=format_data, format=Backup, _use_from_dict=False)
-        return result
-
-    # LocalFileBackupPlugin.RestoreBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'DeleteExistingData', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def restore_backup(self, backup_id: str, delete_existing_data: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Restore a backup.
-
-        Args:
-            backup_id (str): The backup ID to restore.
-            delete_existing_data (bool, optional): Delete the backup after restoring. Defaults to False.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult | str | dict[str, Any] | list | bool | int | None: On success returns a ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "BackupId": backup_id,
-            "DeleteExistingData": delete_existing_data
-        }
-        result = await self._call_api(api='LocalFileBackupPlugin/RestoreBackup', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # LocalFileBackupPlugin.DeleteLocalBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def delete_local_backup(self, backup_id: str) -> None:
-        """
-        Delete a local backup.
-
-        Args:
-            backup_id (str): The backup ID to delete.
-
-        Returns:
-            None
-        """
-        await self._connect()
-        parameters = {
-            "BackupId": backup_id
-        }
-        await self._call_api(api='LocalFileBackupPlugin/DeleteLocalBackup', parameters=parameters)
-        return
-
-    # LocalFileBackupPlugin.SetBackupSticky:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def set_backup_sticky(self, backup_id: str, sticky: bool = False) -> None:
-        """
-        Set a backup as sticky.
-
-        Args:
-            backup_id (str): The backup ID to set as sticky.
-            sticky (bool, optional): Set the backup as sticky. Defaults to False.
-
-        Returns:
-            None
-        """
-        await self._connect()
-        parameters = {
-            "BackupId": backup_id,
-            "Sticky": sticky
-        }
-        await self._call_api(api='LocalFileBackupPlugin/SetBackupSticky', parameters=parameters)
-        return
+from __future__ import annotations
+
+from typing import Union
+
+from .base import Base
+from .types import *
+
+__all__ = ("LocalFileBackupPlugin",)
+
+
+class LocalFileBackupPlugin(Base):
+    """
+    Contains the base functions for any `/API/LocalFileBackupPlugin/` AMP API endpoints.
+
+    """
+    # LocalFileBackupPlugin.TakeBackup:({'Parameters': [{'Name': 'Title', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def take_backup(self, title: str, description: str, sticky: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Takes a backup of the AMP Server/Instance.
+
+        Args:
+            title (str): Title of the backup; aka `Name`
+            description (str): Brief description of why or what the backup is for.
+            sticky (bool, optional): Sticky backups won't be deleted to make room for automatic backups. Defaults to `False`.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: Results from the API call. 
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            "Title": title,
+            "Description": description,
+            "Sticky": sticky
+        }
+        result = await self._call_api(api='LocalFileBackupPlugin/TakeBackup', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # LocalFileBackupPlugin.UploadToS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def upload_to_s3(self, backup_id: str, format_data: Union[bool, None] = None) -> RunningTask:
+        """
+        Upload a backup to S3.
+
+        Args:
+            backup_id (str): The backup ID to upload.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RunningTask: Returns a RunningTask dataclass.
+                See `types.py -> RunningTask` 
+        """
+        await self._connect()
+        parameters = {
+            "BackupId": backup_id
+        }
+        result = await self._call_api(api='LocalFileBackupPlugin/UploadToS3', parameters=parameters, format_data=format_data, format=RunningTask)
+        return result
+
+    # LocalFileBackupPlugin.DownloadFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def download_from_s3(self, backup_id: str, format_data: Union[bool, None] = None) -> RunningTask:
+        """
+        Download a backup from S3.
+
+
+        Args:
+            backup_id (str): The backup ID to download.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RunningTask: Returns a RunningTask dataclass.
+                See `types.py -> RunningTask`
+        """
+        await self._connect()
+        parameters = {
+            "BackupId": backup_id
+        }
+        result = await self._call_api(api='LocalFileBackupPlugin/DownloadFromS3', parameters=parameters, format_data=format_data, format=RunningTask)
+        return result
+
+    # LocalFileBackupPlugin.DeleteFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def delete_from_s3(self, backup_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Delete a backup from S3.
+
+        Args:
+            backup_id (str): The backup ID to delete.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns a ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "BackupId": backup_id
+        }
+        result = await self._call_api(api='LocalFileBackupPlugin/DeleteFromS3', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # LocalFileBackupPlugin.GetBackups:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_backups(self, format_data: Union[bool, None] = None) -> list[Backup]:
+        """
+        Get a list of Backups.
+
+        Returns:
+            list[Backup]: List of backups.
+                See `types.py -> Backup`
+        """
+        await self._connect()
+        result = await self._call_api(api='LocalFileBackupPlugin/GetBackups', format_data=format_data, format=Backup, _use_from_dict=False)
+        return result
+
+    # LocalFileBackupPlugin.RestoreBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'DeleteExistingData', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def restore_backup(self, backup_id: str, delete_existing_data: bool = False, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Restore a backup.
+
+        Args:
+            backup_id (str): The backup ID to restore.
+            delete_existing_data (bool, optional): Delete the backup after restoring. Defaults to False.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult | str | dict[str, Any] | list | bool | int | None: On success returns a ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "BackupId": backup_id,
+            "DeleteExistingData": delete_existing_data
+        }
+        result = await self._call_api(api='LocalFileBackupPlugin/RestoreBackup', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # LocalFileBackupPlugin.DeleteLocalBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def delete_local_backup(self, backup_id: str) -> None:
+        """
+        Delete a local backup.
+
+        Args:
+            backup_id (str): The backup ID to delete.
+
+        Returns:
+            None
+        """
+        await self._connect()
+        parameters = {
+            "BackupId": backup_id
+        }
+        await self._call_api(api='LocalFileBackupPlugin/DeleteLocalBackup', parameters=parameters)
+        return
+
+    # LocalFileBackupPlugin.SetBackupSticky:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def set_backup_sticky(self, backup_id: str, sticky: bool = False) -> None:
+        """
+        Set a backup as sticky.
+
+        Args:
+            backup_id (str): The backup ID to set as sticky.
+            sticky (bool, optional): Set the backup as sticky. Defaults to False.
+
+        Returns:
+            None
+        """
+        await self._connect()
+        parameters = {
+            "BackupId": backup_id,
+            "Sticky": sticky
+        }
+        await self._call_api(api='LocalFileBackupPlugin/SetBackupSticky', parameters=parameters)
+        return
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/filemanager.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/filemanager.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,403 +1,403 @@
-from __future__ import annotations
-
-from typing import Union
-
-from .base import FORMAT_DATA, Base
-from .types import *
-
-__all__ = ("FileManagerPlugin",)
-
-
-class FileManagerPlugin(Base):
-    """
-    Contains the base functions for any `/API/FileManagerPlugin/` AMP API endpoints.
-
-    """
-
-    # FileManagerPlugin.CopyFile:({'Parameters': [{'Name': 'Origin', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def copy_file(self, origin: str, target_directory: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Moves a file from the origin directory to the target_directory. The path is relative to the Server/Instance home directory.\n
-            Example `await Instance.copyFile("eula.txt", "test")` would move `/eula.txt` to `/test/eula.txt`
-
-        Args:
-            origin (str): Directory starts from the Instance home path (`/`) along with the file name and the extension. (eg. "eula.txt")
-                -> (File Manager `/` directory) eg `.ampdata/instance/VM_Minecraft/Minecraft/` *this is the home directory*
-            target_directory (str): Similar to source; do not include the file name. (eg. "test")
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'Origin': origin,
-            'TargetDirectory': target_directory
-        }
-        result = await self._call_api(api='FileManagerPlugin/CopyFile', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.RenameFile:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewFilename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def rename_file(self, file_name: str, new_file_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Changes the name of a file. \n
-            Path's are absolute and relative to the Instances home directory. Do not include the (`/`)
-
-        Args:
-            file_name (str): The path to the file and the file name included. (eg. "test/myfile.txt")
-            new_file_name (str): The file name to be changed; no path needed. (eg. "renamed_myfile.txt")
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-            See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'Filename': file_name,
-            'NewFilename': new_file_name
-        }
-        result = await self._call_api(api='FileManagerPlugin/RenameFile', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.RenameDirectory:({'Description': 'Renames a directory', 'Returns': '', 'Parameters': [{'Name': 'oldDirectory', 'TypeName': 'String', 'Description': 'The full path to the old directory', 'Optional': False}, {'Name': 'NewDirectoryName', 'TypeName': 'String', 'Description': 'The name component of the new directory (not the full path)', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def rename_directory(self, old_directory: str, new_directory_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Rename a directory.\n
-            Path's are absolute and relative to the Instances home directory. Do not include the (`/`)
-
-        Args:
-            old_directory (str): The full path to the old directory.
-            new_directory_name (str): The name component of the new directory (not the full path).
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: Results from the API call.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'oldDirectory': old_directory,
-            'newDirectoryName': new_directory_name
-        }
-        result = await self._call_api(api='FileManagerPlugin/RenameDirectory', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.GetDirectoryListing:({'Parameters': [{'Name': 'Dir', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def get_directory_listing(self, directory: str = "", format_data: Union[bool, None] = None) -> list[Directory]:
-        """
-        Returns a dictionary of the directory's properties and the files contained in the directory and their properties.
-
-        Args:
-            directory (str): Relative to the Server root directory . eg `Minecraft/` - If a file has a similar name it may return the file instead of the directory.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[Directory]: Returns a list of Directory dataclasses.
-                See `types.py -> Directory`
-        """
-
-        await self._connect()
-        parameters = {
-            'Dir': directory
-        }
-        result = await self._call_api(api='FileManagerPlugin/GetDirectoryListing', parameters=parameters, format_data=format_data, format=Directory, _use_from_dict=False)
-        return result
-
-    # FileManagerPlugin.GetFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Position', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'Length', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def get_file_chunk(self, file_name: str, position: int, length: int, format_data: Union[bool, None] = None) -> FileChunk:
-        """
-        Returns a specific section of Base64Data from a file.
-
-        Args:
-            name (str): File to open and read from.
-            position (int): Start position to read from.
-            length (int): How far to read from the start position.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            FileChunk: Returns a FileChunk dataclass.
-                See `types.py -> FileChunk`
-        """
-
-        await self._connect()
-        parameters = {
-            'Filename': file_name,
-            'Position': position,
-            'Length': length
-        }
-        result = await self._call_api(api='FileManagerPlugin/GetFileChunk', parameters=parameters, format_data=format_data, format=FileChunk)
-        return result
-
-    # FileManagerPlugin.WriteFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'FinalChunk', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def write_file_chunk(self, file_name: str, data: str, offset: int, final_chunk: bool, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Write data to a file with an offset.
-
-        Args:
-            file_name (str): File name to write the data to; relative to the Server/Instance root. Supports pathing. eg `home/config`
-            data (str): Binary data to be written.
-            offset (int): Data offset from start of file.
-            final_chunk (bool): Appends the data to the end of the file.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: Results from the API call.
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'Filename': file_name,
-            'Data': data,
-            'Offset': offset,
-            "FinalChunk": final_chunk
-        }
-        result = await self._call_api(api='FileManagerPlugin/WriteFileChunk', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.TrashDirectory:({'Description': 'Moves a directory to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'DirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def trash_directory(self, directory_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Moves a directory to the trash, files must be trashed before they can be `emptied`.\n
-            See `emptyTrash()`.
-
-        Args:
-            directory_name (str): Directory name; relative to the Server/Instance root. Supports pathing. eg `home/config`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: Results from the API call. 
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'DirectoryName': directory_name
-        }
-        result = await self._call_api(api='FileManagerPlugin/TrashDirectory', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.TrashFile:({'Description': 'Moves a file to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def trash_file(self, file_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Moves a file to the trash, files must be trashed before they can be `emptied`. \n
-            See `emptyTrash()`.
-
-        Args:
-            file_name (str): File name; relative to the Server/Instance root. Supports pathing. eg `home/config`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: Results from the API call. 
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'Filename': file_name
-        }
-        result = await self._call_api(api='FileManagerPlugin/TrashFile', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.EmptyTrash:({'Description': 'Empties a trash bin', 'Returns': '', 'Parameters': [{'Name': 'TrashDirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def empty_trash(self, trash_directory_name: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Empties a trash bin for the AMP Server/Instance.
-
-        Args:
-            trash_directory_name (str): Path to the directory; relative to the Server/Instance root. eg `home/config`. \n
-                - Typically the directory is called `Trashed Files`, it is case sensitive and located in the Server/Instance root directory.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: Results from the API call. 
-                See `types.py -> ActionResult`
-        """
-
-        await self._connect()
-        parameters = {
-            'TrashDirectoryName': trash_directory_name
-        }
-        result = await self._call_api(api='FileManagerPlugin/EmptyTrash', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.CalculateFileMD5Sum:({'Parameters': [{'Name': 'FilePath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True})
-    async def calculate_file_md5_sum(self, file_path: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Calculate the MD5 sum of a file.
-
-        Args:
-            file_path (str): Path to the file; relative to the Server/Instance root. eg `home/config`.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "FilePath": file_path
-        }
-        result = await self._call_api(api='FileManagerPlugin/CalculateFileMD5Sum', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.ChangeExclusion:({'Parameters': [{'Name': 'ModifyPath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsDirectory', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Exclude', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def change_exclusion(self, modify_path: str, as_directory: bool, exclude: bool, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Change a file or directory to be excluded from backups.
-
-        Args:
-            modify_path (str): Path to the file; relative to the Server/Instance root. eg `home/config`
-            as_directory (bool): If modify_path is a directory
-            exclude (bool): If modify_path should be excluded
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "ModifyPath": modify_path,
-            "AsDirectory": as_directory,
-            "Exclude": exclude
-        }
-        result = await self._call_api(api='FileManagerPlugin/ChangeExclusion', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.CreateArchive:({'Parameters': [{'Name': 'PathToArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def create_archive(self, path_to_archive: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Create an archive file.
-
-        Args:
-            path_to_archive (str): Path to the file; relative to the Server/Instance root. eg `home/config`
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "PathToArchive": path_to_archive
-        }
-        result = await self._call_api(api='FileManagerPlugin/CreateArchive', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.ExtractArchive:({'Parameters': [{'Name': 'ArchivePath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'DestinationPath', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def extract_archive(self, archive_path: str, destination_path: str | None = None, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Extract an archive file.
-
-        Args:
-            archive_path (str): Path to the archive to extract; relative to the Server/Instance root. eg `home/config`.
-            destination_path (str | None, optional): Path to extract the archive to; relative to the Server/Instance root. eg `home/config`. Defaults to None.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "ArchivePath": archive_path
-        }
-
-        if destination_path != None:
-            parameters["DestinationPath"] = destination_path
-
-        result = await self._call_api(api='FileManagerPlugin/ExtractArchive', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.AppendFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Delete', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def append_file_chunk(self, file_name: str, data: str, delete: bool) -> None:
-        """
-        Append data to a file.
-
-        Args:
-            file_name (str): Path to the file; relative to the Server/Instance root. eg `home/config`.
-            data (str): Binary data to be written.
-            delete (bool): UNK #TODO - What does this do?
-        """
-        await self._connect()
-        parameters = {
-            "Filename": file_name,
-            "Data": data,
-            "Delete": delete
-        }
-        await self._call_api(api='FileManagerPlugin/AppendFileChunk', parameters=parameters)
-        return
-
-    # FileManagerPlugin.ReadFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'ChunkSize', 'TypeName': 'Int64', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True})
-    async def read_file_chunk(self, file_name: str, offset: int, chunk_size: int | None = None, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Read a chunk of data from a file.
-
-        Args:
-            file_name (str): Path to the file; relative to the Server/Instance root. eg `home/config`.
-            offset (int): Data offset from start of file.
-            chunk_size (int | None, optional): Data chunk size. Defaults to None.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "Filename": file_name,
-            "Offset": offset
-        }
-        if chunk_size != None:
-            parameters["ChunkSize"] = chunk_size
-
-        result = await self._call_api(api='FileManagerPlugin/ReadFileChunk', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.DownloadFileFromURL:({'Parameters': [{'Name': 'Source', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def download_file_from_url(self, source: str, target_directory: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Download a file from a URL.
-
-        Args:
-            source (str): URL to file.
-            target_directory (str): Path to the file; relative to the Server/Instance root. eg `home/config`.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "Source": source,
-            "TargetDirectory": target_directory
-        }
-        result = await self._call_api(api='FileManagerPlugin/DownloadFileFromURL', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # FileManagerPlugin.CreateDirectory:({'Description': 'Creates a new directory. The parent directory must already exist.', 'Returns': '', 'Parameters': [{'Name': 'NewPath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def create_directory(self, new_path: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Creates a new directory. The parent directory must already exist.
-
-        Args:
-            new_path (str): Path to the directory; relative to the Server/Instance root. eg `home/config`.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-        await self._connect()
-        parameters = {
-            "NewPath": new_path
-        }
-        result = await self._call_api(api='FileManagerPlugin/CreateDirectory', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
+from __future__ import annotations
+
+from typing import Union
+
+from .base import FORMAT_DATA, Base
+from .types import *
+
+__all__ = ("FileManagerPlugin",)
+
+
+class FileManagerPlugin(Base):
+    """
+    Contains the base functions for any `/API/FileManagerPlugin/` AMP API endpoints.
+
+    """
+
+    # FileManagerPlugin.CopyFile:({'Parameters': [{'Name': 'Origin', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def copy_file(self, origin: str, target_directory: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Moves a file from the origin directory to the target_directory. The path is relative to the Server/Instance home directory.\n
+            Example `await Instance.copyFile("eula.txt", "test")` would move `/eula.txt` to `/test/eula.txt`
+
+        Args:
+            origin (str): Directory starts from the Instance home path (`/`) along with the file name and the extension. (eg. "eula.txt")
+                -> (File Manager `/` directory) eg `.ampdata/instance/VM_Minecraft/Minecraft/` *this is the home directory*
+            target_directory (str): Similar to source; do not include the file name. (eg. "test")
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'Origin': origin,
+            'TargetDirectory': target_directory
+        }
+        result = await self._call_api(api='FileManagerPlugin/CopyFile', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.RenameFile:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewFilename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def rename_file(self, file_name: str, new_file_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Changes the name of a file. \n
+            Path's are absolute and relative to the Instances home directory. Do not include the (`/`)
+
+        Args:
+            file_name (str): The path to the file and the file name included. (eg. "test/myfile.txt")
+            new_file_name (str): The file name to be changed; no path needed. (eg. "renamed_myfile.txt")
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+            See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'Filename': file_name,
+            'NewFilename': new_file_name
+        }
+        result = await self._call_api(api='FileManagerPlugin/RenameFile', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.RenameDirectory:({'Description': 'Renames a directory', 'Returns': '', 'Parameters': [{'Name': 'oldDirectory', 'TypeName': 'String', 'Description': 'The full path to the old directory', 'Optional': False}, {'Name': 'NewDirectoryName', 'TypeName': 'String', 'Description': 'The name component of the new directory (not the full path)', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def rename_directory(self, old_directory: str, new_directory_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Rename a directory.\n
+            Path's are absolute and relative to the Instances home directory. Do not include the (`/`)
+
+        Args:
+            old_directory (str): The full path to the old directory.
+            new_directory_name (str): The name component of the new directory (not the full path).
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: Results from the API call.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'oldDirectory': old_directory,
+            'newDirectoryName': new_directory_name
+        }
+        result = await self._call_api(api='FileManagerPlugin/RenameDirectory', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.GetDirectoryListing:({'Parameters': [{'Name': 'Dir', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def get_directory_listing(self, directory: str = "", format_data: Union[bool, None] = None) -> list[Directory]:
+        """
+        Returns a dictionary of the directory's properties and the files contained in the directory and their properties.
+
+        Args:
+            directory (str): Relative to the Server root directory . eg `Minecraft/` - If a file has a similar name it may return the file instead of the directory.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[Directory]: Returns a list of Directory dataclasses.
+                See `types.py -> Directory`
+        """
+
+        await self._connect()
+        parameters = {
+            'Dir': directory
+        }
+        result = await self._call_api(api='FileManagerPlugin/GetDirectoryListing', parameters=parameters, format_data=format_data, format=Directory, _use_from_dict=False)
+        return result
+
+    # FileManagerPlugin.GetFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Position', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'Length', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def get_file_chunk(self, file_name: str, position: int, length: int, format_data: Union[bool, None] = None) -> FileChunk:
+        """
+        Returns a specific section of Base64Data from a file.
+
+        Args:
+            name (str): File to open and read from.
+            position (int): Start position to read from.
+            length (int): How far to read from the start position.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            FileChunk: Returns a FileChunk dataclass.
+                See `types.py -> FileChunk`
+        """
+
+        await self._connect()
+        parameters = {
+            'Filename': file_name,
+            'Position': position,
+            'Length': length
+        }
+        result = await self._call_api(api='FileManagerPlugin/GetFileChunk', parameters=parameters, format_data=format_data, format=FileChunk)
+        return result
+
+    # FileManagerPlugin.WriteFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'FinalChunk', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def write_file_chunk(self, file_name: str, data: str, offset: int, final_chunk: bool, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Write data to a file with an offset.
+
+        Args:
+            file_name (str): File name to write the data to; relative to the Server/Instance root. Supports pathing. eg `home/config`
+            data (str): Binary data to be written.
+            offset (int): Data offset from start of file.
+            final_chunk (bool): Appends the data to the end of the file.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: Results from the API call.
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'Filename': file_name,
+            'Data': data,
+            'Offset': offset,
+            "FinalChunk": final_chunk
+        }
+        result = await self._call_api(api='FileManagerPlugin/WriteFileChunk', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.TrashDirectory:({'Description': 'Moves a directory to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'DirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def trash_directory(self, directory_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Moves a directory to the trash, files must be trashed before they can be `emptied`.\n
+            See `emptyTrash()`.
+
+        Args:
+            directory_name (str): Directory name; relative to the Server/Instance root. Supports pathing. eg `home/config`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: Results from the API call. 
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'DirectoryName': directory_name
+        }
+        result = await self._call_api(api='FileManagerPlugin/TrashDirectory', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.TrashFile:({'Description': 'Moves a file to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def trash_file(self, file_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Moves a file to the trash, files must be trashed before they can be `emptied`. \n
+            See `emptyTrash()`.
+
+        Args:
+            file_name (str): File name; relative to the Server/Instance root. Supports pathing. eg `home/config`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: Results from the API call. 
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'Filename': file_name
+        }
+        result = await self._call_api(api='FileManagerPlugin/TrashFile', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.EmptyTrash:({'Description': 'Empties a trash bin', 'Returns': '', 'Parameters': [{'Name': 'TrashDirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def empty_trash(self, trash_directory_name: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Empties a trash bin for the AMP Server/Instance.
+
+        Args:
+            trash_directory_name (str): Path to the directory; relative to the Server/Instance root. eg `home/config`. \n
+                - Typically the directory is called `Trashed Files`, it is case sensitive and located in the Server/Instance root directory.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: Results from the API call. 
+                See `types.py -> ActionResult`
+        """
+
+        await self._connect()
+        parameters = {
+            'TrashDirectoryName': trash_directory_name
+        }
+        result = await self._call_api(api='FileManagerPlugin/EmptyTrash', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.CalculateFileMD5Sum:({'Parameters': [{'Name': 'FilePath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True})
+    async def calculate_file_md5_sum(self, file_path: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Calculate the MD5 sum of a file.
+
+        Args:
+            file_path (str): Path to the file; relative to the Server/Instance root. eg `home/config`.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "FilePath": file_path
+        }
+        result = await self._call_api(api='FileManagerPlugin/CalculateFileMD5Sum', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.ChangeExclusion:({'Parameters': [{'Name': 'ModifyPath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsDirectory', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Exclude', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def change_exclusion(self, modify_path: str, as_directory: bool, exclude: bool, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Change a file or directory to be excluded from backups.
+
+        Args:
+            modify_path (str): Path to the file; relative to the Server/Instance root. eg `home/config`
+            as_directory (bool): If modify_path is a directory
+            exclude (bool): If modify_path should be excluded
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "ModifyPath": modify_path,
+            "AsDirectory": as_directory,
+            "Exclude": exclude
+        }
+        result = await self._call_api(api='FileManagerPlugin/ChangeExclusion', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.CreateArchive:({'Parameters': [{'Name': 'PathToArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def create_archive(self, path_to_archive: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Create an archive file.
+
+        Args:
+            path_to_archive (str): Path to the file; relative to the Server/Instance root. eg `home/config`
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "PathToArchive": path_to_archive
+        }
+        result = await self._call_api(api='FileManagerPlugin/CreateArchive', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.ExtractArchive:({'Parameters': [{'Name': 'ArchivePath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'DestinationPath', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def extract_archive(self, archive_path: str, destination_path: str | None = None, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Extract an archive file.
+
+        Args:
+            archive_path (str): Path to the archive to extract; relative to the Server/Instance root. eg `home/config`.
+            destination_path (str | None, optional): Path to extract the archive to; relative to the Server/Instance root. eg `home/config`. Defaults to None.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "ArchivePath": archive_path
+        }
+
+        if destination_path != None:
+            parameters["DestinationPath"] = destination_path
+
+        result = await self._call_api(api='FileManagerPlugin/ExtractArchive', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.AppendFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Delete', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def append_file_chunk(self, file_name: str, data: str, delete: bool) -> None:
+        """
+        Append data to a file.
+
+        Args:
+            file_name (str): Path to the file; relative to the Server/Instance root. eg `home/config`.
+            data (str): Binary data to be written.
+            delete (bool): UNK #TODO - What does this do?
+        """
+        await self._connect()
+        parameters = {
+            "Filename": file_name,
+            "Data": data,
+            "Delete": delete
+        }
+        await self._call_api(api='FileManagerPlugin/AppendFileChunk', parameters=parameters)
+        return
+
+    # FileManagerPlugin.ReadFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'ChunkSize', 'TypeName': 'Int64', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True})
+    async def read_file_chunk(self, file_name: str, offset: int, chunk_size: int | None = None, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Read a chunk of data from a file.
+
+        Args:
+            file_name (str): Path to the file; relative to the Server/Instance root. eg `home/config`.
+            offset (int): Data offset from start of file.
+            chunk_size (int | None, optional): Data chunk size. Defaults to None.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "Filename": file_name,
+            "Offset": offset
+        }
+        if chunk_size != None:
+            parameters["ChunkSize"] = chunk_size
+
+        result = await self._call_api(api='FileManagerPlugin/ReadFileChunk', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.DownloadFileFromURL:({'Parameters': [{'Name': 'Source', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def download_file_from_url(self, source: str, target_directory: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Download a file from a URL.
+
+        Args:
+            source (str): URL to file.
+            target_directory (str): Path to the file; relative to the Server/Instance root. eg `home/config`.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "Source": source,
+            "TargetDirectory": target_directory
+        }
+        result = await self._call_api(api='FileManagerPlugin/DownloadFileFromURL', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # FileManagerPlugin.CreateDirectory:({'Description': 'Creates a new directory. The parent directory must already exist.', 'Returns': '', 'Parameters': [{'Name': 'NewPath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def create_directory(self, new_path: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Creates a new directory. The parent directory must already exist.
+
+        Args:
+            new_path (str): Path to the directory; relative to the Server/Instance root. eg `home/config`.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+        await self._connect()
+        parameters = {
+            "NewPath": new_path
+        }
+        result = await self._call_api(api='FileManagerPlugin/CreateDirectory', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/minecraft.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/minecraft.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,515 +1,515 @@
-from __future__ import annotations
-
-from typing import Any, Union
-
-from dataclass_wizard import fromdict
-
-from .base import FORMAT_DATA, Base
-from .types import *
-
-__all__ = ("MinecraftModule",)
-
-
-class MinecraftModule(Base):
-    """
-    Contains the base functions for any `/API/MinecraftModule/` AMP API endpoints.
-
-    """
-
-    # MinecraftModule.BukGetCategories: ({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
-    async def mc_buk_get_categories(self) -> list[dict[str, Any]]:
-        """
-        Get Bukkit categories.
-
-        Returns:
-            list[dict[str, Any]]: Returns a list of dictionaries containing plugin categories.\n
-
-        ### CATEGORIES:
-        {'id': 2, 'name': 'Bungee - Spigot'}
-        {'id': 3, 'name': 'Bungee - Proxy'}
-        {'id': 4, 'name': 'Spigot'}
-        {'id': 5, 'name': 'Transportation'}
-        {'id': 6, 'name': 'Chat'}
-        {'id': 7, 'name': 'Tools and Utilities'}
-        {'id': 8, 'name': 'Misc'}
-        {'id': 9, 'name': 'Libraries / APIs'}
-        {'id': 10, 'name': 'Transportation'}
-        {'id': 11, 'name': 'Chat'}
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='MinecraftModule/BukGetCategories')
-        return result
-
-    # MinecraftModule.BukGetPopularPlugins: ({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
-    async def mc_buk_get_popular_plugins(self, format_data: Union[bool, None] = None) -> list[BukkitPlugin]:
-        """
-        Get Bukkit popular plugins.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[BukkitPlugin]: Returns a list of BukkitPlugin dataclasses.
-                See `types.py -> BukkitPlugin`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='MinecraftModule/BukGetPopularPlugins', format_data=format_data, format=BukkitPlugin)
-        return result
-
-    # MinecraftModule.BukGetPluginsForCategory: ({'Parameters': [{'Name': 'CategoryId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
-    async def mc_buk_get_plugins_for_category(self, category_id: str, page_number: int = 1, page_size: int = 10, format_data: Union[bool, None] = None) -> list[BukkitPlugin]:
-        """
-        Get Bukkit plugins from category.
-
-        Args:
-            category_id (str): Plugin category ID. See -> `mc_buk_get_categories()`
-            page_number (int): Page Number. Default: 1
-            page_size (int): Page Size. Default: 10
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-
-        Returns:
-            list[BukkitPlugin]: On success returns a list of BukkitPlugin dataclasses.
-                See `types.py -> BukkitPlugin`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "CategoryId": category_id,
-            "PageNumber": page_number,
-            "PageSize": page_size
-        }
-
-        result = await self._call_api(api='MinecraftModule/BukGetPluginsForCategory', parameters=parameters, format_data=format_data, format=BukkitPlugin)
-        return result
-
-    # MinecraftModule.BukGetPluginInfo: ({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
-    async def mc_buk_get_plugin_info(self, plugin_id: int, format_data: Union[bool, None] = None) -> Any:
-        """
-        Get Bukkit plugin info.
-
-
-        Args:
-            plugin_id (int): The plugin ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            Any: UNK data returned by the API.
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "PluginId": plugin_id
-        }
-        result = await self._call_api(api='MinecraftModule/BukGetPluginInfo', parameters=parameters, format_data=format_data)
-        return result
-
-    # MinecraftModule.BukGetInstalledPlugins: ({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
-    async def mc_buk_get_installed_plugins(self, format_data: Union[bool, None] = None) -> list[BukkitPlugin]:
-        """
-        Get Bukkit installed plugins.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)        
-
-        Returns:
-            list[BukkitPlugin]: On success returns a list of BukkitPlugin dataclasses.
-                See `types.py -> BukkitPlugin`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='MinecraftModule/BukGetInstalledPlugins', format_data=format_data, format=BukkitPlugin)
-        return result
-
-    # MinecraftModule.BukGetRemovePlugin: ({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def mc_buk_get_remove_plugin(self, plugin_id: int) -> None:
-        """
-        Remove Bukkit plugin.
-
-        Args:
-            plugin_id (int): The plugin ID.
-
-        Returns:
-            None: ""
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "PluginId": plugin_id
-        }
-        await self._call_api(api='MinecraftModule/BukGetRemovePlugin', parameters=parameters)
-        return
-
-    # MinecraftModule.BukGetInstallUpdatePlugin: ({'Parameters': [{'Name': 'pluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
-    async def mc_buk_get_install_update_plugin(self, plugin_id: int, format_data: Union[bool, None] = None) -> RunningTask:
-        """
-        Get update for Bukkit plugin.
-
-        Args:
-            plugin_id (int): The plugin ID.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            RunningTask: On success returns a RunningTask dataclass.
-                See `types.py -> RunningTask`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "pluginId": plugin_id
-        }
-        result = await self._call_api(api='MinecraftModule/BukGetInstallUpdatePlugin', parameters=parameters, format_data=format_data, format=RunningTask)
-        return result
-
-    # MinecraftModule.BukGetSearch: ({'Parameters': [{'Name': 'Query', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
-    async def mc_buk_get_search(self, query: str, page_number: int = 0, page_size: int = 10, format_data: Union[bool, None] = None) -> list[BukkitPlugin]:
-        """
-        Search for Bukkit plugins.
-
-        Args:
-            Query (str): Search string.
-            PageNumber (int): Page number. Defaults to 0.
-            PageSize (int): Page size. Defaults to 10.
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[BukkitPlugin]: On success returns a list of BukkitPlugin dataclasses.
-                See `types.py -> BukkitPlugin`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "Query": query,
-            "PageNumber": page_number,
-            "PageSize": page_size
-
-        }
-        result = await self._call_api(api='MinecraftModule/BukGetSearch', parameters=parameters, format_data=format_data, format=BukkitPlugin)
-        return result
-
-    # MinecraftModule.GetHeadByUUID: ({'Description': 'Get a skin as a base64 string', 'Returns': '', 'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'String', 'IsComplexType': False})
-    async def mc_get_head_by_uuid(self, id: str) -> str:
-        """
-        Get a skin as a base64 string.
-
-        Args:
-            id (str): Minecraft UUID.
-
-        Returns:
-            str: base64 string. eg. (data:image/gif;base64, data)
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "id": id
-        }
-        result = await self._call_api(api='MinecraftModule/GetHeadByUUID', parameters=parameters)
-        return result
-
-    # MinecraftModule.GetFailureReason: ({'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False})
-    async def mc_get_failure_reason(self) -> str:
-        """
-        Get the failure reason.
-
-        Returns:
-            str: On success returns a string representation of the failure reason.
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='MinecraftModule/GetFailureReason')
-        return result
-
-    # MinecraftModule.AcceptEULA: ({'Parameters': [], 'ReturnTypeName': 'Boolean', 'IsComplexType': False})
-    async def mc_accept_eula(self) -> bool:
-        """
-        Accept the EULA summary.
-
-        Returns:
-            bool: On success returns a Bool.
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='MinecraftModule/AcceptEULA')
-        return result
-
-    # MinecraftModule.BanUserByID: ({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def mc_ban_user_by_id(self, id: str) -> None:
-        """
-        Ban the specified Minecraft UUID.
-
-        Args:
-            id (str): Minecraft UUID.
-
-        Returns:
-            None: ""
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "ID": id
-        }
-        await self._call_api(api='MinecraftModule/BanUserByID', parameters=parameters)
-        return
-
-    # MinecraftModule.KickUserByID: ({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def mc_kick_user_by_id(self, id: str) -> None:
-        """
-        Kick the specified User ID.
-
-        Args:
-            id (str): Minecraft UUID.
-
-        Returns:
-            None
-
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "ID": id
-        }
-        await self._call_api(api='MinecraftModule/KickUserByID', parameters=parameters)
-        return
-
-    # MinecraftModule.ClearInventoryByID: ({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def mc_clear_inventory_by_id(self, id: str) -> None:
-        """
-        Clear a players inventory. 
-
-        Args:
-            id (str): Minecraft UUID.
-
-        Returns:
-            None
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "ID": id
-        }
-        await self._call_api(api='MinecraftModule/ClearInventoryByID', parameters=parameters)
-        return
-
-    # MinecraftModule.KillByID: ({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def mc_kill_by_id(self, id: str) -> None:
-        """
-        Kill the Minecraft player.
-
-        Args:
-            id (str): Minecraft UUID.
-
-        Returns:
-            None
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "ID": id
-        }
-        await self._call_api(api='MinecraftModule/KillByID', parameters=parameters)
-        return
-
-    # MinecraftModule.SmiteByID: ({'Description': 'Strike a player with lightning', 'Returns': '', 'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def mc_smite_by_id(self, id: str) -> None:
-        """
-        Strike a player with lightning
-
-        Args:
-            id (str): Minecraft UUID.
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "ID": id
-        }
-        await self._call_api(api='MinecraftModule/SmiteByID', parameters=parameters)
-        return
-
-    # MinecraftModule.GetOPWhitelist: ({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
-    async def mc_get_op_whitelist(self, format_data: Union[bool, None] = None) -> OPWhitelist:
-        """
-        Get the OP whitelist.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            OPWhitelist: On success returns an OPWhitelist dataclass.
-                See `types.py -> OPWhitelist`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='MinecraftModule/GetOPWhitelist', format_data=format_data, format=OPWhitelist)
-        return result
-
-    # MinecraftModule.GetWhitelist: ({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def mc_get_whitelist(self, format_data: Union[bool, None] = None) -> list[MCUser]:
-        """
-        Get the whitelist.
-
-        Args:
-            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
-
-        Returns:
-            list[Whitelist]: Returns a list of strings containing Minecraft UUIDs.
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='MinecraftModule/GetWhitelist', format_data=format_data, format=MCUser)
-        return result
-
-    # MinecraftModule.LoadOPList: ({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
-    async def mc_load_op_list(self, format_data: Union[bool, None] = None) -> list[OPList]:
-        """
-        Get the OP list.
-
-        Returns:
-            list[OPList]: On success returns a list of OPList dataclasses.
-                See `types.py -> OPList`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        result = await self._call_api(api='MinecraftModule/LoadOPList', format_data=format_data, format=OPList)
-        return result
-
-    # MinecraftModule.AddOPEntry: ({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def mc_add_op_entry(self, user_or_uuid: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Add an entry to the OP list.
-
-        Args:
-            user_or_uuid (str): Minecraft UUID or Username.
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "UserOrUUID": user_or_uuid
-        }
-
-        result = await self._call_api(api='MinecraftModule/AddOPEntry', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # MinecraftModule.RemoveOPEntry: ({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def mc_remove_op_entry(self, user_or_uuid: str) -> None:
-        """
-        Remove an entry from the OP list.
-
-        Args:
-            user_or_uuid (str): Minecraft UUID or Username.
-        """
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "UserOrUUID": user_or_uuid
-        }
-        await self._call_api(api='MinecraftModule/RemoveOPEntry', parameters=parameters)
-        return
-
-    # MinecraftModule.AddToWhitelist: ({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def mc_add_to_whitelist(self, user_or_uuid: str, format_data: Union[bool, None] = None) -> ActionResult:
-        """
-        Add a user to the whitelist.
-
-        Args:
-            user_or_uuid (str): Minecraft UUID or Username.
-
-        Returns:
-            ActionResult: On success returns an ActionResult dataclass.
-                See `types.py -> ActionResult`
-        """
-
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "UserOrUUID": user_or_uuid
-        }
-        result = await self._call_api(api='MinecraftModule/AddToWhitelist', parameters=parameters, format_data=format_data, format=ActionResult)
-        return result
-
-    # MinecraftModule.RemoveWhitelistEntry: ({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
-    async def mc_remove_whitelist_entry(self, user_or_uuid: str) -> None:
-        """
-        Remove a user from the whitelist.
-
-        Args:
-            user_or_uuid (str): Minecraft UUID or Username.
-        """
-        if self.Module != "Minecraft":
-            raise RuntimeError(self.MINECRAFT_ONLY)
-
-        await self._connect()
-        parameters = {
-            "UserOrUUID": user_or_uuid
-        }
-        await self._call_api(api='MinecraftModule/RemoveWhitelistEntry', parameters=parameters)
-        return
+from __future__ import annotations
+
+from typing import Any, Union
+
+from dataclass_wizard import fromdict
+
+from .base import FORMAT_DATA, Base
+from .types import *
+
+__all__ = ("MinecraftModule",)
+
+
+class MinecraftModule(Base):
+    """
+    Contains the base functions for any `/API/MinecraftModule/` AMP API endpoints.
+
+    """
+
+    # MinecraftModule.BukGetCategories: ({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
+    async def mc_buk_get_categories(self) -> list[dict[str, Any]]:
+        """
+        Get Bukkit categories.
+
+        Returns:
+            list[dict[str, Any]]: Returns a list of dictionaries containing plugin categories.\n
+
+        ### CATEGORIES:
+        {'id': 2, 'name': 'Bungee - Spigot'}
+        {'id': 3, 'name': 'Bungee - Proxy'}
+        {'id': 4, 'name': 'Spigot'}
+        {'id': 5, 'name': 'Transportation'}
+        {'id': 6, 'name': 'Chat'}
+        {'id': 7, 'name': 'Tools and Utilities'}
+        {'id': 8, 'name': 'Misc'}
+        {'id': 9, 'name': 'Libraries / APIs'}
+        {'id': 10, 'name': 'Transportation'}
+        {'id': 11, 'name': 'Chat'}
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='MinecraftModule/BukGetCategories')
+        return result
+
+    # MinecraftModule.BukGetPopularPlugins: ({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
+    async def mc_buk_get_popular_plugins(self, format_data: Union[bool, None] = None) -> list[BukkitPlugin]:
+        """
+        Get Bukkit popular plugins.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[BukkitPlugin]: Returns a list of BukkitPlugin dataclasses.
+                See `types.py -> BukkitPlugin`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='MinecraftModule/BukGetPopularPlugins', format_data=format_data, format=BukkitPlugin)
+        return result
+
+    # MinecraftModule.BukGetPluginsForCategory: ({'Parameters': [{'Name': 'CategoryId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
+    async def mc_buk_get_plugins_for_category(self, category_id: str, page_number: int = 1, page_size: int = 10, format_data: Union[bool, None] = None) -> list[BukkitPlugin]:
+        """
+        Get Bukkit plugins from category.
+
+        Args:
+            category_id (str): Plugin category ID. See -> `mc_buk_get_categories()`
+            page_number (int): Page Number. Default: 1
+            page_size (int): Page Size. Default: 10
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+
+        Returns:
+            list[BukkitPlugin]: On success returns a list of BukkitPlugin dataclasses.
+                See `types.py -> BukkitPlugin`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "CategoryId": category_id,
+            "PageNumber": page_number,
+            "PageSize": page_size
+        }
+
+        result = await self._call_api(api='MinecraftModule/BukGetPluginsForCategory', parameters=parameters, format_data=format_data, format=BukkitPlugin)
+        return result
+
+    # MinecraftModule.BukGetPluginInfo: ({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
+    async def mc_buk_get_plugin_info(self, plugin_id: int, format_data: Union[bool, None] = None) -> Any:
+        """
+        Get Bukkit plugin info.
+
+
+        Args:
+            plugin_id (int): The plugin ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            Any: UNK data returned by the API.
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "PluginId": plugin_id
+        }
+        result = await self._call_api(api='MinecraftModule/BukGetPluginInfo', parameters=parameters, format_data=format_data)
+        return result
+
+    # MinecraftModule.BukGetInstalledPlugins: ({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
+    async def mc_buk_get_installed_plugins(self, format_data: Union[bool, None] = None) -> list[BukkitPlugin]:
+        """
+        Get Bukkit installed plugins.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)        
+
+        Returns:
+            list[BukkitPlugin]: On success returns a list of BukkitPlugin dataclasses.
+                See `types.py -> BukkitPlugin`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='MinecraftModule/BukGetInstalledPlugins', format_data=format_data, format=BukkitPlugin)
+        return result
+
+    # MinecraftModule.BukGetRemovePlugin: ({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def mc_buk_get_remove_plugin(self, plugin_id: int) -> None:
+        """
+        Remove Bukkit plugin.
+
+        Args:
+            plugin_id (int): The plugin ID.
+
+        Returns:
+            None: ""
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "PluginId": plugin_id
+        }
+        await self._call_api(api='MinecraftModule/BukGetRemovePlugin', parameters=parameters)
+        return
+
+    # MinecraftModule.BukGetInstallUpdatePlugin: ({'Parameters': [{'Name': 'pluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True})
+    async def mc_buk_get_install_update_plugin(self, plugin_id: int, format_data: Union[bool, None] = None) -> RunningTask:
+        """
+        Get update for Bukkit plugin.
+
+        Args:
+            plugin_id (int): The plugin ID.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            RunningTask: On success returns a RunningTask dataclass.
+                See `types.py -> RunningTask`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "pluginId": plugin_id
+        }
+        result = await self._call_api(api='MinecraftModule/BukGetInstallUpdatePlugin', parameters=parameters, format_data=format_data, format=RunningTask)
+        return result
+
+    # MinecraftModule.BukGetSearch: ({'Parameters': [{'Name': 'Query', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True})
+    async def mc_buk_get_search(self, query: str, page_number: int = 0, page_size: int = 10, format_data: Union[bool, None] = None) -> list[BukkitPlugin]:
+        """
+        Search for Bukkit plugins.
+
+        Args:
+            Query (str): Search string.
+            PageNumber (int): Page number. Defaults to 0.
+            PageSize (int): Page size. Defaults to 10.
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[BukkitPlugin]: On success returns a list of BukkitPlugin dataclasses.
+                See `types.py -> BukkitPlugin`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "Query": query,
+            "PageNumber": page_number,
+            "PageSize": page_size
+
+        }
+        result = await self._call_api(api='MinecraftModule/BukGetSearch', parameters=parameters, format_data=format_data, format=BukkitPlugin)
+        return result
+
+    # MinecraftModule.GetHeadByUUID: ({'Description': 'Get a skin as a base64 string', 'Returns': '', 'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'String', 'IsComplexType': False})
+    async def mc_get_head_by_uuid(self, id: str) -> str:
+        """
+        Get a skin as a base64 string.
+
+        Args:
+            id (str): Minecraft UUID.
+
+        Returns:
+            str: base64 string. eg. (data:image/gif;base64, data)
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "id": id
+        }
+        result = await self._call_api(api='MinecraftModule/GetHeadByUUID', parameters=parameters)
+        return result
+
+    # MinecraftModule.GetFailureReason: ({'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False})
+    async def mc_get_failure_reason(self) -> str:
+        """
+        Get the failure reason.
+
+        Returns:
+            str: On success returns a string representation of the failure reason.
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='MinecraftModule/GetFailureReason')
+        return result
+
+    # MinecraftModule.AcceptEULA: ({'Parameters': [], 'ReturnTypeName': 'Boolean', 'IsComplexType': False})
+    async def mc_accept_eula(self) -> bool:
+        """
+        Accept the EULA summary.
+
+        Returns:
+            bool: On success returns a Bool.
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='MinecraftModule/AcceptEULA')
+        return result
+
+    # MinecraftModule.BanUserByID: ({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def mc_ban_user_by_id(self, id: str) -> None:
+        """
+        Ban the specified Minecraft UUID.
+
+        Args:
+            id (str): Minecraft UUID.
+
+        Returns:
+            None: ""
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "ID": id
+        }
+        await self._call_api(api='MinecraftModule/BanUserByID', parameters=parameters)
+        return
+
+    # MinecraftModule.KickUserByID: ({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def mc_kick_user_by_id(self, id: str) -> None:
+        """
+        Kick the specified User ID.
+
+        Args:
+            id (str): Minecraft UUID.
+
+        Returns:
+            None
+
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "ID": id
+        }
+        await self._call_api(api='MinecraftModule/KickUserByID', parameters=parameters)
+        return
+
+    # MinecraftModule.ClearInventoryByID: ({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def mc_clear_inventory_by_id(self, id: str) -> None:
+        """
+        Clear a players inventory. 
+
+        Args:
+            id (str): Minecraft UUID.
+
+        Returns:
+            None
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "ID": id
+        }
+        await self._call_api(api='MinecraftModule/ClearInventoryByID', parameters=parameters)
+        return
+
+    # MinecraftModule.KillByID: ({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def mc_kill_by_id(self, id: str) -> None:
+        """
+        Kill the Minecraft player.
+
+        Args:
+            id (str): Minecraft UUID.
+
+        Returns:
+            None
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "ID": id
+        }
+        await self._call_api(api='MinecraftModule/KillByID', parameters=parameters)
+        return
+
+    # MinecraftModule.SmiteByID: ({'Description': 'Strike a player with lightning', 'Returns': '', 'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def mc_smite_by_id(self, id: str) -> None:
+        """
+        Strike a player with lightning
+
+        Args:
+            id (str): Minecraft UUID.
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "ID": id
+        }
+        await self._call_api(api='MinecraftModule/SmiteByID', parameters=parameters)
+        return
+
+    # MinecraftModule.GetOPWhitelist: ({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
+    async def mc_get_op_whitelist(self, format_data: Union[bool, None] = None) -> OPWhitelist:
+        """
+        Get the OP whitelist.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            OPWhitelist: On success returns an OPWhitelist dataclass.
+                See `types.py -> OPWhitelist`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='MinecraftModule/GetOPWhitelist', format_data=format_data, format=OPWhitelist)
+        return result
+
+    # MinecraftModule.GetWhitelist: ({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def mc_get_whitelist(self, format_data: Union[bool, None] = None) -> list[MCUser]:
+        """
+        Get the whitelist.
+
+        Args:
+            format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
+
+        Returns:
+            list[Whitelist]: Returns a list of strings containing Minecraft UUIDs.
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='MinecraftModule/GetWhitelist', format_data=format_data, format=MCUser)
+        return result
+
+    # MinecraftModule.LoadOPList: ({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True})
+    async def mc_load_op_list(self, format_data: Union[bool, None] = None) -> list[OPList]:
+        """
+        Get the OP list.
+
+        Returns:
+            list[OPList]: On success returns a list of OPList dataclasses.
+                See `types.py -> OPList`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        result = await self._call_api(api='MinecraftModule/LoadOPList', format_data=format_data, format=OPList)
+        return result
+
+    # MinecraftModule.AddOPEntry: ({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def mc_add_op_entry(self, user_or_uuid: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Add an entry to the OP list.
+
+        Args:
+            user_or_uuid (str): Minecraft UUID or Username.
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "UserOrUUID": user_or_uuid
+        }
+
+        result = await self._call_api(api='MinecraftModule/AddOPEntry', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # MinecraftModule.RemoveOPEntry: ({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def mc_remove_op_entry(self, user_or_uuid: str) -> None:
+        """
+        Remove an entry from the OP list.
+
+        Args:
+            user_or_uuid (str): Minecraft UUID or Username.
+        """
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "UserOrUUID": user_or_uuid
+        }
+        await self._call_api(api='MinecraftModule/RemoveOPEntry', parameters=parameters)
+        return
+
+    # MinecraftModule.AddToWhitelist: ({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+    async def mc_add_to_whitelist(self, user_or_uuid: str, format_data: Union[bool, None] = None) -> ActionResult:
+        """
+        Add a user to the whitelist.
+
+        Args:
+            user_or_uuid (str): Minecraft UUID or Username.
+
+        Returns:
+            ActionResult: On success returns an ActionResult dataclass.
+                See `types.py -> ActionResult`
+        """
+
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "UserOrUUID": user_or_uuid
+        }
+        result = await self._call_api(api='MinecraftModule/AddToWhitelist', parameters=parameters, format_data=format_data, format=ActionResult)
+        return result
+
+    # MinecraftModule.RemoveWhitelistEntry: ({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False})
+    async def mc_remove_whitelist_entry(self, user_or_uuid: str) -> None:
+        """
+        Remove a user from the whitelist.
+
+        Args:
+            user_or_uuid (str): Minecraft UUID or Username.
+        """
+        if self.Module != "Minecraft":
+            raise RuntimeError(self.MINECRAFT_ONLY)
+
+        await self._connect()
+        parameters = {
+            "UserOrUUID": user_or_uuid
+        }
+        await self._call_api(api='MinecraftModule/RemoveWhitelistEntry', parameters=parameters)
+        return
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/util.py` & `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/util.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-from __future__ import annotations
-
-from pathlib import Path
-from typing import Any
-
-from .core import Core
-
-
-class APIUtil():
-    """
-    AMP API util functions to parse specific API calls for specific Data.
-    """
-
-    async def get_node_spec(self, amp: Core) -> str | dict[str, Any] | list | bool | int | None:
-        """
-        Creates a `setting_nodes.txt` in the script directory with nodes from api `Core/GetSettingSpec`
-
-        Args:
-            amp (Core): API_Core class object signed in.
-
-        See -> `amp/util/setting_nodes.txt` 
-
-        """
-        res = await amp.get_settings_spec()
-        dir = Path(__file__).parent.joinpath("../docs/setting_nodes.md")
-        mode = "x"
-        if dir.exists():
-            mode = "w"
-        file = open(dir, mode)
-
-        if not isinstance(res, dict):
-            return res
-
-        for key in res:
-            for value in res[key]:
-                for entry in value:
-                    if entry.lower() == "node":
-                        file.write(f"{value[entry]} \n")
-        file.close()
-
-    async def get_permission_nodes(self, amp: Core) -> str | dict[str, Any] | list | bool | int | None:
-        """
-        Creates a `permission_nodes.txt` in the script directory with nodes from api `Core/GetPermissionsSpec`
-
-        Args:
-            amp (Core): API_Core class object signed in.
-
-        See -> `amp/util/permission_nodes.txt`  
-        """
-        res = await amp.get_permissions_spec()
-        if isinstance(res, list):
-            self.node_scrape(text=res)
-        else:
-            raise ValueError(f"Error - invalid data type returned. {type(res)}")
-
-    def node_scrape(self, text: list[dict], file=None) -> None:
-        """
-        Pulls the key "Nodes" from the list of dictionary results and dumps them to a txt file.
-
-        Args:
-            text (list): The list of dictionary's
-            file (_type_, optional): The file object to dump text to. Defaults to None. `**LEAVE NONE**`
-        """
-        dir = Path(__file__).parent.joinpath("../docs/permission_nodes.md")
-        mode = "x"
-        if dir.exists():
-            mode = "w"
-
-        if file == None:
-            file = open(dir, mode)
-
-        if not isinstance(text, list):
-            return None
-
-        for index in text:
-            if "Node" in index:
-                file.write(f'{index["Node"]} \n')
-            if "Children" in index:
-                self.node_scrape(text=index["Children"], file=file)
-        file.close()
-
-    async def parse_get_api_spec(self, instance_type: str, data: dict) -> None | str | dict[str, Any] | list | bool | int | None:
-        """
-        Creates a `api_spec.txt` in the script directory with nodes from api `Core/GetAPISpec`
-        #TODO - Improve formatting of the Markdown file.
-        Args:
-            amp (Core): API_Core class object signed in.
-
-        See -> `../docs/api_spec.md` 
-        """
-        # res = await amp.get_api_spec()
-        dir = Path(__file__).parent.joinpath(f"../docs/{instance_type}_api_spec.md")
-        mode = "x"
-        if dir.exists():
-            mode = "w"
-        file = open(dir, mode)
-
-        if not isinstance(data, dict):
-            return None
-        else:
-            for parent, parent_value in data.items():
-                if isinstance(parent_value, dict):
-                    for child, child_value in parent_value.items():
-                        file.write(f"{parent}.{child}:({child_value}) \n")
-                else:
-                    file.write(f"{parent}({parent_value}) \n")
-
-        file.close()
+from __future__ import annotations
+
+from pathlib import Path
+from typing import Any
+
+from .core import Core
+
+
+class APIUtil():
+    """
+    AMP API util functions to parse specific API calls for specific Data.
+    """
+
+    async def get_node_spec(self, amp: Core) -> str | dict[str, Any] | list | bool | int | None:
+        """
+        Creates a `setting_nodes.txt` in the script directory with nodes from api `Core/GetSettingSpec`
+
+        Args:
+            amp (Core): API_Core class object signed in.
+
+        See -> `amp/util/setting_nodes.txt` 
+
+        """
+        res = await amp.get_settings_spec()
+        dir = Path(__file__).parent.joinpath("../docs/setting_nodes.md")
+        mode = "x"
+        if dir.exists():
+            mode = "w"
+        file = open(dir, mode)
+
+        if not isinstance(res, dict):
+            return res
+
+        for key in res:
+            for value in res[key]:
+                for entry in value:
+                    if entry.lower() == "node":
+                        file.write(f"{value[entry]} \n")
+        file.close()
+
+    async def get_permission_nodes(self, amp: Core) -> str | dict[str, Any] | list | bool | int | None:
+        """
+        Creates a `permission_nodes.txt` in the script directory with nodes from api `Core/GetPermissionsSpec`
+
+        Args:
+            amp (Core): API_Core class object signed in.
+
+        See -> `amp/util/permission_nodes.txt`  
+        """
+        res = await amp.get_permissions_spec()
+        if isinstance(res, list):
+            self.node_scrape(text=res)
+        else:
+            raise ValueError(f"Error - invalid data type returned. {type(res)}")
+
+    def node_scrape(self, text: list[dict], file=None) -> None:
+        """
+        Pulls the key "Nodes" from the list of dictionary results and dumps them to a txt file.
+
+        Args:
+            text (list): The list of dictionary's
+            file (_type_, optional): The file object to dump text to. Defaults to None. `**LEAVE NONE**`
+        """
+        dir = Path(__file__).parent.joinpath("../docs/permission_nodes.md")
+        mode = "x"
+        if dir.exists():
+            mode = "w"
+
+        if file == None:
+            file = open(dir, mode)
+
+        if not isinstance(text, list):
+            return None
+
+        for index in text:
+            if "Node" in index:
+                file.write(f'{index["Node"]} \n')
+            if "Children" in index:
+                self.node_scrape(text=index["Children"], file=file)
+        file.close()
+
+    async def parse_get_api_spec(self, instance_type: str, data: dict) -> None | str | dict[str, Any] | list | bool | int | None:
+        """
+        Creates a `api_spec.txt` in the script directory with nodes from api `Core/GetAPISpec`
+        #TODO - Improve formatting of the Markdown file.
+        Args:
+            amp (Core): API_Core class object signed in.
+
+        See -> `../docs/api_spec.md` 
+        """
+        # res = await amp.get_api_spec()
+        dir = Path(__file__).parent.joinpath(f"../docs/{instance_type}_api_spec.md")
+        mode = "x"
+        if dir.exists():
+            mode = "w"
+        file = open(dir, mode)
+
+        if not isinstance(data, dict):
+            return None
+        else:
+            for parent, parent_value in data.items():
+                if isinstance(parent_value, dict):
+                    for child, child_value in parent_value.items():
+                        file.write(f"{parent}.{child}:({child_value}) \n")
+                else:
+                    file.write(f"{parent}({parent_value}) \n")
+
+        file.close()
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO` & `cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,17 @@
 Metadata-Version: 2.1
-Name: cubecoders-amp-api-wrapper
-Version: 0.0.40b0
+Name: cubecoders_amp_api_wrapper
+Version: 0.0.41b0
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
-Description: # AMPAPI_Python_wrapper
-        ___
-        CubeCoders AMP API wrapper in Python. 
-        
-        ### Key Features
-        ___
-        
-        - Pythonic API wrapper using `async` and `await`.
-        - Data is in dataclasses for easier management and interaction.
-            - Optional parameter per function or global to disable formatting of data.
-        - Parent classes `ADSInstance` and `AMPInstance` to group endpoints together and make handling of multiple Instances easier.
-            - This will also limit Instance specific API endpoints (eg. Minecraft) to that Instance type only.
-        
-        ### Installing
-        ___
-        
-        *Python 3.9 or higher is required*
-        
-        To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
-        
-        ### Pypi 
-        -> https://pypi.org/project/cubecoders-amp-api-wrapper/
-        ```bash
-        # Linux/macOS
-        pip install cubecoders-amp-api-wrapper
-        
-        # Windows
-        pip install cubecoders-amp-api-wrapper
-        ```
-        
-        
-        ### Quick Example -
-        
-        ```py
-        # You can pull these values from an `.ini` or a `.env` file,
-        # then populate the NamedTuple APIparams from `types -> APIParams`
-        _params = APIParams(url="http://192.168.13.130:8080",
-                            user="amp_username",
-                            password="amp_password")
-        
-        async def Sample_API():
-            """
-            Example API Function to call method Endpoints.
-            """
-            _bridge = Bridge(api_params=_params)
-            ADS: ADSInstance = ADSInstance()
-            # This would populate the ADS class property .AvailableInstances
-            ADS.get_instances()
-            # We can break out all our instances into their own attributes.
-            arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
-            mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
-        
-            # Pre populated from the dataclass and has the API methods too!
-            # You can take a backup really easily.
-            await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
-        
-            # Then you can call instance type specific API methods.
-            await mcinstance.mc_add_to_whitelist(user_or_uuid="k8_thekat")
-        
-            # You can also check attributes and other fields of the instance.
-            mcinstance.InstanceName
-            mcinstance.InstanceID
-        
-            # The State of the Instance. eg. Running, Offline, Restarting. See `types.py -> State_enum
-            # This is NOT updated constantly. See about using `get_status()` to keep it current.
-            if mcinstance.AppState == State_enum.Stopped:
-                await mcinstance.start_instance()
-        
-            # You can also check Metrics of an Instance easily.
-            mcinstance.Status.Metrics
-        
-            # Want to kick a random person? Here ya go~
-            players: list[Players] = await mcinstance.get_user_list()
-            await mcinstance.mc_kick_user_by_id(id=players[0].id)
-        ```
-        
-        
-        ### Controlling data formatting -
-        - All JSON data returned from the API endpoints is formatted into a Dataclass/Enum/etc if possible.
-        - Data formatting can be controlled globally or locally by changing the `format_data` parameter of the method to `False`.
-            - When turning off the data formatting, typically you will get a `dictionary` back.
-        
-        ### Example -
-        ```py
-        # By default all API calls will be formatted into Dataclasses if possible.
-        # You can toggle format_data off with ANY of the API classes that inherit Base().
-        ADS.format_data = False
-        
-        # You can turn data formatting back on globally through any Instance object.
-        arkinstance.format_data = True
-        
-        # You can turn off or on data formatting per function also.
-        await arkinstance.get_updates(format_data=False)
-        await arkinstance.get_role_data(format_data=True)
-        
-        ```
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -117,7 +20,108 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.7.4.post0
+Requires-Dist: dataclass_wizard==0.22.2
+Requires-Dist: pyotp==2.6.0
+
+# AMPAPI_Python_wrapper
+___
+CubeCoders AMP API wrapper in Python. 
+
+### Key Features
+___
+
+- Pythonic API wrapper using `async` and `await`.
+- Data is in dataclasses for easier management and interaction.
+    - Optional parameter per function or global to disable formatting of data.
+- Parent classes `ADSInstance` and `AMPInstance` to group endpoints together and make handling of multiple Instances easier.
+    - This will also limit Instance specific API endpoints (eg. Minecraft) to that Instance type only.
+
+### Installing
+___
+
+*Python 3.9 or higher is required*
+
+To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
+
+### Pypi 
+-> https://pypi.org/project/cubecoders-amp-api-wrapper/
+```bash
+# Linux/macOS
+pip install cubecoders-amp-api-wrapper
+
+# Windows
+pip install cubecoders-amp-api-wrapper
+```
+
+
+### Quick Example -
+
+```py
+# You can pull these values from an `.ini` or a `.env` file,
+# then populate the NamedTuple APIparams from `types -> APIParams`
+_params = APIParams(url="http://192.168.13.130:8080",
+                    user="amp_username",
+                    password="amp_password")
+
+async def Sample_API():
+    """
+    Example API Function to call method Endpoints.
+    """
+    _bridge = Bridge(api_params=_params)
+    ADS: ADSInstance = ADSInstance()
+    # This would populate the ADS class property .AvailableInstances
+    ADS.get_instances()
+    # We can break out all our instances into their own attributes.
+    arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
+    mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
+
+    # Pre populated from the dataclass and has the API methods too!
+    # You can take a backup really easily.
+    await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
+
+    # Then you can call instance type specific API methods.
+    await mcinstance.mc_add_to_whitelist(user_or_uuid="k8_thekat")
+
+    # You can also check attributes and other fields of the instance.
+    mcinstance.InstanceName
+    mcinstance.InstanceID
+
+    # The State of the Instance. eg. Running, Offline, Restarting. See `types.py -> State_enum
+    # This is NOT updated constantly. See about using `get_status()` to keep it current.
+    if mcinstance.AppState == State_enum.Stopped:
+        await mcinstance.start_instance()
+
+    # You can also check Metrics of an Instance easily.
+    mcinstance.Status.Metrics
+
+    # Want to kick a random person? Here ya go~
+    players: list[Players] = await mcinstance.get_user_list()
+    await mcinstance.mc_kick_user_by_id(id=players[0].id)
+```
+
+
+### Controlling data formatting -
+- All JSON data returned from the API endpoints is formatted into a Dataclass/Enum/etc if possible.
+- Data formatting can be controlled globally or locally by changing the `format_data` parameter of the method to `False`.
+    - When turning off the data formatting, typically you will get a `dictionary` back.
+
+### Example -
+```py
+# By default all API calls will be formatted into Dataclasses if possible.
+# You can toggle format_data off with ANY of the API classes that inherit Base().
+ADS.format_data = False
+
+# You can turn data formatting back on globally through any Instance object.
+arkinstance.format_data = True
+
+# You can turn off or on data formatting per function also.
+await arkinstance.get_updates(format_data=False)
+await arkinstance.get_role_data(format_data=True)
+
+```
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt` & `cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/docs/ADS_api_spec.md` & `cubecoders_amp_api_wrapper-0.0.41b0/docs/ADS_api_spec.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-ADSModule.AddDatastore:({'Parameters': [{'Name': 'newDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeleteDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpdateDatastore:({'Parameters': [{'Name': 'updatedDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.GetDatastores:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.RequestDatastoreSizeCalculation:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.RepairDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetDatastoreInstances:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.MoveInstanceDatastore:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetDeploymentTemplates:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.CreateDeploymentTemplate:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpdateDeploymentTemplate:({'Parameters': [{'Name': 'templateToUpdate', 'TypeName': 'DeploymentTemplate', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeleteDeploymentTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.CloneTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.ApplyTemplate:({'Description': "Overlays an existing template on an existing instance. Used to perform package reconfigurations. Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.", 'Returns': '', 'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewFriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'RestartIfPreviouslyRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeployTemplate:({'Parameters': [{'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': 'The ID of the template to be deployed, as per the Template Management UI in AMP itself.', 'Optional': False}, {'Name': 'NewUsername', 'TypeName': 'String', 'Description': 'If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user.', 'Optional': True}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user.", 'Optional': True}, {'Name': 'NewEmail', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user.", 'Optional': True}, {'Name': 'RequiredTags', 'TypeName': 'List<String>', 'Description': "If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings.", 'Optional': True}, {'Name': 'Tag', 'TypeName': 'String', 'Description': "Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique.", 'Optional': True}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': 'A friendly name for this instance. If left blank, AMP will generate one for you.', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': 'Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'ExtraProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': 'A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.', 'Optional': True}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetTargetInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.GetSupportedApplications:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.RefreshAppCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-ADSModule.RefreshRemoteConfigStores:({'Parameters': [{'Name': 'force', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-ADSModule.GetApplicationEndpoints:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.ReactivateLocalInstances:({'Parameters': [], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.GetInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.ModifyCustomFirewallRule:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Range', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Protocol', 'TypeName': 'PortProtocol', 'Description': '', 'Optional': False, 'ParamEnumValues': {'TCP': 0, 'UDP': 1, 'Both': 2}}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Open', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.ManageInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
-ADSModule.GetGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.RefreshGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.GetLocalInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.GetInstanceStatuses:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.GetProvisionFitness:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.AttachADS:({'Parameters': [{'Name': 'Friendly', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IsHTTPS', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Host', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Port', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DetatchTarget:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpdateTargetInfo:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Url', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Tags', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.ConvertToManaged:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.GetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.SetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortMappings', 'TypeName': 'Dictionary<String, Int32>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.ApplyInstanceConfiguration:({'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Args', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'RebuildConfiguration', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.CreateLocalInstance:({'Parameters': [{'Name': 'Instance', 'TypeName': 'LocalAMPInstance', 'Description': '', 'Optional': False}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.CreateInstance:({'Parameters': [{'Name': 'TargetADSInstance', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewInstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Module', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IPBinding', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'AdminUsername', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AdminPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'AutoConfigure', 'TypeName': 'Boolean', 'Description': 'When enabled, all settings other than the Module, Target and FriendlyName are ignored and replaced with automatically generated values.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}, {'Name': 'DisplayImageSource', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'TargetDatastore', 'TypeName': 'Int32', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.SetInstanceConfig:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.RefreshInstanceConfig:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.HandoutInstanceConfigs:({'Parameters': [{'Name': 'ForModule', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Values', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.GetProvisionArguments:({'Parameters': [{'Name': 'ModuleName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<ProvisionSettingInfo>', 'IsComplexType': True}) 
-ADSModule.TestADSLoginDetails:({'Parameters': [{'Name': 'url', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.RegisterTarget:({'Parameters': [{'Name': 'controllerUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'myUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'twoFactorToken', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'friendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpdateTarget:({'Parameters': [{'Name': 'TargetID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-ADSModule.UpdateInstanceInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ExcludeFromFirewall', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'RunInContainer', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ContainerMemory', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'MemoryPolicy', 'TypeName': 'ContainerMemoryPolicy', 'Description': '', 'Optional': False, 'ParamEnumValues': {'NotSpecified': 0, 'Reserve': 100, 'Restrict': 200}}, {'Name': 'ContainerMaxCPU', 'TypeName': 'Single', 'Description': '', 'Optional': False}, {'Name': 'ContainerImage', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.SetInstanceSuspended:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpgradeInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.StartAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.StopAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpgradeAllInstances:({'Parameters': [{'Name': 'RestartRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.StartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.RestartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.StopInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeleteInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.ExtractEverywhere:({'Parameters': [{'Name': 'SourceArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.Servers:({'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'REQ_RAWJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
-FileManagerPlugin.Dummy:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-FileManagerPlugin.CalculateFileMD5Sum:({'Parameters': [{'Name': 'FilePath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
-FileManagerPlugin.ChangeExclusion:({'Parameters': [{'Name': 'ModifyPath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsDirectory', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Exclude', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.CreateArchive:({'Parameters': [{'Name': 'PathToArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.ExtractArchive:({'Parameters': [{'Name': 'ArchivePath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'DestinationPath', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.GetDirectoryListing:({'Parameters': [{'Name': 'Dir', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-FileManagerPlugin.GetFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Position', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'Length', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-FileManagerPlugin.AppendFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Delete', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-FileManagerPlugin.ReadFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'ChunkSize', 'TypeName': 'Int64', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
-FileManagerPlugin.WriteFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'FinalChunk', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.DownloadFileFromURL:({'Parameters': [{'Name': 'Source', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.RenameFile:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewFilename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.CopyFile:({'Parameters': [{'Name': 'Origin', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.TrashFile:({'Description': 'Moves a file to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.TrashDirectory:({'Description': 'Moves a directory to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'DirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.EmptyTrash:({'Description': 'Empties a trash bin', 'Returns': '', 'Parameters': [{'Name': 'TrashDirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.CreateDirectory:({'Description': 'Creates a new directory. The parent directory must already exist.', 'Returns': '', 'Parameters': [{'Name': 'NewPath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.RenameDirectory:({'Description': 'Renames a directory', 'Returns': '', 'Parameters': [{'Name': 'oldDirectory', 'TypeName': 'String', 'Description': 'The full path to the old directory', 'Optional': False}, {'Name': 'NewDirectoryName', 'TypeName': 'String', 'Description': 'The name component of the new directory (not the full path)', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-EmailSenderPlugin.TestSMTPSettings:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-LocalFileBackupPlugin.UploadToS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-LocalFileBackupPlugin.DownloadFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-LocalFileBackupPlugin.DeleteFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-LocalFileBackupPlugin.GetBackups:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-LocalFileBackupPlugin.RestoreBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'DeleteExistingData', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-LocalFileBackupPlugin.DeleteLocalBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-LocalFileBackupPlugin.SetBackupSticky:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-LocalFileBackupPlugin.TakeBackup:({'Parameters': [{'Name': 'Title', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetAuditLogEntries:({'Parameters': [{'Name': 'Before', 'TypeName': 'Nullable<DateTime>', 'Description': '', 'Optional': False}, {'Name': 'Count', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<IAuditLogEntry>', 'IsComplexType': True}) 
-Core.GetSettingsSpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, IEnumerable<JObject>>', 'IsComplexType': True}) 
-Core.RefreshSettingValueList:({'Parameters': [{'Name': 'Node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.RefreshSettingsSourceCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetSettingValues:({'Parameters': [{'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'WithRefresh', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'IDictionary<String, String>', 'IsComplexType': False}) 
-Core.GetProvisionSpec:({'Parameters': [], 'ReturnTypeName': 'List<JObject>', 'IsComplexType': True}) 
-Core.GetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.GetConfigs:({'Parameters': [{'Name': 'nodes', 'TypeName': 'String[]', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-Core.SetConfigs:({'Parameters': [{'Name': 'data', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
-Core.SetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.ActivateAMPLicence:({'Parameters': [{'Name': 'LicenceKey', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'QueryOnly', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<JObject>', 'IsComplexType': True}) 
-Core.GetRoleData:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<AuthRoleSummary>', 'IsComplexType': True}) 
-Core.GetRoleIds:({'Parameters': [], 'ReturnTypeName': 'IDictionary<Guid, String>', 'IsComplexType': False}) 
-Core.GetRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'AuthRoleSummary', 'IsComplexType': True}) 
-Core.CreateRole:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsCommonRole', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True}) 
-Core.DeleteRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.RenameRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.SetAMPRolePermission:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PermissionNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Nullable<Boolean>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetAMPRolePermissions:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<String>', 'IsComplexType': False}) 
-Core.GetScheduleData:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.AddEventTrigger:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.RunEventTriggerImmediately:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.AddIntervalTrigger:({'Parameters': [{'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetTimeIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.EditIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.SetTriggerEnabled:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.AddTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'MethodID', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.EditTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.ChangeTaskOrder:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewOrder', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DeleteTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DeleteTrigger:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetActiveAMPSessions:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-Core.EndUserSession:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetAMPUsersSummary:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfoSummary>', 'IsComplexType': True}) 
-Core.GetAMPUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'UserInfo', 'IsComplexType': True}) 
-Core.GetAllAMPUserInfo:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfo>', 'IsComplexType': True}) 
-Core.SetAMPUserRoleMembership:({'Parameters': [{'Name': 'UserId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'IsMember', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetPermissionsSpec:({'Parameters': [], 'ReturnTypeName': 'IList<IPermissionsTreeNode>', 'IsComplexType': True}) 
-Core.CreateUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True}) 
-Core.DeleteUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.UpdateUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Disabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'PasswordExpires', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'CannotChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'MustChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetWebauthnChallenge:({'Parameters': [], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
-Core.GetWebauthnCredentialIDs:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.WebauthnRegister:({'Parameters': [{'Name': 'attestationObject', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'clientDataJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetWebauthnCredentialSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<WebauthnCredentialSummary>', 'IsComplexType': True}) 
-Core.RevokeWebauthnCredential:({'Parameters': [{'Name': 'ID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.UpdateAccountInfo:({'Parameters': [{'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.EnableTwoFactor:({'Description': 'Sets up two-factor authentication for the given user. ConfirmTwoFactorSetup must be invoked to complete setup.', 'Returns': 'Data container the URI for a QR code that should be scanned by a mobile authenticator.', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<TwoFactorSetupInfo>', 'IsComplexType': True}) 
-Core.ConfirmTwoFactorSetup:({'Description': 'Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DisableTwoFactor:({'Parameters': [{'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.ResetUserPassword:({'Description': 'For administrative users to alter the password of another user', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.ChangeUserPassword:({'Description': 'For a user to change their own password, requires knowing the old password', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'OldPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetUpdates:({'Description': 'Gets changes to the server status, in addition to any notifications or console output that have occured since the last time GetUpdates() was called by the current session.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.GetNewGuid:({'Parameters': [], 'ReturnTypeName': 'Guid', 'IsComplexType': False}) 
-Core.GetUserList:({'Description': 'Returns a list of in-application users', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False}) 
-Core.CurrentSessionHasPermission:({'Parameters': [{'Name': 'PermissionNode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
-Core.GetTasks:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<RunningTask>', 'IsComplexType': True}) 
-Core.GetPortSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<ListeningPortSummary>', 'IsComplexType': True}) 
-Core.GetStatus:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.CancelTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DismissTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DismissAllTasks:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetUserInfo:({'Description': 'Provides information about a given in-application user (as opposed to AMP system users)', 'Returns': '', 'Parameters': [{'Name': 'UID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'SimpleUser', 'IsComplexType': True}) 
-Core.Start:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.Suspend:({'Description': "Prevents the current instance from being started, and stops it if it's currently running.", 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.Resume:({'Description': 'Allows the service to be re-started after previously being suspended.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.Stop:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.Restart:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.Kill:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.Sleep:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.UpdateApplication:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.AcknowledgeAMPUpdate:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetModuleInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.GetAPISpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, Dictionary<String, JObject>>', 'IsComplexType': True}) 
-Core.GetUserActionsSpec:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False}) 
-Core.Login:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'token', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'rememberMe', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.GetRemoteLoginToken:({'Parameters': [{'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'IsTemporary', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
-Core.SendConsoleMessage:({'Parameters': [{'Name': 'message', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.UpdateAMPInstance:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetUpdateInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.Logout:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.RestartAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.UpgradeAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetDiagnosticsInfo:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False}) 
-Core.GetWebserverMetrics:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False}) 
-Core.CreateTestTask:({'Description': 'DEV: Creates a non-ending task with 50% progress for testing purposes', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.AsyncTest:({'Description': 'DEV: Async test method', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
+ADSModule.AddDatastore:({'Parameters': [{'Name': 'newDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.DeleteDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.UpdateDatastore:({'Parameters': [{'Name': 'updatedDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.GetDatastores:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.RequestDatastoreSizeCalculation:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+ADSModule.GetDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+ADSModule.RepairDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+ADSModule.GetDatastoreInstances:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.MoveInstanceDatastore:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+ADSModule.GetDeploymentTemplates:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.CreateDeploymentTemplate:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.UpdateDeploymentTemplate:({'Parameters': [{'Name': 'templateToUpdate', 'TypeName': 'DeploymentTemplate', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.DeleteDeploymentTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.CloneTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.ApplyTemplate:({'Description': "Overlays an existing template on an existing instance. Used to perform package reconfigurations. Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.", 'Returns': '', 'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewFriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'RestartIfPreviouslyRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.DeployTemplate:({'Parameters': [{'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': 'The ID of the template to be deployed, as per the Template Management UI in AMP itself.', 'Optional': False}, {'Name': 'NewUsername', 'TypeName': 'String', 'Description': 'If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user.', 'Optional': True}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user.", 'Optional': True}, {'Name': 'NewEmail', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user.", 'Optional': True}, {'Name': 'RequiredTags', 'TypeName': 'List<String>', 'Description': "If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings.", 'Optional': True}, {'Name': 'Tag', 'TypeName': 'String', 'Description': "Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique.", 'Optional': True}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': 'A friendly name for this instance. If left blank, AMP will generate one for you.', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': 'Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'ExtraProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': 'A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.', 'Optional': True}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+ADSModule.GetTargetInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+ADSModule.GetSupportedApplications:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.RefreshAppCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+ADSModule.RefreshRemoteConfigStores:({'Parameters': [{'Name': 'force', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+ADSModule.GetApplicationEndpoints:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.ReactivateLocalInstances:({'Parameters': [], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+ADSModule.GetInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.GetInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+ADSModule.ModifyCustomFirewallRule:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Range', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Protocol', 'TypeName': 'PortProtocol', 'Description': '', 'Optional': False, 'ParamEnumValues': {'TCP': 0, 'UDP': 1, 'Both': 2}}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Open', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.ManageInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
+ADSModule.GetGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+ADSModule.RefreshGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.GetLocalInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.GetInstanceStatuses:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.GetProvisionFitness:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+ADSModule.AttachADS:({'Parameters': [{'Name': 'Friendly', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IsHTTPS', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Host', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Port', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.DetatchTarget:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.UpdateTargetInfo:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Url', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Tags', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.ConvertToManaged:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.GetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+ADSModule.SetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortMappings', 'TypeName': 'Dictionary<String, Int32>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.ApplyInstanceConfiguration:({'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Args', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'RebuildConfiguration', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.CreateLocalInstance:({'Parameters': [{'Name': 'Instance', 'TypeName': 'LocalAMPInstance', 'Description': '', 'Optional': False}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.CreateInstance:({'Parameters': [{'Name': 'TargetADSInstance', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewInstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Module', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IPBinding', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'AdminUsername', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AdminPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'AutoConfigure', 'TypeName': 'Boolean', 'Description': 'When enabled, all settings other than the Module, Target and FriendlyName are ignored and replaced with automatically generated values.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}, {'Name': 'DisplayImageSource', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'TargetDatastore', 'TypeName': 'Int32', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.SetInstanceConfig:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.RefreshInstanceConfig:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.HandoutInstanceConfigs:({'Parameters': [{'Name': 'ForModule', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Values', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.GetProvisionArguments:({'Parameters': [{'Name': 'ModuleName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<ProvisionSettingInfo>', 'IsComplexType': True}) 
+ADSModule.TestADSLoginDetails:({'Parameters': [{'Name': 'url', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.RegisterTarget:({'Parameters': [{'Name': 'controllerUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'myUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'twoFactorToken', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'friendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.UpdateTarget:({'Parameters': [{'Name': 'TargetID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+ADSModule.UpdateInstanceInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ExcludeFromFirewall', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'RunInContainer', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ContainerMemory', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'MemoryPolicy', 'TypeName': 'ContainerMemoryPolicy', 'Description': '', 'Optional': False, 'ParamEnumValues': {'NotSpecified': 0, 'Reserve': 100, 'Restrict': 200}}, {'Name': 'ContainerMaxCPU', 'TypeName': 'Single', 'Description': '', 'Optional': False}, {'Name': 'ContainerImage', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.SetInstanceSuspended:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.UpgradeInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.StartAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.StopAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.UpgradeAllInstances:({'Parameters': [{'Name': 'RestartRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.StartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.RestartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.StopInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.DeleteInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+ADSModule.ExtractEverywhere:({'Parameters': [{'Name': 'SourceArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+ADSModule.Servers:({'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'REQ_RAWJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+FileManagerPlugin.Dummy:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+FileManagerPlugin.CalculateFileMD5Sum:({'Parameters': [{'Name': 'FilePath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
+FileManagerPlugin.ChangeExclusion:({'Parameters': [{'Name': 'ModifyPath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsDirectory', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Exclude', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.CreateArchive:({'Parameters': [{'Name': 'PathToArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.ExtractArchive:({'Parameters': [{'Name': 'ArchivePath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'DestinationPath', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.GetDirectoryListing:({'Parameters': [{'Name': 'Dir', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+FileManagerPlugin.GetFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Position', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'Length', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+FileManagerPlugin.AppendFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Delete', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+FileManagerPlugin.ReadFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'ChunkSize', 'TypeName': 'Int64', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
+FileManagerPlugin.WriteFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'FinalChunk', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.DownloadFileFromURL:({'Parameters': [{'Name': 'Source', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.RenameFile:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewFilename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.CopyFile:({'Parameters': [{'Name': 'Origin', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.TrashFile:({'Description': 'Moves a file to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.TrashDirectory:({'Description': 'Moves a directory to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'DirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.EmptyTrash:({'Description': 'Empties a trash bin', 'Returns': '', 'Parameters': [{'Name': 'TrashDirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.CreateDirectory:({'Description': 'Creates a new directory. The parent directory must already exist.', 'Returns': '', 'Parameters': [{'Name': 'NewPath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.RenameDirectory:({'Description': 'Renames a directory', 'Returns': '', 'Parameters': [{'Name': 'oldDirectory', 'TypeName': 'String', 'Description': 'The full path to the old directory', 'Optional': False}, {'Name': 'NewDirectoryName', 'TypeName': 'String', 'Description': 'The name component of the new directory (not the full path)', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+EmailSenderPlugin.TestSMTPSettings:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+LocalFileBackupPlugin.UploadToS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+LocalFileBackupPlugin.DownloadFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+LocalFileBackupPlugin.DeleteFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+LocalFileBackupPlugin.GetBackups:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+LocalFileBackupPlugin.RestoreBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'DeleteExistingData', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+LocalFileBackupPlugin.DeleteLocalBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+LocalFileBackupPlugin.SetBackupSticky:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+LocalFileBackupPlugin.TakeBackup:({'Parameters': [{'Name': 'Title', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetAuditLogEntries:({'Parameters': [{'Name': 'Before', 'TypeName': 'Nullable<DateTime>', 'Description': '', 'Optional': False}, {'Name': 'Count', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<IAuditLogEntry>', 'IsComplexType': True}) 
+Core.GetSettingsSpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, IEnumerable<JObject>>', 'IsComplexType': True}) 
+Core.RefreshSettingValueList:({'Parameters': [{'Name': 'Node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.RefreshSettingsSourceCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetSettingValues:({'Parameters': [{'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'WithRefresh', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'IDictionary<String, String>', 'IsComplexType': False}) 
+Core.GetProvisionSpec:({'Parameters': [], 'ReturnTypeName': 'List<JObject>', 'IsComplexType': True}) 
+Core.GetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.GetConfigs:({'Parameters': [{'Name': 'nodes', 'TypeName': 'String[]', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+Core.SetConfigs:({'Parameters': [{'Name': 'data', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
+Core.SetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.ActivateAMPLicence:({'Parameters': [{'Name': 'LicenceKey', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'QueryOnly', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<JObject>', 'IsComplexType': True}) 
+Core.GetRoleData:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<AuthRoleSummary>', 'IsComplexType': True}) 
+Core.GetRoleIds:({'Parameters': [], 'ReturnTypeName': 'IDictionary<Guid, String>', 'IsComplexType': False}) 
+Core.GetRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'AuthRoleSummary', 'IsComplexType': True}) 
+Core.CreateRole:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsCommonRole', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True}) 
+Core.DeleteRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.RenameRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.SetAMPRolePermission:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PermissionNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Nullable<Boolean>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetAMPRolePermissions:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<String>', 'IsComplexType': False}) 
+Core.GetScheduleData:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.AddEventTrigger:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.RunEventTriggerImmediately:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.AddIntervalTrigger:({'Parameters': [{'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetTimeIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.EditIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.SetTriggerEnabled:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.AddTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'MethodID', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.EditTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.ChangeTaskOrder:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewOrder', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DeleteTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DeleteTrigger:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetActiveAMPSessions:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+Core.EndUserSession:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetAMPUsersSummary:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfoSummary>', 'IsComplexType': True}) 
+Core.GetAMPUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'UserInfo', 'IsComplexType': True}) 
+Core.GetAllAMPUserInfo:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfo>', 'IsComplexType': True}) 
+Core.SetAMPUserRoleMembership:({'Parameters': [{'Name': 'UserId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'IsMember', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetPermissionsSpec:({'Parameters': [], 'ReturnTypeName': 'IList<IPermissionsTreeNode>', 'IsComplexType': True}) 
+Core.CreateUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True}) 
+Core.DeleteUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.UpdateUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Disabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'PasswordExpires', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'CannotChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'MustChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetWebauthnChallenge:({'Parameters': [], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
+Core.GetWebauthnCredentialIDs:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.WebauthnRegister:({'Parameters': [{'Name': 'attestationObject', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'clientDataJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetWebauthnCredentialSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<WebauthnCredentialSummary>', 'IsComplexType': True}) 
+Core.RevokeWebauthnCredential:({'Parameters': [{'Name': 'ID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.UpdateAccountInfo:({'Parameters': [{'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.EnableTwoFactor:({'Description': 'Sets up two-factor authentication for the given user. ConfirmTwoFactorSetup must be invoked to complete setup.', 'Returns': 'Data container the URI for a QR code that should be scanned by a mobile authenticator.', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<TwoFactorSetupInfo>', 'IsComplexType': True}) 
+Core.ConfirmTwoFactorSetup:({'Description': 'Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DisableTwoFactor:({'Parameters': [{'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.ResetUserPassword:({'Description': 'For administrative users to alter the password of another user', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.ChangeUserPassword:({'Description': 'For a user to change their own password, requires knowing the old password', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'OldPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetUpdates:({'Description': 'Gets changes to the server status, in addition to any notifications or console output that have occured since the last time GetUpdates() was called by the current session.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.GetNewGuid:({'Parameters': [], 'ReturnTypeName': 'Guid', 'IsComplexType': False}) 
+Core.GetUserList:({'Description': 'Returns a list of in-application users', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False}) 
+Core.CurrentSessionHasPermission:({'Parameters': [{'Name': 'PermissionNode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
+Core.GetTasks:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<RunningTask>', 'IsComplexType': True}) 
+Core.GetPortSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<ListeningPortSummary>', 'IsComplexType': True}) 
+Core.GetStatus:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.CancelTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DismissTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DismissAllTasks:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetUserInfo:({'Description': 'Provides information about a given in-application user (as opposed to AMP system users)', 'Returns': '', 'Parameters': [{'Name': 'UID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'SimpleUser', 'IsComplexType': True}) 
+Core.Start:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.Suspend:({'Description': "Prevents the current instance from being started, and stops it if it's currently running.", 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.Resume:({'Description': 'Allows the service to be re-started after previously being suspended.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.Stop:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.Restart:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.Kill:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.Sleep:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.UpdateApplication:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.AcknowledgeAMPUpdate:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetModuleInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.GetAPISpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, Dictionary<String, JObject>>', 'IsComplexType': True}) 
+Core.GetUserActionsSpec:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False}) 
+Core.Login:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'token', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'rememberMe', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.GetRemoteLoginToken:({'Parameters': [{'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'IsTemporary', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
+Core.SendConsoleMessage:({'Parameters': [{'Name': 'message', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.UpdateAMPInstance:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetUpdateInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.Logout:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.RestartAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.UpgradeAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetDiagnosticsInfo:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False}) 
+Core.GetWebserverMetrics:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False}) 
+Core.CreateTestTask:({'Description': 'DEV: Creates a non-ending task with 50% progress for testing purposes', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.AsyncTest:({'Description': 'DEV: Async test method', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False})
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/docs/Minecraft_api_spec.md` & `cubecoders_amp_api_wrapper-0.0.41b0/docs/Minecraft_api_spec.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-MinecraftModule.BukGetCategories:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
-MinecraftModule.BukGetPopularPlugins:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
-MinecraftModule.BukGetPluginsForCategory:({'Parameters': [{'Name': 'CategoryId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
-MinecraftModule.BukGetPluginInfo:({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
-MinecraftModule.BukGetInstalledPlugins:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
-MinecraftModule.BukGetRemovePlugin:({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-MinecraftModule.BukGetInstallUpdatePlugin:({'Parameters': [{'Name': 'pluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-MinecraftModule.BukGetSearch:({'Parameters': [{'Name': 'Query', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
-MinecraftModule.GetHeadByUUID:({'Description': 'Get a skin as a base64 string', 'Returns': '', 'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
-MinecraftModule.GetFailureReason:({'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
-MinecraftModule.AcceptEULA:({'Parameters': [], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
-MinecraftModule.BanUserByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-MinecraftModule.KickUserByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-MinecraftModule.ClearInventoryByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-MinecraftModule.KillByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-MinecraftModule.SmiteByID:({'Description': 'Strike a player with lightning', 'Returns': '', 'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-MinecraftModule.GetOPWhitelist:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-MinecraftModule.GetWhitelist:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-MinecraftModule.LoadOPList:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-MinecraftModule.AddOPEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-MinecraftModule.RemoveOPEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-MinecraftModule.AddToWhitelist:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-MinecraftModule.RemoveWhitelistEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-FileManagerPlugin.Dummy:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-FileManagerPlugin.CalculateFileMD5Sum:({'Parameters': [{'Name': 'FilePath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
-FileManagerPlugin.ChangeExclusion:({'Parameters': [{'Name': 'ModifyPath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsDirectory', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Exclude', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.CreateArchive:({'Parameters': [{'Name': 'PathToArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.ExtractArchive:({'Parameters': [{'Name': 'ArchivePath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'DestinationPath', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.GetDirectoryListing:({'Parameters': [{'Name': 'Dir', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-FileManagerPlugin.GetFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Position', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'Length', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-FileManagerPlugin.AppendFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Delete', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-FileManagerPlugin.ReadFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'ChunkSize', 'TypeName': 'Int64', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
-FileManagerPlugin.WriteFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'FinalChunk', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.DownloadFileFromURL:({'Parameters': [{'Name': 'Source', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.RenameFile:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewFilename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.CopyFile:({'Parameters': [{'Name': 'Origin', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.TrashFile:({'Description': 'Moves a file to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.TrashDirectory:({'Description': 'Moves a directory to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'DirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.EmptyTrash:({'Description': 'Empties a trash bin', 'Returns': '', 'Parameters': [{'Name': 'TrashDirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.CreateDirectory:({'Description': 'Creates a new directory. The parent directory must already exist.', 'Returns': '', 'Parameters': [{'Name': 'NewPath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-FileManagerPlugin.RenameDirectory:({'Description': 'Renames a directory', 'Returns': '', 'Parameters': [{'Name': 'oldDirectory', 'TypeName': 'String', 'Description': 'The full path to the old directory', 'Optional': False}, {'Name': 'NewDirectoryName', 'TypeName': 'String', 'Description': 'The name component of the new directory (not the full path)', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-EmailSenderPlugin.TestSMTPSettings:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-LocalFileBackupPlugin.UploadToS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-LocalFileBackupPlugin.DownloadFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-LocalFileBackupPlugin.DeleteFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-LocalFileBackupPlugin.GetBackups:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-LocalFileBackupPlugin.RestoreBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'DeleteExistingData', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-LocalFileBackupPlugin.DeleteLocalBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-LocalFileBackupPlugin.SetBackupSticky:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-LocalFileBackupPlugin.TakeBackup:({'Parameters': [{'Name': 'Title', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetAuditLogEntries:({'Parameters': [{'Name': 'Before', 'TypeName': 'Nullable<DateTime>', 'Description': '', 'Optional': False}, {'Name': 'Count', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<IAuditLogEntry>', 'IsComplexType': True}) 
-Core.GetSettingsSpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, IEnumerable<JObject>>', 'IsComplexType': True}) 
-Core.RefreshSettingValueList:({'Parameters': [{'Name': 'Node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.RefreshSettingsSourceCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetSettingValues:({'Parameters': [{'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'WithRefresh', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'IDictionary<String, String>', 'IsComplexType': False}) 
-Core.GetProvisionSpec:({'Parameters': [], 'ReturnTypeName': 'List<JObject>', 'IsComplexType': True}) 
-Core.GetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.GetConfigs:({'Parameters': [{'Name': 'nodes', 'TypeName': 'String[]', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-Core.SetConfigs:({'Parameters': [{'Name': 'data', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
-Core.SetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.ActivateAMPLicence:({'Parameters': [{'Name': 'LicenceKey', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'QueryOnly', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<JObject>', 'IsComplexType': True}) 
-Core.GetRoleData:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<AuthRoleSummary>', 'IsComplexType': True}) 
-Core.GetRoleIds:({'Parameters': [], 'ReturnTypeName': 'IDictionary<Guid, String>', 'IsComplexType': False}) 
-Core.GetRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'AuthRoleSummary', 'IsComplexType': True}) 
-Core.CreateRole:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsCommonRole', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True}) 
-Core.DeleteRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.RenameRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.SetAMPRolePermission:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PermissionNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Nullable<Boolean>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetAMPRolePermissions:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<String>', 'IsComplexType': False}) 
-Core.GetScheduleData:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.AddEventTrigger:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.RunEventTriggerImmediately:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.AddIntervalTrigger:({'Parameters': [{'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetTimeIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.EditIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.SetTriggerEnabled:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.AddTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'MethodID', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.EditTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.ChangeTaskOrder:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewOrder', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DeleteTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DeleteTrigger:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetActiveAMPSessions:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-Core.EndUserSession:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetAMPUsersSummary:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfoSummary>', 'IsComplexType': True}) 
-Core.GetAMPUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'UserInfo', 'IsComplexType': True}) 
-Core.GetAllAMPUserInfo:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfo>', 'IsComplexType': True}) 
-Core.SetAMPUserRoleMembership:({'Parameters': [{'Name': 'UserId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'IsMember', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetPermissionsSpec:({'Parameters': [], 'ReturnTypeName': 'IList<IPermissionsTreeNode>', 'IsComplexType': True}) 
-Core.CreateUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True}) 
-Core.DeleteUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.UpdateUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Disabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'PasswordExpires', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'CannotChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'MustChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetWebauthnChallenge:({'Parameters': [], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
-Core.GetWebauthnCredentialIDs:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.WebauthnRegister:({'Parameters': [{'Name': 'attestationObject', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'clientDataJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetWebauthnCredentialSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<WebauthnCredentialSummary>', 'IsComplexType': True}) 
-Core.RevokeWebauthnCredential:({'Parameters': [{'Name': 'ID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.UpdateAccountInfo:({'Parameters': [{'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.EnableTwoFactor:({'Description': 'Sets up two-factor authentication for the given user. ConfirmTwoFactorSetup must be invoked to complete setup.', 'Returns': 'Data container the URI for a QR code that should be scanned by a mobile authenticator.', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<TwoFactorSetupInfo>', 'IsComplexType': True}) 
-Core.ConfirmTwoFactorSetup:({'Description': 'Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DisableTwoFactor:({'Parameters': [{'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.ResetUserPassword:({'Description': 'For administrative users to alter the password of another user', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.ChangeUserPassword:({'Description': 'For a user to change their own password, requires knowing the old password', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'OldPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetUpdates:({'Description': 'Gets changes to the server status, in addition to any notifications or console output that have occured since the last time GetUpdates() was called by the current session.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.GetNewGuid:({'Parameters': [], 'ReturnTypeName': 'Guid', 'IsComplexType': False}) 
-Core.GetUserList:({'Description': 'Returns a list of in-application users', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False}) 
-Core.CurrentSessionHasPermission:({'Parameters': [{'Name': 'PermissionNode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
-Core.GetTasks:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<RunningTask>', 'IsComplexType': True}) 
-Core.GetPortSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<ListeningPortSummary>', 'IsComplexType': True}) 
-Core.GetStatus:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.CancelTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DismissTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.DismissAllTasks:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.GetUserInfo:({'Description': 'Provides information about a given in-application user (as opposed to AMP system users)', 'Returns': '', 'Parameters': [{'Name': 'UID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'SimpleUser', 'IsComplexType': True}) 
-Core.Start:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.Suspend:({'Description': "Prevents the current instance from being started, and stops it if it's currently running.", 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.Resume:({'Description': 'Allows the service to be re-started after previously being suspended.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.Stop:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.Restart:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.Kill:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.Sleep:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.UpdateApplication:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-Core.AcknowledgeAMPUpdate:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetModuleInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.GetAPISpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, Dictionary<String, JObject>>', 'IsComplexType': True}) 
-Core.GetUserActionsSpec:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False}) 
-Core.Login:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'token', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'rememberMe', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.GetRemoteLoginToken:({'Parameters': [{'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'IsTemporary', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
-Core.SendConsoleMessage:({'Parameters': [{'Name': 'message', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.UpdateAMPInstance:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetUpdateInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-Core.Logout:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.RestartAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.UpgradeAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.GetDiagnosticsInfo:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False}) 
-Core.GetWebserverMetrics:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False}) 
-Core.CreateTestTask:({'Description': 'DEV: Creates a non-ending task with 50% progress for testing purposes', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-Core.AsyncTest:({'Description': 'DEV: Async test method', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
+MinecraftModule.BukGetCategories:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetPopularPlugins:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetPluginsForCategory:({'Parameters': [{'Name': 'CategoryId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetPluginInfo:({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetInstalledPlugins:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetRemovePlugin:({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.BukGetInstallUpdatePlugin:({'Parameters': [{'Name': 'pluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+MinecraftModule.BukGetSearch:({'Parameters': [{'Name': 'Query', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.GetHeadByUUID:({'Description': 'Get a skin as a base64 string', 'Returns': '', 'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
+MinecraftModule.GetFailureReason:({'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
+MinecraftModule.AcceptEULA:({'Parameters': [], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
+MinecraftModule.BanUserByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.KickUserByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.ClearInventoryByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.KillByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.SmiteByID:({'Description': 'Strike a player with lightning', 'Returns': '', 'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.GetOPWhitelist:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+MinecraftModule.GetWhitelist:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+MinecraftModule.LoadOPList:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+MinecraftModule.AddOPEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+MinecraftModule.RemoveOPEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.AddToWhitelist:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+MinecraftModule.RemoveWhitelistEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+FileManagerPlugin.Dummy:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+FileManagerPlugin.CalculateFileMD5Sum:({'Parameters': [{'Name': 'FilePath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
+FileManagerPlugin.ChangeExclusion:({'Parameters': [{'Name': 'ModifyPath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsDirectory', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Exclude', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.CreateArchive:({'Parameters': [{'Name': 'PathToArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.ExtractArchive:({'Parameters': [{'Name': 'ArchivePath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'DestinationPath', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.GetDirectoryListing:({'Parameters': [{'Name': 'Dir', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+FileManagerPlugin.GetFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Position', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'Length', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+FileManagerPlugin.AppendFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Delete', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+FileManagerPlugin.ReadFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'ChunkSize', 'TypeName': 'Int64', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
+FileManagerPlugin.WriteFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Data', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Offset', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'FinalChunk', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.DownloadFileFromURL:({'Parameters': [{'Name': 'Source', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.RenameFile:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewFilename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.CopyFile:({'Parameters': [{'Name': 'Origin', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TargetDirectory', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.TrashFile:({'Description': 'Moves a file to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.TrashDirectory:({'Description': 'Moves a directory to trash, files must be trashed before they can be deleted.', 'Returns': '', 'Parameters': [{'Name': 'DirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.EmptyTrash:({'Description': 'Empties a trash bin', 'Returns': '', 'Parameters': [{'Name': 'TrashDirectoryName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.CreateDirectory:({'Description': 'Creates a new directory. The parent directory must already exist.', 'Returns': '', 'Parameters': [{'Name': 'NewPath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+FileManagerPlugin.RenameDirectory:({'Description': 'Renames a directory', 'Returns': '', 'Parameters': [{'Name': 'oldDirectory', 'TypeName': 'String', 'Description': 'The full path to the old directory', 'Optional': False}, {'Name': 'NewDirectoryName', 'TypeName': 'String', 'Description': 'The name component of the new directory (not the full path)', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+EmailSenderPlugin.TestSMTPSettings:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+LocalFileBackupPlugin.UploadToS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+LocalFileBackupPlugin.DownloadFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+LocalFileBackupPlugin.DeleteFromS3:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+LocalFileBackupPlugin.GetBackups:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+LocalFileBackupPlugin.RestoreBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'DeleteExistingData', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+LocalFileBackupPlugin.DeleteLocalBackup:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+LocalFileBackupPlugin.SetBackupSticky:({'Parameters': [{'Name': 'BackupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+LocalFileBackupPlugin.TakeBackup:({'Parameters': [{'Name': 'Title', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Sticky', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetAuditLogEntries:({'Parameters': [{'Name': 'Before', 'TypeName': 'Nullable<DateTime>', 'Description': '', 'Optional': False}, {'Name': 'Count', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<IAuditLogEntry>', 'IsComplexType': True}) 
+Core.GetSettingsSpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, IEnumerable<JObject>>', 'IsComplexType': True}) 
+Core.RefreshSettingValueList:({'Parameters': [{'Name': 'Node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.RefreshSettingsSourceCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetSettingValues:({'Parameters': [{'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'WithRefresh', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'IDictionary<String, String>', 'IsComplexType': False}) 
+Core.GetProvisionSpec:({'Parameters': [], 'ReturnTypeName': 'List<JObject>', 'IsComplexType': True}) 
+Core.GetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.GetConfigs:({'Parameters': [{'Name': 'nodes', 'TypeName': 'String[]', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+Core.SetConfigs:({'Parameters': [{'Name': 'data', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
+Core.SetConfig:({'Parameters': [{'Name': 'node', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.ActivateAMPLicence:({'Parameters': [{'Name': 'LicenceKey', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'QueryOnly', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<JObject>', 'IsComplexType': True}) 
+Core.GetRoleData:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<AuthRoleSummary>', 'IsComplexType': True}) 
+Core.GetRoleIds:({'Parameters': [], 'ReturnTypeName': 'IDictionary<Guid, String>', 'IsComplexType': False}) 
+Core.GetRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'AuthRoleSummary', 'IsComplexType': True}) 
+Core.CreateRole:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsCommonRole', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True}) 
+Core.DeleteRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.RenameRole:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.SetAMPRolePermission:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PermissionNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Nullable<Boolean>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetAMPRolePermissions:({'Parameters': [{'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<String>', 'IsComplexType': False}) 
+Core.GetScheduleData:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.AddEventTrigger:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.RunEventTriggerImmediately:({'Parameters': [{'Name': 'triggerId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.AddIntervalTrigger:({'Parameters': [{'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetTimeIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.EditIntervalTrigger:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'months', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'days', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'hours', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'minutes', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'daysOfMonth', 'TypeName': 'Int32[]', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.SetTriggerEnabled:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Enabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.AddTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'MethodID', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.EditTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'ParameterMapping', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.ChangeTaskOrder:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewOrder', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DeleteTask:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TaskID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DeleteTrigger:({'Parameters': [{'Name': 'TriggerID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetActiveAMPSessions:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+Core.EndUserSession:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetAMPUsersSummary:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfoSummary>', 'IsComplexType': True}) 
+Core.GetAMPUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'UserInfo', 'IsComplexType': True}) 
+Core.GetAllAMPUserInfo:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<UserInfo>', 'IsComplexType': True}) 
+Core.SetAMPUserRoleMembership:({'Parameters': [{'Name': 'UserId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'RoleId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'IsMember', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetPermissionsSpec:({'Parameters': [], 'ReturnTypeName': 'IList<IPermissionsTreeNode>', 'IsComplexType': True}) 
+Core.CreateUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<Guid>', 'IsComplexType': True}) 
+Core.DeleteUser:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.UpdateUserInfo:({'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Disabled', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'PasswordExpires', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'CannotChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'MustChangePassword', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetWebauthnChallenge:({'Parameters': [], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
+Core.GetWebauthnCredentialIDs:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.WebauthnRegister:({'Parameters': [{'Name': 'attestationObject', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'clientDataJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'description', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetWebauthnCredentialSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<WebauthnCredentialSummary>', 'IsComplexType': True}) 
+Core.RevokeWebauthnCredential:({'Parameters': [{'Name': 'ID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.UpdateAccountInfo:({'Parameters': [{'Name': 'EmailAddress', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.EnableTwoFactor:({'Description': 'Sets up two-factor authentication for the given user. ConfirmTwoFactorSetup must be invoked to complete setup.', 'Returns': 'Data container the URI for a QR code that should be scanned by a mobile authenticator.', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<TwoFactorSetupInfo>', 'IsComplexType': True}) 
+Core.ConfirmTwoFactorSetup:({'Description': 'Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DisableTwoFactor:({'Parameters': [{'Name': 'Password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorCode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.ResetUserPassword:({'Description': 'For administrative users to alter the password of another user', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.ChangeUserPassword:({'Description': 'For a user to change their own password, requires knowing the old password', 'Returns': '', 'Parameters': [{'Name': 'Username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'OldPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'TwoFactorPIN', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetUpdates:({'Description': 'Gets changes to the server status, in addition to any notifications or console output that have occured since the last time GetUpdates() was called by the current session.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.GetNewGuid:({'Parameters': [], 'ReturnTypeName': 'Guid', 'IsComplexType': False}) 
+Core.GetUserList:({'Description': 'Returns a list of in-application users', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False}) 
+Core.CurrentSessionHasPermission:({'Parameters': [{'Name': 'PermissionNode', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
+Core.GetTasks:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<RunningTask>', 'IsComplexType': True}) 
+Core.GetPortSummaries:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<ListeningPortSummary>', 'IsComplexType': True}) 
+Core.GetStatus:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.CancelTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DismissTask:({'Parameters': [{'Name': 'TaskId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.DismissAllTasks:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.GetUserInfo:({'Description': 'Provides information about a given in-application user (as opposed to AMP system users)', 'Returns': '', 'Parameters': [{'Name': 'UID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'SimpleUser', 'IsComplexType': True}) 
+Core.Start:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.Suspend:({'Description': "Prevents the current instance from being started, and stops it if it's currently running.", 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.Resume:({'Description': 'Allows the service to be re-started after previously being suspended.', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.Stop:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.Restart:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.Kill:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.Sleep:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.UpdateApplication:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+Core.AcknowledgeAMPUpdate:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetModuleInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.GetAPISpec:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, Dictionary<String, JObject>>', 'IsComplexType': True}) 
+Core.GetUserActionsSpec:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False}) 
+Core.Login:({'Parameters': [{'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'token', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'rememberMe', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.GetRemoteLoginToken:({'Parameters': [{'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'IsTemporary', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
+Core.SendConsoleMessage:({'Parameters': [{'Name': 'message', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.UpdateAMPInstance:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetUpdateInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+Core.Logout:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.RestartAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.UpgradeAMP:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.GetDiagnosticsInfo:({'Parameters': [], 'ReturnTypeName': 'Dictionary<String, String>', 'IsComplexType': False}) 
+Core.GetWebserverMetrics:({'Parameters': [], 'ReturnTypeName': 'Object', 'IsComplexType': False}) 
+Core.CreateTestTask:({'Description': 'DEV: Creates a non-ending task with 50% progress for testing purposes', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+Core.AsyncTest:({'Description': 'DEV: Async test method', 'Returns': '', 'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False})
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/docs/permission_nodes.md` & `cubecoders_amp_api_wrapper-0.0.41b0/docs/permission_nodes.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-Settings 
-Settings.Core 
-Settings.Core.Security 
-Settings.Core.Security.EnablePassthruAuth 
-Settings.Core.Security.AuthFailureTimeWindow 
-Settings.Core.Security.AuthFailureAttemptsInWindow 
-Settings.Core.Security.TwoFactorMode 
-Settings.Core.Security.RequireSessionIPStickiness 
-Settings.Core.Security.AllowUserPasswords 
-Settings.Core.Webserver 
-Settings.Core.Webserver.APIRateLimit 
-Settings.Core.Webserver.AllowGETForAPIEndpoints 
-Settings.Core.Webserver.CORSOrigin 
-Settings.Core.Webserver.DisableCompression 
-Settings.Core.Login 
-Settings.Core.Login.UseAuthServer 
-Settings.Core.Login.AuthServerURL 
-Settings.Core.Branding 
-Settings.Core.Branding.DisplayBranding 
-Settings.Core.Branding.PageTitle 
-Settings.Core.Branding.CompanyName 
-Settings.Core.Branding.WelcomeMessage 
-Settings.Core.Branding.BrandingMessage 
-Settings.Core.Branding.ShortBrandingMessage 
-Settings.Core.Branding.URL 
-Settings.Core.Branding.SupportURL 
-Settings.Core.Branding.SupportText 
-Settings.Core.Branding.SubmitTicketURL 
-Settings.Core.Branding.LogoURL 
-Settings.Core.Branding.BackgroundURL 
-Settings.Core.Branding.SplashFrameURL 
-Settings.Core.Branding.ForgotPasswordURL 
-Settings.Core.AMP 
-Settings.Core.AMP.ScheduleOffsetSeconds 
-Settings.Core.AMP.AppStartupMode 
-Settings.Core.AMP.FirstStart 
-Settings.Core.AMP.MapAllPluginStores 
-Settings.Core.AMP.Theme 
-Settings.Core.AMP.ShowHelpOnStatus 
-Settings.Core.Monitoring 
-Settings.Core.Monitoring.UseMulticoreCPUCalc 
-Settings.Core.Monitoring.IgnoreSMTCores 
-Settings.Core.Monitoring.ConsoleScrollback 
-Settings.Core.Monitoring.LogLevel 
-Settings.Core.Monitoring.FullMetricsGathering 
-Settings.Core.Monitoring.ReportPhysicalMemoryAsTotal 
-Settings.Core.Monitoring.MetricsPollInterval 
-Settings.Core.Privacy 
-Settings.Core.Privacy.PrivacySettingsSet 
-Settings.Core.Privacy.AutoReportFatalExceptions 
-Settings.Core.Privacy.AllowAnalytics 
-Settings.ADSModule 
-Settings.ADSModule.Limits 
-Settings.ADSModule.Limits.InstanceLimit 
-Settings.ADSModule.Limits.CreateLocalInstances 
-Settings.ADSModule.Defaults 
-Settings.ADSModule.Defaults.NewInstanceKey 
-Settings.ADSModule.Defaults.DefaultSettings 
-Settings.ADSModule.Defaults.DefaultReleaseStream 
-Settings.ADSModule.Defaults.UseDocker 
-Settings.ADSModule.Defaults.DefaultAuthServerURL 
-Settings.ADSModule.Defaults.PropagateAuthServer 
-Settings.ADSModule.Defaults.PropogateRepos 
-Settings.ADSModule.Defaults.UseOverlays 
-Settings.ADSModule.Defaults.MatchVersion 
-Settings.ADSModule.Defaults.DefaultPostCreate 
-Settings.ADSModule.Defaults.ExcludeFromFirewall 
-Settings.ADSModule.ADS 
-Settings.ADSModule.ADS.AutoReactivate 
-Settings.ADSModule.ADS.Mode 
-Settings.ADSModule.ADS.AutostartInstances 
-Settings.ADSModule.ADS.InstanceStartDelay 
-Settings.ADSModule.ADS.ConfigurationRepositories 
-Settings.ADSModule.ADS.ShowDeprecated 
-Settings.ADSModule.Network 
-Settings.ADSModule.Network.DefaultIPBinding 
-Settings.ADSModule.Network.DefaultAppIPBinding 
-Settings.ADSModule.Network.DockerExternalIPBinding 
-Settings.ADSModule.Network.AMPPortRanges 
-Settings.ADSModule.Network.PortAssignment 
-Settings.ADSModule.Network.AppPortRanges 
-Settings.ADSModule.Network.AppPortExclusions 
-Settings.ADSModule.Network.MetricsServerPort 
-Settings.ADSModule.Network.UseDockerHostNetwork 
-Settings.ADSModule.Network.UseTraefik 
-Settings.ADSModule.Network.TraefikNetworkName 
-Settings.ADSModule.Network.TraefikDomainWildcard 
-Settings.ADSModule.Network.AccessMode 
-Settings.ADSModule.Network.BaseURL 
-Settings.FileManagerPlugin 
-Settings.FileManagerPlugin.Security 
-Settings.FileManagerPlugin.Security.RestrictUploadExtensions 
-Settings.FileManagerPlugin.Security.RestrictDownloadExtensions 
-Settings.FileManagerPlugin.Security.DownloadableExtensions 
-Settings.FileManagerPlugin.Security.UploadableExtensions 
-Settings.FileManagerPlugin.Security.AllowExtensionChange 
-Settings.FileManagerPlugin.Security.AllowArchiveOperations 
-Settings.FileManagerPlugin.Security.OnlyExtractUploadableExtensionsFromArchives 
-Settings.FileManagerPlugin.Security.HoneypotSFTPLogins 
-Settings.FileManagerPlugin.FileManager 
-Settings.FileManagerPlugin.FileManager.AdditionalVirtualDirectories 
-Settings.FileManagerPlugin.FileManager.FastFileTransfers 
-Settings.FileManagerPlugin.SFTP 
-Settings.FileManagerPlugin.SFTP.EnableCompression 
-Settings.EmailSenderPlugin 
-Settings.EmailSenderPlugin.SMTP 
-Settings.EmailSenderPlugin.SMTP.UseSSL 
-Settings.EmailSenderPlugin.SMTP.Host 
-Settings.EmailSenderPlugin.SMTP.Port 
-Settings.EmailSenderPlugin.SMTP.Username 
-Settings.EmailSenderPlugin.SMTP.Password 
-Settings.EmailSenderPlugin.SMTP.EmailFrom 
-Settings.WebRequestPlugin 
-Settings.WebRequestPlugin.WebhookLogins 
-Settings.WebRequestPlugin.WebhookLogins.PushbulletAccessToken 
-Settings.LocalFileBackupPlugin 
-Settings.LocalFileBackupPlugin.Limits 
-Settings.LocalFileBackupPlugin.Limits.MaxTotalSizeMB 
-Settings.LocalFileBackupPlugin.Limits.MaxIndividualSizeMB 
-Settings.LocalFileBackupPlugin.Limits.MaxBackupCount 
-Settings.LocalFileBackupPlugin.Limits.ReplacePolicy 
-Settings.LocalFileBackupPlugin.Limits.Compression 
-Settings.LocalFileBackupPlugin.Cloud 
-Settings.LocalFileBackupPlugin.Cloud.UseS3Storage 
-Settings.LocalFileBackupPlugin.Cloud.S3ServiceURL 
-Settings.LocalFileBackupPlugin.Cloud.S3AuthenticationRegion 
-Settings.LocalFileBackupPlugin.Cloud.S3BucketName 
-Settings.LocalFileBackupPlugin.Cloud.S3AccessKey 
-Settings.LocalFileBackupPlugin.Cloud.S3SecretKey 
-Settings.LocalFileBackupPlugin.Cloud.S3UploadMode 
-Settings.LocalFileBackupPlugin.Cloud.S3StorageClass 
-Settings.steamcmdplugin 
-Settings.steamcmdplugin.SteamWorkshop 
-Settings.steamcmdplugin.SteamWorkshop.WorkshopItemIDs 
-Settings.steamcmdplugin.SteamUpdateSettings 
-Settings.steamcmdplugin.SteamUpdateSettings.AutomaticallyRetryOnFailure 
-Settings.steamcmdplugin.SteamUpdateSettings.AutomaticRetryLimit 
-Settings.steamcmdplugin.SteamUpdateSettings.UpdateCheckMethod 
-Settings.steamcmdplugin.SteamUpdateSettings.SteamCMDBetaPassword 
-Settings.steamcmdplugin.SteamUpdateSettings.ThrottleDownloadSpeed 
-Settings.steamcmdplugin.SteamUpdateSettings.KeepSteamCMDScripts 
-ADS 
-ADS.DatastoreManagement 
-ADS.DatastoreManagement.ManageDatastores 
-ADS.TemplateManagement 
-ADS.TemplateManagement.ManageTemplates 
-ADS.InstanceManagement 
-ADS.InstanceManagement.RegisterToController 
-ADS.InstanceManagement.CreateInstance 
-ADS.InstanceManagement.SuspendInstances 
-ADS.InstanceManagement.UpgradeInstances 
-ADS.InstanceManagement.StopInstances 
-ADS.InstanceManagement.DeleteInstances 
-ADS.InstanceManagement.StartInstances 
-ADS.InstanceManagement.AttachRemoteADSInstance 
-ADS.InstanceManagement.RemoveRemoteADSInstance 
-ADS.InstanceManagement.EditRemoteTargets 
-ADS.InstanceManagement.Convert 
-ADS.InstanceManagement.Reconfigure 
-ADS.InstanceManagement.RestartInstances 
-ADS.InstanceManagement.RefreshConfiguration 
-ADS.InstanceManagement.RefreshRemoteConfigStores 
-ADS.InstanceManagement.ManageSuspendedInstances 
-FileManager 
-FileManager.FileManager 
-FileManager.FileManager.CreateArchive 
-FileManager.FileManager.ExtractArchive 
-FileManager.FileManager.BrowseFiles 
-FileManager.FileManager.DownloadFiles 
-FileManager.FileManager.UploadFiles 
-FileManager.FileManager.RenameFiles 
-FileManager.FileManager.ChangeFileExtension 
-FileManager.FileManager.CopyFiles 
-FileManager.FileManager.TrashFiles 
-FileManager.FileManager.TrashDirectories 
-FileManager.FileManager.EmptyTrash 
-FileManager.FileManager.CreateDirectory 
-FileManager.FileManager.RenameDirectories 
-FileManager.FileManager.ChangeBackupExclusions 
-FileManager.FileManager.DownloadFromURL 
-FileManager.FileManager.ModifyAMPConfigFiles 
-FileManager.FileManager.ConnectViaSFTP 
-LocalFileBackup 
-LocalFileBackup.Backup 
-LocalFileBackup.Backup.ViewBackupsList 
-LocalFileBackup.Backup.CreateBackup 
-LocalFileBackup.Backup.DeleteBackup 
-LocalFileBackup.Backup.RestoreBackup 
-LocalFileBackup.Backup.ToggleStickiness 
-LocalFileBackup.Backup.ArchiveBackup 
-LocalFileBackup.Backup.TransferBackup 
-Core 
-Core.AuditLog 
-Core.AuditLog.ViewAuditLog 
-Core.Special 
-Core.Special.CancelOtherUsersTasks 
-Core.Special.ViewOtherUsersTasks 
-Core.Special.UpdateAMPInstance 
-Core.Special.UseDevMethods 
-Core.Special.RestartAMP 
-Core.Special.Diagnostics 
-Core.Special.UpgradeAMP 
-Core.Special.BypassSettingValueLimits 
-Core.Special.QueryLicenceInformation 
-Core.Special.ActivateAMP 
-Core.RoleManagement 
-Core.RoleManagement.ViewRoles 
-Core.RoleManagement.CreateRole 
-Core.RoleManagement.DeleteRoles 
-Core.RoleManagement.EditRoleInfo 
-Core.RoleManagement.EditRolePermissions 
-Core.RoleManagement.CreateCommonRoles 
-Core.Scheduler 
-Core.Scheduler.ViewSchedule 
-Core.Scheduler.CreateTrigger 
-Core.Scheduler.EditTrigger 
-Core.Scheduler.CreateTask 
-Core.Scheduler.DeleteTask 
-Core.Scheduler.DeleteTrigger 
-Core.Scheduler.EditTask 
-Core.Scheduler.EditOtherUsersTasks 
-Core.UserManagement 
-Core.UserManagement.ChangeRoleMembership 
-Core.UserManagement.UpdateUserInfo 
-Core.UserManagement.UpdateOwnAccount 
-Core.UserManagement.DeleteUser 
-Core.UserManagement.ResetUserPassword 
-Core.UserManagement.CreateNewUser 
-Core.UserManagement.ViewOtherUsersSessions 
-Core.UserManagement.EndUserSessions 
-Core.UserManagement.ViewUserInfo 
-Core.UserManagement.AccessExternalPermissions 
-Core.AppManagement 
-Core.AppManagement.StartApplication 
-Core.AppManagement.StopApplication 
-Core.AppManagement.RestartApplication 
-Core.AppManagement.UpdateApplication 
-Core.AppManagement.SendConsoleInput 
-Core.AppManagement.ReadConsole 
-Instances 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Start 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Stop 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Restart 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Update 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Manage 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Start 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Stop 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Restart 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Update 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Manage 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Start 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Stop 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Restart 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Update 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Manage 
+Settings 
+Settings.Core 
+Settings.Core.Security 
+Settings.Core.Security.EnablePassthruAuth 
+Settings.Core.Security.AuthFailureTimeWindow 
+Settings.Core.Security.AuthFailureAttemptsInWindow 
+Settings.Core.Security.TwoFactorMode 
+Settings.Core.Security.RequireSessionIPStickiness 
+Settings.Core.Security.AllowUserPasswords 
+Settings.Core.Webserver 
+Settings.Core.Webserver.APIRateLimit 
+Settings.Core.Webserver.AllowGETForAPIEndpoints 
+Settings.Core.Webserver.CORSOrigin 
+Settings.Core.Webserver.DisableCompression 
+Settings.Core.Login 
+Settings.Core.Login.UseAuthServer 
+Settings.Core.Login.AuthServerURL 
+Settings.Core.Branding 
+Settings.Core.Branding.DisplayBranding 
+Settings.Core.Branding.PageTitle 
+Settings.Core.Branding.CompanyName 
+Settings.Core.Branding.WelcomeMessage 
+Settings.Core.Branding.BrandingMessage 
+Settings.Core.Branding.ShortBrandingMessage 
+Settings.Core.Branding.URL 
+Settings.Core.Branding.SupportURL 
+Settings.Core.Branding.SupportText 
+Settings.Core.Branding.SubmitTicketURL 
+Settings.Core.Branding.LogoURL 
+Settings.Core.Branding.BackgroundURL 
+Settings.Core.Branding.SplashFrameURL 
+Settings.Core.Branding.ForgotPasswordURL 
+Settings.Core.AMP 
+Settings.Core.AMP.ScheduleOffsetSeconds 
+Settings.Core.AMP.AppStartupMode 
+Settings.Core.AMP.FirstStart 
+Settings.Core.AMP.MapAllPluginStores 
+Settings.Core.AMP.Theme 
+Settings.Core.AMP.ShowHelpOnStatus 
+Settings.Core.Monitoring 
+Settings.Core.Monitoring.UseMulticoreCPUCalc 
+Settings.Core.Monitoring.IgnoreSMTCores 
+Settings.Core.Monitoring.ConsoleScrollback 
+Settings.Core.Monitoring.LogLevel 
+Settings.Core.Monitoring.FullMetricsGathering 
+Settings.Core.Monitoring.ReportPhysicalMemoryAsTotal 
+Settings.Core.Monitoring.MetricsPollInterval 
+Settings.Core.Privacy 
+Settings.Core.Privacy.PrivacySettingsSet 
+Settings.Core.Privacy.AutoReportFatalExceptions 
+Settings.Core.Privacy.AllowAnalytics 
+Settings.ADSModule 
+Settings.ADSModule.Limits 
+Settings.ADSModule.Limits.InstanceLimit 
+Settings.ADSModule.Limits.CreateLocalInstances 
+Settings.ADSModule.Defaults 
+Settings.ADSModule.Defaults.NewInstanceKey 
+Settings.ADSModule.Defaults.DefaultSettings 
+Settings.ADSModule.Defaults.DefaultReleaseStream 
+Settings.ADSModule.Defaults.UseDocker 
+Settings.ADSModule.Defaults.DefaultAuthServerURL 
+Settings.ADSModule.Defaults.PropagateAuthServer 
+Settings.ADSModule.Defaults.PropogateRepos 
+Settings.ADSModule.Defaults.UseOverlays 
+Settings.ADSModule.Defaults.MatchVersion 
+Settings.ADSModule.Defaults.DefaultPostCreate 
+Settings.ADSModule.Defaults.ExcludeFromFirewall 
+Settings.ADSModule.ADS 
+Settings.ADSModule.ADS.AutoReactivate 
+Settings.ADSModule.ADS.Mode 
+Settings.ADSModule.ADS.AutostartInstances 
+Settings.ADSModule.ADS.InstanceStartDelay 
+Settings.ADSModule.ADS.ConfigurationRepositories 
+Settings.ADSModule.ADS.ShowDeprecated 
+Settings.ADSModule.Network 
+Settings.ADSModule.Network.DefaultIPBinding 
+Settings.ADSModule.Network.DefaultAppIPBinding 
+Settings.ADSModule.Network.DockerExternalIPBinding 
+Settings.ADSModule.Network.AMPPortRanges 
+Settings.ADSModule.Network.PortAssignment 
+Settings.ADSModule.Network.AppPortRanges 
+Settings.ADSModule.Network.AppPortExclusions 
+Settings.ADSModule.Network.MetricsServerPort 
+Settings.ADSModule.Network.UseDockerHostNetwork 
+Settings.ADSModule.Network.UseTraefik 
+Settings.ADSModule.Network.TraefikNetworkName 
+Settings.ADSModule.Network.TraefikDomainWildcard 
+Settings.ADSModule.Network.AccessMode 
+Settings.ADSModule.Network.BaseURL 
+Settings.FileManagerPlugin 
+Settings.FileManagerPlugin.Security 
+Settings.FileManagerPlugin.Security.RestrictUploadExtensions 
+Settings.FileManagerPlugin.Security.RestrictDownloadExtensions 
+Settings.FileManagerPlugin.Security.DownloadableExtensions 
+Settings.FileManagerPlugin.Security.UploadableExtensions 
+Settings.FileManagerPlugin.Security.AllowExtensionChange 
+Settings.FileManagerPlugin.Security.AllowArchiveOperations 
+Settings.FileManagerPlugin.Security.OnlyExtractUploadableExtensionsFromArchives 
+Settings.FileManagerPlugin.Security.HoneypotSFTPLogins 
+Settings.FileManagerPlugin.FileManager 
+Settings.FileManagerPlugin.FileManager.AdditionalVirtualDirectories 
+Settings.FileManagerPlugin.FileManager.FastFileTransfers 
+Settings.FileManagerPlugin.SFTP 
+Settings.FileManagerPlugin.SFTP.EnableCompression 
+Settings.EmailSenderPlugin 
+Settings.EmailSenderPlugin.SMTP 
+Settings.EmailSenderPlugin.SMTP.UseSSL 
+Settings.EmailSenderPlugin.SMTP.Host 
+Settings.EmailSenderPlugin.SMTP.Port 
+Settings.EmailSenderPlugin.SMTP.Username 
+Settings.EmailSenderPlugin.SMTP.Password 
+Settings.EmailSenderPlugin.SMTP.EmailFrom 
+Settings.WebRequestPlugin 
+Settings.WebRequestPlugin.WebhookLogins 
+Settings.WebRequestPlugin.WebhookLogins.PushbulletAccessToken 
+Settings.LocalFileBackupPlugin 
+Settings.LocalFileBackupPlugin.Limits 
+Settings.LocalFileBackupPlugin.Limits.MaxTotalSizeMB 
+Settings.LocalFileBackupPlugin.Limits.MaxIndividualSizeMB 
+Settings.LocalFileBackupPlugin.Limits.MaxBackupCount 
+Settings.LocalFileBackupPlugin.Limits.ReplacePolicy 
+Settings.LocalFileBackupPlugin.Limits.Compression 
+Settings.LocalFileBackupPlugin.Cloud 
+Settings.LocalFileBackupPlugin.Cloud.UseS3Storage 
+Settings.LocalFileBackupPlugin.Cloud.S3ServiceURL 
+Settings.LocalFileBackupPlugin.Cloud.S3AuthenticationRegion 
+Settings.LocalFileBackupPlugin.Cloud.S3BucketName 
+Settings.LocalFileBackupPlugin.Cloud.S3AccessKey 
+Settings.LocalFileBackupPlugin.Cloud.S3SecretKey 
+Settings.LocalFileBackupPlugin.Cloud.S3UploadMode 
+Settings.LocalFileBackupPlugin.Cloud.S3StorageClass 
+Settings.steamcmdplugin 
+Settings.steamcmdplugin.SteamWorkshop 
+Settings.steamcmdplugin.SteamWorkshop.WorkshopItemIDs 
+Settings.steamcmdplugin.SteamUpdateSettings 
+Settings.steamcmdplugin.SteamUpdateSettings.AutomaticallyRetryOnFailure 
+Settings.steamcmdplugin.SteamUpdateSettings.AutomaticRetryLimit 
+Settings.steamcmdplugin.SteamUpdateSettings.UpdateCheckMethod 
+Settings.steamcmdplugin.SteamUpdateSettings.SteamCMDBetaPassword 
+Settings.steamcmdplugin.SteamUpdateSettings.ThrottleDownloadSpeed 
+Settings.steamcmdplugin.SteamUpdateSettings.KeepSteamCMDScripts 
+ADS 
+ADS.DatastoreManagement 
+ADS.DatastoreManagement.ManageDatastores 
+ADS.TemplateManagement 
+ADS.TemplateManagement.ManageTemplates 
+ADS.InstanceManagement 
+ADS.InstanceManagement.RegisterToController 
+ADS.InstanceManagement.CreateInstance 
+ADS.InstanceManagement.SuspendInstances 
+ADS.InstanceManagement.UpgradeInstances 
+ADS.InstanceManagement.StopInstances 
+ADS.InstanceManagement.DeleteInstances 
+ADS.InstanceManagement.StartInstances 
+ADS.InstanceManagement.AttachRemoteADSInstance 
+ADS.InstanceManagement.RemoveRemoteADSInstance 
+ADS.InstanceManagement.EditRemoteTargets 
+ADS.InstanceManagement.Convert 
+ADS.InstanceManagement.Reconfigure 
+ADS.InstanceManagement.RestartInstances 
+ADS.InstanceManagement.RefreshConfiguration 
+ADS.InstanceManagement.RefreshRemoteConfigStores 
+ADS.InstanceManagement.ManageSuspendedInstances 
+FileManager 
+FileManager.FileManager 
+FileManager.FileManager.CreateArchive 
+FileManager.FileManager.ExtractArchive 
+FileManager.FileManager.BrowseFiles 
+FileManager.FileManager.DownloadFiles 
+FileManager.FileManager.UploadFiles 
+FileManager.FileManager.RenameFiles 
+FileManager.FileManager.ChangeFileExtension 
+FileManager.FileManager.CopyFiles 
+FileManager.FileManager.TrashFiles 
+FileManager.FileManager.TrashDirectories 
+FileManager.FileManager.EmptyTrash 
+FileManager.FileManager.CreateDirectory 
+FileManager.FileManager.RenameDirectories 
+FileManager.FileManager.ChangeBackupExclusions 
+FileManager.FileManager.DownloadFromURL 
+FileManager.FileManager.ModifyAMPConfigFiles 
+FileManager.FileManager.ConnectViaSFTP 
+LocalFileBackup 
+LocalFileBackup.Backup 
+LocalFileBackup.Backup.ViewBackupsList 
+LocalFileBackup.Backup.CreateBackup 
+LocalFileBackup.Backup.DeleteBackup 
+LocalFileBackup.Backup.RestoreBackup 
+LocalFileBackup.Backup.ToggleStickiness 
+LocalFileBackup.Backup.ArchiveBackup 
+LocalFileBackup.Backup.TransferBackup 
+Core 
+Core.AuditLog 
+Core.AuditLog.ViewAuditLog 
+Core.Special 
+Core.Special.CancelOtherUsersTasks 
+Core.Special.ViewOtherUsersTasks 
+Core.Special.UpdateAMPInstance 
+Core.Special.UseDevMethods 
+Core.Special.RestartAMP 
+Core.Special.Diagnostics 
+Core.Special.UpgradeAMP 
+Core.Special.BypassSettingValueLimits 
+Core.Special.QueryLicenceInformation 
+Core.Special.ActivateAMP 
+Core.RoleManagement 
+Core.RoleManagement.ViewRoles 
+Core.RoleManagement.CreateRole 
+Core.RoleManagement.DeleteRoles 
+Core.RoleManagement.EditRoleInfo 
+Core.RoleManagement.EditRolePermissions 
+Core.RoleManagement.CreateCommonRoles 
+Core.Scheduler 
+Core.Scheduler.ViewSchedule 
+Core.Scheduler.CreateTrigger 
+Core.Scheduler.EditTrigger 
+Core.Scheduler.CreateTask 
+Core.Scheduler.DeleteTask 
+Core.Scheduler.DeleteTrigger 
+Core.Scheduler.EditTask 
+Core.Scheduler.EditOtherUsersTasks 
+Core.UserManagement 
+Core.UserManagement.ChangeRoleMembership 
+Core.UserManagement.UpdateUserInfo 
+Core.UserManagement.UpdateOwnAccount 
+Core.UserManagement.DeleteUser 
+Core.UserManagement.ResetUserPassword 
+Core.UserManagement.CreateNewUser 
+Core.UserManagement.ViewOtherUsersSessions 
+Core.UserManagement.EndUserSessions 
+Core.UserManagement.ViewUserInfo 
+Core.UserManagement.AccessExternalPermissions 
+Core.AppManagement 
+Core.AppManagement.StartApplication 
+Core.AppManagement.StopApplication 
+Core.AppManagement.RestartApplication 
+Core.AppManagement.UpdateApplication 
+Core.AppManagement.SendConsoleInput 
+Core.AppManagement.ReadConsole 
+Instances 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Start 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Stop 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Restart 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Update 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Manage 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Start 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Stop 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Restart 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Update 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Manage 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Start 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Stop 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Restart 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Update 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Manage
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/docs/permission_nodes.txt` & `cubecoders_amp_api_wrapper-0.0.41b0/docs/permission_nodes.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-Settings 
-Settings.Core 
-Settings.Core.Security 
-Settings.Core.Security.EnablePassthruAuth 
-Settings.Core.Security.AuthFailureTimeWindow 
-Settings.Core.Security.AuthFailureAttemptsInWindow 
-Settings.Core.Security.TwoFactorMode 
-Settings.Core.Security.RequireSessionIPStickiness 
-Settings.Core.Security.AllowUserPasswords 
-Settings.Core.Webserver 
-Settings.Core.Webserver.APIRateLimit 
-Settings.Core.Webserver.AllowGETForAPIEndpoints 
-Settings.Core.Webserver.CORSOrigin 
-Settings.Core.Webserver.DisableCompression 
-Settings.Core.Login 
-Settings.Core.Login.UseAuthServer 
-Settings.Core.Login.AuthServerURL 
-Settings.Core.Branding 
-Settings.Core.Branding.DisplayBranding 
-Settings.Core.Branding.PageTitle 
-Settings.Core.Branding.CompanyName 
-Settings.Core.Branding.WelcomeMessage 
-Settings.Core.Branding.BrandingMessage 
-Settings.Core.Branding.ShortBrandingMessage 
-Settings.Core.Branding.URL 
-Settings.Core.Branding.SupportURL 
-Settings.Core.Branding.SupportText 
-Settings.Core.Branding.SubmitTicketURL 
-Settings.Core.Branding.LogoURL 
-Settings.Core.Branding.BackgroundURL 
-Settings.Core.Branding.SplashFrameURL 
-Settings.Core.Branding.ForgotPasswordURL 
-Settings.Core.AMP 
-Settings.Core.AMP.ScheduleOffsetSeconds 
-Settings.Core.AMP.AppStartupMode 
-Settings.Core.AMP.FirstStart 
-Settings.Core.AMP.MapAllPluginStores 
-Settings.Core.AMP.Theme 
-Settings.Core.AMP.ShowHelpOnStatus 
-Settings.Core.Monitoring 
-Settings.Core.Monitoring.UseMulticoreCPUCalc 
-Settings.Core.Monitoring.IgnoreSMTCores 
-Settings.Core.Monitoring.ConsoleScrollback 
-Settings.Core.Monitoring.LogLevel 
-Settings.Core.Monitoring.FullMetricsGathering 
-Settings.Core.Monitoring.ReportPhysicalMemoryAsTotal 
-Settings.Core.Monitoring.MetricsPollInterval 
-Settings.Core.Privacy 
-Settings.Core.Privacy.PrivacySettingsSet 
-Settings.Core.Privacy.AutoReportFatalExceptions 
-Settings.Core.Privacy.AllowAnalytics 
-Settings.ADSModule 
-Settings.ADSModule.Limits 
-Settings.ADSModule.Limits.InstanceLimit 
-Settings.ADSModule.Limits.CreateLocalInstances 
-Settings.ADSModule.Defaults 
-Settings.ADSModule.Defaults.NewInstanceKey 
-Settings.ADSModule.Defaults.DefaultSettings 
-Settings.ADSModule.Defaults.DefaultReleaseStream 
-Settings.ADSModule.Defaults.UseDocker 
-Settings.ADSModule.Defaults.DefaultAuthServerURL 
-Settings.ADSModule.Defaults.PropagateAuthServer 
-Settings.ADSModule.Defaults.PropogateRepos 
-Settings.ADSModule.Defaults.UseOverlays 
-Settings.ADSModule.Defaults.MatchVersion 
-Settings.ADSModule.Defaults.DefaultPostCreate 
-Settings.ADSModule.Defaults.ExcludeFromFirewall 
-Settings.ADSModule.ADS 
-Settings.ADSModule.ADS.AutoReactivate 
-Settings.ADSModule.ADS.Mode 
-Settings.ADSModule.ADS.AutostartInstances 
-Settings.ADSModule.ADS.InstanceStartDelay 
-Settings.ADSModule.ADS.ConfigurationRepositories 
-Settings.ADSModule.ADS.ShowDeprecated 
-Settings.ADSModule.Network 
-Settings.ADSModule.Network.DefaultIPBinding 
-Settings.ADSModule.Network.DefaultAppIPBinding 
-Settings.ADSModule.Network.DockerExternalIPBinding 
-Settings.ADSModule.Network.AMPPortRanges 
-Settings.ADSModule.Network.PortAssignment 
-Settings.ADSModule.Network.AppPortRanges 
-Settings.ADSModule.Network.AppPortExclusions 
-Settings.ADSModule.Network.MetricsServerPort 
-Settings.ADSModule.Network.UseDockerHostNetwork 
-Settings.ADSModule.Network.UseTraefik 
-Settings.ADSModule.Network.TraefikNetworkName 
-Settings.ADSModule.Network.TraefikDomainWildcard 
-Settings.ADSModule.Network.AccessMode 
-Settings.ADSModule.Network.BaseURL 
-Settings.FileManagerPlugin 
-Settings.FileManagerPlugin.Security 
-Settings.FileManagerPlugin.Security.RestrictUploadExtensions 
-Settings.FileManagerPlugin.Security.RestrictDownloadExtensions 
-Settings.FileManagerPlugin.Security.DownloadableExtensions 
-Settings.FileManagerPlugin.Security.UploadableExtensions 
-Settings.FileManagerPlugin.Security.AllowExtensionChange 
-Settings.FileManagerPlugin.Security.AllowArchiveOperations 
-Settings.FileManagerPlugin.Security.OnlyExtractUploadableExtensionsFromArchives 
-Settings.FileManagerPlugin.Security.HoneypotSFTPLogins 
-Settings.FileManagerPlugin.FileManager 
-Settings.FileManagerPlugin.FileManager.AdditionalVirtualDirectories 
-Settings.FileManagerPlugin.FileManager.FastFileTransfers 
-Settings.FileManagerPlugin.SFTP 
-Settings.FileManagerPlugin.SFTP.EnableCompression 
-Settings.EmailSenderPlugin 
-Settings.EmailSenderPlugin.SMTP 
-Settings.EmailSenderPlugin.SMTP.UseSSL 
-Settings.EmailSenderPlugin.SMTP.Host 
-Settings.EmailSenderPlugin.SMTP.Port 
-Settings.EmailSenderPlugin.SMTP.Username 
-Settings.EmailSenderPlugin.SMTP.Password 
-Settings.EmailSenderPlugin.SMTP.EmailFrom 
-Settings.WebRequestPlugin 
-Settings.WebRequestPlugin.WebhookLogins 
-Settings.WebRequestPlugin.WebhookLogins.PushbulletAccessToken 
-Settings.LocalFileBackupPlugin 
-Settings.LocalFileBackupPlugin.Limits 
-Settings.LocalFileBackupPlugin.Limits.MaxTotalSizeMB 
-Settings.LocalFileBackupPlugin.Limits.MaxIndividualSizeMB 
-Settings.LocalFileBackupPlugin.Limits.MaxBackupCount 
-Settings.LocalFileBackupPlugin.Limits.ReplacePolicy 
-Settings.LocalFileBackupPlugin.Limits.Compression 
-Settings.LocalFileBackupPlugin.Cloud 
-Settings.LocalFileBackupPlugin.Cloud.UseS3Storage 
-Settings.LocalFileBackupPlugin.Cloud.S3ServiceURL 
-Settings.LocalFileBackupPlugin.Cloud.S3AuthenticationRegion 
-Settings.LocalFileBackupPlugin.Cloud.S3BucketName 
-Settings.LocalFileBackupPlugin.Cloud.S3AccessKey 
-Settings.LocalFileBackupPlugin.Cloud.S3SecretKey 
-Settings.LocalFileBackupPlugin.Cloud.S3UploadMode 
-Settings.LocalFileBackupPlugin.Cloud.S3StorageClass 
-Settings.steamcmdplugin 
-Settings.steamcmdplugin.SteamWorkshop 
-Settings.steamcmdplugin.SteamWorkshop.WorkshopItemIDs 
-Settings.steamcmdplugin.SteamUpdateSettings 
-Settings.steamcmdplugin.SteamUpdateSettings.AutomaticallyRetryOnFailure 
-Settings.steamcmdplugin.SteamUpdateSettings.AutomaticRetryLimit 
-Settings.steamcmdplugin.SteamUpdateSettings.UpdateCheckMethod 
-Settings.steamcmdplugin.SteamUpdateSettings.SteamCMDBetaPassword 
-Settings.steamcmdplugin.SteamUpdateSettings.ThrottleDownloadSpeed 
-Settings.steamcmdplugin.SteamUpdateSettings.KeepSteamCMDScripts 
-ADS 
-ADS.DatastoreManagement 
-ADS.DatastoreManagement.ManageDatastores 
-ADS.TemplateManagement 
-ADS.TemplateManagement.ManageTemplates 
-ADS.InstanceManagement 
-ADS.InstanceManagement.RegisterToController 
-ADS.InstanceManagement.CreateInstance 
-ADS.InstanceManagement.SuspendInstances 
-ADS.InstanceManagement.UpgradeInstances 
-ADS.InstanceManagement.StopInstances 
-ADS.InstanceManagement.DeleteInstances 
-ADS.InstanceManagement.StartInstances 
-ADS.InstanceManagement.AttachRemoteADSInstance 
-ADS.InstanceManagement.RemoveRemoteADSInstance 
-ADS.InstanceManagement.EditRemoteTargets 
-ADS.InstanceManagement.Convert 
-ADS.InstanceManagement.Reconfigure 
-ADS.InstanceManagement.RestartInstances 
-ADS.InstanceManagement.RefreshConfiguration 
-ADS.InstanceManagement.RefreshRemoteConfigStores 
-ADS.InstanceManagement.ManageSuspendedInstances 
-FileManager 
-FileManager.FileManager 
-FileManager.FileManager.CreateArchive 
-FileManager.FileManager.ExtractArchive 
-FileManager.FileManager.BrowseFiles 
-FileManager.FileManager.DownloadFiles 
-FileManager.FileManager.UploadFiles 
-FileManager.FileManager.RenameFiles 
-FileManager.FileManager.ChangeFileExtension 
-FileManager.FileManager.CopyFiles 
-FileManager.FileManager.TrashFiles 
-FileManager.FileManager.TrashDirectories 
-FileManager.FileManager.EmptyTrash 
-FileManager.FileManager.CreateDirectory 
-FileManager.FileManager.RenameDirectories 
-FileManager.FileManager.ChangeBackupExclusions 
-FileManager.FileManager.DownloadFromURL 
-FileManager.FileManager.ModifyAMPConfigFiles 
-FileManager.FileManager.ConnectViaSFTP 
-LocalFileBackup 
-LocalFileBackup.Backup 
-LocalFileBackup.Backup.ViewBackupsList 
-LocalFileBackup.Backup.CreateBackup 
-LocalFileBackup.Backup.DeleteBackup 
-LocalFileBackup.Backup.RestoreBackup 
-LocalFileBackup.Backup.ToggleStickiness 
-LocalFileBackup.Backup.ArchiveBackup 
-LocalFileBackup.Backup.TransferBackup 
-Core 
-Core.AuditLog 
-Core.AuditLog.ViewAuditLog 
-Core.Special 
-Core.Special.CancelOtherUsersTasks 
-Core.Special.ViewOtherUsersTasks 
-Core.Special.UpdateAMPInstance 
-Core.Special.UseDevMethods 
-Core.Special.RestartAMP 
-Core.Special.Diagnostics 
-Core.Special.UpgradeAMP 
-Core.Special.BypassSettingValueLimits 
-Core.Special.QueryLicenceInformation 
-Core.Special.ActivateAMP 
-Core.RoleManagement 
-Core.RoleManagement.ViewRoles 
-Core.RoleManagement.CreateRole 
-Core.RoleManagement.DeleteRoles 
-Core.RoleManagement.EditRoleInfo 
-Core.RoleManagement.EditRolePermissions 
-Core.RoleManagement.CreateCommonRoles 
-Core.Scheduler 
-Core.Scheduler.ViewSchedule 
-Core.Scheduler.CreateTrigger 
-Core.Scheduler.EditTrigger 
-Core.Scheduler.CreateTask 
-Core.Scheduler.DeleteTask 
-Core.Scheduler.DeleteTrigger 
-Core.Scheduler.EditTask 
-Core.Scheduler.EditOtherUsersTasks 
-Core.UserManagement 
-Core.UserManagement.ChangeRoleMembership 
-Core.UserManagement.UpdateUserInfo 
-Core.UserManagement.UpdateOwnAccount 
-Core.UserManagement.DeleteUser 
-Core.UserManagement.ResetUserPassword 
-Core.UserManagement.CreateNewUser 
-Core.UserManagement.ViewOtherUsersSessions 
-Core.UserManagement.EndUserSessions 
-Core.UserManagement.ViewUserInfo 
-Core.UserManagement.AccessExternalPermissions 
-Core.AppManagement 
-Core.AppManagement.StartApplication 
-Core.AppManagement.StopApplication 
-Core.AppManagement.RestartApplication 
-Core.AppManagement.UpdateApplication 
-Core.AppManagement.SendConsoleInput 
-Core.AppManagement.ReadConsole 
-Instances 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Start 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Stop 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Restart 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Update 
-Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Manage 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Start 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Stop 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Restart 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Update 
-Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Manage 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Start 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Stop 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Restart 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Update 
-Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Manage 
+Settings 
+Settings.Core 
+Settings.Core.Security 
+Settings.Core.Security.EnablePassthruAuth 
+Settings.Core.Security.AuthFailureTimeWindow 
+Settings.Core.Security.AuthFailureAttemptsInWindow 
+Settings.Core.Security.TwoFactorMode 
+Settings.Core.Security.RequireSessionIPStickiness 
+Settings.Core.Security.AllowUserPasswords 
+Settings.Core.Webserver 
+Settings.Core.Webserver.APIRateLimit 
+Settings.Core.Webserver.AllowGETForAPIEndpoints 
+Settings.Core.Webserver.CORSOrigin 
+Settings.Core.Webserver.DisableCompression 
+Settings.Core.Login 
+Settings.Core.Login.UseAuthServer 
+Settings.Core.Login.AuthServerURL 
+Settings.Core.Branding 
+Settings.Core.Branding.DisplayBranding 
+Settings.Core.Branding.PageTitle 
+Settings.Core.Branding.CompanyName 
+Settings.Core.Branding.WelcomeMessage 
+Settings.Core.Branding.BrandingMessage 
+Settings.Core.Branding.ShortBrandingMessage 
+Settings.Core.Branding.URL 
+Settings.Core.Branding.SupportURL 
+Settings.Core.Branding.SupportText 
+Settings.Core.Branding.SubmitTicketURL 
+Settings.Core.Branding.LogoURL 
+Settings.Core.Branding.BackgroundURL 
+Settings.Core.Branding.SplashFrameURL 
+Settings.Core.Branding.ForgotPasswordURL 
+Settings.Core.AMP 
+Settings.Core.AMP.ScheduleOffsetSeconds 
+Settings.Core.AMP.AppStartupMode 
+Settings.Core.AMP.FirstStart 
+Settings.Core.AMP.MapAllPluginStores 
+Settings.Core.AMP.Theme 
+Settings.Core.AMP.ShowHelpOnStatus 
+Settings.Core.Monitoring 
+Settings.Core.Monitoring.UseMulticoreCPUCalc 
+Settings.Core.Monitoring.IgnoreSMTCores 
+Settings.Core.Monitoring.ConsoleScrollback 
+Settings.Core.Monitoring.LogLevel 
+Settings.Core.Monitoring.FullMetricsGathering 
+Settings.Core.Monitoring.ReportPhysicalMemoryAsTotal 
+Settings.Core.Monitoring.MetricsPollInterval 
+Settings.Core.Privacy 
+Settings.Core.Privacy.PrivacySettingsSet 
+Settings.Core.Privacy.AutoReportFatalExceptions 
+Settings.Core.Privacy.AllowAnalytics 
+Settings.ADSModule 
+Settings.ADSModule.Limits 
+Settings.ADSModule.Limits.InstanceLimit 
+Settings.ADSModule.Limits.CreateLocalInstances 
+Settings.ADSModule.Defaults 
+Settings.ADSModule.Defaults.NewInstanceKey 
+Settings.ADSModule.Defaults.DefaultSettings 
+Settings.ADSModule.Defaults.DefaultReleaseStream 
+Settings.ADSModule.Defaults.UseDocker 
+Settings.ADSModule.Defaults.DefaultAuthServerURL 
+Settings.ADSModule.Defaults.PropagateAuthServer 
+Settings.ADSModule.Defaults.PropogateRepos 
+Settings.ADSModule.Defaults.UseOverlays 
+Settings.ADSModule.Defaults.MatchVersion 
+Settings.ADSModule.Defaults.DefaultPostCreate 
+Settings.ADSModule.Defaults.ExcludeFromFirewall 
+Settings.ADSModule.ADS 
+Settings.ADSModule.ADS.AutoReactivate 
+Settings.ADSModule.ADS.Mode 
+Settings.ADSModule.ADS.AutostartInstances 
+Settings.ADSModule.ADS.InstanceStartDelay 
+Settings.ADSModule.ADS.ConfigurationRepositories 
+Settings.ADSModule.ADS.ShowDeprecated 
+Settings.ADSModule.Network 
+Settings.ADSModule.Network.DefaultIPBinding 
+Settings.ADSModule.Network.DefaultAppIPBinding 
+Settings.ADSModule.Network.DockerExternalIPBinding 
+Settings.ADSModule.Network.AMPPortRanges 
+Settings.ADSModule.Network.PortAssignment 
+Settings.ADSModule.Network.AppPortRanges 
+Settings.ADSModule.Network.AppPortExclusions 
+Settings.ADSModule.Network.MetricsServerPort 
+Settings.ADSModule.Network.UseDockerHostNetwork 
+Settings.ADSModule.Network.UseTraefik 
+Settings.ADSModule.Network.TraefikNetworkName 
+Settings.ADSModule.Network.TraefikDomainWildcard 
+Settings.ADSModule.Network.AccessMode 
+Settings.ADSModule.Network.BaseURL 
+Settings.FileManagerPlugin 
+Settings.FileManagerPlugin.Security 
+Settings.FileManagerPlugin.Security.RestrictUploadExtensions 
+Settings.FileManagerPlugin.Security.RestrictDownloadExtensions 
+Settings.FileManagerPlugin.Security.DownloadableExtensions 
+Settings.FileManagerPlugin.Security.UploadableExtensions 
+Settings.FileManagerPlugin.Security.AllowExtensionChange 
+Settings.FileManagerPlugin.Security.AllowArchiveOperations 
+Settings.FileManagerPlugin.Security.OnlyExtractUploadableExtensionsFromArchives 
+Settings.FileManagerPlugin.Security.HoneypotSFTPLogins 
+Settings.FileManagerPlugin.FileManager 
+Settings.FileManagerPlugin.FileManager.AdditionalVirtualDirectories 
+Settings.FileManagerPlugin.FileManager.FastFileTransfers 
+Settings.FileManagerPlugin.SFTP 
+Settings.FileManagerPlugin.SFTP.EnableCompression 
+Settings.EmailSenderPlugin 
+Settings.EmailSenderPlugin.SMTP 
+Settings.EmailSenderPlugin.SMTP.UseSSL 
+Settings.EmailSenderPlugin.SMTP.Host 
+Settings.EmailSenderPlugin.SMTP.Port 
+Settings.EmailSenderPlugin.SMTP.Username 
+Settings.EmailSenderPlugin.SMTP.Password 
+Settings.EmailSenderPlugin.SMTP.EmailFrom 
+Settings.WebRequestPlugin 
+Settings.WebRequestPlugin.WebhookLogins 
+Settings.WebRequestPlugin.WebhookLogins.PushbulletAccessToken 
+Settings.LocalFileBackupPlugin 
+Settings.LocalFileBackupPlugin.Limits 
+Settings.LocalFileBackupPlugin.Limits.MaxTotalSizeMB 
+Settings.LocalFileBackupPlugin.Limits.MaxIndividualSizeMB 
+Settings.LocalFileBackupPlugin.Limits.MaxBackupCount 
+Settings.LocalFileBackupPlugin.Limits.ReplacePolicy 
+Settings.LocalFileBackupPlugin.Limits.Compression 
+Settings.LocalFileBackupPlugin.Cloud 
+Settings.LocalFileBackupPlugin.Cloud.UseS3Storage 
+Settings.LocalFileBackupPlugin.Cloud.S3ServiceURL 
+Settings.LocalFileBackupPlugin.Cloud.S3AuthenticationRegion 
+Settings.LocalFileBackupPlugin.Cloud.S3BucketName 
+Settings.LocalFileBackupPlugin.Cloud.S3AccessKey 
+Settings.LocalFileBackupPlugin.Cloud.S3SecretKey 
+Settings.LocalFileBackupPlugin.Cloud.S3UploadMode 
+Settings.LocalFileBackupPlugin.Cloud.S3StorageClass 
+Settings.steamcmdplugin 
+Settings.steamcmdplugin.SteamWorkshop 
+Settings.steamcmdplugin.SteamWorkshop.WorkshopItemIDs 
+Settings.steamcmdplugin.SteamUpdateSettings 
+Settings.steamcmdplugin.SteamUpdateSettings.AutomaticallyRetryOnFailure 
+Settings.steamcmdplugin.SteamUpdateSettings.AutomaticRetryLimit 
+Settings.steamcmdplugin.SteamUpdateSettings.UpdateCheckMethod 
+Settings.steamcmdplugin.SteamUpdateSettings.SteamCMDBetaPassword 
+Settings.steamcmdplugin.SteamUpdateSettings.ThrottleDownloadSpeed 
+Settings.steamcmdplugin.SteamUpdateSettings.KeepSteamCMDScripts 
+ADS 
+ADS.DatastoreManagement 
+ADS.DatastoreManagement.ManageDatastores 
+ADS.TemplateManagement 
+ADS.TemplateManagement.ManageTemplates 
+ADS.InstanceManagement 
+ADS.InstanceManagement.RegisterToController 
+ADS.InstanceManagement.CreateInstance 
+ADS.InstanceManagement.SuspendInstances 
+ADS.InstanceManagement.UpgradeInstances 
+ADS.InstanceManagement.StopInstances 
+ADS.InstanceManagement.DeleteInstances 
+ADS.InstanceManagement.StartInstances 
+ADS.InstanceManagement.AttachRemoteADSInstance 
+ADS.InstanceManagement.RemoveRemoteADSInstance 
+ADS.InstanceManagement.EditRemoteTargets 
+ADS.InstanceManagement.Convert 
+ADS.InstanceManagement.Reconfigure 
+ADS.InstanceManagement.RestartInstances 
+ADS.InstanceManagement.RefreshConfiguration 
+ADS.InstanceManagement.RefreshRemoteConfigStores 
+ADS.InstanceManagement.ManageSuspendedInstances 
+FileManager 
+FileManager.FileManager 
+FileManager.FileManager.CreateArchive 
+FileManager.FileManager.ExtractArchive 
+FileManager.FileManager.BrowseFiles 
+FileManager.FileManager.DownloadFiles 
+FileManager.FileManager.UploadFiles 
+FileManager.FileManager.RenameFiles 
+FileManager.FileManager.ChangeFileExtension 
+FileManager.FileManager.CopyFiles 
+FileManager.FileManager.TrashFiles 
+FileManager.FileManager.TrashDirectories 
+FileManager.FileManager.EmptyTrash 
+FileManager.FileManager.CreateDirectory 
+FileManager.FileManager.RenameDirectories 
+FileManager.FileManager.ChangeBackupExclusions 
+FileManager.FileManager.DownloadFromURL 
+FileManager.FileManager.ModifyAMPConfigFiles 
+FileManager.FileManager.ConnectViaSFTP 
+LocalFileBackup 
+LocalFileBackup.Backup 
+LocalFileBackup.Backup.ViewBackupsList 
+LocalFileBackup.Backup.CreateBackup 
+LocalFileBackup.Backup.DeleteBackup 
+LocalFileBackup.Backup.RestoreBackup 
+LocalFileBackup.Backup.ToggleStickiness 
+LocalFileBackup.Backup.ArchiveBackup 
+LocalFileBackup.Backup.TransferBackup 
+Core 
+Core.AuditLog 
+Core.AuditLog.ViewAuditLog 
+Core.Special 
+Core.Special.CancelOtherUsersTasks 
+Core.Special.ViewOtherUsersTasks 
+Core.Special.UpdateAMPInstance 
+Core.Special.UseDevMethods 
+Core.Special.RestartAMP 
+Core.Special.Diagnostics 
+Core.Special.UpgradeAMP 
+Core.Special.BypassSettingValueLimits 
+Core.Special.QueryLicenceInformation 
+Core.Special.ActivateAMP 
+Core.RoleManagement 
+Core.RoleManagement.ViewRoles 
+Core.RoleManagement.CreateRole 
+Core.RoleManagement.DeleteRoles 
+Core.RoleManagement.EditRoleInfo 
+Core.RoleManagement.EditRolePermissions 
+Core.RoleManagement.CreateCommonRoles 
+Core.Scheduler 
+Core.Scheduler.ViewSchedule 
+Core.Scheduler.CreateTrigger 
+Core.Scheduler.EditTrigger 
+Core.Scheduler.CreateTask 
+Core.Scheduler.DeleteTask 
+Core.Scheduler.DeleteTrigger 
+Core.Scheduler.EditTask 
+Core.Scheduler.EditOtherUsersTasks 
+Core.UserManagement 
+Core.UserManagement.ChangeRoleMembership 
+Core.UserManagement.UpdateUserInfo 
+Core.UserManagement.UpdateOwnAccount 
+Core.UserManagement.DeleteUser 
+Core.UserManagement.ResetUserPassword 
+Core.UserManagement.CreateNewUser 
+Core.UserManagement.ViewOtherUsersSessions 
+Core.UserManagement.EndUserSessions 
+Core.UserManagement.ViewUserInfo 
+Core.UserManagement.AccessExternalPermissions 
+Core.AppManagement 
+Core.AppManagement.StartApplication 
+Core.AppManagement.StopApplication 
+Core.AppManagement.RestartApplication 
+Core.AppManagement.UpdateApplication 
+Core.AppManagement.SendConsoleInput 
+Core.AppManagement.ReadConsole 
+Instances 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Start 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Stop 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Restart 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Update 
+Instances.0009776e-0d48-44ff-93de-b3852ce3fdad.Manage 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Start 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Stop 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Restart 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Update 
+Instances.f45a0859-8e0b-4e53-9feb-3ff77fd89268.Manage 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Start 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Stop 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Restart 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Update 
+Instances.5777fd47-4092-4f5c-9223-4d8f5c934e81.Manage
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/docs/setting_nodes.md` & `cubecoders_amp_api_wrapper-0.0.41b0/docs/setting_nodes.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-Core.Webserver.EnableWebSockets 
-Core.Webserver.EnableFetchPostEndpoints 
-Core.Webserver.APIRateLimit 
-Core.Webserver.AllowGETForAPIEndpoints 
-Core.Webserver.CORSOrigin 
-Core.Webserver.DisableCompression 
-Core.AMP.ScheduleOffsetSeconds 
-Core.AMP.AppStartupMode 
-Core.AMP.FirstStart 
-Core.AMP.ShutdownProperly 
-Core.AMP.SafeMode 
-Core.AMP.PreviousVersion 
-Core.AMP.StoreIPAddressesAsMACAddresses 
-Core.AMP.MapAllPluginStores 
-Core.AMP.Theme 
-Core.AMP.ShowHelpOnStatus 
-Core.Branding.DisplayBranding 
-Core.Branding.PageTitle 
-Core.Branding.CompanyName 
-Core.Branding.WelcomeMessage 
-Core.Branding.BrandingMessage 
-Core.Branding.ShortBrandingMessage 
-Core.Branding.URL 
-Core.Branding.SupportURL 
-Core.Branding.SupportText 
-Core.Branding.SubmitTicketURL 
-Core.Branding.LogoURL 
-Core.Branding.BackgroundURL 
-Core.Branding.SplashFrameURL 
-Core.Branding.ForgotPasswordURL 
-LocalFileBackupPlugin.Cloud.UseS3Storage 
-LocalFileBackupPlugin.Cloud.S3ServiceURL 
-LocalFileBackupPlugin.Cloud.S3AuthenticationRegion 
-LocalFileBackupPlugin.Cloud.S3BucketName 
-LocalFileBackupPlugin.Cloud.S3AccessKey 
-LocalFileBackupPlugin.Cloud.S3SecretKey 
-LocalFileBackupPlugin.Cloud.S3UploadMode 
-LocalFileBackupPlugin.Cloud.S3StorageClass 
-EmailSenderPlugin.SMTP.UseSSL 
-EmailSenderPlugin.SMTP.Host 
-EmailSenderPlugin.SMTP.Port 
-EmailSenderPlugin.SMTP.Username 
-EmailSenderPlugin.SMTP.Password 
-EmailSenderPlugin.SMTP.EmailFrom 
-WebRequestPlugin.WebhookLogins.PushbulletAccessToken 
-FileManagerPlugin.FileManager.BasePath 
-FileManagerPlugin.FileManager.AdditionalVirtualDirectories 
-FileManagerPlugin.FileManager.FastFileTransfers 
-ADSModule.ADS.AutoReactivate 
-ADSModule.ADS.Mode 
-ADSModule.ADS.AutostartInstances 
-ADSModule.ADS.InstanceStartDelay 
-ADSModule.ADS.IgnoreCompatibility 
-ADSModule.ADS.ConfigurationRepositories 
-ADSModule.ADS.ShowDeprecated 
-Core.Login.UseAuthServer 
-Core.Login.AuthServerURL 
-Core.Monitoring.UseMulticoreCPUCalc 
-Core.Monitoring.IgnoreSMTCores 
-Core.Monitoring.ConsoleScrollback 
-Core.Monitoring.LogLevel 
-Core.Monitoring.FullMetricsGathering 
-Core.Monitoring.ReportPhysicalMemoryAsTotal 
-Core.Monitoring.MetricsPollInterval 
-ADSModule.Networking.DefaultIPBinding 
-ADSModule.Networking.DefaultAppIPBinding 
-ADSModule.Networking.DockerExternalIPBinding 
-ADSModule.Networking.AMPPortRanges 
-ADSModule.Networking.PortAssignment 
-ADSModule.Networking.AppPortRanges 
-ADSModule.Networking.AppPortExclusions 
-ADSModule.Networking.MetricsServerPort 
-ADSModule.Networking.UseDockerHostNetwork 
-ADSModule.Networking.UseTraefik 
-ADSModule.Networking.TraefikNetworkName 
-ADSModule.Networking.TraefikDomainWildcard 
-ADSModule.Networking.AccessMode 
-ADSModule.Networking.BaseURL 
-ADSModule.Defaults.NewInstanceKey 
-ADSModule.Defaults.DefaultSettings 
-ADSModule.Defaults.DefaultReleaseStream 
-ADSModule.Defaults.UseDocker 
-ADSModule.Defaults.CreateAsShared 
-ADSModule.Defaults.DefaultAuthServerURL 
-ADSModule.Defaults.PropagateAuthServer 
-ADSModule.Defaults.PropogateRepos 
-ADSModule.Defaults.UseOverlays 
-ADSModule.Defaults.OverlayPath 
-ADSModule.Defaults.MatchVersion 
-ADSModule.Defaults.DefaultPostCreate 
-ADSModule.Defaults.ExcludeFromFirewall 
-ADSModule.Limits.InstanceLimit 
-ADSModule.Limits.CreateLocalInstances 
-LocalFileBackupPlugin.Limits.MaxTotalSizeMB 
-LocalFileBackupPlugin.Limits.MaxIndividualSizeMB 
-LocalFileBackupPlugin.Limits.MaxBackupCount 
-LocalFileBackupPlugin.Limits.ReplacePolicy 
-LocalFileBackupPlugin.Limits.Compression 
-Core.Security.EnablePassthruAuth 
-Core.Security.AuthFailureTimeWindow 
-Core.Security.AuthFailureAttemptsInWindow 
-Core.Security.TwoFactorMode 
-Core.Security.RequireSessionIPStickiness 
-Core.Security.AllowUserPasswords 
-Core.Privacy.PrivacySettingsSet 
-Core.Privacy.AutoReportFatalExceptions 
-Core.Privacy.AllowAnalytics 
-FileManagerPlugin.Security.RestrictUploadExtensions 
-FileManagerPlugin.Security.RestrictDownloadExtensions 
-FileManagerPlugin.Security.DownloadableExtensions 
-FileManagerPlugin.Security.UploadableExtensions 
-FileManagerPlugin.Security.AllowExtensionChange 
-FileManagerPlugin.Security.AllowArchiveOperations 
-FileManagerPlugin.Security.OnlyExtractUploadableExtensionsFromArchives 
-FileManagerPlugin.Security.HoneypotSFTPLogins 
-FileManagerPlugin.SFTP.SFTPEnabled 
-FileManagerPlugin.SFTP.SFTPPortNumber 
-FileManagerPlugin.SFTP.EnableCompression 
-steamcmdplugin.SteamWorkshop.WorkshopItemIDs 
-steamcmdplugin.SteamUpdateSettings.AutomaticallyRetryOnFailure 
-steamcmdplugin.SteamUpdateSettings.AutomaticRetryLimit 
-steamcmdplugin.SteamUpdateSettings.UpdateCheckMethod 
-steamcmdplugin.SteamUpdateSettings.SteamCMDBetaPassword 
-steamcmdplugin.SteamUpdateSettings.ThrottleDownloadSpeed 
-steamcmdplugin.SteamUpdateSettings.KeepSteamCMDScripts 
+Core.Webserver.EnableWebSockets 
+Core.Webserver.EnableFetchPostEndpoints 
+Core.Webserver.APIRateLimit 
+Core.Webserver.AllowGETForAPIEndpoints 
+Core.Webserver.CORSOrigin 
+Core.Webserver.DisableCompression 
+Core.AMP.ScheduleOffsetSeconds 
+Core.AMP.AppStartupMode 
+Core.AMP.FirstStart 
+Core.AMP.ShutdownProperly 
+Core.AMP.SafeMode 
+Core.AMP.PreviousVersion 
+Core.AMP.StoreIPAddressesAsMACAddresses 
+Core.AMP.MapAllPluginStores 
+Core.AMP.Theme 
+Core.AMP.ShowHelpOnStatus 
+Core.Branding.DisplayBranding 
+Core.Branding.PageTitle 
+Core.Branding.CompanyName 
+Core.Branding.WelcomeMessage 
+Core.Branding.BrandingMessage 
+Core.Branding.ShortBrandingMessage 
+Core.Branding.URL 
+Core.Branding.SupportURL 
+Core.Branding.SupportText 
+Core.Branding.SubmitTicketURL 
+Core.Branding.LogoURL 
+Core.Branding.BackgroundURL 
+Core.Branding.SplashFrameURL 
+Core.Branding.ForgotPasswordURL 
+LocalFileBackupPlugin.Cloud.UseS3Storage 
+LocalFileBackupPlugin.Cloud.S3ServiceURL 
+LocalFileBackupPlugin.Cloud.S3AuthenticationRegion 
+LocalFileBackupPlugin.Cloud.S3BucketName 
+LocalFileBackupPlugin.Cloud.S3AccessKey 
+LocalFileBackupPlugin.Cloud.S3SecretKey 
+LocalFileBackupPlugin.Cloud.S3UploadMode 
+LocalFileBackupPlugin.Cloud.S3StorageClass 
+EmailSenderPlugin.SMTP.UseSSL 
+EmailSenderPlugin.SMTP.Host 
+EmailSenderPlugin.SMTP.Port 
+EmailSenderPlugin.SMTP.Username 
+EmailSenderPlugin.SMTP.Password 
+EmailSenderPlugin.SMTP.EmailFrom 
+WebRequestPlugin.WebhookLogins.PushbulletAccessToken 
+FileManagerPlugin.FileManager.BasePath 
+FileManagerPlugin.FileManager.AdditionalVirtualDirectories 
+FileManagerPlugin.FileManager.FastFileTransfers 
+ADSModule.ADS.AutoReactivate 
+ADSModule.ADS.Mode 
+ADSModule.ADS.AutostartInstances 
+ADSModule.ADS.InstanceStartDelay 
+ADSModule.ADS.IgnoreCompatibility 
+ADSModule.ADS.ConfigurationRepositories 
+ADSModule.ADS.ShowDeprecated 
+Core.Login.UseAuthServer 
+Core.Login.AuthServerURL 
+Core.Monitoring.UseMulticoreCPUCalc 
+Core.Monitoring.IgnoreSMTCores 
+Core.Monitoring.ConsoleScrollback 
+Core.Monitoring.LogLevel 
+Core.Monitoring.FullMetricsGathering 
+Core.Monitoring.ReportPhysicalMemoryAsTotal 
+Core.Monitoring.MetricsPollInterval 
+ADSModule.Networking.DefaultIPBinding 
+ADSModule.Networking.DefaultAppIPBinding 
+ADSModule.Networking.DockerExternalIPBinding 
+ADSModule.Networking.AMPPortRanges 
+ADSModule.Networking.PortAssignment 
+ADSModule.Networking.AppPortRanges 
+ADSModule.Networking.AppPortExclusions 
+ADSModule.Networking.MetricsServerPort 
+ADSModule.Networking.UseDockerHostNetwork 
+ADSModule.Networking.UseTraefik 
+ADSModule.Networking.TraefikNetworkName 
+ADSModule.Networking.TraefikDomainWildcard 
+ADSModule.Networking.AccessMode 
+ADSModule.Networking.BaseURL 
+ADSModule.Defaults.NewInstanceKey 
+ADSModule.Defaults.DefaultSettings 
+ADSModule.Defaults.DefaultReleaseStream 
+ADSModule.Defaults.UseDocker 
+ADSModule.Defaults.CreateAsShared 
+ADSModule.Defaults.DefaultAuthServerURL 
+ADSModule.Defaults.PropagateAuthServer 
+ADSModule.Defaults.PropogateRepos 
+ADSModule.Defaults.UseOverlays 
+ADSModule.Defaults.OverlayPath 
+ADSModule.Defaults.MatchVersion 
+ADSModule.Defaults.DefaultPostCreate 
+ADSModule.Defaults.ExcludeFromFirewall 
+ADSModule.Limits.InstanceLimit 
+ADSModule.Limits.CreateLocalInstances 
+LocalFileBackupPlugin.Limits.MaxTotalSizeMB 
+LocalFileBackupPlugin.Limits.MaxIndividualSizeMB 
+LocalFileBackupPlugin.Limits.MaxBackupCount 
+LocalFileBackupPlugin.Limits.ReplacePolicy 
+LocalFileBackupPlugin.Limits.Compression 
+Core.Security.EnablePassthruAuth 
+Core.Security.AuthFailureTimeWindow 
+Core.Security.AuthFailureAttemptsInWindow 
+Core.Security.TwoFactorMode 
+Core.Security.RequireSessionIPStickiness 
+Core.Security.AllowUserPasswords 
+Core.Privacy.PrivacySettingsSet 
+Core.Privacy.AutoReportFatalExceptions 
+Core.Privacy.AllowAnalytics 
+FileManagerPlugin.Security.RestrictUploadExtensions 
+FileManagerPlugin.Security.RestrictDownloadExtensions 
+FileManagerPlugin.Security.DownloadableExtensions 
+FileManagerPlugin.Security.UploadableExtensions 
+FileManagerPlugin.Security.AllowExtensionChange 
+FileManagerPlugin.Security.AllowArchiveOperations 
+FileManagerPlugin.Security.OnlyExtractUploadableExtensionsFromArchives 
+FileManagerPlugin.Security.HoneypotSFTPLogins 
+FileManagerPlugin.SFTP.SFTPEnabled 
+FileManagerPlugin.SFTP.SFTPPortNumber 
+FileManagerPlugin.SFTP.EnableCompression 
+steamcmdplugin.SteamWorkshop.WorkshopItemIDs 
+steamcmdplugin.SteamUpdateSettings.AutomaticallyRetryOnFailure 
+steamcmdplugin.SteamUpdateSettings.AutomaticRetryLimit 
+steamcmdplugin.SteamUpdateSettings.UpdateCheckMethod 
+steamcmdplugin.SteamUpdateSettings.SteamCMDBetaPassword 
+steamcmdplugin.SteamUpdateSettings.ThrottleDownloadSpeed 
+steamcmdplugin.SteamUpdateSettings.KeepSteamCMDScripts
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/docs/setting_nodes.txt` & `cubecoders_amp_api_wrapper-0.0.41b0/docs/setting_nodes.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-Core.Webserver.EnableWebSockets 
-Core.Webserver.EnableFetchPostEndpoints 
-Core.Webserver.APIRateLimit 
-Core.Webserver.AllowGETForAPIEndpoints 
-Core.Webserver.CORSOrigin 
-Core.Webserver.DisableCompression 
-Core.AMP.ScheduleOffsetSeconds 
-Core.AMP.AppStartupMode 
-Core.AMP.FirstStart 
-Core.AMP.ShutdownProperly 
-Core.AMP.SafeMode 
-Core.AMP.PreviousVersion 
-Core.AMP.StoreIPAddressesAsMACAddresses 
-Core.AMP.MapAllPluginStores 
-Core.AMP.Theme 
-Core.AMP.ShowHelpOnStatus 
-Core.Branding.DisplayBranding 
-Core.Branding.PageTitle 
-Core.Branding.CompanyName 
-Core.Branding.WelcomeMessage 
-Core.Branding.BrandingMessage 
-Core.Branding.ShortBrandingMessage 
-Core.Branding.URL 
-Core.Branding.SupportURL 
-Core.Branding.SupportText 
-Core.Branding.SubmitTicketURL 
-Core.Branding.LogoURL 
-Core.Branding.BackgroundURL 
-Core.Branding.SplashFrameURL 
-Core.Branding.ForgotPasswordURL 
-LocalFileBackupPlugin.Cloud.UseS3Storage 
-LocalFileBackupPlugin.Cloud.S3ServiceURL 
-LocalFileBackupPlugin.Cloud.S3AuthenticationRegion 
-LocalFileBackupPlugin.Cloud.S3BucketName 
-LocalFileBackupPlugin.Cloud.S3AccessKey 
-LocalFileBackupPlugin.Cloud.S3SecretKey 
-LocalFileBackupPlugin.Cloud.S3UploadMode 
-LocalFileBackupPlugin.Cloud.S3StorageClass 
-EmailSenderPlugin.SMTP.UseSSL 
-EmailSenderPlugin.SMTP.Host 
-EmailSenderPlugin.SMTP.Port 
-EmailSenderPlugin.SMTP.Username 
-EmailSenderPlugin.SMTP.Password 
-EmailSenderPlugin.SMTP.EmailFrom 
-WebRequestPlugin.WebhookLogins.PushbulletAccessToken 
-FileManagerPlugin.FileManager.BasePath 
-FileManagerPlugin.FileManager.AdditionalVirtualDirectories 
-FileManagerPlugin.FileManager.FastFileTransfers 
-ADSModule.ADS.AutoReactivate 
-ADSModule.ADS.Mode 
-ADSModule.ADS.AutostartInstances 
-ADSModule.ADS.InstanceStartDelay 
-ADSModule.ADS.IgnoreCompatibility 
-ADSModule.ADS.ConfigurationRepositories 
-ADSModule.ADS.ShowDeprecated 
-Core.Login.UseAuthServer 
-Core.Login.AuthServerURL 
-Core.Monitoring.UseMulticoreCPUCalc 
-Core.Monitoring.IgnoreSMTCores 
-Core.Monitoring.ConsoleScrollback 
-Core.Monitoring.LogLevel 
-Core.Monitoring.FullMetricsGathering 
-Core.Monitoring.ReportPhysicalMemoryAsTotal 
-Core.Monitoring.MetricsPollInterval 
-ADSModule.Network.DefaultIPBinding 
-ADSModule.Network.DefaultAppIPBinding 
-ADSModule.Network.DockerExternalIPBinding 
-ADSModule.Network.AMPPortRanges 
-ADSModule.Network.PortAssignment 
-ADSModule.Network.AppPortRanges 
-ADSModule.Network.AppPortExclusions 
-ADSModule.Network.MetricsServerPort 
-ADSModule.Network.UseDockerHostNetwork 
-ADSModule.Network.UseTraefik 
-ADSModule.Network.TraefikNetworkName 
-ADSModule.Network.TraefikDomainWildcard 
-ADSModule.Network.AccessMode 
-ADSModule.Network.BaseURL 
-ADSModule.Defaults.NewInstanceKey 
-ADSModule.Defaults.DefaultSettings 
-ADSModule.Defaults.DefaultReleaseStream 
-ADSModule.Defaults.UseDocker 
-ADSModule.Defaults.CreateAsShared 
-ADSModule.Defaults.DefaultAuthServerURL 
-ADSModule.Defaults.PropagateAuthServer 
-ADSModule.Defaults.PropogateRepos 
-ADSModule.Defaults.UseOverlays 
-ADSModule.Defaults.OverlayPath 
-ADSModule.Defaults.MatchVersion 
-ADSModule.Defaults.DefaultPostCreate 
-ADSModule.Defaults.ExcludeFromFirewall 
-ADSModule.Limits.InstanceLimit 
-ADSModule.Limits.CreateLocalInstances 
-LocalFileBackupPlugin.Limits.MaxTotalSizeMB 
-LocalFileBackupPlugin.Limits.MaxIndividualSizeMB 
-LocalFileBackupPlugin.Limits.MaxBackupCount 
-LocalFileBackupPlugin.Limits.ReplacePolicy 
-LocalFileBackupPlugin.Limits.Compression 
-Core.Security.EnablePassthruAuth 
-Core.Security.AuthFailureTimeWindow 
-Core.Security.AuthFailureAttemptsInWindow 
-Core.Security.TwoFactorMode 
-Core.Security.RequireSessionIPStickiness 
-Core.Security.AllowUserPasswords 
-Core.Privacy.PrivacySettingsSet 
-Core.Privacy.AutoReportFatalExceptions 
-Core.Privacy.AllowAnalytics 
-FileManagerPlugin.Security.RestrictUploadExtensions 
-FileManagerPlugin.Security.RestrictDownloadExtensions 
-FileManagerPlugin.Security.DownloadableExtensions 
-FileManagerPlugin.Security.UploadableExtensions 
-FileManagerPlugin.Security.AllowExtensionChange 
-FileManagerPlugin.Security.AllowArchiveOperations 
-FileManagerPlugin.Security.OnlyExtractUploadableExtensionsFromArchives 
-FileManagerPlugin.Security.HoneypotSFTPLogins 
-FileManagerPlugin.SFTP.SFTPEnabled 
-FileManagerPlugin.SFTP.SFTPPortNumber 
-FileManagerPlugin.SFTP.EnableCompression 
-steamcmdplugin.SteamWorkshop.WorkshopItemIDs 
-steamcmdplugin.SteamUpdateSettings.AutomaticallyRetryOnFailure 
-steamcmdplugin.SteamUpdateSettings.AutomaticRetryLimit 
-steamcmdplugin.SteamUpdateSettings.UpdateCheckMethod 
-steamcmdplugin.SteamUpdateSettings.SteamCMDBetaPassword 
-steamcmdplugin.SteamUpdateSettings.ThrottleDownloadSpeed 
-steamcmdplugin.SteamUpdateSettings.KeepSteamCMDScripts 
+Core.Webserver.EnableWebSockets 
+Core.Webserver.EnableFetchPostEndpoints 
+Core.Webserver.APIRateLimit 
+Core.Webserver.AllowGETForAPIEndpoints 
+Core.Webserver.CORSOrigin 
+Core.Webserver.DisableCompression 
+Core.AMP.ScheduleOffsetSeconds 
+Core.AMP.AppStartupMode 
+Core.AMP.FirstStart 
+Core.AMP.ShutdownProperly 
+Core.AMP.SafeMode 
+Core.AMP.PreviousVersion 
+Core.AMP.StoreIPAddressesAsMACAddresses 
+Core.AMP.MapAllPluginStores 
+Core.AMP.Theme 
+Core.AMP.ShowHelpOnStatus 
+Core.Branding.DisplayBranding 
+Core.Branding.PageTitle 
+Core.Branding.CompanyName 
+Core.Branding.WelcomeMessage 
+Core.Branding.BrandingMessage 
+Core.Branding.ShortBrandingMessage 
+Core.Branding.URL 
+Core.Branding.SupportURL 
+Core.Branding.SupportText 
+Core.Branding.SubmitTicketURL 
+Core.Branding.LogoURL 
+Core.Branding.BackgroundURL 
+Core.Branding.SplashFrameURL 
+Core.Branding.ForgotPasswordURL 
+LocalFileBackupPlugin.Cloud.UseS3Storage 
+LocalFileBackupPlugin.Cloud.S3ServiceURL 
+LocalFileBackupPlugin.Cloud.S3AuthenticationRegion 
+LocalFileBackupPlugin.Cloud.S3BucketName 
+LocalFileBackupPlugin.Cloud.S3AccessKey 
+LocalFileBackupPlugin.Cloud.S3SecretKey 
+LocalFileBackupPlugin.Cloud.S3UploadMode 
+LocalFileBackupPlugin.Cloud.S3StorageClass 
+EmailSenderPlugin.SMTP.UseSSL 
+EmailSenderPlugin.SMTP.Host 
+EmailSenderPlugin.SMTP.Port 
+EmailSenderPlugin.SMTP.Username 
+EmailSenderPlugin.SMTP.Password 
+EmailSenderPlugin.SMTP.EmailFrom 
+WebRequestPlugin.WebhookLogins.PushbulletAccessToken 
+FileManagerPlugin.FileManager.BasePath 
+FileManagerPlugin.FileManager.AdditionalVirtualDirectories 
+FileManagerPlugin.FileManager.FastFileTransfers 
+ADSModule.ADS.AutoReactivate 
+ADSModule.ADS.Mode 
+ADSModule.ADS.AutostartInstances 
+ADSModule.ADS.InstanceStartDelay 
+ADSModule.ADS.IgnoreCompatibility 
+ADSModule.ADS.ConfigurationRepositories 
+ADSModule.ADS.ShowDeprecated 
+Core.Login.UseAuthServer 
+Core.Login.AuthServerURL 
+Core.Monitoring.UseMulticoreCPUCalc 
+Core.Monitoring.IgnoreSMTCores 
+Core.Monitoring.ConsoleScrollback 
+Core.Monitoring.LogLevel 
+Core.Monitoring.FullMetricsGathering 
+Core.Monitoring.ReportPhysicalMemoryAsTotal 
+Core.Monitoring.MetricsPollInterval 
+ADSModule.Network.DefaultIPBinding 
+ADSModule.Network.DefaultAppIPBinding 
+ADSModule.Network.DockerExternalIPBinding 
+ADSModule.Network.AMPPortRanges 
+ADSModule.Network.PortAssignment 
+ADSModule.Network.AppPortRanges 
+ADSModule.Network.AppPortExclusions 
+ADSModule.Network.MetricsServerPort 
+ADSModule.Network.UseDockerHostNetwork 
+ADSModule.Network.UseTraefik 
+ADSModule.Network.TraefikNetworkName 
+ADSModule.Network.TraefikDomainWildcard 
+ADSModule.Network.AccessMode 
+ADSModule.Network.BaseURL 
+ADSModule.Defaults.NewInstanceKey 
+ADSModule.Defaults.DefaultSettings 
+ADSModule.Defaults.DefaultReleaseStream 
+ADSModule.Defaults.UseDocker 
+ADSModule.Defaults.CreateAsShared 
+ADSModule.Defaults.DefaultAuthServerURL 
+ADSModule.Defaults.PropagateAuthServer 
+ADSModule.Defaults.PropogateRepos 
+ADSModule.Defaults.UseOverlays 
+ADSModule.Defaults.OverlayPath 
+ADSModule.Defaults.MatchVersion 
+ADSModule.Defaults.DefaultPostCreate 
+ADSModule.Defaults.ExcludeFromFirewall 
+ADSModule.Limits.InstanceLimit 
+ADSModule.Limits.CreateLocalInstances 
+LocalFileBackupPlugin.Limits.MaxTotalSizeMB 
+LocalFileBackupPlugin.Limits.MaxIndividualSizeMB 
+LocalFileBackupPlugin.Limits.MaxBackupCount 
+LocalFileBackupPlugin.Limits.ReplacePolicy 
+LocalFileBackupPlugin.Limits.Compression 
+Core.Security.EnablePassthruAuth 
+Core.Security.AuthFailureTimeWindow 
+Core.Security.AuthFailureAttemptsInWindow 
+Core.Security.TwoFactorMode 
+Core.Security.RequireSessionIPStickiness 
+Core.Security.AllowUserPasswords 
+Core.Privacy.PrivacySettingsSet 
+Core.Privacy.AutoReportFatalExceptions 
+Core.Privacy.AllowAnalytics 
+FileManagerPlugin.Security.RestrictUploadExtensions 
+FileManagerPlugin.Security.RestrictDownloadExtensions 
+FileManagerPlugin.Security.DownloadableExtensions 
+FileManagerPlugin.Security.UploadableExtensions 
+FileManagerPlugin.Security.AllowExtensionChange 
+FileManagerPlugin.Security.AllowArchiveOperations 
+FileManagerPlugin.Security.OnlyExtractUploadableExtensionsFromArchives 
+FileManagerPlugin.Security.HoneypotSFTPLogins 
+FileManagerPlugin.SFTP.SFTPEnabled 
+FileManagerPlugin.SFTP.SFTPPortNumber 
+FileManagerPlugin.SFTP.EnableCompression 
+steamcmdplugin.SteamWorkshop.WorkshopItemIDs 
+steamcmdplugin.SteamUpdateSettings.AutomaticallyRetryOnFailure 
+steamcmdplugin.SteamUpdateSettings.AutomaticRetryLimit 
+steamcmdplugin.SteamUpdateSettings.UpdateCheckMethod 
+steamcmdplugin.SteamUpdateSettings.SteamCMDBetaPassword 
+steamcmdplugin.SteamUpdateSettings.ThrottleDownloadSpeed 
+steamcmdplugin.SteamUpdateSettings.KeepSteamCMDScripts
```

### Comparing `cubecoders_amp_api_wrapper-0.0.40b0/setup.py` & `cubecoders_amp_api_wrapper-0.0.41b0/setup.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import re
-
-from setuptools import setup
-
-requirements: list[str] = []
-with open("./requirements.txt") as file:
-    requirements = file.read().splitlines()
-
-readme = ''
-with open('./README.md') as file:
-    readme: str = file.read()
-
-version = ''
-with open('./ampapi/__init__.py') as file:
-    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', file.read(), re.MULTILINE).group(1)  # type:ignore
-
-if not version:
-    raise RuntimeError("version is not set")
-
-packages = ["ampapi",]  # I believe this will affect the open #LN13
-
-setup(
-    name='cubecoders_amp_api_wrapper',
-    version=version,
-    description='A python wrapper for the AMP API by CubeCoders',
-    url='https://github.com/k8thekat/AMPAPI_Python',
-    author='Katelynn Cadwallader',
-    author_email='Cadwalladerkatelynn+AMPAPI@gmail.com',
-    license='GNU',
-    project_urls={
-        'GitHub': 'https://github.com/k8thekat/AMPAPI_Python',
-        'Changelog': 'https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md',
-    },
-    packages=packages,
-    package_data={
-        "docs": ["docs/api_spec.md", "docs/permission_nodes.md", "docs/setting_nodes.md"],
-        "license": ["LICENSE"],
-        "requirements": ["requirements.txt"],
-        "readme": ["README.md"],
-        "changelog": ["CHANGELOG.md"]},
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    install_requires=requirements,
-    python_requires='>=3.9.0',
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Framework :: AsyncIO',
-        'Topic :: Internet',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-        'Typing :: Typed',
-    ],
-)
+import re
+
+from setuptools import setup
+
+requirements: list[str] = []
+with open("./requirements.txt") as file:
+    requirements = file.read().splitlines()
+
+readme = ''
+with open('./README.md') as file:
+    readme: str = file.read()
+
+version = ''
+with open('./ampapi/__init__.py') as file:
+    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', file.read(), re.MULTILINE).group(1)  # type:ignore
+
+if not version:
+    raise RuntimeError("version is not set")
+
+packages = ["ampapi",]  # I believe this will affect the open #LN13
+
+setup(
+    name='cubecoders_amp_api_wrapper',
+    version=version,
+    description='A python wrapper for the AMP API by CubeCoders',
+    url='https://github.com/k8thekat/AMPAPI_Python',
+    author='Katelynn Cadwallader',
+    author_email='Cadwalladerkatelynn+AMPAPI@gmail.com',
+    license='GNU',
+    project_urls={
+        'GitHub': 'https://github.com/k8thekat/AMPAPI_Python',
+        'Changelog': 'https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md',
+    },
+    packages=packages,
+    package_data={
+        "docs": ["docs/api_spec.md", "docs/permission_nodes.md", "docs/setting_nodes.md"],
+        "license": ["LICENSE"],
+        "requirements": ["requirements.txt"],
+        "readme": ["README.md"],
+        "changelog": ["CHANGELOG.md"]},
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    install_requires=requirements,
+    python_requires='>=3.9.0',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Framework :: AsyncIO',
+        'Topic :: Internet',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Utilities',
+        'Typing :: Typed',
+    ],
+)
```

