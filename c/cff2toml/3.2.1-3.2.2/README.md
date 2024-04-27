# Comparing `tmp/cff2toml-3.2.1.tar.gz` & `tmp/cff2toml-3.2.2.tar.gz`

## Comparing `cff2toml-3.2.1.tar` & `cff2toml-3.2.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-3.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-3.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/__init__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/app.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/command_metadata_output.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/context_helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/about_command/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/about_command/about_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/change_command/__init__.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/change_command/change_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/view_command/__init__.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/cli/view_command/view_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/__init__.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/basic_model.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/agents/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/agents/authors/cff_entity_author.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/agents/authors/cff_person_author.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/agents/authors/pyproject_toml_author.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/agents/organizations/cff_entity.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/agents/people/cff_person.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/agents/people/human_name.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/files/__init__.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/files/cff_file.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/files/metadata_file.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/files/pyproject_toml_file.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/files/toml_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/files/synchronizers/__init__.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/__init__.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/conftest.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/temp_copied_file.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/agents/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/agents/authors/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/agents/authors/synchronizers/__init__.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/agents/organizations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/agents/people/__init__.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/agents/people/test_human_name_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/files/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/files/test_cff_file.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/files/test_metadata_file.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/files/test_pyproject_toml_file.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/files/test_toml_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/files/synchronizers/__init__.py
--rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 cff2toml-3.2.1/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 cff2toml-3.2.1/src/cff2toml/CITATION.cff
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-3.2.1/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-3.2.1/LICENSE
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 cff2toml-3.2.1/README.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 cff2toml-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 cff2toml-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-3.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-3.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/__init__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/app.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/command_metadata_output.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/context_helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/about_command/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/about_command/about_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/change_command/__init__.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/change_command/change_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/view_command/__init__.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/cli/view_command/view_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/__init__.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/basic_model.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/agents/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/agents/authors/cff_entity_author.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/agents/authors/cff_person_author.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/agents/authors/pyproject_toml_author.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/agents/organizations/cff_entity.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/agents/people/cff_person.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/agents/people/human_name.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/files/__init__.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/files/cff_file.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/files/metadata_file.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/files/pyproject_toml_file.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/files/toml_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/files/synchronizers/__init__.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/conftest.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/temp_copied_file.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/agents/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/agents/authors/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/agents/authors/synchronizers/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/agents/organizations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/agents/people/__init__.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/agents/people/test_human_name_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/files/__init__.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/files/test_cff_file.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/files/test_metadata_file.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/files/test_pyproject_toml_file.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/files/test_toml_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/files/synchronizers/__init__.py
+-rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 cff2toml-3.2.2/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 cff2toml-3.2.2/src/cff2toml/CITATION.cff
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-3.2.2/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-3.2.2/LICENSE
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 cff2toml-3.2.2/README.md
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 cff2toml-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 cff2toml-3.2.2/PKG-INFO
```

### Comparing `cff2toml-3.2.1/.github/workflows/python-publish.yml` & `cff2toml-3.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/cli/app.py` & `cff2toml-3.2.2/src/cff2toml/cli/app.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/cli/command_metadata_output.py` & `cff2toml-3.2.2/src/cff2toml/cli/command_metadata_output.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/cli/context_helpers.py` & `cff2toml-3.2.2/src/cff2toml/cli/context_helpers.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/cli/about_command/about_command.py` & `cff2toml-3.2.2/src/cff2toml/cli/about_command/about_command.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/cli/change_command/change_command.py` & `cff2toml-3.2.2/src/cff2toml/cli/change_command/change_command.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/cli/view_command/view_command.py` & `cff2toml-3.2.2/src/cff2toml/cli/view_command/view_command.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/models/basic_model.py` & `cff2toml-3.2.2/src/cff2toml/models/basic_model.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/models/metadata.py` & `cff2toml-3.2.2/src/cff2toml/models/metadata.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py` & `cff2toml-3.2.2/src/cff2toml/models/agents/authors/synchronizers/cff_and_pyproject_toml_author_synchronizer.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/models/agents/organizations/cff_entity.py` & `cff2toml-3.2.2/src/cff2toml/models/agents/organizations/cff_entity.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/models/agents/people/cff_person.py` & `cff2toml-3.2.2/src/cff2toml/models/agents/people/cff_person.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/models/agents/people/human_name.py` & `cff2toml-3.2.2/src/cff2toml/models/agents/people/human_name.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/models/files/cff_file.py` & `cff2toml-3.2.2/src/cff2toml/models/files/cff_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
     def save(self, file_path: Union[str, None] = None) -> None:
         if file_path is None:
             file_path = self.file_path
         if self._metadata is not None:
             try:
                 with open(file_path, 'w') as cff_file:
-                    yaml.safe_dump(self._metadata.to_dict(), cff_file)
+                    yaml.safe_dump(self._metadata.to_dict(),
+                                   cff_file, sort_keys=False)
             except:
                 raise SaveCffFileException(
                     f"Cannot save this CFF file: {file_path}")
         else:
             raise SaveCffFileException(
                 f"Cannot save this CFF file: {file_path} because there is no data.")
```

### Comparing `cff2toml-3.2.1/src/cff2toml/models/files/metadata_file.py` & `cff2toml-3.2.2/src/cff2toml/models/files/metadata_file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, List
 
 from pydantic import BaseModel
 
 from cff2toml.models.metadata import Metadata
 
 DEFAULT_DIR: str = '.'
 
@@ -20,7 +20,11 @@
 
     def delete_metadata(self, property_path: str) -> None:
         if self._metadata is not None:
             self._metadata.delete(property_path=property_path)
 
     def has_metadata(self, property_path: str) -> bool:
         return self._metadata.has(property_path=property_path)
+
+    @property
+    def metadata(self) -> Metadata:
+        return self._metadata
```

### Comparing `cff2toml-3.2.1/src/cff2toml/models/files/pyproject_toml_file.py` & `cff2toml-3.2.2/src/cff2toml/models/files/pyproject_toml_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/models/files/toml_file.py` & `cff2toml-3.2.2/src/cff2toml/models/files/toml_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Union
-import toml
+from typing import OrderedDict, Union
 from cff2toml.models.files.metadata_file import MetadataFile
+import tomlkit
 
 
 class LoadTomlFileException(Exception):
     pass
 
 
 class SaveTomlFileException(Exception):
@@ -14,25 +14,27 @@
 class TomlFile(MetadataFile):
 
     def __init__(self, file_path: str):
         super().__init__(file_path=file_path)
         self.file_path = file_path
         try:
             with open(self.file_path, 'r') as toml_file:
-                self._metadata.from_dict(toml.load(toml_file))
+                self._metadata.from_dict(
+                    OrderedDict(tomlkit.load(toml_file).value))
         except:
             raise LoadTomlFileException(
                 f"Cannot load this TOML file: {self.file_path}")
 
     def save(self, file_path: Union[str, None] = None) -> None:
         if file_path is None:
             file_path = self.file_path
         if self._metadata is not None:
             try:
                 with open(file_path, 'w') as toml_file:
-                    toml.dump(self._metadata.to_dict(), toml_file)
+                    tomlkit.dump(OrderedDict(self._metadata.to_dict()),
+                                 toml_file)
             except:
                 raise SaveTomlFileException(
                     f"Cannot save this TOML file: {file_path}")
         else:
             raise SaveTomlFileException(
                 f"Cannot save this TOML file: {file_path} because there is no data.")
```

### Comparing `cff2toml-3.2.1/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py` & `cff2toml-3.2.2/src/cff2toml/models/files/synchronizers/cff_and_pyproject_toml_file_synchronizer.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/tests/conftest.py` & `cff2toml-3.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/tests/temp_copied_file.py` & `cff2toml-3.2.2/tests/temp_copied_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-3.2.2/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-3.2.2/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py` & `cff2toml-3.2.2/tests/models/agents/authors/synchronizers/test_cff_and_pyproject_toml_author_synchronizer.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/tests/models/agents/people/test_human_name_parser.py` & `cff2toml-3.2.2/tests/models/agents/people/test_human_name_parser.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/tests/models/files/test_metadata_file.py` & `cff2toml-3.2.2/tests/models/files/test_metadata_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pytest import fixture
 from cff2toml.models.files.metadata_file import MetadataFile
 
 
 @fixture
 def dummy_metadata_file():
     metadata_file = MetadataFile()
-    metadata_file._metadata.from_dict({'some': {'nestedproperty': 'somedata'}})
+    metadata_file._metadata.from_dict(
+        {'some': {'nestedproperty': 'somedata'}, 'other': 'otherdata'})
     return metadata_file
 
 
 def test_get_metadata_for_existing_property(dummy_metadata_file):
     assert dummy_metadata_file.has_metadata('some.nestedproperty') == True
     assert dummy_metadata_file.get_metadata(
         'some.nestedproperty') == 'somedata'
```

### Comparing `cff2toml-3.2.1/tests/models/files/test_pyproject_toml_file.py` & `cff2toml-3.2.2/tests/models/files/test_pyproject_toml_file.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py` & `cff2toml-3.2.2/tests/models/files/synchronizers/test_cff_and_pyproject_toml_synchronizer.py`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/src/cff2toml/CITATION.cff` & `cff2toml-3.2.2/src/cff2toml/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
   A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 keywords:
   - Citation File Format
   - TOML
   - pyproject.toml
   - CITATION.cff
 license: Apache-2.0
-version: "3.2.1"
+version: "3.2.2"
```

### Comparing `cff2toml-3.2.1/LICENSE` & `cff2toml-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-3.2.1/README.md` & `cff2toml-3.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -62,7 +62,26 @@
 1. Improve CLI tool to view and change other metadata fields.
 2. Improve documentation of the underlying classes.
 3. Fix the output order so that it creates a more useful semantic ordering of propreties (not alphabetical).
 
 ## License
 
 `cff2toml` is distributed under the terms of the [Apache 2.0](https://spdx.org/licenses/Apache-2.0.html) license
+
+## Contribution
+
+Contributions in the form of feature requests, bug reports, bug fixes, tests, and feature implementations are welcome. To contribute code, please fork the project, and then do a pull request.
+
+### Developer Notes
+
+#### Buildiing Locally
+
+To build the tool locally, please follow the general advice from [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
+
+```
+python3 -m pip install --upgrade build
+python3 -m build
+```
+
+#### Deploying
+
+To deploy the tool, use the Github Action defined in .github/workflows/python-publish.yml
```

### Comparing `cff2toml-3.2.1/pyproject.toml` & `cff2toml-3.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "3.2.1"
+version = "3.2.2"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
     "Topic :: Utilities"
 ]
-dependencies = ["toml>=0.10.2", "PyYAML>=6.0.1", "pydash>=8.0.0", "pydantic>=2.6.4", "typer>=0.12.1"]
+dependencies = ["tomlkit>=0.12.4", "PyYAML>=6.0.1", "pydash>=8.0.0", "pydantic>=2.6.4", "typer>=0.12.1"]
 
 [project.scripts]
 cff2toml = "cff2toml.main:start"
 
 [project.urls]
 Documentation = "https://github.com/willynilly/cff2toml#readme"
 Issues = "https://github.com/willynilly/cff2toml/issues"
```

### Comparing `cff2toml-3.2.1/PKG-INFO` & `cff2toml-3.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 3.2.1
+Version: 3.2.2
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -26,15 +26,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: pydash>=8.0.0
 Requires-Dist: pyyaml>=6.0.1
-Requires-Dist: toml>=0.10.2
+Requires-Dist: tomlkit>=0.12.4
 Requires-Dist: typer>=0.12.1
 Provides-Extra: testing
 Requires-Dist: pytest>=8.1.1; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # cff2toml
 
@@ -100,7 +100,26 @@
 1. Improve CLI tool to view and change other metadata fields.
 2. Improve documentation of the underlying classes.
 3. Fix the output order so that it creates a more useful semantic ordering of propreties (not alphabetical).
 
 ## License
 
 `cff2toml` is distributed under the terms of the [Apache 2.0](https://spdx.org/licenses/Apache-2.0.html) license
+
+## Contribution
+
+Contributions in the form of feature requests, bug reports, bug fixes, tests, and feature implementations are welcome. To contribute code, please fork the project, and then do a pull request.
+
+### Developer Notes
+
+#### Buildiing Locally
+
+To build the tool locally, please follow the general advice from [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
+
+```
+python3 -m pip install --upgrade build
+python3 -m build
+```
+
+#### Deploying
+
+To deploy the tool, use the Github Action defined in .github/workflows/python-publish.yml
```

