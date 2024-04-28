# Comparing `tmp/zato_apitest-24.1.15.tar.gz` & `tmp/zato-apitest-24.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zato_apitest-24.1.15.tar", last modified: Sun Apr 28 07:55:10 2024, max compression
+gzip compressed data, was "zato-apitest-24.1.9.tar", last modified: Tue Mar 12 11:43:29 2024, max compression
```

## Comparing `zato_apitest-24.1.15.tar` & `zato-apitest-24.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 07:55:10.040561 zato_apitest-24.1.15/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.15/LICENSE.txt
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.15/MANIFEST.in
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-28 07:55:10.040561 zato_apitest-24.1.15/PKG-INFO
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.15/README.md
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.15/requirements.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-28 07:55:10.040561 zato_apitest-24.1.15/setup.cfg
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2635 2024-04-28 07:54:48.000000 zato_apitest-24.1.15/setup.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 07:55:10.036561 zato_apitest-24.1.15/src/
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 07:55:10.036561 zato_apitest-24.1.15/src/zato/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.15/src/zato/__init__.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 07:55:10.036561 zato_apitest-24.1.15/src/zato/apitest/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.15/src/zato/apitest/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4327 2024-04-28 07:51:04.000000 zato_apitest-24.1.15/src/zato/apitest/cli.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 07:55:10.036561 zato_apitest-24.1.15/src/zato/apitest/console/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.15/src/zato/apitest/console/apitest
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     5139 2024-04-28 07:51:06.000000 zato_apitest-24.1.15/src/zato/apitest/init.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1922 2024-04-28 07:51:07.000000 zato_apitest-24.1.15/src/zato/apitest/run.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 07:55:10.036561 zato_apitest-24.1.15/src/zato/apitest/steps/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.15/src/zato/apitest/steps/__init__.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    31464 2024-04-28 07:50:57.000000 zato_apitest-24.1.15/src/zato/apitest/steps/common.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.15/src/zato/apitest/steps/json.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.15/src/zato/apitest/typing_.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    13732 2024-04-28 07:50:51.000000 zato_apitest-24.1.15/src/zato/apitest/util.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 07:55:10.040561 zato_apitest-24.1.15/src/zato_apitest.egg-info/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-28 07:55:10.000000 zato_apitest-24.1.15/src/zato_apitest.egg-info/PKG-INFO
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-28 07:55:10.000000 zato_apitest-24.1.15/src/zato_apitest.egg-info/SOURCES.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-28 07:55:10.000000 zato_apitest-24.1.15/src/zato_apitest.egg-info/dependency_links.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-28 07:55:10.000000 zato_apitest-24.1.15/src/zato_apitest.egg-info/namespace_packages.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-28 07:55:07.000000 zato_apitest-24.1.15/src/zato_apitest.egg-info/not-zip-safe
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-28 07:55:10.000000 zato_apitest-24.1.15/src/zato_apitest.egg-info/requires.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-28 07:55:10.000000 zato_apitest-24.1.15/src/zato_apitest.egg-info/top_level.txt
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.672277 zato-apitest-24.1.9/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    42880 2019-06-24 21:01:23.000000 zato-apitest-24.1.9/LICENSE.txt
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato-apitest-24.1.9/MANIFEST.in
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2348 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/PKG-INFO
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato-apitest-24.1.9/README.md
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato-apitest-24.1.9/requirements.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-03-12 11:43:29.672277 zato-apitest-24.1.9/setup.cfg
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2634 2024-03-12 11:43:11.000000 zato-apitest-24.1.9/setup.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      227 2024-03-10 13:49:27.000000 zato-apitest-24.1.9/src/zato/__init__.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1816 2024-03-10 14:48:12.000000 zato-apitest-24.1.9/src/zato/apitest/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4343 2024-03-11 14:35:09.000000 zato-apitest-24.1.9/src/zato/apitest/cli.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/console/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      226 2024-03-11 14:35:24.000000 zato-apitest-24.1.9/src/zato/apitest/console/apitest
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4721 2024-03-11 14:47:07.000000 zato-apitest-24.1.9/src/zato/apitest/init.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1882 2024-03-11 14:38:08.000000 zato-apitest-24.1.9/src/zato/apitest/run.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/steps/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      172 2024-03-11 12:18:58.000000 zato-apitest-24.1.9/src/zato/apitest/steps/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29777 2024-03-12 11:41:01.000000 zato-apitest-24.1.9/src/zato/apitest/steps/common.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22095 2024-03-12 11:34:29.000000 zato-apitest-24.1.9/src/zato/apitest/steps/json.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7341 2024-03-11 14:38:39.000000 zato-apitest-24.1.9/src/zato/apitest/typing_.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    13748 2024-03-11 14:38:52.000000 zato-apitest-24.1.9/src/zato/apitest/util.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato_apitest.egg-info/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2348 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/PKG-INFO
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/namespace_packages.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-03-12 11:43:27.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/not-zip-safe
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/requires.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/top_level.txt
```

### Comparing `zato_apitest-24.1.15/LICENSE.txt` & `zato-apitest-24.1.9/LICENSE.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,170 +1,842 @@
-Server Side Public License
+                   GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
 
-VERSION 1, OCTOBER 16, 2018
-
-Copyright © 2018 MongoDB, Inc.
-
-Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
-TERMS AND CONDITIONS
-0. Definitions.
-
-“This License” refers to Server Side Public License.
-
-“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
-
-“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you”. “Licensees” and “recipients” may be individuals or organizations.
-
-To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.
-
-A “covered work” means either the unmodified Program or a work based on the Program.
-
-To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
-
-To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
-
-An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
-1. Source Code.
-
-The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
-
-A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
-
-The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
-
-The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same work.
-2. Basic Permissions.
-
-All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program, subject to section 13. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
-
-Subject to section 13, you may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
-3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
-
-When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
-4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
-5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
-    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
-    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
-    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
-
-A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
-6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
-    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
-    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
-    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
-    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
-
-A “User Product” is either (1) a “consumer product”, which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, “normally used” refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
-
-“Installation Information” for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
-
-The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
-
-Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
-7. Additional Terms.
-
-“Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
-    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
-    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
-    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
-    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
-    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
-
-All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
-8. Termination.
-
-You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
-
-However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
-
-Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
-9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
-10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
-
-An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
-11. Patents.
-
-A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
-
-A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
-
-In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. “Knowingly relying” means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
-
-A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
-12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot use, propagate or convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not use, propagate or convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
-13. Offering the Program as a Service.
-
-If you make the functionality of the Program or a modified version available to third parties as a service, you must make the Service Source Code available via network download to everyone at no charge, under the terms of this License. Making the functionality of the Program or modified version available to third parties as a service includes, without limitation, enabling third parties to interact with the functionality of the Program or modified version remotely through a computer network, offering a service the value of which entirely or primarily derives from the value of the Program or modified version, or offering a service that accomplishes for users the primary purpose of the Program or modified version.
-
-“Service Source Code” means the Corresponding Source for the Program or the modified version, and the Corresponding Source for all programs that you use to make the Program or modified version available as a service, including, without limitation, management software, user interfaces, application program interfaces, automation software, monitoring software, backup software, storage software and hosting software, all such that a user could run an instance of the service using the Service Source Code you make available.
-14. Revised Versions of this License.
-
-MongoDB, Inc. may publish revised and/or new versions of the Server Side Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the Server Side Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by MongoDB, Inc. If the Program does not specify a version number of the Server Side Public License, you may choose any version ever published by MongoDB, Inc.
-
-If the Program specifies that a proxy can decide which future versions of the Server Side Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
-
-Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
-15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+
+  This version of the GNU Lesser General Public License incorporates
+the terms and conditions of version 3 of the GNU General Public
+License, supplemented by the additional permissions listed below.
+
+  0. Additional Definitions.
+
+  As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the GNU
+General Public License.
+
+  "The Library" refers to a covered work governed by this License,
+other than an Application or a Combined Work as defined below.
+
+  An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+  A "Combined Work" is a work produced by combining or linking an
+Application with the Library.  The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+  The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+  The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+  1. Exception to Section 3 of the GNU GPL.
+
+  You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+  2. Conveying Modified Versions.
+
+  If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+   a) under this License, provided that you make a good faith effort to
+   ensure that, in the event an Application does not supply the
+   function or data, the facility still operates, and performs
+   whatever part of its purpose remains meaningful, or
+
+   b) under the GNU GPL, with none of the additional permissions of
+   this License applicable to that copy.
+
+  3. Object Code Incorporating Material from Library Header Files.
+
+  The object code form of an Application may incorporate material from
+a header file that is part of the Library.  You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+   a) Give prominent notice with each copy of the object code that the
+   Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the object code with a copy of the GNU GPL and this license
+   document.
+
+  4. Combined Works.
+
+  You may convey a Combined Work under terms of your choice that,
+taken together, effectively do not restrict modification of the
+portions of the Library contained in the Combined Work and reverse
+engineering for debugging such modifications, if you also do each of
+the following:
+
+   a) Give prominent notice with each copy of the Combined Work that
+   the Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the Combined Work with a copy of the GNU GPL and this license
+   document.
+
+   c) For a Combined Work that displays copyright notices during
+   execution, include the copyright notice for the Library among
+   these notices, as well as a reference directing the user to the
+   copies of the GNU GPL and this license document.
+
+   d) Do one of the following:
+
+       0) Convey the Minimal Corresponding Source under the terms of this
+       License, and the Corresponding Application Code in a form
+       suitable for, and under terms that permit, the user to
+       recombine or relink the Application with a modified version of
+       the Linked Version to produce a modified Combined Work, in the
+       manner specified by section 6 of the GNU GPL for conveying
+       Corresponding Source.
+
+       1) Use a suitable shared library mechanism for linking with the
+       Library.  A suitable mechanism is one that (a) uses at run time
+       a copy of the Library already present on the user's computer
+       system, and (b) will operate properly with a modified version
+       of the Library that is interface-compatible with the Linked
+       Version.
+
+   e) Provide Installation Information, but only if you would otherwise
+   be required to provide such information under section 6 of the
+   GNU GPL, and only to the extent that such information is
+   necessary to install and execute a modified version of the
+   Combined Work produced by recombining or relinking the
+   Application with a modified version of the Linked Version. (If
+   you use option 4d0, the Installation Information must accompany
+   the Minimal Corresponding Source and Corresponding Application
+   Code. If you use option 4d1, you must provide the Installation
+   Information in the manner specified by section 6 of the GNU GPL
+   for conveying Corresponding Source.)
+
+  5. Combined Libraries.
+
+  You may place library facilities that are a work based on the
+Library side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+   a) Accompany the combined library with a copy of the same work based
+   on the Library, uncombined with any other library facilities,
+   conveyed under the terms of this License.
+
+   b) Give prominent notice with the combined library that part of it
+   is a work based on the Library, and explaining where to find the
+   accompanying uncombined form of the same work.
+
+  6. Revised Versions of the GNU Lesser General Public License.
+
+  The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+  Each version is given a distinguishing version number. If the
+Library as you received it specifies that a certain numbered version
+of the GNU Lesser General Public License "or any later version"
+applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version
+published by the Free Software Foundation. If the Library as you
+received it does not specify a version number of the GNU Lesser
+General Public License, you may choose any version of the GNU Lesser
+General Public License ever published by the Free Software Foundation.
+
+  If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
+
+================================================================================
+
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
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
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
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
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zato_apitest-24.1.15/PKG-INFO` & `zato-apitest-24.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.15
+Version: 24.1.9
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
 License: Proprietary
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.15 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.9 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.15/setup.py` & `zato-apitest-24.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import os
 from setuptools import setup, find_packages
 
-version = '24.1.15'
+version = '24.1.9'
 
 LONG_DESCRIPTION = """
 
 Write API tests for your [API integrations](https://zato.io) in plain English, with no programming needed.
 
 Here is how it looks:
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- """ Copyright (C) 2024, Zato Source s.r.o. https://
 zato.io Proprietary product. This is not open source software, reproduction is
 prohibited. """ # stdlib import os from setuptools import setup, find_packages
-version = '24.1.15' LONG_DESCRIPTION = """ Write API tests for your [API
+version = '24.1.9' LONG_DESCRIPTION = """ Write API tests for your [API
 integrations](https://zato.io) in plain English, with no programming needed.
 Here is how it looks: _!_[_A_P_I_ _t_e_s_t_i_n_g_ _i_n_ _P_y_t_h_o_n_]_(_h_t_t_p_s_:_/_/_u_p_c_d_n_._i_o_/_k_W_1_5_b_q_q_/_r_a_w_/
 _r_o_o_t_/_s_t_a_t_i_c_/_i_m_g_/_a_p_i_t_e_s_t_/_a_p_i_t_e_s_t_._j_p_g_) More information about API testing at
 https://zato.io. """ def parse_requirements(requirements): # type: ignore
 ignored = ['#', 'setuptools', '-e'] with open(requirements) as f: return [line
 for line in f if line.strip() and not any(line.startswith(prefix) for prefix in
 ignored)] setup( name = 'zato-apitest', version = version, scripts = ['src/
```

### Comparing `zato_apitest-24.1.15/src/zato/apitest/cli.py` & `zato-apitest-24.1.9/src/zato/apitest/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 Copyright (C) 2024, Zato Source s.r.o. https://zato.io
 
-Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
+Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import os, sys, tempfile, uuid
 
 # Click
 import click
```

### Comparing `zato_apitest-24.1.15/src/zato/apitest/init.py` & `zato-apitest-24.1.9/src/zato/apitest/init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 Copyright (C) 2024, Zato Source s.r.o. https://zato.io
 
-Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
+Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import os
 
 # ################################################################################################################################
 # ################################################################################################################################
@@ -49,15 +49,15 @@
 '''
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 CONFIG_INI = """
 [behave]
-options=--format pretty
+options=--format pretty --no-source --no-timings
 
 [user]
 sample=Hello
 """
 
 # ################################################################################################################################
 # ################################################################################################################################
@@ -91,49 +91,36 @@
     # You can also compare responses directly with files disk
     And response is equal to that from "demo.json"
 """
 
 DEMO_JSON_REQ = """{"hello":"world"}"""
 DEMO_JSON_RESP = """{"action":{"code":0, "msg":"How do you do?", "flow":["Ack", "Done"]}}"""
 
-Demo_XML = """<?xml version="1.0" encoding="UTF-8"?><root/>"""
-
 # ################################################################################################################################
 # ################################################################################################################################
 
 def handle(base_path:'str') -> 'None':
     """ Sets up runtime directories and sample features.
     """
     # Top-level directory for tests
     features_dir = os.path.join(base_path, 'features')
     os.mkdir(features_dir)
 
     # Requests and responses
     request_json_dir = os.path.join(base_path, 'features', 'json', 'request')
     response_json_dir = os.path.join(base_path, 'features', 'json', 'response')
 
-    request_xml_dir = os.path.join(base_path, 'features', 'xml', 'request')
-    response_xml_dir = os.path.join(base_path, 'features', 'xml', 'response')
-
     os.makedirs(request_json_dir)
     os.makedirs(response_json_dir)
 
-    os.makedirs(request_xml_dir)
-    os.makedirs(response_xml_dir)
-
     # Demo feature
     _ = open(os.path.join(features_dir, 'demo.feature'), 'w').write(DEMO_FEATURE)
     _ = open(os.path.join(request_json_dir, 'demo.json'), 'w').write(DEMO_JSON_REQ)
     _ = open(os.path.join(response_json_dir, 'demo.json'), 'w').write(DEMO_JSON_RESP)
 
-    # Demo XML
-
-    _ = open(os.path.join(request_xml_dir, 'demo.xml'), 'w').write(Demo_XML)
-    _ = open(os.path.join(response_xml_dir, 'demo.xml'), 'w').write(Demo_XML)
-
     # Add environment.py
     _ = open(os.path.join(features_dir, 'environment.py'), 'w').write(ENVIRONMENT)
 
     # Add steps
     steps_dir = os.path.join(features_dir, 'steps')
     os.mkdir(steps_dir)
     _ = open(os.path.join(steps_dir, 'steps.py'), 'w').write(STEPS)
```

### Comparing `zato_apitest-24.1.15/src/zato/apitest/run.py` & `zato-apitest-24.1.9/src/zato/apitest/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 Copyright (C) 2024, Zato Source s.r.o. https://zato.io
 
-Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
+Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import os
 
 # Behave
 from behave.configuration import Configuration # type: ignore
@@ -22,17 +22,15 @@
 if 0:
     from zato.apitest.typing_ import strlistnone
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 def handle(path:'str', args:'strlistnone'=None):
-    e
     file_conf = ConfigObj(os.path.join(path, 'features', 'config.ini'))
-    w
     try:
         behave_options = file_conf['behave']['options'] # type: ignore
     except KeyError:
         raise ValueError("Behave config not found. Are you running with the correct path?")
     if args:
         behave_options += ' ' + ' '.join(args)
 
@@ -40,14 +38,11 @@
     if tags:
         behave_options += ' --tags '
         behave_options += ','.join(tags.split())
 
     conf = Configuration(behave_options)
     conf.paths = [os.path.join(path, 'features')]
     runner = Runner(conf)
-    result = runner.run()
-    import time
-    time.sleep(0.5)
-    z
+    return runner.run()
 
 # ################################################################################################################################
 # ################################################################################################################################
```

### Comparing `zato_apitest-24.1.15/src/zato/apitest/steps/common.py` & `zato-apitest-24.1.9/src/zato/apitest/steps/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
 """
 Copyright (C) 2024, Zato Source s.r.o. https://zato.io
 
-Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
+Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import ast
 import json
-import http
 import time
 import os
+from logging import getLogger
 
 # Behave
 from behave import given, when, then # type: ignore
 
 # Bunch
 from bunch import Bunch
 
@@ -41,39 +41,24 @@
 
 if 0:
     from zato.apitest.typing_ import any_, anylistnone, callable_
 
 # ################################################################################################################################
 # ################################################################################################################################
 
-import logging
-logger = logging.getLogger('apitest')
+logger = getLogger(__name__)
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 Context = Bunch
 
 # ################################################################################################################################
 # ################################################################################################################################
 
-def patch_http_send():
-
-    orig_send = http.client.HTTPConnection.send # type: ignore
-    def _send(self, data): # type: ignore
-        logger.info('\n--------- BEGIN Send ---------\n%s\n--------- END Send ---------' % data.decode('utf8'))
-        return orig_send(self, data)
-
-    http.client.HTTPConnection.send = _send # type: ignore
-
-patch_http_send()
-
-# ################################################################################################################################
-# ################################################################################################################################
-
 @when('the URL is invoked')
 def when_the_url_is_invoked(ctx:'Context', adapters:'anylistnone'=None) -> 'None':
 
     response_data = None
 
     try:
 
@@ -87,62 +72,53 @@
             # If no response_format is set, assume it's the same as the request format.
             # If the request format hasn't been specified either, assume 'RAW'.
             response_format = ctx.zato.request.get('response_format', ctx.zato.request.get('format', 'JSON'))
 
             if response_format == 'JSON':
                 ctx.zato.response.data_impl = json.loads(ctx.zato.response.data_text)
 
-            elif response_format in {'RAW', 'FORM', 'XML'}:
+            elif response_format == 'RAW':
+                ctx.zato.response.data_impl = ctx.zato.response.data_text
+
+            elif response_format == 'FORM':
                 ctx.zato.response.data_impl = ctx.zato.response.data_text
 
     except Exception as e:
         logger.warn('Caught an exception while invoking `%s` with `%s`; req=`%s`; resp=`%s`, (%s)',
             ctx.zato.full_address, ctx.zato.request.method, ctx.zato.request.data, response_data, e.args[0])
         raise
 
 # ################################################################################################################################
 # ################################################################################################################################
 
-@when('this scenario is invoked')
-def when_this_scenario_is_invoked(ctx:'Context', adapters:'anylistnone'=None) -> 'None':
-    pass
-
-# ################################################################################################################################
-# ################################################################################################################################
-
 def invoke_http(ctx:'Context', adapters:'anylistnone'=None) -> 'None':
 
     adapters = adapters or []
     method = ctx.zato.request.get('method', 'GET')
     address = ctx.zato.request.get('address')
     url_path = ctx.zato.request.get('url_path', '/')
     qs = ctx.zato.request.get('query_string', '')
     files = None
     data = ''
 
     if 'data_impl' in ctx.zato.request:
-        if ctx.zato.request.get('is_xml'):
+        if ctx.zato.request.is_xml:
             data = etree.tostring(ctx.zato.request.data_impl)
-        elif ctx.zato.request.get('is_json'):
+        elif ctx.zato.request.is_json:
             data = json.dumps(ctx.zato.request.data_impl, indent=2)
             ctx.zato.request.headers['Content-Type'] = 'application/json'
-        elif ctx.zato.request.get('is_raw'):
+        elif ctx.zato.request.is_raw:
             data = ctx.zato.request.data_impl
-        elif ctx.zato.request.get('is_form'):
+        elif ctx.zato.request.is_form:
             data = ctx.zato.request.get('form', '')
             files = ctx.zato.request.get('files', None)
             ctx.zato.request.headers['Content-Type'] = 'application/x-www-form-urlencoded'
-
             if files is not None:
                 # multipart/formdata should let requests set the content-type header
                 del ctx.zato.request.headers['Content-Type']
-        else:
-            # Default to JSON
-            data = json.dumps(ctx.zato.request.data_impl, indent=2)
-            ctx.zato.request.headers['Content-Type'] = 'application/json'
 
     ctx.zato.request.method = method
     ctx.zato.request.data = data
     ctx.zato.full_address = '{}{}{}'.format(address, url_path, qs)
 
     auth = None
 
@@ -163,26 +139,16 @@
         method,
         ctx.zato.full_address,
         data=data,
         files=files,
         headers=ctx.zato.request.headers,
         auth=auth)
 
-    # Always assume that responses are in UTF8
-    data_received = ctx.zato.response.data.content.decode('utf8')
-
-    # Log what we received
-    logger.info('\n--------- BEGIN Receive ---------\n%s\n--------- END Receive ---------' % data_received)
-
-    # Assign the response for later use
     ctx.zato.response.data_text = ctx.zato.response.data.text
 
-    # This is needed here to prevent behave from not logging the above
-    logger.info('')
-
 # ################################################################################################################################
 # ################################################################################################################################
 
 def invoke_zato_web_sockets_service(ctx:'Context') -> 'None':
 
     ctx.zato.response = Bunch()
     ctx.zato.response.data_text = json.dumps(ctx.zato.wsx_client.invoke(ctx.zato.request.data_impl).data)
@@ -260,19 +226,17 @@
 
     ctx.zato.request.data = data
 
     if ctx.zato.request.get('is_json'):
         ctx.zato.request.data_impl = json.loads(ctx.zato.request.data)
     elif ctx.zato.request.get('is_raw'):
         ctx.zato.request.data_impl = ctx.zato.request.data
-    elif ctx.zato.request.get('is_xml'):
-        data = ctx.zato.request.data.encode('utf8')
-        ctx.zato.request.data_impl = etree.fromstring(data) # type: ignore
     else:
-        ctx.zato.request.data_impl = json.loads(ctx.zato.request.data)
+        if not ctx.zato.request.format:
+            raise ValueError('Format not set, cannot proceed')
 
 # ################################################################################################################################
 
 @given('request "{request_path}"')
 @util.obtain_values
 def given_request(ctx:'Context', request_path:'str') -> 'None':
     return given_request_impl(ctx, util.get_data(ctx, 'request', request_path))
@@ -299,15 +263,15 @@
 
     files[name] = open(full_path, 'rb')
 
     ctx.zato.request.files = files
 
 # ################################################################################################################################
 
-@given('form field "{name}" is "{value}"')
+@given('request param "{name}" is "{value}"')
 @util.obtain_values
 def given_request_param(ctx:'Context', name:'str', value:'any_') -> 'None':
     ctx.zato.request.data_impl = None
     form = ctx.zato.request.get('form', {})
     if name in form:
         if isinstance(form[name], list):
             form[name].append(value)
@@ -381,22 +345,14 @@
 @util.obtain_values
 def given_i_store_a_random_date_under_name(ctx:'Context', name:'str', format:'str') -> 'None':
     ctx.zato.user_ctx[name] = util.rand_date(ctx.zato.date_formats[format])
 
 # ################################################################################################################################
 # ################################################################################################################################
 
-@given('I encode "{value}" using Base64 under "{name}"')
-@util.obtain_values
-def given_i_encode_value_using_base64_under_name(ctx:'Context', value:'str', name:'str') -> 'None':
-    ctx.zato.user_ctx[name] = value.encode('base64','strict')
-
-# ################################################################################################################################
-# ################################################################################################################################
-
 @then('context is cleaned up')
 @util.obtain_values
 def then_context_is_cleaned_up(ctx:'Context') -> 'None':
     ctx.zato = util.new_context(ctx, '')
 
 # ################################################################################################################################
 
@@ -536,15 +492,15 @@
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 @then('I store "{path}" from response under "{name}", default "{default}"')
 @util.obtain_values
 def then_store_path_under_name_with_default(ctx:'Context', path:'str', name:'str', default:'str') -> 'None':
-    if ctx.zato.request.get('is_xml'):
+    if ctx.zato.request.is_xml:
         value = ctx.zato.response.data_impl.xpath(path)
         if value:
             if len(value) == 1:
                 value = value[0].text
             else:
                 value = [elem.text for elem in value]
         else:
@@ -581,47 +537,54 @@
 def _response_is_equal_to(ctx:'Context', expected:'any_') -> 'bool':
     assert_equals(expected, ctx.zato.response.data_impl)
     return True
 
 # ################################################################################################################################
 
 @then('response is equal to that from "{path}"')
+@needs_json
 @util.obtain_values
 def then_response_is_equal_to_that_from(ctx:'Context', path:'str') -> 'bool':
-    data = util.get_data(ctx, 'response', path)
-    if ctx.zato.request.is_json:
-        data = json.loads(data)
-    return _response_is_equal_to(ctx, data)
+    return _response_is_equal_to(ctx, json.loads(util.get_data(ctx, 'response', path)))
 
 # ################################################################################################################################
 
-@then('response is equal to "{expected}"')
+@then('JSON response is equal to "{expected}"')
+@needs_json
 @util.obtain_values
 def then_response_is_equal_to(ctx:'Context', expected:'any_') -> 'bool':
-    return _response_is_equal_to(ctx, expected)
+    return _response_is_equal_to(ctx, json.loads(expected))
 
 # ################################################################################################################################
 
-@then('JSON response is equal to "{expected}"')
-@needs_json
-@util.obtain_values
-def then_json_response_is_equal_to(ctx:'Context', expected:'any_') -> 'bool':
-    return _response_is_equal_to(ctx, json.loads(expected))
+#@then('response is equal to "{expected}"')
+#@needs_json
+#@util.obtain_values
+#def then_response_is_equal_to(ctx:'Context', expected:'any_') -> 'None':
+#    return _response_is_equal_to(ctx, expected)
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 @then('I sleep for "{sleep_time}"')
 @util.obtain_values
 def then_i_sleep_for(ctx:'Context', sleep_time:'int') -> 'None':
     time.sleep(float(sleep_time))
 
 # ################################################################################################################################
 # ################################################################################################################################
 
+@given('I encode "{value}" using Base64 under "{name}"')
+@util.obtain_values
+def given_i_encode_value_using_base64_under_name(ctx:'Context', value:'str', name:'str') -> 'None':
+    ctx.zato.user_ctx[name] = value.encode('base64','strict')
+
+# ################################################################################################################################
+# ################################################################################################################################
+
 def variable_is(variable:'any_', value:'any_') -> 'None':
     expected_value = ast.literal_eval(value)
     assert variable == expected_value, 'Value `{}` is not equal to expected `{}`'.format(variable, expected_value)
 
 # ################################################################################################################################
 
 @then('variable "{variable}" is a list "{value}"')
```

### Comparing `zato_apitest-24.1.15/src/zato/apitest/steps/json.py` & `zato-apitest-24.1.9/src/zato/apitest/steps/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 Copyright (C) 2024, Zato Source s.r.o. https://zato.io
 
-Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
+Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import json
 import uuid
 from ast import literal_eval
 
@@ -276,23 +276,14 @@
     actual = get_pointer(ctx.zato.response.data_impl, path)
     assert isinstance(actual, bool), \
         'Expected a bool in {}, got a `{}`'.format(path, type(actual))
     return True
 
 # ################################################################################################################################
 
-@then('path "{path}" is any string')
-@util.obtain_values
-def then_json_pointer_is_any_string(ctx:'Context', path:'str') -> 'bool':
-    actual = get_pointer(ctx.zato.response.data_impl, path)
-    assert isinstance(actual, str), 'Expected a str in {}, got a `{}`'.format(path, type(actual))
-    return True
-
-# ################################################################################################################################
-
 @then('path "{path}" is a list "{value}"')
 @util.obtain_values
 def then_json_pointer_is_a_list(ctx:'Context', path:'str', value:'any_') -> 'bool':
     return assert_value(ctx, path, value, util.parse_list)
 
 # ################################################################################################################################
```

### Comparing `zato_apitest-24.1.15/src/zato/apitest/typing_.py` & `zato-apitest-24.1.9/src/zato/apitest/typing_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 Copyright (C) 2024, Zato Source s.r.o. https://zato.io
 
-Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
+Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 # stdlib
 from datetime import date, datetime
```

### Comparing `zato_apitest-24.1.15/src/zato/apitest/util.py` & `zato-apitest-24.1.9/src/zato/apitest/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 Copyright (C) 2024, Zato Source s.r.o. https://zato.io
 
-Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
+Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import csv, operator, os, random, uuid, re
 from collections import OrderedDict
 from datetime import timedelta
 from io import StringIO
```

### Comparing `zato_apitest-24.1.15/src/zato_apitest.egg-info/PKG-INFO` & `zato-apitest-24.1.9/src/zato_apitest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.15
+Version: 24.1.9
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
 License: Proprietary
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.15 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.9 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.15/src/zato_apitest.egg-info/SOURCES.txt` & `zato-apitest-24.1.9/src/zato_apitest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

