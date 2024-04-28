# Comparing `tmp/hatch_cython-0.5.1.tar.gz` & `tmp/hatch_cython-0.6.0rc0.tar.gz`

## Comparing `hatch_cython-0.5.1.tar` & `hatch_cython-0.6.0rc0.tar`

### file list

```diff
@@ -1,92 +1,104 @@
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/COVERAGE.md
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/cliff.toml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/taskfile.yaml
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/.github/workflows/ruff.yaml
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/__about__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/constants.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/devel.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/hooks.py
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/plugin.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/temp.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/types.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/utils.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/__init__.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/autoimport.py
--rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/config.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/defaults.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/files.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/flags.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/includes.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/macros.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/platform.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/src/hatch_cython/config/templates.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/bootstrap.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/simple_structure/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/simple_structure/LICENSE.txt
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/simple_structure/README.md
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/simple_structure/hatch.toml
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/simple_structure/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/simple_structure/example_lib/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/simple_structure/tests/.gitkeep
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/LICENSE.txt
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/README.md
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/hatch.toml
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/include/.gitkeep
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/include/something.cc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/scripts/.gitkeep
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/scripts/custom_include.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/__about__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/_alias.pyx
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/custom_includes.pyi
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/custom_includes.pyx
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/normal.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/templated.pyi.in
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/templated.pyx.in
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyi
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyx
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/test.pyi
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/test.pyx
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/mod_a/__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/mod_a/adds.pyi
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/mod_a/adds.pyx
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/mod_a/some_defn.pxd
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/mod_a/some_defn.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/mod_a/deep_nest/creates.pyx
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/no_compile/abc.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/platform/darwin.pyx
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/platform/freebsd.pyx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/platform/linux.pyx
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/platform/windows.pyx
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/tests/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/tests/test_aliased.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/tests/test_custom_includes.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/tests/test_example.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/tests/test_normal.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/tests/test_platform.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/tests/test_submodule.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/test_libraries/src_structure/tests/test_templated.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     9696 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_config.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_files.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_includes.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_macros.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_platform_pyversion.py
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_plugin.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_setuppy.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_templates.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/test_xenv_merge.py
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/tests/utils.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0    16785 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/README.md
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    18375 2020-02-02 00:00:00.000000 hatch_cython-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/COVERAGE.md
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/cliff.toml
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/taskfile.yaml
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/.github/workflows/ruff.yaml
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/__about__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/constants.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/devel.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/hooks.py
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/plugin.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/temp.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/types.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/utils.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/__init__.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/autoimport.py
+-rw-r--r--   0        0        0     9361 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/config.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/defaults.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/files.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/flags.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/includes.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/macros.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/platform.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/src/hatch_cython/config/templates.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/bootstrap.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/LICENSE.txt
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/hatch.toml
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/pyproject.toml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/src/example_only_included/__about__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/src/example_only_included/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/src/example_only_included/compile.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/src/example_only_included/did.pyi
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/src/example_only_included/dont_compile.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/tests/__init__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/tests/test_compiled.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/only_included/tests/test_didnt.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/simple_structure/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/simple_structure/LICENSE.txt
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/simple_structure/hatch.toml
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/simple_structure/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/simple_structure/example_lib/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/simple_structure/tests/.gitkeep
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/LICENSE.txt
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/hatch.toml
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/include/.gitkeep
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/include/something.cc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/scripts/.gitkeep
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/scripts/custom_include.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/__about__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/_alias.pyx
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/custom_includes.pyi
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/custom_includes.pyx
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/normal.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/templated.pyi.in
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/templated.pyx.in
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyi
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyx
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/test.pyi
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/test.pyx
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/mod_a/__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/mod_a/adds.pyi
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/mod_a/adds.pyx
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/mod_a/some_defn.pxd
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/mod_a/some_defn.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/mod_a/deep_nest/creates.pyx
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/no_compile/abc.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/platform/darwin.pyx
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/platform/freebsd.pyx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/platform/linux.pyx
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/platform/windows.pyx
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/tests/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/tests/test_aliased.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/tests/test_custom_includes.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/tests/test_example.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/tests/test_normal.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/tests/test_platform.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/tests/test_submodule.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/test_libraries/src_structure/tests/test_templated.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_config.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_files.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_includes.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_macros.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_platform.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_platform_pyversion.py
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_plugin.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_plugin_excludes.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_setuppy.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_templates.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_utils.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/test_xenv_merge.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/tests/utils.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/LICENSE.txt
+-rw-r--r--   0        0        0    17723 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/README.md
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    19316 2020-02-02 00:00:00.000000 hatch_cython-0.6.0rc0/PKG-INFO
```

### Comparing `hatch_cython-0.5.1/.pre-commit-config.yaml` & `hatch_cython-0.6.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/CHANGELOG.md` & `hatch_cython-0.6.0rc0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,30 @@
 
 All notable changes to this project will be documented in this file.
 
 ## [unreleased]
 
 ### Bug Fixes
 
+- Implementation
+
+### Features
+
+- Explicit build targets (#46, #47)
+
+## [0.5.1] - 2024-02-19
+
+### Bug Fixes
+
 - Build permissions ([#28](https://github.com/joshua-auchincloss/hatch-cython/issues/28))
 - Ci
 - No auto changelog
 - Release ci [ci skip] ([#40](https://github.com/joshua-auchincloss/hatch-cython/issues/40))
+- Ci
+- Release
 
 ### Features
 
 - Gh releases
 
 ### Miscellaneous Tasks
 
@@ -23,20 +35,27 @@
 - Pr #35 - ci
 - Add 3.12 for validation [ci skip]
 - Pr #36 - ci
 - Doc [ci skip]
 - Changelog
 - Pr #38 from dev
 - Tighten ci ([#39](https://github.com/joshua-auchincloss/hatch-cython/issues/39))
+- Changelog
+- V0.5.1
 
 ### Merge
 
 - #29 from build
 - Pr #37 from dev
 
+### Release
+
+- V0.5.1
+- V0.5.1
+
 ## [0.5.0] - 2023-11-30
 
 ### Bug Fixes
 
 - Version [ci skip]
 - Trigger build
 - Depreciate `retain_intermediate_artifacts`
```

### Comparing `hatch_cython-0.5.1/COVERAGE.md` & `hatch_cython-0.6.0rc0/COVERAGE.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 | Name                                    |   Stmts |   Miss |  Branch | BrPart |   Cover |
 | --------------------------------------- | ------: | -----: | ------: | -----: | ------: |
 | src/hatch_cython/\_\_init\_\_.py        |       2 |      0 |       0 |      0 |    100% |
 | src/hatch_cython/config/\_\_init\_\_.py |       2 |      0 |       0 |      0 |    100% |
 | src/hatch_cython/config/autoimport.py   |       9 |      0 |       2 |      0 |    100% |
-| src/hatch_cython/config/config.py       |     139 |      9 |      58 |      5 |     92% |
-| src/hatch_cython/config/defaults.py     |       6 |      0 |       0 |      0 |    100% |
-| src/hatch_cython/config/files.py        |      27 |      1 |      12 |      2 |     92% |
-| src/hatch_cython/config/flags.py        |      70 |      1 |      24 |      0 |     99% |
-| src/hatch_cython/config/includes.py     |      15 |      1 |       8 |      1 |     91% |
+| src/hatch_cython/config/config.py       |     143 |      9 |      60 |      6 |     92% |
+| src/hatch_cython/config/defaults.py     |      27 |      0 |       8 |      1 |     97% |
+| src/hatch_cython/config/files.py        |      35 |      0 |      16 |      1 |     98% |
+| src/hatch_cython/config/flags.py        |      69 |      1 |      24 |      0 |     99% |
+| src/hatch_cython/config/includes.py     |      15 |      0 |       8 |      0 |    100% |
 | src/hatch_cython/config/macros.py       |      12 |      0 |       7 |      0 |    100% |
-| src/hatch_cython/config/platform.py     |      75 |      2 |      30 |      4 |     94% |
-| src/hatch_cython/config/templates.py    |      62 |      7 |      30 |      3 |     89% |
-| src/hatch_cython/constants.py           |      11 |      0 |       0 |      0 |    100% |
+| src/hatch_cython/config/platform.py     |      75 |      0 |      30 |      3 |     97% |
+| src/hatch_cython/config/templates.py    |      62 |      5 |      32 |      4 |     90% |
+| src/hatch_cython/constants.py           |      15 |      0 |       0 |      0 |    100% |
 | src/hatch_cython/devel.py               |       5 |      0 |       0 |      0 |    100% |
 | src/hatch_cython/hooks.py               |       5 |      1 |       2 |      0 |     86% |
-| src/hatch_cython/plugin.py              |     232 |     12 |     144 |     10 |     94% |
+| src/hatch_cython/plugin.py              |     248 |     12 |     156 |     10 |     95% |
 | src/hatch_cython/temp.py                |      13 |      0 |       2 |      0 |    100% |
-| src/hatch_cython/utils.py               |      43 |      4 |      18 |      1 |     89% |
-| **TOTAL**                               | **728** | **38** | **337** | **26** | **94%** |
+| src/hatch_cython/utils.py               |      39 |      0 |      16 |      0 |    100% |
+| **TOTAL**                               | **776** | **28** | **363** | **25** | **95%** |
```

### Comparing `hatch_cython-0.5.1/cliff.toml` & `hatch_cython-0.6.0rc0/cliff.toml`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/taskfile.yaml` & `hatch_cython-0.6.0rc0/taskfile.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 version: '3'
 
 tasks:
     std-test:
-        dir: '{{.DIR}}'
+        dir: '{{ .DIR }}'
         env:
             HATCH_CYTHON_DEVEL: 1
         cmds:
         -   hatch --verbose build --clean
+        -   if [ -d "/Users/runner" ]; then hatch env remove; fi
         -   hatch run test
 
     example:
         dir: test_libraries/src_structure
         cmds:
         -   task: std-test
             vars:
                 DIR: test_libraries/src_structure
         -   if [ "$(cat ./caller_outputs.json |  jaq .call)" -ne "true" ]; then exit 1; fi
         -   if [ "$(cat ./caller_outputs.json |  jaq .includes)" -ne "true" ]; then exit 1; fi
 
+    only-included:
+        dir: test_libraries/only_included
+        cmds:
+        -   task: std-test
+            vars:
+                DIR: test_libraries/only_included
+
     simple-structure:
         dir: test_libraries/simple_structure
         cmds:
         -   rm -rf ./example_lib/*
         -   rm -rf ./tests/*
         -   cp -r ../src_structure/src/example_lib/* ./example_lib/
         -   cp -r ../src_structure/tests/* ./tests/
```

### Comparing `hatch_cython-0.5.1/.github/workflows/build.yaml` & `hatch_cython-0.6.0rc0/.github/workflows/build.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -28,81 +28,89 @@
             matrix:
                 os: [ubuntu-latest, windows-latest, macos-latest]
                 python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
         steps:
         -   uses: actions/checkout@v4
 
-        -   uses: actions/setup-go@v5
-            with:
-                go-version: stable
-
-        -   name: Install Task
-            run: |
-                go install github.com/go-task/task/v3/cmd/task@latest
-
         -   name: Install llvm
-            if: startsWith(matrix.os, 'macos-')
+            if: startsWith(matrix.os, 'macos')
             run: |
-                brew cleanup
-                brew update -f
+                brew remove --ignore-dependencies python
                 rm -rf /usr/local/bin/2to3*
                 rm -rf /usr/local/bin/idle3*
                 rm -rf /usr/local/bin/pydoc3*
                 rm -rf /usr/local/bin/python*
-                brew install libomp
-                brew install llvm
+                brew cleanup
+                brew update -f
+                brew install libomp llvm
                 echo "
-                export PATH=\"/usr/local/opt/llvm/bin:\$PATH\"
-                export LDFLAGS=\"-L/usr/local/opt/llvm/lib\"
-                export CPPFLAGS=\"-I/usr/local/opt/llvm/include\"
+                export PATH=\"$(brew --prefix)/opt/llvm/bin:\$PATH\"
+                export DYLD_LIBRARY_PATH=\"$(brew --prefix)/lib:$DYLD_LIBRARY_PATH\"
+                export LDFLAGS=\"-L$(brew --prefix)/opt/llvm/lib\"
+                export CPPFLAGS=\"-I$(brew --prefix)/opt/llvm/include\"
                 export LD=ld.lld
                 export AR=llvm-ar
                 export RANLIB=llvm-ranlib
+
                 " >> $HOME/.bash_profile
 
+        -   uses: actions/setup-go@v5
+            with:
+                go-version: stable
+
+        -   name: Install Task
+            run: |
+                go install github.com/go-task/task/v3/cmd/task@latest
+
         -   uses: hecrj/setup-rust-action@v2
             with:
                 rust-version: stable
 
         -   uses: cargo-bins/cargo-binstall@main
 
         -   name: Install jaq
             run: |
                 cargo binstall -y jaq
 
         -   name: Set up Python ${{ matrix.python-version }}
-            uses: actions/setup-python@v4
+            uses: actions/setup-python@v5
             with:
-                architecture: x64
                 python-version: ${{ matrix.python-version }}
 
         -   name: Install Hatch
-            run: pip install --upgrade hatch
+            run: |
+                pip install --upgrade pip
+                pip install --upgrade hatch
 
         -   name: Run tests
             run: hatch run cov
 
         -   name: Test src lib compilation
             shell: bash
             run: |
                 task example
 
         -   name: Test simple lib compilation
             shell: bash
             run: |
                 task simple-structure
 
+        -   name: Test build target directives
+            shell: bash
+            run: |
+                task only-included
+
     sdist:
         needs: [validate]
         runs-on: ubuntu-latest
         steps:
         -   uses: actions/checkout@v4
         -   name: Set up Python
-            uses: actions/setup-python@v4
+            uses: actions/setup-python@v5
         -   name: Install dependencies
             run: |
                 python -m pip install --upgrade pip
                 pip install hatch
         -   name: Build package
             run: hatch build -t sdist
         -   name: Upload sdist
@@ -117,17 +125,16 @@
         strategy:
             matrix:
                 python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
                 os: [ubuntu-latest, windows-latest, macos-latest]
         steps:
         -   uses: actions/checkout@v4
         -   name: Set up Python ${{ matrix.python-version }}
-            uses: actions/setup-python@v4
+            uses: actions/setup-python@v5
             with:
-                architecture: x64
                 python-version: ${{ matrix.python-version }}
         -   name: Install dependencies
             run: |
                 python -m pip install --upgrade pip
                 pip install hatch
         -   name: Build package
             run: hatch build -t wheel
@@ -149,15 +156,16 @@
             uses: actions/download-artifact@v4
             with:
                 path: dist/
                 merge-multiple: true
         -   name: Display downloaded files
             run: ls -R ./dist
         -   name: Release
-            uses: softprops/action-gh-release@v1
+            uses: softprops/action-gh-release@v2
             with:
                 generate_release_notes: true
                 fail_on_unmatched_files: true
+                prerelease: ${{ contains(github.ref, 'rc') }}
                 files: |-
                     dist/*
         -   name: Publish package
             uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `hatch_cython-0.5.1/.github/workflows/coverage.yaml` & `hatch_cython-0.6.0rc0/.github/workflows/coverage.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 jobs:
     cov:
         runs-on: ubuntu-latest
         steps:
         -   name: Checkout
             uses: actions/checkout@v4
         -   name: Set up Python 3.11
-            uses: actions/setup-python@v4
+            uses: actions/setup-python@v5
             with:
                 python-version: '3.11'
         -   name: Install dependencies
             run: pip install '.[test]'
         -   name: Run tests and collect coverage
             run: pytest --cov --ignore=test_libraries
         -   name: Upload coverage to Codecov
             uses: codecov/codecov-action@v3
+            env:
+                CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `hatch_cython-0.5.1/.github/workflows/test.yml` & `hatch_cython-0.6.0rc0/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -23,66 +23,74 @@
             matrix:
                 os: [ubuntu-latest, windows-latest, macos-latest]
                 python-version: ['3.8', '3.9', '3.10', '3.11']
 
         steps:
         -   uses: actions/checkout@v4
 
-        -   uses: actions/setup-go@v5
-            with:
-                go-version: stable
-
-        -   name: Install Task
-            run: |
-                go install github.com/go-task/task/v3/cmd/task@latest
-
         -   name: Install llvm
-            if: startsWith(matrix.os, 'macos-')
+            if: startsWith(matrix.os, 'macos')
             run: |
-                brew cleanup
-                brew update -f
+                brew remove --ignore-dependencies python
                 rm -rf /usr/local/bin/2to3*
                 rm -rf /usr/local/bin/idle3*
                 rm -rf /usr/local/bin/pydoc3*
                 rm -rf /usr/local/bin/python*
-                brew install libomp
-                brew install llvm
+                brew cleanup
+                brew update -f
+                brew install libomp llvm
                 echo "
-                export PATH=\"/usr/local/opt/llvm/bin:\$PATH\"
-                export LDFLAGS=\"-L/usr/local/opt/llvm/lib\"
-                export CPPFLAGS=\"-I/usr/local/opt/llvm/include\"
+                export PATH=\"$(brew --prefix)/opt/llvm/bin:\$PATH\"
+                export DYLD_LIBRARY_PATH=\"$(brew --prefix)/lib:$DYLD_LIBRARY_PATH\"
+                export LDFLAGS=\"-L$(brew --prefix)/opt/llvm/lib\"
+                export CPPFLAGS=\"-I$(brew --prefix)/opt/llvm/include\"
                 export LD=ld.lld
                 export AR=llvm-ar
                 export RANLIB=llvm-ranlib
+
                 " >> $HOME/.bash_profile
 
+        -   uses: actions/setup-go@v5
+            with:
+                go-version: stable
+
+        -   name: Install Task
+            run: |
+                go install github.com/go-task/task/v3/cmd/task@latest
+
         -   uses: hecrj/setup-rust-action@v2
             with:
                 rust-version: stable
 
         -   uses: cargo-bins/cargo-binstall@main
 
         -   name: Install jaq
             run: |
                 cargo binstall -y jaq
 
         -   name: Set up Python ${{ matrix.python-version }}
-            uses: actions/setup-python@v4
+            uses: actions/setup-python@v5
             with:
-                architecture: x64
                 python-version: ${{ matrix.python-version }}
 
         -   name: Install Hatch
-            run: pip install --upgrade hatch
+            run: |
+                pip install --upgrade pip
+                pip install --upgrade hatch
 
         -   name: Run tests
             run: hatch run cov
 
         -   name: Test src lib compilation
             shell: bash
             run: |
                 task example
 
         -   name: Test simple lib compilation
             shell: bash
             run: |
                 task simple-structure
+
+        -   name: Test build target directives
+            shell: bash
+            run: |
+                task only-included
```

### Comparing `hatch_cython-0.5.1/src/hatch_cython/plugin.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 import os
 import re
 import subprocess
 import sys
 from contextlib import contextmanager
 from glob import glob
 from tempfile import TemporaryDirectory
-from typing import ClassVar
 
 from Cython.Tempita import sub as render_template
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
 from hatch_cython.config import parse_from_dict
+from hatch_cython.constants import (
+    compiled_extensions,
+    intermediate_extensions,
+    precompiled_extensions,
+    templated_extensions,
+)
 from hatch_cython.temp import ExtensionArg, setup_py
-from hatch_cython.types import CallableT, DictT, ListStr, ListT, P
+from hatch_cython.types import CallableT, DictT, ListStr, ListT, P, Set
 from hatch_cython.utils import autogenerated, memo, parse_user_glob, plat
 
 
 class CythonBuildHook(BuildHookInterface):
     PLUGIN_NAME = "cython"
 
-    precompiled_extensions: ClassVar[list] = [
-        # py is left out as we have it optional / runtime value
-        ".pyx",
-        ".pxd",
-    ]
-    templated_extensions: ClassVar[list] = [f"{f}.in" for f in {".py", ".pyi", *precompiled_extensions}]
-    intermediate_extensions: ClassVar[list] = [
-        ".c",
-        ".cpp",
-    ]
-    compiled_extensions: ClassVar[list] = [
-        ".dll",
-        # unix
-        ".so",
-        # windows
-        ".pyd",
-    ]
+    precompiled_extensions: Set[str]
+    intermediate_extensions: Set[str]
+    templated_extensions: Set[str]
+    compiled_extensions: Set[str]
 
     def __init__(self, *args: P.args, **kwargs: P.kwargs):
+        self.precompiled_extensions = precompiled_extensions.copy()
+        self.intermediate_extensions = intermediate_extensions.copy()
+        self.templated_extensions = templated_extensions.copy()
+        self.compiled_extensions = compiled_extensions.copy()
+
         super().__init__(*args, **kwargs)
 
+        _ = self.options
+
     @property
     @memo
     def is_src(self):
         return os.path.exists(os.path.join(self.root, "src"))
 
     @property
     def is_windows(self):
@@ -91,38 +90,45 @@
         return list(set(_globs))
 
     @property
     @memo
     def options_exclude(self):
         return [parse_user_glob(e.matches) for e in self.options.files.exclude if e.applies()]
 
+    @property
+    @memo
+    def options_include(self):
+        return [parse_user_glob(e.matches) for e in self.options.files.targets if e.applies()]
+
     def wanted(self, item: str):
-        return not any(re.match(e, self.normalize_glob(item), re.IGNORECASE) for e in self.options_exclude)
+        not_excluded = not any(re.match(e, self.normalize_glob(item), re.IGNORECASE) for e in self.options_exclude)
+        if self.options.files.explicit_targets:
+            return not_excluded and any(re.match(opt, self.normalize_glob(item)) for opt in self.options_include)
+        return not_excluded
 
     def filter_ensure_wanted(self, tgts: ListStr):
         return list(
             filter(
                 self.wanted,
                 tgts,
             )
         )
 
     @property
     def included_files(self):
-        included = []
-        _normu = [self.normalize_glob(parse_user_glob(e.matches)) for e in self.options.files.exclude if e.applies()]
+        included = set()
         self.app.display_debug("user globs")
-        self.app.display_debug(_normu)
         for patt in self.precompiled_globs:
             globbed = glob(patt, recursive=True)
+            self.app.display_info(f"{patt} globbed {globbed!r}")
             if len(globbed) == 0:
                 continue
             matched = self.filter_ensure_wanted(globbed)
-            included.extend(matched)
-        return included
+            included = included.union(matched)
+        return list(included)
 
     @property
     def normalized_included_files(self):
         """
         Produces files in posix format
         """
         return list({self.normalize_glob(f) for f in self.included_files})
@@ -245,15 +251,20 @@
         self.rm_recurse(self.compiled)
 
     @property
     @memo
     def options(self):
         config = parse_from_dict(self)
         if config.compile_py:
-            self.precompiled_extensions.append(".py")
+            self.precompiled_extensions.add(".py")
+        if config.files.explicit_targets:
+            self.precompiled_extensions.add(".py")
+            self.precompiled_extensions.add(".c")
+            self.precompiled_extensions.add(".cc")
+            self.precompiled_extensions.add(".cpp")
         return config
 
     @property
     def sdist(self):
         return self.target_name == "sdist"
 
     @property
```

### Comparing `hatch_cython-0.5.1/src/hatch_cython/temp.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/temp.py`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/src/hatch_cython/types.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 if vmaj >= (3, 10):
     from collections.abc import Callable
     from typing import ParamSpec
 
     TupleT = tuple
     DictT = dict
     ListT = list
+    Set = set
 else:
-    from typing import Callable, Dict, List, Tuple  # noqa: UP035
+    from typing import Callable, Dict, List, Set, Tuple  # noqa: UP035, F401
 
     from typing_extensions import ParamSpec
 
     TupleT = Tuple  # noqa: UP006
     DictT = Dict  # noqa: UP006
     ListT = List  # noqa: UP006
```

### Comparing `hatch_cython-0.5.1/src/hatch_cython/config/autoimport.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/config/autoimport.py`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/src/hatch_cython/config/config.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/config/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 from typing import Optional
 
 from hatch.utils.ci import running_in_ci
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
 from hatch_cython.config.autoimport import Autoimport
-from hatch_cython.config.defaults import get_default_compile, get_default_link
+from hatch_cython.config.defaults import brew_path, get_default_compile, get_default_link
 from hatch_cython.config.files import FileArgs
 from hatch_cython.config.flags import EnvFlags, parse_env_args
 from hatch_cython.config.includes import parse_includes
 from hatch_cython.config.macros import DefineMacros, parse_macros
 from hatch_cython.config.platform import ListedArgs, PlatformArgs, parse_platform_args
 from hatch_cython.config.templates import Templates, parse_template_kwds
 from hatch_cython.constants import DIRECTIVES, EXIST_TRIM, INCLUDE, LTPY311, MUST_UNIQUE
@@ -40,70 +40,99 @@
 
 
 def parse_from_dict(cls: BuildHookInterface):
     given = cls.config.get("options", {})
 
     passed = given.copy()
     kwargs = {}
-    for kw, val in given.items():
-        if kw in __known__:
+    for key, val in given.items():
+        if key in __known__:
             parsed: any
-            if kw == "files":
+            if key == "files":
                 val: dict
                 parsed: FileArgs = FileArgs(**val)
-            elif kw == "define_macros":
+            elif key == "define_macros":
                 val: list
                 parsed: DefineMacros = parse_macros(val)
-            elif kw == "templates":
+            elif key == "templates":
                 val: dict
                 parsed: Templates = parse_template_kwds(val)
             else:
                 val: any
                 parsed: any = val
-            kwargs[kw] = parsed
-            passed.pop(kw)
+            kwargs[key] = parsed
+            passed.pop(key)
             continue
 
     compile_args = parse_platform_args(kwargs, "compile_args", get_default_compile)
     link_args = parse_platform_args(kwargs, "extra_link_args", get_default_link)
     envflags = parse_env_args(kwargs)
     cfg = Config(**kwargs, compile_args=compile_args, extra_link_args=link_args, envflags=envflags)
 
-    for kw, val in passed.copy().items():
-        is_include = kw.startswith(INCLUDE)
-        if is_include and val:
+    for maybe_dep, spec in passed.copy().items():
+        is_include = maybe_dep.startswith(INCLUDE)
+        if is_include and spec:
             cfg.resolve_pkg(
                 cls,
-                parse_includes(kw, val),
+                parse_includes(maybe_dep, spec),
             )
-            passed.pop(kw)
+            passed.pop(maybe_dep)
             continue
         elif is_include:
-            passed.pop(kw)
+            passed.pop(maybe_dep)
             continue
-        elif kw == "parallel" and passed.get(kw):
+        elif maybe_dep == "parallel" and passed.get(maybe_dep):
             comp = [
                 PlatformArgs(arg="/openmp", platforms="windows"),
                 PlatformArgs(arg="-fopenmp", platforms=["linux"]),
             ]
             link = [
                 PlatformArgs(arg="/openmp", platforms="windows"),
                 PlatformArgs(arg="-fopenmp", platforms="linux"),
-                PlatformArgs(arg="-lomp", platforms="darwin", marker=LTPY311, apply_to_marker=running_in_ci),
                 PlatformArgs(
-                    arg="-L/usr/local/opt/llvm/lib/c++ -Wl,-rpath,/usr/local/opt/llvm/lib/c++",
-                    platforms=["darwin"],
-                    depends_path=True,
+                    arg="-lomp", platforms="darwin", arch=["x86_64"], marker=LTPY311, apply_to_marker=running_in_ci
                 ),
             ]
+
+            brew = brew_path()
+            if brew:
+                comp.extend(
+                    [
+                        PlatformArgs(
+                            arg=f"-I{brew}/opt/llvm/include",
+                            platforms=["darwin"],
+                            depends_path=True,
+                        ),
+                        PlatformArgs(
+                            arg=f"-I{brew}/opt/libomp/include",
+                            platforms=["darwin"],
+                            depends_path=True,
+                        ),
+                    ]
+                )
+                link.extend(
+                    [
+                        PlatformArgs(
+                            arg=f"-L{brew}/opt/llvm/lib/c++ -Wl,-rpath,{brew}/llvm/lib/c++",
+                            platforms=["darwin"],
+                            depends_path=True,
+                        ),
+                        PlatformArgs(
+                            arg=f"-L{brew}/opt/libomp/lib -Wl,-rpath,{brew}/opt/libomp/lib",
+                            platforms=["darwin"],
+                            depends_path=True,
+                        ),
+                    ]
+                )
+
             cma = ({*cfg.compile_args}).union({*comp})
             cfg.compile_args = list(cma)
             seb = ({*cfg.extra_link_args}).union({*link})
             cfg.extra_link_args = list(seb)
-            passed.pop(kw)
+            passed.pop(maybe_dep)
 
     cfg.compile_kwargs = passed
     return cfg
 
 
 @dataclass
 class Config:
@@ -227,20 +256,20 @@
                 for v in it:
                     flush(v)
             else:
                 flat.append(it)
 
         # side effect
         list(map(flush, args.values()))
-        return flat
+        return list({*flat})
 
     def asdict(self):
         d = asdict(self)
         d["envflags"]["env"] = self.envflags.masked_environ()
         d["templates"] = self.templates.asdict()
         return d
 
     def validate_include_opts(self):
         for opt in self.includes:
             if not path.exists(opt):
-                msg = "%s does not exist" % opt
+                msg = f"{opt} does not exist"
                 raise ValueError(msg)
```

### Comparing `hatch_cython-0.5.1/src/hatch_cython/config/flags.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/config/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from dataclasses import dataclass, field
-from os import environ
+from os import environ, pathsep
 from typing import ClassVar
 
 from hatch_cython.config.platform import PlatformArgs, parse_to_plat
 from hatch_cython.types import CallableT, DictT
-from hatch_cython.utils import path_delim
 
 
 @dataclass
 class EnvFlag(PlatformArgs):
     env: str = field(default="")
     merges: bool = field(default=False)
     sep: str = field(default=" ")
@@ -25,15 +24,15 @@
     EnvFlag(env="CCSHARED", merges=True),
     EnvFlag(env="CPPFLAGS", merges=True),
     EnvFlag(env="LDFLAGS", merges=True),
     EnvFlag(env="LDSHARED", merges=True),
     EnvFlag(env="SHLIB_SUFFIX", merges=False),
     EnvFlag(env="AR", merges=False),
     EnvFlag(env="ARFLAGS", merges=True),
-    EnvFlag(env="PATH", merges=True, sep=path_delim()),
+    EnvFlag(env="PATH", merges=True, sep=pathsep),
 )
 
 
 @dataclass
 class EnvFlags:
     CC: PlatformArgs = None
     CPP: PlatformArgs = None
```

### Comparing `hatch_cython-0.5.1/src/hatch_cython/config/includes.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/config/includes.py`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/src/hatch_cython/config/macros.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/config/macros.py`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/src/hatch_cython/config/platform.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/config/platform.py`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/src/hatch_cython/config/templates.py` & `hatch_cython-0.6.0rc0/src/hatch_cython/config/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,20 +57,15 @@
                     "'keyword = { abc = 1, ... }' in your "
                     "pyproject.toml / hatch.toml"
                 )
                 raise ValueError(msg, arg)
         self.kwargs = kwargs
 
     def __repr__(self) -> str:
-        return dedent(
-            f"""Templates(
-    index={self.index},
-    kwargs={self.kwargs}
-)"""
-        )
+        return dedent(f"""Templates(index={self.index!r}, kwargs={self.kwargs!r})""")
 
     def asdict(self):
         return {
             "index": [asdict(i) for i in self.index],
             "kwargs": self.kwargs,
         }
 
@@ -90,15 +85,16 @@
                         )
                         cls.app.display_warning(msg)
                     else:
                         kwds = {**kwds, **add}
         # raise ValueError(kwds, files, self.index)
         return kwds
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Templates):
+            return False
+        return other.index == self.index and other.kwargs == self.kwargs
+
 
 def parse_template_kwds(clsvars: dict):
-    try:
-        idx = clsvars.pop("index")
-    except KeyError:
-        idx = []
-    idx = [IndexItem(**kw) for kw in idx]
+    idx = [IndexItem(**kw) for kw in clsvars.pop("index", [])]
     return Templates(index=idx, **clsvars)
```

### Comparing `hatch_cython-0.5.1/test_libraries/simple_structure/LICENSE.txt` & `hatch_cython-0.6.0rc0/test_libraries/simple_structure/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/test_libraries/simple_structure/hatch.toml` & `hatch_cython-0.6.0rc0/test_libraries/simple_structure/hatch.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,14 @@
   {arg = "-v"},
   {platforms = [
     "linux",
     "darwin"
   ], arg = "-Wcpp"},
   {platforms = [
     "darwin"
-  ], arch = "x86_64", arg = "-arch x86_64"},
-  {platforms = [
-    "darwin"
-  ], arch = "arm64", arg = "-arch arm64"},
-  {platforms = [
-    "darwin"
   ], arch = "x86_64", arg = "-I/usr/local/opt/llvm/include", depends_path = true, marker = "python_version <= '3.10'"},
   {platforms = [
     "darwin"
   ], arch = "x86_64", arg = "-I/opt/homebrew/opt/llvm/include", depends_path = true, marker = "python_version <= '3.10'"}
 ]
 cythonize_kwargs = {annotate = true, nthreads = 4}
 define_macros = [["NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION"]]
@@ -99,18 +93,19 @@
     "windows"
   ]}
 ]
 templated_mac = {supported = ["int", "float"]}
 templated_win = {supported = ["int", "float", "complex"]}
 
 [build.targets.wheel]
+macos-max-compat = false
 packages = ["example_lib"]
 
 [[envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [envs.default]
 dependencies = ["coverage", "pytest", "beartype", "numpy"]
 
 [envs.default.scripts]
 cov = ["install", "test-cov", "cov-report"]
 cov-report = ["- coverage combine", "coverage report"]
```

### Comparing `hatch_cython-0.5.1/test_libraries/simple_structure/pyproject.toml` & `hatch_cython-0.6.0rc0/test_libraries/simple_structure/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,20 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy"
 ]
-dependencies = [
-  "pytest"
-]
+dependencies = ["pytest"]
 description = ''
 dynamic = ["version"]
 keywords = []
 license = {file = "LICENSE.txt"}
 name = "example_lib"
-readme = "README.md"
 requires-python = ">=3.7"
 
 [project.urls]
 Documentation = "https://github.com/unknown/example#readme"
 Issues = "https://github.com/unknown/simple_structure/issues"
 Source = "https://github.com/unknown/example"
 
@@ -38,32 +35,30 @@
 target-version = ["py37"]
 
 [tool.coverage.paths]
 example = ["*/example_lib/*", "*/example_lib", "*/simple_structure/example_lib"]
 tests = ["tests", "*/simple_structure/tests"]
 
 [tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:"
-]
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.coverage.run]
 branch = true
-omit = [
-  "example_lib/__about__.py"
-]
+omit = ["example_lib/__about__.py"]
 parallel = true
 source_pkgs = ["example_lib"]
 
 [tool.hatch.version]
 path = "example_lib/__about__.py"
 
 [tool.ruff]
+line-length = 120
+target-version = "py37"
+
+[tool.ruff.lint]
 ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
   "S105",
@@ -72,15 +67,14 @@
   # Ignore complexity
   "C901",
   "PLR0911",
   "PLR0912",
   "PLR0913",
   "PLR0915"
 ]
-line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -100,20 +94,18 @@
   "S",
   "T",
   "TID",
   "UP",
   "W",
   "YTT"
 ]
-target-version = "py37"
-unfixable = [
-]
+unfixable = []
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["example", "example_lib"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
```

### Comparing `hatch_cython-0.5.1/test_libraries/src_structure/LICENSE.txt` & `hatch_cython-0.6.0rc0/test_libraries/src_structure/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/test_libraries/src_structure/hatch.toml` & `hatch_cython-0.6.0rc0/test_libraries/src_structure/hatch.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,14 @@
   {arg = "-v"},
   {platforms = [
     "linux",
     "darwin"
   ], arg = "-Wcpp"},
   {platforms = [
     "darwin"
-  ], arch = "x86_64", arg = "-arch x86_64"},
-  {platforms = [
-    "darwin"
-  ], arch = "arm64", arg = "-arch arm64"},
-  {platforms = [
-    "darwin"
   ], arch = "x86_64", arg = "-I/usr/local/opt/llvm/include", depends_path = true, marker = "python_version <= '3.10'"},
   {platforms = [
     "darwin"
   ], arch = "x86_64", arg = "-I/opt/homebrew/opt/llvm/include", depends_path = true, marker = "python_version <= '3.10'"}
 ]
 compiled_sdist = true
 cythonize_kwargs = {annotate = true, nthreads = 4}
@@ -108,22 +102,23 @@
 "include" = "include/"
 "scripts" = "scripts/"
 
 [build.targets.sdist]
 include = ["scripts/", "include/", "src/"]
 
 [build.targets.wheel]
+macos-max-compat = false
 packages = ["src/example_lib"]
 
 [build.targets.wheel.force-include]
 "include" = "include/"
 "scripts" = "scripts/"
 
 [[envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [envs.default]
 dependencies = ["coverage", "pytest", "beartype", "numpy"]
 skip-install = true
 
 [envs.default.scripts]
 cov = ["install", "test-cov", "cov-report"]
```

### Comparing `hatch_cython-0.5.1/test_libraries/src_structure/pyproject.toml` & `hatch_cython-0.6.0rc0/test_libraries/src_structure/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,20 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy"
 ]
-dependencies = [
-  "pytest"
-]
+dependencies = ["pytest"]
 description = ''
 dynamic = ["version"]
 keywords = []
 license = {file = "LICENSE.txt"}
 name = "example_lib"
-readme = "README.md"
 requires-python = ">=3.7"
 
 [project.urls]
 Documentation = "https://github.com/unknown/example#readme"
 Issues = "https://github.com/unknown/example/issues"
 Source = "https://github.com/unknown/example"
 
@@ -38,32 +35,30 @@
 target-version = ["py37"]
 
 [tool.coverage.paths]
 example = ["*/example_lib/*", "*/src/example_lib", "*/example/src/example_lib"]
 tests = ["tests", "*/example/tests"]
 
 [tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:"
-]
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.coverage.run]
 branch = true
-omit = [
-  "src/example_lib/__about__.py"
-]
+omit = ["src/example_lib/__about__.py"]
 parallel = true
 source_pkgs = ["example_lib"]
 
 [tool.hatch.version]
 path = "src/example_lib/__about__.py"
 
 [tool.ruff]
+line-length = 120
+target-version = "py37"
+
+[tool.ruff.lint]
 ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
   "S105",
@@ -72,15 +67,14 @@
   # Ignore complexity
   "C901",
   "PLR0911",
   "PLR0912",
   "PLR0913",
   "PLR0915"
 ]
-line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -100,20 +94,18 @@
   "S",
   "T",
   "TID",
   "UP",
   "W",
   "YTT"
 ]
-target-version = "py37"
-unfixable = [
-]
+unfixable = []
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["example", "example_lib"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
```

### Comparing `hatch_cython-0.5.1/test_libraries/src_structure/scripts/custom_include.py` & `hatch_cython-0.6.0rc0/test_libraries/src_structure/scripts/custom_include.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def update():
     with open("caller_outputs.json", "w") as f:
         f.write(
             json.dumps(
                 {
-                    "call": True,
+                    "call": CALLED_MUST,
                     "includes": CALLED_INCLUDES,
                 }
             )
         )
 
 
 def must_call():
```

### Comparing `hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyi` & `hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyi`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyx` & `hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyx`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/test_libraries/src_structure/src/example_lib/test.pyx` & `hatch_cython-0.6.0rc0/test_libraries/src_structure/src/example_lib/test.pyx`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/tests/test_includes.py` & `hatch_cython-0.6.0rc0/tests/test_includes.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,35 @@
         "include": "gets_include",
         "libraries": "gets_libraries",
         "library_dirs": "gets_library_dirs",
         "required_call": "some_setup_op",
     }
     ok = parse_includes(
         "include_abc",
-        parse,
+        parse.copy(),
     )
     assert ok == Autoimport(**parse)
     ok = parse_includes(
         "include_abc",
         "some_attr",
     )
     assert ok == Autoimport(pkg="abc", include="some_attr")
 
 
+def test_with_resolved():
+    parse = {
+        "include": "gets_include",
+        "libraries": "gets_libraries",
+        "library_dirs": "gets_library_dirs",
+        "required_call": "some_setup_op",
+    }
+    ok = parse_includes(
+        "include_abc",
+        parse.copy(),
+    )
+
+    assert ok == Autoimport(pkg="abc", **parse)
+
+
 def test_invalid():
     with raises(ValueError, match="either provide a known package"):
         parse_includes("list", [])
```

### Comparing `hatch_cython-0.5.1/tests/test_macros.py` & `hatch_cython-0.6.0rc0/tests/test_macros.py`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/tests/test_plugin.py` & `hatch_cython-0.6.0rc0/tests/test_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 @pytest.fixture
 def new_src_proj(tmp_path):
     project_dir = tmp_path / "app"
     project_dir.mkdir()
     (project_dir / "bootstrap.py").write_text(read("test_libraries/bootstrap.py"))
     (project_dir / "pyproject.toml").write_text(read("test_libraries/src_structure/pyproject.toml"))
     (project_dir / "hatch.toml").write_text(read("test_libraries/src_structure/hatch.toml"))
-    (project_dir / "README.md").write_text(read("test_libraries/src_structure/README.md"))
     (project_dir / "LICENSE.txt").write_text(read("test_libraries/src_structure/LICENSE.txt"))
     shutil.copytree(join("test_libraries/src_structure", "src"), (project_dir / "src"))
     shutil.copytree(join("test_libraries/src_structure", "tests"), (project_dir / "tests"))
     shutil.copytree(join("test_libraries/src_structure", "include"), (project_dir / "include"))
     shutil.copytree(join("test_libraries/src_structure", "scripts"), (project_dir / "scripts"))
     return project_dir
 
@@ -47,14 +46,16 @@
             SimpleNamespace(name="example_lib"),
             directory=new_src_proj,
             target_name="wheel",
         )
 
         assert hook.is_src
 
+        assert not hook.options.files.explicit_targets
+
         with arch_platform("", "windows"):
             assert hook.is_windows
 
         with arch_platform("", "darwin"):
             assert not hook.is_windows
 
         with arch_platform("", "linux"):
@@ -163,7 +164,9 @@
             ]
         )
         assert sorted(hook.normalized_dist_globs) == rf
         assert build_data.get("infer_tag")
         assert not build_data.get("pure_python")
         assert sorted(hook.artifacts) == sorted(build_data.get("artifacts")) == sorted([f"/{f}" for f in rf])
         assert len(build_data.get("force_include")) == 12
+
+    syspath.remove(str(new_src_proj))
```

### Comparing `hatch_cython-0.5.1/tests/test_setuppy.py` & `hatch_cython-0.6.0rc0/tests/test_setuppy.py`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/tests/test_templates.py` & `hatch_cython-0.6.0rc0/tests/test_templates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from hatch_cython.config.templates import parse_template_kwds
+from hatch_cython.config.templates import Templates, parse_template_kwds
 
 from .utils import arch_platform
 
 
 def test_templates():
     def test(kwds: dict):
         with arch_platform("x86_64", "darwin"):
@@ -38,7 +38,13 @@
             {"keyword": "templated_win", "matches": "*/templated*", "platforms": ["windows"]},
         ],
         "global": {"supported": ["int"]},
         "templated_mac": {"supported": ["int", "float"]},
         "templated_win": {"supported": ["int", "float", "complex"]},
     }
     test(form2)
+
+
+def test_defaults():
+    parsed = parse_template_kwds({})
+    assert parsed == Templates(index=[])
+    assert repr(parsed) == "Templates(index=[], kwargs={})"
```

### Comparing `hatch_cython-0.5.1/tests/test_xenv_merge.py` & `hatch_cython-0.6.0rc0/tests/test_xenv_merge.py`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/tests/utils.py` & `hatch_cython-0.6.0rc0/tests/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from contextlib import contextmanager
 from types import SimpleNamespace
 from unittest.mock import patch
 
+from hatch_cython.types import UnionT
+
 
 def true_if_eq(*vals):
     def inner(v: str, *extra):
         merge = [*vals, *extra]
         ok = any(v == val for val in merge)
         print(f"ok: {v} {ok} ", merge)  # noqa: T201
         return ok
@@ -30,29 +32,44 @@
         return h(path, *extra)
 
     with patch("hatch_cython.config.config.path.exists", wrap):
         yield
 
 
 @contextmanager
-def arch_platform(arch: str, platform: str):
+def patch_brew(prefix):
+    with patch("hatch_cython.config.defaults.brew_path", lambda: prefix):
+        yield
+
+
+@contextmanager
+def arch_platform(arch: str, platform: str, brew: UnionT[str, None] = True):
     def aarchgetter():
         return arch
 
     def platformgetter():
         return platform
 
+    expect_brew = None
+    if platform == "darwin":
+        expect_brew = "/usr/local" if arch == "x86_64" else "/opt/homebrew"
+
     try:
         with patch("hatch_cython.utils.plat", platformgetter):
-            with patch("hatch_cython.utils.plat", platformgetter):
+            with patch("hatch_cython.config.defaults.plat", platformgetter):
                 with patch("hatch_cython.config.platform.plat", platformgetter):
                     with patch("hatch_cython.plugin.plat", platformgetter):
                         with patch("hatch_cython.utils.aarch", aarchgetter):
-                            with patch("hatch_cython.config.platform.aarch", aarchgetter):
-                                yield
+                            with patch("hatch_cython.config.defaults.aarch", aarchgetter):
+                                with patch("hatch_cython.config.platform.aarch", aarchgetter):
+                                    if brew:
+                                        with patch_brew(expect_brew):
+                                            yield
+                                    else:
+                                        yield
     finally:
         print(f"Clean {arch}-{platform}")  # noqa: T201
         del aarchgetter, platformgetter
         pass
 
 
 @contextmanager
```

### Comparing `hatch_cython-0.5.1/LICENSE.txt` & `hatch_cython-0.6.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_cython-0.5.1/README.md` & `hatch_cython-0.6.0rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -97,29 +97,29 @@
     # ["ABC"] -> ["ABC", "FOO"] | ["ABC", "DEF"]
     ["NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION"],
 ]
 ```
 
 ## Configuration Options
 
-| Field                                                  | Type                                                                                                                                                                                                                                                                                                                                                                                                |
-| ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| src                                                    | `str \| None` <br/> directory within `src` dir or `.`  which aliases the package being built. e.g. `package_a` -> `src/package_a_lib` <br/> `src = "package_a"`                                                                                                                                                                                                                                     |
-| directives                                             | directives to cython (see [compiler-directives])                                                                                                                                                                                                                                                                                                                                                    |
-| compile_args                                           | str or `{ platforms = ["*"] \| "*", arg = str }`. see [extensions] for what args may be relevant                                                                                                                                                                                                                                                                                                    |
-| extra_link_args                                        | str or `{ platforms = ["*"] \| "*", arg = str }`. see [extensions] for what args may be relevant                                                                                                                                                                                                                                                                                                    |
-| env                                                    | `{ env = "VAR1", arg = "VALUE", platforms = ["*"], arch = ["*"] }`<br/> if flag is one of:<br/> - ARFLAGS<br/> - LDSHARED <br/> - LDFLAGS<br/> - CPPFLAGS <br/> - CFLAGS <br/> - CCSHARED<br/>the current env vars will be merged with the value (provided platform & arch applies), separated by a space. This can be enabled by adding `{ env = "MYVAR" ... , merges = true }` to the definition. |
-| includes                                               | list str                                                                                                                                                                                                                                                                                                                                                                                            |
-| include\_{package}                                     | `{ pkg = str, include = str, libraries = str\| None, library_dirs = str \| None , required_call = str \| None }` <br/>where all fields, but `pkg`, are attributes of `pkg` in the type of `callable() -> list[str] \| str` \| `list[str] \| str`. `pkg` is a module, or loadable module object, which may be imported through `import x.y.z`.                                                       |
-| include_numpy \| include_pyarrow \| include_pythran    | bool<br/>3rd party named imports. must have the respective opt in `dependencies`                                                                                                                                                                                                                                                                                                                    |
-| parallel                                               | bool = False <br/>if parallel, add openmp headers<br/>important: if using macos, you need the *homebrew* llvm vs _apple's_ llvm in order to pass `-fopenmp` to clang compiler                                                                                                                                                                                                                       |
-| compiler                                               | compiler used at build-time. if `msvc` (Microsoft Visual Studio), `/openmp` is used as argument to compile instead of `-fopenmp`  when `parallel = true`. `default = false`                                                                                                                                                                                                                         |
-| compile_py                                             | whether to include `.py` files when building cython exts. note, this can be enabled & you can do per file / matched file ignores as below. `default = true`                                                                                                                                                                                                                                         |
-| define_macros                                          | list of list str (of len 1 or 2). len 1 == [KEY] == `#define KEY FOO` . len 2 == [KEY, VALUE] == `#define KEY VALUE`. see [extensions]                                                                                                                                                                                                                                                              |
-| \*\* kwargs                                            | keyword = value pair arguments to pass to the extension module when building. see [extensions]                                                                                                                                                                                                                                                                                                      |
+| Field                                               | Type                                                                                                                                                                                                                                                                                                                                                                                                |
+| --------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| src                                                 | `str \| None` <br/> directory within `src` dir or `.`  which aliases the package being built. e.g. `package_a` -> `src/package_a_lib` <br/> `src = "package_a"`                                                                                                                                                                                                                                     |
+| directives                                          | directives to cython (see [compiler-directives])                                                                                                                                                                                                                                                                                                                                                    |
+| compile_args                                        | str or `{ platforms = ["*"] \| "*", arg = str }`. see [extensions] for what args may be relevant                                                                                                                                                                                                                                                                                                    |
+| extra_link_args                                     | str or `{ platforms = ["*"] \| "*", arg = str }`. see [extensions] for what args may be relevant                                                                                                                                                                                                                                                                                                    |
+| env                                                 | `{ env = "VAR1", arg = "VALUE", platforms = ["*"], arch = ["*"] }`<br/> if flag is one of:<br/> - ARFLAGS<br/> - LDSHARED <br/> - LDFLAGS<br/> - CPPFLAGS <br/> - CFLAGS <br/> - CCSHARED<br/>the current env vars will be merged with the value (provided platform & arch applies), separated by a space. This can be enabled by adding `{ env = "MYVAR" ... , merges = true }` to the definition. |
+| includes                                            | list str                                                                                                                                                                                                                                                                                                                                                                                            |
+| include\_{package}                                  | `{ pkg = str, include = str, libraries = str\| None, library_dirs = str \| None , required_call = str \| None }` <br/>where all fields, but `pkg`, are attributes of `pkg` in the type of `callable() -> list[str] \| str` \| `list[str] \| str`. `pkg` is a module, or loadable module object, which may be imported through `import x.y.z`.                                                       |
+| include_numpy \| include_pyarrow \| include_pythran | bool<br/>3rd party named imports. must have the respective opt in `dependencies`                                                                                                                                                                                                                                                                                                                    |
+| parallel                                            | bool = False <br/>if parallel, add openmp headers<br/>important: if using macos, you need the *homebrew* llvm vs _apple's_ llvm in order to pass `-fopenmp` to clang compiler                                                                                                                                                                                                                       |
+| compiler                                            | compiler used at build-time. if `msvc` (Microsoft Visual Studio), `/openmp` is used as argument to compile instead of `-fopenmp`  when `parallel = true`. `default = false`                                                                                                                                                                                                                         |
+| compile_py                                          | whether to include `.py` files when building cython exts. note, this can be enabled & you can do per file / matched file ignores as below. `default = true`                                                                                                                                                                                                                                         |
+| define_macros                                       | list of list str (of len 1 or 2). len 1 == [KEY] == `#define KEY FOO` . len 2 == [KEY, VALUE] == `#define KEY VALUE`. see [extensions]                                                                                                                                                                                                                                                              |
+| \*\* kwargs                                         | keyword = value pair arguments to pass to the extension module when building. see [extensions]                                                                                                                                                                                                                                                                                                      |
 
 ### Files
 
 ```toml
 [build.targets.wheel.hooks.cython.options.files]
 exclude = [
     # anything matching no_compile is ignored by cython
@@ -136,26 +136,41 @@
     { matches = "*/linux", platforms = ["darwin", "freebsd", "windows"] },
     # only freebsd
     { matches = "*/freebsd", platforms = ["linux", "darwin", "windows"] }
 ]
 aliases = {"abclib._filewithoutsuffix" = "abclib.importalias"}
 ```
 
+### Explicit Build Targets
+
+If explicit targets are required (i.e. `hatch-cython` _only_ builds the files specified), use `options.files.targets`. Specifying this option will implicly enable `compile_py`, in addition to checking all `c`, `cpp`, and `cc` files against the specified inclusions.
+
+```toml
+[build.targets.wheel.hooks.cython.options.files]
+targets = [
+  # using a single string
+  "*/compile.py",
+  # or a match clause
+  { matches = "*/windows", platforms = ["windows"] },
+  { matches = "*/posix", platforms = ["darwin", "freebsd", "linux"] },
+]
+```
+
 ## sdist
 
-Sdist archives may be generated normally. `hatch` must be defined as the `build-system` build-backend in your `pyproject.toml`. As such, hatch will automatically install `hatch-cython`, and perform the specified e.g. platform-specific adjustments to the compile-time arguments. This allows the full build-process to be respected, and generated following specifications of the developer._Note_: If you specify `hatch-cython` to run outside of simply wheel-step processes, the extension module is skipped. As such, the `.c` & `.cpp`, as well as templated files, may be generated and stored in the sdist should you wish. However, there is currently little purpose to this, as the extension will likely have differed compile arguments.
+Sdist archives may be generated normally. `hatch` must be defined as the `build-system` build-backend in `pyproject.toml`. As such, hatch will automatically install `hatch-cython`, and perform the specified e.g. platform-specific adjustments to the compile-time arguments. This allows the full build-process to be respected, and generated following specifications of the developer._Note_: If `hatch-cython` is specified to run outside of a wheel-step processes, the extension module is skipped. As such, the `.c` & `.cpp`, as well as templated files, may be generated and stored in the sdist should you wish. However, there is currently little purpose to this, as the extension will likely have differed compile arguments.
 
 ## Templating
 
 Cython tempita is supported for any files suffixed with `.in`, where the extension output is:
 
 - `.pyx.in`
 - `.pyd.in`
 - `.pyi.in`
-  For these files, you may expect the output `.pyx.in` -> `.pyx`. Thus, with aliasing this would look like:
+  For these files, expect the output `.pyx.in` -> `.pyx`. Thus, with aliasing this would look like:
 
 ```toml
 [build.targets.wheel.hooks.cython.options.files]
 aliases = {"abclib._somemod" = "abclib.somemod"}
 ```
 
 - 1. Source files `somemod.pyi.in`, `_somemod.pyx.in`
@@ -167,17 +182,17 @@
 - [pyi stub file](./test_libraries/src_structure/src/example_lib/templated.pyi.in)
 - [pyx cython source file](./test_libraries/src_structure/src/example_lib/templated.pyx.in)
 - [pyi stub (rendered)](./test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyi)
 - [pyx cython source (rendered)](./test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyi)
 
 ### Template Arguments
 
-You may also supply arguments for per-file matched namespaces. This follows the above `platforms`, `arch`, & `marker` formats, where if supplied & passing the condition the argument is passed to the template as a named series of keyword arguments.
+Per-file matched namespaces are supported for templating. This follows the above `platforms`, `arch`, & `marker` formats, where if supplied & passing the condition the argument is passed to the template as a named series of keyword arguments.
 
-You supply an `index` value, and all other kwargs to templates are `keywords` for each index value. Follows FIFO priority for all keys except global, which is evaluated first and overriden if there are other matching index directives. The engine will attempt to merge the items of the keywords, roughly following:
+If an `index` value is provided, and all other kwargs to templates are `keywords` for each index value. Follows FIFO priority for all keys except global, which is evaluated first and overriden if there are other matching index directives. The engine will attempt to merge the items of the keywords, roughly following:
 
 ```py
 args = {
     "index": [
         {"keyword": "global", ...},
         {"keyword": "thisenv", ...},
     ],
@@ -211,14 +226,26 @@
 
 templated_win = { supported = ["int", "float", "complex"] }
 
 # assuming numpy is cimported in the template
 templated_win_x86_64 = { supported = ["int", "float", "np.double"]}
 ```
 
+## Notes
+
+- MacOS users with brew installed will have `brew --prefix` libs and include paths added in compilation step. Code parsing is found [here](./src/hatch_cython/config/defaults.py#L11)
+- Github Runners now run MacOS on m1 platforms. You may have ci issues if you are using MacOS m1 runners and you do not disable `macos-max-compat` in hatch. e.g.
+
+  ```toml
+  # hatch.toml
+
+  [build.targets.wheel]
+  macos-max-compat = false
+  ```
+
 ## Development
 
 ### Requirements
 
 - a c / c++ compiler
 - python 3.8-<=3.12
 - [git-cliff] (`pip install git-cliff`)
```

### Comparing `hatch_cython-0.5.1/pyproject.toml` & `hatch_cython-0.6.0rc0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,21 @@
 target-version = ["py310"]
 
 [tool.coverage.paths]
 hatch_cython = ["src/hatch_cython", "*/hatch-cython/src/hatch_cython"]
 tests = ["tests", "*/hatch-cython/tests"]
 
 [tool.coverage.report]
-exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
+exclude_lines = [
+  "pragma: no cover",
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:"
+]
+skip_empty = true
 
 [tool.coverage.run]
 branch = true
 omit = ["src/hatch_cython/__about__.py", "src/hatch_cython/types.py"]
 parallel = true
 source_pkgs = ["hatch_cython"]
 
@@ -92,28 +98,32 @@
 style = ["ruff {args:.}", "black --check --diff {args:.}"]
 typing = "mypy --install-types --non-interactive {args:src/hatch_cython tests}"
 
 [tool.hatch.version]
 path = "src/hatch_cython/__about__.py"
 
 [tool.ruff]
+line-length = 120
+target-version = "py310"
+
+[tool.ruff.lint]
 ignore = [
   "B027",
   "FBT001",
+  "FBT002",
   "FBT003",
   "S105",
   "S106",
   "S107",
   "C901",
   "PLR0911",
   "PLR0912",
   "PLR0913",
   "PLR0915"
 ]
-line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -133,20 +143,19 @@
   "S",
   "T",
   "TID",
   "UP",
   "W",
   "YTT"
 ]
-target-version = "py310"
 unfixable = []
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["hatch_cython"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "**/__init__.py" = ["F401"]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
```

### Comparing `hatch_cython-0.5.1/PKG-INFO` & `hatch_cython-0.6.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hatch-cython
-Version: 0.5.1
+Version: 0.6.0rc0
 Summary: Cython build hooks for hatch
 Project-URL: Documentation, https://github.com/joshua-auchincloss/hatch-cython#readme
 Project-URL: Issues, https://github.com/joshua-auchincloss/hatch-cython/issues
 Project-URL: Source, https://github.com/joshua-auchincloss/hatch-cython
 Author-email: joshua-auchincloss <joshua.auchincloss@proton.me>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -134,29 +134,29 @@
     # ["ABC"] -> ["ABC", "FOO"] | ["ABC", "DEF"]
     ["NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION"],
 ]
 ```
 
 ## Configuration Options
 
-| Field                                                  | Type                                                                                                                                                                                                                                                                                                                                                                                                |
-| ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| src                                                    | `str \| None` <br/> directory within `src` dir or `.`  which aliases the package being built. e.g. `package_a` -> `src/package_a_lib` <br/> `src = "package_a"`                                                                                                                                                                                                                                     |
-| directives                                             | directives to cython (see [compiler-directives])                                                                                                                                                                                                                                                                                                                                                    |
-| compile_args                                           | str or `{ platforms = ["*"] \| "*", arg = str }`. see [extensions] for what args may be relevant                                                                                                                                                                                                                                                                                                    |
-| extra_link_args                                        | str or `{ platforms = ["*"] \| "*", arg = str }`. see [extensions] for what args may be relevant                                                                                                                                                                                                                                                                                                    |
-| env                                                    | `{ env = "VAR1", arg = "VALUE", platforms = ["*"], arch = ["*"] }`<br/> if flag is one of:<br/> - ARFLAGS<br/> - LDSHARED <br/> - LDFLAGS<br/> - CPPFLAGS <br/> - CFLAGS <br/> - CCSHARED<br/>the current env vars will be merged with the value (provided platform & arch applies), separated by a space. This can be enabled by adding `{ env = "MYVAR" ... , merges = true }` to the definition. |
-| includes                                               | list str                                                                                                                                                                                                                                                                                                                                                                                            |
-| include\_{package}                                     | `{ pkg = str, include = str, libraries = str\| None, library_dirs = str \| None , required_call = str \| None }` <br/>where all fields, but `pkg`, are attributes of `pkg` in the type of `callable() -> list[str] \| str` \| `list[str] \| str`. `pkg` is a module, or loadable module object, which may be imported through `import x.y.z`.                                                       |
-| include_numpy \| include_pyarrow \| include_pythran    | bool<br/>3rd party named imports. must have the respective opt in `dependencies`                                                                                                                                                                                                                                                                                                                    |
-| parallel                                               | bool = False <br/>if parallel, add openmp headers<br/>important: if using macos, you need the *homebrew* llvm vs _apple's_ llvm in order to pass `-fopenmp` to clang compiler                                                                                                                                                                                                                       |
-| compiler                                               | compiler used at build-time. if `msvc` (Microsoft Visual Studio), `/openmp` is used as argument to compile instead of `-fopenmp`  when `parallel = true`. `default = false`                                                                                                                                                                                                                         |
-| compile_py                                             | whether to include `.py` files when building cython exts. note, this can be enabled & you can do per file / matched file ignores as below. `default = true`                                                                                                                                                                                                                                         |
-| define_macros                                          | list of list str (of len 1 or 2). len 1 == [KEY] == `#define KEY FOO` . len 2 == [KEY, VALUE] == `#define KEY VALUE`. see [extensions]                                                                                                                                                                                                                                                              |
-| \*\* kwargs                                            | keyword = value pair arguments to pass to the extension module when building. see [extensions]                                                                                                                                                                                                                                                                                                      |
+| Field                                               | Type                                                                                                                                                                                                                                                                                                                                                                                                |
+| --------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| src                                                 | `str \| None` <br/> directory within `src` dir or `.`  which aliases the package being built. e.g. `package_a` -> `src/package_a_lib` <br/> `src = "package_a"`                                                                                                                                                                                                                                     |
+| directives                                          | directives to cython (see [compiler-directives])                                                                                                                                                                                                                                                                                                                                                    |
+| compile_args                                        | str or `{ platforms = ["*"] \| "*", arg = str }`. see [extensions] for what args may be relevant                                                                                                                                                                                                                                                                                                    |
+| extra_link_args                                     | str or `{ platforms = ["*"] \| "*", arg = str }`. see [extensions] for what args may be relevant                                                                                                                                                                                                                                                                                                    |
+| env                                                 | `{ env = "VAR1", arg = "VALUE", platforms = ["*"], arch = ["*"] }`<br/> if flag is one of:<br/> - ARFLAGS<br/> - LDSHARED <br/> - LDFLAGS<br/> - CPPFLAGS <br/> - CFLAGS <br/> - CCSHARED<br/>the current env vars will be merged with the value (provided platform & arch applies), separated by a space. This can be enabled by adding `{ env = "MYVAR" ... , merges = true }` to the definition. |
+| includes                                            | list str                                                                                                                                                                                                                                                                                                                                                                                            |
+| include\_{package}                                  | `{ pkg = str, include = str, libraries = str\| None, library_dirs = str \| None , required_call = str \| None }` <br/>where all fields, but `pkg`, are attributes of `pkg` in the type of `callable() -> list[str] \| str` \| `list[str] \| str`. `pkg` is a module, or loadable module object, which may be imported through `import x.y.z`.                                                       |
+| include_numpy \| include_pyarrow \| include_pythran | bool<br/>3rd party named imports. must have the respective opt in `dependencies`                                                                                                                                                                                                                                                                                                                    |
+| parallel                                            | bool = False <br/>if parallel, add openmp headers<br/>important: if using macos, you need the *homebrew* llvm vs _apple's_ llvm in order to pass `-fopenmp` to clang compiler                                                                                                                                                                                                                       |
+| compiler                                            | compiler used at build-time. if `msvc` (Microsoft Visual Studio), `/openmp` is used as argument to compile instead of `-fopenmp`  when `parallel = true`. `default = false`                                                                                                                                                                                                                         |
+| compile_py                                          | whether to include `.py` files when building cython exts. note, this can be enabled & you can do per file / matched file ignores as below. `default = true`                                                                                                                                                                                                                                         |
+| define_macros                                       | list of list str (of len 1 or 2). len 1 == [KEY] == `#define KEY FOO` . len 2 == [KEY, VALUE] == `#define KEY VALUE`. see [extensions]                                                                                                                                                                                                                                                              |
+| \*\* kwargs                                         | keyword = value pair arguments to pass to the extension module when building. see [extensions]                                                                                                                                                                                                                                                                                                      |
 
 ### Files
 
 ```toml
 [build.targets.wheel.hooks.cython.options.files]
 exclude = [
     # anything matching no_compile is ignored by cython
@@ -173,26 +173,41 @@
     { matches = "*/linux", platforms = ["darwin", "freebsd", "windows"] },
     # only freebsd
     { matches = "*/freebsd", platforms = ["linux", "darwin", "windows"] }
 ]
 aliases = {"abclib._filewithoutsuffix" = "abclib.importalias"}
 ```
 
+### Explicit Build Targets
+
+If explicit targets are required (i.e. `hatch-cython` _only_ builds the files specified), use `options.files.targets`. Specifying this option will implicly enable `compile_py`, in addition to checking all `c`, `cpp`, and `cc` files against the specified inclusions.
+
+```toml
+[build.targets.wheel.hooks.cython.options.files]
+targets = [
+  # using a single string
+  "*/compile.py",
+  # or a match clause
+  { matches = "*/windows", platforms = ["windows"] },
+  { matches = "*/posix", platforms = ["darwin", "freebsd", "linux"] },
+]
+```
+
 ## sdist
 
-Sdist archives may be generated normally. `hatch` must be defined as the `build-system` build-backend in your `pyproject.toml`. As such, hatch will automatically install `hatch-cython`, and perform the specified e.g. platform-specific adjustments to the compile-time arguments. This allows the full build-process to be respected, and generated following specifications of the developer._Note_: If you specify `hatch-cython` to run outside of simply wheel-step processes, the extension module is skipped. As such, the `.c` & `.cpp`, as well as templated files, may be generated and stored in the sdist should you wish. However, there is currently little purpose to this, as the extension will likely have differed compile arguments.
+Sdist archives may be generated normally. `hatch` must be defined as the `build-system` build-backend in `pyproject.toml`. As such, hatch will automatically install `hatch-cython`, and perform the specified e.g. platform-specific adjustments to the compile-time arguments. This allows the full build-process to be respected, and generated following specifications of the developer._Note_: If `hatch-cython` is specified to run outside of a wheel-step processes, the extension module is skipped. As such, the `.c` & `.cpp`, as well as templated files, may be generated and stored in the sdist should you wish. However, there is currently little purpose to this, as the extension will likely have differed compile arguments.
 
 ## Templating
 
 Cython tempita is supported for any files suffixed with `.in`, where the extension output is:
 
 - `.pyx.in`
 - `.pyd.in`
 - `.pyi.in`
-  For these files, you may expect the output `.pyx.in` -> `.pyx`. Thus, with aliasing this would look like:
+  For these files, expect the output `.pyx.in` -> `.pyx`. Thus, with aliasing this would look like:
 
 ```toml
 [build.targets.wheel.hooks.cython.options.files]
 aliases = {"abclib._somemod" = "abclib.somemod"}
 ```
 
 - 1. Source files `somemod.pyi.in`, `_somemod.pyx.in`
@@ -204,17 +219,17 @@
 - [pyi stub file](./test_libraries/src_structure/src/example_lib/templated.pyi.in)
 - [pyx cython source file](./test_libraries/src_structure/src/example_lib/templated.pyx.in)
 - [pyi stub (rendered)](./test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyi)
 - [pyx cython source (rendered)](./test_libraries/src_structure/src/example_lib/templated_maxosx_sample.pyi)
 
 ### Template Arguments
 
-You may also supply arguments for per-file matched namespaces. This follows the above `platforms`, `arch`, & `marker` formats, where if supplied & passing the condition the argument is passed to the template as a named series of keyword arguments.
+Per-file matched namespaces are supported for templating. This follows the above `platforms`, `arch`, & `marker` formats, where if supplied & passing the condition the argument is passed to the template as a named series of keyword arguments.
 
-You supply an `index` value, and all other kwargs to templates are `keywords` for each index value. Follows FIFO priority for all keys except global, which is evaluated first and overriden if there are other matching index directives. The engine will attempt to merge the items of the keywords, roughly following:
+If an `index` value is provided, and all other kwargs to templates are `keywords` for each index value. Follows FIFO priority for all keys except global, which is evaluated first and overriden if there are other matching index directives. The engine will attempt to merge the items of the keywords, roughly following:
 
 ```py
 args = {
     "index": [
         {"keyword": "global", ...},
         {"keyword": "thisenv", ...},
     ],
@@ -248,14 +263,26 @@
 
 templated_win = { supported = ["int", "float", "complex"] }
 
 # assuming numpy is cimported in the template
 templated_win_x86_64 = { supported = ["int", "float", "np.double"]}
 ```
 
+## Notes
+
+- MacOS users with brew installed will have `brew --prefix` libs and include paths added in compilation step. Code parsing is found [here](./src/hatch_cython/config/defaults.py#L11)
+- Github Runners now run MacOS on m1 platforms. You may have ci issues if you are using MacOS m1 runners and you do not disable `macos-max-compat` in hatch. e.g.
+
+  ```toml
+  # hatch.toml
+
+  [build.targets.wheel]
+  macos-max-compat = false
+  ```
+
 ## Development
 
 ### Requirements
 
 - a c / c++ compiler
 - python 3.8-<=3.12
 - [git-cliff] (`pip install git-cliff`)
```

