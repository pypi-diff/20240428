# Comparing `tmp/config_ninja-1.2.0rc1.tar.gz` & `tmp/config_ninja-1.3.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_ninja-1.2.0rc1.tar", max compression
+gzip compressed data, was "config_ninja-1.3.0b4.tar", max compression
```

## Comparing `config_ninja-1.2.0rc1.tar` & `config_ninja-1.3.0b4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-03-04 20:22:32.347156 config_ninja-1.2.0rc1/LICENSE
--rw-r--r--   0        0        0     5441 2024-03-04 20:22:32.347156 config_ninja-1.2.0rc1/README.md
--rw-r--r--   0        0        0    32810 2024-03-04 20:23:11.423299 config_ninja-1.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1454 2024-03-04 20:23:11.427299 config_ninja-1.2.0rc1/src/config_ninja/__init__.py
--rw-r--r--   0        0        0      464 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/__main__.py
--rw-r--r--   0        0        0     2432 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/backend.py
--rw-r--r--   0        0        0     3592 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/cli.md
--rw-r--r--   0        0        0    15936 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/cli.py
--rw-r--r--   0        0        0     1014 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/contrib/__init__.py
--rw-r--r--   0        0        0    10869 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/contrib/appconfig.py
--rw-r--r--   0        0        0     2142 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/contrib/local.py
--rw-r--r--   0        0        0     7429 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/systemd.py
--rw-r--r--   0        0        0      668 2024-03-04 20:22:32.355156 config_ninja-1.2.0rc1/src/config_ninja/templates/systemd.service.j2
--rw-r--r--   0        0        0     7019 1970-01-01 00:00:00.000000 config_ninja-1.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-28 21:02:47.107949 config_ninja-1.3.0b4/LICENSE
+-rw-r--r--   0        0        0     5427 2024-04-28 21:02:47.107949 config_ninja-1.3.0b4/README.md
+-rw-r--r--   0        0        0    32807 2024-04-28 21:03:24.983878 config_ninja-1.3.0b4/pyproject.toml
+-rw-r--r--   0        0        0     1454 2024-04-28 21:03:24.987878 config_ninja-1.3.0b4/src/config_ninja/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/__main__.py
+-rw-r--r--   0        0        0     2433 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/backend.py
+-rw-r--r--   0        0        0     3592 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/cli.md
+-rw-r--r--   0        0        0    18047 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/cli.py
+-rw-r--r--   0        0        0     1015 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/contrib/__init__.py
+-rw-r--r--   0        0        0    10870 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/contrib/appconfig.py
+-rw-r--r--   0        0        0     2143 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/contrib/local.py
+-rw-r--r--   0        0        0     7643 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/systemd.py
+-rw-r--r--   0        0        0      620 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/templates/systemd.service.j2
+-rw-r--r--   0        0        0     7002 1970-01-01 00:00:00.000000 config_ninja-1.3.0b4/PKG-INFO
```

### Comparing `config_ninja-1.2.0rc1/LICENSE` & `config_ninja-1.3.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `config_ninja-1.2.0rc1/README.md` & `config_ninja-1.3.0b4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Config Ninja 🥷
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![🎨 poe (push)](https://github.com/bryant-finney/config-ninja/actions/workflows/push-poe.yaml/badge.svg)](https://github.com/bryant-finney/config-ninja/actions/workflows/push-poe.yaml)
-[![pylint](https://bryant-finney.github.io/config-ninja/reports/pylint.svg)](https://bryant-finney.github.io/config-ninja/reports/pylint-report.txt)
-[![codecov](https://codecov.io/gh/bryant-finney/config-ninja/graph/badge.svg?token=R3DFDSNK9U)](https://codecov.io/gh/bryant-finney/config-ninja)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/bryant-finney/config-ninja/main.svg)](https://results.pre-commit.ci/latest/github/bryant-finney/config-ninja/main)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://bryant-finney.github.io/config-ninja/reports/mypy-html)
-[![docs: pdoc](https://img.shields.io/badge/docs-pdoc-blueviolet?logo=github)](https://bryant-finney.github.io/config-ninja/config_ninja.html)
+[![🎨 poe (push)](https://github.com/config-ninja/config-ninja/actions/workflows/push-poe.yaml/badge.svg)](https://github.com/config-ninja/config-ninja/actions/workflows/push-poe.yaml)
+[![pylint](https://config-ninja.github.io/config-ninja/reports/pylint.svg)](https://config-ninja.github.io/config-ninja/reports/pylint-report.txt)
+[![codecov](https://codecov.io/gh/config-ninja/config-ninja/graph/badge.svg?token=R3DFDSNK9U)](https://codecov.io/gh/config-ninja/config-ninja)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/config-ninja/config-ninja/main.svg)](https://results.pre-commit.ci/latest/github/config-ninja/config-ninja/main)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://config-ninja.github.io/config-ninja/reports/mypy-html)
+[![docs: pdoc](https://img.shields.io/badge/docs-pdoc-blueviolet?logo=github)](https://config-ninja.github.io/config-ninja/config_ninja.html)
 [![readthedocs](https://readthedocs.org/projects/config-ninja/badge/?version=latest)](https://config-ninja.readthedocs.io/en/latest/home.html)
 [![PyPI version](https://badge.fury.io/py/config-ninja.svg)](https://badge.fury.io/py/config-ninja)
 [![Downloads](https://static.pepy.tech/badge/config-ninja)](https://pepy.tech/project/config-ninja)
 
 Similar to [`confd`](https://github.com/kelseyhightower/confd), manage your system configuration files by populating [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) templates with data from a remote provider.
 
 ## Installation
@@ -18,21 +18,21 @@
 `config-ninja` is installed using the official installer or with `pip` / `pipx`. If your system supports `systemd`, you can then enable `config-ninja` as a `systemd` service.
 
 ### Official Installer
 
 The recommended way to install `config-ninja` is with the official installer:
 
 ```sh
-curl -sSL https://bryant-finney.github.io/config-ninja/install.py | python3 -
+curl -sSL https://config-ninja.github.io/config-ninja/install.py | python3 -
 ```
 
 To view available installation options, run the installer with the `--help` flag:
 
 ```sh
-curl -sSL https://bryant-finney.github.io/config-ninja/install.py | python3 - --help
+curl -sSL https://config-ninja.github.io/config-ninja/install.py | python3 - --help
 ```
 
 ```
 usage: install [-h] [--version VERSION] [--pre] [--uninstall] [--force] [--path PATH] [--backends BACKENDS]
 
 Installs the latest (or given) version of config-ninja
 
@@ -59,15 +59,15 @@
 After installing `config-ninja`, enable it as a `systemd` service for the current user:
 
 ```sh
 # omit '--user' to install the agent at the system level
 config-ninja self install --user
 ```
 
-[all available backends]: https://bryant-finney.github.io/config-ninja/config_ninja/contrib.html#available-backends
+[all available backends]: https://config-ninja.github.io/config-ninja/config_ninja/contrib.html#available-backends
 
 ## How It Works
 
 To demonstrate how the mechanics work locally:
 
 1. create a settings file for `config-ninja`:
    ```sh
@@ -126,15 +126,15 @@
      },
      "example-1": {
        "1": "third value",
        "2": "fourth value"
      }
    }
    ```
-   Chances are, you'll want to update the `config-ninja-settings.yaml` file to use a remote backend (instead of `local`). See [config_ninja.contrib](https://bryant-finney.github.io/config-ninja/config_ninja/contrib.html) for a list of supported config providers.
+   Chances are, you'll want to update the `config-ninja-settings.yaml` file to use a remote backend (instead of `local`). See [config_ninja.contrib](https://config-ninja.github.io/config-ninja/config_ninja/contrib.html) for a list of supported config providers.
 
 ## Configuration Architecture
 
 The `config-ninja` agent monitors the backend source for changes. When the source data is changed, the agent updates the local configuration file with the new data:
 
 ```mermaid
 sequenceDiagram
```

### Comparing `config_ninja-1.2.0rc1/pyproject.toml` & `config_ninja-1.3.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 # https://python-poetry.org/docs/pyproject/
 name = "config-ninja"
-version = "1.2.0rc1"
+version = "1.3.0b4"
 description = "Use special ninja powers to manage system configurations 🥷"
 authors = ["Bryant Finney <bryant.finney@outlook.com>"]
 documentation = "https://config-ninja.readthedocs.org/home.html"
 exclude = ["**/conftest.py"]
-homepage = "https://bryant-finney.github.io/config-ninja/config_ninja.html"
+homepage = "https://config-ninja.github.io/config-ninja/config_ninja.html"
 license = "MIT"
 readme = "README.md"
-repository = "https://github.com/bryant-finney/config-ninja"
+repository = "https://github.com/config-ninja/config-ninja"
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -130,23 +130,23 @@
 # https://python-poetry.org/docs/pyproject/#extras
 all = ["boto3", "watchfiles"]
 appconfig = ["boto3"]
 local = ["watchfiles"]
 
 
 [tool.poetry.group.dev.dependencies]
-boto3-stubs = {version = "1.34.54", extras = ["appconfig", "appconfigdata"]}
+boto3-stubs = {version = "1.34.93", extras = ["appconfig", "appconfigdata"]}
 poethepoet = ">=0.20,<0.26"
 types-pyyaml = "^6"
 
 [tool.poetry.group.lint.dependencies]
 anybadge = "^1.14"
 pylint = "^3.0"
 safety = ">=2.3,<4.0"
-shellcheck-py = {version = ">=0.8,<0.10", markers = "platform_machine != 'arm64'"}
+shellcheck-py = {version = ">=0.8,<0.11", markers = "platform_machine != 'arm64'"}
 pre-commit = [
   {version = "<3.6", python = "<3.9"},
   {version = ">=3.6", python = ">=3.9"}
 ]
 
 [tool.poetry.group.misc.dependencies]
 certifi = ">=2023.07.22"
@@ -160,20 +160,20 @@
 python-semantic-release = ">=8.0.8,<10.0.0"
 
 [tool.poetry.group.test.dependencies]
 # dependencies for testing
 coverage = { extras = ["toml"], version = ">=6.4,<8.0" }
 pytest = ">=7.4.4,<9.0.0"
 pytest-clarity = "^1.0.1"
-pytest-cov = ">=3,<5"
+pytest-cov = ">=3,<6"
 pytest-mock = "^3.8"
 
 [tool.poetry.group.pre-commit.dependencies]
 # note: these must be synchronized with `.pre-commit-config.yaml`
-ruff = ">=0.1.9,<0.4.0"
+ruff = ">=0.1.9,<0.5.0"
 mypy = { extras = ["reports"], version = "^1.4.1" }
 lxml = {version = ">=4.9.3", python = ">=3.12"}
 pyright = "^1.1.344"
 
 [tool.coverage.report]
 # https://coverage.readthedocs.io/en/latest/config.html#report
 fail_under = 50
```

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/__init__.py` & `config_ninja-1.3.0b4/src/config_ninja/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # Navigation
 - `config_ninja.contrib` for supported backends:
     - `config_ninja.contrib.appconfig`
     - `config_ninja.contrib.local`
 - `config_ninja.cli` for commands and CLI documentation
 - `config_ninja.systemd` for `systemd` integration
 """  # noqa: D415
+
 from __future__ import annotations
 
-__version__ = '1.2.0rc1'
+__version__ = '1.3.0b4'
 
 from pathlib import Path
 
 from pyspry import Settings
 
 __all__ = ['DEFAULT_SETTINGS_PATHS', 'load_settings', 'resolve_settings_path']
```

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/backend.py` & `config_ninja-1.3.0b4/src/config_ninja/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the API for config backends."""
+
 from __future__ import annotations
 
 import abc
 import json
 import logging
 import typing
 from typing import Any, AsyncIterator, Callable, Dict
```

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/cli.md` & `config_ninja-1.3.0b4/src/config_ninja/cli.md`

 * *Files identical despite different names*

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/cli.py` & `config_ninja-1.3.0b4/src/config_ninja/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,23 @@
 
 import config_ninja
 from config_ninja import systemd
 from config_ninja.backend import DUMPERS, Backend, FormatT, dumps, loads
 from config_ninja.contrib import get_backend
 
 try:
-    from typing import Annotated, TypeAlias  # type: ignore[attr-defined,unused-ignore]
+    from typing import (
+        Annotated,  # type: ignore[attr-defined,unused-ignore]
+        TypeAlias,
+    )
 except ImportError:  # pragma: no cover
-    from typing_extensions import Annotated, TypeAlias  # type: ignore[assignment,unused-ignore]
+    from typing_extensions import (  # type: ignore[assignment,unused-ignore]
+        Annotated,
+        TypeAlias,
+    )
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     import sh
 
     SYSTEMD_AVAILABLE = True
 else:
     try:
@@ -118,18 +124,19 @@
         '-c',
         '--config',
         help="Path to [bold blue]config-ninja[/]'s own configuration file.",
         show_default=False,
     ),
 ]
 UserAnnotation: TypeAlias = Annotated[
-    typing.Optional[bool],
+    bool,
     typer.Option(
         '-u',
         '--user',
+        '--user-mode',
         help='User mode installation (does not require [bold orange3]sudo[/])',
         show_default=False,
     ),
 ]
 WorkdirAnnotation: TypeAlias = Annotated[
     typing.Optional[Path],
     typer.Option(
@@ -152,17 +159,79 @@
 
 
 EnvNamesAnnotation: TypeAlias = Annotated[
     typing.Optional[typing.List[str]],
     typer.Option(
         '-e',
         '--env',
-        help='Embed these environment variables into the unit file.',
+        help='Embed these environment variables into the unit file. Can be used multiple times.',
         show_default=False,
         callback=parse_env,
+        metavar='NAME[,NAME...]',
+    ),
+]
+
+
+class UserGroup(typing.NamedTuple):
+    """Run the service using this user (and optionally group)."""
+
+    user: str
+    """The user to run the service as."""
+
+    group: typing.Optional[str] = None
+    """The group to run the service as."""
+
+    @classmethod
+    def parse(cls, value: str) -> 'UserGroup':
+        """Parse the `--run-as user[:group]` argument for the `systemd` service."""
+        return cls(*value.split(':'))
+
+
+RunAsAnnotation: TypeAlias = typing.Annotated[
+    typing.Optional[UserGroup],
+    typer.Option(
+        '--run-as',
+        help='Configure the systemd unit to run the service as this user (and optionally group).',
+        metavar='user[:group]',
+        parser=UserGroup.parse,
+    ),
+]
+
+
+class Variable(typing.NamedTuple):
+    """Set this variable in the shell used to run the `systemd` service."""
+
+    name: str
+    """The name of the variable."""
+
+    value: str
+    """The value of the variable."""
+
+
+def parse_var(value: str) -> Variable:
+    """Parse the `--var VARIABLE=VALUE` arguments for setting variables in the `systemd` service."""
+    try:
+        parsed = Variable(*value.split('='))
+    except TypeError as exc:
+        print(
+            f'[red]ERROR[/]: Invalid argument (expected [yellow]VARIABLE=VALUE[/] pair): [purple]{value}[/]'
+        )
+        raise typer.Exit(1) from exc
+
+    return parsed
+
+
+VariableAnnotation: TypeAlias = Annotated[
+    typing.Optional[typing.List[Variable]],
+    typer.Option(
+        '--var',
+        help='Embed the specified [yellow]VARIABLE=VALUE[/] into the unit file. Can be used multiple times.',
+        metavar='VARIABLE=VALUE',
+        show_default=False,
+        parser=parse_var,
     ),
 ]
 
 
 def version_callback(ctx: typer.Context, value: typing.Optional[bool] = None) -> None:
     """Print the version of the package."""
     if ctx.resilient_parsing:  # pragma: no cover  # this is for tab completions
@@ -400,56 +469,65 @@
     if not SYSTEMD_AVAILABLE:
         print('[red]ERROR[/]: Missing [bold gray93]systemd[/]!')
         print('Currently, this command only works on linux.')
         raise typer.Exit(1)
 
 
 @self_app.command()
-def install(
+def install(  # noqa: PLR0913
     env_names: EnvNamesAnnotation = None,
     print_only: PrintAnnotation = None,
-    user: UserAnnotation = None,
+    run_as: RunAsAnnotation = None,
+    user_mode: UserAnnotation = False,
+    variables: VariableAnnotation = None,
     workdir: WorkdirAnnotation = None,
 ) -> None:
     """Install [bold blue]config-ninja[/] as a [bold gray93]systemd[/] service.
 
-    The --env argument can be passed multiple times with comma-separated strings.
+    Both --env and --var can be passed multiple times.
 
     Example:
-            config-ninja self install --env FOO,BAR,BAZ --env SPAM --env EGGS
+            config-ninja self install --env FOO,BAR,BAZ --env SPAM --var EGGS=42
 
-    The environment variables [purple]FOO[/], [purple]BAR[/], [purple]BAZ[/], [purple]SPAM[/], and [purple]EGGS[/] will be read from the current shell and written to the service file.
+    The environment variables [purple]FOO[/], [purple]BAR[/], [purple]BAZ[/], and [purple]SPAM[/] will be read from the current shell and written to the service file, while [purple]EGGS[/] will be set to [yellow]42[/].
     """
+    environ = {name: os.environ[name] for name in env_names or [] if name in os.environ}
+    environ.update(variables)  # type: ignore[arg-type]
+
     kwargs = {
         # the command to use when invoking config-ninja from systemd
         'config_ninja_cmd': sys.argv[0]
         if sys.argv[0].endswith('config-ninja')
         else f'{sys.executable} {sys.argv[0]}',
         # write these environment variables into the systemd service file
-        'environ': {name: os.environ[name] for name in env_names or [] if name in os.environ},
+        'environ': environ,
         # run `config-ninja` from this directory (if specified)
         'workdir': workdir,
     }
+    if run_as:
+        kwargs['user'] = run_as.user
+        if run_as.group:
+            kwargs['group'] = run_as.group
 
-    svc = systemd.Service('config_ninja', 'systemd.service.j2', user or False)
+    svc = systemd.Service('config_ninja', 'systemd.service.j2', user_mode)
     if print_only:
         rendered = svc.render(**kwargs)
         print(Markdown(f'# {svc.path}\n```systemd\n{rendered}\n```'))
         raise typer.Exit(0)
 
     _check_systemd()
 
     print(f'Installing {svc.path}')
     print(svc.install(**kwargs))
 
     print('[green]SUCCESS[/] :white_check_mark:')
 
 
 @self_app.command()
-def uninstall(print_only: PrintAnnotation = None, user: UserAnnotation = None) -> None:
+def uninstall(print_only: PrintAnnotation = None, user: UserAnnotation = False) -> None:
     """Uninstall the [bold blue]config-ninja[/] [bold gray93]systemd[/] service."""
     svc = systemd.Service('config_ninja', 'systemd.service.j2', user or False)
     if print_only:
         print(Markdown(f'# {svc.path}\n```systemd\n{svc.read()}\n```'))
         raise typer.Exit(0)
 
     _check_systemd()
```

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/contrib/__init__.py` & `config_ninja-1.3.0b4/src/config_ninja/contrib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 package. The `get_backend()` function is used to retrieve the backend class given its module name.
 
 ## Available Backends
 
 - `config_ninja.contrib.appconfig`
 - `config_ninja.contrib.local`
 """
+
 from __future__ import annotations
 
 import importlib
 
 from config_ninja.backend import Backend
```

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/contrib/appconfig.py` & `config_ninja-1.3.0b4/src/config_ninja/contrib/appconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ```yaml
 .. include:: ../../../examples/appconfig-backend.yaml
 ```
 
 .. _config-ninja: https://bryant-finney.github.io/config-ninja/config_ninja.html
 """
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import warnings
 from typing import TYPE_CHECKING, Any, AsyncIterator, Literal
```

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/contrib/local.py` & `config_ninja-1.3.0b4/src/config_ninja/contrib/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ```yaml
 .. include:: ../../../examples/local-backend.yaml
 ```
 
 .. _config-ninja: https://bryant-finney.github.io/config-ninja/config_ninja.html
 """
+
 from __future__ import annotations
 
 import logging
 import warnings
 from pathlib import Path
 from typing import AsyncIterator
```

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/systemd.py` & `config_ninja-1.3.0b4/src/config_ninja/systemd.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 Jan 21 22:37:52 ubuntu systemd[592]: Started config synchronization daemon.
 
 SUCCESS ✅
 ```
 
 .. _install: https://bryant-finney.github.io/config-ninja/config_ninja/cli.html#config-ninja-self-install
 """  # noqa: RUF002
+
 from __future__ import annotations
 
 import contextlib
 import logging
 import os
 import typing
 from pathlib import Path
@@ -63,23 +64,30 @@
     Path(os.getenv('XDG_CONFIG_HOME') or Path.home() / '.config') / 'systemd' / 'user'
 )
 """The file path for user-local installation."""
 
 __all__ = ['SYSTEM_INSTALL_PATH', 'USER_INSTALL_PATH', 'Service', 'notify']
 logger = logging.getLogger(__name__)
 
+
+@contextlib.contextmanager
+def dummy() -> typing.Iterator[None]:
+    """Define a dummy context manager to use instead of `sudo`.
+
+    There are a few scenarios where `sudo` is unavailable or unnecessary:
+    - running on Windows
+    - running in a container without `sudo` installed
+    - already running as root
+    """
+    yield  # pragma: no cover
+
+
 try:
     sudo = sh.contrib.sudo
 except AttributeError:  # pragma: no cover
-
-    @contextlib.contextmanager
-    def dummy() -> typing.Iterator[None]:
-        """We might be running inside a container; or we might be on Windows."""
-        yield
-
     sudo = dummy()
 
 
 def notify() -> None:  # pragma: no cover
     """Notify `systemd` that the service has finished starting up and is ready."""
     sock = sdnotify.SystemdNotifier()
     sock.notify('READY=1')  # pyright: ignore[reportUnknownMemberType]
@@ -128,86 +136,95 @@
 
     >>> svc.uninstall()
     """
 
     path: Path
     """The installation location of the `systemd` unit file."""
 
+    sudo: typing.ContextManager[None]
+
     tmpl: jinja2.Template
     """Load the template on initialization."""
 
     user_mode: bool
     """Whether to install the service for the full system or just the current user."""
 
     def __init__(self, provider: str, template: str, user_mode: bool) -> None:
         """Prepare to render the specified `template` from the `provider` package."""
         loader = jinja2.PackageLoader(provider)
         env = jinja2.Environment(autoescape=jinja2.select_autoescape(default=True), loader=loader)
         self.tmpl = env.get_template(template)
         self.user_mode = user_mode
         self.path = (USER_INSTALL_PATH if user_mode else SYSTEM_INSTALL_PATH) / SERVICE_NAME
 
+        if os.geteuid() == 0:
+            self.sudo = dummy()
+        else:
+            self.sudo = sudo
+
     def _install_system(self, content: str) -> str:
-        with sudo:
-            logger.info('writing to %s', self.path)
-            sh.mkdir('-p', str(self.path.parent))
-            sh.tee(str(self.path), _in=content, _out='/dev/null')
-
-            logger.info('enabling and starting %s', self.path.name)
-            sh.systemctl.start(self.path.name)
-            return sh.systemctl.status(self.path.name)
+        logger.info('writing to %s', self.path)
+        sh.mkdir('-p', str(self.path.parent))
+        sh.tee(str(self.path), _in=content, _out='/dev/null')
+
+        logger.info('enabling and starting %s', self.path.name)
+        sh.systemctl.start(self.path.name)
+        return sh.systemctl.status(self.path.name)
 
     def _install_user(self, content: str) -> str:
         logger.info('writing to %s', self.path)
         self.path.parent.mkdir(parents=True, exist_ok=True)
         self.path.write_text(content, encoding='utf-8')
 
         logger.info('enabling and starting %s', self.path.name)
         sh.systemctl.start('--user', self.path.name)
         return sh.systemctl.status('--user', self.path.name)
 
     def _uninstall_system(self) -> None:
-        with sudo:
-            logger.info('stopping and disabling %s', self.path.name)
-            sh.systemctl.disable('--now', self.path.name)
+        logger.info('stopping and disabling %s', self.path.name)
+        sh.systemctl.disable('--now', self.path.name)
 
-            logger.info('removing %s', self.path)
-            sh.rm(str(self.path))
+        logger.info('removing %s', self.path)
+        sh.rm(str(self.path))
 
     def _uninstall_user(self) -> None:
         logger.info('stopping and disabling %s', self.path.name)
         sh.systemctl.disable('--user', '--now', self.path.name)
 
         logger.info('removing %s', self.path)
         self.path.unlink()
 
     def install(self, **kwargs: typing.Any) -> str:
         """Render the `systemd` service file from `kwargs` and install it."""
         rendered = self.render(**kwargs)
         if self.user_mode:
             return self._install_user(rendered)
-        return self._install_system(rendered)
+
+        if os.geteuid() == 0:
+            return self._install_system(rendered)
+
+        with sudo:
+            return self._install_system(rendered)
 
     def read(self) -> str:
         """Read the `systemd` service file."""
         return self.path.read_text(encoding='utf-8')
 
     def render(self, **kwargs: typing.Any) -> str:
         """Render the `systemd` service file from the given parameters."""
         if workdir := kwargs.get('workdir'):
             kwargs['workdir'] = Path(workdir).absolute()
 
         kwargs.setdefault('user_mode', self.user_mode)
-        if hasattr(os, 'geteuid'):  # pragma: no cover  # windows
-            kwargs.setdefault('user', os.geteuid())
-
-        if hasattr(os, 'getegid'):  # pragma: no cover  # windows
-            kwargs.setdefault('group', os.getegid())
 
         return self.tmpl.render(**kwargs)
 
     def uninstall(self) -> None:
         """Disable, stop, and delete the service."""
         if self.user_mode:
-            self._uninstall_user()
-        else:
-            self._uninstall_system()
+            return self._uninstall_user()
+
+        if os.geteuid() == 0:
+            return self._uninstall_system()
+
+        with sudo:
+            return self._uninstall_system()
```

### Comparing `config_ninja-1.2.0rc1/src/config_ninja/templates/systemd.service.j2` & `config_ninja-1.3.0b4/src/config_ninja/templates/systemd.service.j2`

 * *Files 26% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 {% endfor -%}
 {% endif -%}
 ExecStartPre={{ config_ninja_cmd }} self print
 ExecStart={{ config_ninja_cmd }} monitor
 Restart=always
 RestartSec=30s
 Type=notify
-{%- if not user_mode %}
-# always run as the calling user, even when installed to the system
+{%- if user %}
 User={{ user }}
+{%- endif %}
+{%- if group %}
 Group={{ group }}
 {%- endif %}
 {%- if workdir %}
 WorkingDirectory={{ workdir }}
 {%- endif %}
 
 [Install]
```

### Comparing `config_ninja-1.2.0rc1/PKG-INFO` & `config_ninja-1.3.0b4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: config-ninja
-Version: 1.2.0rc1
+Version: 1.3.0b4
 Summary: Use special ninja powers to manage system configurations 🥷
-Home-page: https://bryant-finney.github.io/config-ninja/config_ninja.html
+Home-page: https://config-ninja.github.io/config-ninja/config_ninja.html
 License: MIT
 Author: Bryant Finney
 Author-email: bryant.finney@outlook.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,26 +27,26 @@
 Requires-Dist: sdnotify (>=0.3.2,<0.4.0)
 Requires-Dist: sh (>=2.0.6,<3.0.0) ; sys_platform != "win32"
 Requires-Dist: tomlkit (>=0.12.3,<0.13.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0) ; python_version == "3.8"
 Requires-Dist: watchfiles (>=0.21.0,<0.22.0) ; extra == "all" or extra == "local"
 Project-URL: Documentation, https://config-ninja.readthedocs.org/home.html
-Project-URL: Repository, https://github.com/bryant-finney/config-ninja
+Project-URL: Repository, https://github.com/config-ninja/config-ninja
 Description-Content-Type: text/markdown
 
 # Config Ninja 🥷
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![🎨 poe (push)](https://github.com/bryant-finney/config-ninja/actions/workflows/push-poe.yaml/badge.svg)](https://github.com/bryant-finney/config-ninja/actions/workflows/push-poe.yaml)
-[![pylint](https://bryant-finney.github.io/config-ninja/reports/pylint.svg)](https://bryant-finney.github.io/config-ninja/reports/pylint-report.txt)
-[![codecov](https://codecov.io/gh/bryant-finney/config-ninja/graph/badge.svg?token=R3DFDSNK9U)](https://codecov.io/gh/bryant-finney/config-ninja)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/bryant-finney/config-ninja/main.svg)](https://results.pre-commit.ci/latest/github/bryant-finney/config-ninja/main)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://bryant-finney.github.io/config-ninja/reports/mypy-html)
-[![docs: pdoc](https://img.shields.io/badge/docs-pdoc-blueviolet?logo=github)](https://bryant-finney.github.io/config-ninja/config_ninja.html)
+[![🎨 poe (push)](https://github.com/config-ninja/config-ninja/actions/workflows/push-poe.yaml/badge.svg)](https://github.com/config-ninja/config-ninja/actions/workflows/push-poe.yaml)
+[![pylint](https://config-ninja.github.io/config-ninja/reports/pylint.svg)](https://config-ninja.github.io/config-ninja/reports/pylint-report.txt)
+[![codecov](https://codecov.io/gh/config-ninja/config-ninja/graph/badge.svg?token=R3DFDSNK9U)](https://codecov.io/gh/config-ninja/config-ninja)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/config-ninja/config-ninja/main.svg)](https://results.pre-commit.ci/latest/github/config-ninja/config-ninja/main)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://config-ninja.github.io/config-ninja/reports/mypy-html)
+[![docs: pdoc](https://img.shields.io/badge/docs-pdoc-blueviolet?logo=github)](https://config-ninja.github.io/config-ninja/config_ninja.html)
 [![readthedocs](https://readthedocs.org/projects/config-ninja/badge/?version=latest)](https://config-ninja.readthedocs.io/en/latest/home.html)
 [![PyPI version](https://badge.fury.io/py/config-ninja.svg)](https://badge.fury.io/py/config-ninja)
 [![Downloads](https://static.pepy.tech/badge/config-ninja)](https://pepy.tech/project/config-ninja)
 
 Similar to [`confd`](https://github.com/kelseyhightower/confd), manage your system configuration files by populating [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) templates with data from a remote provider.
 
 ## Installation
@@ -54,21 +54,21 @@
 `config-ninja` is installed using the official installer or with `pip` / `pipx`. If your system supports `systemd`, you can then enable `config-ninja` as a `systemd` service.
 
 ### Official Installer
 
 The recommended way to install `config-ninja` is with the official installer:
 
 ```sh
-curl -sSL https://bryant-finney.github.io/config-ninja/install.py | python3 -
+curl -sSL https://config-ninja.github.io/config-ninja/install.py | python3 -
 ```
 
 To view available installation options, run the installer with the `--help` flag:
 
 ```sh
-curl -sSL https://bryant-finney.github.io/config-ninja/install.py | python3 - --help
+curl -sSL https://config-ninja.github.io/config-ninja/install.py | python3 - --help
 ```
 
 ```
 usage: install [-h] [--version VERSION] [--pre] [--uninstall] [--force] [--path PATH] [--backends BACKENDS]
 
 Installs the latest (or given) version of config-ninja
 
@@ -95,15 +95,15 @@
 After installing `config-ninja`, enable it as a `systemd` service for the current user:
 
 ```sh
 # omit '--user' to install the agent at the system level
 config-ninja self install --user
 ```
 
-[all available backends]: https://bryant-finney.github.io/config-ninja/config_ninja/contrib.html#available-backends
+[all available backends]: https://config-ninja.github.io/config-ninja/config_ninja/contrib.html#available-backends
 
 ## How It Works
 
 To demonstrate how the mechanics work locally:
 
 1. create a settings file for `config-ninja`:
    ```sh
@@ -162,15 +162,15 @@
      },
      "example-1": {
        "1": "third value",
        "2": "fourth value"
      }
    }
    ```
-   Chances are, you'll want to update the `config-ninja-settings.yaml` file to use a remote backend (instead of `local`). See [config_ninja.contrib](https://bryant-finney.github.io/config-ninja/config_ninja/contrib.html) for a list of supported config providers.
+   Chances are, you'll want to update the `config-ninja-settings.yaml` file to use a remote backend (instead of `local`). See [config_ninja.contrib](https://config-ninja.github.io/config-ninja/config_ninja/contrib.html) for a list of supported config providers.
 
 ## Configuration Architecture
 
 The `config-ninja` agent monitors the backend source for changes. When the source data is changed, the agent updates the local configuration file with the new data:
 
 ```mermaid
 sequenceDiagram
```

