# Comparing `tmp/micromanubot-0.4.0.tar.gz` & `tmp/micromanubot-0.4.1.tar.gz`

## Comparing `micromanubot-0.4.0.tar` & `micromanubot-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 micromanubot-0.4.0/.python-version
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 micromanubot-0.4.0/requirements-dev.lock
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 micromanubot-0.4.0/requirements.lock
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/.gitignore
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/umb.toml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/.umb/citations_cache.bib
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/.umb/figures_cache.json
--rw-r--r--   0        0        0    77827 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/.umb/images/sample-figure-bar-graph_tcm11-261608_w1024_n.jpg
--rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/assets/arxiv.sty
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/assets/orcid.pdf
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/1.introduction.tex
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/2.results.tex
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/3.discussion.tex
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/4.methods.tex
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/abstract.tex
--rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/arxiv.sty
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/imports.tex
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/main.aux
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/main.bbl
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/main.blg
--rw-r--r--   0        0        0    20129 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/main.log
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/main.out
--rw-r--r--   0        0        0   164568 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/main.pdf
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/main.tex
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/orcid.pdf
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/references.bib
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/supplement.tex
--rw-r--r--   0        0        0    77827 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/build/images/sample-figure-bar-graph_tcm11-261608_w1024_n.jpg
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/content/1.introduction.tex
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/content/2.results.tex
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/content/3.discussion.tex
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/content/4.methods.tex
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/content/abstract.tex
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/content/imports.tex
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/content/manual_references.bib
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 micromanubot-0.4.0/abc/content/supplement.tex
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/__main__.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/build.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/cite.py
--rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/cli.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/config.py
--rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/figures.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/install.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/new.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/pytinytex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/assets/__init__.py
--rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/assets/arxiv.sty
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/assets/orcid.pdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/build/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/build/main.tex
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/1.introduction.tex
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/2.results.tex
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/3.discussion.tex
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/4.methods.tex
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/__init__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/abstract.tex
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/imports.tex
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/manual_references.bib
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 micromanubot-0.4.0/src/micromanubot/template_data/content/supplement.tex
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 micromanubot-0.4.0/tests/test_build.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 micromanubot-0.4.0/tests/test_cite.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 micromanubot-0.4.0/tests/test_cli.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 micromanubot-0.4.0/tests/test_figures.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 micromanubot-0.4.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 micromanubot-0.4.0/LICENSE
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 micromanubot-0.4.0/README.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 micromanubot-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 micromanubot-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 micromanubot-0.4.1/.python-version
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 micromanubot-0.4.1/requirements-dev.lock
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 micromanubot-0.4.1/requirements.lock
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/.gitignore
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/umb.toml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/.umb/citations_cache.bib
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/.umb/figures_cache.json
+-rw-r--r--   0        0        0    77827 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/.umb/images/sample-figure-bar-graph_tcm11-261608_w1024_n.jpg
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/assets/arxiv.sty
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/assets/orcid.pdf
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/1.introduction.tex
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/2.results.tex
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/3.discussion.tex
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/4.methods.tex
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/abstract.tex
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/arxiv.sty
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/imports.tex
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/main.aux
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/main.bbl
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/main.blg
+-rw-r--r--   0        0        0    20129 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/main.log
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/main.out
+-rw-r--r--   0        0        0   164568 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/main.pdf
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/main.tex
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/orcid.pdf
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/references.bib
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/supplement.tex
+-rw-r--r--   0        0        0    77827 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/build/images/sample-figure-bar-graph_tcm11-261608_w1024_n.jpg
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/content/1.introduction.tex
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/content/2.results.tex
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/content/3.discussion.tex
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/content/4.methods.tex
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/content/abstract.tex
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/content/imports.tex
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/content/manual_references.bib
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 micromanubot-0.4.1/abc/content/supplement.tex
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/__main__.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/build.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/cite.py
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/cli.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/config.py
+-rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/figures.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/install.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/new.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/pytinytex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/assets/__init__.py
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/assets/arxiv.sty
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/assets/orcid.pdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/build/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/build/main.tex
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/1.introduction.tex
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/2.results.tex
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/3.discussion.tex
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/4.methods.tex
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/__init__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/abstract.tex
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/imports.tex
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/manual_references.bib
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 micromanubot-0.4.1/src/micromanubot/template_data/content/supplement.tex
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 micromanubot-0.4.1/tests/test_build.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 micromanubot-0.4.1/tests/test_cite.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 micromanubot-0.4.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 micromanubot-0.4.1/tests/test_figures.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 micromanubot-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 micromanubot-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 micromanubot-0.4.1/README.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 micromanubot-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 micromanubot-0.4.1/PKG-INFO
```

### Comparing `micromanubot-0.4.0/requirements-dev.lock` & `micromanubot-0.4.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/requirements.lock` & `micromanubot-0.4.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/.umb/images/sample-figure-bar-graph_tcm11-261608_w1024_n.jpg` & `micromanubot-0.4.1/abc/.umb/images/sample-figure-bar-graph_tcm11-261608_w1024_n.jpg`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/assets/arxiv.sty` & `micromanubot-0.4.1/abc/assets/arxiv.sty`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/assets/orcid.pdf` & `micromanubot-0.4.1/abc/assets/orcid.pdf`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/1.introduction.tex` & `micromanubot-0.4.1/abc/build/1.introduction.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/abstract.tex` & `micromanubot-0.4.1/abc/build/abstract.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/arxiv.sty` & `micromanubot-0.4.1/abc/build/arxiv.sty`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/imports.tex` & `micromanubot-0.4.1/abc/build/imports.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/main.aux` & `micromanubot-0.4.1/abc/build/main.aux`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/main.blg` & `micromanubot-0.4.1/abc/build/main.blg`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/main.log` & `micromanubot-0.4.1/abc/build/main.log`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/main.pdf` & `micromanubot-0.4.1/abc/build/main.pdf`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/main.tex` & `micromanubot-0.4.1/abc/build/main.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/orcid.pdf` & `micromanubot-0.4.1/abc/build/orcid.pdf`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/references.bib` & `micromanubot-0.4.1/abc/build/references.bib`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/build/images/sample-figure-bar-graph_tcm11-261608_w1024_n.jpg` & `micromanubot-0.4.1/abc/build/images/sample-figure-bar-graph_tcm11-261608_w1024_n.jpg`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/content/1.introduction.tex` & `micromanubot-0.4.1/abc/content/1.introduction.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/content/abstract.tex` & `micromanubot-0.4.1/abc/content/abstract.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/abc/content/imports.tex` & `micromanubot-0.4.1/abc/content/imports.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/build.py` & `micromanubot-0.4.1/src/micromanubot/build.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/cite.py` & `micromanubot-0.4.1/src/micromanubot/cite.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/cli.py` & `micromanubot-0.4.1/src/micromanubot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,14 @@
     if args.type in {"all", "pdf"}:
         micromanubot.install.check_pdflatex_bibtex_installed()
         micromanubot.build.build_latex_pdf(cwd)
     print("   [bold green]Finished[/] building the manuscript")
 
 
 def handle_install(args: argparse.Namespace) -> None:
-    micromanubot.install.check_extra_installed()
     is_installed = micromanubot.install.is_tinytex_installed()
     if is_installed and not args.force:
         print("TinyTeX already installed (use --force to reinstall)")
         return
     if is_installed and args.force:
         print("   [bold green]Removing[/] existing TinyTeX installation")
         micromanubot.install.uninstall_tinytex(args.root)
```

### Comparing `micromanubot-0.4.0/src/micromanubot/config.py` & `micromanubot-0.4.1/src/micromanubot/config.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/figures.py` & `micromanubot-0.4.1/src/micromanubot/figures.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/install.py` & `micromanubot-0.4.1/src/micromanubot/install.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/new.py` & `micromanubot-0.4.1/src/micromanubot/new.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/pytinytex.py` & `micromanubot-0.4.1/src/micromanubot/pytinytex.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/template_data/assets/arxiv.sty` & `micromanubot-0.4.1/src/micromanubot/template_data/assets/arxiv.sty`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/template_data/assets/orcid.pdf` & `micromanubot-0.4.1/src/micromanubot/template_data/assets/orcid.pdf`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/template_data/content/1.introduction.tex` & `micromanubot-0.4.1/src/micromanubot/template_data/content/1.introduction.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/template_data/content/abstract.tex` & `micromanubot-0.4.1/src/micromanubot/template_data/content/abstract.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/src/micromanubot/template_data/content/imports.tex` & `micromanubot-0.4.1/src/micromanubot/template_data/content/imports.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/tests/test_build.py` & `micromanubot-0.4.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/tests/test_cite.py` & `micromanubot-0.4.1/tests/test_cite.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/tests/test_cli.py` & `micromanubot-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/tests/test_figures.py` & `micromanubot-0.4.1/tests/test_figures.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/LICENSE` & `micromanubot-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/README.md` & `micromanubot-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.0/pyproject.toml` & `micromanubot-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "micromanubot"
-version = "0.4.0"
+version = "0.4.1"
 description = "A build tool for academic manuscripts"
 authors = [
     { name = "zietzm", email = "michael.zietz@gmail.com" }
 ]
 dependencies = [
     "tomlkit>=0.12.4",
     "pydantic>=2.7.1",
```

### Comparing `micromanubot-0.4.0/PKG-INFO` & `micromanubot-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: micromanubot
-Version: 0.4.0
+Version: 0.4.1
 Summary: A build tool for academic manuscripts
 Author-email: zietzm <michael.zietz@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Requires-Python: >=3.8
```

