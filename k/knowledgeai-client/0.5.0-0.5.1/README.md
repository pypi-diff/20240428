# Comparing `tmp/knowledgeai_client-0.5.0.tar.gz` & `tmp/knowledgeai_client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgeai_client-0.5.0.tar", max compression
+gzip compressed data, was "knowledgeai_client-0.5.1.tar", max compression
```

## Comparing `knowledgeai_client-0.5.0.tar` & `knowledgeai_client-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1080 2024-02-12 12:45:05.581822 knowledgeai_client-0.5.0/LICENSE
--rw-r--r--   0        0        0     7385 2024-04-19 14:53:31.500483 knowledgeai_client-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-02-12 12:45:05.582349 knowledgeai_client-0.5.0/knowledgeai/__init__.py
--rw-r--r--   0        0        0      392 2024-04-19 14:53:31.499925 knowledgeai_client-0.5.0/knowledgeai/client/__init__.py
--rw-r--r--   0        0        0     5050 2024-04-19 14:49:37.775006 knowledgeai_client-0.5.0/knowledgeai/client/admin.py
--rw-r--r--   0        0        0    12964 2024-04-19 15:20:04.932119 knowledgeai_client-0.5.0/knowledgeai/client/client.py
--rw-r--r--   0        0        0     2044 2024-04-19 15:19:14.290191 knowledgeai_client-0.5.0/knowledgeai/client/schema.py
--rw-r--r--   0        0        0     4465 2024-04-19 14:59:02.915726 knowledgeai_client-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8212 1970-01-01 00:00:00.000000 knowledgeai_client-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-02-12 12:45:05.000000 knowledgeai_client-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7385 2024-04-28 11:41:59.000000 knowledgeai_client-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-02-12 12:45:05.000000 knowledgeai_client-0.5.1/knowledgeai/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-28 11:41:59.000000 knowledgeai_client-0.5.1/knowledgeai/client/__init__.py
+-rw-r--r--   0        0        0     5208 2024-04-22 07:11:20.000000 knowledgeai_client-0.5.1/knowledgeai/client/admin.py
+-rw-r--r--   0        0        0    13271 2024-04-28 11:29:35.000000 knowledgeai_client-0.5.1/knowledgeai/client/client.py
+-rw-r--r--   0        0        0     2044 2024-04-19 15:19:14.000000 knowledgeai_client-0.5.1/knowledgeai/client/schema.py
+-rw-r--r--   0        0        0     4252 2024-04-28 11:41:59.000000 knowledgeai_client-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8212 1970-01-01 00:00:00.000000 knowledgeai_client-0.5.1/PKG-INFO
```

### Comparing `knowledgeai_client-0.5.0/LICENSE` & `knowledgeai_client-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledgeai_client-0.5.0/README.md` & `knowledgeai_client-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Avvia Intelligence - KnowledgeAI Python Client
 
-Version: 0.5.0, (c) 2024 Arvato Systems
+Version: 0.5.1, (c) 2024 Arvato Systems
 
 This library is designed to provide easy access to the KnowledgeAI backend service. It enables users to manage projects, upload documents, and perform various tasks programmatically. The client offers an intuitive interface for seamless integration into Python applications.
 
 ## Installation
 ```bash
 pip install knowledgeai-client
 ```
```

### Comparing `knowledgeai_client-0.5.0/knowledgeai/client/admin.py` & `knowledgeai_client-0.5.1/knowledgeai/client/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import logging
-from typing import Any, List
+from typing import Any
 
 import requests
 from requests.models import Response
 
 from knowledgeai.client import User
 
 log: logging.Logger = logging.getLogger(__name__)
@@ -20,22 +20,23 @@
     def __init__(self, url: str, admin_api_key: str, timeout: int = 90) -> None:
         """
         Constructor for the KnowledgeAIAdminClient.
 
         Args:
             url (str): The base URL of the Aila Knowledge API.
             admin_api_key (str): The API key for the admin user.
-            timeout (int, optional): The timeout for the HTTP requests. Defaults to 90.
+            timeout (int, optional): The timeout for the HTTP requests.
+            Defaults to 90.
         """
 
         self.url: str = url
         self.api_key: str = admin_api_key
         self.timeout = timeout
 
-    def list_users(self) -> List[User]:
+    def list_users(self) -> list[User]:
         """
         Method to list all users.
 
         Returns:
             List[User]: A list of User objects.
 
         Raises:
@@ -47,14 +48,15 @@
             ...     print(user.name)
         """
 
         url: str = self.url + "/admin/user/"
         headers: dict[str, str] = {
             "accept": "application/json",
             "Authorization": self.api_key,
+            "x-apikey": self.api_key,
         }
         response: Response = requests.get(url, headers=headers, timeout=self.timeout)
         response.raise_for_status()
         return [User(**user) for user in response.json()]
 
     def create_user(self, user: User) -> User:
         """
@@ -81,14 +83,15 @@
             >>> client.create_user(user)
         """
 
         url: str = self.url + "/admin/user"
         headers: dict[str, str] = {
             "accept": "application/json",
             "Authorization": self.api_key,
+            "x-apikey": self.api_key,
             "Content-Type": "application/x-www-form-urlencoded",
         }
         data: dict[str, Any] = {
             "name": user.name,
             "company": user.company,
             "language": user.language.value,
             "plan": user.plan.value,
@@ -120,14 +123,15 @@
             >>> print(user.name)
         """
 
         url: str = self.url + "/admin/user/" + api_key
         headers: dict[str, str] = {
             "accept": "application/json",
             "Authorization": self.api_key,
+            "x-apikey": self.api_key,
         }
         response: Response = requests.get(url, headers=headers, timeout=self.timeout)
         response.raise_for_status()
         return User(**response.json())
 
     def update_user(self, user: User) -> User:
         """
@@ -148,14 +152,15 @@
             >>> client.update_user(user)
         """
 
         url: str = self.url + "/admin/user/" + user.api_key
         headers: dict[str, str] = {
             "accept": "application/json",
             "Authorization": self.api_key,
+            "x-apikey": self.api_key,
             "Content-Type": "application/x-www-form-urlencoded",
         }
         data = {
             "api_key": user.api_key,
             "name": user.name,
             "company": user.company,
             "language": user.language.value,
```

### Comparing `knowledgeai_client-0.5.0/knowledgeai/client/client.py` & `knowledgeai_client-0.5.1/knowledgeai/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 import os
 from pathlib import Path
-from typing import Any, List, Optional
+from typing import Any
 
 import httpx
 import magic
 from httpx import Response
 from tqdm import tqdm
 
 from knowledgeai.client import (
@@ -22,40 +22,42 @@
 )
 
 log: logging.Logger = logging.getLogger(__name__)
 limits = httpx.Limits(max_keepalive_connections=20, max_connections=None)
 
 
 class KnowledgeAIClient:
-    def __init__(self, url: str, api_key: str, timeout: int = 30) -> None:
+    def __init__(self, url: str, api_key: str, timeout: int = 90) -> None:
         self.url: str = url
         self.api_key: str = api_key
         self.timeout = timeout
 
     @staticmethod
-    def read_files_from_directory(directory: str) -> List[Path]:
+    def read_files_from_directory(directory: str) -> list[Path]:
         current_directory = Path(directory)
-        files = []
-        for file in os.listdir(directory):
-            if Path.is_file(current_directory / file):
-                files.append(current_directory / file)
+        files: list[Path] = [
+            current_directory / file
+            for file in os.listdir(directory)
+            if Path.is_file(current_directory / file)
+        ]
         return files
 
     def _api_call(
         self,
         method: HttpMethod,
         url: str,
-        data: Optional[Any] = None,
-        params: Optional[Any] = None,
-        headers: Optional[dict[str, str]] = None,
+        data: Any | None = None,
+        params: Any | None = None,
+        headers: dict[str, str] | None = None,
         form: bool = True,
     ) -> Response:
         headers_default: dict[str, str] = {
             "accept": "application/json",
             "Authorization": self.api_key,
+            "x-apikey": self.api_key,
         }
 
         if form:
             headers_default["Content-Type"] = "application/x-www-form-urlencoded"
 
         with httpx.Client(
             limits=limits,
@@ -92,28 +94,34 @@
         Raises:
             requests.exceptions.RequestException: If an error occurs while uploading
             the documents.
 
         Example:
           >>> client.upload_directory("project_id", "/path/to/directory", "admin,user")
         """
-        files: List[Path] = self.read_files_from_directory(directory)
+        files: list[Path] = self.read_files_from_directory(directory)
         self.index_documents(project_id, files, roles)
 
     def index_documents(
-        self, project_id: int, files: List[Path], roles: str = "user"
+        self,
+        project_id: int,
+        files: list[Path],
+        roles: str = "user",
+        timeout: int = 300,
     ) -> None:
         """
         Uploads multiple documents to the specified project.
 
         Args:
             project_id (str): The ID of the project to upload the documents to.
             files (List[str]): A list of file paths to upload.
             roles (str, optional): The roles to assign to the uploaded documents.
                 Comma separated list, defaults to "user".
+            timeout (int, optional): set the timeout in seconds for the indexing. Use
+                at least 300s for PDF documents.
 
         Returns:
             None
 
         Raises:
             requests.exceptions.RequestException: If an error occurs while uploading
             the documents.
@@ -126,18 +134,19 @@
         """
         url: str = "/index/document"
         filesp = tqdm(files)
 
         headers: dict[str, str] = {
             "accept": "application/json",
             "Authorization": self.api_key,
+            "x-apikey": self.api_key,
         }
 
         with httpx.Client(
-            limits=limits, base_url=self.url, headers=headers, timeout=self.timeout
+            limits=limits, base_url=self.url, headers=headers, timeout=timeout
         ) as client:
             for file in filesp:
                 log.debug("Uploading file: %s", file)
                 upload_file = {
                     "file": (
                         file.name,
                         open(file, "rb"),  # noqa: SIM115, PTH123
@@ -153,15 +162,15 @@
                     files=upload_file,
                 )
                 response.raise_for_status()
 
                 log.debug(msg=response.content)
 
     def index_urls(
-        self, project_id: int, index_urls: List[str], roles: Optional[str]
+        self, project_id: int, index_urls: list[str], roles: str | None
     ) -> None:
         """
         Indexes the specified URL to the specified project.
 
         Args:
             project_id (str): The ID of the project to index the URL to.
             url (str): The URLs to index.
@@ -177,15 +186,15 @@
         Example:
           >>> client.index_url("project_id", "https://www.example.com", roles="user")
         """
         url = "/index/urls"
         data = {"project_id": project_id, "urls": index_urls, "roles": roles}
         self._api_call(HttpMethod.POST, url, data=data)
 
-    def list_projects(self) -> List[Project]:
+    def list_projects(self) -> list[Project]:
         """
         Lists all projects.
 
         Returns:
             List[Project]: A list of projects.
 
         Raises:
@@ -193,15 +202,15 @@
 
         Example:
             >>> projects = client.list_projects()
             >>> for project in projects:
             ...     print(project.name)
         """
         url: str = "/project/"
-        response = self._api_call(HttpMethod.GET, url, form=False)
+        response: Response = self._api_call(HttpMethod.GET, url, form=False)
 
         return [Project(**project) for project in response.json()]
 
     def get_project(self, project_id: int, with_documents: bool = False) -> Project:
         """
         Gets the project with the specified ID.
 
@@ -218,16 +227,16 @@
             requests.exceptions.RequestException: If an error occurs.
 
         Example:
             >>> project = client.get_project(1)
             >>> print(project.name)
         """
         url: str = "/project/" + str(project_id)
-        data = {"with_documents": with_documents}
-        response = self._api_call(HttpMethod.GET, url, params=data)
+        data: dict[str, bool] = {"with_documents": with_documents}
+        response: Response = self._api_call(HttpMethod.GET, url, params=data)
 
         project = response.json()
         return Project(**project)
 
     def create_project(
         self,
         project_name: str,
@@ -256,25 +265,25 @@
 
         Example:
             >>> project = client.create_project("New Project")
             >>> print(project.name)
         """
         url: str = "/project/create"
 
-        data = {
+        data: dict[str, str] = {
             "name": project_name,
             "language": language.value,
             "llm": llm.value,
             "prompt": "x",
         }
 
         if prompt:
             data["prompt"] = prompt
 
-        response = self._api_call(HttpMethod.POST, url, data=data)
+        response: Response = self._api_call(HttpMethod.POST, url, data=data)
         project = response.json()
         return Project(**project)
 
     def update_project(self, project: Project) -> Response:
         """Updates the specified project.
 
         Args:
@@ -324,16 +333,16 @@
         Example:
             >>> project = client.update_project_configuration(
                     1, ProjectConfigKey.WELCOME_MESSAGE, "value"
                 )
         """
 
         url: str = "/project/" + str(project_id) + "/configuration/" + key.value
-        data = {"value": value}
-        response = self._api_call(HttpMethod.PUT, url, data=data)
+        data: dict[str, str] = {"value": value}
+        response: Response = self._api_call(HttpMethod.PUT, url, data=data)
 
         return Project(**response.json())
 
     def ask(self, project_id: int, question: str) -> AskResponse:
         """Asks a question to the specified project.
 
         Args:
@@ -353,31 +362,31 @@
 
         url: str = "/chat/ask"
         data = {
             "project_id": project_id,
             "question": question,
         }
 
-        response = self._api_call(HttpMethod.POST, url, data=data)
+        response: Response = self._api_call(HttpMethod.POST, url, data=data)
         content = json.loads(response.content)
 
-        references: List[SourceDocument] = []
-        for reference in content["source_documents"]:
-            references.append(SourceDocument(**reference))
+        references: list[SourceDocument] = [
+            SourceDocument(**reference) for reference in content["source_documents"]
+        ]
 
         return AskResponse(
             question=content["question"],
             answer=content["answer"],
             source_paragraphs=content["source_paragraphs"],
             source_documents=references,
         )
 
     def retrieve(
         self, project_id: int, query: str, retrieval_type: Retriever = Retriever.default
-    ) -> List[RetrievedDocument]:
+    ) -> list[RetrievedDocument]:
         """Retrieves documents for the specified project.
 
         Args:
 
             project_id (int):
                 The ID of the project to retrieve documents from.
             query (str):
@@ -400,15 +409,15 @@
         url: str = "/index/retrieve"
         data = {
             "project_id": project_id,
             "query": query,
             "retriever_type": retrieval_type.value,
         }
 
-        response = self._api_call(HttpMethod.POST, url, data=data)
+        response: Response = self._api_call(HttpMethod.POST, url, data=data)
         content = json.loads(response.content)
 
-        references: List[RetrievedDocument] = []
-        for reference in content["documents"]:
-            references.append(RetrievedDocument(**reference))
+        references: list[RetrievedDocument] = [
+            RetrievedDocument(**reference) for reference in content["documents"]
+        ]
 
         return references
```

### Comparing `knowledgeai_client-0.5.0/knowledgeai/client/schema.py` & `knowledgeai_client-0.5.1/knowledgeai/client/schema.py`

 * *Files identical despite different names*

### Comparing `knowledgeai_client-0.5.0/pyproject.toml` & `knowledgeai_client-0.5.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,150 +1,122 @@
 [tool.poetry]
-authors = ["Arvato Systems"]
+authors     = ["Arvato Systems"]
 description = "A python client for the Avvia Intelligence - Knowledge AI Rest API"
-homepage = "https://github.com/arvato-systems-aila-solutions/KnowledgeAI-Python-Client"
-keywords = [
-    "AI",
-    "Knowledge Retrieval",
-    "arvato systems",
-    "avvia intelligence",
-    "knowledgeai",
-]
-license = "MIT"
-name = "knowledgeai-client"
-packages = [{ include = "knowledgeai", from = "." }]
-readme = "README.md"
-version = "0.5.0"
+homepage    = "https://github.com/arvato-systems-aila-solutions/KnowledgeAI-Python-Client"
+keywords    = ["AI", "Knowledge Retrieval", "arvato systems", "avvia intelligence", "knowledgeai"]
+license     = "MIT"
+name        = "knowledgeai-client"
+packages    = [{ include = "knowledgeai", from = "." }]
+readme      = "README.md"
+version     = "0.5.1"
 
 [tool.poetry.dependencies]
 python = ">=3.11"
 
-httpx         = "0.27.0"
-pydantic      = "2.7.0"
+httpx             = "0.27.0"
+pydantic          = "2.7.0"
 pydantic-settings = "2.2.1"
-python-iso639 = "2024.2.7"
-python-magic  = "0.4.27"
-tqdm          = "4.66.2"
+python-iso639     = "2024.2.7"
+python-magic      = "0.4.27"
+tqdm              = "4.66.2"
 
 
 [tool.poetry.group.dev.dependencies]
-detect-secrets    = "1.4.0"
-mypy              = "1.9.0"
-pre-commit        = "3.7.0"
-ruff              = "0.4.1"
-types-requests    = "2.31.0.20240406"
-types-tqdm        = "4.66.0.20240417"
+detect-secrets = "1.4.0"
+isort          = "5.13.2"
+mypy           = "1.9.0"
+pre-commit     = "3.7.0"
+ruff           = "0.4.1"
+types-requests = "2.31.0.20240406"
+types-tqdm     = "4.66.0.20240417"
 
 
 [tool.poetry.group.test.dependencies]
 codecov       = "2.1.13"
 coverage      = "7.4.4"
 pytest        = "8.1.1"
 pytest-dotenv = "0.5.2"
 
 [tool.pytest.ini_options]
 cache_dir = ".cache/pytest"
 testpaths = ["tests"]
 
 
 [tool.ruff]
-cache-dir      = ".cache/ruff"
-line-length    = 88
+cache-dir = ".cache/ruff"
+indent-width = 4
+line-length = 88
 target-version = "py311"
-# Rules: https://beta.ruff.rs/docs/rules
-# If you violate a rule, lookup the rule on the Rules page in ruff docs.
-# Many rules have links you can click with a explanation of the rule and how to fix it.
-# If there isn't a link, go to the project the rule was source from (e.g. flake8-bugbear)
-# and review it's docs for the corresponding rule.
-# If you're still confused, ask a fellow developer for assistance.
-# You can also run "ruff rule <rule>" to explain a rule on the command line, without a browser or internet access.
-extend-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".git-rewrite",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pyenv",
-    ".pytest_cache",
-    ".python_packages",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    ".vscode",
-    "__pycache__",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "site-packages",
-    "venv",
-]
-lint.select = [
-    "A",   # flake8-builtins
-    "ARG", # flake8-unused-arguments
-    "B",   # flake8-bugbear
-    "C4",  # flake8-comprehensions
-    "E",   # pycodestyle
-    "EXE", # flake8-executable,
-    "F",   # Pyflakes
-    "G",   # flake8-logging-format
-    "ISC", # flake8-implicit-str-concat
-    "PGH", # pygrep-hooks
-    "PIE", # flake8-pie
-    "PLC", # Pylint Convention
-    "PLE", # Pylint Errors
-    "PLW", # Pylint Warnings
-    "PT",  # flake8-pytest-style
-    "PTH", # flake8-use-pathlib
-    "RET", # flake8-return
-    "RSE", # flake8-raise
-    "RUF", # Ruff-specific rules
-    "SIM", # flake8-simplify
-    "T10", # flake8-debugger
-    "T20", # flake8-print
-    "TID", # flake8-tidy-imports
-    "W",   # Warning
+extend-exclude = [".cache", ".venv", ".venv.mac", "build", "dist"]
+ignore = [
+    "PT011",   # pytest-raises-too-broad
+    "PT012",   # pytest.raises() block should contain a single simple statement
+    "ISC001",  # Implicit string concatenation
+    "PLR0913", # Too many arguments in function
+    "RUF100",  # unused noqa
+    "N805",    # First argument of a method should be named `self`"
+    "N818",    # Exception name {name} should be named with an Error suffix
+    "N811",    # Constant {name} imported as non-constant {asname}
+    "RUF012",  # Mutable class attributes should be annotated with typing.ClassVar
+    "SIM300",  # Yoda conditions are discouraged, use {suggestion} instead
+    "C",
 ]
-# Linting error codes to ignore
-lint.ignore = [
-    "PT011",  # pytest-raises-too-broad
-    "PT012",  # pytest.raises() block should contain a single simple statement
-    "ISC001", # Implicit string concatenation
+select = [
+    "E",      # Pyflakes
+    "W",      # pycodestyle
+    "F",      # Pyflakes
+    "N",      # Naming
+    "UP",     # PyUpgrade - will show hints for deprecated syntax in python 3.11
+    "ANN001",
+    "ANN201", # Missing return type annotation
+    "ASYNC",  # Flake8-async
+    "S",      # Flake8-bandit
+    "C4",     # Flake8-comprehensions
+    "DTZ",    # Flake8-datetimez
+    "ICN",    # Flake8-import-conventions
+    "LOG",    # Flake8-logging
+    "G",      # Flake8-logging-format
+    "T20",    # Flake8-print
+    "PT",     # Flake8-pytest-style
+    "SLF001", # Flake8-self
+    "SIM",    # Flake8-simplify
+    "TID",    # Flake8-tidy-imports
+    "PTH",    # Flake8-use-pathlib
+    "PL",     # PyLint
+    "PERF",   # Perflint
+    "RUF",    # Ruff
 ]
 
 [tool.ruff.lint.per-file-ignores]
-"__init__.py" = ["F401"] # {name} imported but unused
+"__init__.py" = ["F401"]                              # {name} imported but unused
+"test_**.py"  = ["S101", "PLR2004", "ANN001", "S106"]
+
+[tool.ruff.format]
+quote-style                = "double"
+indent-style               = "space"
+skip-magic-trailing-comma  = false
+line-ending                = "auto"
+docstring-code-format      = true
+docstring-code-line-length = "dynamic"
 
 [tool.mypy]
 cache_dir              = ".cache/mypy"
 disallow_untyped_defs  = true
 exclude                = [".cache", "build", "dist"]
 ignore_missing_imports = false
 incremental            = true
-plugins                = ["pydantic.mypy"]
 python_version         = "3.11"
 warn_return_any        = true
 warn_unused_configs    = true
 warn_unused_ignores    = true
 
-[tool.pydantic-mypy]
-init_forbid_extra             = true
-init_typed                    = true
-warn_required_dynamic_aliases = true
-
 [[tool.mypy.overrides]]
 disallow_untyped_defs  = true
 ignore_missing_imports = true
+ignore_errors          = true
 module                 = ["iso639"]
 
 [tool.coverage.run]
 branch = true
 omit   = ["tests/*"]
 source = ["ailabackend"]
```

### Comparing `knowledgeai_client-0.5.0/PKG-INFO` & `knowledgeai_client-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgeai-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python client for the Avvia Intelligence - Knowledge AI Rest API
 Home-page: https://github.com/arvato-systems-aila-solutions/KnowledgeAI-Python-Client
 License: MIT
 Keywords: AI,Knowledge Retrieval,arvato systems,avvia intelligence,knowledgeai
 Author: Arvato Systems
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Requires-Dist: python-magic (==0.4.27)
 Requires-Dist: tqdm (==4.66.2)
 Description-Content-Type: text/markdown
 
 
 # Avvia Intelligence - KnowledgeAI Python Client
 
-Version: 0.5.0, (c) 2024 Arvato Systems
+Version: 0.5.1, (c) 2024 Arvato Systems
 
 This library is designed to provide easy access to the KnowledgeAI backend service. It enables users to manage projects, upload documents, and perform various tasks programmatically. The client offers an intuitive interface for seamless integration into Python applications.
 
 ## Installation
 ```bash
 pip install knowledgeai-client
 ```
```

