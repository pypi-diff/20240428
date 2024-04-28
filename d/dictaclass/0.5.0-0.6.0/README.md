# Comparing `tmp/dictaclass-0.5.0.tar.gz` & `tmp/dictaclass-0.6.0.tar.gz`

## Comparing `dictaclass-0.5.0.tar` & `dictaclass-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.env
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dictaclass-0.5.0/requirements.dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dictaclass-0.5.0/requirements.txt
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dictaclass-0.5.0/test.Dockerfile
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dictaclass-0.5.0/dictaclass/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 dictaclass-0.5.0/dictaclass/dictaclass.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dictaclass-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 dictaclass-0.5.0/tests/test_dictaclass.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 dictaclass-0.5.0/tests/test_meta.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.gitignore
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 dictaclass-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 dictaclass-0.5.0/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 dictaclass-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 dictaclass-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dictaclass-0.6.0/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dictaclass-0.6.0/.env
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dictaclass-0.6.0/requirements.dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dictaclass-0.6.0/requirements.txt
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dictaclass-0.6.0/test.Dockerfile
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 dictaclass-0.6.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dictaclass-0.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dictaclass-0.6.0/dictaclass/__init__.py
+-rw-r--r--   0        0        0    12077 2020-02-02 00:00:00.000000 dictaclass-0.6.0/dictaclass/dictaclass.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dictaclass-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 dictaclass-0.6.0/tests/test_dictaclass.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 dictaclass-0.6.0/tests/test_meta.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dictaclass-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 dictaclass-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 dictaclass-0.6.0/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 dictaclass-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 dictaclass-0.6.0/PKG-INFO
```

### Comparing `dictaclass-0.5.0/.devcontainer/devcontainer.json` & `dictaclass-0.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dictaclass-0.5.0/dictaclass/dictaclass.py` & `dictaclass-0.6.0/dictaclass/dictaclass.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-from typing import Any, Dict, Type, TypeVar, List, Set, Dict, Callable, Union, Optional, get_type_hints
+from typing import (
+    Any,
+    Dict,
+    Type,
+    TypeVar,
+    List,
+    Set,
+    Callable,
+    Union,
+    Optional,
+    get_type_hints,
+)
 from dataclasses import is_dataclass, asdict
+from datetime import datetime, timezone
 
 import sys
 
 T = TypeVar("T")
 
 
 def _transformer_noop(source: str) -> str:
@@ -89,14 +101,28 @@
                     value,
                     key_transformer,
                     on_extra_field,
                     implicit_optional,
                 )
                 for key, value in dict_value.items()
             }
+        elif annotation_type is datetime:
+            if isinstance(dict_value, (int, float)):
+                dataclass_dict[annotation_name] = datetime.fromtimestamp(
+                    dict_value,
+                    tz=timezone.utc,
+                )
+            elif isinstance(dict_value, str):
+                dataclass_dict[annotation_name] = datetime.fromisoformat(dict_value)
+            elif isinstance(dict_value, datetime):
+                dataclass_dict[annotation_name] = dict_value
+            else:
+                raise ValueError(
+                    f"Unsupported type for datetime: {type(dict_value)}: {dict_value}"
+                )
         else:
             dataclass_dict[annotation_name] = _to_dataclass_38(
                 annotation_type,
                 dict_value,
                 key_transformer,
                 on_extra_field,
                 implicit_optional,
@@ -218,14 +244,28 @@
                         on_extra_field,
                         implicit_optional,
                     )
                     for k, v in dict_value.items()
                 }
             else:
                 raise Exception(f"Unsupported typehint __origin__ = {origin}.")
+        elif annotation_type is datetime:
+            if isinstance(dict_value, (int, float)):
+                dataclass_dict[annotation_name] = datetime.fromtimestamp(
+                    dict_value,
+                    tz=timezone.utc,
+                )
+            elif isinstance(dict_value, str):
+                dataclass_dict[annotation_name] = datetime.fromisoformat(dict_value)
+            elif isinstance(dict_value, datetime):
+                dataclass_dict[annotation_name] = dict_value
+            else:
+                raise ValueError(
+                    f"Unsupported type for datetime: {type(dict_value)}: {dict_value}"
+                )
         else:
             dataclass_dict[annotation_name] = _to_dataclass_37(
                 annotation_type,
                 dict_value,
                 key_transformer,
                 on_extra_field,
                 implicit_optional,
@@ -319,7 +359,14 @@
 
 
 def dataclass_to_dict(dataclassObject: Any) -> Dict[str, Any]:
     """
     Convert a dataclass hierarchy to a simple dict/list hierarchy.
     """
     return asdict(dataclassObject)
+
+
+def json_dumps_default(obj: Any) -> Any:
+    if isinstance(obj, datetime):
+        return obj.astimezone(timezone.utc).timestamp()
+    else:
+        return obj
```

### Comparing `dictaclass-0.5.0/tests/test_dictaclass.py` & `dictaclass-0.6.0/tests/test_dictaclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dictaclass.dictaclass import to_dataclass
+from dictaclass.dictaclass import to_dataclass, dataclass_to_dict, json_dumps_default
 
 from dataclasses import dataclass
 
 from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
 
 import pytest
 
@@ -420,7 +420,33 @@
         class ExampleDC:
             url_encoded: str
 
         v = to_dataclass(ExampleDC, dict(UrlEncoded="asdf"), inflection.camelize)
 
         assert isinstance(v, ExampleDC)
         assert v.url_encoded == "asdf"
+
+
+class Test_Dictaclass_Datetime:
+    def test_with_datetime(self) -> None:
+        import json
+        import datetime
+
+        utc = datetime.timezone.utc
+
+        @dataclass(frozen=True)
+        class ExampleDC:
+            timestamp: datetime.datetime
+
+        dc = ExampleDC(timestamp=datetime.datetime.now())
+        dc_dict = dataclass_to_dict(dc)
+        dc_json = json.dumps(dc_dict, default=json_dumps_default)
+
+        jdc_dict = json.loads(dc_json)
+        assert isinstance(jdc_dict["timestamp"], (int, float))
+
+        jdc = to_dataclass(ExampleDC, jdc_dict)
+        assert jdc.timestamp.day == dc.timestamp.day
+        assert isinstance(jdc.timestamp, datetime.datetime)
+
+        # NOTE: We can't compare the timezone directly because the timezone is set to UTC when deserializing.
+        assert jdc.timestamp.astimezone(utc) == dc.timestamp.astimezone(utc)
```

### Comparing `dictaclass-0.5.0/tests/test_meta.py` & `dictaclass-0.6.0/tests/test_meta.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import os
-import pytest
-
-
-in_docker = os.path.exists(os.path.expanduser("/.dockerenv"))
-
-
-def _test_all_python(py_version: str):
-    try:
-        assert (
-            os.system(
-                f"docker build"
-                f" -q"
-                f" -t dictaclass-test:{py_version}"
-                f" -f test.Dockerfile"
-                f" --build-arg PY_VERSION={py_version}"
-                f" ."
-            )
-            == 0
-        )
-        assert os.system(f"docker run -t --rm dictaclass-test:{py_version}") == 0
-    finally:
-        os.system(f"docker image rm dictaclass-test:{py_version}")
-
-
-@pytest.mark.skip("3.6 is not supported.")
-@pytest.mark.skipif(in_docker, reason="DinDon't")
-def test_all_python_3_6():
-    _test_all_python("3.6")
-
-
-@pytest.mark.skipif(in_docker, reason="DinDon't")
-def test_all_python_3_7():
-    _test_all_python("3.7")
-
-
-@pytest.mark.skipif(in_docker, reason="DinDon't")
-def test_all_python_3_7_2():
-    _test_all_python("3.7.2")
-
-
-@pytest.mark.skipif(in_docker, reason="DinDon't")
-def test_all_python_3_8():
-    _test_all_python("3.8")
-
-
-@pytest.mark.skipif(in_docker, reason="DinDon't")
-def test_all_python_3_9():
-    _test_all_python("3.9")
-
-
-@pytest.mark.skipif(in_docker, reason="DinDon't")
-def test_all_python_3_10():
-    _test_all_python("3.10")
-
-
-@pytest.mark.skipif(in_docker, reason="DinDon't")
-def test_all_python_3_11():
-    _test_all_python("3.11")
+import os
+import pytest
+
+
+in_docker = os.path.exists(os.path.expanduser("/.dockerenv"))
+
+
+def _test_all_python(py_version: str):
+    try:
+        assert (
+            os.system(
+                f"docker build"
+                f" -q"
+                f" -t dictaclass-test:{py_version}"
+                f" -f test.Dockerfile"
+                f" --build-arg PY_VERSION={py_version}"
+                f" ."
+            )
+            == 0
+        )
+        assert os.system(f"docker run -t --rm dictaclass-test:{py_version}") == 0
+    finally:
+        os.system(f"docker image rm dictaclass-test:{py_version}")
+
+
+@pytest.mark.skip("3.6 is not supported.")
+@pytest.mark.skipif(in_docker, reason="DinDon't")
+def test_all_python_3_6():
+    _test_all_python("3.6")
+
+
+@pytest.mark.skipif(in_docker, reason="DinDon't")
+def test_all_python_3_7():
+    _test_all_python("3.7")
+
+
+@pytest.mark.skipif(in_docker, reason="DinDon't")
+def test_all_python_3_7_2():
+    _test_all_python("3.7.2")
+
+
+@pytest.mark.skipif(in_docker, reason="DinDon't")
+def test_all_python_3_8():
+    _test_all_python("3.8")
+
+
+@pytest.mark.skipif(in_docker, reason="DinDon't")
+def test_all_python_3_9():
+    _test_all_python("3.9")
+
+
+@pytest.mark.skipif(in_docker, reason="DinDon't")
+def test_all_python_3_10():
+    _test_all_python("3.10")
+
+
+@pytest.mark.skipif(in_docker, reason="DinDon't")
+def test_all_python_3_11():
+    _test_all_python("3.11")
```

### Comparing `dictaclass-0.5.0/LICENSE.txt` & `dictaclass-0.6.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-              Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022 Bozhidar Stoyanov
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+              Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 Bozhidar Stoyanov
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `dictaclass-0.5.0/README.md` & `dictaclass-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # dictaclass - dicts to dataclasses
 
 Have you ever been handed an "example JSON" and wanted to have it in an intellisense-friendly structure?
-Just define the JSON structure as a hierarchy of dataclasses and run `to_dataclass(MyJsonDatatclass, json.loads(source))`
+Just define the JSON structure as a hierarchy of dataclasses and run `to_dataclass(MyJsonDataclass, json.loads(source))`
 
 
 Well, the library works with whatever source of data you have, as long as you can represent the way `json.loads` does - `dict`s, `list`s, and values.
 
 
 ## Features
 
 - Supports deeply nested dataclasses (duh)
 - Supports inheritance
 - Supports collections
   - `list`
   - `set`
   - `dict`
 - Supports `frozen` dataclasses
+- Supports timestamps as `datetime` objects
 
 ## Limitations
 
 - Requires Python 3.7+ 
 - Cannot guess types.
 - Cannot use mixed types.
 - Cannot use Union[].
```

### Comparing `dictaclass-0.5.0/pyproject.toml` & `dictaclass-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dictaclass"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
     { name = "Bozhidar Stoyanov", email="glav0r3zzz4@gmail.com"}
 ]
 description = "Convert heirarchies of dicts/list/sets/values (JSON?) to heirarchies of type annotated dataclasses."
 readme = "README.md"
 requires-python = ">=3.7.2"
 classifiers = [
```

### Comparing `dictaclass-0.5.0/PKG-INFO` & `dictaclass-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dictaclass
-Version: 0.5.0
+Version: 0.6.0
 Summary: Convert heirarchies of dicts/list/sets/values (JSON?) to heirarchies of type annotated dataclasses.
 Project-URL: Homepage, https://github.com/BraynStorm/dictaclass
 Project-URL: Bug Tracker, https://github.com/BraynStorm/dictaclass/issues
 Author-email: Bozhidar Stoyanov <glav0r3zzz4@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 
 # dictaclass - dicts to dataclasses
 
 Have you ever been handed an "example JSON" and wanted to have it in an intellisense-friendly structure?
-Just define the JSON structure as a hierarchy of dataclasses and run `to_dataclass(MyJsonDatatclass, json.loads(source))`
+Just define the JSON structure as a hierarchy of dataclasses and run `to_dataclass(MyJsonDataclass, json.loads(source))`
 
 
 Well, the library works with whatever source of data you have, as long as you can represent the way `json.loads` does - `dict`s, `list`s, and values.
 
 
 ## Features
 
 - Supports deeply nested dataclasses (duh)
 - Supports inheritance
 - Supports collections
   - `list`
   - `set`
   - `dict`
 - Supports `frozen` dataclasses
+- Supports timestamps as `datetime` objects
 
 ## Limitations
 
 - Requires Python 3.7+ 
 - Cannot guess types.
 - Cannot use mixed types.
 - Cannot use Union[].
```

