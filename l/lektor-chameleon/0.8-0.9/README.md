# Comparing `tmp/lektor_chameleon-0.8.tar.gz` & `tmp/lektor_chameleon-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor_chameleon-0.8.tar", last modified: Sat Apr 27 19:46:38 2024, max compression
+gzip compressed data, was "lektor_chameleon-0.9.tar", last modified: Sun Apr 28 20:46:53 2024, max compression
```

## Comparing `lektor_chameleon-0.8.tar` & `lektor_chameleon-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1496 2024-04-27 16:35:46.000000 lektor_chameleon-0.8/LICENSE.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)     4072 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/PKG-INFO
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1130 2024-04-27 19:18:39.000000 lektor_chameleon-0.8/README.rst
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/lektor_chameleon.egg-info/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     4072 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/PKG-INFO
--rw-r--r--   0 uyar      (1000) uyar      (1000)      323 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/SOURCES.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/dependency_links.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       62 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/entry_points.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)      100 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/requires.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       17 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/top_level.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)     2920 2024-04-27 19:18:39.000000 lektor_chameleon-0.8/lektor_chameleon.py
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1964 2024-04-27 16:45:38.000000 lektor_chameleon-0.8/pyproject.toml
--rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/setup.cfg
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/tests/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1885 2024-04-27 19:18:39.000000 lektor_chameleon-0.8/tests/test_chameleon.py
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-28 20:46:53.308902 lektor_chameleon-0.9/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1496 2024-04-27 16:35:46.000000 lektor_chameleon-0.9/LICENSE.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     5226 2024-04-28 20:46:53.308902 lektor_chameleon-0.9/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     2284 2024-04-28 20:45:28.000000 lektor_chameleon-0.9/README.rst
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-28 20:46:53.308902 lektor_chameleon-0.9/lektor_chameleon.egg-info/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     5226 2024-04-28 20:46:53.000000 lektor_chameleon-0.9/lektor_chameleon.egg-info/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      323 2024-04-28 20:46:53.000000 lektor_chameleon-0.9/lektor_chameleon.egg-info/SOURCES.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2024-04-28 20:46:53.000000 lektor_chameleon-0.9/lektor_chameleon.egg-info/dependency_links.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       62 2024-04-28 20:46:53.000000 lektor_chameleon-0.9/lektor_chameleon.egg-info/entry_points.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      100 2024-04-28 20:46:53.000000 lektor_chameleon-0.9/lektor_chameleon.egg-info/requires.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       17 2024-04-28 20:46:53.000000 lektor_chameleon-0.9/lektor_chameleon.egg-info/top_level.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     2331 2024-04-28 20:28:26.000000 lektor_chameleon-0.9/lektor_chameleon.py
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1964 2024-04-28 20:28:31.000000 lektor_chameleon-0.9/pyproject.toml
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2024-04-28 20:46:53.308902 lektor_chameleon-0.9/setup.cfg
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-28 20:46:53.308902 lektor_chameleon-0.9/tests/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     5947 2024-04-28 20:26:44.000000 lektor_chameleon-0.9/tests/test_chameleon.py
```

### Comparing `lektor_chameleon-0.8/LICENSE.txt` & `lektor_chameleon-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lektor_chameleon-0.8/lektor_chameleon.py` & `lektor_chameleon-0.9/lektor_chameleon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,35 @@
 # Copyright (C) 2018-2024 H. Turgut Uyar <uyar@tekir.org>
 #
 # lektor-chameleon is released under the BSD license.
 # Read the included LICENSE.txt file for details.
 
-__version__ = "0.8"
+__version__ = "0.9"
 
 from functools import partial
 
 from chameleon import PageTemplateLoader
 from chameleon.loader import TemplateLoader
 from lektor.context import get_ctx
 from lektor.pluginsystem import Plugin
 from lektor.reporter import reporter
-from markupsafe import Markup
 
 
-_CONTEXT_FILTERS = {
-    "url", "asseturl", "markdown",
-}
-
-_STR_FILTERS = {
-    "capitalize", "center", "indent", "length", "lower", "replace", "title",
-    "trim", "truncate", "upper", "wordcount", "wordwrap",
-}
-
-_JINJA_ENV_FILTERS = {
-    "attr", "replace", "truncate", "wordwrap",
-}
-
-
-class Filter:
-    def __init__(self, name, func):
-        self.name = name
-        self.func = func
-        self.ctx = self.name in _CONTEXT_FILTERS
-        self.str = self.name in _STR_FILTERS
-
-    def __call__(self, *args, **kwargs):
-        return Filter(self.name, partial(self.func, *args, **kwargs))
-
-    def __rrshift__(self, x):
-        markup = self.str and hasattr(x, "html")
-        p = x.html if markup else x
-        t = self.func(p)
-        y = t.unescape() if hasattr(t, "unescape") else t
-        return Markup(y) if markup else y
+chameleon_load = TemplateLoader.load
 
 
-chameleon_load = TemplateLoader.load
+REG_FILTERS = [
+    "filesizeformat", "indent", "latformat", "latlongformat", "longformat",
+    "striptags", "tojson",
+]
+
+ENV_FILTERS = [
+    "asseturl", "dateformat", "datetimeformat", "markdown", "truncate", "url",
+    "wordwrap",
+]
 
 
 def load_template(self, filename, *args, **kwargs):
     ctx = get_ctx()
     if filename == ctx.source.datamodel.id + ".html":
         filename = ctx.source.datamodel.id + ".pt"
     template = chameleon_load(self, filename, *args, **kwargs)
@@ -60,32 +38,34 @@
 
 
 def render_template(self, name, pad=None, this=None, values=None, alt=None):
     if isinstance(name, list):
         name = name[0]
     ctx = self.make_default_tmpl_values(pad, this, values, alt, template=name)
     ctx.update(self.chameleon_env.globals)
-    for f_name, f_filter in self.chameleon_env.filters.items():
-        ctx[f_name] = f_filter(ctx) if f_filter.ctx else f_filter
+    ctx.update(self.chameleon_env.filters)
     template = self.chameleon_env.loader.load(name)
     return template(**ctx)
 
 
 class ChameleonEnvironment:
     def __init__(self, jinja_env) -> None:
         self.loader = PageTemplateLoader(jinja_env.loader.searchpath,
                                          auto_reload=True)
         self.globals = jinja_env.globals
-        self.filters = {n: Filter(n, f) for n, f in jinja_env.filters.items()}
-        for f_name in _JINJA_ENV_FILTERS:
-            self.filters[f_name] = self.filters[f_name](jinja_env)
+        self.filters = {}
+        for filter_name in REG_FILTERS:
+            self.filters[filter_name] = jinja_env.filters[filter_name]
+        for filter_name in ENV_FILTERS:
+            self.filters[filter_name] = partial(jinja_env.filters[filter_name],
+                                                jinja_env)
 
 
 class ChameleonPlugin(Plugin):
     name = "chameleon"
-    description = "Chameleon support for templating"
+    description = "Support for Chameleon templates."
 
     def on_setup_env(self, **extra):
         reporter.report_generic("Setting up to use Chameleon templates")
+        self.env.chameleon_env = ChameleonEnvironment(self.env.jinja_env)
         TemplateLoader.load = load_template
         self.env.__class__.render_template = render_template
-        self.env.chameleon_env = ChameleonEnvironment(self.env.jinja_env)
```

### Comparing `lektor_chameleon-0.8/pyproject.toml` & `lektor_chameleon-0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lektor-chameleon"
-version = "0.8"
+version = "0.9"
 description = "Chameleon template support for Lektor."
 readme = "README.rst"
 
 authors = [{name = "H. Turgut Uyar", email = "uyar@tekir.org"}]
 license = {file = "LICENSE.txt"}
 
 keywords = ["lektor", "plugin", "chameleon", "template"]
```

