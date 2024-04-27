# Comparing `tmp/datasette-enrichments-0.3.2.tar.gz` & `tmp/datasette_enrichments-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-enrichments-0.3.2.tar", last modified: Tue Apr  9 20:07:20 2024, max compression
+gzip compressed data, was "datasette_enrichments-0.4.tar", last modified: Sat Apr 27 06:04:22 2024, max compression
```

## Comparing `datasette-enrichments-0.3.2.tar` & `datasette_enrichments-0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.427827 datasette-enrichments-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-09 20:07:20.427827 datasette-enrichments-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.423827 datasette-enrichments-0.3.2/datasette_enrichments/
--rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.423827 datasette-enrichments-0.3.2/datasette_enrichments/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/templates/enrichment.html
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/templates/enrichment_picker.html
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.423827 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:07:20.427827 datasette-enrichments-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.423827 datasette-enrichments-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/tests/test_enrichments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.381303 datasette_enrichments-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-27 06:04:22.381303 datasette_enrichments-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.377303 datasette_enrichments-0.4/datasette_enrichments/
+-rw-r--r--   0 runner    (1001) docker     (127)    16287 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.377303 datasette_enrichments-0.4/datasette_enrichments/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/templates/enrichment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/templates/enrichment_picker.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/datasette_enrichments/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.377303 datasette_enrichments-0.4/datasette_enrichments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 06:04:22.000000 datasette_enrichments-0.4/datasette_enrichments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:04:22.381303 datasette_enrichments-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:04:22.377303 datasette_enrichments-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-27 06:04:10.000000 datasette_enrichments-0.4/tests/test_enrichments.py
```

### Comparing `datasette-enrichments-0.3.2/LICENSE` & `datasette_enrichments-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.2/PKG-INFO` & `datasette_enrichments-0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments
-Version: 0.3.2
+Version: 0.4
 Summary: Tools for running enrichments against data stored in Datasette
 Home-page: https://github.com/simonw/datasette-enrichments
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-enrichments/issues
 Project-URL: CI, https://github.com/simonw/datasette-enrichments/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-enrichments/releases
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasette
 Requires-Dist: WTForms
+Requires-Dist: datasette-secrets>=0.2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: packaging; extra == "test"
 Provides-Extra: docs
```

### Comparing `datasette-enrichments-0.3.2/README.md` & `datasette_enrichments-0.4/README.md`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.2/datasette_enrichments/__init__.py` & `datasette_enrichments-0.4/datasette_enrichments/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from abc import ABC, abstractmethod
 import asyncio
 from datasette import hookimpl
 from datasette.utils import async_call_with_supported_arguments, tilde_encode
+from datasette_secrets import Secret, get_secret
 import json
 import secrets
 import traceback
 import urllib
 from datasette.plugins import pm
+from markupsafe import Markup, escape
 from .views import enrichment_picker, enrichment_view
+from wtforms import PasswordField
+from wtforms.validators import DataRequired
 from .utils import get_with_auth, mark_job_complete, pks_for_rows
 from . import hookspecs
 
 from datasette.utils import await_me_maybe
 
-from typing import TYPE_CHECKING, Any, Tuple, Union, List
+from typing import TYPE_CHECKING, Any, List, Optional, Tuple, Union
 
 if TYPE_CHECKING:
     from datasette.app import Datasette
     from datasette.database import Database
 
 pm.add_hookspecs(hookspecs)
 
@@ -61,15 +65,30 @@
     created_at text,
     row_pks text, -- JSON list of row primary keys
     error text
 )
 """.strip()
 
 
+@hookimpl
+def register_secrets():
+    secrets = []
+    for subclass in Enrichment._subclasses:
+        if subclass.secret:
+            secrets.append(subclass.secret)
+    return secrets
+
+
+class SecretError(Exception):
+    pass
+
+
 class Enrichment(ABC):
+    _subclasses = []
+
     batch_size: int = 100
     # Cancel run after this many errors
     default_max_errors: int = 5
     log_traceback: bool = False
 
     @property
     @abstractmethod
@@ -79,19 +98,44 @@
 
     @property
     @abstractmethod
     def name(self):
         # The name of this enrichment
         ...
 
-    description = ""  # Short description of this enrichment
+    description: str = ""  # Short description of this enrichment
+    secret: Optional[Secret] = None
+
+    def __init_subclass__(cls, **kwargs):
+        super().__init_subclass__(**kwargs)
+        cls._subclasses.append(cls)
 
     def __repr__(self):
         return "<Enrichment: {}>".format(self.slug)
 
+    async def get_secret(self, datasette: "Datasette", config: dict):
+        if self.secret is None:
+            breakpoint()
+            raise SecretError("No secret defined for this enrichment")
+        secret = await get_secret(datasette, self.secret.name)
+        if secret is not None:
+            return secret
+        # Try the stashed secrets instead
+        if not hasattr(datasette, "_enrichments_stashed_secrets"):
+            breakpoint()
+            raise SecretError("No secrets have been stashed")
+        stashed_keys = datasette._enrichments_stashed_secrets
+        stash_key = config.get("enrichment_secret")
+        if stash_key not in stashed_keys:
+            breakpoint()
+            raise SecretError(
+                "No secret found in stash for {}".format(self.secret.name)
+            )
+        return stashed_keys[stash_key]
+
     async def log_error(
         self, db: "Database", job_id: int, ids: List[IdType], error: str
     ):
         if self.log_traceback:
             error += "\n\n" + traceback.format_exc()
         # Record error and increment error_count
         await db.execute_write(
@@ -109,14 +153,59 @@
         """,
             (len(ids), job_id),
         )
 
     async def get_config_form(self, datasette: "Datasette", db: "Database", table: str):
         return None
 
+    async def _get_config_form(
+        self, datasette: "Datasette", db: "Database", table: str
+    ):
+        # Helper method that adds a `_secret` form field if the enrichment has a secret
+        FormClass = await async_call_with_supported_arguments(
+            self.get_config_form, datasette=datasette, db=db, table=table
+        )
+        if self.secret is None:
+            return FormClass
+        # If secret is already set, return form unmodified
+        if await get_secret(datasette, self.secret.name):
+            return FormClass
+
+        # Otherwise, return form with secret field
+        def stash_api_key(form, field):
+            if not hasattr(datasette, "_enrichments_stashed_secrets"):
+                datasette._enrichments_stashed_secrets = {}
+            key = secrets.token_urlsafe(16)
+            datasette._enrichments_stashed_secrets[key] = field.data
+            field.data = key
+
+        formatted_description = self.secret.description
+        if self.secret.obtain_url and self.secret.obtain_label:
+            html_bits = []
+            if self.secret.description:
+                html_bits.append(escape(self.secret.description))
+                html_bits.append(" - ")
+            html_bits.append(
+                f'<a href="{self.secret.obtain_url}" target="_blank">{self.secret.obtain_label}</a>'
+            )
+            formatted_description = Markup("".join(html_bits))
+
+        class FormWithSecret(FormClass):
+            enrichment_secret = PasswordField(
+                self.secret.name,
+                description=formatted_description,
+                validators=[
+                    DataRequired(message="Secret is required."),
+                    stash_api_key,
+                ],
+                render_kw={"autocomplete": "off"},
+            )
+
+        return FormWithSecret
+
     async def initialize(
         self, datasette: "Datasette", db: "Database", table: str, config: dict
     ):
         pass
 
     async def finalize(
         self, datasette: "Datasette", db: "Database", table: str, config: dict
```

### Comparing `datasette-enrichments-0.3.2/datasette_enrichments/templates/enrichment.html` & `datasette_enrichments-0.4/datasette_enrichments/templates/enrichment.html`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.2/datasette_enrichments/templates/enrichment_picker.html` & `datasette_enrichments-0.4/datasette_enrichments/templates/enrichment_picker.html`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.2/datasette_enrichments/utils.py` & `datasette_enrichments-0.4/datasette_enrichments/utils.py`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.2/datasette_enrichments/views.py` & `datasette_enrichments-0.4/datasette_enrichments/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # If an enrichment is selected, use that UI
 
     if request.method == "POST":
         return await enrich_data_post(datasette, request, enrichment, filtered_data)
 
     form = (
         await async_call_with_supported_arguments(
-            enrichment.get_config_form,
+            enrichment._get_config_form,
             datasette=datasette,
             db=datasette.get_database(database),
             table=table,
         )
     )()
 
     return Response.html(
@@ -166,15 +166,15 @@
     filter_querystring = urllib.parse.urlencode(filters)
 
     # Roll our own form parsing because .post_vars() eliminates duplicate names
     body = await request.post_body()
     post_vars = MultiParams(urllib.parse.parse_qs(body.decode("utf-8")))
 
     Form = await async_call_with_supported_arguments(
-        enrichment.get_config_form, datasette=datasette, db=db, table=table
+        enrichment._get_config_form, datasette=datasette, db=db, table=table
     )
 
     form = Form(post_vars)
 
     if not form.validate():
         return Response.html(
             await datasette.render_template(
```

### Comparing `datasette-enrichments-0.3.2/datasette_enrichments.egg-info/PKG-INFO` & `datasette_enrichments-0.4/datasette_enrichments.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments
-Version: 0.3.2
+Version: 0.4
 Summary: Tools for running enrichments against data stored in Datasette
 Home-page: https://github.com/simonw/datasette-enrichments
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-enrichments/issues
 Project-URL: CI, https://github.com/simonw/datasette-enrichments/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-enrichments/releases
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasette
 Requires-Dist: WTForms
+Requires-Dist: datasette-secrets>=0.2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: packaging; extra == "test"
 Provides-Extra: docs
```

### Comparing `datasette-enrichments-0.3.2/datasette_enrichments.egg-info/SOURCES.txt` & `datasette_enrichments-0.4/datasette_enrichments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.2/setup.py` & `datasette_enrichments-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3.2"
+VERSION = "0.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -28,15 +28,15 @@
     classifiers=[
         "Framework :: Datasette",
         "License :: OSI Approved :: Apache Software License",
     ],
     version=VERSION,
     packages=["datasette_enrichments"],
     entry_points={"datasette": ["enrichments = datasette_enrichments"]},
-    install_requires=["datasette", "WTForms"],
+    install_requires=["datasette", "WTForms", "datasette-secrets>=0.2"],
     extras_require={
         "test": ["pytest", "pytest-asyncio", "black", "ruff", "packaging"],
         "docs": [
             "sphinx==7.2.6",
             "furo==2023.9.10",
             "sphinx-autobuild",
             "sphinx-copybutton",
```

