# Comparing `tmp/yanga-1.6.0.tar.gz` & `tmp/yanga-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanga-1.6.0.tar", max compression
+gzip compressed data, was "yanga-1.7.0.tar", max compression
```

## Comparing `yanga-1.6.0.tar` & `yanga-1.7.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     1066 2024-03-29 11:09:20.865177 yanga-1.6.0/LICENSE
--rw-r--r--   0        0        0     4761 2024-03-29 11:09:20.865177 yanga-1.6.0/README.md
--rw-r--r--   0        0        0     3419 2024-03-29 11:09:21.761185 yanga-1.6.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-29 11:09:21.761185 yanga-1.6.0/src/yanga/__init__.py
--rw-r--r--   0        0        0      355 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/__run.py
--rw-r--r--   0        0        0        0 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/cmake/__init__.py
--rw-r--r--   0        0        0     4370 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/cmake/builder.py
--rw-r--r--   0        0        0    13602 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/cmake/cmake_backend.py
--rw-r--r--   0        0        0     4046 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/cmake/create_executable.py
--rw-r--r--   0        0        0      534 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/cmake/generator.py
--rw-r--r--   0        0        0     6708 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/cmake/gtest.py
--rw-r--r--   0        0        0     1414 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/cmake/runner.py
--rw-r--r--   0        0        0        0 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/__init__.py
--rw-r--r--   0        0        0     1902 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/base.py
--rw-r--r--   0        0        0      857 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/gui.py
--rw-r--r--   0        0        0     5551 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/init.py
--rw-r--r--   0        0        0     1271 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/install.py
--rw-r--r--   0        0        0        0 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/__init__.py
--rw-r--r--   0        0        0       13 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/common/.gitignore
--rw-r--r--   0        0        0      377 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/common/.vscode/tasks.json
--rw-r--r--   0        0        0      785 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/common/cleanup.ps1
--rw-r--r--   0        0        0       34 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/common/poetry.toml
--rw-r--r--   0        0        0      219 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/common/scoopfile.json
--rw-r--r--   0        0        0      188 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/common/west.yaml
--rw-r--r--   0        0        0      115 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/common/yanga.ps1
--rw-r--r--   0        0        0      601 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/CMakeLists.txt
--rw-r--r--   0        0        0      410 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/cmake.ps1
--rw-r--r--   0        0        0      523 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/platforms/arduino/index.rst
--rw-r--r--   0        0        0      247 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/platforms/arduino/yanga.yaml
--rw-r--r--   0        0        0     2410 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/platforms/index.rst
--rw-r--r--   0        0        0      448 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/platforms/windows_app/index.rst
--rw-r--r--   0        0        0      152 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/platforms/windows_app/yanga.yaml
--rw-r--r--   0        0        0      203 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/low_pass_filter/CMakeLists.txt
--rw-r--r--   0        0        0      231 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/low_pass_filter/src/low_pass_filter.c
--rw-r--r--   0        0        0      347 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/low_pass_filter/src/low_pass_filter.h
--rw-r--r--   0        0        0      148 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/low_pass_filter/src/low_pass_filter_avg.c
--rw-r--r--   0        0        0      586 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/low_pass_filter/test/test_low_pass_filter.c
--rw-r--r--   0        0        0      531 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/low_pass_filter/yanga.yaml
--rw-r--r--   0        0        0      964 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/main.c
--rw-r--r--   0        0        0      464 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/platform.h
--rw-r--r--   0        0        0      158 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/sensor/CMakeLists.txt
--rw-r--r--   0        0        0      240 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/sensor/src/sensor.c
--rw-r--r--   0        0        0      224 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/sensor/src/sensor.h
--rw-r--r--   0        0        0       83 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/sensor/yanga.yaml
--rw-r--r--   0        0        0      193 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/state_machine/CMakeLists.txt
--rw-r--r--   0        0        0      248 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/state_machine/src/state_machine.c
--rw-r--r--   0        0        0      299 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/state_machine/src/state_machine.h
--rw-r--r--   0        0        0      624 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/state_machine/src/test_state_machine.c
--rw-r--r--   0        0        0      148 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/state_machine/yanga.yaml
--rw-r--r--   0        0        0       75 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/src/yanga.yaml
--rw-r--r--   0        0        0      476 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/stages/my_stage.py
--rw-r--r--   0        0        0      265 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/variants/var1/yanga.yaml
--rw-r--r--   0        0        0      326 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/variants/var2/yanga.yaml
--rw-r--r--   0        0        0      220 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/variants/yanga.yaml
--rw-r--r--   0        0        0      412 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/max/yanga.yaml
--rw-r--r--   0        0        0      319 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/.vscode/cmake-kits.json
--rw-r--r--   0        0        0      551 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/.vscode/cmake-variants.json
--rw-r--r--   0        0        0      844 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/.vscode/launch.json
--rw-r--r--   0        0        0     1261 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/.vscode/settings.json
--rw-r--r--   0        0        0      377 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/.vscode/tasks.json
--rw-r--r--   0        0        0      138 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/CMakeLists.txt
--rw-r--r--   0        0        0       58 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/KConfig
--rw-r--r--   0        0        0       17 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/config_de.txt
--rw-r--r--   0        0        0      295 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/greeter.c
--rw-r--r--   0        0        0      148 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/greeter.h
--rw-r--r--   0        0        0      327 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/greeter_test.cc
--rw-r--r--   0        0        0      136 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/main.c
--rw-r--r--   0        0        0      189 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/platforms/windows/clang.cmake
--rw-r--r--   0        0        0      183 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/platforms/windows/gcc.cmake
--rw-r--r--   0        0        0      438 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/platforms/windows/yanga.yaml
--rw-r--r--   0        0        0     1020 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/mini/yanga.yaml
--rw-r--r--   0        0        0        0 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/template/__init__.py
--rw-r--r--   0        0        0      343 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/template/bootstrap_j2.json
--rw-r--r--   0        0        0     5543 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/template/bootstrap_j2.ps1
--rw-r--r--   0        0        0    15591 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/template/bootstrap_j2.py
--rw-r--r--   0        0        0      669 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/template/cookiecutter.json
--rw-r--r--   0        0        0      271 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/project_templates/template/{{ cookiecutter.project_dir_name }}/pyproject.toml
--rw-r--r--   0        0        0     5947 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/commands/run.py
--rw-r--r--   0        0        0        0 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/domain/__init__.py
--rw-r--r--   0        0        0     2188 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/domain/artifacts.py
--rw-r--r--   0        0        0     1765 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/domain/component_analyzer.py
--rw-r--r--   0        0        0      911 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/domain/components.py
--rw-r--r--   0        0        0     4807 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/domain/config.py
--rw-r--r--   0        0        0     2697 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/domain/config_slurper.py
--rw-r--r--   0        0        0     3333 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/domain/execution_context.py
--rw-r--r--   0        0        0      817 2024-03-29 11:09:20.869177 yanga-1.6.0/src/yanga/domain/pipeline.py
--rw-r--r--   0        0        0     8351 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/domain/project_slurper.py
--rw-r--r--   0        0        0       54 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/gui/__init__.py
--rw-r--r--   0        0        0      537 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/gui/icons.py
--rw-r--r--   0        0        0   258062 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/gui/resources/yanga.ico
--rw-r--r--   0        0        0    29743 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/gui/resources/yanga.png
--rw-r--r--   0        0        0    18735 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/gui/ygui.py
--rw-r--r--   0        0        0        0 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/py.typed
--rw-r--r--   0        0        0        0 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/steps/__init__.py
--rw-r--r--   0        0        0     1690 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/steps/create_venv.py
--rw-r--r--   0        0        0     2172 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/steps/execute_build.py
--rw-r--r--   0        0        0     2295 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/steps/kconfig_gen.py
--rw-r--r--   0        0        0     2088 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/steps/scoop_install.py
--rw-r--r--   0        0        0     1792 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/steps/west_install.py
--rw-r--r--   0        0        0     3169 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/ymain.py
--rw-r--r--   0        0        0     5386 2024-03-29 11:09:20.873177 yanga-1.6.0/src/yanga/yrun.py
--rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 yanga-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 11:16:06.318234 yanga-1.7.0/LICENSE
+-rw-r--r--   0        0        0     4761 2024-04-28 11:16:06.318234 yanga-1.7.0/README.md
+-rw-r--r--   0        0        0     3442 2024-04-28 11:16:07.206228 yanga-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-28 11:16:07.206228 yanga-1.7.0/src/yanga/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/__run.py
+-rw-r--r--   0        0        0        0 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/cmake/__init__.py
+-rw-r--r--   0        0        0     4370 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/cmake/builder.py
+-rw-r--r--   0        0        0    13621 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/cmake/cmake_backend.py
+-rw-r--r--   0        0        0     4046 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/cmake/create_executable.py
+-rw-r--r--   0        0        0      534 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/cmake/generator.py
+-rw-r--r--   0        0        0    13827 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/cmake/gtest.py
+-rw-r--r--   0        0        0     1414 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/cmake/runner.py
+-rw-r--r--   0        0        0        0 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/__init__.py
+-rw-r--r--   0        0        0     1902 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/base.py
+-rw-r--r--   0        0        0      857 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/gui.py
+-rw-r--r--   0        0        0     5551 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/init.py
+-rw-r--r--   0        0        0     1271 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/install.py
+-rw-r--r--   0        0        0        0 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/__init__.py
+-rw-r--r--   0        0        0       13 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/common/.gitignore
+-rw-r--r--   0        0        0      377 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/common/.vscode/tasks.json
+-rw-r--r--   0        0        0      785 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/common/cleanup.ps1
+-rw-r--r--   0        0        0       34 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/common/poetry.toml
+-rw-r--r--   0        0        0      219 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/common/scoopfile.json
+-rw-r--r--   0        0        0      188 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/common/west.yaml
+-rw-r--r--   0        0        0      115 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/common/yanga.ps1
+-rw-r--r--   0        0        0      601 2024-04-28 11:16:06.318234 yanga-1.7.0/src/yanga/commands/project_templates/max/CMakeLists.txt
+-rw-r--r--   0        0        0      410 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/cmake.ps1
+-rw-r--r--   0        0        0      523 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/platforms/arduino/index.rst
+-rw-r--r--   0        0        0      247 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/platforms/arduino/yanga.yaml
+-rw-r--r--   0        0        0     2410 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/platforms/index.rst
+-rw-r--r--   0        0        0      448 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/platforms/windows_app/index.rst
+-rw-r--r--   0        0        0      152 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/platforms/windows_app/yanga.yaml
+-rw-r--r--   0        0        0      203 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/low_pass_filter/CMakeLists.txt
+-rw-r--r--   0        0        0      231 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/low_pass_filter/src/low_pass_filter.c
+-rw-r--r--   0        0        0      347 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/low_pass_filter/src/low_pass_filter.h
+-rw-r--r--   0        0        0      148 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/low_pass_filter/src/low_pass_filter_avg.c
+-rw-r--r--   0        0        0      586 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/low_pass_filter/test/test_low_pass_filter.c
+-rw-r--r--   0        0        0      531 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/low_pass_filter/yanga.yaml
+-rw-r--r--   0        0        0      964 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/main.c
+-rw-r--r--   0        0        0      464 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/platform.h
+-rw-r--r--   0        0        0      158 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/sensor/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/sensor/src/sensor.c
+-rw-r--r--   0        0        0      224 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/sensor/src/sensor.h
+-rw-r--r--   0        0        0       83 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/sensor/yanga.yaml
+-rw-r--r--   0        0        0      193 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/state_machine/CMakeLists.txt
+-rw-r--r--   0        0        0      248 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/state_machine/src/state_machine.c
+-rw-r--r--   0        0        0      299 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/state_machine/src/state_machine.h
+-rw-r--r--   0        0        0      624 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/state_machine/src/test_state_machine.c
+-rw-r--r--   0        0        0      148 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/state_machine/yanga.yaml
+-rw-r--r--   0        0        0       75 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/src/yanga.yaml
+-rw-r--r--   0        0        0      476 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/stages/my_stage.py
+-rw-r--r--   0        0        0      265 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/variants/var1/yanga.yaml
+-rw-r--r--   0        0        0      326 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/variants/var2/yanga.yaml
+-rw-r--r--   0        0        0      220 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/variants/yanga.yaml
+-rw-r--r--   0        0        0      412 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/max/yanga.yaml
+-rw-r--r--   0        0        0      319 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/.vscode/cmake-kits.json
+-rw-r--r--   0        0        0      551 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/.vscode/cmake-variants.json
+-rw-r--r--   0        0        0      844 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/.vscode/launch.json
+-rw-r--r--   0        0        0     1261 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/.vscode/settings.json
+-rw-r--r--   0        0        0      377 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/.vscode/tasks.json
+-rw-r--r--   0        0        0      138 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/CMakeLists.txt
+-rw-r--r--   0        0        0       58 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/KConfig
+-rw-r--r--   0        0        0       17 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/config_de.txt
+-rw-r--r--   0        0        0      295 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/greeter.c
+-rw-r--r--   0        0        0      148 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/greeter.h
+-rw-r--r--   0        0        0      327 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/greeter_test.cc
+-rw-r--r--   0        0        0      136 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/main.c
+-rw-r--r--   0        0        0      189 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/platforms/windows/clang.cmake
+-rw-r--r--   0        0        0      183 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/platforms/windows/gcc.cmake
+-rw-r--r--   0        0        0      438 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/platforms/windows/yanga.yaml
+-rw-r--r--   0        0        0     1020 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/mini/yanga.yaml
+-rw-r--r--   0        0        0        0 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/template/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/template/bootstrap_j2.json
+-rw-r--r--   0        0        0     5543 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/template/bootstrap_j2.ps1
+-rw-r--r--   0        0        0    15591 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/template/bootstrap_j2.py
+-rw-r--r--   0        0        0      669 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/template/cookiecutter.json
+-rw-r--r--   0        0        0      271 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/project_templates/template/{{ cookiecutter.project_dir_name }}/pyproject.toml
+-rw-r--r--   0        0        0     5947 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/commands/run.py
+-rw-r--r--   0        0        0        0 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/__init__.py
+-rw-r--r--   0        0        0     2188 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/artifacts.py
+-rw-r--r--   0        0        0     1765 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/component_analyzer.py
+-rw-r--r--   0        0        0      911 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/components.py
+-rw-r--r--   0        0        0     4807 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/config.py
+-rw-r--r--   0        0        0     2697 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/config_slurper.py
+-rw-r--r--   0        0        0     3354 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/execution_context.py
+-rw-r--r--   0        0        0      817 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/pipeline.py
+-rw-r--r--   0        0        0     8351 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/domain/project_slurper.py
+-rw-r--r--   0        0        0       54 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/gui/__init__.py
+-rw-r--r--   0        0        0      537 2024-04-28 11:16:06.322234 yanga-1.7.0/src/yanga/gui/icons.py
+-rw-r--r--   0        0        0   258062 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/gui/resources/yanga.ico
+-rw-r--r--   0        0        0    29743 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/gui/resources/yanga.png
+-rw-r--r--   0        0        0    18735 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/gui/ygui.py
+-rw-r--r--   0        0        0        0 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/py.typed
+-rw-r--r--   0        0        0        0 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/steps/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/steps/create_venv.py
+-rw-r--r--   0        0        0     2172 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/steps/execute_build.py
+-rw-r--r--   0        0        0     2295 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/steps/kconfig_gen.py
+-rw-r--r--   0        0        0     2088 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/steps/scoop_install.py
+-rw-r--r--   0        0        0     1792 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/steps/west_install.py
+-rw-r--r--   0        0        0     3169 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/ymain.py
+-rw-r--r--   0        0        0     5386 2024-04-28 11:16:06.326233 yanga-1.7.0/src/yanga/yrun.py
+-rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 yanga-1.7.0/PKG-INFO
```

### Comparing `yanga-1.6.0/LICENSE` & `yanga-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/README.md` & `yanga-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/pyproject.toml` & `yanga-1.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yanga"
-version = "1.6.0"
+version = "1.7.0"
 description = "Yet another ninja generator to build C/CPP projects."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/yanga"
 documentation = "https://yanga.readthedocs.io"
 classifiers = [
@@ -32,14 +32,15 @@
 cookiecutter = "^2.1.1"
 py-app-dev = "^2.0.0"
 customtkinter = "^5.2.0"
 pillow = "^10.1.0"
 kspl = "^1.0.0"
 pick = "^2.2.0"
 typer = "^0.11.1"
+hammocking = "^0.2.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0"
 pytest-cov = "^4.1"
 black = "^24.2.0"
 pre-commit = "^3.6.2"
 pyinstaller = "^6.4.0"
@@ -76,15 +77,15 @@
 match = "main"
 
 [tool.semantic_release.branches.noop]
 match = "(?!main$)"
 prerelease = true
 
 [tool.pytest.ini_options]
-addopts = "-v -Wdefault --cov=yanga --cov-report=term-missing:skip-covered -s"
+addopts = "-vv -Wdefault --cov=yanga --cov-report=term-missing:skip-covered -s"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [
@@ -93,15 +94,15 @@
     "if TYPE_CHECKING",
     "raise NotImplementedError",
     'if __name__ == "__main__":',
 ]
 
 [tool.ruff]
 target-version = "py38"
-line-length = 120
+line-length = 180
 lint.select = [
     "B",   # flake8-bugbear
     "C4",  # flake8-comprehensions
     "S",   # flake8-bandit
     "F",   # pyflake
     "E",   # pycodestyle
     "W",   # pycodestyle
```

### Comparing `yanga-1.6.0/src/yanga/cmake/builder.py` & `yanga-1.7.0/src/yanga/cmake/builder.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/cmake/cmake_backend.py` & `yanga-1.7.0/src/yanga/cmake/cmake_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     ) -> None:
         super().__init__()
         self.path = path
         self.variable = variable
         self.relative_path = relative_path
 
     def to_cmake_element(self) -> Optional[CMakeElement]:
-        return CMakeVariable(self.variable, self.to_string()) if self.variable else None
+        return CMakeVariable(self.variable, self.to_path().as_posix()) if self.variable else None
 
     def to_string(self) -> str:
         if self.variable:
             path = f"${{{self.variable}}}"
         else:
             path = self.path.as_posix()
         if self.relative_path:
@@ -177,15 +177,14 @@
 
     def _add_tabulated_path(self, path: CMakePath) -> str:
         return self.tab_prefix + path.to_string()
 
 
 @dataclass
 class CMakeAddExecutable(CMakeElement):
-
     name: str
     sources: List[Union[str, CMakePath, CMakeObjectLibrary]]
     libraries: List[str] = field(default_factory=list)
     compile_options: List[str] = field(default_factory=list)
     link_options: List[str] = field(default_factory=list)
     exclude_from_all: bool = False
 
@@ -288,15 +287,15 @@
         content.extend(self._get_outputs())
         content.append(CMakeDepends(self.depends).to_string())
         content.extend(self._get_commands())
         content.append(")")
         return "\n".join(str(line) for line in content)
 
     def _get_outputs(self) -> List[str]:
-        return [f"{self.tab_prefix}OUTPUT {output.to_string()}" for output in self.outputs]
+        return [f"{self.tab_prefix}OUTPUT {' '.join([output.to_string() for output in self.outputs])}"]
 
     def _get_commands(self) -> List[str]:
         return [self.tab_prefix + str(command) for command in self.commands]
 
 
 @dataclass
 class CMakeCustomTarget(CMakeElement):
```

### Comparing `yanga-1.6.0/src/yanga/cmake/create_executable.py` & `yanga-1.7.0/src/yanga/cmake/create_executable.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/cmake/generator.py` & `yanga-1.7.0/src/yanga/cmake/generator.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/cmake/runner.py` & `yanga-1.7.0/src/yanga/cmake/runner.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/base.py` & `yanga-1.7.0/src/yanga/commands/base.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/gui.py` & `yanga-1.7.0/src/yanga/commands/gui.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/init.py` & `yanga-1.7.0/src/yanga/commands/init.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/install.py` & `yanga-1.7.0/src/yanga/commands/install.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/common/cleanup.ps1` & `yanga-1.7.0/src/yanga/commands/project_templates/common/cleanup.ps1`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/max/CMakeLists.txt` & `yanga-1.7.0/src/yanga/commands/project_templates/max/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/max/platforms/arduino/index.rst` & `yanga-1.7.0/src/yanga/commands/project_templates/max/platforms/arduino/index.rst`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/max/platforms/index.rst` & `yanga-1.7.0/src/yanga/commands/project_templates/max/platforms/index.rst`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/max/src/low_pass_filter/test/test_low_pass_filter.c` & `yanga-1.7.0/src/yanga/commands/project_templates/max/src/low_pass_filter/test/test_low_pass_filter.c`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/max/src/low_pass_filter/yanga.yaml` & `yanga-1.7.0/src/yanga/commands/project_templates/max/src/low_pass_filter/yanga.yaml`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/max/src/main.c` & `yanga-1.7.0/src/yanga/commands/project_templates/max/src/main.c`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/max/src/state_machine/src/test_state_machine.c` & `yanga-1.7.0/src/yanga/commands/project_templates/max/src/state_machine/src/test_state_machine.c`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/mini/.vscode/cmake-variants.json` & `yanga-1.7.0/src/yanga/commands/project_templates/mini/.vscode/cmake-variants.json`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/mini/.vscode/launch.json` & `yanga-1.7.0/src/yanga/commands/project_templates/mini/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/mini/.vscode/settings.json` & `yanga-1.7.0/src/yanga/commands/project_templates/mini/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/mini/yanga.yaml` & `yanga-1.7.0/src/yanga/commands/project_templates/mini/yanga.yaml`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/template/bootstrap_j2.ps1` & `yanga-1.7.0/src/yanga/commands/project_templates/template/bootstrap_j2.ps1`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/template/bootstrap_j2.py` & `yanga-1.7.0/src/yanga/commands/project_templates/template/bootstrap_j2.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/project_templates/template/cookiecutter.json` & `yanga-1.7.0/src/yanga/commands/project_templates/template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/commands/run.py` & `yanga-1.7.0/src/yanga/commands/run.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/domain/artifacts.py` & `yanga-1.7.0/src/yanga/domain/artifacts.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/domain/component_analyzer.py` & `yanga-1.7.0/src/yanga/domain/component_analyzer.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/domain/components.py` & `yanga-1.7.0/src/yanga/domain/components.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/domain/config.py` & `yanga-1.7.0/src/yanga/domain/config.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/domain/config_slurper.py` & `yanga-1.7.0/src/yanga/domain/config_slurper.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/domain/execution_context.py` & `yanga-1.7.0/src/yanga/domain/execution_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class UserRequestTarget(Enum):
     NONE = auto()
     ALL = auto()
     BUILD = auto()
     COMPILE = auto()
     CLEAN = auto()
     TEST = auto()
+    MOCKUP = auto()
 
     def __str__(self) -> str:
         return self.name.lower()
 
 
 class UserRequestScope(Enum):
     VARIANT = auto()
```

### Comparing `yanga-1.6.0/src/yanga/domain/pipeline.py` & `yanga-1.7.0/src/yanga/domain/pipeline.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/domain/project_slurper.py` & `yanga-1.7.0/src/yanga/domain/project_slurper.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/gui/icons.py` & `yanga-1.7.0/src/yanga/gui/icons.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/gui/resources/yanga.ico` & `yanga-1.7.0/src/yanga/gui/resources/yanga.ico`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/gui/resources/yanga.png` & `yanga-1.7.0/src/yanga/gui/resources/yanga.png`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/gui/ygui.py` & `yanga-1.7.0/src/yanga/gui/ygui.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/steps/create_venv.py` & `yanga-1.7.0/src/yanga/steps/create_venv.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/steps/execute_build.py` & `yanga-1.7.0/src/yanga/steps/execute_build.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/steps/kconfig_gen.py` & `yanga-1.7.0/src/yanga/steps/kconfig_gen.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/steps/scoop_install.py` & `yanga-1.7.0/src/yanga/steps/scoop_install.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/steps/west_install.py` & `yanga-1.7.0/src/yanga/steps/west_install.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/ymain.py` & `yanga-1.7.0/src/yanga/ymain.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/src/yanga/yrun.py` & `yanga-1.7.0/src/yanga/yrun.py`

 * *Files identical despite different names*

### Comparing `yanga-1.6.0/PKG-INFO` & `yanga-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanga
-Version: 1.6.0
+Version: 1.7.0
 Summary: Yet another ninja generator to build C/CPP projects.
 Home-page: https://github.com/cuinixam/yanga
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: customtkinter (>=5.2.0,<6.0.0)
+Requires-Dist: hammocking (>=0.2.5,<0.3.0)
 Requires-Dist: kspl (>=1.0.0,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mashumaro (>=3.5,<4.0)
 Requires-Dist: pick (>=2.2.0,<3.0.0)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
 Requires-Dist: py-app-dev (>=2.0.0,<3.0.0)
 Requires-Dist: typer (>=0.11.1,<0.12.0)
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: yanga Version: 1.6.0 Summary: Yet another ninja
+Metadata-Version: 2.1 Name: yanga Version: 1.7.0 Summary: Yet another ninja
 generator to build C/CPP projects. Home-page: https://github.com/cuinixam/yanga
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<3.13 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Requires-Dist: cookiecutter
 (>=2.1.1,<3.0.0) Requires-Dist: customtkinter (>=5.2.0,<6.0.0) Requires-Dist:
-kspl (>=1.0.0,<2.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist:
-mashumaro (>=3.5,<4.0) Requires-Dist: pick (>=2.2.0,<3.0.0) Requires-Dist:
-pillow (>=10.1.0,<11.0.0) Requires-Dist: py-app-dev (>=2.0.0,<3.0.0) Requires-
-Dist: typer (>=0.11.1,<0.12.0) Project-URL: Bug Tracker, https://github.com/
-cuinixam/yanga/issues Project-URL: Changelog, https://github.com/cuinixam/
-yanga/blob/main/CHANGELOG.md Project-URL: Documentation, https://
-yanga.readthedocs.io Project-URL: Repository, https://github.com/cuinixam/yanga
-Description-Content-Type: text/markdown # README
+hammocking (>=0.2.5,<0.3.0) Requires-Dist: kspl (>=1.0.0,<2.0.0) Requires-Dist:
+loguru (>=0.7.0,<0.8.0) Requires-Dist: mashumaro (>=3.5,<4.0) Requires-Dist:
+pick (>=2.2.0,<3.0.0) Requires-Dist: pillow (>=10.1.0,<11.0.0) Requires-Dist:
+py-app-dev (>=2.0.0,<3.0.0) Requires-Dist: typer (>=0.11.1,<0.12.0) Project-
+URL: Bug Tracker, https://github.com/cuinixam/yanga/issues Project-URL:
+Changelog, https://github.com/cuinixam/yanga/blob/main/CHANGELOG.md Project-
+URL: Documentation, https://yanga.readthedocs.io Project-URL: Repository,
+https://github.com/cuinixam/yanga Description-Content-Type: text/markdown #
+README
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_r_u_f_f_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 Yet another ninja generator to build C/CPP projects. ## Installation Install
 this via pip (or your favourite package manager): `pip install yanga` ## Start
 developing The project uses Poetry for dependencies management and packaging.
 If you do not have Poetry installed, you can run the `bootstrap.ps1` script.
```

