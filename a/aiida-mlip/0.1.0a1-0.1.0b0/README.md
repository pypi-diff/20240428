# Comparing `tmp/aiida_mlip-0.1.0a1.tar.gz` & `tmp/aiida_mlip-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_mlip-0.1.0a1.tar", max compression
+gzip compressed data, was "aiida_mlip-0.1.0b0.tar", max compression
```

## Comparing `aiida_mlip-0.1.0a1.tar` & `aiida_mlip-0.1.0b0.tar`

### file list

```diff
@@ -1,10 +1,21 @@
--rw-r--r--   0        0        0     1533 2024-02-13 14:34:05.438251 aiida_mlip-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     6938 2024-02-13 14:34:05.438251 aiida_mlip-0.1.0a1/README.md
--rw-r--r--   0        0        0       98 2024-02-13 14:34:05.438251 aiida_mlip-0.1.0a1/aiida_mlip/__init__.py
--rw-r--r--   0        0        0     2963 2024-02-13 14:34:05.442251 aiida_mlip-0.1.0a1/aiida_mlip/calculations.py
--rw-r--r--   0        0        0     1601 2024-02-13 14:34:05.442251 aiida_mlip-0.1.0a1/aiida_mlip/cli.py
--rw-r--r--   0        0        0     2679 2024-02-13 14:34:05.442251 aiida_mlip-0.1.0a1/aiida_mlip/data/__init__.py
--rw-r--r--   0        0        0     2764 2024-02-13 14:34:05.442251 aiida_mlip-0.1.0a1/aiida_mlip/helpers.py
--rw-r--r--   0        0        0     1922 2024-02-13 14:34:05.442251 aiida_mlip-0.1.0a1/aiida_mlip/parsers.py
--rw-r--r--   0        0        0     2701 2024-02-13 14:34:05.442251 aiida_mlip-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     7994 1970-01-01 00:00:00.000000 aiida_mlip-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/LICENSE
+-rw-r--r--   0        0        0     8039 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/README.md
+-rw-r--r--   0        0        0       87 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/__init__.py
+-rw-r--r--   0        0        0     9272 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/base.py
+-rw-r--r--   0        0        0     4497 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/geomopt.py
+-rw-r--r--   0        0        0     4409 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/md.py
+-rw-r--r--   0        0        0     3496 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/singlepoint.py
+-rw-r--r--   0        0        0       43 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/data/__init__.py
+-rw-r--r--   0        0        0     4349 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/data/config.py
+-rw-r--r--   0        0        0     8231 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/data/model.py
+-rw-r--r--   0        0        0       40 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/helpers/__init__.py
+-rw-r--r--   0        0        0     2826 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/helpers/converters.py
+-rw-r--r--   0        0        0     2650 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/helpers/help_load.py
+-rw-r--r--   0        0        0       34 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/__init__.py
+-rw-r--r--   0        0        0     2332 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/base_parser.py
+-rw-r--r--   0        0        0     3643 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/md_parser.py
+-rw-r--r--   0        0        0     2563 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/opt_parser.py
+-rw-r--r--   0        0        0     2891 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/sp_parser.py
+-rw-r--r--   0        0        0     3344 2024-04-28 20:47:33.741153 aiida_mlip-0.1.0b0/pyproject.toml
+-rw-r--r--   0        0        0     9132 1970-01-01 00:00:00.000000 aiida_mlip-0.1.0b0/PKG-INFO
```

### Comparing `aiida_mlip-0.1.0a1/LICENSE` & `aiida_mlip-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0a1/aiida_mlip/parsers.py` & `aiida_mlip-0.1.0b0/aiida_mlip/parsers/sp_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,106 @@
 """
 Parsers provided by aiida_mlip.
-
-Register parsers via the "aiida.parsers" entry point in setup.json.
 """
 
+from pathlib import Path
+
+from ase.io import read
+
 from aiida.common import exceptions
 from aiida.engine import ExitCode
-from aiida.orm import SinglefileData
-from aiida.parsers.parser import Parser
+from aiida.orm import Dict, SinglefileData
+from aiida.orm.nodes.process.process import ProcessNode
 from aiida.plugins import CalculationFactory
 
-DiffCalculation = CalculationFactory("mlip")
+from aiida_mlip.helpers.converters import convert_numpy
+from aiida_mlip.parsers.base_parser import BaseParser
+
+singlePointCalculation = CalculationFactory("janus.sp")
 
 
-class DiffParser(Parser):
+class SPParser(BaseParser):
     """
     Parser class for parsing output of calculation.
+
+    Parameters
+    ----------
+    node : aiida.orm.nodes.process.process.ProcessNode
+        ProcessNode of calculation.
+
+    Methods
+    -------
+    __init__(node: aiida.orm.nodes.process.process.ProcessNode)
+        Initialize the SPParser instance.
+
+    parse(**kwargs: Any) -> int:
+        Parse outputs, store results in the database.
+
+    Returns
+    -------
+    int
+        An exit code.
+
+    Raises
+    ------
+    exceptions.ParsingError
+        If the ProcessNode being passed was not produced by a singlePointCalculation.
     """
 
-    def __init__(self, node):
+    def __init__(self, node: ProcessNode):
         """
-        Initialize Parser instance
-
-        Checks that the ProcessNode being passed was produced by a DiffCalculation.
+        Check that the ProcessNode being passed was produced by a `Singlepoint`.
 
-        :param node: ProcessNode of calculation
-        :param type node: :class:`aiida.orm.nodes.process.process.ProcessNode`
+        Parameters
+        ----------
+        node : aiida.orm.nodes.process.process.ProcessNode
+            ProcessNode of calculation.
         """
         super().__init__(node)
-        if not issubclass(node.process_class, DiffCalculation):
-            raise exceptions.ParsingError("Can only parse DiffCalculation")
 
-    def parse(self, **kwargs):
+        if not issubclass(node.process_class, singlePointCalculation):
+            raise exceptions.ParsingError("Can only parse `Singlepoint` calculations")
+
+    def parse(self, **kwargs) -> int:
         """
-        Parse outputs, store results in database.
+        Parse outputs, store results in the database.
 
-        :returns: an exit code, if parsing fails (or nothing if parsing succeeds)
+        Parameters
+        ----------
+        **kwargs : Any
+            Any keyword arguments.
+
+        Returns
+        -------
+        int
+            An exit code.
         """
-        output_filename = self.node.get_option("output_filename")
+
+        exit_code = super().parse(**kwargs)
+
+        if exit_code != ExitCode(0):
+            return exit_code
+
+        xyz_output = (self.node.inputs.out).value
 
         # Check that folder content is as expected
         files_retrieved = self.retrieved.list_object_names()
-        files_expected = [output_filename]
-        # Note: set(A) <= set(B) checks whether A is a subset of B
-        if not set(files_expected) <= set(files_retrieved):
+
+        files_expected = {xyz_output}
+        if not files_expected.issubset(files_retrieved):
             self.logger.error(
                 f"Found files '{files_retrieved}', expected to find '{files_expected}'"
             )
             return self.exit_codes.ERROR_MISSING_OUTPUT_FILES
 
-        # add output file
-        self.logger.info(f"Parsing '{output_filename}'")
-        with self.retrieved.open(output_filename, "rb") as handle:
-            output_node = SinglefileData(file=handle)
-        self.out("mlip", output_node)
+        # Add output file to the outputs
+        self.logger.info(f"Parsing '{xyz_output}'")
+
+        with self.retrieved.open(xyz_output, "rb") as handle:
+            self.out("xyz_output", SinglefileData(file=handle))
+
+        content = read(Path(self.node.get_remote_workdir(), xyz_output))
+        results = convert_numpy(content.todict())
+        results_node = Dict(results)
+        self.out("results_dict", results_node)
 
         return ExitCode(0)
```

### Comparing `aiida_mlip-0.1.0a1/pyproject.toml` & `aiida_mlip-0.1.0b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiida-mlip"
-version = "0.1.0a1"
+version = "0.1.0b0"
 description = "machine learning interatomic potentials aiida plugin"
 authors = [
     "Federica Zanca",
     "Elliott Kasoar",
     "Jacob Wilkins",
     "Alin M. Elena",
 ]
@@ -24,18 +24,20 @@
 
 [tool.poetry.urls]
 "Source" = "https://github.com/aiidateam/aiida-mlip"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiida-core = "^2.5"
+ase = "^3.22.1"
 voluptuous = "^0.14"
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = "^7.4.1"}
+janus-core = "^0.2.0b4"
 pgtest = "^1.3.2"
 pytest = "^8.0"
 pytest-cov = "^4.1.0"
 tox = "^4.12.1"
 wheel = "^0.42"
 
 [tool.poetry.group.pre-commit]
@@ -46,60 +48,83 @@
 pylint = "^2.15.10"
 
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 furo = "^2024.1.29"
 markupsafe = "<2.1"
+numpydoc = "^1.6.0"
 sphinx = "^7.2.6"
 sphinxcontrib-contentui = "^0.2.5"
 sphinxcontrib-details-directive = "^0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins] # Optional super table
 
 [tool.poetry.plugins."aiida.data"]
-"mlip" = "aiida_mlip.data:DiffParameters"
+"janus.modeldata" = "aiida_mlip.data.model:ModelData"
+"janus.config" = "aiida_mlip.data.config:JanusConfigfile"
 
 [tool.poetry.plugins."aiida.calculations"]
-"mlip" = "aiida_mlip.calculations:DiffCalculation"
+"janus.sp" = "aiida_mlip.calculations.singlepoint:Singlepoint"
+"janus.opt" = "aiida_mlip.calculations.geomopt:GeomOpt"
+"janus.md" = "aiida_mlip.calculations.md:MD"
 
 [tool.poetry.plugins."aiida.parsers"]
-"mlip" = "aiida_mlip.parsers:DiffParser"
+"janus.sp_parser" = "aiida_mlip.parsers.sp_parser:SPParser"
+"janus.opt_parser" = "aiida_mlip.parsers.opt_parser:GeomOptParser"
+"janus.md_parser" = "aiida_mlip.parsers.md_parser:MDParser"
 
-[tool.poetry.plugins."aiida.cmdline.data"]
-"mlip" = "aiida_mlip.cli:data_cli"
+[tool.black]
+line-length = 88
 
 [tool.pylint.format]
-max-line-length = 125
+max-line-length = 88
 
 [tool.pylint.messages_control]
 disable = [
     "too-many-ancestors",
     "invalid-name",
     "duplicate-code",
 ]
 
 [tool.pytest.ini_options]
 # Configuration for [pytest](https://docs.pytest.org)
 python_files = "test_*.py example_*.py"
+addopts = '--cov-report xml'
 filterwarnings = [
     "ignore::DeprecationWarning:aiida:",
     "ignore:Creating AiiDA configuration folder:",
     "ignore::DeprecationWarning:plumpy:",
     "ignore::DeprecationWarning:yaml:",
 ]
+pythonpath = ["."]
 
 [tool.coverage.run]
 # Configuration of [coverage.py](https://coverage.readthedocs.io)
 # reporting which lines of your plugin are covered by tests
 source=["aiida_mlip"]
 
 [tool.isort]
 # Configuration of [isort](https://isort.readthedocs.io)
-line_length = 120
 force_sort_within_sections = true
+line_length = 88
+profile = "black"
 sections = ['FUTURE', 'STDLIB', 'THIRDPARTY', 'AIIDA', 'FIRSTPARTY', 'LOCALFOLDER']
 known_aiida = ['aiida']
+
+[tool.numpydoc_validation]
+# report on all checks, except the below
+checks = [
+    "all",
+    "EX01",
+    "SA01",
+    "ES01",
+]
+# Don't report on objects that match any of these regex
+exclude = [
+    ".__weakref__$",
+    ".__repr__$",
+]
```

