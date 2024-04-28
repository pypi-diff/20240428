# Comparing `tmp/cnrl_conex-0.1.3.tar.gz` & `tmp/cnrl_conex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnrl_conex-0.1.3.tar", last modified: Wed Apr 24 10:32:11 2024, max compression
+gzip compressed data, was "cnrl_conex-0.1.4.tar", last modified: Sun Apr 28 11:36:50 2024, max compression
```

## Comparing `cnrl_conex-0.1.3.tar` & `cnrl_conex-0.1.4.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.656105 cnrl_conex-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/AUTHORS.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.656105 cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-24 10:32:11.000000 cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-24 10:32:11.000000 cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:32:11.000000 cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:32:11.000000 cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 10:32:11.000000 cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 10:32:11.000000 cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-24 10:32:11.656105 cnrl_conex-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.648105 cnrl_conex-0.1.3/conex/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.648105 cnrl_conex-0.1.3/conex/behaviors/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.648105 cnrl_conex-0.1.3/conex/behaviors/layer/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/layer/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.648105 cnrl_conex-0.1.3/conex/behaviors/network/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/network/neuromodulators.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/network/payoff.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/network/time_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.648105 cnrl_conex-0.1.3/conex/behaviors/neurons/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/neurons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/neurons/axon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/neurons/dendrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/neurons/homeostasis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.648105 cnrl_conex-0.1.3/conex/behaviors/neurons/neuron_types/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/neurons/neuron_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/neurons/neuron_types/lif_neurons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/neurons/setters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/neurons/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.648105 cnrl_conex-0.1.3/conex/behaviors/synapses/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/synapses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16685 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/synapses/dendrites.py
--rw-r--r--   0 runner    (1001) docker     (127)    20844 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/synapses/learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/behaviors/synapses/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.648105 cnrl_conex-0.1.3/conex/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/priority.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.652105 cnrl_conex-0.1.3/conex/nn/structure/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/cortical_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/cortical_layer_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/io_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/neocortex.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/structure/synapsis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.652105 cnrl_conex-0.1.3/conex/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/conex/nn/utils/replication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.652105 cnrl_conex-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4928 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-24 10:32:11.656105 cnrl_conex-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.652105 cnrl_conex-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-24 10:32:04.000000 cnrl_conex-0.1.3/tests/test_CoNeX.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.301693 cnrl_conex-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/AUTHORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.301693 cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-28 11:36:50.000000 cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-28 11:36:50.000000 cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:36:50.000000 cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:36:50.000000 cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 11:36:50.000000 cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 11:36:50.000000 cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-28 11:36:50.301693 cnrl_conex-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.293693 cnrl_conex-0.1.4/conex/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.293693 cnrl_conex-0.1.4/conex/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.293693 cnrl_conex-0.1.4/conex/behaviors/layer/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/layer/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.293693 cnrl_conex-0.1.4/conex/behaviors/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/network/neuromodulators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/network/payoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/network/time_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.293693 cnrl_conex-0.1.4/conex/behaviors/neurons/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/neurons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/neurons/axon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/neurons/dendrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/neurons/homeostasis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.293693 cnrl_conex-0.1.4/conex/behaviors/neurons/neuron_types/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/neurons/neuron_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/neurons/neuron_types/lif_neurons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/neurons/setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/neurons/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.297693 cnrl_conex-0.1.4/conex/behaviors/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/synapses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16685 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/synapses/dendrites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20844 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/synapses/learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/behaviors/synapses/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.297693 cnrl_conex-0.1.4/conex/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/helpers/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/helpers/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.297693 cnrl_conex-0.1.4/conex/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/priority.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.297693 cnrl_conex-0.1.4/conex/nn/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/cortical_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/cortical_layer_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/io_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/neocortex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/structure/synapsis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.297693 cnrl_conex-0.1.4/conex/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/conex/nn/utils/replication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.301693 cnrl_conex-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4928 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-28 11:36:50.301693 cnrl_conex-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:36:50.301693 cnrl_conex-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-28 11:36:46.000000 cnrl_conex-0.1.4/tests/test_CoNeX.py
```

### Comparing `cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/PKG-INFO` & `cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNRL-CoNeX
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cortical Network for everything!
 Home-page: https://github.com/cnrl/CoNeX
 Author: CNRL
 Author-email: ashenatena@gmail.com
 License: MIT license
 Keywords: CNRL-CoNeX
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cnrl_conex-0.1.3/CNRL_CoNeX.egg-info/SOURCES.txt` & `cnrl_conex-0.1.4/CNRL_CoNeX.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 conex/behaviors/neurons/specs.py
 conex/behaviors/neurons/neuron_types/__init__.py
 conex/behaviors/neurons/neuron_types/lif_neurons.py
 conex/behaviors/synapses/__init__.py
 conex/behaviors/synapses/dendrites.py
 conex/behaviors/synapses/learning.py
 conex/behaviors/synapses/specs.py
+conex/helpers/__init__.py
+conex/helpers/data.py
+conex/helpers/filters.py
 conex/nn/__init__.py
 conex/nn/priority.py
 conex/nn/structure/__init__.py
 conex/nn/structure/container.py
 conex/nn/structure/cortical_column.py
 conex/nn/structure/cortical_layer_connection.py
 conex/nn/structure/io_layer.py
```

### Comparing `cnrl_conex-0.1.3/CONTRIBUTING.rst` & `cnrl_conex-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/LICENSE` & `cnrl_conex-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/PKG-INFO` & `cnrl_conex-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNRL-CoNeX
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cortical Network for everything!
 Home-page: https://github.com/cnrl/CoNeX
 Author: CNRL
 Author-email: ashenatena@gmail.com
 License: MIT license
 Keywords: CNRL-CoNeX
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cnrl_conex-0.1.3/conex/behaviors/layer/dataset.py` & `cnrl_conex-0.1.4/conex/behaviors/layer/dataset.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/network/neuromodulators.py` & `cnrl_conex-0.1.4/conex/behaviors/network/neuromodulators.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/network/payoff.py` & `cnrl_conex-0.1.4/conex/behaviors/network/payoff.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/network/time_resolution.py` & `cnrl_conex-0.1.4/conex/behaviors/network/time_resolution.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/neurons/axon.py` & `cnrl_conex-0.1.4/conex/behaviors/neurons/axon.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/neurons/dendrite.py` & `cnrl_conex-0.1.4/conex/behaviors/neurons/dendrite.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/neurons/homeostasis.py` & `cnrl_conex-0.1.4/conex/behaviors/neurons/homeostasis.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/neurons/neuron_types/lif_neurons.py` & `cnrl_conex-0.1.4/conex/behaviors/neurons/neuron_types/lif_neurons.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/neurons/setters.py` & `cnrl_conex-0.1.4/conex/behaviors/neurons/setters.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/neurons/specs.py` & `cnrl_conex-0.1.4/conex/behaviors/neurons/specs.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/synapses/dendrites.py` & `cnrl_conex-0.1.4/conex/behaviors/synapses/dendrites.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/synapses/learning.py` & `cnrl_conex-0.1.4/conex/behaviors/synapses/learning.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/behaviors/synapses/specs.py` & `cnrl_conex-0.1.4/conex/behaviors/synapses/specs.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/priority.py` & `cnrl_conex-0.1.4/conex/nn/priority.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/structure/container.py` & `cnrl_conex-0.1.4/conex/nn/structure/container.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/structure/cortical_column.py` & `cnrl_conex-0.1.4/conex/nn/structure/cortical_column.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/structure/cortical_layer_connection.py` & `cnrl_conex-0.1.4/conex/nn/structure/cortical_layer_connection.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/structure/io_layer.py` & `cnrl_conex-0.1.4/conex/nn/structure/io_layer.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/structure/layer.py` & `cnrl_conex-0.1.4/conex/nn/structure/layer.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/structure/neocortex.py` & `cnrl_conex-0.1.4/conex/nn/structure/neocortex.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/structure/port.py` & `cnrl_conex-0.1.4/conex/nn/structure/port.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/structure/synapsis.py` & `cnrl_conex-0.1.4/conex/nn/structure/synapsis.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/conex/nn/utils/replication.py` & `cnrl_conex-0.1.4/conex/nn/utils/replication.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/docs/Makefile` & `cnrl_conex-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/docs/conf.py` & `cnrl_conex-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/docs/installation.rst` & `cnrl_conex-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/docs/make.bat` & `cnrl_conex-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.3/setup.py` & `cnrl_conex-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,14 @@
     description="Cortical Network for everything!",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + "\n\n" + history,
     include_package_data=True,
     keywords="CNRL-CoNeX",
     name="CNRL-CoNeX",
-    packages=find_packages(include=['conex', 'conex.*']),
+    packages=find_packages(include=["conex", "conex.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cnrl/CoNeX",
-    version="0.1.3",
+    version="0.1.4",
     zip_safe=False,
 )
```

